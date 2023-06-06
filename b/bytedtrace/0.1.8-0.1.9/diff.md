# Comparing `tmp/bytedtrace-000000.1.8.tar.gz` & `tmp/bytedtrace-000000.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bytedtrace-0.1.8.tar", last modified: Tue Jun  6 15:57:35 2023, max compression
+gzip compressed data, was "bytedtrace-0.1.9.tar", last modified: Tue Jun  6 15:57:37 2023, max compression
```

## Comparing `bytedtrace-000000.1.8.tar` & `bytedtrace-000000.1.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 li4n0      (501) staff       (20)        0 2023-06-06 15:57:35.396589 bytedtrace-0.1.8/
--rw-r--r--   0 li4n0      (501) staff       (20)    57284 2023-05-22 15:11:02.000000 bytedtrace-0.1.8/HISTORY.md
--rw-r--r--   0 li4n0      (501) staff       (20)    10142 2023-05-22 15:08:07.000000 bytedtrace-0.1.8/LICENSE
--rw-r--r--   0 li4n0      (501) staff       (20)       75 2023-06-06 14:42:17.000000 bytedtrace-0.1.8/MANIFEST.in
--rw-r--r--   0 li4n0      (501) staff       (20)       38 2023-05-22 15:08:07.000000 bytedtrace-0.1.8/NOTICE
--rw-r--r--   0 li4n0      (501) staff       (20)      165 2023-06-06 15:57:35.396733 bytedtrace-0.1.8/PKG-INFO
--rw-r--r--   0 li4n0      (501) staff       (20)     2922 2023-05-22 15:08:07.000000 bytedtrace-0.1.8/README.md
-drwxr-xr-x   0 li4n0      (501) staff       (20)        0 2023-06-06 15:57:35.386933 bytedtrace-0.1.8/bytedtrace/
--rw-r--r--   0 li4n0      (501) staff       (20)      326 2023-06-06 14:19:39.000000 bytedtrace-0.1.8/bytedtrace/__init__py.py
-drwxr-xr-x   0 li4n0      (501) staff       (20)        0 2023-06-06 15:57:35.389216 bytedtrace-0.1.8/bytedtrace.egg-info/
--rw-r--r--   0 li4n0      (501) staff       (20)      165 2023-06-06 15:57:35.000000 bytedtrace-0.1.8/bytedtrace.egg-info/PKG-INFO
--rw-r--r--   0 li4n0      (501) staff       (20)      630 2023-06-06 15:57:35.000000 bytedtrace-0.1.8/bytedtrace.egg-info/SOURCES.txt
--rw-r--r--   0 li4n0      (501) staff       (20)        1 2023-06-06 15:57:35.000000 bytedtrace-0.1.8/bytedtrace.egg-info/dependency_links.txt
--rw-r--r--   0 li4n0      (501) staff       (20)        1 2023-06-06 14:05:14.000000 bytedtrace-0.1.8/bytedtrace.egg-info/not-zip-safe
--rw-r--r--   0 li4n0      (501) staff       (20)        9 2023-06-06 15:57:35.000000 bytedtrace-0.1.8/bytedtrace.egg-info/requires.txt
--rw-r--r--   0 li4n0      (501) staff       (20)       11 2023-06-06 15:57:35.000000 bytedtrace-0.1.8/bytedtrace.egg-info/top_level.txt
--rw-r--r--   0 li4n0      (501) staff       (20)      257 2023-05-22 15:08:07.000000 bytedtrace-0.1.8/pyproject.toml
--rw-r--r--   0 li4n0      (501) staff       (20)      250 2023-05-22 15:08:07.000000 bytedtrace-0.1.8/requirements-dev.txt
--rw-r--r--   0 li4n0      (501) staff       (20)      360 2023-06-06 15:57:35.397355 bytedtrace-0.1.8/setup.cfg
--rwxr-xr-x   0 li4n0      (501) staff       (20)     1049 2023-06-06 15:56:54.000000 bytedtrace-0.1.8/setup.py
-drwxr-xr-x   0 li4n0      (501) staff       (20)        0 2023-06-06 15:57:35.394675 bytedtrace-0.1.8/tests/
--rw-r--r--   0 li4n0      (501) staff       (20)      469 2023-05-22 15:08:07.000000 bytedtrace-0.1.8/tests/__init__.py
--rw-r--r--   0 li4n0      (501) staff       (20)      480 2023-05-22 15:08:07.000000 bytedtrace-0.1.8/tests/compat.py
--rw-r--r--   0 li4n0      (501) staff       (20)     1581 2023-05-22 15:08:07.000000 bytedtrace-0.1.8/tests/conftest.py
--rw-r--r--   0 li4n0      (501) staff       (20)      808 2023-05-22 15:08:07.000000 bytedtrace-0.1.8/tests/test_help.py
--rw-r--r--   0 li4n0      (501) staff       (20)      424 2023-05-22 15:08:07.000000 bytedtrace-0.1.8/tests/test_hooks.py
--rw-r--r--   0 li4n0      (501) staff       (20)    15343 2023-05-22 15:08:07.000000 bytedtrace-0.1.8/tests/test_lowlevel.py
--rw-r--r--   0 li4n0      (501) staff       (20)      229 2023-05-22 15:08:07.000000 bytedtrace-0.1.8/tests/test_packages.py
--rw-r--r--   0 li4n0      (501) staff       (20)    98058 2023-05-22 15:11:02.000000 bytedtrace-0.1.8/tests/test_requests.py
--rw-r--r--   0 li4n0      (501) staff       (20)     2279 2023-05-22 15:08:07.000000 bytedtrace-0.1.8/tests/test_structures.py
--rw-r--r--   0 li4n0      (501) staff       (20)     5553 2023-05-22 15:08:07.000000 bytedtrace-0.1.8/tests/test_testserver.py
--rw-r--r--   0 li4n0      (501) staff       (20)    28254 2023-05-22 15:08:07.000000 bytedtrace-0.1.8/tests/test_utils.py
-drwxr-xr-x   0 li4n0      (501) staff       (20)        0 2023-06-06 15:57:35.395279 bytedtrace-0.1.8/tests/testserver/
--rw-r--r--   0 li4n0      (501) staff       (20)        0 2023-05-22 15:08:07.000000 bytedtrace-0.1.8/tests/testserver/__init__.py
--rw-r--r--   0 li4n0      (501) staff       (20)     3832 2023-05-22 15:08:07.000000 bytedtrace-0.1.8/tests/testserver/server.py
--rw-r--r--   0 li4n0      (501) staff       (20)      366 2023-05-22 15:08:07.000000 bytedtrace-0.1.8/tests/utils.py
+drwxr-xr-x   0 li4n0      (501) staff       (20)        0 2023-06-06 15:57:37.154737 bytedtrace-0.1.9/
+-rw-r--r--   0 li4n0      (501) staff       (20)    57284 2023-05-22 15:11:02.000000 bytedtrace-0.1.9/HISTORY.md
+-rw-r--r--   0 li4n0      (501) staff       (20)    10142 2023-05-22 15:08:07.000000 bytedtrace-0.1.9/LICENSE
+-rw-r--r--   0 li4n0      (501) staff       (20)       75 2023-06-06 14:42:17.000000 bytedtrace-0.1.9/MANIFEST.in
+-rw-r--r--   0 li4n0      (501) staff       (20)       38 2023-05-22 15:08:07.000000 bytedtrace-0.1.9/NOTICE
+-rw-r--r--   0 li4n0      (501) staff       (20)      165 2023-06-06 15:57:37.154961 bytedtrace-0.1.9/PKG-INFO
+-rw-r--r--   0 li4n0      (501) staff       (20)     2922 2023-05-22 15:08:07.000000 bytedtrace-0.1.9/README.md
+drwxr-xr-x   0 li4n0      (501) staff       (20)        0 2023-06-06 15:57:37.136688 bytedtrace-0.1.9/bytedtrace/
+-rw-r--r--   0 li4n0      (501) staff       (20)      326 2023-06-06 14:19:39.000000 bytedtrace-0.1.9/bytedtrace/__init__py.py
+drwxr-xr-x   0 li4n0      (501) staff       (20)        0 2023-06-06 15:57:37.141600 bytedtrace-0.1.9/bytedtrace.egg-info/
+-rw-r--r--   0 li4n0      (501) staff       (20)      165 2023-06-06 15:57:37.000000 bytedtrace-0.1.9/bytedtrace.egg-info/PKG-INFO
+-rw-r--r--   0 li4n0      (501) staff       (20)      630 2023-06-06 15:57:37.000000 bytedtrace-0.1.9/bytedtrace.egg-info/SOURCES.txt
+-rw-r--r--   0 li4n0      (501) staff       (20)        1 2023-06-06 15:57:37.000000 bytedtrace-0.1.9/bytedtrace.egg-info/dependency_links.txt
+-rw-r--r--   0 li4n0      (501) staff       (20)        1 2023-06-06 14:05:14.000000 bytedtrace-0.1.9/bytedtrace.egg-info/not-zip-safe
+-rw-r--r--   0 li4n0      (501) staff       (20)        9 2023-06-06 15:57:37.000000 bytedtrace-0.1.9/bytedtrace.egg-info/requires.txt
+-rw-r--r--   0 li4n0      (501) staff       (20)       11 2023-06-06 15:57:37.000000 bytedtrace-0.1.9/bytedtrace.egg-info/top_level.txt
+-rw-r--r--   0 li4n0      (501) staff       (20)      257 2023-05-22 15:08:07.000000 bytedtrace-0.1.9/pyproject.toml
+-rw-r--r--   0 li4n0      (501) staff       (20)      250 2023-05-22 15:08:07.000000 bytedtrace-0.1.9/requirements-dev.txt
+-rw-r--r--   0 li4n0      (501) staff       (20)      360 2023-06-06 15:57:37.156561 bytedtrace-0.1.9/setup.cfg
+-rwxr-xr-x   0 li4n0      (501) staff       (20)     1049 2023-06-06 15:56:54.000000 bytedtrace-0.1.9/setup.py
+drwxr-xr-x   0 li4n0      (501) staff       (20)        0 2023-06-06 15:57:37.151304 bytedtrace-0.1.9/tests/
+-rw-r--r--   0 li4n0      (501) staff       (20)      469 2023-05-22 15:08:07.000000 bytedtrace-0.1.9/tests/__init__.py
+-rw-r--r--   0 li4n0      (501) staff       (20)      480 2023-05-22 15:08:07.000000 bytedtrace-0.1.9/tests/compat.py
+-rw-r--r--   0 li4n0      (501) staff       (20)     1581 2023-05-22 15:08:07.000000 bytedtrace-0.1.9/tests/conftest.py
+-rw-r--r--   0 li4n0      (501) staff       (20)      808 2023-05-22 15:08:07.000000 bytedtrace-0.1.9/tests/test_help.py
+-rw-r--r--   0 li4n0      (501) staff       (20)      424 2023-05-22 15:08:07.000000 bytedtrace-0.1.9/tests/test_hooks.py
+-rw-r--r--   0 li4n0      (501) staff       (20)    15343 2023-05-22 15:08:07.000000 bytedtrace-0.1.9/tests/test_lowlevel.py
+-rw-r--r--   0 li4n0      (501) staff       (20)      229 2023-05-22 15:08:07.000000 bytedtrace-0.1.9/tests/test_packages.py
+-rw-r--r--   0 li4n0      (501) staff       (20)    98058 2023-05-22 15:11:02.000000 bytedtrace-0.1.9/tests/test_requests.py
+-rw-r--r--   0 li4n0      (501) staff       (20)     2279 2023-05-22 15:08:07.000000 bytedtrace-0.1.9/tests/test_structures.py
+-rw-r--r--   0 li4n0      (501) staff       (20)     5553 2023-05-22 15:08:07.000000 bytedtrace-0.1.9/tests/test_testserver.py
+-rw-r--r--   0 li4n0      (501) staff       (20)    28254 2023-05-22 15:08:07.000000 bytedtrace-0.1.9/tests/test_utils.py
+drwxr-xr-x   0 li4n0      (501) staff       (20)        0 2023-06-06 15:57:37.154224 bytedtrace-0.1.9/tests/testserver/
+-rw-r--r--   0 li4n0      (501) staff       (20)        0 2023-05-22 15:08:07.000000 bytedtrace-0.1.9/tests/testserver/__init__.py
+-rw-r--r--   0 li4n0      (501) staff       (20)     3832 2023-05-22 15:08:07.000000 bytedtrace-0.1.9/tests/testserver/server.py
+-rw-r--r--   0 li4n0      (501) staff       (20)      366 2023-05-22 15:08:07.000000 bytedtrace-0.1.9/tests/utils.py
```

### Comparing `bytedtrace-0.1.8/HISTORY.md` & `bytedtrace-0.1.9/HISTORY.md`

 * *Files identical despite different names*

### Comparing `bytedtrace-0.1.8/LICENSE` & `bytedtrace-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bytedtrace-0.1.8/README.md` & `bytedtrace-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `bytedtrace-0.1.8/bytedtrace.egg-info/SOURCES.txt` & `bytedtrace-0.1.9/bytedtrace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bytedtrace-0.1.8/setup.py` & `bytedtrace-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `bytedtrace-0.1.8/tests/conftest.py` & `bytedtrace-0.1.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `bytedtrace-0.1.8/tests/test_help.py` & `bytedtrace-0.1.9/tests/test_help.py`

 * *Files identical despite different names*

### Comparing `bytedtrace-0.1.8/tests/test_lowlevel.py` & `bytedtrace-0.1.9/tests/test_lowlevel.py`

 * *Files identical despite different names*

### Comparing `bytedtrace-0.1.8/tests/test_requests.py` & `bytedtrace-0.1.9/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `bytedtrace-0.1.8/tests/test_structures.py` & `bytedtrace-0.1.9/tests/test_structures.py`

 * *Files identical despite different names*

### Comparing `bytedtrace-0.1.8/tests/test_testserver.py` & `bytedtrace-0.1.9/tests/test_testserver.py`

 * *Files identical despite different names*

### Comparing `bytedtrace-0.1.8/tests/test_utils.py` & `bytedtrace-0.1.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `bytedtrace-0.1.8/tests/testserver/server.py` & `bytedtrace-0.1.9/tests/testserver/server.py`

 * *Files identical despite different names*

