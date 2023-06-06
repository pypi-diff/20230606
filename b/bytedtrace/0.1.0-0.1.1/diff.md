# Comparing `tmp/bytedtrace-0.1.0.tar.gz` & `tmp/bytedtrace-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bytedtrace-0.1.0.tar", last modified: Tue Jun  6 14:48:50 2023, max compression
+gzip compressed data, was "bytedtrace-0.1.1.tar", last modified: Tue Jun  6 14:49:02 2023, max compression
```

## Comparing `bytedtrace-0.1.0.tar` & `bytedtrace-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 li4n0      (501) staff       (20)        0 2023-06-06 14:48:50.693844 bytedtrace-0.1.0/
--rw-r--r--   0 li4n0      (501) staff       (20)    57284 2023-05-22 15:11:02.000000 bytedtrace-0.1.0/HISTORY.md
--rw-r--r--   0 li4n0      (501) staff       (20)    10142 2023-05-22 15:08:07.000000 bytedtrace-0.1.0/LICENSE
--rw-r--r--   0 li4n0      (501) staff       (20)       75 2023-06-06 14:42:17.000000 bytedtrace-0.1.0/MANIFEST.in
--rw-r--r--   0 li4n0      (501) staff       (20)       38 2023-05-22 15:08:07.000000 bytedtrace-0.1.0/NOTICE
--rw-r--r--   0 li4n0      (501) staff       (20)      165 2023-06-06 14:48:50.694082 bytedtrace-0.1.0/PKG-INFO
--rw-r--r--   0 li4n0      (501) staff       (20)     2922 2023-05-22 15:08:07.000000 bytedtrace-0.1.0/README.md
-drwxr-xr-x   0 li4n0      (501) staff       (20)        0 2023-06-06 14:48:50.674837 bytedtrace-0.1.0/bytedtrace/
--rw-r--r--   0 li4n0      (501) staff       (20)      326 2023-06-06 14:19:39.000000 bytedtrace-0.1.0/bytedtrace/__init__py.py
-drwxr-xr-x   0 li4n0      (501) staff       (20)        0 2023-06-06 14:48:50.678383 bytedtrace-0.1.0/bytedtrace.egg-info/
--rw-r--r--   0 li4n0      (501) staff       (20)      165 2023-06-06 14:48:50.000000 bytedtrace-0.1.0/bytedtrace.egg-info/PKG-INFO
--rw-r--r--   0 li4n0      (501) staff       (20)      630 2023-06-06 14:48:50.000000 bytedtrace-0.1.0/bytedtrace.egg-info/SOURCES.txt
--rw-r--r--   0 li4n0      (501) staff       (20)        1 2023-06-06 14:48:50.000000 bytedtrace-0.1.0/bytedtrace.egg-info/dependency_links.txt
--rw-r--r--   0 li4n0      (501) staff       (20)        1 2023-06-06 14:05:14.000000 bytedtrace-0.1.0/bytedtrace.egg-info/not-zip-safe
--rw-r--r--   0 li4n0      (501) staff       (20)       11 2023-06-06 14:48:50.000000 bytedtrace-0.1.0/bytedtrace.egg-info/requires.txt
--rw-r--r--   0 li4n0      (501) staff       (20)       11 2023-06-06 14:48:50.000000 bytedtrace-0.1.0/bytedtrace.egg-info/top_level.txt
--rw-r--r--   0 li4n0      (501) staff       (20)      257 2023-05-22 15:08:07.000000 bytedtrace-0.1.0/pyproject.toml
--rw-r--r--   0 li4n0      (501) staff       (20)      250 2023-05-22 15:08:07.000000 bytedtrace-0.1.0/requirements-dev.txt
--rw-r--r--   0 li4n0      (501) staff       (20)      360 2023-06-06 14:48:50.695143 bytedtrace-0.1.0/setup.cfg
--rwxr-xr-x   0 li4n0      (501) staff       (20)      511 2023-06-06 14:47:55.000000 bytedtrace-0.1.0/setup.py
-drwxr-xr-x   0 li4n0      (501) staff       (20)        0 2023-06-06 14:48:50.692036 bytedtrace-0.1.0/tests/
--rw-r--r--   0 li4n0      (501) staff       (20)      469 2023-05-22 15:08:07.000000 bytedtrace-0.1.0/tests/__init__.py
--rw-r--r--   0 li4n0      (501) staff       (20)      480 2023-05-22 15:08:07.000000 bytedtrace-0.1.0/tests/compat.py
--rw-r--r--   0 li4n0      (501) staff       (20)     1581 2023-05-22 15:08:07.000000 bytedtrace-0.1.0/tests/conftest.py
--rw-r--r--   0 li4n0      (501) staff       (20)      808 2023-05-22 15:08:07.000000 bytedtrace-0.1.0/tests/test_help.py
--rw-r--r--   0 li4n0      (501) staff       (20)      424 2023-05-22 15:08:07.000000 bytedtrace-0.1.0/tests/test_hooks.py
--rw-r--r--   0 li4n0      (501) staff       (20)    15343 2023-05-22 15:08:07.000000 bytedtrace-0.1.0/tests/test_lowlevel.py
--rw-r--r--   0 li4n0      (501) staff       (20)      229 2023-05-22 15:08:07.000000 bytedtrace-0.1.0/tests/test_packages.py
--rw-r--r--   0 li4n0      (501) staff       (20)    98058 2023-05-22 15:11:02.000000 bytedtrace-0.1.0/tests/test_requests.py
--rw-r--r--   0 li4n0      (501) staff       (20)     2279 2023-05-22 15:08:07.000000 bytedtrace-0.1.0/tests/test_structures.py
--rw-r--r--   0 li4n0      (501) staff       (20)     5553 2023-05-22 15:08:07.000000 bytedtrace-0.1.0/tests/test_testserver.py
--rw-r--r--   0 li4n0      (501) staff       (20)    28254 2023-05-22 15:08:07.000000 bytedtrace-0.1.0/tests/test_utils.py
-drwxr-xr-x   0 li4n0      (501) staff       (20)        0 2023-06-06 14:48:50.693171 bytedtrace-0.1.0/tests/testserver/
--rw-r--r--   0 li4n0      (501) staff       (20)        0 2023-05-22 15:08:07.000000 bytedtrace-0.1.0/tests/testserver/__init__.py
--rw-r--r--   0 li4n0      (501) staff       (20)     3832 2023-05-22 15:08:07.000000 bytedtrace-0.1.0/tests/testserver/server.py
--rw-r--r--   0 li4n0      (501) staff       (20)      366 2023-05-22 15:08:07.000000 bytedtrace-0.1.0/tests/utils.py
+drwxr-xr-x   0 li4n0      (501) staff       (20)        0 2023-06-06 14:49:02.315808 bytedtrace-0.1.1/
+-rw-r--r--   0 li4n0      (501) staff       (20)    57284 2023-05-22 15:11:02.000000 bytedtrace-0.1.1/HISTORY.md
+-rw-r--r--   0 li4n0      (501) staff       (20)    10142 2023-05-22 15:08:07.000000 bytedtrace-0.1.1/LICENSE
+-rw-r--r--   0 li4n0      (501) staff       (20)       75 2023-06-06 14:42:17.000000 bytedtrace-0.1.1/MANIFEST.in
+-rw-r--r--   0 li4n0      (501) staff       (20)       38 2023-05-22 15:08:07.000000 bytedtrace-0.1.1/NOTICE
+-rw-r--r--   0 li4n0      (501) staff       (20)      165 2023-06-06 14:49:02.315930 bytedtrace-0.1.1/PKG-INFO
+-rw-r--r--   0 li4n0      (501) staff       (20)     2922 2023-05-22 15:08:07.000000 bytedtrace-0.1.1/README.md
+drwxr-xr-x   0 li4n0      (501) staff       (20)        0 2023-06-06 14:49:02.296697 bytedtrace-0.1.1/bytedtrace/
+-rw-r--r--   0 li4n0      (501) staff       (20)      326 2023-06-06 14:19:39.000000 bytedtrace-0.1.1/bytedtrace/__init__py.py
+drwxr-xr-x   0 li4n0      (501) staff       (20)        0 2023-06-06 14:49:02.300347 bytedtrace-0.1.1/bytedtrace.egg-info/
+-rw-r--r--   0 li4n0      (501) staff       (20)      165 2023-06-06 14:49:02.000000 bytedtrace-0.1.1/bytedtrace.egg-info/PKG-INFO
+-rw-r--r--   0 li4n0      (501) staff       (20)      630 2023-06-06 14:49:02.000000 bytedtrace-0.1.1/bytedtrace.egg-info/SOURCES.txt
+-rw-r--r--   0 li4n0      (501) staff       (20)        1 2023-06-06 14:49:02.000000 bytedtrace-0.1.1/bytedtrace.egg-info/dependency_links.txt
+-rw-r--r--   0 li4n0      (501) staff       (20)        1 2023-06-06 14:05:14.000000 bytedtrace-0.1.1/bytedtrace.egg-info/not-zip-safe
+-rw-r--r--   0 li4n0      (501) staff       (20)       11 2023-06-06 14:49:02.000000 bytedtrace-0.1.1/bytedtrace.egg-info/requires.txt
+-rw-r--r--   0 li4n0      (501) staff       (20)       11 2023-06-06 14:49:02.000000 bytedtrace-0.1.1/bytedtrace.egg-info/top_level.txt
+-rw-r--r--   0 li4n0      (501) staff       (20)      257 2023-05-22 15:08:07.000000 bytedtrace-0.1.1/pyproject.toml
+-rw-r--r--   0 li4n0      (501) staff       (20)      250 2023-05-22 15:08:07.000000 bytedtrace-0.1.1/requirements-dev.txt
+-rw-r--r--   0 li4n0      (501) staff       (20)      360 2023-06-06 14:49:02.316417 bytedtrace-0.1.1/setup.cfg
+-rwxr-xr-x   0 li4n0      (501) staff       (20)      511 2023-06-06 14:47:55.000000 bytedtrace-0.1.1/setup.py
+drwxr-xr-x   0 li4n0      (501) staff       (20)        0 2023-06-06 14:49:02.313929 bytedtrace-0.1.1/tests/
+-rw-r--r--   0 li4n0      (501) staff       (20)      469 2023-05-22 15:08:07.000000 bytedtrace-0.1.1/tests/__init__.py
+-rw-r--r--   0 li4n0      (501) staff       (20)      480 2023-05-22 15:08:07.000000 bytedtrace-0.1.1/tests/compat.py
+-rw-r--r--   0 li4n0      (501) staff       (20)     1581 2023-05-22 15:08:07.000000 bytedtrace-0.1.1/tests/conftest.py
+-rw-r--r--   0 li4n0      (501) staff       (20)      808 2023-05-22 15:08:07.000000 bytedtrace-0.1.1/tests/test_help.py
+-rw-r--r--   0 li4n0      (501) staff       (20)      424 2023-05-22 15:08:07.000000 bytedtrace-0.1.1/tests/test_hooks.py
+-rw-r--r--   0 li4n0      (501) staff       (20)    15343 2023-05-22 15:08:07.000000 bytedtrace-0.1.1/tests/test_lowlevel.py
+-rw-r--r--   0 li4n0      (501) staff       (20)      229 2023-05-22 15:08:07.000000 bytedtrace-0.1.1/tests/test_packages.py
+-rw-r--r--   0 li4n0      (501) staff       (20)    98058 2023-05-22 15:11:02.000000 bytedtrace-0.1.1/tests/test_requests.py
+-rw-r--r--   0 li4n0      (501) staff       (20)     2279 2023-05-22 15:08:07.000000 bytedtrace-0.1.1/tests/test_structures.py
+-rw-r--r--   0 li4n0      (501) staff       (20)     5553 2023-05-22 15:08:07.000000 bytedtrace-0.1.1/tests/test_testserver.py
+-rw-r--r--   0 li4n0      (501) staff       (20)    28254 2023-05-22 15:08:07.000000 bytedtrace-0.1.1/tests/test_utils.py
+drwxr-xr-x   0 li4n0      (501) staff       (20)        0 2023-06-06 14:49:02.315107 bytedtrace-0.1.1/tests/testserver/
+-rw-r--r--   0 li4n0      (501) staff       (20)        0 2023-05-22 15:08:07.000000 bytedtrace-0.1.1/tests/testserver/__init__.py
+-rw-r--r--   0 li4n0      (501) staff       (20)     3832 2023-05-22 15:08:07.000000 bytedtrace-0.1.1/tests/testserver/server.py
+-rw-r--r--   0 li4n0      (501) staff       (20)      366 2023-05-22 15:08:07.000000 bytedtrace-0.1.1/tests/utils.py
```

### Comparing `bytedtrace-0.1.0/HISTORY.md` & `bytedtrace-0.1.1/HISTORY.md`

 * *Files identical despite different names*

### Comparing `bytedtrace-0.1.0/LICENSE` & `bytedtrace-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bytedtrace-0.1.0/README.md` & `bytedtrace-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `bytedtrace-0.1.0/bytedtrace.egg-info/SOURCES.txt` & `bytedtrace-0.1.1/bytedtrace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bytedtrace-0.1.0/tests/conftest.py` & `bytedtrace-0.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `bytedtrace-0.1.0/tests/test_help.py` & `bytedtrace-0.1.1/tests/test_help.py`

 * *Files identical despite different names*

### Comparing `bytedtrace-0.1.0/tests/test_lowlevel.py` & `bytedtrace-0.1.1/tests/test_lowlevel.py`

 * *Files identical despite different names*

### Comparing `bytedtrace-0.1.0/tests/test_requests.py` & `bytedtrace-0.1.1/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `bytedtrace-0.1.0/tests/test_structures.py` & `bytedtrace-0.1.1/tests/test_structures.py`

 * *Files identical despite different names*

### Comparing `bytedtrace-0.1.0/tests/test_testserver.py` & `bytedtrace-0.1.1/tests/test_testserver.py`

 * *Files identical despite different names*

### Comparing `bytedtrace-0.1.0/tests/test_utils.py` & `bytedtrace-0.1.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `bytedtrace-0.1.0/tests/testserver/server.py` & `bytedtrace-0.1.1/tests/testserver/server.py`

 * *Files identical despite different names*

