# Comparing `tmp/xdeps-0.1.0.tar.gz` & `tmp/xdeps-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xdeps-0.1.0.tar", last modified: Tue May 30 19:19:39 2023, max compression
+gzip compressed data, was "xdeps-0.1.1.tar", last modified: Tue Jun  6 14:39:39 2023, max compression
```

## Comparing `xdeps-0.1.0.tar` & `xdeps-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-05-30 19:19:39.649571 xdeps-0.1.0/
--rw-r--r--   0 giadarol   (503) staff       (20)    11356 2023-03-23 11:04:37.000000 xdeps-0.1.0/LICENSE
--rw-r--r--   0 giadarol   (503) staff       (20)      559 2023-05-30 19:19:39.649420 xdeps-0.1.0/PKG-INFO
--rw-r--r--   0 giadarol   (503) staff       (20)       38 2023-05-30 19:19:39.649618 xdeps-0.1.0/setup.cfg
--rw-r--r--   0 giadarol   (503) staff       (20)     1253 2023-03-23 11:04:37.000000 xdeps-0.1.0/setup.py
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-05-30 19:19:39.644337 xdeps-0.1.0/xdeps/
--rw-r--r--   0 giadarol   (503) staff       (20)      391 2023-05-30 19:18:47.000000 xdeps-0.1.0/xdeps/__init__.py
--rw-r--r--   0 giadarol   (503) staff       (20)       22 2023-05-30 19:19:10.000000 xdeps-0.1.0/xdeps/_version.py
--rw-r--r--   0 giadarol   (503) staff       (20)      160 2023-05-30 19:18:47.000000 xdeps-0.1.0/xdeps/general.py
--rw-r--r--   0 giadarol   (503) staff       (20)     5506 2023-04-05 12:43:31.000000 xdeps-0.1.0/xdeps/madxutils.py
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-05-30 19:19:39.649187 xdeps-0.1.0/xdeps/optimize/
--rw-r--r--   0 giadarol   (503) staff       (20)      118 2023-05-30 19:18:47.000000 xdeps-0.1.0/xdeps/optimize/__init__.py
--rw-r--r--   0 giadarol   (503) staff       (20)     3511 2023-05-30 19:18:47.000000 xdeps-0.1.0/xdeps/optimize/jacobian.py
--rw-r--r--   0 giadarol   (503) staff       (20)    11173 2023-05-30 19:18:47.000000 xdeps-0.1.0/xdeps/optimize/optimize.py
--rw-r--r--   0 giadarol   (503) staff       (20)    21520 2023-05-30 19:18:47.000000 xdeps-0.1.0/xdeps/refs.py
--rw-r--r--   0 giadarol   (503) staff       (20)     2093 2023-04-05 12:43:31.000000 xdeps-0.1.0/xdeps/sorting.py
--rw-r--r--   0 giadarol   (503) staff       (20)    14604 2023-05-23 20:23:29.000000 xdeps-0.1.0/xdeps/tasks.py
--rw-r--r--   0 giadarol   (503) staff       (20)      932 2023-04-05 12:43:31.000000 xdeps-0.1.0/xdeps/utils.py
-drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-05-30 19:19:39.648398 xdeps-0.1.0/xdeps.egg-info/
--rw-r--r--   0 giadarol   (503) staff       (20)      559 2023-05-30 19:19:39.000000 xdeps-0.1.0/xdeps.egg-info/PKG-INFO
--rw-r--r--   0 giadarol   (503) staff       (20)      374 2023-05-30 19:19:39.000000 xdeps-0.1.0/xdeps.egg-info/SOURCES.txt
--rw-r--r--   0 giadarol   (503) staff       (20)        1 2023-05-30 19:19:39.000000 xdeps-0.1.0/xdeps.egg-info/dependency_links.txt
--rw-r--r--   0 giadarol   (503) staff       (20)       21 2023-05-30 19:19:39.000000 xdeps-0.1.0/xdeps.egg-info/requires.txt
--rw-r--r--   0 giadarol   (503) staff       (20)        6 2023-05-30 19:19:39.000000 xdeps-0.1.0/xdeps.egg-info/top_level.txt
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-06-06 14:39:39.243203 xdeps-0.1.1/
+-rw-r--r--   0 giadarol   (503) staff       (20)    11356 2023-03-23 11:04:37.000000 xdeps-0.1.1/LICENSE
+-rw-r--r--   0 giadarol   (503) staff       (20)      559 2023-06-06 14:39:39.243002 xdeps-0.1.1/PKG-INFO
+-rw-r--r--   0 giadarol   (503) staff       (20)       38 2023-06-06 14:39:39.243276 xdeps-0.1.1/setup.cfg
+-rw-r--r--   0 giadarol   (503) staff       (20)     1253 2023-03-23 11:04:37.000000 xdeps-0.1.1/setup.py
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-06-06 14:39:39.234983 xdeps-0.1.1/xdeps/
+-rw-r--r--   0 giadarol   (503) staff       (20)      416 2023-06-06 14:39:09.000000 xdeps-0.1.1/xdeps/__init__.py
+-rw-r--r--   0 giadarol   (503) staff       (20)       22 2023-06-06 14:39:22.000000 xdeps-0.1.1/xdeps/_version.py
+-rw-r--r--   0 giadarol   (503) staff       (20)      160 2023-05-30 19:18:47.000000 xdeps-0.1.1/xdeps/general.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     5506 2023-04-05 12:43:31.000000 xdeps-0.1.1/xdeps/madxutils.py
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-06-06 14:39:39.242693 xdeps-0.1.1/xdeps/optimize/
+-rw-r--r--   0 giadarol   (503) staff       (20)      118 2023-05-30 19:18:47.000000 xdeps-0.1.1/xdeps/optimize/__init__.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     3511 2023-05-30 19:18:47.000000 xdeps-0.1.1/xdeps/optimize/jacobian.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    11173 2023-05-30 19:18:47.000000 xdeps-0.1.1/xdeps/optimize/optimize.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    21520 2023-05-30 19:18:47.000000 xdeps-0.1.1/xdeps/refs.py
+-rw-r--r--   0 giadarol   (503) staff       (20)     2093 2023-04-05 12:43:31.000000 xdeps-0.1.1/xdeps/sorting.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    16572 2023-06-06 14:39:09.000000 xdeps-0.1.1/xdeps/table.py
+-rw-r--r--   0 giadarol   (503) staff       (20)    14604 2023-05-23 20:23:29.000000 xdeps-0.1.1/xdeps/tasks.py
+-rw-r--r--   0 giadarol   (503) staff       (20)      932 2023-04-05 12:43:31.000000 xdeps-0.1.1/xdeps/utils.py
+drwxr-xr-x   0 giadarol   (503) staff       (20)        0 2023-06-06 14:39:39.241591 xdeps-0.1.1/xdeps.egg-info/
+-rw-r--r--   0 giadarol   (503) staff       (20)      559 2023-06-06 14:39:38.000000 xdeps-0.1.1/xdeps.egg-info/PKG-INFO
+-rw-r--r--   0 giadarol   (503) staff       (20)      389 2023-06-06 14:39:39.000000 xdeps-0.1.1/xdeps.egg-info/SOURCES.txt
+-rw-r--r--   0 giadarol   (503) staff       (20)        1 2023-06-06 14:39:38.000000 xdeps-0.1.1/xdeps.egg-info/dependency_links.txt
+-rw-r--r--   0 giadarol   (503) staff       (20)       21 2023-06-06 14:39:38.000000 xdeps-0.1.1/xdeps.egg-info/requires.txt
+-rw-r--r--   0 giadarol   (503) staff       (20)        6 2023-06-06 14:39:38.000000 xdeps-0.1.1/xdeps.egg-info/top_level.txt
```

### Comparing `xdeps-0.1.0/LICENSE` & `xdeps-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xdeps-0.1.0/PKG-INFO` & `xdeps-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xdeps
-Version: 0.1.0
+Version: 0.1.1
 Summary: Data dependency manager
 Home-page: https://xsuite.readthedocs.io/
 Download-URL: https://pypi.python.org/pypi/xdeps
 Author: Riccardo De Maria
 Author-email: riccardo.de.maria@cern.ch
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/xsuite/xsuite/issues
```

### Comparing `xdeps-0.1.0/setup.py` & `xdeps-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `xdeps-0.1.0/xdeps/madxutils.py` & `xdeps-0.1.1/xdeps/madxutils.py`

 * *Files identical despite different names*

