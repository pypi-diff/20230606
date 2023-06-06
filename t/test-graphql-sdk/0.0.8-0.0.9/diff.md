# Comparing `tmp/test_graphql_sdk-0.0.8.tar.gz` & `tmp/test_graphql_sdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_graphql_sdk-0.0.8.tar", last modified: Mon Jun  5 12:59:32 2023, max compression
+gzip compressed data, was "test_graphql_sdk-0.0.9.tar", last modified: Mon Jun  5 13:04:17 2023, max compression
```

## Comparing `test_graphql_sdk-0.0.8.tar` & `test_graphql_sdk-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-05 12:59:32.261044 test_graphql_sdk-0.0.8/
--rw-r--r--   0 sarvesh    (501) staff       (20)     3204 2023-06-05 12:59:32.261092 test_graphql_sdk-0.0.8/PKG-INFO
--rw-r--r--   0 sarvesh    (501) staff       (20)     2692 2023-06-05 12:41:34.000000 test_graphql_sdk-0.0.8/README.md
--rw-r--r--   0 sarvesh    (501) staff       (20)       85 2023-05-31 07:35:04.000000 test_graphql_sdk-0.0.8/pyproject.toml
--rw-r--r--   0 sarvesh    (501) staff       (20)      659 2023-06-05 12:59:32.261289 test_graphql_sdk-0.0.8/setup.cfg
-drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-05 12:59:32.259390 test_graphql_sdk-0.0.8/src/
-drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-05 12:59:32.260402 test_graphql_sdk-0.0.8/src/airstack/
--rw-r--r--   0 sarvesh    (501) staff       (20)        0 2023-06-05 12:53:03.000000 test_graphql_sdk-0.0.8/src/airstack/__init__.py
--rw-r--r--   0 sarvesh    (501) staff       (20)      210 2023-06-01 15:14:21.000000 test_graphql_sdk-0.0.8/src/airstack/constant.py
--rw-r--r--   0 sarvesh    (501) staff       (20)     2288 2023-06-05 11:32:00.000000 test_graphql_sdk-0.0.8/src/airstack/example.py
--rw-r--r--   0 sarvesh    (501) staff       (20)     4792 2023-06-05 12:59:05.000000 test_graphql_sdk-0.0.8/src/airstack/execute_query.py
--rw-r--r--   0 sarvesh    (501) staff       (20)     5723 2023-06-02 16:57:40.000000 test_graphql_sdk-0.0.8/src/airstack/generic.py
--rw-r--r--   0 sarvesh    (501) staff       (20)     1807 2023-06-05 12:59:05.000000 test_graphql_sdk-0.0.8/src/airstack/send_request.py
-drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-05 12:59:32.260906 test_graphql_sdk-0.0.8/src/test_graphql_sdk.egg-info/
--rw-r--r--   0 sarvesh    (501) staff       (20)     3204 2023-06-05 12:59:32.000000 test_graphql_sdk-0.0.8/src/test_graphql_sdk.egg-info/PKG-INFO
--rw-r--r--   0 sarvesh    (501) staff       (20)      367 2023-06-05 12:59:32.000000 test_graphql_sdk-0.0.8/src/test_graphql_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 sarvesh    (501) staff       (20)        1 2023-06-05 12:59:32.000000 test_graphql_sdk-0.0.8/src/test_graphql_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 sarvesh    (501) staff       (20)        9 2023-06-05 12:59:32.000000 test_graphql_sdk-0.0.8/src/test_graphql_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-05 13:04:17.979684 test_graphql_sdk-0.0.9/
+-rw-r--r--   0 sarvesh    (501) staff       (20)     3204 2023-06-05 13:04:17.979735 test_graphql_sdk-0.0.9/PKG-INFO
+-rw-r--r--   0 sarvesh    (501) staff       (20)     2692 2023-06-05 12:41:34.000000 test_graphql_sdk-0.0.9/README.md
+-rw-r--r--   0 sarvesh    (501) staff       (20)       85 2023-05-31 07:35:04.000000 test_graphql_sdk-0.0.9/pyproject.toml
+-rw-r--r--   0 sarvesh    (501) staff       (20)      659 2023-06-05 13:04:17.979953 test_graphql_sdk-0.0.9/setup.cfg
+drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-05 13:04:17.977466 test_graphql_sdk-0.0.9/src/
+drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-05 13:04:17.978963 test_graphql_sdk-0.0.9/src/airstack/
+-rw-r--r--   0 sarvesh    (501) staff       (20)        0 2023-06-05 12:53:03.000000 test_graphql_sdk-0.0.9/src/airstack/__init__.py
+-rw-r--r--   0 sarvesh    (501) staff       (20)      210 2023-06-01 15:14:21.000000 test_graphql_sdk-0.0.9/src/airstack/constant.py
+-rw-r--r--   0 sarvesh    (501) staff       (20)     4819 2023-06-05 13:03:57.000000 test_graphql_sdk-0.0.9/src/airstack/execute_query.py
+-rw-r--r--   0 sarvesh    (501) staff       (20)     5723 2023-06-02 16:57:40.000000 test_graphql_sdk-0.0.9/src/airstack/generic.py
+-rw-r--r--   0 sarvesh    (501) staff       (20)     1816 2023-06-05 13:02:01.000000 test_graphql_sdk-0.0.9/src/airstack/send_request.py
+drwxr-xr-x   0 sarvesh    (501) staff       (20)        0 2023-06-05 13:04:17.979584 test_graphql_sdk-0.0.9/src/test_graphql_sdk.egg-info/
+-rw-r--r--   0 sarvesh    (501) staff       (20)     3204 2023-06-05 13:04:17.000000 test_graphql_sdk-0.0.9/src/test_graphql_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 sarvesh    (501) staff       (20)      343 2023-06-05 13:04:17.000000 test_graphql_sdk-0.0.9/src/test_graphql_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 sarvesh    (501) staff       (20)        1 2023-06-05 13:04:17.000000 test_graphql_sdk-0.0.9/src/test_graphql_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 sarvesh    (501) staff       (20)        9 2023-06-05 13:04:17.000000 test_graphql_sdk-0.0.9/src/test_graphql_sdk.egg-info/top_level.txt
```

### Comparing `test_graphql_sdk-0.0.8/PKG-INFO` & `test_graphql_sdk-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test_graphql_sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python sdk for airstack apis
 Home-page: https://github.com/Airstack-xyz/airstack-python-sdk
 Author: Sarvesh
 Author-email: sarveshsingh.03@gmail.com
 Project-URL: Bug Tracker, https://github.com/Airstack-xyz/airstack-python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `test_graphql_sdk-0.0.8/README.md` & `test_graphql_sdk-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `test_graphql_sdk-0.0.8/setup.cfg` & `test_graphql_sdk-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = test_graphql_sdk
