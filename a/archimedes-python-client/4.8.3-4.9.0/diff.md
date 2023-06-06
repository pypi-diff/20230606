# Comparing `tmp/archimedes_python_client-4.8.3.tar.gz` & `tmp/archimedes_python_client-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archimedes_python_client-4.8.3.tar", max compression
+gzip compressed data, was "archimedes_python_client-4.9.0.tar", max compression
```

## Comparing `archimedes_python_client-4.8.3.tar` & `archimedes_python_client-4.9.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1884 2022-11-08 13:33:37.902415 archimedes_python_client-4.8.3/archimedes/__init__.py
--rw-r--r--   0        0        0     5005 2022-11-08 13:33:37.902415 archimedes_python_client-4.8.3/archimedes/auth.py
--rw-r--r--   0        0        0     2714 2022-11-08 13:33:37.902415 archimedes_python_client-4.8.3/archimedes/configuration.py
--rw-r--r--   0        0        0        0 2022-11-08 13:33:37.902415 archimedes_python_client-4.8.3/archimedes/data/__init__.py
--rw-r--r--   0        0        0        0 2022-11-08 13:33:37.902415 archimedes_python_client-4.8.3/archimedes/data/api/__init__.py
--rw-r--r--   0        0        0    11434 2022-11-08 13:33:37.902415 archimedes_python_client-4.8.3/archimedes/data/api/forecast.py
--rw-r--r--   0        0        0     7413 2022-11-08 13:33:37.902415 archimedes_python_client-4.8.3/archimedes/data/api/intraday.py
--rw-r--r--   0        0        0     3767 2022-11-08 13:33:37.902415 archimedes_python_client-4.8.3/archimedes/data/api/metadata.py
--rw-r--r--   0        0        0    10957 2022-11-08 13:33:37.902415 archimedes_python_client-4.8.3/archimedes/data/api/observation.py
--rw-r--r--   0        0        0     8897 2022-11-08 13:33:37.902415 archimedes_python_client-4.8.3/archimedes/data/api/prediction.py
--rw-r--r--   0        0        0     7025 2022-11-08 13:33:37.902415 archimedes_python_client-4.8.3/archimedes/data/api/rk_within_day.py
--rw-r--r--   0        0        0      163 2022-11-08 13:33:37.902415 archimedes_python_client-4.8.3/archimedes/data/common.py
--rw-r--r--   0        0        0      330 2022-11-08 13:33:37.902415 archimedes_python_client-4.8.3/archimedes/data/types.py
--rw-r--r--   0        0        0       62 2022-11-08 13:33:37.902415 archimedes_python_client-4.8.3/archimedes/testdata/__init__.py
--rw-r--r--   0        0        0        0 2022-11-08 13:33:37.902415 archimedes_python_client-4.8.3/archimedes/testdata/datasets/rkspot.csv
--rw-r--r--   0        0        0      829 2022-11-08 13:33:37.902415 archimedes_python_client-4.8.3/archimedes/testdata/testdata.py
--rw-r--r--   0        0        0      656 2022-11-08 13:33:37.902415 archimedes_python_client-4.8.3/archimedes/token_cache.py
--rw-r--r--   0        0        0       83 2022-11-08 13:33:37.902415 archimedes_python_client-4.8.3/archimedes/utils/__init__.py
--rw-r--r--   0        0        0     3326 2022-11-08 13:33:37.902415 archimedes_python_client-4.8.3/archimedes/utils/api_request.py
--rw-r--r--   0        0        0     1511 2022-11-08 13:33:37.902415 archimedes_python_client-4.8.3/archimedes/utils/date.py
--rw-r--r--   0        0        0      859 2022-11-08 13:33:37.902415 archimedes_python_client-4.8.3/archimedes/utils/environ_context.py
--rw-r--r--   0        0        0    10739 2022-11-08 13:33:37.902415 archimedes_python_client-4.8.3/archimedes/utils/format.py
--rw-r--r--   0        0        0       73 2022-11-08 13:33:37.902415 archimedes_python_client-4.8.3/archimedes/utils/split/__init__.py
--rw-r--r--   0        0        0     6694 2022-11-08 13:33:37.902415 archimedes_python_client-4.8.3/archimedes/utils/split/config.py
--rw-r--r--   0        0        0    10437 2022-11-08 13:33:37.902415 archimedes_python_client-4.8.3/archimedes/utils/split/split.py
--rw-r--r--   0        0        0     1796 2022-11-08 13:33:37.902415 archimedes_python_client-4.8.3/archimedes/utils/threaded_executor.py
--rw-r--r--   0        0        0      684 2022-11-08 13:33:37.902415 archimedes_python_client-4.8.3/pyproject.toml
--rw-r--r--   0        0        0      968 1970-01-01 00:00:00.000000 archimedes_python_client-4.8.3/setup.py
--rw-r--r--   0        0        0      768 1970-01-01 00:00:00.000000 archimedes_python_client-4.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1884 2022-11-10 16:26:48.546366 archimedes_python_client-4.9.0/archimedes/__init__.py
+-rw-r--r--   0        0        0     5005 2022-11-10 16:26:48.546366 archimedes_python_client-4.9.0/archimedes/auth.py
+-rw-r--r--   0        0        0     2714 2022-11-10 16:26:48.546366 archimedes_python_client-4.9.0/archimedes/configuration.py
+-rw-r--r--   0        0        0        0 2022-11-10 16:26:48.546366 archimedes_python_client-4.9.0/archimedes/data/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-10 16:26:48.546366 archimedes_python_client-4.9.0/archimedes/data/api/__init__.py
+-rw-r--r--   0        0        0    11434 2022-11-10 16:26:48.546366 archimedes_python_client-4.9.0/archimedes/data/api/forecast.py
+-rw-r--r--   0        0        0     7413 2022-11-10 16:26:48.546366 archimedes_python_client-4.9.0/archimedes/data/api/intraday.py
+-rw-r--r--   0        0        0     3767 2022-11-10 16:26:48.546366 archimedes_python_client-4.9.0/archimedes/data/api/metadata.py
+-rw-r--r--   0        0        0    10957 2022-11-10 16:26:48.546366 archimedes_python_client-4.9.0/archimedes/data/api/observation.py
+-rw-r--r--   0        0        0     8897 2022-11-10 16:26:48.546366 archimedes_python_client-4.9.0/archimedes/data/api/prediction.py
+-rw-r--r--   0        0        0     7025 2022-11-10 16:26:48.546366 archimedes_python_client-4.9.0/archimedes/data/api/rk_within_day.py
+-rw-r--r--   0        0        0      163 2022-11-10 16:26:48.550366 archimedes_python_client-4.9.0/archimedes/data/common.py
+-rw-r--r--   0        0        0      330 2022-11-10 16:26:48.550366 archimedes_python_client-4.9.0/archimedes/data/types.py
+-rw-r--r--   0        0        0       62 2022-11-10 16:26:48.550366 archimedes_python_client-4.9.0/archimedes/testdata/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-10 16:26:48.550366 archimedes_python_client-4.9.0/archimedes/testdata/datasets/rkspot.csv
+-rw-r--r--   0        0        0      829 2022-11-10 16:26:48.550366 archimedes_python_client-4.9.0/archimedes/testdata/testdata.py
+-rw-r--r--   0        0        0      656 2022-11-10 16:26:48.550366 archimedes_python_client-4.9.0/archimedes/token_cache.py
+-rw-r--r--   0        0        0       83 2022-11-10 16:26:48.550366 archimedes_python_client-4.9.0/archimedes/utils/__init__.py
+-rw-r--r--   0        0        0     3326 2022-11-10 16:26:48.550366 archimedes_python_client-4.9.0/archimedes/utils/api_request.py
+-rw-r--r--   0        0        0     1511 2022-11-10 16:26:48.550366 archimedes_python_client-4.9.0/archimedes/utils/date.py
+-rw-r--r--   0        0        0      859 2022-11-10 16:26:48.550366 archimedes_python_client-4.9.0/archimedes/utils/environ_context.py
+-rw-r--r--   0        0        0    10739 2022-11-10 16:26:48.550366 archimedes_python_client-4.9.0/archimedes/utils/format.py
+-rw-r--r--   0        0        0       73 2022-11-10 16:26:48.550366 archimedes_python_client-4.9.0/archimedes/utils/split/__init__.py
+-rw-r--r--   0        0        0     6694 2022-11-10 16:26:48.550366 archimedes_python_client-4.9.0/archimedes/utils/split/config.py
+-rw-r--r--   0        0        0    10437 2022-11-10 16:26:48.550366 archimedes_python_client-4.9.0/archimedes/utils/split/split.py
+-rw-r--r--   0        0        0     1796 2022-11-10 16:26:48.550366 archimedes_python_client-4.9.0/archimedes/utils/threaded_executor.py
+-rw-r--r--   0        0        0      684 2022-11-10 16:26:48.550366 archimedes_python_client-4.9.0/pyproject.toml
+-rw-r--r--   0        0        0      968 1970-01-01 00:00:00.000000 archimedes_python_client-4.9.0/setup.py
+-rw-r--r--   0        0        0      769 1970-01-01 00:00:00.000000 archimedes_python_client-4.9.0/PKG-INFO
```

### Comparing `archimedes_python_client-4.8.3/archimedes/__init__.py` & `archimedes_python_client-4.9.0/archimedes/__init__.py`

 * *Files identical despite different names*

### Comparing `archimedes_python_client-4.8.3/archimedes/auth.py` & `archimedes_python_client-4.9.0/archimedes/auth.py`

 * *Files identical despite different names*

### Comparing `archimedes_python_client-4.8.3/archimedes/configuration.py` & `archimedes_python_client-4.9.0/archimedes/configuration.py`

 * *Files identical despite different names*

### Comparing `archimedes_python_client-4.8.3/archimedes/data/api/forecast.py` & `archimedes_python_client-4.9.0/archimedes/data/api/forecast.py`

 * *Files identical despite different names*

### Comparing `archimedes_python_client-4.8.3/archimedes/data/api/intraday.py` & `archimedes_python_client-4.9.0/archimedes/data/api/intraday.py`

 * *Files identical despite different names*

### Comparing `archimedes_python_client-4.8.3/archimedes/data/api/metadata.py` & `archimedes_python_client-4.9.0/archimedes/data/api/metadata.py`

 * *Files identical despite different names*

### Comparing `archimedes_python_client-4.8.3/archimedes/data/api/observation.py` & `archimedes_python_client-4.9.0/archimedes/data/api/observation.py`

 * *Files identical despite different names*

### Comparing `archimedes_python_client-4.8.3/archimedes/data/api/prediction.py` & `archimedes_python_client-4.9.0/archimedes/data/api/prediction.py`

 * *Files identical despite different names*

### Comparing `archimedes_python_client-4.8.3/archimedes/data/api/rk_within_day.py` & `archimedes_python_client-4.9.0/archimedes/data/api/rk_within_day.py`

 * *Files identical despite different names*

### Comparing `archimedes_python_client-4.8.3/archimedes/testdata/testdata.py` & `archimedes_python_client-4.9.0/archimedes/testdata/testdata.py`

 * *Files identical despite different names*

### Comparing `archimedes_python_client-4.8.3/archimedes/token_cache.py` & `archimedes_python_client-4.9.0/archimedes/token_cache.py`

 * *Files identical despite different names*

### Comparing `archimedes_python_client-4.8.3/archimedes/utils/api_request.py` & `archimedes_python_client-4.9.0/archimedes/utils/api_request.py`

 * *Files identical despite different names*

### Comparing `archimedes_python_client-4.8.3/archimedes/utils/date.py` & `archimedes_python_client-4.9.0/archimedes/utils/date.py`

 * *Files identical despite different names*

### Comparing `archimedes_python_client-4.8.3/archimedes/utils/environ_context.py` & `archimedes_python_client-4.9.0/archimedes/utils/environ_context.py`

 * *Files identical despite different names*

### Comparing `archimedes_python_client-4.8.3/archimedes/utils/format.py` & `archimedes_python_client-4.9.0/archimedes/utils/format.py`

 * *Files identical despite different names*

### Comparing `archimedes_python_client-4.8.3/archimedes/utils/split/config.py` & `archimedes_python_client-4.9.0/archimedes/utils/split/config.py`

 * *Files identical despite different names*

### Comparing `archimedes_python_client-4.8.3/archimedes/utils/split/split.py` & `archimedes_python_client-4.9.0/archimedes/utils/split/split.py`

 * *Files identical despite different names*

### Comparing `archimedes_python_client-4.8.3/archimedes/utils/threaded_executor.py` & `archimedes_python_client-4.9.0/archimedes/utils/threaded_executor.py`

 * *Files identical despite different names*

### Comparing `archimedes_python_client-4.8.3/pyproject.toml` & `archimedes_python_client-4.9.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "archimedes-python-client"
-version = "4.8.3"
+version = "4.9.0"
 description = "The Python library for Archimedes"
 authors = ["Optimeering AS <dev@optimeering.com>"]
 license = "Apache-2.0"
 packages = [{include = "archimedes"}]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
