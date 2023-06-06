# Comparing `tmp/neo4cdisc-1.0.5.2.tar.gz` & `tmp/neo4cdisc-1.0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neo4cdisc-1.0.5.2.tar", last modified: Mon Jun  5 09:35:14 2023, max compression
+gzip compressed data, was "neo4cdisc-1.0.5.3.tar", last modified: Tue Jun  6 15:03:19 2023, max compression
```

## Comparing `neo4cdisc-1.0.5.2.tar` & `neo4cdisc-1.0.5.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-05 09:35:14.499385 neo4cdisc-1.0.5.2/
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    11357 2023-04-21 05:47:21.000000 neo4cdisc-1.0.5.2/LICENSE
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    11783 2023-06-05 09:35:14.499385 neo4cdisc-1.0.5.2/PKG-INFO
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     1088 2023-04-21 05:47:21.000000 neo4cdisc-1.0.5.2/README.md
-drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-05 09:35:14.495385 neo4cdisc-1.0.5.2/cdisc_data_providers/
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       69 2023-04-21 05:47:21.000000 neo4cdisc-1.0.5.2/cdisc_data_providers/__init__.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    11169 2023-04-21 05:47:21.000000 neo4cdisc-1.0.5.2/cdisc_data_providers/sdtm_data_provider.py
-drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-05 09:35:14.495385 neo4cdisc-1.0.5.2/cdisc_model_managers/
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)      126 2023-04-21 05:47:21.000000 neo4cdisc-1.0.5.2/cdisc_model_managers/__init__.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     1044 2023-04-21 05:47:21.000000 neo4cdisc-1.0.5.2/cdisc_model_managers/cdisc_api.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    21929 2023-04-21 05:47:21.000000 neo4cdisc-1.0.5.2/cdisc_model_managers/cdisc_model_manager.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    18806 2023-06-05 08:26:54.000000 neo4cdisc-1.0.5.2/cdisc_model_managers/cdisc_standard_loader.py
-drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-05 09:35:14.499385 neo4cdisc-1.0.5.2/neo4cdisc.egg-info/
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    11783 2023-06-05 09:35:14.000000 neo4cdisc-1.0.5.2/neo4cdisc.egg-info/PKG-INFO
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)      531 2023-06-05 09:35:14.000000 neo4cdisc-1.0.5.2/neo4cdisc.egg-info/SOURCES.txt
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)        1 2023-06-05 09:35:14.000000 neo4cdisc-1.0.5.2/neo4cdisc.egg-info/dependency_links.txt
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       17 2023-06-05 09:35:14.000000 neo4cdisc-1.0.5.2/neo4cdisc.egg-info/requires.txt
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       42 2023-06-05 09:35:14.000000 neo4cdisc-1.0.5.2/neo4cdisc.egg-info/top_level.txt
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       38 2023-06-05 09:35:14.499385 neo4cdisc-1.0.5.2/setup.cfg
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     2172 2023-06-05 09:33:53.000000 neo4cdisc-1.0.5.2/setup.py
-drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-05 09:35:14.499385 neo4cdisc-1.0.5.2/tests/
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     2360 2023-04-21 05:47:21.000000 neo4cdisc-1.0.5.2/tests/test_cdisc_model_manager.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     7150 2023-04-21 05:47:21.000000 neo4cdisc-1.0.5.2/tests/test_sdtm_data_provider.py
--rw-rw-r--   0 ak956494  (1000) ak956494  (1000)      659 2023-04-21 05:47:21.000000 neo4cdisc-1.0.5.2/tests/test_sdtm_data_provider_dfcheck.py
+drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-06 15:03:19.103385 neo4cdisc-1.0.5.3/
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    11357 2023-04-21 05:47:21.000000 neo4cdisc-1.0.5.3/LICENSE
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    11783 2023-06-06 15:03:19.103385 neo4cdisc-1.0.5.3/PKG-INFO
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     1088 2023-04-21 05:47:21.000000 neo4cdisc-1.0.5.3/README.md
+drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-06 15:03:19.095385 neo4cdisc-1.0.5.3/cdisc_data_providers/
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       69 2023-04-21 05:47:21.000000 neo4cdisc-1.0.5.3/cdisc_data_providers/__init__.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    11169 2023-04-21 05:47:21.000000 neo4cdisc-1.0.5.3/cdisc_data_providers/sdtm_data_provider.py
+drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-06 15:03:19.099385 neo4cdisc-1.0.5.3/cdisc_model_managers/
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)      126 2023-04-21 05:47:21.000000 neo4cdisc-1.0.5.3/cdisc_model_managers/__init__.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     1044 2023-04-21 05:47:21.000000 neo4cdisc-1.0.5.3/cdisc_model_managers/cdisc_api.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    21929 2023-04-21 05:47:21.000000 neo4cdisc-1.0.5.3/cdisc_model_managers/cdisc_model_manager.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    18806 2023-06-05 08:26:54.000000 neo4cdisc-1.0.5.3/cdisc_model_managers/cdisc_standard_loader.py
+drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-06 15:03:19.103385 neo4cdisc-1.0.5.3/neo4cdisc.egg-info/
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)    11783 2023-06-06 15:03:18.000000 neo4cdisc-1.0.5.3/neo4cdisc.egg-info/PKG-INFO
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)      531 2023-06-06 15:03:19.000000 neo4cdisc-1.0.5.3/neo4cdisc.egg-info/SOURCES.txt
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)        1 2023-06-06 15:03:18.000000 neo4cdisc-1.0.5.3/neo4cdisc.egg-info/dependency_links.txt
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       17 2023-06-06 15:03:18.000000 neo4cdisc-1.0.5.3/neo4cdisc.egg-info/requires.txt
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       42 2023-06-06 15:03:18.000000 neo4cdisc-1.0.5.3/neo4cdisc.egg-info/top_level.txt
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)       38 2023-06-06 15:03:19.103385 neo4cdisc-1.0.5.3/setup.cfg
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     2172 2023-06-06 15:03:09.000000 neo4cdisc-1.0.5.3/setup.py
+drwxrwxr-x   0 ak956494  (1000) ak956494  (1000)        0 2023-06-06 15:03:19.103385 neo4cdisc-1.0.5.3/tests/
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     2360 2023-04-21 05:47:21.000000 neo4cdisc-1.0.5.3/tests/test_cdisc_model_manager.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)     7150 2023-04-21 05:47:21.000000 neo4cdisc-1.0.5.3/tests/test_sdtm_data_provider.py
+-rw-rw-r--   0 ak956494  (1000) ak956494  (1000)      659 2023-04-21 05:47:21.000000 neo4cdisc-1.0.5.3/tests/test_sdtm_data_provider_dfcheck.py
```

### Comparing `neo4cdisc-1.0.5.2/LICENSE` & `neo4cdisc-1.0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `neo4cdisc-1.0.5.2/PKG-INFO` & `neo4cdisc-1.0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neo4cdisc
-Version: 1.0.5.2
+Version: 1.0.5.3
 Summary: Clinical Linked Data: Example of loading the FDA CDISC pilot study into Neo4J using the tab2neo python package
 Home-page: UNKNOWN
 Author: Alexey Kuznetsov
 License:                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
```

