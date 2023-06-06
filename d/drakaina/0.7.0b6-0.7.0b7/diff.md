# Comparing `tmp/drakaina-0.7.0b6.tar.gz` & `tmp/drakaina-0.7.0b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drakaina-0.7.0b6.tar", max compression
+gzip compressed data, was "drakaina-0.7.0b7.tar", max compression
```

## Comparing `drakaina-0.7.0b6.tar` & `drakaina-0.7.0b7.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     9270 2023-06-02 11:15:23.718906 drakaina-0.7.0b6/drakaina/__init__.py
--rw-r--r--   0        0        0        0 2023-01-24 15:15:01.981448 drakaina-0.7.0b6/drakaina/contrib/__init__.py
--rw-r--r--   0        0        0     1225 2023-04-04 16:39:30.455695 drakaina-0.7.0b6/drakaina/contrib/django/__init__.py
--rw-r--r--   0        0        0     6267 2023-06-01 12:00:05.542467 drakaina-0.7.0b6/drakaina/contrib/django/middleware.py
--rw-r--r--   0        0        0     3532 2023-04-20 14:07:49.356702 drakaina-0.7.0b6/drakaina/contrib/django/views.py
--rw-r--r--   0        0        0      402 2023-04-07 16:25:48.140700 drakaina-0.7.0b6/drakaina/contrib/jwt/__init__.py
--rw-r--r--   0        0        0      348 2023-03-10 11:02:10.213372 drakaina-0.7.0b6/drakaina/contrib/jwt/errors.py
--rw-r--r--   0        0        0     8847 2023-06-02 11:15:23.719893 drakaina-0.7.0b6/drakaina/contrib/jwt/middleware.py
--rw-r--r--   0        0        0      911 2023-05-29 22:21:28.708378 drakaina-0.7.0b6/drakaina/contrib/jwt/types.py
--rw-r--r--   0        0        0    18201 2023-06-02 11:15:23.720890 drakaina-0.7.0b6/drakaina/contrib/jwt/utils.py
--rw-r--r--   0        0        0     1327 2023-05-11 09:46:59.367413 drakaina-0.7.0b6/drakaina/exceptions.py
--rw-r--r--   0        0        0      357 2023-04-04 11:19:41.564726 drakaina-0.7.0b6/drakaina/middleware/__init__.py
--rw-r--r--   0        0        0     1370 2023-05-29 22:21:28.722375 drakaina-0.7.0b6/drakaina/middleware/base.py
--rw-r--r--   0        0        0     7364 2023-06-02 11:15:23.721960 drakaina-0.7.0b6/drakaina/middleware/cors.py
--rw-r--r--   0        0        0     1967 2023-06-02 11:15:23.721960 drakaina-0.7.0b6/drakaina/middleware/exception.py
--rw-r--r--   0        0        0     1072 2023-05-29 22:42:27.401282 drakaina-0.7.0b6/drakaina/middleware/request_wrapper.py
--rw-r--r--   0        0        0    12337 2023-06-02 11:15:23.722960 drakaina-0.7.0b6/drakaina/registries.py
--rw-r--r--   0        0        0      155 2023-03-02 17:41:49.563857 drakaina-0.7.0b6/drakaina/rpc_protocols/__init__.py
--rw-r--r--   0        0        0     7317 2023-06-02 11:15:23.722960 drakaina-0.7.0b6/drakaina/rpc_protocols/base.py
--rw-r--r--   0        0        0    13954 2023-06-02 11:15:23.723959 drakaina-0.7.0b6/drakaina/rpc_protocols/jsonrpc20.py
--rw-r--r--   0        0        0     4643 2023-05-12 10:10:59.326403 drakaina-0.7.0b6/drakaina/serializers.py
--rw-r--r--   0        0        0    30834 2023-06-02 11:15:23.724958 drakaina-0.7.0b6/drakaina/types.py
--rw-r--r--   0        0        0     3625 2023-06-02 11:15:23.725965 drakaina-0.7.0b6/drakaina/utils.py
--rw-r--r--   0        0        0     8212 2023-06-02 11:15:23.726959 drakaina-0.7.0b6/drakaina/wsgi.py
--rw-r--r--   0        0        0    11372 2023-01-24 23:31:45.206801 drakaina-0.7.0b6/LICENSE
--rw-r--r--   0        0        0     2672 2023-06-02 10:50:25.172544 drakaina-0.7.0b6/pyproject.toml
--rw-r--r--   0        0        0     5366 2023-06-02 11:15:23.718906 drakaina-0.7.0b6/README.md
--rw-r--r--   0        0        0     7010 1970-01-01 00:00:00.000000 drakaina-0.7.0b6/PKG-INFO
+-rw-r--r--   0        0        0     9020 2023-06-06 11:46:13.593707 drakaina-0.7.0b7/drakaina/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-24 15:15:01.981448 drakaina-0.7.0b7/drakaina/contrib/__init__.py
+-rw-r--r--   0        0        0     1225 2023-04-04 16:39:30.455695 drakaina-0.7.0b7/drakaina/contrib/django/__init__.py
+-rw-r--r--   0        0        0     6410 2023-06-06 11:38:21.333031 drakaina-0.7.0b7/drakaina/contrib/django/middleware.py
+-rw-r--r--   0        0        0     3532 2023-04-20 14:07:49.356702 drakaina-0.7.0b7/drakaina/contrib/django/views.py
+-rw-r--r--   0        0        0      402 2023-04-07 16:25:48.140700 drakaina-0.7.0b7/drakaina/contrib/jwt/__init__.py
+-rw-r--r--   0        0        0      348 2023-03-10 11:02:10.213372 drakaina-0.7.0b7/drakaina/contrib/jwt/errors.py
+-rw-r--r--   0        0        0     8847 2023-06-06 11:46:13.593707 drakaina-0.7.0b7/drakaina/contrib/jwt/middleware.py
+-rw-r--r--   0        0        0      911 2023-05-29 22:21:28.708378 drakaina-0.7.0b7/drakaina/contrib/jwt/types.py
+-rw-r--r--   0        0        0    18201 2023-06-06 11:46:13.594707 drakaina-0.7.0b7/drakaina/contrib/jwt/utils.py
+-rw-r--r--   0        0        0     1490 2023-06-02 16:00:38.817771 drakaina-0.7.0b7/drakaina/exceptions.py
+-rw-r--r--   0        0        0      357 2023-04-04 11:19:41.564726 drakaina-0.7.0b7/drakaina/middleware/__init__.py
+-rw-r--r--   0        0        0     1370 2023-05-29 22:21:28.722375 drakaina-0.7.0b7/drakaina/middleware/base.py
+-rw-r--r--   0        0        0     7364 2023-06-06 11:46:13.594707 drakaina-0.7.0b7/drakaina/middleware/cors.py
+-rw-r--r--   0        0        0     1967 2023-06-06 11:46:13.594707 drakaina-0.7.0b7/drakaina/middleware/exception.py
+-rw-r--r--   0        0        0     1072 2023-05-29 22:42:27.401282 drakaina-0.7.0b7/drakaina/middleware/request_wrapper.py
+-rw-r--r--   0        0        0    12337 2023-06-06 11:46:13.595708 drakaina-0.7.0b7/drakaina/registries.py
+-rw-r--r--   0        0        0      155 2023-03-02 17:41:49.563857 drakaina-0.7.0b7/drakaina/rpc_protocols/__init__.py
+-rw-r--r--   0        0        0     7317 2023-06-06 11:46:13.595708 drakaina-0.7.0b7/drakaina/rpc_protocols/base.py
+-rw-r--r--   0        0        0    13954 2023-06-06 11:46:13.595708 drakaina-0.7.0b7/drakaina/rpc_protocols/jsonrpc20.py
+-rw-r--r--   0        0        0     4643 2023-05-12 10:10:59.326403 drakaina-0.7.0b7/drakaina/serializers.py
+-rw-r--r--   0        0        0    30828 2023-06-06 11:46:13.596708 drakaina-0.7.0b7/drakaina/types.py
+-rw-r--r--   0        0        0     3627 2023-06-06 11:46:13.596708 drakaina-0.7.0b7/drakaina/utils.py
+-rw-r--r--   0        0        0     8212 2023-06-06 11:46:13.597709 drakaina-0.7.0b7/drakaina/wsgi.py
+-rw-r--r--   0        0        0    11372 2023-01-24 23:31:45.206801 drakaina-0.7.0b7/LICENSE
+-rw-r--r--   0        0        0     2710 2023-06-06 11:39:11.129309 drakaina-0.7.0b7/pyproject.toml
+-rw-r--r--   0        0        0     5366 2023-06-06 11:46:13.593707 drakaina-0.7.0b7/README.md
+-rw-r--r--   0        0        0     6888 1970-01-01 00:00:00.000000 drakaina-0.7.0b7/PKG-INFO
```

### Comparing `drakaina-0.7.0b6/drakaina/__init__.py` & `drakaina-0.7.0b7/drakaina/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from __future__ import annotations
 
 from asyncio import iscoroutinefunction
 from functools import update_wrapper
 from typing import Any
 from typing import Callable
 from typing import Iterable