+python = ">=3.9,<3.12"
 pandas = ">=1.0.5"
 requests = ">=2.27.0"
 msal = ">=1.10.0,<2.0.0"
 msal-extensions = "^1.0.0"
 retry = "^0.9.2"
 iteration-utilities = "^0.11.0"
 cachetools = "^5.2.0"
```

### Comparing `archimedes_python_client-4.8.3/setup.py` & `archimedes_python_client-4.9.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,23 +19,23 @@
  'msal>=1.10.0,<2.0.0',
  'pandas>=1.0.5',
  'requests>=2.27.0',
  'retry>=0.9.2,<0.10.0']
 
 setup_kwargs = {
     'name': 'archimedes-python-client',
-    'version': '4.8.3',
+    'version': '4.9.0',
     'description': 'The Python library for Archimedes',
     'long_description': 'None',
     'author': 'Optimeering AS',
     'author_email': 'dev@optimeering.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.11',
+    'python_requires': '>=3.9,<3.12',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `archimedes_python_client-4.8.3/PKG-INFO` & `archimedes_python_client-4.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: archimedes-python-client
-Version: 4.8.3
+Version: 4.9.0
 Summary: The Python library for Archimedes
 License: Apache-2.0
 Author: Optimeering AS
 Author-email: dev@optimeering.com
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cachetools (>=5.2.0,<6.0.0)
 Requires-Dist: iteration-utilities (>=0.11.0,<0.12.0)
 Requires-Dist: msal (>=1.10.0,<2.0.0)
 Requires-Dist: msal-extensions (>=1.0.0,<2.0.0)
 Requires-Dist: pandas (>=1.0.5)
 Requires-Dist: requests (>=2.27.0)
 Requires-Dist: retry (>=0.9.2,<0.10.0)
```

