# Comparing `tmp/tab2neo-1.3.0.2.tar.gz` & `tmp/tab2neo-1.3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tab2neo-1.3.0.2.tar", last modified: Mon Jun  5 09:34:16 2023, max compression
+gzip compressed data, was "tab2neo-1.3.0.3.tar", last modified: Tue Jun  6 15:02:14 2023, max compression
```

## Comparing `tab2neo-1.3.0.2.tar` & `tab2neo-1.3.0.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-05 09:34:16.363385 tab2neo-1.3.0.2/
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    11357 2023-04-21 05:47:21.000000 tab2neo-1.3.0.2/LICENSE
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    11844 2023-06-05 09:34:16.363385 tab2neo-1.3.0.2/PKG-INFO
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     5418 2023-06-05 07:59:59.000000 tab2neo-1.3.0.2/README.md
-drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-05 09:34:16.343385 tab2neo-1.3.0.2/data_loaders/
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)      241 2023-04-21 05:47:21.000000 tab2neo-1.3.0.2/data_loaders/__init__.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     3401 2023-04-21 05:47:21.000000 tab2neo-1.3.0.2/data_loaders/azure_data_loader.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    18843 2023-04-27 08:50:20.000000 tab2neo-1.3.0.2/data_loaders/file_data_loader.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     1492 2023-04-21 05:47:21.000000 tab2neo-1.3.0.2/data_loaders/hive_data_loader.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     1157 2023-04-21 05:47:21.000000 tab2neo-1.3.0.2/data_loaders/sql_server_data_loader.py
-drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-05 09:34:16.343385 tab2neo-1.3.0.2/data_providers/
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       54 2023-04-21 05:47:21.000000 tab2neo-1.3.0.2/data_providers/__init__.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    10972 2023-06-05 07:59:59.000000 tab2neo-1.3.0.2/data_providers/data_provider.py
-drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-05 09:34:16.351385 tab2neo-1.3.0.2/derivation_method/
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)      229 2023-06-05 07:59:59.000000 tab2neo-1.3.0.2/derivation_method/__init__.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)   103937 2023-06-05 09:34:07.000000 tab2neo-1.3.0.2/derivation_method/action.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    68853 2023-06-05 07:59:59.000000 tab2neo-1.3.0.2/derivation_method/derivation_method.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     3784 2023-06-05 07:59:59.000000 tab2neo-1.3.0.2/derivation_method/method.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     3223 2023-06-05 07:59:59.000000 tab2neo-1.3.0.2/derivation_method/predict_links.cql
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     1043 2023-06-05 07:59:59.000000 tab2neo-1.3.0.2/derivation_method/predict_output_classes.cql
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    48787 2023-06-05 07:59:59.000000 tab2neo-1.3.0.2/derivation_method/super_method.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    10250 2023-06-05 07:59:59.000000 tab2neo-1.3.0.2/derivation_method/utils.py
-drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-05 09:34:16.351385 tab2neo-1.3.0.2/logger/
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)        0 2023-04-21 05:47:21.000000 tab2neo-1.3.0.2/logger/__init__.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     1217 2023-04-21 05:47:21.000000 tab2neo-1.3.0.2/logger/logger.py
-drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-05 09:34:16.355385 tab2neo-1.3.0.2/model_appliers/
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       53 2023-04-21 05:47:21.000000 tab2neo-1.3.0.2/model_appliers/__init__.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    29312 2023-06-05 07:59:59.000000 tab2neo-1.3.0.2/model_appliers/model_applier.py
-drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-05 09:34:16.355385 tab2neo-1.3.0.2/model_managers/
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       53 2023-04-21 05:47:21.000000 tab2neo-1.3.0.2/model_managers/__init__.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    55794 2023-06-05 07:59:59.000000 tab2neo-1.3.0.2/model_managers/model_manager.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)      103 2023-04-21 05:47:21.000000 tab2neo-1.3.0.2/pyproject.toml
-drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-05 09:34:16.359385 tab2neo-1.3.0.2/query_builders/
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       53 2023-04-21 05:47:21.000000 tab2neo-1.3.0.2/query_builders/__init__.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    40776 2023-04-27 08:50:20.000000 tab2neo-1.3.0.2/query_builders/query_builder.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       38 2023-06-05 09:34:16.363385 tab2neo-1.3.0.2/setup.cfg
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     2318 2023-06-05 09:34:07.000000 tab2neo-1.3.0.2/setup.py
-drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-05 09:34:16.363385 tab2neo-1.3.0.2/tab2neo.egg-info/
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    11844 2023-06-05 09:34:16.000000 tab2neo-1.3.0.2/tab2neo.egg-info/PKG-INFO
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)      933 2023-06-05 09:34:16.000000 tab2neo-1.3.0.2/tab2neo.egg-info/SOURCES.txt
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)        1 2023-06-05 09:34:16.000000 tab2neo-1.3.0.2/tab2neo.egg-info/dependency_links.txt
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)      544 2023-06-05 09:34:16.000000 tab2neo-1.3.0.2/tab2neo.egg-info/requires.txt
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       98 2023-06-05 09:34:16.000000 tab2neo-1.3.0.2/tab2neo.egg-info/top_level.txt
-drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-05 09:34:16.363385 tab2neo-1.3.0.2/tests/
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    11269 2023-06-05 07:59:59.000000 tab2neo-1.3.0.2/tests/test_comparison_utilities.py
+drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-06 15:02:14.883385 tab2neo-1.3.0.3/
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    11357 2023-06-06 14:59:45.000000 tab2neo-1.3.0.3/LICENSE
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    11844 2023-06-06 15:02:14.879385 tab2neo-1.3.0.3/PKG-INFO
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     5418 2023-06-06 14:59:45.000000 tab2neo-1.3.0.3/README.md
+drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-06 15:02:14.863385 tab2neo-1.3.0.3/data_loaders/
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)      241 2023-06-06 14:59:45.000000 tab2neo-1.3.0.3/data_loaders/__init__.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     3401 2023-06-06 14:59:45.000000 tab2neo-1.3.0.3/data_loaders/azure_data_loader.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    18843 2023-06-06 14:59:45.000000 tab2neo-1.3.0.3/data_loaders/file_data_loader.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     1492 2023-06-06 14:59:45.000000 tab2neo-1.3.0.3/data_loaders/hive_data_loader.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     1157 2023-06-06 14:59:45.000000 tab2neo-1.3.0.3/data_loaders/sql_server_data_loader.py
+drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-06 15:02:14.863385 tab2neo-1.3.0.3/data_providers/
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       54 2023-06-06 14:59:45.000000 tab2neo-1.3.0.3/data_providers/__init__.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    10972 2023-06-06 14:59:45.000000 tab2neo-1.3.0.3/data_providers/data_provider.py
+drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-06 15:02:14.867385 tab2neo-1.3.0.3/derivation_method/
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)      229 2023-06-06 14:59:46.000000 tab2neo-1.3.0.3/derivation_method/__init__.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)   104146 2023-06-06 14:59:46.000000 tab2neo-1.3.0.3/derivation_method/action.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    68853 2023-06-06 14:59:46.000000 tab2neo-1.3.0.3/derivation_method/derivation_method.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     3784 2023-06-06 14:59:46.000000 tab2neo-1.3.0.3/derivation_method/method.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     3223 2023-06-06 14:59:46.000000 tab2neo-1.3.0.3/derivation_method/predict_links.cql
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     1043 2023-06-06 14:59:46.000000 tab2neo-1.3.0.3/derivation_method/predict_output_classes.cql
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    48787 2023-06-06 14:59:46.000000 tab2neo-1.3.0.3/derivation_method/super_method.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    10250 2023-06-06 14:59:46.000000 tab2neo-1.3.0.3/derivation_method/utils.py
+drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-06 15:02:14.867385 tab2neo-1.3.0.3/logger/
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)        0 2023-06-06 14:59:46.000000 tab2neo-1.3.0.3/logger/__init__.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     1217 2023-06-06 14:59:46.000000 tab2neo-1.3.0.3/logger/logger.py
+drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-06 15:02:14.871385 tab2neo-1.3.0.3/model_appliers/
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       53 2023-06-06 14:59:46.000000 tab2neo-1.3.0.3/model_appliers/__init__.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    29312 2023-06-06 14:59:46.000000 tab2neo-1.3.0.3/model_appliers/model_applier.py
+drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-06 15:02:14.871385 tab2neo-1.3.0.3/model_managers/
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       53 2023-06-06 14:59:46.000000 tab2neo-1.3.0.3/model_managers/__init__.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    55794 2023-06-06 14:59:46.000000 tab2neo-1.3.0.3/model_managers/model_manager.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)      103 2023-06-06 14:59:46.000000 tab2neo-1.3.0.3/pyproject.toml
+drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-06 15:02:14.875385 tab2neo-1.3.0.3/query_builders/
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       53 2023-06-06 14:59:46.000000 tab2neo-1.3.0.3/query_builders/__init__.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    40776 2023-06-06 14:59:46.000000 tab2neo-1.3.0.3/query_builders/query_builder.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       38 2023-06-06 15:02:14.883385 tab2neo-1.3.0.3/setup.cfg
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     2318 2023-06-06 14:59:46.000000 tab2neo-1.3.0.3/setup.py
+drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-06 15:02:14.879385 tab2neo-1.3.0.3/tab2neo.egg-info/
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    11844 2023-06-06 15:02:14.000000 tab2neo-1.3.0.3/tab2neo.egg-info/PKG-INFO
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)      933 2023-06-06 15:02:14.000000 tab2neo-1.3.0.3/tab2neo.egg-info/SOURCES.txt
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)        1 2023-06-06 15:02:14.000000 tab2neo-1.3.0.3/tab2neo.egg-info/dependency_links.txt
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)      544 2023-06-06 15:02:14.000000 tab2neo-1.3.0.3/tab2neo.egg-info/requires.txt
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       98 2023-06-06 15:02:14.000000 tab2neo-1.3.0.3/tab2neo.egg-info/top_level.txt
+drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-06 15:02:14.879385 tab2neo-1.3.0.3/tests/
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    11269 2023-06-06 14:59:46.000000 tab2neo-1.3.0.3/tests/test_comparison_utilities.py
```

### Comparing `tab2neo-1.3.0.2/LICENSE` & `tab2neo-1.3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.2/PKG-INFO` & `tab2neo-1.3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tab2neo
-Version: 1.3.0.2
+Version: 1.3.0.3
 Summary: Clinical Linked Data: High-level Python classes to load, model and reshape tabular data imported into Neo4j database
 Home-page: UNKNOWN
 Author: Alexey Kuznetsov
 License:                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