### Comparing `xdeps-0.1.0/xdeps/optimize/jacobian.py` & `xdeps-0.1.1/xdeps/optimize/jacobian.py`

 * *Files identical despite different names*

### Comparing `xdeps-0.1.0/xdeps/optimize/optimize.py` & `xdeps-0.1.1/xdeps/optimize/optimize.py`

 * *Files identical despite different names*

### Comparing `xdeps-0.1.0/xdeps/refs.py` & `xdeps-0.1.1/xdeps/refs.py`

 * *Files identical despite different names*

### Comparing `xdeps-0.1.0/xdeps/sorting.py` & `xdeps-0.1.1/xdeps/sorting.py`

 * *Files identical despite different names*

### Comparing `xdeps-0.1.0/xdeps/tasks.py` & `xdeps-0.1.1/xdeps/tasks.py`

 * *Files identical despite different names*

### Comparing `xdeps-0.1.0/xdeps/utils.py` & `xdeps-0.1.1/xdeps/utils.py`

 * *Files identical despite different names*

### Comparing `xdeps-0.1.0/xdeps.egg-info/PKG-INFO` & `xdeps-0.1.1/xdeps.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xdeps
-Version: 0.1.0
+Version: 0.1.1
 Summary: Data dependency manager
 Home-page: https://xsuite.readthedocs.io/
 Download-URL: https://pypi.python.org/pypi/xdeps
 Author: Riccardo De Maria
 Author-email: riccardo.de.maria@cern.ch
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/xsuite/xsuite/issues
```

