# Comparing `tmp/zeph1rr_fastapi_utils-1.0.0.tar.gz` & `tmp/zeph1rr_fastapi_utils-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeph1rr_fastapi_utils-1.0.0.tar", max compression
+gzip compressed data, was "zeph1rr_fastapi_utils-1.0.1.tar", max compression
```

## Comparing `zeph1rr_fastapi_utils-1.0.0.tar` & `zeph1rr_fastapi_utils-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      527 2023-05-30 22:47:33.985842 zeph1rr_fastapi_utils-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-28 20:54:40.889819 zeph1rr_fastapi_utils-1.0.0/README.md
--rw-r--r--   0        0        0      158 2023-05-28 20:57:48.425054 zeph1rr_fastapi_utils-1.0.0/zeph1rr_fastapi_utils/__init__.py
--rw-r--r--   0        0        0     1852 2023-05-28 21:03:01.524784 zeph1rr_fastapi_utils-1.0.0/zeph1rr_fastapi_utils/logger.py
--rw-r--r--   0        0        0     2234 2023-05-30 22:47:23.232714 zeph1rr_fastapi_utils-1.0.0/zeph1rr_fastapi_utils/utils.py
--rw-r--r--   0        0        0      623 1970-01-01 00:00:00.000000 zeph1rr_fastapi_utils-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      527 2023-06-06 17:00:06.824063 zeph1rr_fastapi_utils-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-28 20:54:40.889819 zeph1rr_fastapi_utils-1.0.1/README.md
+-rw-r--r--   0        0        0      158 2023-05-28 20:57:48.425054 zeph1rr_fastapi_utils-1.0.1/zeph1rr_fastapi_utils/__init__.py
+-rw-r--r--   0        0        0     1810 2023-06-06 16:59:35.503580 zeph1rr_fastapi_utils-1.0.1/zeph1rr_fastapi_utils/logger.py
+-rw-r--r--   0        0        0     2234 2023-05-30 22:47:23.232714 zeph1rr_fastapi_utils-1.0.1/zeph1rr_fastapi_utils/utils.py
+-rw-r--r--   0        0        0      623 1970-01-01 00:00:00.000000 zeph1rr_fastapi_utils-1.0.1/PKG-INFO
```

### Comparing `zeph1rr_fastapi_utils-1.0.0/pyproject.toml` & `zeph1rr_fastapi_utils-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zeph1rr-fastapi-utils"
-version = "1.0.0"
+version = "1.0.1"
 description = "Package for unificate functions in fastapi"
 authors = ["Zeph1rr <grianton535@gmail.com>"]
 readme = "README.md"
 packages = [{include = "zeph1rr_fastapi_utils"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `zeph1rr_fastapi_utils-1.0.0/zeph1rr_fastapi_utils/logger.py` & `zeph1rr_fastapi_utils-1.0.1/zeph1rr_fastapi_utils/logger.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,14 +24,15 @@
             pathlib.Path(log_path, f"{app_name}.log"),
             format=logger_format,
             level=log_level,
             rotation="500mb",
             compression="gz",
         )
 
+
 async def loggingMiddleware(request: Request, call_next: Callable) -> Response:
     start_time = time.time()
     request_logger_data = {
         "type": "REQUEST",
         "method": request.method,
         "path": request.url.path,
     }
@@ -41,19 +42,15 @@
         "type": "RESPONSE",
         "status_code": response.status_code,
         "request_time_duration": time.time() - start_time,
     }
     if response.status_code != 200:
         response_body = [chunk async for chunk in response.body_iterator]
         response.body_iterator = iterate_in_threadpool(iter(response_body))
-        response_body = json.loads(response_body[0].decode())
-        logger.error(
-            json.dumps(
-                {
-                    **response_logger_data, 
-                    "error": response_body['detail']
-                }
+        if len(response_body):
+            response_body = json.loads(response_body[0].decode())
+            logger.error(
+                json.dumps({**response_logger_data, "error": response_body["detail"]})
             )
-        )
     else:
         logger.success(json.dumps(response_logger_data))
-    return response
+    return response
```

### Comparing `zeph1rr_fastapi_utils-1.0.0/zeph1rr_fastapi_utils/utils.py` & `zeph1rr_fastapi_utils-1.0.1/zeph1rr_fastapi_utils/utils.py`

 * *Files identical despite different names*

### Comparing `zeph1rr_fastapi_utils-1.0.0/PKG-INFO` & `zeph1rr_fastapi_utils-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeph1rr-fastapi-utils
-Version: 1.0.0
+Version: 1.0.1
 Summary: Package for unificate functions in fastapi
 Author: Zeph1rr
 Author-email: grianton535@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bcrypt (>=4.0.1,<5.0.0)
```

