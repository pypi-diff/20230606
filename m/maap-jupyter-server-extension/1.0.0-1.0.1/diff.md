# Comparing `tmp/maap_jupyter_server_extension-1.0.0.tar.gz` & `tmp/maap_jupyter_server_extension-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maap_jupyter_server_extension-1.0.0.tar", last modified: Thu Mar 30 22:34:34 2023, max compression
+gzip compressed data, was "maap_jupyter_server_extension-1.0.1.tar", last modified: Mon Jun  5 22:16:31 2023, max compression
```

## Comparing `maap_jupyter_server_extension-1.0.0.tar` & `maap_jupyter_server_extension-1.0.1.tar`

### file list

```diff
@@ -1,49 +1,45 @@
-drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-03-30 22:34:34.747537 maap_jupyter_server_extension-1.0.0/
--rw-r--r--   0 mlucas     (502) staff       (20)       86 2022-07-22 16:01:37.000000 maap_jupyter_server_extension-1.0.0/CHANGELOG.md
--rw-r--r--   0 mlucas     (502) staff       (20)    10988 2023-02-13 22:24:25.000000 maap_jupyter_server_extension-1.0.0/LICENSE
--rw-r--r--   0 mlucas     (502) staff       (20)      512 2022-09-16 17:04:10.000000 maap_jupyter_server_extension-1.0.0/MANIFEST.in
--rw-r--r--   0 mlucas     (502) staff       (20)     4834 2023-03-30 22:34:34.746518 maap_jupyter_server_extension-1.0.0/PKG-INFO
--rw-r--r--   0 mlucas     (502) staff       (20)     3763 2023-01-20 01:31:26.000000 maap_jupyter_server_extension-1.0.0/README.md
--rw-r--r--   0 mlucas     (502) staff       (20)      211 2022-08-17 17:39:04.000000 maap_jupyter_server_extension-1.0.0/conftest.py
--rw-r--r--   0 mlucas     (502) staff       (20)      209 2022-08-17 17:39:15.000000 maap_jupyter_server_extension-1.0.0/install.json
-drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-03-30 22:34:34.645020 maap_jupyter_server_extension-1.0.0/jupyter-config/
-drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-03-30 22:34:34.679594 maap_jupyter_server_extension-1.0.0/jupyter-config/nb-config/
--rw-r--r--   0 mlucas     (502) staff       (20)      101 2022-08-17 17:42:45.000000 maap_jupyter_server_extension-1.0.0/jupyter-config/nb-config/dps_jupyter_server_extension.json
-drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-03-30 22:34:34.681940 maap_jupyter_server_extension-1.0.0/jupyter-config/server-config/
--rw-r--r--   0 mlucas     (502) staff       (20)       99 2022-08-17 17:42:45.000000 maap_jupyter_server_extension-1.0.0/jupyter-config/server-config/dps_jupyter_server_extension.json
-drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-03-30 22:34:34.689443 maap_jupyter_server_extension-1.0.0/jupyter_server_extension/
--rw-r--r--   0 mlucas     (502) staff       (20)     1007 2022-08-17 18:22:56.000000 maap_jupyter_server_extension-1.0.0/jupyter_server_extension/__init__.py
--rw-r--r--   0 mlucas     (502) staff       (20)      624 2022-08-17 18:21:56.000000 maap_jupyter_server_extension-1.0.0/jupyter_server_extension/_version.py
--rw-r--r--   0 mlucas     (502) staff       (20)    22318 2023-02-13 21:12:50.000000 maap_jupyter_server_extension-1.0.0/jupyter_server_extension/handlers.py
-drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-03-30 22:34:34.695025 maap_jupyter_server_extension-1.0.0/jupyter_server_extension/labextension/
--rw-r--r--   0 mlucas     (502) staff       (20)    21302 2023-03-30 22:33:24.000000 maap_jupyter_server_extension-1.0.0/jupyter_server_extension/labextension/build_log.json
--rw-r--r--   0 mlucas     (502) staff       (20)     2762 2023-03-30 22:33:25.000000 maap_jupyter_server_extension-1.0.0/jupyter_server_extension/labextension/package.json
-drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-03-30 22:34:34.715396 maap_jupyter_server_extension-1.0.0/jupyter_server_extension/labextension/static/
--rw-r--r--   0 mlucas     (502) staff       (20)     3767 2023-03-30 22:33:25.000000 maap_jupyter_server_extension-1.0.0/jupyter_server_extension/labextension/static/lib_index_js.b825374fb283016bd2c5.js
--rw-r--r--   0 mlucas     (502) staff       (20)     2449 2023-03-30 22:33:25.000000 maap_jupyter_server_extension-1.0.0/jupyter_server_extension/labextension/static/lib_index_js.b825374fb283016bd2c5.js.map
--rw-r--r--   0 mlucas     (502) staff       (20)    27859 2023-03-30 22:33:25.000000 maap_jupyter_server_extension-1.0.0/jupyter_server_extension/labextension/static/remoteEntry.a7294d496ffc3bc2f9ee.js
--rw-r--r--   0 mlucas     (502) staff       (20)    26770 2023-03-30 22:33:25.000000 maap_jupyter_server_extension-1.0.0/jupyter_server_extension/labextension/static/remoteEntry.a7294d496ffc3bc2f9ee.js.map
--rw-r--r--   0 mlucas     (502) staff       (20)      167 2023-03-30 22:33:24.000000 maap_jupyter_server_extension-1.0.0/jupyter_server_extension/labextension/static/style.js
--rw-r--r--   0 mlucas     (502) staff       (20)     4620 2023-03-30 22:33:25.000000 maap_jupyter_server_extension-1.0.0/jupyter_server_extension/labextension/static/style_index_js.7329fa0ca43a9baa0782.js
--rw-r--r--   0 mlucas     (502) staff       (20)     1817 2023-03-30 22:33:25.000000 maap_jupyter_server_extension-1.0.0/jupyter_server_extension/labextension/static/style_index_js.7329fa0ca43a9baa0782.js.map
--rw-r--r--   0 mlucas     (502) staff       (20)    12078 2023-03-30 22:33:25.000000 maap_jupyter_server_extension-1.0.0/jupyter_server_extension/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.0c791b6b3e0f57b64021.js
--rw-r--r--   0 mlucas     (502) staff       (20)    13820 2023-03-30 22:33:25.000000 maap_jupyter_server_extension-1.0.0/jupyter_server_extension/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.0c791b6b3e0f57b64021.js.map
-drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-03-30 22:34:34.729300 maap_jupyter_server_extension-1.0.0/maap_jupyter_server_extension.egg-info/
--rw-r--r--   0 mlucas     (502) staff       (20)     4834 2023-03-30 22:34:34.000000 maap_jupyter_server_extension-1.0.0/maap_jupyter_server_extension.egg-info/PKG-INFO
--rw-r--r--   0 mlucas     (502) staff       (20)     1749 2023-03-30 22:34:34.000000 maap_jupyter_server_extension-1.0.0/maap_jupyter_server_extension.egg-info/SOURCES.txt
--rw-r--r--   0 mlucas     (502) staff       (20)        1 2023-03-30 22:34:34.000000 maap_jupyter_server_extension-1.0.0/maap_jupyter_server_extension.egg-info/dependency_links.txt
--rw-r--r--   0 mlucas     (502) staff       (20)        1 2023-03-30 22:34:33.000000 maap_jupyter_server_extension-1.0.0/maap_jupyter_server_extension.egg-info/not-zip-safe
--rw-r--r--   0 mlucas     (502) staff       (20)       88 2023-03-30 22:34:34.000000 maap_jupyter_server_extension-1.0.0/maap_jupyter_server_extension.egg-info/requires.txt
--rw-r--r--   0 mlucas     (502) staff       (20)       25 2023-03-30 22:34:34.000000 maap_jupyter_server_extension-1.0.0/maap_jupyter_server_extension.egg-info/top_level.txt
--rw-r--r--   0 mlucas     (502) staff       (20)     2620 2023-03-30 20:42:42.000000 maap_jupyter_server_extension-1.0.0/package.json
--rw-r--r--   0 mlucas     (502) staff       (20)      631 2023-03-30 20:17:57.000000 maap_jupyter_server_extension-1.0.0/pyproject.toml
--rw-r--r--   0 mlucas     (502) staff       (20)       38 2023-03-30 22:34:34.748250 maap_jupyter_server_extension-1.0.0/setup.cfg
--rw-r--r--   0 mlucas     (502) staff       (20)     3431 2023-03-30 22:32:37.000000 maap_jupyter_server_extension-1.0.0/setup.py
-drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-03-30 22:34:34.733693 maap_jupyter_server_extension-1.0.0/src/
--rw-r--r--   0 mlucas     (502) staff       (20)     1111 2022-08-17 17:56:43.000000 maap_jupyter_server_extension-1.0.0/src/handler.ts
--rw-r--r--   0 mlucas     (502) staff       (20)      716 2022-08-17 17:56:43.000000 maap_jupyter_server_extension-1.0.0/src/index.ts
-drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-03-30 22:34:34.742259 maap_jupyter_server_extension-1.0.0/style/
--rw-r--r--   0 mlucas     (502) staff       (20)      138 2022-07-22 16:01:37.000000 maap_jupyter_server_extension-1.0.0/style/base.css
--rw-r--r--   0 mlucas     (502) staff       (20)       25 2022-07-22 16:01:37.000000 maap_jupyter_server_extension-1.0.0/style/index.css
--rw-r--r--   0 mlucas     (502) staff       (20)       21 2022-07-22 16:01:37.000000 maap_jupyter_server_extension-1.0.0/style/index.js
--rw-r--r--   0 mlucas     (502) staff       (20)      537 2023-03-30 20:28:25.000000 maap_jupyter_server_extension-1.0.0/tsconfig.json
+drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-05 22:16:31.376349 maap_jupyter_server_extension-1.0.1/
+-rw-r--r--   0 mlucas     (502) staff       (20)       86 2022-07-22 16:01:37.000000 maap_jupyter_server_extension-1.0.1/CHANGELOG.md
+-rw-r--r--   0 mlucas     (502) staff       (20)    10988 2023-02-13 22:24:25.000000 maap_jupyter_server_extension-1.0.1/LICENSE
+-rw-r--r--   0 mlucas     (502) staff       (20)      512 2022-09-16 17:04:10.000000 maap_jupyter_server_extension-1.0.1/MANIFEST.in
+-rw-r--r--   0 mlucas     (502) staff       (20)     4834 2023-06-05 22:16:31.376021 maap_jupyter_server_extension-1.0.1/PKG-INFO
+-rw-r--r--   0 mlucas     (502) staff       (20)     3763 2023-01-20 01:31:26.000000 maap_jupyter_server_extension-1.0.1/README.md
+-rw-r--r--   0 mlucas     (502) staff       (20)      211 2022-08-17 17:39:04.000000 maap_jupyter_server_extension-1.0.1/conftest.py
+-rw-r--r--   0 mlucas     (502) staff       (20)      209 2022-08-17 17:39:15.000000 maap_jupyter_server_extension-1.0.1/install.json
+drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-05 22:16:31.347484 maap_jupyter_server_extension-1.0.1/jupyter-config/
+drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-05 22:16:31.355713 maap_jupyter_server_extension-1.0.1/jupyter-config/nb-config/
+-rw-r--r--   0 mlucas     (502) staff       (20)      101 2022-08-17 17:42:45.000000 maap_jupyter_server_extension-1.0.1/jupyter-config/nb-config/dps_jupyter_server_extension.json
+drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-05 22:16:31.356643 maap_jupyter_server_extension-1.0.1/jupyter-config/server-config/
+-rw-r--r--   0 mlucas     (502) staff       (20)       99 2022-08-17 17:42:45.000000 maap_jupyter_server_extension-1.0.1/jupyter-config/server-config/dps_jupyter_server_extension.json
+drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-05 22:16:31.359655 maap_jupyter_server_extension-1.0.1/jupyter_server_extension/
+-rw-r--r--   0 mlucas     (502) staff       (20)     1007 2022-08-17 18:22:56.000000 maap_jupyter_server_extension-1.0.1/jupyter_server_extension/__init__.py
+-rw-r--r--   0 mlucas     (502) staff       (20)      624 2022-08-17 18:21:56.000000 maap_jupyter_server_extension-1.0.1/jupyter_server_extension/_version.py
+-rw-r--r--   0 mlucas     (502) staff       (20)    22639 2023-06-05 20:49:32.000000 maap_jupyter_server_extension-1.0.1/jupyter_server_extension/handlers.py
+drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-05 22:16:31.361130 maap_jupyter_server_extension-1.0.1/jupyter_server_extension/labextension/
+-rw-r--r--   0 mlucas     (502) staff       (20)     2885 2023-06-05 22:08:16.000000 maap_jupyter_server_extension-1.0.1/jupyter_server_extension/labextension/package.json
+drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-05 22:16:31.369512 maap_jupyter_server_extension-1.0.1/jupyter_server_extension/labextension/static/
+-rw-r--r--   0 mlucas     (502) staff       (20)     3524 2023-06-05 22:08:16.000000 maap_jupyter_server_extension-1.0.1/jupyter_server_extension/labextension/static/747.4ce08d0080c49e3989d8.js
+-rw-r--r--   0 mlucas     (502) staff       (20)      904 2023-06-05 22:08:16.000000 maap_jupyter_server_extension-1.0.1/jupyter_server_extension/labextension/static/763.c8afe390b9ba053ca78e.js
+-rw-r--r--   0 mlucas     (502) staff       (20)     6490 2023-06-05 22:08:16.000000 maap_jupyter_server_extension-1.0.1/jupyter_server_extension/labextension/static/remoteEntry.fbf9e31991f55b086f94.js
+-rw-r--r--   0 mlucas     (502) staff       (20)      167 2023-06-05 22:08:15.000000 maap_jupyter_server_extension-1.0.1/jupyter_server_extension/labextension/static/style.js
+-rw-r--r--   0 mlucas     (502) staff       (20)     2452 2023-06-05 22:08:16.000000 maap_jupyter_server_extension-1.0.1/jupyter_server_extension/labextension/static/third-party-licenses.json
+drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-05 22:16:31.372658 maap_jupyter_server_extension-1.0.1/maap_jupyter_server_extension.egg-info/
+-rw-r--r--   0 mlucas     (502) staff       (20)     4834 2023-06-05 22:16:31.000000 maap_jupyter_server_extension-1.0.1/maap_jupyter_server_extension.egg-info/PKG-INFO
+-rw-r--r--   0 mlucas     (502) staff       (20)     1154 2023-06-05 22:16:31.000000 maap_jupyter_server_extension-1.0.1/maap_jupyter_server_extension.egg-info/SOURCES.txt
+-rw-r--r--   0 mlucas     (502) staff       (20)        1 2023-06-05 22:16:31.000000 maap_jupyter_server_extension-1.0.1/maap_jupyter_server_extension.egg-info/dependency_links.txt
+-rw-r--r--   0 mlucas     (502) staff       (20)        1 2023-06-05 22:16:30.000000 maap_jupyter_server_extension-1.0.1/maap_jupyter_server_extension.egg-info/not-zip-safe
+-rw-r--r--   0 mlucas     (502) staff       (20)       88 2023-06-05 22:16:31.000000 maap_jupyter_server_extension-1.0.1/maap_jupyter_server_extension.egg-info/requires.txt
+-rw-r--r--   0 mlucas     (502) staff       (20)       25 2023-06-05 22:16:31.000000 maap_jupyter_server_extension-1.0.1/maap_jupyter_server_extension.egg-info/top_level.txt
+-rw-r--r--   0 mlucas     (502) staff       (20)     2748 2023-06-05 22:12:27.000000 maap_jupyter_server_extension-1.0.1/package.json
+-rw-r--r--   0 mlucas     (502) staff       (20)      631 2023-03-30 20:17:57.000000 maap_jupyter_server_extension-1.0.1/pyproject.toml
+-rw-r--r--   0 mlucas     (502) staff       (20)       38 2023-06-05 22:16:31.376452 maap_jupyter_server_extension-1.0.1/setup.cfg
+-rw-r--r--   0 mlucas     (502) staff       (20)     3431 2023-06-05 22:15:51.000000 maap_jupyter_server_extension-1.0.1/setup.py
+drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-05 22:16:31.373703 maap_jupyter_server_extension-1.0.1/src/
+-rw-r--r--   0 mlucas     (502) staff       (20)     1111 2022-08-17 17:56:43.000000 maap_jupyter_server_extension-1.0.1/src/handler.ts
+-rw-r--r--   0 mlucas     (502) staff       (20)      716 2022-08-17 17:56:43.000000 maap_jupyter_server_extension-1.0.1/src/index.ts
+drwxr-xr-x   0 mlucas     (502) staff       (20)        0 2023-06-05 22:16:31.375504 maap_jupyter_server_extension-1.0.1/style/
+-rw-r--r--   0 mlucas     (502) staff       (20)      138 2022-07-22 16:01:37.000000 maap_jupyter_server_extension-1.0.1/style/base.css
+-rw-r--r--   0 mlucas     (502) staff       (20)       25 2022-07-22 16:01:37.000000 maap_jupyter_server_extension-1.0.1/style/index.css
+-rw-r--r--   0 mlucas     (502) staff       (20)       21 2022-07-22 16:01:37.000000 maap_jupyter_server_extension-1.0.1/style/index.js
+-rw-r--r--   0 mlucas     (502) staff       (20)      669 2023-06-05 20:12:23.000000 maap_jupyter_server_extension-1.0.1/tsconfig.json
+-rw-r--r--   0 mlucas     (502) staff       (20)   223606 2023-06-05 22:07:59.000000 maap_jupyter_server_extension-1.0.1/yarn.lock
```

### Comparing `maap_jupyter_server_extension-1.0.0/LICENSE` & `maap_jupyter_server_extension-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.0.0/MANIFEST.in` & `maap_jupyter_server_extension-1.0.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.0.0/PKG-INFO` & `maap_jupyter_server_extension-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maap_jupyter_server_extension
-Version: 1.0.0
+Version: 1.0.1
 Summary: A JupyterLab extension.
 Home-page: https://github.com/MAAP-Project/jupyter-server-extension
 Author: Marjorie Lucas
 Author-email: marjorie.j.lucas@jpl.nasa.gov
 License: Apache 2.0
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `maap_jupyter_server_extension-1.0.0/README.md` & `maap_jupyter_server_extension-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.0.0/jupyter_server_extension/__init__.py` & `maap_jupyter_server_extension-1.0.1/jupyter_server_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.0.0/jupyter_server_extension/_version.py` & `maap_jupyter_server_extension-1.0.1/jupyter_server_extension/_version.py`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.0.0/jupyter_server_extension/handlers.py` & `maap_jupyter_server_extension-1.0.1/jupyter_server_extension/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from maap.maap import MAAP
 import functools
 import os
 import xml.etree.ElementTree as ET
 import xmltodict
 import logging
 import requests
