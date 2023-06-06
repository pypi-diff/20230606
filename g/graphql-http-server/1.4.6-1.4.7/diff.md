# Comparing `tmp/graphql_http_server-1.4.6.tar.gz` & `tmp/graphql_http_server-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphql_http_server-1.4.6.tar", last modified: Thu May  4 16:12:25 2023, max compression
+gzip compressed data, was "graphql_http_server-1.4.7.tar", last modified: Tue Jun  6 17:35:38 2023, max compression
```

## Comparing `graphql_http_server-1.4.6.tar` & `graphql_http_server-1.4.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 16:12:25.778420 graphql_http_server-1.4.6/
--rwxrwxrwx   0 root         (0) root         (0)     1069 2023-05-04 16:12:16.000000 graphql_http_server-1.4.6/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      149 2023-05-04 16:12:16.000000 graphql_http_server-1.4.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      747 2023-05-04 16:12:25.778420 graphql_http_server-1.4.6/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)       90 2023-05-04 16:12:16.000000 graphql_http_server-1.4.6/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-05-04 16:12:25.000000 graphql_http_server-1.4.6/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 16:12:25.774419 graphql_http_server-1.4.6/graphql_http_server/
--rwxrwxrwx   0 root         (0) root         (0)       71 2023-05-04 16:12:16.000000 graphql_http_server-1.4.6/graphql_http_server/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      745 2023-05-04 16:12:16.000000 graphql_http_server-1.4.6/graphql_http_server/error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 16:12:25.776419 graphql_http_server-1.4.6/graphql_http_server/graphiql/
--rw-rw-rw-   0 root         (0) root         (0)     3100 2023-05-04 16:12:16.000000 graphql_http_server-1.4.6/graphql_http_server/graphiql/index.html
--rw-rw-rw-   0 root         (0) root         (0)     6574 2023-05-04 16:12:16.000000 graphql_http_server-1.4.6/graphql_http_server/helpers.py
--rwxrwxrwx   0 root         (0) root         (0)     8905 2023-05-04 16:12:16.000000 graphql_http_server-1.4.6/graphql_http_server/server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 16:12:25.776419 graphql_http_server-1.4.6/graphql_http_server.egg-info/
--rw-r--r--   0 root         (0) root         (0)      747 2023-05-04 16:12:25.000000 graphql_http_server-1.4.6/graphql_http_server.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      525 2023-05-04 16:12:25.000000 graphql_http_server-1.4.6/graphql_http_server.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 16:12:25.000000 graphql_http_server-1.4.6/graphql_http_server.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      120 2023-05-04 16:12:25.000000 graphql_http_server-1.4.6/graphql_http_server.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-05-04 16:12:25.000000 graphql_http_server-1.4.6/graphql_http_server.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       79 2023-05-04 16:12:25.778420 graphql_http_server-1.4.6/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1319 2023-05-04 16:12:16.000000 graphql_http_server-1.4.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 16:12:25.778420 graphql_http_server-1.4.6/tests/
--rwxrwxrwx   0 root         (0) root         (0)        0 2023-05-04 16:12:16.000000 graphql_http_server-1.4.6/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      489 2023-05-04 16:12:16.000000 graphql_http_server-1.4.6/tests/app.py
--rwxrwxrwx   0 root         (0) root         (0)      399 2023-05-04 16:12:16.000000 graphql_http_server-1.4.6/tests/conftest.py
--rwxrwxrwx   0 root         (0) root         (0)     2211 2023-05-04 16:12:16.000000 graphql_http_server-1.4.6/tests/test_app.py
--rw-rw-rw-   0 root         (0) root         (0)     2664 2023-05-04 16:12:16.000000 graphql_http_server-1.4.6/tests/test_graphql_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:35:38.785602 graphql_http_server-1.4.7/
+-rwxrwxrwx   0 root         (0) root         (0)     1069 2023-06-06 17:35:30.000000 graphql_http_server-1.4.7/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      149 2023-06-06 17:35:30.000000 graphql_http_server-1.4.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      747 2023-06-06 17:35:38.785602 graphql_http_server-1.4.7/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)       90 2023-06-06 17:35:30.000000 graphql_http_server-1.4.7/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-06-06 17:35:38.000000 graphql_http_server-1.4.7/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:35:38.783602 graphql_http_server-1.4.7/graphql_http_server/
+-rwxrwxrwx   0 root         (0) root         (0)       71 2023-06-06 17:35:30.000000 graphql_http_server-1.4.7/graphql_http_server/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      745 2023-06-06 17:35:30.000000 graphql_http_server-1.4.7/graphql_http_server/error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:35:38.784602 graphql_http_server-1.4.7/graphql_http_server/graphiql/
+-rw-rw-rw-   0 root         (0) root         (0)     3100 2023-06-06 17:35:30.000000 graphql_http_server-1.4.7/graphql_http_server/graphiql/index.html
+-rw-rw-rw-   0 root         (0) root         (0)     6574 2023-06-06 17:35:30.000000 graphql_http_server-1.4.7/graphql_http_server/helpers.py
+-rwxrwxrwx   0 root         (0) root         (0)    10429 2023-06-06 17:35:30.000000 graphql_http_server-1.4.7/graphql_http_server/server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:35:38.784602 graphql_http_server-1.4.7/graphql_http_server.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      747 2023-06-06 17:35:38.000000 graphql_http_server-1.4.7/graphql_http_server.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      525 2023-06-06 17:35:38.000000 graphql_http_server-1.4.7/graphql_http_server.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 17:35:38.000000 graphql_http_server-1.4.7/graphql_http_server.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      141 2023-06-06 17:35:38.000000 graphql_http_server-1.4.7/graphql_http_server.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-06-06 17:35:38.000000 graphql_http_server-1.4.7/graphql_http_server.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       79 2023-06-06 17:35:38.786602 graphql_http_server-1.4.7/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1351 2023-06-06 17:35:30.000000 graphql_http_server-1.4.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:35:38.785602 graphql_http_server-1.4.7/tests/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2023-06-06 17:35:30.000000 graphql_http_server-1.4.7/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      489 2023-06-06 17:35:30.000000 graphql_http_server-1.4.7/tests/app.py
+-rwxrwxrwx   0 root         (0) root         (0)      399 2023-06-06 17:35:30.000000 graphql_http_server-1.4.7/tests/conftest.py
+-rwxrwxrwx   0 root         (0) root         (0)     2211 2023-06-06 17:35:30.000000 graphql_http_server-1.4.7/tests/test_app.py
+-rw-rw-rw-   0 root         (0) root         (0)     2664 2023-06-06 17:35:30.000000 graphql_http_server-1.4.7/tests/test_graphql_api.py
```

### Comparing `graphql_http_server-1.4.6/LICENSE` & `graphql_http_server-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `graphql_http_server-1.4.6/PKG-INFO` & `graphql_http_server-1.4.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql_http_server
-Version: 1.4.6
+Version: 1.4.7
 Summary: HTTPServer for GraphQL.
 Home-page: https://gitlab.com/parob/graphql-http-server
-Download-URL: https://gitlab.com/parob/graphql-http-server/-/archive/master/graphql-http-server-v1.4.6.zip
+Download-URL: https://gitlab.com/parob/graphql-http-server/-/archive/master/graphql-http-server-v1.4.7.zip
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL,HTTPServer,werkzeug
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql_http_server-1.4.6/graphql_http_server/error.py` & `graphql_http_server-1.4.7/graphql_http_server/error.py`

 * *Files identical despite different names*

