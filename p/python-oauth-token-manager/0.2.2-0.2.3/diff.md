# Comparing `tmp/python-oauth-token-manager-0.2.2.tar.gz` & `tmp/python-oauth-token-manager-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-oauth-token-manager-0.2.2.tar", last modified: Thu May 18 18:02:58 2023, max compression
+gzip compressed data, was "python-oauth-token-manager-0.2.3.tar", last modified: Tue Jun  6 15:24:28 2023, max compression
```

## Comparing `python-oauth-token-manager-0.2.2.tar` & `python-oauth-token-manager-0.2.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-05-18 18:02:58.649086 python-oauth-token-manager-0.2.2/
--rw-rw-r--   0 davidharcombe (261421) primarygroup (89939)    11357 2022-07-15 13:28:45.000000 python-oauth-token-manager-0.2.2/LICENSE
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2936 2023-05-18 18:02:58.649086 python-oauth-token-manager-0.2.2/PKG-INFO
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2344 2022-08-23 16:30:58.000000 python-oauth-token-manager-0.2.2/README.md
-drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-05-18 18:02:58.645086 python-oauth-token-manager-0.2.2/auth/
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      749 2023-05-18 18:01:29.000000 python-oauth-token-manager-0.2.2/auth/__init__.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     4035 2022-07-08 21:15:10.000000 python-oauth-token-manager-0.2.2/auth/abstract_datastore.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5774 2023-05-16 15:53:57.000000 python-oauth-token-manager-0.2.2/auth/credentials.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1322 2022-07-12 16:38:02.000000 python-oauth-token-manager-0.2.2/auth/credentials_helpers.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1057 2022-07-12 16:36:52.000000 python-oauth-token-manager-0.2.2/auth/credentials_helpers_test.py
-drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-05-18 18:02:58.649086 python-oauth-token-manager-0.2.2/auth/datastore/
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      610 2023-05-18 18:02:08.000000 python-oauth-token-manager-0.2.2/auth/datastore/__init__.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5969 2023-05-18 14:50:53.000000 python-oauth-token-manager-0.2.2/auth/datastore/cloud_storage.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     8319 2023-05-18 14:50:53.000000 python-oauth-token-manager-0.2.2/auth/datastore/cloud_storage_test.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     4687 2023-05-18 14:47:50.000000 python-oauth-token-manager-0.2.2/auth/datastore/firestore.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5048 2023-05-18 14:51:31.000000 python-oauth-token-manager-0.2.2/auth/datastore/local_file.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     6154 2023-05-18 14:53:49.000000 python-oauth-token-manager-0.2.2/auth/datastore/local_file_test.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5986 2023-05-18 14:49:59.000000 python-oauth-token-manager-0.2.2/auth/datastore/secret_manager.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     1517 2022-08-17 14:18:37.000000 python-oauth-token-manager-0.2.2/auth/decorators.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     1030 2022-08-09 16:45:46.000000 python-oauth-token-manager-0.2.2/auth/decorators_test.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      739 2022-07-08 21:14:30.000000 python-oauth-token-manager-0.2.2/auth/exceptions.py
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       98 2022-08-24 18:15:10.000000 python-oauth-token-manager-0.2.2/pyproject.toml
-drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-05-18 18:02:58.649086 python-oauth-token-manager-0.2.2/python_oauth_token_manager.egg-info/
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2936 2023-05-18 18:02:58.000000 python-oauth-token-manager-0.2.2/python_oauth_token_manager.egg-info/PKG-INFO
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      746 2023-05-18 18:02:58.000000 python-oauth-token-manager-0.2.2/python_oauth_token_manager.egg-info/SOURCES.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        1 2023-05-18 18:02:58.000000 python-oauth-token-manager-0.2.2/python_oauth_token_manager.egg-info/dependency_links.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        1 2022-08-24 18:09:16.000000 python-oauth-token-manager-0.2.2/python_oauth_token_manager.egg-info/not-zip-safe
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      495 2023-05-18 18:02:58.000000 python-oauth-token-manager-0.2.2/python_oauth_token_manager.egg-info/requires.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        5 2023-05-18 18:02:58.000000 python-oauth-token-manager-0.2.2/python_oauth_token_manager.egg-info/top_level.txt
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       38 2023-05-18 18:02:58.649086 python-oauth-token-manager-0.2.2/setup.cfg
--rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2516 2023-05-18 18:02:25.000000 python-oauth-token-manager-0.2.2/setup.py
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-06 15:24:28.556372 python-oauth-token-manager-0.2.3/
+-rw-rw-r--   0 davidharcombe (261421) primarygroup (89939)    11357 2022-07-15 13:28:45.000000 python-oauth-token-manager-0.2.3/LICENSE
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2938 2023-06-06 15:24:28.556372 python-oauth-token-manager-0.2.3/PKG-INFO
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2344 2022-08-23 16:30:58.000000 python-oauth-token-manager-0.2.3/README.md
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-06 15:24:28.552372 python-oauth-token-manager-0.2.3/auth/
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      749 2023-05-18 18:01:29.000000 python-oauth-token-manager-0.2.3/auth/__init__.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     4035 2022-07-08 21:15:10.000000 python-oauth-token-manager-0.2.3/auth/abstract_datastore.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5774 2023-05-16 15:53:57.000000 python-oauth-token-manager-0.2.3/auth/credentials.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1322 2022-07-12 16:38:02.000000 python-oauth-token-manager-0.2.3/auth/credentials_helpers.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1057 2022-07-12 16:36:52.000000 python-oauth-token-manager-0.2.3/auth/credentials_helpers_test.py
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-06 15:24:28.556372 python-oauth-token-manager-0.2.3/auth/datastore/
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      610 2023-05-18 18:02:08.000000 python-oauth-token-manager-0.2.3/auth/datastore/__init__.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5969 2023-05-18 14:50:53.000000 python-oauth-token-manager-0.2.3/auth/datastore/cloud_storage.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     8319 2023-05-18 14:50:53.000000 python-oauth-token-manager-0.2.3/auth/datastore/cloud_storage_test.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     4687 2023-05-18 14:47:50.000000 python-oauth-token-manager-0.2.3/auth/datastore/firestore.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5048 2023-05-18 14:51:31.000000 python-oauth-token-manager-0.2.3/auth/datastore/local_file.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     6154 2023-05-18 14:53:49.000000 python-oauth-token-manager-0.2.3/auth/datastore/local_file_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     5986 2023-05-18 14:49:59.000000 python-oauth-token-manager-0.2.3/auth/datastore/secret_manager.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     1517 2022-08-17 14:18:37.000000 python-oauth-token-manager-0.2.3/auth/decorators.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     1030 2022-08-09 16:45:46.000000 python-oauth-token-manager-0.2.3/auth/decorators_test.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      739 2022-07-08 21:14:30.000000 python-oauth-token-manager-0.2.3/auth/exceptions.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1266 2023-06-06 15:24:18.000000 python-oauth-token-manager-0.2.3/pyproject.toml
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-06 15:24:28.556372 python-oauth-token-manager-0.2.3/python_oauth_token_manager.egg-info/
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2938 2023-06-06 15:24:28.000000 python-oauth-token-manager-0.2.3/python_oauth_token_manager.egg-info/PKG-INFO
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      746 2023-06-06 15:24:28.000000 python-oauth-token-manager-0.2.3/python_oauth_token_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        1 2023-06-06 15:24:28.000000 python-oauth-token-manager-0.2.3/python_oauth_token_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        1 2023-06-06 15:22:23.000000 python-oauth-token-manager-0.2.3/python_oauth_token_manager.egg-info/not-zip-safe
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      495 2023-06-06 15:24:28.000000 python-oauth-token-manager-0.2.3/python_oauth_token_manager.egg-info/requires.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        5 2023-06-06 15:24:28.000000 python-oauth-token-manager-0.2.3/python_oauth_token_manager.egg-info/top_level.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       38 2023-06-06 15:24:28.556372 python-oauth-token-manager-0.2.3/setup.cfg
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     2532 2023-06-06 15:17:47.000000 python-oauth-token-manager-0.2.3/setup.py
```

### Comparing `python-oauth-token-manager-0.2.2/LICENSE` & `python-oauth-token-manager-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.2/PKG-INFO` & `python-oauth-token-manager-0.2.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: python-oauth-token-manager
-Version: 0.2.2
+Version: 0.2.3
 Summary: API for managing stored OAuth credentials.
 Home-page: 
 Author: David Harcombe