-from typing import MutableMapping
+from typing import Mapping
 from typing import Optional
 from typing import TypeVar
 
-from drakaina.exceptions import AuthenticationFailedError
 from drakaina.exceptions import ForbiddenError
 from drakaina.registries import RPC_REGISTRY
 from drakaina.registries import RPCRegistry
 from drakaina.types import AnyRequest
 from drakaina.types import Comparator
 from drakaina.utils import iterable_str_arg
 
@@ -187,31 +186,34 @@
     if len(_args) > 0:
         if callable(_args[0]):
             return __decorator(_args[0])
         else:
             raise TypeError("Expected first argument to be a callable")
 
     def decorator(procedure):
-        assert callable(procedure)
+        if not callable(procedure):
+            raise TypeError("Expected first argument to be a callable")
         return __decorator(procedure)
 
     return decorator
 
 
-def match_any(required: Iterable[str], provided: str | Iterable[str]) -> bool:
+def match_any(required: Iterable[str], provided: Iterable[str]) -> bool:
+    if not (bool(required) or bool(provided)):  # If both are empty
+        return True
     return any((scope in provided for scope in required))
 
 
-def match_all(required: Iterable[str], provided: str | Iterable[str]) -> bool:
+def match_all(required: Iterable[str], provided: Iterable[str]) -> bool:
     return set(required).issubset(set(provided))
 
 
 def check_permissions(
     scopes: str | Iterable[str],
-    comparator: Comparator = match_all,
+    comparator: Comparator = match_any,
 ) -> Callable:
     """Permission decorator.
 
     Gives access to the procedure only to authorized users.
 
     """
     if not (
@@ -223,15 +225,15 @@
     ):
         raise TypeError(
             "The `scopes` argument must be a string or Iterable[string]",
         )
     if not callable(comparator):
         raise TypeError(
             "The `comparator` argument must be a function that implements "
-            "the Comparator interface",
+            "the `types.Comparator` interface",
         )
 
     procedure_scopes = iterable_str_arg(scopes)
 
     def __decorator(procedure: T) -> T:
         registry: RPCRegistry = getattr(procedure, RPC_REGISTRY, None)
         if registry is None:
@@ -245,38 +247,28 @@
             async def wrapper(*args, **kwargs):
                 request = _get_request(*args, **kwargs)  # noqa
 
                 if not _is_authenticated(request):
                     raise ForbiddenError("Authentication required")
 
                 user_scopes = _get_scopes(request)
-                if not isinstance(user_scopes, Iterable):
-                    raise AuthenticationFailedError(
-                        "Invalid permissions format",
-                    )
-
                 if not comparator(procedure_scopes, user_scopes):
                     raise ForbiddenError("Forbidden")
 
                 return await procedure(*args, **kwargs)
 
         else:
 
             def wrapper(*args, **kwargs):
                 request = _get_request(*args, **kwargs)  # noqa
 
                 if not _is_authenticated(request):
                     raise ForbiddenError("Authentication required")
 
                 user_scopes = _get_scopes(request)
-                if not isinstance(user_scopes, Iterable):
-                    raise AuthenticationFailedError(
-                        "Invalid permissions format",
-                    )
-
                 if not comparator(procedure_scopes, user_scopes):
                     raise ForbiddenError("Forbidden")
 
                 return procedure(*args, **kwargs)
 
         wrapper = update_wrapper(wrapper, procedure)
         registry.replace(procedure, wrapper)
@@ -289,20 +281,21 @@
     if len(args) == 0:
         return kwargs.get("request")
     else:
         return args[0]
 
 
 def _is_authenticated(request: AnyRequest) -> bool:
-    if isinstance(request, (dict, MutableMapping)):
+    if isinstance(request, (dict, Mapping)):
         return request.get(ENV_IS_AUTHENTICATED, False)
     else:
         return getattr(request, ENV_IS_AUTHENTICATED, False)
 
 
-def _get_scopes(request: AnyRequest) -> Optional[Iterable[str]]:
-    if isinstance(request, (dict, MutableMapping)):
+def _get_scopes(request: AnyRequest) -> Iterable[str]:
+    if isinstance(request, (dict, Mapping)) or hasattr(request, "get"):
         scopes = request.get(ENV_AUTH_SCOPES, None)
     else:
         scopes = getattr(request, ENV_AUTH_SCOPES, None)
-    if scopes is not None:
+    if isinstance(scopes, (str, Iterable)):
         return iterable_str_arg(scopes)
+    return ()
```

### Comparing `drakaina-0.7.0b6/drakaina/contrib/django/__init__.py` & `drakaina-0.7.0b7/drakaina/contrib/django/__init__.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b6/drakaina/contrib/django/middleware.py` & `drakaina-0.7.0b7/drakaina/contrib/django/middleware.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,23 +103,26 @@
 
         if not token and self.credentials_required:
             return self._error_response(
                 AuthenticationFailedError("Credential required"),
             )
 
         if token is not None:
-            payload = decode_jwt_token(
-                token,
-                algorithms=self.algorithms,
-                verify_key=self.__verify_key,
-                verify=True,
-                decode_options=self.decode_options,
-                verify_values=self.verify_values,
-                leeway=self.leeway,
-            )
+            try:
+                payload = decode_jwt_token(
+                    token,
+                    algorithms=self.algorithms,
+                    verify_key=self.__verify_key,
+                    verify=True,
+                    decode_options=self.decode_options,
+                    verify_values=self.verify_values,
+                    leeway=self.leeway,
+                )
+            except Exception as error:
+                return self._error_response(error)
 
             if callable(self.token_is_revoked):
                 if self.token_is_revoked(request, payload):
                     return self._error_response(
                         ForbiddenError("Token is revoked"),
                     )
```

### Comparing `drakaina-0.7.0b6/drakaina/contrib/django/views.py` & `drakaina-0.7.0b7/drakaina/contrib/django/views.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b6/drakaina/contrib/jwt/middleware.py` & `drakaina-0.7.0b7/drakaina/contrib/jwt/middleware.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b6/drakaina/contrib/jwt/types.py` & `drakaina-0.7.0b7/drakaina/contrib/jwt/types.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b6/drakaina/contrib/jwt/utils.py` & `drakaina-0.7.0b7/drakaina/contrib/jwt/utils.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b6/drakaina/exceptions.py` & `drakaina-0.7.0b7/drakaina/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,18 +8,22 @@
 
     def __init__(self, *args):
         super().__init__(*args)
         if len(args) > 0:
             self.message = str(args[0])
 
     def __str__(self) -> str:
-        return f"{self.__class__.__name__} ({self.message})"
+        if self.message:
+            return f"{self.__class__.__name__} ({self.message})"
+        return f"{self.__class__.__name__}"
 
     def __repr__(self) -> str:
-        return f"<{self.__class__.__name__} ({self.message})>"
+        if self.message:
+            return f"<{self.__class__.__name__} ({self.message})>"
+        return f"<{self.__class__.__name__}>"
 
     def as_dict(self) -> dict[str, str]:
         return {
             "error": self.__class__.__name__,
             "message": self.message or "",
         }
 
@@ -28,23 +32,27 @@
     """Serialization error"""
 
 
 class DeserializationError(RPCError):
     """Deserialization error"""
 
 