+import yaml
 
 logging.basicConfig(format='%(asctime)s %(message)s')
 
 @functools.lru_cache(maxsize=128)
 def get_maap_config(host):
     print(os.environ)
     path_to_json = os.path.join(os.path.dirname(os.path.abspath(__file__)), '..', os.environ['ENVIRONMENTS_FILE_PATH'])
@@ -544,14 +545,33 @@
         )
         print(r.text)
 
         resp = json.loads(r.text)   
         self.finish({"status_code":200, "message": "success", "url":resp['url']})
 
 
+class CreateFileHandler(IPythonHandler):
+    def get(self):
+
+        file_name = self.get_argument("fileName")
+        data = self.get_argument("data")
+
+        algo = json.loads(data)
+        print(algo)
+
+        try:
+            print("Attempting to create file.")
+            with open(file_name, 'w') as f:
+                yaml.dump(algo, f)
+                # f.write(yaml.dump(data))
+        except:
+            print("Failed to create file.")
+            self.finish()
+
+
 def setup_handlers(web_app):
     host_pattern = ".*$"
 
     base_url = web_app.settings["base_url"]
 
     # DPS
     web_app.add_handlers(host_pattern, [(url_path_join(base_url, "jupyter-server-extension", "get_example"), RouteHandler)])
@@ -563,26 +583,25 @@
     web_app.add_handlers(host_pattern, [(url_path_join(base_url, "jupyter-server-extension", "getCMRCollections"), GetCMRCollectionsHandler)])
     web_app.add_handlers(host_pattern, [(url_path_join(base_url, "jupyter-server-extension", "listUserJobs"), ListUserJobsHandler)])
     web_app.add_handlers(host_pattern, [(url_path_join(base_url, "jupyter-server-extension", "submitJob"), SubmitJobHandler)])
     web_app.add_handlers(host_pattern, [(url_path_join(base_url, "jupyter-server-extension", "getJobStatus"), GetJobStatusHandler)])
     web_app.add_handlers(host_pattern, [(url_path_join(base_url, "jupyter-server-extension", "getJobResult"), GetJobResultHandler)])
     web_app.add_handlers(host_pattern, [(url_path_join(base_url, "jupyter-server-extension", "getJobMetrics"), GetJobMetricsHandler)])
 
