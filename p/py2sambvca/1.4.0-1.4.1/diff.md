# Comparing `tmp/py2sambvca-1.4.0.tar.gz` & `tmp/py2sambvca-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py2sambvca-1.4.0.tar", last modified: Sat Jun  3 19:47:04 2023, max compression
+gzip compressed data, was "py2sambvca-1.4.1.tar", last modified: Tue Jun  6 13:56:21 2023, max compression
```

## Comparing `py2sambvca-1.4.0.tar` & `py2sambvca-1.4.1.tar`

### file list

```diff
@@ -1,17 +1,22 @@
-drwxrwxr-x   0 jackson   (1000) jackson   (1000)        0 2023-06-03 19:47:04.459173 py2sambvca-1.4.0/
--rw-r--r--   0 jackson   (1000) jackson   (1000)    35129 2023-02-05 17:11:46.000000 py2sambvca-1.4.0/LICENSE
--rw-rw-r--   0 jackson   (1000) jackson   (1000)     8111 2023-06-03 19:47:04.459173 py2sambvca-1.4.0/PKG-INFO
--rw-r--r--   0 jackson   (1000) jackson   (1000)     7468 2023-06-03 19:01:26.000000 py2sambvca-1.4.0/README.md
-drwxrwxr-x   0 jackson   (1000) jackson   (1000)        0 2023-06-03 19:47:04.459173 py2sambvca-1.4.0/py2sambvca/
--rw-r--r--   0 jackson   (1000) jackson   (1000)       84 2023-06-03 19:45:53.000000 py2sambvca-1.4.0/py2sambvca/__init__.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)    18655 2023-06-03 19:38:22.000000 py2sambvca-1.4.0/py2sambvca/py2sambvca.py
-drwxrwxr-x   0 jackson   (1000) jackson   (1000)        0 2023-06-03 19:47:04.459173 py2sambvca-1.4.0/py2sambvca.egg-info/
--rw-rw-r--   0 jackson   (1000) jackson   (1000)     8111 2023-06-03 19:47:04.000000 py2sambvca-1.4.0/py2sambvca.egg-info/PKG-INFO
--rw-rw-r--   0 jackson   (1000) jackson   (1000)      261 2023-06-03 19:47:04.000000 py2sambvca-1.4.0/py2sambvca.egg-info/SOURCES.txt
--rw-rw-r--   0 jackson   (1000) jackson   (1000)        1 2023-06-03 19:47:04.000000 py2sambvca-1.4.0/py2sambvca.egg-info/dependency_links.txt
--rw-rw-r--   0 jackson   (1000) jackson   (1000)       11 2023-06-03 19:47:04.000000 py2sambvca-1.4.0/py2sambvca.egg-info/top_level.txt
--rw-rw-r--   0 jackson   (1000) jackson   (1000)       38 2023-06-03 19:47:04.459173 py2sambvca-1.4.0/setup.cfg
--rw-r--r--   0 jackson   (1000) jackson   (1000)     1483 2023-06-03 16:19:52.000000 py2sambvca-1.4.0/setup.py
-drwxrwxr-x   0 jackson   (1000) jackson   (1000)        0 2023-06-03 19:47:04.459173 py2sambvca-1.4.0/test/
--rw-r--r--   0 jackson   (1000) jackson   (1000)    13614 2023-06-03 19:13:59.000000 py2sambvca-1.4.0/test/test_py2sambvca.py
--rw-r--r--   0 jackson   (1000) jackson   (1000)     1783 2023-06-03 16:19:52.000000 py2sambvca-1.4.0/test/test_static_output.py
+drwxrwxr-x   0 jackson   (1000) jackson   (1000)        0 2023-06-06 13:56:21.741900 py2sambvca-1.4.1/
+-rw-r--r--   0 jackson   (1000) jackson   (1000)    35129 2023-02-05 17:11:46.000000 py2sambvca-1.4.1/LICENSE
+-rw-rw-r--   0 jackson   (1000) jackson   (1000)     8111 2023-06-06 13:56:21.741900 py2sambvca-1.4.1/PKG-INFO
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     7468 2023-06-03 19:01:26.000000 py2sambvca-1.4.1/README.md
+drwxrwxr-x   0 jackson   (1000) jackson   (1000)        0 2023-06-06 13:56:21.737900 py2sambvca-1.4.1/py2sambvca/
+-rw-r--r--   0 jackson   (1000) jackson   (1000)       84 2023-06-06 13:55:41.000000 py2sambvca-1.4.1/py2sambvca/__init__.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)    18655 2023-06-03 19:38:22.000000 py2sambvca-1.4.1/py2sambvca/py2sambvca.py
+drwxrwxr-x   0 jackson   (1000) jackson   (1000)        0 2023-06-06 13:56:21.737900 py2sambvca-1.4.1/py2sambvca/radii_tables/
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      330 2023-06-03 19:40:00.000000 py2sambvca-1.4.1/py2sambvca/radii_tables/__init__.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     1767 2023-06-03 19:03:43.000000 py2sambvca-1.4.1/py2sambvca/radii_tables/default.py
+-rw-rw-r--   0 jackson   (1000) jackson   (1000)      800 2023-06-03 19:31:48.000000 py2sambvca-1.4.1/py2sambvca/radii_tables/format_table.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)      315 2023-06-03 19:21:26.000000 py2sambvca-1.4.1/py2sambvca/radii_tables/vanDerWaals.py
+drwxrwxr-x   0 jackson   (1000) jackson   (1000)        0 2023-06-06 13:56:21.737900 py2sambvca-1.4.1/py2sambvca.egg-info/
+-rw-rw-r--   0 jackson   (1000) jackson   (1000)     8111 2023-06-06 13:56:21.000000 py2sambvca-1.4.1/py2sambvca.egg-info/PKG-INFO
+-rw-rw-r--   0 jackson   (1000) jackson   (1000)      411 2023-06-06 13:56:21.000000 py2sambvca-1.4.1/py2sambvca.egg-info/SOURCES.txt
+-rw-rw-r--   0 jackson   (1000) jackson   (1000)        1 2023-06-06 13:56:21.000000 py2sambvca-1.4.1/py2sambvca.egg-info/dependency_links.txt
+-rw-rw-r--   0 jackson   (1000) jackson   (1000)       11 2023-06-06 13:56:21.000000 py2sambvca-1.4.1/py2sambvca.egg-info/top_level.txt
+-rw-rw-r--   0 jackson   (1000) jackson   (1000)       38 2023-06-06 13:56:21.741900 py2sambvca-1.4.1/setup.cfg
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     1510 2023-06-06 13:55:41.000000 py2sambvca-1.4.1/setup.py
+drwxrwxr-x   0 jackson   (1000) jackson   (1000)        0 2023-06-06 13:56:21.741900 py2sambvca-1.4.1/test/
+-rw-r--r--   0 jackson   (1000) jackson   (1000)    13614 2023-06-03 19:13:59.000000 py2sambvca-1.4.1/test/test_py2sambvca.py
+-rw-r--r--   0 jackson   (1000) jackson   (1000)     1783 2023-06-03 16:19:52.000000 py2sambvca-1.4.1/test/test_static_output.py
```

### Comparing `py2sambvca-1.4.0/LICENSE` & `py2sambvca-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py2sambvca-1.4.0/PKG-INFO` & `py2sambvca-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2sambvca
-Version: 1.4.0
+Version: 1.4.1
 Summary: Simple thin client to interface python scripts with SambVca catalytic pocket Fortran calculator.
 Home-page: https://github.com/JacksonBurns/py2sambvca
 Author: Jackson Burns
 License: GNU GPLv3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `py2sambvca-1.4.0/README.md` & `py2sambvca-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `py2sambvca-1.4.0/py2sambvca/py2sambvca.py` & `py2sambvca-1.4.1/py2sambvca/py2sambvca.py`

 * *Files identical despite different names*

### Comparing `py2sambvca-1.4.0/py2sambvca.egg-info/PKG-INFO` & `py2sambvca-1.4.1/py2sambvca.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2sambvca
-Version: 1.4.0
+Version: 1.4.1
 Summary: Simple thin client to interface python scripts with SambVca catalytic pocket Fortran calculator.
 Home-page: https://github.com/JacksonBurns/py2sambvca
 Author: Jackson Burns
 License: GNU GPLv3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `py2sambvca-1.4.0/setup.py` & `py2sambvca-1.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,10 +39,10 @@
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
-    packages=["py2sambvca"],
+    packages=["py2sambvca", "py2sambvca.radii_tables"],
     include_package_data=True
 )
```

### Comparing `py2sambvca-1.4.0/test/test_py2sambvca.py` & `py2sambvca-1.4.1/test/test_py2sambvca.py`

 * *Files identical despite different names*

### Comparing `py2sambvca-1.4.0/test/test_static_output.py` & `py2sambvca-1.4.1/test/test_static_output.py`

 * *Files identical despite different names*

