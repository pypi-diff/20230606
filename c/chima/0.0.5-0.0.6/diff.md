# Comparing `tmp/chima-0.0.5.tar.gz` & `tmp/chima-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chima-0.0.5.tar", max compression
+gzip compressed data, was "chima-0.0.6.tar", max compression
```

## Comparing `chima-0.0.5.tar` & `chima-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     2253 2023-06-06 21:31:49.027920 chima-0.0.5/README.md
--rw-r--r--   0        0        0      365 2023-06-06 21:31:49.027920 chima-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      191 2023-06-06 21:31:49.027920 chima-0.0.5/src/chima/__init__.py
--rw-r--r--   0        0        0     6351 2023-06-06 21:31:49.027920 chima-0.0.5/src/chima/client.py
--rw-r--r--   0        0        0      348 2023-06-06 21:31:49.027920 chima-0.0.5/src/chima/core/__init__.py
--rw-r--r--   0        0        0      426 2023-06-06 21:31:49.027920 chima-0.0.5/src/chima/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-06-06 21:31:49.027920 chima-0.0.5/src/chima/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-06-06 21:31:49.027920 chima-0.0.5/src/chima/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-06-06 21:31:49.027920 chima-0.0.5/src/chima/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      159 2023-06-06 21:31:49.027920 chima-0.0.5/src/chima/environment.py
--rw-r--r--   0        0        0        0 2023-06-06 21:31:49.027920 chima-0.0.5/src/chima/py.typed
--rw-r--r--   0        0        0      139 2023-06-06 21:31:49.027920 chima-0.0.5/src/chima/types/__init__.py
--rw-r--r--   0        0        0      920 2023-06-06 21:31:49.027920 chima-0.0.5/src/chima/types/search_response.py
--rw-r--r--   0        0        0     2683 1970-01-01 00:00:00.000000 chima-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     2253 2023-06-06 21:54:43.678602 chima-0.0.6/README.md
+-rw-r--r--   0        0        0      365 2023-06-06 21:54:43.678602 chima-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      191 2023-06-06 21:54:43.678602 chima-0.0.6/src/chima/__init__.py
+-rw-r--r--   0        0        0     4966 2023-06-06 21:54:43.678602 chima-0.0.6/src/chima/client.py
+-rw-r--r--   0        0        0      348 2023-06-06 21:54:43.678602 chima-0.0.6/src/chima/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-06-06 21:54:43.678602 chima-0.0.6/src/chima/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-06-06 21:54:43.678602 chima-0.0.6/src/chima/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-06-06 21:54:43.678602 chima-0.0.6/src/chima/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-06-06 21:54:43.678602 chima-0.0.6/src/chima/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      159 2023-06-06 21:54:43.682602 chima-0.0.6/src/chima/environment.py
+-rw-r--r--   0        0        0        0 2023-06-06 21:54:43.682602 chima-0.0.6/src/chima/py.typed
+-rw-r--r--   0        0        0      139 2023-06-06 21:54:43.682602 chima-0.0.6/src/chima/types/__init__.py
+-rw-r--r--   0        0        0      920 2023-06-06 21:54:43.682602 chima-0.0.6/src/chima/types/search_response.py
+-rw-r--r--   0        0        0     2683 1970-01-01 00:00:00.000000 chima-0.0.6/PKG-INFO
```

### Comparing `chima-0.0.5/README.md` & `chima-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `chima-0.0.5/src/chima/client.py` & `chima-0.0.6/src/chima/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -66,29 +66,14 @@
                 return
             try:
                 _response_json = _response.json()
             except JSONDecodeError:
                 raise ApiError(status_code=_response.status_code, body=_response.text)
             raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def notify(self, *, cloud_id: str) -> str:
-        _response = httpx.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._environment.value}/", "notify"),
-            json=jsonable_encoder({"cloudId": cloud_id}),
-            timeout=60,
-        )
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(str, _response_json)  # type: ignore
-        raise ApiError(status_code=_response.status_code, body=_response_json)
-
 
 class AsyncChima:
     def __init__(self, *, environment: ChimaEnvironment = ChimaEnvironment.PRODUCTION):
         self._environment = environment
 
     async def search(
         self,
@@ -136,23 +121,7 @@
                         yield pydantic.parse_obj_as(str, json.loads(_text))  # type: ignore
                     return
                 try:
                     _response_json = _response.json()
                 except JSONDecodeError:
                     raise ApiError(status_code=_response.status_code, body=_response.text)
                 raise ApiError(status_code=_response.status_code, body=_response_json)
-
-    async def notify(self, *, cloud_id: str) -> str:
-        async with httpx.AsyncClient() as _client:
-            _response = await _client.request(
-                "POST",
-                urllib.parse.urljoin(f"{self._environment.value}/", "notify"),
-                json=jsonable_encoder({"cloudId": cloud_id}),
-                timeout=60,
-            )
-        try:
-            _response_json = _response.json()
-        except JSONDecodeError:
-            raise ApiError(status_code=_response.status_code, body=_response.text)
-        if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(str, _response_json)  # type: ignore
-        raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `chima-0.0.5/src/chima/core/datetime_utils.py` & `chima-0.0.6/src/chima/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `chima-0.0.5/src/chima/core/jsonable_encoder.py` & `chima-0.0.6/src/chima/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `chima-0.0.5/src/chima/types/search_response.py` & `chima-0.0.6/src/chima/types/search_response.py`

 * *Files identical despite different names*

### Comparing `chima-0.0.5/PKG-INFO` & `chima-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chima
-Version: 0.0.5
+Version: 0.0.6
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

