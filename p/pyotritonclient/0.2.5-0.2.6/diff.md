# Comparing `tmp/pyotritonclient-0.2.5.tar.gz` & `tmp/pyotritonclient-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyotritonclient-0.2.5.tar", last modified: Tue Jan 31 17:24:58 2023, max compression
+gzip compressed data, was "pyotritonclient-0.2.6.tar", last modified: Tue Jun  6 08:48:18 2023, max compression
```

## Comparing `pyotritonclient-0.2.5.tar` & `pyotritonclient-0.2.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 weiouyang  (1002) weiouyang  (1002)        0 2023-01-31 17:24:58.330597 pyotritonclient-0.2.5/
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     2057 2022-01-31 13:44:37.000000 pyotritonclient-0.2.5/.gitignore
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     1533 2021-09-23 13:56:19.000000 pyotritonclient-0.2.5/LICENSE.txt
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)       31 2022-01-31 13:44:37.000000 pyotritonclient-0.2.5/MANIFEST.in
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     6108 2023-01-31 17:24:58.330597 pyotritonclient-0.2.5/PKG-INFO
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     4787 2022-01-31 13:44:37.000000 pyotritonclient-0.2.5/README.md
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     4365 2022-01-31 13:44:37.000000 pyotritonclient-0.2.5/codex-instructions.md
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)      164 2021-09-23 13:56:19.000000 pyotritonclient-0.2.5/publish.sh
-drwxrwxr-x   0 weiouyang  (1002) weiouyang  (1002)        0 2023-01-31 17:24:58.326597 pyotritonclient-0.2.5/pyotritonclient/
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)       26 2023-01-31 17:24:13.000000 pyotritonclient-0.2.5/pyotritonclient/VERSION
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)    10387 2023-01-31 17:23:42.000000 pyotritonclient-0.2.5/pyotritonclient/__init__.py
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)    59318 2022-06-11 16:54:40.000000 pyotritonclient-0.2.5/pyotritonclient/http.py
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     2911 2022-05-05 15:16:00.000000 pyotritonclient-0.2.5/pyotritonclient/httpclient.py
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     2941 2022-05-05 11:48:28.000000 pyotritonclient-0.2.5/pyotritonclient/pyohttpclient.py
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     8090 2021-09-25 20:17:19.000000 pyotritonclient-0.2.5/pyotritonclient/utils.py
-drwxrwxr-x   0 weiouyang  (1002) weiouyang  (1002)        0 2023-01-31 17:24:58.330597 pyotritonclient-0.2.5/pyotritonclient.egg-info/
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     6108 2023-01-31 17:24:58.000000 pyotritonclient-0.2.5/pyotritonclient.egg-info/PKG-INFO
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)      554 2023-01-31 17:24:58.000000 pyotritonclient-0.2.5/pyotritonclient.egg-info/SOURCES.txt
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)        1 2023-01-31 17:24:58.000000 pyotritonclient-0.2.5/pyotritonclient.egg-info/dependency_links.txt
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)        1 2021-09-23 16:25:06.000000 pyotritonclient-0.2.5/pyotritonclient.egg-info/not-zip-safe
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)      116 2023-01-31 17:24:58.000000 pyotritonclient-0.2.5/pyotritonclient.egg-info/requires.txt
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)       16 2023-01-31 17:24:58.000000 pyotritonclient-0.2.5/pyotritonclient.egg-info/top_level.txt
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     1552 2022-05-04 15:51:57.000000 pyotritonclient-0.2.5/requirements.txt
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)       38 2023-01-31 17:24:58.330597 pyotritonclient-0.2.5/setup.cfg
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     3897 2022-05-05 15:16:36.000000 pyotritonclient-0.2.5/setup.py
-drwxrwxr-x   0 weiouyang  (1002) weiouyang  (1002)        0 2023-01-31 17:24:58.330597 pyotritonclient-0.2.5/tests/
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     3009 2022-01-31 13:44:37.000000 pyotritonclient-0.2.5/tests/test_client.py
--rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     1983 2023-01-31 17:23:58.000000 pyotritonclient-0.2.5/tests/test_imjoy_serialization.py
+drwxrwxr-x   0 weiouyang  (1002) weiouyang  (1002)        0 2023-06-06 08:48:18.828197 pyotritonclient-0.2.6/
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     2057 2022-01-31 13:44:37.000000 pyotritonclient-0.2.6/.gitignore
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     1533 2021-09-23 13:56:19.000000 pyotritonclient-0.2.6/LICENSE.txt
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)       31 2022-01-31 13:44:37.000000 pyotritonclient-0.2.6/MANIFEST.in
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     6108 2023-06-06 08:48:18.828197 pyotritonclient-0.2.6/PKG-INFO
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     4787 2022-01-31 13:44:37.000000 pyotritonclient-0.2.6/README.md
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     4365 2022-01-31 13:44:37.000000 pyotritonclient-0.2.6/codex-instructions.md
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)      164 2021-09-23 13:56:19.000000 pyotritonclient-0.2.6/publish.sh
+drwxrwxr-x   0 weiouyang  (1002) weiouyang  (1002)        0 2023-06-06 08:48:18.828197 pyotritonclient-0.2.6/pyotritonclient/
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)       26 2023-06-06 08:48:05.000000 pyotritonclient-0.2.6/pyotritonclient/VERSION
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)    10387 2023-01-31 17:23:42.000000 pyotritonclient-0.2.6/pyotritonclient/__init__.py
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)    59318 2022-06-11 16:54:40.000000 pyotritonclient-0.2.6/pyotritonclient/http.py
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     2911 2022-05-05 15:16:00.000000 pyotritonclient-0.2.6/pyotritonclient/httpclient.py
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     3005 2023-06-06 08:47:40.000000 pyotritonclient-0.2.6/pyotritonclient/pyohttpclient.py
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     8090 2021-09-25 20:17:19.000000 pyotritonclient-0.2.6/pyotritonclient/utils.py
+drwxrwxr-x   0 weiouyang  (1002) weiouyang  (1002)        0 2023-06-06 08:48:18.828197 pyotritonclient-0.2.6/pyotritonclient.egg-info/
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     6108 2023-06-06 08:48:18.000000 pyotritonclient-0.2.6/pyotritonclient.egg-info/PKG-INFO
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)      554 2023-06-06 08:48:18.000000 pyotritonclient-0.2.6/pyotritonclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)        1 2023-06-06 08:48:18.000000 pyotritonclient-0.2.6/pyotritonclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)        1 2021-09-23 16:25:06.000000 pyotritonclient-0.2.6/pyotritonclient.egg-info/not-zip-safe
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)      116 2023-06-06 08:48:18.000000 pyotritonclient-0.2.6/pyotritonclient.egg-info/requires.txt
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)       16 2023-06-06 08:48:18.000000 pyotritonclient-0.2.6/pyotritonclient.egg-info/top_level.txt
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     1552 2022-05-04 15:51:57.000000 pyotritonclient-0.2.6/requirements.txt
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)       38 2023-06-06 08:48:18.828197 pyotritonclient-0.2.6/setup.cfg
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     3897 2022-05-05 15:16:36.000000 pyotritonclient-0.2.6/setup.py
+drwxrwxr-x   0 weiouyang  (1002) weiouyang  (1002)        0 2023-06-06 08:48:18.828197 pyotritonclient-0.2.6/tests/
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     3009 2022-01-31 13:44:37.000000 pyotritonclient-0.2.6/tests/test_client.py
+-rw-rw-r--   0 weiouyang  (1002) weiouyang  (1002)     1983 2023-01-31 17:23:58.000000 pyotritonclient-0.2.6/tests/test_imjoy_serialization.py
```

### Comparing `pyotritonclient-0.2.5/.gitignore` & `pyotritonclient-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pyotritonclient-0.2.5/LICENSE.txt` & `pyotritonclient-0.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyotritonclient-0.2.5/PKG-INFO` & `pyotritonclient-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyotritonclient
-Version: 0.2.5
+Version: 0.2.6
 Summary: A lightweight http client library for communicating with Nvidia Triton Inference Server (with Pyodide support in the browser)
 Home-page: https://github.com/oeway/pyotritonclient
 Author: Wei OUYANG
 Author-email: oeway007@gmail.com
 License: BSD
 Keywords: pyodide,http,triton,tensorrt,inference,server,service,client,nvidia
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyotritonclient-0.2.5/README.md` & `pyotritonclient-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `pyotritonclient-0.2.5/codex-instructions.md` & `pyotritonclient-0.2.6/codex-instructions.md`

 * *Files identical despite different names*