-    # MAAPSEC
-    # web_app.add_handlers(host_pattern, [(url_path_join(base_url, "jupyter-server-extension", "maapsec", "environment"), MaapEnvironmentHandler)])
-    # web_app.add_handlers(host_pattern, [(url_path_join(base_url, "jupyter-server-extension", "maapsec", "login"), MaapLoginHandler)])
-
-    # EDSC
-    web_app.add_handlers(host_pattern, [(url_path_join(base_url, "jupyter-server-extension", "edsc", "getGranules"), GetGranulesHandler)])
-    web_app.add_handlers(host_pattern, [(url_path_join(base_url, "jupyter-server-extension", "edsc", "getQuery"), GetQueryHandler)])
-    web_app.add_handlers(host_pattern, [(url_path_join(base_url, "jupyter-server-extension", "edsc"), IFrameHandler, {'welcome': welcome, 'sites': sites}), (url_path_join(base_url, 'jupyter-server-extension/edsc/proxy'), IFrameProxyHandler)])
-
     # USER WORKSPACE MANAGEMENT
     web_app.add_handlers(host_pattern, [(url_path_join(base_url, "jupyter-server-extension", "uwm", "test"), RouteTestHandler)])
     web_app.add_handlers(host_pattern, [(url_path_join(base_url, "jupyter-server-extension", "uwm", "injectPublicKey"), InjectKeyHandler)])
     web_app.add_handlers(host_pattern, [(url_path_join(base_url, "jupyter-server-extension", "uwm", "getSSHInfo"), GetSSHInfoHandler)])
     web_app.add_handlers(host_pattern, [(url_path_join(base_url, "jupyter-server-extension", "uwm", "getSignedS3Url"), Presigneds3UrlHandler)])
 
