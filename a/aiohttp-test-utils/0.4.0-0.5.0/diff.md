# Comparing `tmp/aiohttp_test_utils-0.4.0.tar.gz` & `tmp/aiohttp_test_utils-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiohttp_test_utils-0.4.0.tar", last modified: Thu May 25 19:45:31 2023, max compression
+gzip compressed data, was "aiohttp_test_utils-0.5.0.tar", last modified: Tue Jun  6 19:30:08 2023, max compression
```

## Comparing `aiohttp_test_utils-0.4.0.tar` & `aiohttp_test_utils-0.5.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 19:45:31.526536 aiohttp_test_utils-0.4.0/
--rw-rw-rw-   0        0        0      532 2023-05-25 19:45:31.526536 aiohttp_test_utils-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0       46 2023-02-16 05:06:40.000000 aiohttp_test_utils-0.4.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-25 19:45:31.518121 aiohttp_test_utils-0.4.0/aiohttp_test_utils/
--rw-rw-rw-   0        0        0     1768 2023-05-25 19:45:28.000000 aiohttp_test_utils-0.4.0/aiohttp_test_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 19:45:31.526536 aiohttp_test_utils-0.4.0/aiohttp_test_utils.egg-info/
--rw-rw-rw-   0        0        0      532 2023-05-25 19:45:31.000000 aiohttp_test_utils-0.4.0/aiohttp_test_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-05-25 19:45:31.000000 aiohttp_test_utils-0.4.0/aiohttp_test_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 19:45:31.000000 aiohttp_test_utils-0.4.0/aiohttp_test_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-05-25 19:45:31.000000 aiohttp_test_utils-0.4.0/aiohttp_test_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-25 19:45:31.000000 aiohttp_test_utils-0.4.0/aiohttp_test_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-02-16 05:09:35.000000 aiohttp_test_utils-0.4.0/aiohttp_test_utils.egg-info/zip-safe
--rw-rw-rw-   0        0        0     1012 2023-05-25 17:54:50.000000 aiohttp_test_utils-0.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-25 19:45:31.526536 aiohttp_test_utils-0.4.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-06 19:30:08.009917 aiohttp_test_utils-0.5.0/
+-rw-rw-rw-   0        0        0      532 2023-06-06 19:30:08.008920 aiohttp_test_utils-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0       46 2023-02-16 05:06:40.000000 aiohttp_test_utils-0.5.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-06 19:30:07.994958 aiohttp_test_utils-0.5.0/aiohttp_test_utils/
+-rw-rw-rw-   0        0        0     2334 2023-06-06 19:30:05.000000 aiohttp_test_utils-0.5.0/aiohttp_test_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 19:30:08.007927 aiohttp_test_utils-0.5.0/aiohttp_test_utils.egg-info/
+-rw-rw-rw-   0        0        0      532 2023-06-06 19:30:07.000000 aiohttp_test_utils-0.5.0/aiohttp_test_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-06-06 19:30:07.000000 aiohttp_test_utils-0.5.0/aiohttp_test_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 19:30:07.000000 aiohttp_test_utils-0.5.0/aiohttp_test_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-06-06 19:30:07.000000 aiohttp_test_utils-0.5.0/aiohttp_test_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-06 19:30:07.000000 aiohttp_test_utils-0.5.0/aiohttp_test_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-02-16 05:09:35.000000 aiohttp_test_utils-0.5.0/aiohttp_test_utils.egg-info/zip-safe
+-rw-rw-rw-   0        0        0     1012 2023-05-25 17:54:50.000000 aiohttp_test_utils-0.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-06 19:30:08.009917 aiohttp_test_utils-0.5.0/setup.cfg
```

### Comparing `aiohttp_test_utils-0.4.0/PKG-INFO` & `aiohttp_test_utils-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiohttp_test_utils
-Version: 0.4.0
+Version: 0.5.0
 Summary: a small library used for testing aiohttp projects
 Author-email: 5j9 <5j9@users.noreply.github.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/5j9/aiohttp_test_utils
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
```

### Comparing `aiohttp_test_utils-0.4.0/aiohttp_test_utils/__init__.py` & `aiohttp_test_utils-0.5.0/aiohttp_test_utils/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-__version__ = '0.4.0'
-
+__version__ = '0.5.0'
+import atexit
 from asyncio import new_event_loop
 from unittest.mock import patch
 
 from decouple import config
 from pytest import fixture
 
 
 def init_tests():
-    global RECORD_MODE, OFFLINE_MODE, TESTS_PATH
+    global RECORD_MODE, OFFLINE_MODE, TESTS_PATH, REMOVE_UNUSED_TESTDATA
 
     config.search_path = TESTS_PATH = config._caller_path()
 
     RECORD_MODE = config('RECORD_MODE', False, cast=bool)
     OFFLINE_MODE = config('OFFLINE_MODE', False, cast=bool) and not RECORD_MODE
+    REMOVE_UNUSED_TESTDATA = config('REMOVE_UNUSED_TESTDATA', False, cast=bool) and OFFLINE_MODE
 
 
 class EqualToEverything:
     def __eq__(self, other):
         return True
 
 class FakeResponse:
@@ -70,9 +71,24 @@
 @fixture(scope='session')
 def event_loop():
     loop = new_event_loop()
     yield loop
     loop.close()
 
 
+def remove_unsed_file_names():
+    if REMOVE_UNUSED_TESTDATA is not True:
+        return
+    import os
+    for filename in set(os.listdir(f'{TESTS_PATH}/testdata/')) - USED_FILENAMES:
+        os.remove(f'{TESTS_PATH}/testdata/{filename}')
+        print(f'removed unsed file: {filename}')
+
+
+USED_FILENAMES = set()
+atexit.register(remove_unsed_file_names)
+
+
 def file(filename):
+    if REMOVE_UNUSED_TESTDATA is True:
+        USED_FILENAMES.add(filename)
     return patch.object(FakeResponse, 'file', f'{TESTS_PATH}/testdata/{filename}')
```

### Comparing `aiohttp_test_utils-0.4.0/aiohttp_test_utils.egg-info/PKG-INFO` & `aiohttp_test_utils-0.5.0/aiohttp_test_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiohttp-test-utils
-Version: 0.4.0
+Version: 0.5.0
 Summary: a small library used for testing aiohttp projects
 Author-email: 5j9 <5j9@users.noreply.github.com>
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Homepage, https://github.com/5j9/aiohttp_test_utils
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
```

### Comparing `aiohttp_test_utils-0.4.0/pyproject.toml` & `aiohttp_test_utils-0.5.0/pyproject.toml`

 * *Files identical despite different names*