-Author-email: david.harcombe@gmail.com
+Author-email: David Harcombe <david.harcombe@gmail.com>
 License: Apache 2.0
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development
-Classifier: License :: OSI Approved :: Apache Software License
+Project-URL: Homepage, https://github.com/googleworkspace/python-oauth-token-manager
+Project-URL: Bug Tracker, https://github.com/googleworkspace/python-oauth-token-manager/issues
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Python Library for storing OAuth credentials in many locations
 
 ## What's this for?
```

### Comparing `python-oauth-token-manager-0.2.2/README.md` & `python-oauth-token-manager-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.2/auth/__init__.py` & `python-oauth-token-manager-0.2.3/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.2/auth/abstract_datastore.py` & `python-oauth-token-manager-0.2.3/auth/abstract_datastore.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.2/auth/credentials.py` & `python-oauth-token-manager-0.2.3/auth/credentials.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.2/auth/credentials_helpers.py` & `python-oauth-token-manager-0.2.3/auth/credentials_helpers.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.2/auth/credentials_helpers_test.py` & `python-oauth-token-manager-0.2.3/auth/credentials_helpers_test.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.2/auth/datastore/__init__.py` & `python-oauth-token-manager-0.2.3/auth/datastore/__init__.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.2/auth/datastore/cloud_storage.py` & `python-oauth-token-manager-0.2.3/auth/datastore/cloud_storage.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.2/auth/datastore/cloud_storage_test.py` & `python-oauth-token-manager-0.2.3/auth/datastore/cloud_storage_test.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.2/auth/datastore/firestore.py` & `python-oauth-token-manager-0.2.3/auth/datastore/firestore.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.2/auth/datastore/local_file.py` & `python-oauth-token-manager-0.2.3/auth/datastore/local_file.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.2/auth/datastore/local_file_test.py` & `python-oauth-token-manager-0.2.3/auth/datastore/local_file_test.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.2/auth/datastore/secret_manager.py` & `python-oauth-token-manager-0.2.3/auth/datastore/secret_manager.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.2/auth/decorators.py` & `python-oauth-token-manager-0.2.3/auth/decorators.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.2/auth/decorators_test.py` & `python-oauth-token-manager-0.2.3/auth/decorators_test.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.2/auth/exceptions.py` & `python-oauth-token-manager-0.2.3/auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.2/python_oauth_token_manager.egg-info/PKG-INFO` & `python-oauth-token-manager-0.2.3/python_oauth_token_manager.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: python-oauth-token-manager
-Version: 0.2.2
+Version: 0.2.3
 Summary: API for managing stored OAuth credentials.
 Home-page: 
 Author: David Harcombe
-Author-email: david.harcombe@gmail.com
+Author-email: David Harcombe <david.harcombe@gmail.com>
 License: Apache 2.0
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development
-Classifier: License :: OSI Approved :: Apache Software License
+Project-URL: Homepage, https://github.com/googleworkspace/python-oauth-token-manager
+Project-URL: Bug Tracker, https://github.com/googleworkspace/python-oauth-token-manager/issues
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Python Library for storing OAuth credentials in many locations
 
 ## What's this for?
```

### Comparing `python-oauth-token-manager-0.2.2/python_oauth_token_manager.egg-info/SOURCES.txt` & `python-oauth-token-manager-0.2.3/python_oauth_token_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-oauth-token-manager-0.2.2/setup.py` & `python-oauth-token-manager-0.2.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import setuptools
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
   long_description = fh.read()
 
 setuptools.setup(
-    name='python-oauth-token-manager',
+    name='API for managing stored OAuth credentials.',
     version='0.2.2',
     description='API for managing stored OAuth credentials.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='',
     author='David Harcombe',
     author_email='david.harcombe@gmail.com',
```