### Comparing `graphql_http_server-1.4.6/graphql_http_server/graphiql/index.html` & `graphql_http_server-1.4.7/graphql_http_server/graphiql/index.html`

 * *Files identical despite different names*

### Comparing `graphql_http_server-1.4.6/graphql_http_server/helpers.py` & `graphql_http_server-1.4.7/graphql_http_server/helpers.py`

 * *Files identical despite different names*

### Comparing `graphql_http_server-1.4.6/graphql_http_server/server.py` & `graphql_http_server-1.4.7/graphql_http_server/server.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,25 +4,34 @@
 
 from inspect import signature
 from typing import Any, List, Callable, Optional, Type
 
 from graphql import GraphQLError
 from werkzeug.wrappers import Request, Response
 from werkzeug.test import Client
+from json import JSONDecodeError
 
 from graphql.type.schema import GraphQLSchema
 from graphql.execution.execute import ExecutionContext
 
 from graphql_http_server.helpers import (
     HttpQueryError,
     encode_execution_results,
     json_encode,
     load_json_body,
     run_http_query,
 )
+import jwt
+from jwt import (
+    PyJWKClient,
+    InvalidTokenError,
+    InvalidAudienceError,
+    InvalidIssuerError,
+    DecodeError
+)
 
 
 def run_simple(
     schema,
     root_value: Any = None,
     middleware: List[Callable[[Callable, Any], Any]] = None,
     hostname: str = None,
@@ -87,28 +96,35 @@
         context: Any = None,
         serve_graphiql: bool = True,
         graphiql_default_query: str = None,
         graphiql_default_variables: str = None,
         allow_cors: bool = False,
         health_path: str = None,
         execution_context_class: Optional[Type[ExecutionContext]] = None,
+        auth_domain: str = None,
+        auth_audience: str = None,
+        auth_enabled: bool = False,
     ):
         if middleware is None:
             middleware = []
 
         self.schema = schema
         self.root_value = root_value
         self.middleware = middleware
         self.context = context
         self.serve_graphiql = serve_graphiql
         self.graphiql_default_query = graphiql_default_query
         self.graphiql_default_variables = graphiql_default_variables
         self.allow_cors = allow_cors
         self.health_path = health_path
         self.execution_context_class = execution_context_class