+class InternalServerError(RPCError):
+    """Server error"""
+
+
 class BadRequestError(RPCError):
     """Bad request error"""
 
 
-class NotFoundError(RPCError):
+class NotFoundError(BadRequestError):
     """Not found error"""
 
 
-class InvalidParametersError(RPCError):
+class InvalidParametersError(BadRequestError):
     """Invalid parameters error"""
 
 
 class AuthenticationFailedError(RPCError):
     """Authentication failed"""
 
 
@@ -52,13 +60,9 @@
     """Invalid token error"""
 
 
 class ForbiddenError(AuthenticationFailedError):
     """Forbidden error"""
 
 
-class InvalidPermissionsError(ForbiddenError):
+class InvalidPermissionsError(BadRequestError):
     """Invalid permissions error"""
-
-
-class InternalServerError(RPCError):
-    """Server error"""
```

### Comparing `drakaina-0.7.0b6/drakaina/middleware/base.py` & `drakaina-0.7.0b7/drakaina/middleware/base.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b6/drakaina/middleware/cors.py` & `drakaina-0.7.0b7/drakaina/middleware/cors.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b6/drakaina/middleware/exception.py` & `drakaina-0.7.0b7/drakaina/middleware/exception.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b6/drakaina/middleware/request_wrapper.py` & `drakaina-0.7.0b7/drakaina/middleware/request_wrapper.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b6/drakaina/registries.py` & `drakaina-0.7.0b7/drakaina/registries.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b6/drakaina/rpc_protocols/base.py` & `drakaina-0.7.0b7/drakaina/rpc_protocols/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,15 @@
             "You must implement the `handle` method in the child class",
         )
 
     def handle_error(
         self,
         error: RPCError | Type[RPCError] | Exception | Type[Exception],
     ) -> RPCError:
-        """Returns an exception object corresponding to the ROC protocol.
+        """Returns an exception object corresponding to the RPC protocol.
 
         :param error:
             The instance or class of the error.
         :type error: RPCError | Type[RPCError] | Exception | Type[Exception]
         :returns: Protocol specific error object.
         :rtype: RPCError
```

### Comparing `drakaina-0.7.0b6/drakaina/rpc_protocols/jsonrpc20.py` & `drakaina-0.7.0b7/drakaina/rpc_protocols/jsonrpc20.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b6/drakaina/serializers.py` & `drakaina-0.7.0b7/drakaina/serializers.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b6/drakaina/types.py` & `drakaina-0.7.0b7/drakaina/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1028,15 +1028,15 @@
 """
 
 
 class Comparator(Protocol):
     def __call__(
         self,
         required: Iterable[str],
-        provided: str | Iterable[str],
+        provided: Iterable[str],
     ) -> bool:
         ...
 
 
 class ProxyRequest(MutableMapping):
     """A wrapper class for environment mapping.
```

### Comparing `drakaina-0.7.0b6/drakaina/utils.py` & `drakaina-0.7.0b7/drakaina/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 from datetime import timedelta
 from functools import partial
 from typing import Callable
 from typing import Iterable
 from typing import Literal
 
 
-def iterable_str_arg(s: str | Iterable[str]) -> list[str]:
+def iterable_str_arg(s: str | Iterable[str]) -> tuple[str]:
     if isinstance(s, str):
         s = s.replace(",", " ").strip().replace("  ", " ").split()
-    return list(map(str, s))
+    return tuple(map(str, s))
 
 
 def unwrap_func(func: Callable) -> Callable:
     _func = func
     while hasattr(_func, "__wrapped__") or isinstance(_func, partial):
         _func = getattr(_func, "__wrapped__", None) or _func.func
     return _func
```

### Comparing `drakaina-0.7.0b6/drakaina/wsgi.py` & `drakaina-0.7.0b7/drakaina/wsgi.py`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b6/LICENSE` & `drakaina-0.7.0b7/LICENSE`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b6/pyproject.toml` & `drakaina-0.7.0b7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drakaina"
-version = "0.7.0-beta.6"
+version = "0.7.0-beta.7"
 description = "Module for simple RPC service implementation"
 authors = ["Aleksey Terentyev <terentyev.a@pm.me>"]
 license = "Apache License 2.0"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Web Environment",