+    web_app.add_handlers(host_pattern, [(url_path_join(base_url, "jupyter-server-extension", "createFile"), CreateFileHandler)])
+
+
+    # EDSC
+    web_app.add_handlers(host_pattern, [(url_path_join(base_url, "jupyter-server-extension", "edsc", "getGranules"), GetGranulesHandler)])
+    web_app.add_handlers(host_pattern, [(url_path_join(base_url, "jupyter-server-extension", "edsc", "getQuery"), GetQueryHandler)])
+    web_app.add_handlers(host_pattern, [(url_path_join(base_url, "jupyter-server-extension", "edsc"), IFrameHandler, {'welcome': welcome, 'sites': sites}), (url_path_join(base_url, 'jupyter-server-extension/edsc/proxy'), IFrameProxyHandler)])
+
 
 
     web_app.add_handlers(host_pattern, handlers)
```

### Comparing `maap_jupyter_server_extension-1.0.0/jupyter_server_extension/labextension/package.json` & `maap_jupyter_server_extension-1.0.1/jupyter_server_extension/labextension/package.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9578373015873015%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^3.6.4', '@jupyterlab/coreutils': '^5.6.4', "*

 * *                   "'@jupyterlab/services': '^6.6.4', '@jupyterlab/apputils': '^3.6.4', "*

 * *                   "'@jupyterlab/rendermime-interfaces': '^3.6.4', '@lumino/widgets': '^1.37.2'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.fbf9e31991f55b086f94.js'}}",*

 * * "'version'": "'1.0.1'"}*