-version = 0.0.8
+version = 0.0.9
 author = Sarvesh
 author_email = sarveshsingh.03@gmail.com
 description = Python sdk for airstack apis
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Airstack-xyz/airstack-python-sdk
 project_urls =
```

### Comparing `test_graphql_sdk-0.0.8/src/airstack/execute_query.py` & `test_graphql_sdk-0.0.9/src/airstack/execute_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import re
-from send_request import SendRequest
+from airstack.send_request import SendRequest
 from graphql import parse, print_ast
-from generic import find_page_info, add_cursor_to_input_field, replace_cursor_value, \
+from airstack.generic import find_page_info, add_cursor_to_input_field, replace_cursor_value, \
     has_cursor
-from constant import AirstackConstants
+from airstack.constant import AirstackConstants
 
 
 class AirstackClient:
     """Class to create api client for airstack api's
     """
 
     def __init__(self, url=None, api_key=None):
```

### Comparing `test_graphql_sdk-0.0.8/src/airstack/generic.py` & `test_graphql_sdk-0.0.9/src/airstack/generic.py`

 * *Files identical despite different names*

### Comparing `test_graphql_sdk-0.0.8/src/airstack/send_request.py` & `test_graphql_sdk-0.0.9/src/airstack/send_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __author__ = 'sarvesh.singh'
 
 import aiohttp
 import json
-from constant import AirstackConstants
+from airstack.constant import AirstackConstants
 
 
 class SendRequest:
     """
     Send Request
     """
```

### Comparing `test_graphql_sdk-0.0.8/src/test_graphql_sdk.egg-info/PKG-INFO` & `test_graphql_sdk-0.0.9/src/test_graphql_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: test-graphql-sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python sdk for airstack apis
 Home-page: https://github.com/Airstack-xyz/airstack-python-sdk
 Author: Sarvesh
 Author-email: sarveshsingh.03@gmail.com
 Project-URL: Bug Tracker, https://github.com/Airstack-xyz/airstack-python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

