# Comparing `tmp/python-messytable-handler-0.1.0.tar.gz` & `tmp/python-messytable-handler-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-messytable-handler-0.1.0.tar", last modified: Fri May  5 16:50:06 2023, max compression
+gzip compressed data, was "python-messytable-handler-0.2.3.tar", last modified: Tue Jun  6 15:59:45 2023, max compression
```

## Comparing `python-messytable-handler-0.1.0.tar` & `python-messytable-handler-0.2.3.tar`

### file list

```diff
@@ -1,38 +1,36 @@
-drwxr-x---   0 davidharcombe (261421) primarygroup (89939)        0 2023-05-05 16:50:06.927028 python-messytable-handler-0.1.0/
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)      996 2023-05-05 16:50:06.927028 python-messytable-handler-0.1.0/PKG-INFO
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)      841 2023-05-05 16:36:19.000000 python-messytable-handler-0.1.0/README.md
-drwxr-x---   0 davidharcombe (261421) primarygroup (89939)        0 2023-05-05 16:50:06.923028 python-messytable-handler-0.1.0/messytables/
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     1081 2023-05-05 16:36:19.000000 python-messytable-handler-0.1.0/messytables/__init__.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     6222 2023-05-05 16:36:19.000000 python-messytable-handler-0.1.0/messytables/any.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     7034 2023-05-05 16:36:19.000000 python-messytable-handler-0.1.0/messytables/commas.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)      486 2023-05-05 16:36:19.000000 python-messytable-handler-0.1.0/messytables/compat23.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     7596 2023-05-05 16:38:17.000000 python-messytable-handler-0.1.0/messytables/core.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     2152 2023-05-05 16:36:19.000000 python-messytable-handler-0.1.0/messytables/dateparser.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)      411 2023-05-05 16:36:19.000000 python-messytable-handler-0.1.0/messytables/error.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     8762 2023-05-05 16:36:19.000000 python-messytable-handler-0.1.0/messytables/excel.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     3666 2023-05-05 16:36:19.000000 python-messytable-handler-0.1.0/messytables/headers.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     8075 2023-05-05 16:36:19.000000 python-messytable-handler-0.1.0/messytables/html.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     1304 2023-05-05 16:36:19.000000 python-messytable-handler-0.1.0/messytables/jts.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     7592 2023-05-05 16:36:19.000000 python-messytable-handler-0.1.0/messytables/ods.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)    10128 2023-05-05 16:36:19.000000 python-messytable-handler-0.1.0/messytables/types.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     3179 2023-05-05 16:36:19.000000 python-messytable-handler-0.1.0/messytables/util.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     1201 2023-05-05 16:36:19.000000 python-messytable-handler-0.1.0/messytables/zip.py
-drwxr-x---   0 davidharcombe (261421) primarygroup (89939)        0 2023-05-05 16:50:06.923028 python-messytable-handler-0.1.0/python_messytable_handler.egg-info/
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)      996 2023-05-05 16:50:06.000000 python-messytable-handler-0.1.0/python_messytable_handler.egg-info/PKG-INFO
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)      847 2023-05-05 16:50:06.000000 python-messytable-handler-0.1.0/python_messytable_handler.egg-info/SOURCES.txt
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)        1 2023-05-05 16:50:06.000000 python-messytable-handler-0.1.0/python_messytable_handler.egg-info/dependency_links.txt
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)        1 2023-05-05 16:50:06.000000 python-messytable-handler-0.1.0/python_messytable_handler.egg-info/namespace_packages.txt
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)        1 2023-05-05 16:50:06.000000 python-messytable-handler-0.1.0/python_messytable_handler.egg-info/not-zip-safe
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)      139 2023-05-05 16:50:06.000000 python-messytable-handler-0.1.0/python_messytable_handler.egg-info/requires.txt
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)       12 2023-05-05 16:50:06.000000 python-messytable-handler-0.1.0/python_messytable_handler.egg-info/top_level.txt
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)       38 2023-05-05 16:50:06.927028 python-messytable-handler-0.1.0/setup.cfg
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     1750 2023-05-05 16:47:35.000000 python-messytable-handler-0.1.0/setup.py
-drwxr-x---   0 davidharcombe (261421) primarygroup (89939)        0 2023-05-05 16:50:06.927028 python-messytable-handler-0.1.0/test/
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     2301 2023-05-05 16:36:19.000000 python-messytable-handler-0.1.0/test/test_any.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     6546 2023-05-05 16:36:19.000000 python-messytable-handler-0.1.0/test/test_guessing.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     7234 2023-05-05 16:36:19.000000 python-messytable-handler-0.1.0/test/test_properties.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)    24915 2023-05-05 16:36:19.000000 python-messytable-handler-0.1.0/test/test_read.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)      536 2023-05-05 16:36:19.000000 python-messytable-handler-0.1.0/test/test_rowset.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)     2706 2023-05-05 16:36:19.000000 python-messytable-handler-0.1.0/test/test_stream.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)      916 2023-05-05 16:36:19.000000 python-messytable-handler-0.1.0/test/test_tableset.py
--rw-r-----   0 davidharcombe (261421) primarygroup (89939)      656 2023-05-05 16:36:19.000000 python-messytable-handler-0.1.0/test/test_unit.py
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-06 15:59:45.718475 python-messytable-handler-0.2.3/
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1434 2023-06-06 15:59:45.718475 python-messytable-handler-0.2.3/PKG-INFO
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)      841 2023-06-06 15:40:21.000000 python-messytable-handler-0.2.3/README.md
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-06 15:59:45.714475 python-messytable-handler-0.2.3/messytables/
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     1081 2023-06-06 15:40:21.000000 python-messytable-handler-0.2.3/messytables/__init__.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     6222 2023-06-06 15:40:21.000000 python-messytable-handler-0.2.3/messytables/any.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     7034 2023-06-06 15:40:21.000000 python-messytable-handler-0.2.3/messytables/commas.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)      486 2023-06-06 15:40:21.000000 python-messytable-handler-0.2.3/messytables/compat23.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     7596 2023-06-06 15:40:21.000000 python-messytable-handler-0.2.3/messytables/core.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     2152 2023-06-06 15:40:21.000000 python-messytable-handler-0.2.3/messytables/dateparser.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)      411 2023-06-06 15:40:21.000000 python-messytable-handler-0.2.3/messytables/error.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     8762 2023-06-06 15:40:21.000000 python-messytable-handler-0.2.3/messytables/excel.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     3666 2023-06-06 15:40:21.000000 python-messytable-handler-0.2.3/messytables/headers.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     8075 2023-06-06 15:40:21.000000 python-messytable-handler-0.2.3/messytables/html.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     1304 2023-06-06 15:40:21.000000 python-messytable-handler-0.2.3/messytables/jts.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     7592 2023-06-06 15:40:21.000000 python-messytable-handler-0.2.3/messytables/ods.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)    10128 2023-06-06 15:40:21.000000 python-messytable-handler-0.2.3/messytables/types.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     3179 2023-06-06 15:40:21.000000 python-messytable-handler-0.2.3/messytables/util.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     1201 2023-06-06 15:40:21.000000 python-messytable-handler-0.2.3/messytables/zip.py
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1506 2023-06-06 15:58:59.000000 python-messytable-handler-0.2.3/pyproject.toml
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-06 15:59:45.718475 python-messytable-handler-0.2.3/python_messytable_handler.egg-info/
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)     1434 2023-06-06 15:59:45.000000 python-messytable-handler-0.2.3/python_messytable_handler.egg-info/PKG-INFO
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      747 2023-06-06 15:59:45.000000 python-messytable-handler-0.2.3/python_messytable_handler.egg-info/SOURCES.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)        1 2023-06-06 15:59:45.000000 python-messytable-handler-0.2.3/python_messytable_handler.egg-info/dependency_links.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)      139 2023-06-06 15:59:45.000000 python-messytable-handler-0.2.3/python_messytable_handler.egg-info/requires.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       12 2023-06-06 15:59:45.000000 python-messytable-handler-0.2.3/python_messytable_handler.egg-info/top_level.txt
+-rw-r--r--   0 davidharcombe (261421) primarygroup (89939)       38 2023-06-06 15:59:45.718475 python-messytable-handler-0.2.3/setup.cfg
+drwxr-xr-x   0 davidharcombe (261421) primarygroup (89939)        0 2023-06-06 15:59:45.718475 python-messytable-handler-0.2.3/test/
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     2301 2023-06-06 15:40:21.000000 python-messytable-handler-0.2.3/test/test_any.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     6546 2023-06-06 15:40:21.000000 python-messytable-handler-0.2.3/test/test_guessing.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     7234 2023-06-06 15:40:21.000000 python-messytable-handler-0.2.3/test/test_properties.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)    24915 2023-06-06 15:40:21.000000 python-messytable-handler-0.2.3/test/test_read.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)      536 2023-06-06 15:40:21.000000 python-messytable-handler-0.2.3/test/test_rowset.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)     2706 2023-06-06 15:40:21.000000 python-messytable-handler-0.2.3/test/test_stream.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)      916 2023-06-06 15:40:21.000000 python-messytable-handler-0.2.3/test/test_tableset.py
+-rw-r-----   0 davidharcombe (261421) primarygroup (89939)      656 2023-06-06 15:40:21.000000 python-messytable-handler-0.2.3/test/test_unit.py
```

### Comparing `python-messytable-handler-0.1.0/README.md` & `python-messytable-handler-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `python-messytable-handler-0.1.0/messytables/__init__.py` & `python-messytable-handler-0.2.3/messytables/__init__.py`

 * *Files identical despite different names*