```

### Comparing `tab2neo-1.3.0.2/README.md` & `tab2neo-1.3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.2/data_loaders/azure_data_loader.py` & `tab2neo-1.3.0.3/data_loaders/azure_data_loader.py`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.2/data_loaders/file_data_loader.py` & `tab2neo-1.3.0.3/data_loaders/file_data_loader.py`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.2/data_loaders/hive_data_loader.py` & `tab2neo-1.3.0.3/data_loaders/hive_data_loader.py`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.2/data_loaders/sql_server_data_loader.py` & `tab2neo-1.3.0.3/data_loaders/sql_server_data_loader.py`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.2/data_providers/data_provider.py` & `tab2neo-1.3.0.3/data_providers/data_provider.py`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.2/derivation_method/action.py` & `tab2neo-1.3.0.3/derivation_method/action.py`

 * *Files 1% similar despite different names*

```diff
@@ -1099,14 +1099,19 @@
         # check if func and params both have values that are not None
         assert all([api_packet[i] for i in ["func", "params"]])
 
         # REQUIRES THE TWO ENVIRONMENT VARIABLES BELOW
         api_url = os.environ.get("CLD_API_HOST")
         api_auth = os.getenv('CLD_API_AUTH')
 
+        if "items" not in api_url:
+            api_url = api_url+"items/" if api_url.endswith('/') else api_url+"/items/"
+        else:
+            api_url = api_url if api_url.endswith('/') else api_url+"/"
+
         logger.info(f"calling api at {api_url} with function: {self.meta.get('script')}")
         if self.meta.get("github_repo"):
             logger.info(
                 f"source code from: {github_base_url}/{self.meta.get('github_repo')}/"
                 f"{self.meta.get('repo_scripts_path')}"
             )
             logger.info(f'Using branch {github_branch}')
```

