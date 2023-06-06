# Comparing `tmp/pylacus-1.5.0.tar.gz` & `tmp/pylacus-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylacus-1.5.0.tar", max compression
+gzip compressed data, was "pylacus-1.5.1.tar", max compression
```

## Comparing `pylacus-1.5.0.tar` & `pylacus-1.5.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1548 2022-09-21 08:51:05.297797 pylacus-1.5.0/LICENSE
--rw-r--r--   0        0        0     1246 2022-10-19 12:48:44.949008 pylacus-1.5.0/README.md
--rw-r--r--   0        0        0     1532 2022-09-22 10:52:07.800972 pylacus-1.5.0/pylacus/__init__.py
--rw-r--r--   0        0        0     8415 2022-11-01 13:48:16.210836 pylacus-1.5.0/pylacus/api.py
--rw-r--r--   0        0        0        0 2022-09-21 08:47:31.320167 pylacus-1.5.0/pylacus/py.typed
--rw-r--r--   0        0        0     1452 2023-05-31 14:22:28.750006 pylacus-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     2720 1970-01-01 00:00:00.000000 pylacus-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1548 2022-09-21 08:51:05.297797 pylacus-1.5.1/LICENSE
+-rw-r--r--   0        0        0     1246 2022-10-19 12:48:44.949008 pylacus-1.5.1/README.md
+-rw-r--r--   0        0        0     1532 2022-09-22 10:52:07.800972 pylacus-1.5.1/pylacus/__init__.py
+-rw-r--r--   0        0        0     9282 2023-06-06 14:49:26.427656 pylacus-1.5.1/pylacus/api.py
+-rw-r--r--   0        0        0        0 2022-09-21 08:47:31.320167 pylacus-1.5.1/pylacus/py.typed
+-rw-r--r--   0        0        0     1452 2023-06-06 15:50:22.958019 pylacus-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2470 1970-01-01 00:00:00.000000 pylacus-1.5.1/PKG-INFO
```

### Comparing `pylacus-1.5.0/LICENSE` & `pylacus-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pylacus-1.5.0/README.md` & `pylacus-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pylacus-1.5.0/pylacus/__init__.py` & `pylacus-1.5.1/pylacus/__init__.py`

 * *Files identical despite different names*

### Comparing `pylacus-1.5.0/pylacus/api.py` & `pylacus-1.5.1/pylacus/api.py`

 * *Files 17% similar despite different names*

```diff
@@ -62,15 +62,19 @@
     browser: Optional[str]
     device_name: Optional[str]
     user_agent: Optional[str]
     proxy: Optional[Union[str, Dict[str, str]]]
     general_timeout_in_sec: Optional[int]
     cookies: Optional[List[Dict[str, Any]]]
     headers: Optional[Union[str, Dict[str, str]]]
-    http_credentials: Optional[Dict[str, int]]
+    http_credentials: Optional[Dict[str, str]]
+    geolocation: Optional[Dict[str, float]]
+    timezone_id: Optional[str]
+    locale: Optional[str]
+    color_scheme: Optional[str]
     viewport: Optional[Dict[str, int]]
     referer: Optional[str]
     force: Optional[bool]
     recapture_interval: Optional[int]
     priority: Optional[int]
     uuid: Optional[str]
 
@@ -118,15 +122,19 @@
                 depth: int=0,
                 browser: Optional[BROWSER]=None, device_name: Optional[str]=None,
                 user_agent: Optional[str]=None,
                 proxy: Optional[Union[str, Dict[str, str]]]=None,
                 general_timeout_in_sec: Optional[int]=None,
                 cookies: Optional[List[Dict[str, Any]]]=None,
                 headers: Optional[Union[str, Dict[str, str]]]=None,
-                http_credentials: Optional[Dict[str, int]]=None,
+                http_credentials: Optional[Dict[str, str]]=None,
+                geolocation: Optional[Dict[str, float]]=None,
+                timezone_id: Optional[str]=None,
+                locale: Optional[str]=None,
+                color_scheme: Optional[str]=None,
                 viewport: Optional[Dict[str, int]]=None,
                 referer: Optional[str]=None,
                 rendered_hostname_only: bool=True,
                 force: bool=False,
                 recapture_interval: int=300,
                 priority: int=0,
                 uuid: Optional[str]=None,
@@ -140,15 +148,19 @@
                 depth: int=0,
                 browser: Optional[BROWSER]=None, device_name: Optional[str]=None,
                 user_agent: Optional[str]=None,
                 proxy: Optional[Union[str, Dict[str, str]]]=None,
                 general_timeout_in_sec: Optional[int]=None,
                 cookies: Optional[List[Dict[str, Any]]]=None,
                 headers: Optional[Union[str, Dict[str, str]]]=None,
-                http_credentials: Optional[Dict[str, int]]=None,
+                http_credentials: Optional[Dict[str, str]]=None,
+                geolocation: Optional[Dict[str, float]]=None,
+                timezone_id: Optional[str]=None,
+                locale: Optional[str]=None,
+                color_scheme: Optional[str]=None,
                 viewport: Optional[Dict[str, int]]=None,
                 referer: Optional[str]=None,
                 rendered_hostname_only: bool=True,
                 force: bool=False,
                 recapture_interval: int=300,
                 priority: int=0,
                 uuid: Optional[str]=None,
@@ -177,14 +189,22 @@
                 to_enqueue['general_timeout_in_sec'] = general_timeout_in_sec
             if cookies:
                 to_enqueue['cookies'] = cookies
             if headers:
                 to_enqueue['headers'] = headers
             if http_credentials:
                 to_enqueue['http_credentials'] = http_credentials
+            if geolocation:
+                to_enqueue['geolocation'] = geolocation
+            if timezone_id:
+                to_enqueue['timezone_id'] = timezone_id
+            if locale:
+                to_enqueue['locale'] = locale
+            if color_scheme:
+                to_enqueue['color_scheme'] = color_scheme
             if viewport:
                 to_enqueue['viewport'] = viewport
             if referer:
                 to_enqueue['referer'] = referer
             if uuid:
                 to_enqueue['uuid'] = uuid
```

### Comparing `pylacus-1.5.0/pyproject.toml` & `pylacus-1.5.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pylacus"
-version = "1.5.0"
+version = "1.5.1"
 description = "Python CLI and module for lacus"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/ail-project/PyLacus"
 documentation = "https://pylacus.readthedocs.io/en/latest/index.html"
 
 readme = "README.md"
```

### Comparing `pylacus-1.5.0/PKG-INFO` & `pylacus-1.5.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylacus
-Version: 1.5.0
+Version: 1.5.1
 Summary: Python CLI and module for lacus
 Home-page: https://github.com/ail-project/PyLacus
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,19 +15,14 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet
 Classifier: Topic :: Security
 Provides-Extra: docs
 Requires-Dist: Sphinx (>=7.0.1,<8.0.0) ; extra == "docs"
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Documentation, https://pylacus.readthedocs.io/en/latest/index.html
 Project-URL: Repository, https://github.com/ail-project/PyLacus
```

