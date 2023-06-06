# Comparing `tmp/watchmen_storage_oss-16.5.3.tar.gz` & `tmp/watchmen_storage_oss-16.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_storage_oss-16.5.3.tar", max compression
+gzip compressed data, was "watchmen_storage_oss-16.5.4.tar", max compression
```

## Comparing `watchmen_storage_oss-16.5.3.tar` & `watchmen_storage_oss-16.5.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1061 2023-06-05 01:29:03.560124 watchmen_storage_oss-16.5.3/LICENSE
--rw-r--r--   0        0        0      449 2023-06-05 01:29:03.560124 watchmen_storage_oss-16.5.3/pyproject.toml
--rw-r--r--   0        0        0      112 2023-06-05 01:29:03.560124 watchmen_storage_oss-16.5.3/src/watchmen_storage_oss/__init__.py
--rw-r--r--   0        0        0     1299 2023-06-05 01:29:03.560124 watchmen_storage_oss-16.5.3/src/watchmen_storage_oss/data_source_oss.py
--rw-r--r--   0        0        0      495 2023-06-05 01:29:03.560124 watchmen_storage_oss-16.5.3/src/watchmen_storage_oss/object_defs_oss.py
--rw-r--r--   0        0        0     1657 2023-06-05 01:29:03.560124 watchmen_storage_oss-16.5.3/src/watchmen_storage_oss/object_storage_service.py
--rw-r--r--   0        0        0     8903 2023-06-05 01:29:03.560124 watchmen_storage_oss-16.5.3/src/watchmen_storage_oss/storage_oss.py
--rw-r--r--   0        0        0     1836 2023-06-05 01:29:03.560124 watchmen_storage_oss-16.5.3/src/watchmen_storage_oss/storage_oss_configuration.py
--rw-r--r--   0        0        0      518 1970-01-01 00:00:00.000000 watchmen_storage_oss-16.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-06 01:45:59.161403 watchmen_storage_oss-16.5.4/LICENSE
+-rw-r--r--   0        0        0      449 2023-06-06 01:45:59.161403 watchmen_storage_oss-16.5.4/pyproject.toml
+-rw-r--r--   0        0        0      112 2023-06-06 01:45:59.161403 watchmen_storage_oss-16.5.4/src/watchmen_storage_oss/__init__.py
+-rw-r--r--   0        0        0     1299 2023-06-06 01:45:59.161403 watchmen_storage_oss-16.5.4/src/watchmen_storage_oss/data_source_oss.py
+-rw-r--r--   0        0        0      495 2023-06-06 01:45:59.161403 watchmen_storage_oss-16.5.4/src/watchmen_storage_oss/object_defs_oss.py
+-rw-r--r--   0        0        0     1657 2023-06-06 01:45:59.161403 watchmen_storage_oss-16.5.4/src/watchmen_storage_oss/object_storage_service.py
+-rw-r--r--   0        0        0     8903 2023-06-06 01:45:59.161403 watchmen_storage_oss-16.5.4/src/watchmen_storage_oss/storage_oss.py
+-rw-r--r--   0        0        0     1836 2023-06-06 01:45:59.161403 watchmen_storage_oss-16.5.4/src/watchmen_storage_oss/storage_oss_configuration.py
+-rw-r--r--   0        0        0      518 1970-01-01 00:00:00.000000 watchmen_storage_oss-16.5.4/PKG-INFO
```

### Comparing `watchmen_storage_oss-16.5.3/LICENSE` & `watchmen_storage_oss-16.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_storage_oss-16.5.3/src/watchmen_storage_oss/data_source_oss.py` & `watchmen_storage_oss-16.5.4/src/watchmen_storage_oss/data_source_oss.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_oss-16.5.3/src/watchmen_storage_oss/object_storage_service.py` & `watchmen_storage_oss-16.5.4/src/watchmen_storage_oss/object_storage_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_oss-16.5.3/src/watchmen_storage_oss/storage_oss.py` & `watchmen_storage_oss-16.5.4/src/watchmen_storage_oss/storage_oss.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_oss-16.5.3/src/watchmen_storage_oss/storage_oss_configuration.py` & `watchmen_storage_oss-16.5.4/src/watchmen_storage_oss/storage_oss_configuration.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_oss-16.5.3/PKG-INFO` & `watchmen_storage_oss-16.5.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: watchmen-storage-oss
-Version: 16.5.3
+Version: 16.5.4
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: oss2 (==2.15.0)
-Requires-Dist: watchmen-storage (==16.5.3)
+Requires-Dist: watchmen-storage (==16.5.4)
```