```diff
@@ -3,17 +3,20 @@
         "email": "marjorie.j.lucas@jpl.nasa.gov",
         "name": "Marjorie Lucas"
     },
     "bugs": {
         "url": "https://github.com/MAAP-Project/jupyter-server-extension/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.6.1",
-        "@jupyterlab/coreutils": "^5.4.4",
-        "@jupyterlab/services": "^6.1.0"
+        "@jupyterlab/application": "^3.6.4",
+        "@jupyterlab/apputils": "^3.6.4",
+        "@jupyterlab/coreutils": "^5.6.4",
+        "@jupyterlab/rendermime-interfaces": "^3.6.4",
+        "@jupyterlab/services": "^6.6.4",
+        "@lumino/widgets": "^1.37.2"
     },
     "description": "A JupyterLab extension.",
     "devDependencies": {
         "@babel/core": "^7.0.0",
         "@babel/preset-env": "^7.0.0",
         "@jupyterlab/builder": "^3.1.0",
         "@types/node": "^16.14.2",
@@ -37,15 +40,15 @@
                 "jlpm clean:all"
             ]
         }
     },
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.a7294d496ffc3bc2f9ee.js",
+            "load": "static/remoteEntry.fbf9e31991f55b086f94.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyter_server_extension"
                 },
@@ -90,9 +93,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "1.0.0"
+    "version": "1.0.1"
 }
```