### Comparing `neo4cdisc-1.0.5.2/README.md` & `neo4cdisc-1.0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `neo4cdisc-1.0.5.2/cdisc_data_providers/sdtm_data_provider.py` & `neo4cdisc-1.0.5.3/cdisc_data_providers/sdtm_data_provider.py`

 * *Files identical despite different names*

### Comparing `neo4cdisc-1.0.5.2/cdisc_model_managers/cdisc_api.py` & `neo4cdisc-1.0.5.3/cdisc_model_managers/cdisc_api.py`

 * *Files identical despite different names*

### Comparing `neo4cdisc-1.0.5.2/cdisc_model_managers/cdisc_model_manager.py` & `neo4cdisc-1.0.5.3/cdisc_model_managers/cdisc_model_manager.py`

 * *Files identical despite different names*

### Comparing `neo4cdisc-1.0.5.2/cdisc_model_managers/cdisc_standard_loader.py` & `neo4cdisc-1.0.5.3/cdisc_model_managers/cdisc_standard_loader.py`

 * *Files identical despite different names*

### Comparing `neo4cdisc-1.0.5.2/neo4cdisc.egg-info/PKG-INFO` & `neo4cdisc-1.0.5.3/neo4cdisc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neo4cdisc
-Version: 1.0.5.2
+Version: 1.0.5.3
 Summary: Clinical Linked Data: Example of loading the FDA CDISC pilot study into Neo4J using the tab2neo python package
 Home-page: UNKNOWN
 Author: Alexey Kuznetsov
 License:                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
```

### Comparing `neo4cdisc-1.0.5.2/neo4cdisc.egg-info/SOURCES.txt` & `neo4cdisc-1.0.5.3/neo4cdisc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neo4cdisc-1.0.5.2/setup.py` & `neo4cdisc-1.0.5.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             print('Dependency to a git repository should have the format:')
             print('git+ssh://git@github.com/xxxxx/xxxxxx#egg=package_name')
     else:
         required.append(line)
 
 setuptools.setup(
     name="neo4cdisc",                           # This is the name of the package
-    version="1.0.5.2",                      # Release.Major Feature.Minor Feature.Bug Fix
+    version="1.0.5.3",                      # Release.Major Feature.Minor Feature.Bug Fix
     author="Alexey Kuznetsov",              # Full name of the author
     description="Clinical Linked Data: Example of loading the FDA CDISC pilot study into Neo4J using the tab2neo python package",
     #long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(include=[
         "cdisc_model_managers",
         "cdisc_data_providers",
```

### Comparing `neo4cdisc-1.0.5.2/tests/test_cdisc_model_manager.py` & `neo4cdisc-1.0.5.3/tests/test_cdisc_model_manager.py`

 * *Files identical despite different names*

### Comparing `neo4cdisc-1.0.5.2/tests/test_sdtm_data_provider.py` & `neo4cdisc-1.0.5.3/tests/test_sdtm_data_provider.py`

 * *Files identical despite different names*

### Comparing `neo4cdisc-1.0.5.2/tests/test_sdtm_data_provider_dfcheck.py` & `neo4cdisc-1.0.5.3/tests/test_sdtm_data_provider_dfcheck.py`

 * *Files identical despite different names*