+        self.auth_domain = auth_domain
+        self.jwks_client = PyJWKClient(f"https://{auth_domain}/.well-known/jwks.json")
+        self.auth_audience = auth_audience
+        self.auth_enabled = auth_enabled
 
     def create_context(self):
         return copy.copy(self.context)
 
     @staticmethod
     def format_error(error: GraphQLError) -> {}:
         return error.formatted
@@ -129,14 +145,39 @@
         try:
             request_method = request.method.lower()
             data = self.parse_body(request=request)
 
             if self.health_path and request.path == self.health_path:
                 return Response("OK")
 
+            if self.auth_enabled and request_method != "options":
+                try:
+                    token = request.headers["Authorization"]
+                    token = token[len("Bearer "):]
+
+                    header = jwt.get_unverified_header(token)
+                    signing_key = self.jwks_client.get_signing_key(header["kid"])
+
+                    jwt.decode(
+                        token,
+                        audience=self.auth_audience,
+                        issuer=f"https://{self.auth_domain}/",
+                        key=signing_key.key,
+                        algorithms=["RS256"]
+                    )
+                except (
+                        InvalidTokenError,
+                        InvalidAudienceError,
+                        InvalidIssuerError,
+                        JSONDecodeError,
+                        DecodeError,
+                        KeyError,
+                ) as e:
+                    return self.error_response(e, status=401)
+
             if context is None:
                 context = self.create_context()
 
             is_get = request_method == "get"
             should_serve = self.should_serve_graphiql(request=request)
 
             show_graphiql = is_get and should_serve
@@ -191,20 +232,20 @@
                 content_type="application/json",
                 headers=headers,
             )
 
         except HttpQueryError as e:
             return self.error_response(e, headers)
 
-    def error_response(self, e, headers=None):
+    def error_response(self, e, headers=None, status=None):
         if headers is None:
             headers = {}
         return Response(
             self.encode({"errors": [str(e)]}),
-            status=getattr(e, "status_code", 200),
+            status=status if status is not None else getattr(e, "status_code", 200),
             headers={**(getattr(e, "headers", {}) or {}), **headers},
             content_type="application/json",
         )
 
     # noinspection PyMethodMayBeStatic
     def parse_body(self, request):
         content_type = request.mimetype
```

### Comparing `graphql_http_server-1.4.6/graphql_http_server.egg-info/PKG-INFO` & `graphql_http_server-1.4.7/graphql_http_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql-http-server
-Version: 1.4.6
+Version: 1.4.7
 Summary: HTTPServer for GraphQL.
 Home-page: https://gitlab.com/parob/graphql-http-server
-Download-URL: https://gitlab.com/parob/graphql-http-server/-/archive/master/graphql-http-server-v1.4.6.zip
+Download-URL: https://gitlab.com/parob/graphql-http-server/-/archive/master/graphql-http-server-v1.4.7.zip
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL,HTTPServer,werkzeug
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql_http_server-1.4.6/graphql_http_server.egg-info/SOURCES.txt` & `graphql_http_server-1.4.7/graphql_http_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphql_http_server-1.4.6/setup.py` & `graphql_http_server-1.4.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     install_requires=[
         "graphql-core>=3.2.0",
         "graphql-api>=1.3.0",
         "werkzeug>=2.2.2",
         "context-helper>=1.0.2",
         "packaging>=21.3",
         "graphql-schema-diff>=1.2.4",
+        "pyjwt[crypto]==2.7.0",
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

### Comparing `graphql_http_server-1.4.6/tests/test_app.py` & `graphql_http_server-1.4.7/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `graphql_http_server-1.4.6/tests/test_graphql_api.py` & `graphql_http_server-1.4.7/tests/test_graphql_api.py`

 * *Files identical despite different names*