### Comparing `python-messytable-handler-0.1.0/messytables/any.py` & `python-messytable-handler-0.2.3/messytables/any.py`

 * *Files identical despite different names*

### Comparing `python-messytable-handler-0.1.0/messytables/commas.py` & `python-messytable-handler-0.2.3/messytables/commas.py`

 * *Files identical despite different names*

### Comparing `python-messytable-handler-0.1.0/messytables/core.py` & `python-messytable-handler-0.2.3/messytables/core.py`

 * *Files identical despite different names*

### Comparing `python-messytable-handler-0.1.0/messytables/dateparser.py` & `python-messytable-handler-0.2.3/messytables/dateparser.py`

 * *Files identical despite different names*

### Comparing `python-messytable-handler-0.1.0/messytables/excel.py` & `python-messytable-handler-0.2.3/messytables/excel.py`

 * *Files identical despite different names*

### Comparing `python-messytable-handler-0.1.0/messytables/headers.py` & `python-messytable-handler-0.2.3/messytables/headers.py`

 * *Files identical despite different names*

### Comparing `python-messytable-handler-0.1.0/messytables/html.py` & `python-messytable-handler-0.2.3/messytables/html.py`

 * *Files identical despite different names*

### Comparing `python-messytable-handler-0.1.0/messytables/jts.py` & `python-messytable-handler-0.2.3/messytables/jts.py`

 * *Files identical despite different names*