@@ -34,36 +34,42 @@
 
 [tool.poetry.extras]
 jwt = ["PyJWT"]
 ujson = ["ujson"]
 orjson = ["orjson"]
 msgpack = ["msgpack"]
 docs = ["docstring-parser"]
-tests = ["pytest", "httpx", "ujson", "orjson", "msgpack", "pyjwt", "django", "docstring-parser"]
+
+[tool.poetry.group.dev]
+optional = true
 
 [tool.poetry.group.dev.dependencies]
 black = {extras = ["d"], version = "^22.12.0"}
 pre-commit = "^3.3.2"
 ruff = "^0.0.269"
 msgpack = "^1.0.4"
 orjson = "^3.8.6"
 pytest = "^7.3.1"
 ujson = "^5.7.0"
 pyjwt = "^2.7.0"
 django = ">=3.2"
 
-[tool.poetry.group.tests.dependencies]
+[tool.poetry.group.test]
+optional = true
+
+[tool.poetry.group.test.dependencies]
 pytest = "^7.2.1"
+pytest-asyncio = "^0.21.0"
 pytest-cov = "^4.1.0"
 httpx = "^0.23.3"
 
 [tool.pytest.ini_options]
 cache_dir = ".pytest_cache"
 testpaths = "tests"
-addopts = "-vl --cov=drakaina --tb=auto --capture=sys"
+addopts = "-vl --cov=drakaina --cov-report term-missing --tb=auto --capture=sys"
 
 [tool.ruff]
 # Enable Pyflakes `E` and `F` codes by default.
 select = ["E", "F"]
 ignore = []
 
 # Allow autofix for all enabled rules (when `--fix`) is provided.
```

### Comparing `drakaina-0.7.0b6/README.md` & `drakaina-0.7.0b7/README.md`

 * *Files identical despite different names*

### Comparing `drakaina-0.7.0b6/PKG-INFO` & `drakaina-0.7.0b7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drakaina
-Version: 0.7.0b6
+Version: 0.7.0b7
 Summary: Module for simple RPC service implementation
 Home-page: https://gitlab.com/tau_lex/drakaina
 License: Apache-2.0
 Keywords: rpc,jsonrpc,openrpc
 Author: Aleksey Terentyev
 Author-email: terentyev.a@pm.me
 Requires-Python: >=3.8,<4.0
@@ -21,22 +21,21 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Networking
 Provides-Extra: docs
 Provides-Extra: jwt
 Provides-Extra: msgpack
 Provides-Extra: orjson
-Provides-Extra: tests
 Provides-Extra: ujson
-Requires-Dist: docstring-parser (>=0.15,<0.16) ; extra == "docs" or extra == "tests"
-Requires-Dist: msgpack (>=1.0.5,<2.0.0) ; extra == "msgpack" or extra == "tests"
-Requires-Dist: orjson (>=3.8.14,<4.0.0) ; extra == "orjson" or extra == "tests"
-Requires-Dist: pyjwt (>=2.7.0,<3.0.0) ; extra == "jwt" or extra == "tests"
+Requires-Dist: docstring-parser (>=0.15,<0.16) ; extra == "docs"
+Requires-Dist: msgpack (>=1.0.5,<2.0.0) ; extra == "msgpack"
+Requires-Dist: orjson (>=3.8.14,<4.0.0) ; extra == "orjson"
+Requires-Dist: pyjwt (>=2.7.0,<3.0.0) ; extra == "jwt"
 Requires-Dist: typing-extensions (>=4.6.2,<5.0.0)
-Requires-Dist: ujson (>=5.7.0,<6.0.0) ; extra == "ujson" or extra == "tests"
+Requires-Dist: ujson (>=5.7.0,<6.0.0) ; extra == "ujson"
 Project-URL: Repository, https://gitlab.com/tau_lex/drakaina
 Description-Content-Type: text/markdown
 
 # drakaina
 
 ![Drakaina](content/drakaina.png "Drakaina"){width=200px height=205px}
```