### Comparing `tab2neo-1.3.0.2/derivation_method/derivation_method.py` & `tab2neo-1.3.0.3/derivation_method/derivation_method.py`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.2/derivation_method/method.py` & `tab2neo-1.3.0.3/derivation_method/method.py`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.2/derivation_method/predict_links.cql` & `tab2neo-1.3.0.3/derivation_method/predict_links.cql`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.2/derivation_method/predict_output_classes.cql` & `tab2neo-1.3.0.3/derivation_method/predict_output_classes.cql`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.2/derivation_method/super_method.py` & `tab2neo-1.3.0.3/derivation_method/super_method.py`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.2/derivation_method/utils.py` & `tab2neo-1.3.0.3/derivation_method/utils.py`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.2/logger/logger.py` & `tab2neo-1.3.0.3/logger/logger.py`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.2/model_appliers/model_applier.py` & `tab2neo-1.3.0.3/model_appliers/model_applier.py`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.2/model_managers/model_manager.py` & `tab2neo-1.3.0.3/model_managers/model_manager.py`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.2/query_builders/query_builder.py` & `tab2neo-1.3.0.3/query_builders/query_builder.py`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.2/setup.py` & `tab2neo-1.3.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
             print('Dependency to a git repository should have the format:')
             print('git+ssh://git@github.com/xxxxx/xxxxxx#egg=package_name')
     else:
         required.append(line)
 
 setuptools.setup(
     name="tab2neo",                         # This is the name of the package
-    version="1.3.0.2",                      # Release.Major Feature.Minor Feature.Bug Fix
+    version="1.3.0.3",                      # Release.Major Feature.Minor Feature.Bug Fix
     author="Alexey Kuznetsov",              # Full name of the author
     description="Clinical Linked Data: High-level Python classes to load, model and reshape tabular data imported into Neo4j database",
     long_description="https://github.com/GSK-Biostatistics/tab2neo/blob/main/README.md",      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(include=[
         "logger",
         "analysis_metadata",
```

### Comparing `tab2neo-1.3.0.2/tab2neo.egg-info/PKG-INFO` & `tab2neo-1.3.0.3/tab2neo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tab2neo
-Version: 1.3.0.2
+Version: 1.3.0.3
 Summary: Clinical Linked Data: High-level Python classes to load, model and reshape tabular data imported into Neo4j database
 Home-page: UNKNOWN
 Author: Alexey Kuznetsov
 License:                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
```

### Comparing `tab2neo-1.3.0.2/tab2neo.egg-info/SOURCES.txt` & `tab2neo-1.3.0.3/tab2neo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.2/tab2neo.egg-info/requires.txt` & `tab2neo-1.3.0.3/tab2neo.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tab2neo-1.3.0.2/tests/test_comparison_utilities.py` & `tab2neo-1.3.0.3/tests/test_comparison_utilities.py`

 * *Files identical despite different names*