### Comparing `python-messytable-handler-0.1.0/messytables/ods.py` & `python-messytable-handler-0.2.3/messytables/ods.py`

 * *Files identical despite different names*

### Comparing `python-messytable-handler-0.1.0/messytables/types.py` & `python-messytable-handler-0.2.3/messytables/types.py`

 * *Files identical despite different names*

### Comparing `python-messytable-handler-0.1.0/messytables/util.py` & `python-messytable-handler-0.2.3/messytables/util.py`

 * *Files identical despite different names*

### Comparing `python-messytable-handler-0.1.0/messytables/zip.py` & `python-messytable-handler-0.2.3/messytables/zip.py`

 * *Files identical despite different names*

### Comparing `python-messytable-handler-0.1.0/python_messytable_handler.egg-info/SOURCES.txt` & `python-messytable-handler-0.2.3/python_messytable_handler.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 README.md
-setup.py
+pyproject.toml
 messytables/__init__.py
 messytables/any.py
 messytables/commas.py
 messytables/compat23.py
 messytables/core.py
 messytables/dateparser.py
 messytables/error.py
@@ -14,16 +14,14 @@
 messytables/ods.py
 messytables/types.py
 messytables/util.py
 messytables/zip.py
 python_messytable_handler.egg-info/PKG-INFO
 python_messytable_handler.egg-info/SOURCES.txt
 python_messytable_handler.egg-info/dependency_links.txt
-python_messytable_handler.egg-info/namespace_packages.txt
-python_messytable_handler.egg-info/not-zip-safe
 python_messytable_handler.egg-info/requires.txt
 python_messytable_handler.egg-info/top_level.txt
 test/test_any.py
 test/test_guessing.py
 test/test_properties.py
 test/test_read.py
 test/test_rowset.py
```

### Comparing `python-messytable-handler-0.1.0/test/test_any.py` & `python-messytable-handler-0.2.3/test/test_any.py`

 * *Files identical despite different names*

### Comparing `python-messytable-handler-0.1.0/test/test_guessing.py` & `python-messytable-handler-0.2.3/test/test_guessing.py`

 * *Files identical despite different names*

### Comparing `python-messytable-handler-0.1.0/test/test_properties.py` & `python-messytable-handler-0.2.3/test/test_properties.py`

 * *Files identical despite different names*

### Comparing `python-messytable-handler-0.1.0/test/test_read.py` & `python-messytable-handler-0.2.3/test/test_read.py`

 * *Files identical despite different names*

### Comparing `python-messytable-handler-0.1.0/test/test_rowset.py` & `python-messytable-handler-0.2.3/test/test_rowset.py`

 * *Files identical despite different names*

### Comparing `python-messytable-handler-0.1.0/test/test_stream.py` & `python-messytable-handler-0.2.3/test/test_stream.py`

 * *Files identical despite different names*

### Comparing `python-messytable-handler-0.1.0/test/test_tableset.py` & `python-messytable-handler-0.2.3/test/test_tableset.py`

 * *Files identical despite different names*

### Comparing `python-messytable-handler-0.1.0/test/test_unit.py` & `python-messytable-handler-0.2.3/test/test_unit.py`

 * *Files identical despite different names*

