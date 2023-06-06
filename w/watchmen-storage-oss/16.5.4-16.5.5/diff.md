# Comparing `tmp/watchmen_storage_oss-16.5.4.tar.gz` & `tmp/watchmen_storage_oss-16.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_storage_oss-16.5.4.tar", max compression
+gzip compressed data, was "watchmen_storage_oss-16.5.5.tar", max compression
```

## Comparing `watchmen_storage_oss-16.5.4.tar` & `watchmen_storage_oss-16.5.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1061 2023-06-06 01:45:59.161403 watchmen_storage_oss-16.5.4/LICENSE
--rw-r--r--   0        0        0      449 2023-06-06 01:45:59.161403 watchmen_storage_oss-16.5.4/pyproject.toml
--rw-r--r--   0        0        0      112 2023-06-06 01:45:59.161403 watchmen_storage_oss-16.5.4/src/watchmen_storage_oss/__init__.py
--rw-r--r--   0        0        0     1299 2023-06-06 01:45:59.161403 watchmen_storage_oss-16.5.4/src/watchmen_storage_oss/data_source_oss.py
--rw-r--r--   0        0        0      495 2023-06-06 01:45:59.161403 watchmen_storage_oss-16.5.4/src/watchmen_storage_oss/object_defs_oss.py
--rw-r--r--   0        0        0     1657 2023-06-06 01:45:59.161403 watchmen_storage_oss-16.5.4/src/watchmen_storage_oss/object_storage_service.py
--rw-r--r--   0        0        0     8903 2023-06-06 01:45:59.161403 watchmen_storage_oss-16.5.4/src/watchmen_storage_oss/storage_oss.py
--rw-r--r--   0        0        0     1836 2023-06-06 01:45:59.161403 watchmen_storage_oss-16.5.4/src/watchmen_storage_oss/storage_oss_configuration.py
--rw-r--r--   0        0        0      518 1970-01-01 00:00:00.000000 watchmen_storage_oss-16.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-06 07:52:17.121012 watchmen_storage_oss-16.5.5/LICENSE
+-rw-r--r--   0        0        0      449 2023-06-06 07:52:17.121012 watchmen_storage_oss-16.5.5/pyproject.toml
+-rw-r--r--   0        0        0      112 2023-06-06 07:52:17.121012 watchmen_storage_oss-16.5.5/src/watchmen_storage_oss/__init__.py
+-rw-r--r--   0        0        0     1299 2023-06-06 07:52:17.121012 watchmen_storage_oss-16.5.5/src/watchmen_storage_oss/data_source_oss.py
+-rw-r--r--   0        0        0      495 2023-06-06 07:52:17.121012 watchmen_storage_oss-16.5.5/src/watchmen_storage_oss/object_defs_oss.py
+-rw-r--r--   0        0        0     1657 2023-06-06 07:52:17.121012 watchmen_storage_oss-16.5.5/src/watchmen_storage_oss/object_storage_service.py
+-rw-r--r--   0        0        0     8903 2023-06-06 07:52:17.121012 watchmen_storage_oss-16.5.5/src/watchmen_storage_oss/storage_oss.py
+-rw-r--r--   0        0        0     1836 2023-06-06 07:52:17.121012 watchmen_storage_oss-16.5.5/src/watchmen_storage_oss/storage_oss_configuration.py
+-rw-r--r--   0        0        0      518 1970-01-01 00:00:00.000000 watchmen_storage_oss-16.5.5/PKG-INFO
```

### Comparing `watchmen_storage_oss-16.5.4/LICENSE` & `watchmen_storage_oss-16.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_storage_oss-16.5.4/src/watchmen_storage_oss/data_source_oss.py` & `watchmen_storage_oss-16.5.5/src/watchmen_storage_oss/data_source_oss.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_oss-16.5.4/src/watchmen_storage_oss/object_storage_service.py` & `watchmen_storage_oss-16.5.5/src/watchmen_storage_oss/object_storage_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_oss-16.5.4/src/watchmen_storage_oss/storage_oss.py` & `watchmen_storage_oss-16.5.5/src/watchmen_storage_oss/storage_oss.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_oss-16.5.4/src/watchmen_storage_oss/storage_oss_configuration.py` & `watchmen_storage_oss-16.5.5/src/watchmen_storage_oss/storage_oss_configuration.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_oss-16.5.4/PKG-INFO` & `watchmen_storage_oss-16.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: watchmen-storage-oss
-Version: 16.5.4
+Version: 16.5.5
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
-Requires-Dist: watchmen-storage (==16.5.4)
+Requires-Dist: watchmen-storage (==16.5.5)
```

