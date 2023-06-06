# Comparing `tmp/watchmen_storage_s3-16.5.4.tar.gz` & `tmp/watchmen_storage_s3-16.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_storage_s3-16.5.4.tar", max compression
+gzip compressed data, was "watchmen_storage_s3-16.5.5.tar", max compression
```

## Comparing `watchmen_storage_s3-16.5.4.tar` & `watchmen_storage_s3-16.5.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1061 2023-06-06 01:45:59.165403 watchmen_storage_s3-16.5.4/LICENSE
--rw-r--r--   0        0        0      450 2023-06-06 01:45:59.165403 watchmen_storage_s3-16.5.4/pyproject.toml
--rw-r--r--   0        0        0      180 2023-06-06 01:45:59.165403 watchmen_storage_s3-16.5.4/src/watchmen_storage_s3/__init__.py
--rw-r--r--   0        0        0     1308 2023-06-06 01:45:59.165403 watchmen_storage_s3-16.5.4/src/watchmen_storage_s3/data_source_s3.py
--rw-r--r--   0        0        0     1001 2023-06-06 01:45:59.165403 watchmen_storage_s3-16.5.4/src/watchmen_storage_s3/object_defs_s3.py
--rw-r--r--   0        0        0     3750 2023-06-06 01:45:59.165403 watchmen_storage_s3-16.5.4/src/watchmen_storage_s3/simple_storage_service.py
--rw-r--r--   0        0        0     8836 2023-06-06 01:45:59.165403 watchmen_storage_s3-16.5.4/src/watchmen_storage_s3/storage_s3.py
--rw-r--r--   0        0        0     1818 2023-06-06 01:45:59.165403 watchmen_storage_s3-16.5.4/src/watchmen_storage_s3/storage_s3_configuration.py
--rw-r--r--   0        0        0      526 1970-01-01 00:00:00.000000 watchmen_storage_s3-16.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-06 07:52:17.125012 watchmen_storage_s3-16.5.5/LICENSE
+-rw-r--r--   0        0        0      431 2023-06-06 07:52:17.125012 watchmen_storage_s3-16.5.5/pyproject.toml
+-rw-r--r--   0        0        0      180 2023-06-06 07:52:17.125012 watchmen_storage_s3-16.5.5/src/watchmen_storage_s3/__init__.py
+-rw-r--r--   0        0        0     1308 2023-06-06 07:52:17.125012 watchmen_storage_s3-16.5.5/src/watchmen_storage_s3/data_source_s3.py
+-rw-r--r--   0        0        0     1001 2023-06-06 07:52:17.125012 watchmen_storage_s3-16.5.5/src/watchmen_storage_s3/object_defs_s3.py
+-rw-r--r--   0        0        0     3750 2023-06-06 07:52:17.125012 watchmen_storage_s3-16.5.5/src/watchmen_storage_s3/simple_storage_service.py
+-rw-r--r--   0        0        0     8836 2023-06-06 07:52:17.125012 watchmen_storage_s3-16.5.5/src/watchmen_storage_s3/storage_s3.py
+-rw-r--r--   0        0        0     1818 2023-06-06 07:52:17.125012 watchmen_storage_s3-16.5.5/src/watchmen_storage_s3/storage_s3_configuration.py
+-rw-r--r--   0        0        0      486 1970-01-01 00:00:00.000000 watchmen_storage_s3-16.5.5/PKG-INFO
```

### Comparing `watchmen_storage_s3-16.5.4/LICENSE` & `watchmen_storage_s3-16.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_storage_s3-16.5.4/src/watchmen_storage_s3/data_source_s3.py` & `watchmen_storage_s3-16.5.5/src/watchmen_storage_s3/data_source_s3.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_s3-16.5.4/src/watchmen_storage_s3/object_defs_s3.py` & `watchmen_storage_s3-16.5.5/src/watchmen_storage_s3/object_defs_s3.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_s3-16.5.4/src/watchmen_storage_s3/simple_storage_service.py` & `watchmen_storage_s3-16.5.5/src/watchmen_storage_s3/simple_storage_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_s3-16.5.4/src/watchmen_storage_s3/storage_s3.py` & `watchmen_storage_s3-16.5.5/src/watchmen_storage_s3/storage_s3.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_s3-16.5.4/src/watchmen_storage_s3/storage_s3_configuration.py` & `watchmen_storage_s3-16.5.5/src/watchmen_storage_s3/storage_s3_configuration.py`

 * *Files identical despite different names*