### Comparing `maap_jupyter_server_extension-1.0.0/maap_jupyter_server_extension.egg-info/PKG-INFO` & `maap_jupyter_server_extension-1.0.1/maap_jupyter_server_extension.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maap-jupyter-server-extension
-Version: 1.0.0
+Version: 1.0.1
 Summary: A JupyterLab extension.
 Home-page: https://github.com/MAAP-Project/jupyter-server-extension
 Author: Marjorie Lucas
 Author-email: marjorie.j.lucas@jpl.nasa.gov
 License: Apache 2.0
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
```

### Comparing `maap_jupyter_server_extension-1.0.0/package.json` & `maap_jupyter_server_extension-1.0.1/package.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9345238095238095%*

 * *Differences: {"'dependencies'": "{'@jupyterlab/application': '^3.6.4', '@jupyterlab/coreutils': '^5.6.4', "*

 * *                   "'@jupyterlab/services': '^6.6.4', '@jupyterlab/apputils': '^3.6.4', "*

 * *                   "'@jupyterlab/rendermime-interfaces': '^3.6.4', '@lumino/widgets': '^1.37.2'}",*

 * * "'name'": "'maap-jupyter-server-extension'",*

 * * "'version'": "'1.0.1'"}*

```diff
@@ -3,17 +3,20 @@
         "email": "marjorie.j.lucas@jpl.nasa.gov",
         "name": "Marjorie Lucas"
     },
     "bugs": {
         "url": "https://github.com/MAAP-Project/jupyter-server-extension/issues"
     },
     "dependencies": {
-        "@jupyterlab/application": "^3.6.1",
-        "@jupyterlab/coreutils": "^5.4.4",
-        "@jupyterlab/services": "^6.1.0"
+        "@jupyterlab/application": "^3.6.4",
+        "@jupyterlab/apputils": "^3.6.4",
+        "@jupyterlab/coreutils": "^5.6.4",
+        "@jupyterlab/rendermime-interfaces": "^3.6.4",
+        "@jupyterlab/services": "^6.6.4",
+        "@lumino/widgets": "^1.37.2"
     },
     "description": "A JupyterLab extension.",
     "devDependencies": {
         "@babel/core": "^7.0.0",
         "@babel/preset-env": "^7.0.0",
         "@jupyterlab/builder": "^3.1.0",
         "@types/node": "^16.14.2",
@@ -55,15 +58,15 @@
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "Apache 2.0",
     "main": "lib/index.js",
-    "name": "jupyter-server-extension",
+    "name": "maap-jupyter-server-extension",
     "publishConfig": {
         "access": "public"
     },
     "repository": {
         "type": "git",
         "url": "https://github.com/MAAP-Project/jupyter-server-extension.git"
     },
@@ -85,9 +88,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "1.0.0"
+    "version": "1.0.1"
 }
```

### Comparing `maap_jupyter_server_extension-1.0.0/pyproject.toml` & `maap_jupyter_server_extension-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.0.0/setup.py` & `maap_jupyter_server_extension-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.0.0/src/handler.ts` & `maap_jupyter_server_extension-1.0.1/src/handler.ts`

 * *Files identical despite different names*

### Comparing `maap_jupyter_server_extension-1.0.0/src/index.ts` & `maap_jupyter_server_extension-1.0.1/src/index.ts`

 * *Files identical despite different names*

