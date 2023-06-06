# Comparing `tmp/mlflow_oidc_client-0.2.3.tar.gz` & `tmp/mlflow_oidc_client-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlflow_oidc_client-0.2.3.tar", max compression
+gzip compressed data, was "mlflow_oidc_client-0.2.4.tar", max compression
```

## Comparing `mlflow_oidc_client-0.2.3.tar` & `mlflow_oidc_client-0.2.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1085 2023-04-27 14:59:27.607743 mlflow_oidc_client-0.2.3/LICENSE.md
--rw-r--r--   0        0        0     3638 2023-04-27 14:59:27.607743 mlflow_oidc_client-0.2.3/README.md
--rw-r--r--   0        0        0       76 2023-04-27 14:59:27.607743 mlflow_oidc_client-0.2.3/mlflow_oidc_client/__init__.py
--rw-r--r--   0        0        0     3187 2023-04-27 14:59:27.607743 mlflow_oidc_client-0.2.3/mlflow_oidc_client/config.py
--rw-r--r--   0        0        0     4758 2023-04-27 14:59:27.608743 mlflow_oidc_client-0.2.3/mlflow_oidc_client/oidc_session.py
--rw-r--r--   0        0        0     1352 2023-04-27 14:59:27.608743 mlflow_oidc_client-0.2.3/mlflow_oidc_client/request_header_provider.py
--rw-r--r--   0        0        0     1407 2023-04-27 14:59:27.609743 mlflow_oidc_client-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     4610 1970-01-01 00:00:00.000000 mlflow_oidc_client-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-06-06 13:47:25.890180 mlflow_oidc_client-0.2.4/LICENSE.md
+-rw-r--r--   0        0        0     3638 2023-06-06 13:47:25.890180 mlflow_oidc_client-0.2.4/README.md
+-rw-r--r--   0        0        0       76 2023-06-06 13:47:25.890180 mlflow_oidc_client-0.2.4/mlflow_oidc_client/__init__.py
+-rw-r--r--   0        0        0     3187 2023-06-06 13:47:25.890180 mlflow_oidc_client-0.2.4/mlflow_oidc_client/config.py
+-rw-r--r--   0        0        0     4977 2023-06-06 13:47:25.890180 mlflow_oidc_client-0.2.4/mlflow_oidc_client/oidc_session.py
+-rw-r--r--   0        0        0     1352 2023-06-06 13:47:25.890180 mlflow_oidc_client-0.2.4/mlflow_oidc_client/request_header_provider.py
+-rw-r--r--   0        0        0     1407 2023-06-06 13:47:25.891180 mlflow_oidc_client-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     4508 1970-01-01 00:00:00.000000 mlflow_oidc_client-0.2.4/PKG-INFO
```

### Comparing `mlflow_oidc_client-0.2.3/LICENSE.md` & `mlflow_oidc_client-0.2.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_client-0.2.3/README.md` & `mlflow_oidc_client-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_client-0.2.3/mlflow_oidc_client/config.py` & `mlflow_oidc_client-0.2.4/mlflow_oidc_client/config.py`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_client-0.2.3/mlflow_oidc_client/oidc_session.py` & `mlflow_oidc_client-0.2.4/mlflow_oidc_client/oidc_session.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+import threading
 from dataclasses import asdict, replace
 from datetime import datetime, timezone
 from pathlib import Path
 from typing import Type
 
 import jwt
 from oidc_client import AuthorizationError, TokenResponse, fetch_provider_config, login
@@ -15,23 +16,30 @@
     from typing_extensions import Self
 
 DEFAULT_CACHE_PATH = Path.home() / ".mlflow" / "oidc_client" / "cache"
 
 JWT_CLAIM_EXPIRY = "exp"
 JWT_OPTION_VERIFY_SIGNATURE = "verify_signature"
 
+# Global session lock
+lock = threading.Lock()
+
 
 class OIDCSessionError(RuntimeError):
     """Raised when the OAuth 2.1 authorization flow fails."""
 
     pass
 
 
 class OIDCSession:
-    """Authentication session, caching proxy for OIDC Client's TokenResponse."""
+    """Authentication session, caching proxy for OIDC Client's TokenResponse.
+
+    Note: only a single active session is allowed globally, even if MLflow uses
+    multiple threads.
+    """
 
     def __init__(
         self,
         issuer: str,
         client_id: str,
         client_secret: str | None = None,
         redirect_uri: str = DEFAULT_REDIRECT_URI,
@@ -46,28 +54,31 @@
         self.client_secret = client_secret
         self.redirect_uri = redirect_uri
         self.audience = audience
         self.scope = scope
         self.interactive = interactive
 
         self._cache_file = cache_path / f"{client_id}.json"
+
+        lock.acquire()
         try:
             with self._cache_file.open() as fd:
                 self._cache = TokenResponse(**json.loads(fd.read()))
         except (TypeError, FileNotFoundError, json.JSONDecodeError):
             self.refresh_cache()
 
     def close(self) -> None:
         """Close the session and write cache to file."""
         self._cache_file.parent.mkdir(parents=True, exist_ok=True)
 
         with self._cache_file.open("w") as fd:
             fd.write(json.dumps(asdict(self._cache)))
 
         self._cache_file.chmod(0o600)
+        lock.release()
 
     def refresh_cache(self) -> None:
         """Refresh the cached TokenResponse from the OAuth/OIDC authorization server."""
         try:
             self._cache = login(
                 fetch_provider_config(self.issuer),
                 client_id=self.client_id,
```

### Comparing `mlflow_oidc_client-0.2.3/mlflow_oidc_client/request_header_provider.py` & `mlflow_oidc_client-0.2.4/mlflow_oidc_client/request_header_provider.py`

 * *Files identical despite different names*

### Comparing `mlflow_oidc_client-0.2.3/pyproject.toml` & `mlflow_oidc_client-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlflow-oidc-client"
-version = "0.2.3"
+version = "0.2.4"
 description = "MLflow plugin adding OIDC/OAuth 2.1 client authorization"
 authors = ["Loris Zinsou <lzinsou@protonmail.com>"]
 readme = "README.md"
 keywords = ["mlflow", "plugin", "mlops", "oidc", "oauth", "oauth2"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Plugins",
```

### Comparing `mlflow_oidc_client-0.2.3/PKG-INFO` & `mlflow_oidc_client-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: mlflow-oidc-client
-Version: 0.2.3
+Version: 0.2.4
 Summary: MLflow plugin adding OIDC/OAuth 2.1 client authorization
 Home-page: https://gitlab.com/lzinsou/mlflow-oidc-client
 Keywords: mlflow,plugin,mlops,oidc,oauth,oauth2
 Author: Loris Zinsou
 Author-email: lzinsou@protonmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Plugins
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: oidc-client (>=0.2.3,<0.3.0)
 Requires-Dist: pyjwt (>=2,<3)
 Requires-Dist: toml (>=0.10.2,<0.11.0) ; python_version < "3.11"
 Requires-Dist: typing-extensions (>=4.0.1) ; python_version < "3.11"
 Project-URL: Repository, https://gitlab.com/lzinsou/mlflow-oidc-client
 Description-Content-Type: text/markdown
```