### Comparing `pyotritonclient-0.2.5/pyotritonclient/__init__.py` & `pyotritonclient-0.2.6/pyotritonclient/__init__.py`

 * *Files identical despite different names*

### Comparing `pyotritonclient-0.2.5/pyotritonclient/http.py` & `pyotritonclient-0.2.6/pyotritonclient/http.py`

 * *Files identical despite different names*

### Comparing `pyotritonclient-0.2.5/pyotritonclient/httpclient.py` & `pyotritonclient-0.2.6/pyotritonclient/httpclient.py`

 * *Files identical despite different names*

### Comparing `pyotritonclient-0.2.5/pyotritonclient/pyohttpclient.py` & `pyotritonclient-0.2.6/pyotritonclient/pyohttpclient.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 import json
-from pyodide import to_js
+try:
+    from pyodide.ffi import to_js
+except ImportError:
+    from pyodide import to_js
+
 from js import Object, fetch
 
 
 class HTTPResponse:
     def __init__(self, js_response, body_buffer, method="GET"):
         self.method = method.upper()
         self.status_message = None
```

### Comparing `pyotritonclient-0.2.5/pyotritonclient/utils.py` & `pyotritonclient-0.2.6/pyotritonclient/utils.py`

 * *Files identical despite different names*

### Comparing `pyotritonclient-0.2.5/pyotritonclient.egg-info/PKG-INFO` & `pyotritonclient-0.2.6/pyotritonclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyotritonclient
-Version: 0.2.5
+Version: 0.2.6
 Summary: A lightweight http client library for communicating with Nvidia Triton Inference Server (with Pyodide support in the browser)
 Home-page: https://github.com/oeway/pyotritonclient
 Author: Wei OUYANG
 Author-email: oeway007@gmail.com
 License: BSD
 Keywords: pyodide,http,triton,tensorrt,inference,server,service,client,nvidia
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyotritonclient-0.2.5/pyotritonclient.egg-info/SOURCES.txt` & `pyotritonclient-0.2.6/pyotritonclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyotritonclient-0.2.5/requirements.txt` & `pyotritonclient-0.2.6/requirements.txt`

 * *Files identical despite different names*

### Comparing `pyotritonclient-0.2.5/setup.py` & `pyotritonclient-0.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `pyotritonclient-0.2.5/tests/test_client.py` & `pyotritonclient-0.2.6/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pyotritonclient-0.2.5/tests/test_imjoy_serialization.py` & `pyotritonclient-0.2.6/tests/test_imjoy_serialization.py`

 * *Files identical despite different names*

