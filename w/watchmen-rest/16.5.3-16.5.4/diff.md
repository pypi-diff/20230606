# Comparing `tmp/watchmen_rest-16.5.3.tar.gz` & `tmp/watchmen_rest-16.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_rest-16.5.3.tar", max compression
+gzip compressed data, was "watchmen_rest-16.5.4.tar", max compression
```

## Comparing `watchmen_rest-16.5.3.tar` & `watchmen_rest-16.5.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1061 2023-06-05 01:29:03.540124 watchmen_rest-16.5.3/LICENSE
--rw-r--r--   0        0        0      658 2023-06-05 01:29:03.540124 watchmen_rest-16.5.3/pyproject.toml
--rw-r--r--   0        0        0      668 2023-06-05 01:29:03.540124 watchmen_rest-16.5.3/src/watchmen_rest/__init__.py
--rw-r--r--   0        0        0     2089 2023-06-05 01:29:03.540124 watchmen_rest-16.5.3/src/watchmen_rest/auth_helper.py
--rw-r--r--   0        0        0     5801 2023-06-05 01:29:03.540124 watchmen_rest-16.5.3/src/watchmen_rest/authentication.py
--rw-r--r--   0        0        0      419 2023-06-05 01:29:03.540124 watchmen_rest-16.5.3/src/watchmen_rest/cors.py
--rw-r--r--   0        0        0       98 2023-06-05 01:29:03.540124 watchmen_rest-16.5.3/src/watchmen_rest/exceptions.py
--rw-r--r--   0        0        0      295 2023-06-05 01:29:03.540124 watchmen_rest-16.5.3/src/watchmen_rest/prometheus.py
--rw-r--r--   0        0        0     2492 2023-06-05 01:29:03.540124 watchmen_rest-16.5.3/src/watchmen_rest/rest_app.py
--rw-r--r--   0        0        0      938 2023-06-05 01:29:03.540124 watchmen_rest-16.5.3/src/watchmen_rest/settings.py
--rw-r--r--   0        0        0        0 2023-06-05 01:29:03.540124 watchmen_rest-16.5.3/src/watchmen_rest/system/__init__.py
--rw-r--r--   0        0        0      139 2023-06-05 01:29:03.540124 watchmen_rest-16.5.3/src/watchmen_rest/system/health_router.py
--rw-r--r--   0        0        0      130 2023-06-05 01:29:03.540124 watchmen_rest-16.5.3/src/watchmen_rest/util/__init__.py
--rw-r--r--   0        0        0     1467 2023-06-05 01:29:03.540124 watchmen_rest-16.5.3/src/watchmen_rest/util/raise_http_exception.py
--rw-r--r--   0        0        0      949 2023-06-05 01:29:03.540124 watchmen_rest-16.5.3/src/watchmen_rest/util/validator.py
--rw-r--r--   0        0        0      793 1970-01-01 00:00:00.000000 watchmen_rest-16.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-06 01:45:59.149403 watchmen_rest-16.5.4/LICENSE
+-rw-r--r--   0        0        0      658 2023-06-06 01:45:59.149403 watchmen_rest-16.5.4/pyproject.toml
+-rw-r--r--   0        0        0      668 2023-06-06 01:45:59.149403 watchmen_rest-16.5.4/src/watchmen_rest/__init__.py
+-rw-r--r--   0        0        0     2089 2023-06-06 01:45:59.149403 watchmen_rest-16.5.4/src/watchmen_rest/auth_helper.py
+-rw-r--r--   0        0        0     5801 2023-06-06 01:45:59.149403 watchmen_rest-16.5.4/src/watchmen_rest/authentication.py
+-rw-r--r--   0        0        0      419 2023-06-06 01:45:59.149403 watchmen_rest-16.5.4/src/watchmen_rest/cors.py
+-rw-r--r--   0        0        0       98 2023-06-06 01:45:59.149403 watchmen_rest-16.5.4/src/watchmen_rest/exceptions.py
+-rw-r--r--   0        0        0      295 2023-06-06 01:45:59.149403 watchmen_rest-16.5.4/src/watchmen_rest/prometheus.py
+-rw-r--r--   0        0        0     2492 2023-06-06 01:45:59.149403 watchmen_rest-16.5.4/src/watchmen_rest/rest_app.py
+-rw-r--r--   0        0        0      938 2023-06-06 01:45:59.149403 watchmen_rest-16.5.4/src/watchmen_rest/settings.py
+-rw-r--r--   0        0        0        0 2023-06-06 01:45:59.149403 watchmen_rest-16.5.4/src/watchmen_rest/system/__init__.py
+-rw-r--r--   0        0        0      139 2023-06-06 01:45:59.149403 watchmen_rest-16.5.4/src/watchmen_rest/system/health_router.py
+-rw-r--r--   0        0        0      130 2023-06-06 01:45:59.149403 watchmen_rest-16.5.4/src/watchmen_rest/util/__init__.py
+-rw-r--r--   0        0        0     1467 2023-06-06 01:45:59.149403 watchmen_rest-16.5.4/src/watchmen_rest/util/raise_http_exception.py
+-rw-r--r--   0        0        0      949 2023-06-06 01:45:59.149403 watchmen_rest-16.5.4/src/watchmen_rest/util/validator.py
+-rw-r--r--   0        0        0      793 1970-01-01 00:00:00.000000 watchmen_rest-16.5.4/PKG-INFO
```

### Comparing `watchmen_rest-16.5.3/LICENSE` & `watchmen_rest-16.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_rest-16.5.3/src/watchmen_rest/__init__.py` & `watchmen_rest-16.5.4/src/watchmen_rest/__init__.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest-16.5.3/src/watchmen_rest/auth_helper.py` & `watchmen_rest-16.5.4/src/watchmen_rest/auth_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest-16.5.3/src/watchmen_rest/authentication.py` & `watchmen_rest-16.5.4/src/watchmen_rest/authentication.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest-16.5.3/src/watchmen_rest/rest_app.py` & `watchmen_rest-16.5.4/src/watchmen_rest/rest_app.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest-16.5.3/src/watchmen_rest/settings.py` & `watchmen_rest-16.5.4/src/watchmen_rest/settings.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest-16.5.3/src/watchmen_rest/util/raise_http_exception.py` & `watchmen_rest-16.5.4/src/watchmen_rest/util/raise_http_exception.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest-16.5.3/src/watchmen_rest/util/validator.py` & `watchmen_rest-16.5.4/src/watchmen_rest/util/validator.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest-16.5.3/PKG-INFO` & `watchmen_rest-16.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchmen-rest
-Version: 16.5.3
+Version: 16.5.4
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,9 +13,9 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: fastapi (>=0.75.1,<0.76.0)
 Requires-Dist: jsonschema (>=4.4.0,<5.0.0)
 Requires-Dist: python-dotenv (>=0.20.0,<0.21.0)
 Requires-Dist: python-jose (>=3.3.0,<4.0.0)
 Requires-Dist: starlette-prometheus (>=0.9.0,<0.10.0)
 Requires-Dist: uvicorn (>=0.17.6,<0.18.0)
-Requires-Dist: watchmen-auth (==16.5.3)
-Requires-Dist: watchmen-storage (==16.5.3)
+Requires-Dist: watchmen-auth (==16.5.4)
+Requires-Dist: watchmen-storage (==16.5.4)
```

