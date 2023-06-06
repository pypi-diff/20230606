# Comparing `tmp/watchmen_storage_postgresql-16.5.5.tar.gz` & `tmp/watchmen_storage_postgresql-16.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_storage_postgresql-16.5.5.tar", max compression
+gzip compressed data, was "watchmen_storage_postgresql-16.5.6.tar", max compression
```

## Comparing `watchmen_storage_postgresql-16.5.5.tar` & `watchmen_storage_postgresql-16.5.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1061 2023-06-06 07:52:17.121012 watchmen_storage_postgresql-16.5.5/LICENSE
--rw-r--r--   0        0        0      478 2023-06-06 07:52:17.125012 watchmen_storage_postgresql-16.5.5/pyproject.toml
--rw-r--r--   0        0        0      309 2023-06-06 07:52:17.125012 watchmen_storage_postgresql-16.5.5/src/watchmen_storage_postgresql/__init__.py
--rw-r--r--   0        0        0     3557 2023-06-06 07:52:17.125012 watchmen_storage_postgresql-16.5.5/src/watchmen_storage_postgresql/data_source_postgresql.py
--rw-r--r--   0        0        0     2485 2023-06-06 07:52:17.125012 watchmen_storage_postgresql-16.5.5/src/watchmen_storage_postgresql/script_builder_postgresql.py
--rw-r--r--   0        0        0     7620 2023-06-06 07:52:17.125012 watchmen_storage_postgresql-16.5.5/src/watchmen_storage_postgresql/storage_postgresql.py
--rw-r--r--   0        0        0     2045 2023-06-06 07:52:17.125012 watchmen_storage_postgresql-16.5.5/src/watchmen_storage_postgresql/storage_postgresql_configuration.py
--rw-r--r--   0        0        0     7816 2023-06-06 07:52:17.125012 watchmen_storage_postgresql-16.5.5/src/watchmen_storage_postgresql/table_creator.py
--rw-r--r--   0        0        0    12688 2023-06-06 07:52:17.125012 watchmen_storage_postgresql-16.5.5/src/watchmen_storage_postgresql/where_build.py
--rw-r--r--   0        0        0      546 1970-01-01 00:00:00.000000 watchmen_storage_postgresql-16.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-06 17:50:48.823399 watchmen_storage_postgresql-16.5.6/LICENSE
+-rw-r--r--   0        0        0      478 2023-06-06 17:50:48.823399 watchmen_storage_postgresql-16.5.6/pyproject.toml
+-rw-r--r--   0        0        0      309 2023-06-06 17:50:48.823399 watchmen_storage_postgresql-16.5.6/src/watchmen_storage_postgresql/__init__.py
+-rw-r--r--   0        0        0     3557 2023-06-06 17:50:48.823399 watchmen_storage_postgresql-16.5.6/src/watchmen_storage_postgresql/data_source_postgresql.py
+-rw-r--r--   0        0        0     2485 2023-06-06 17:50:48.823399 watchmen_storage_postgresql-16.5.6/src/watchmen_storage_postgresql/script_builder_postgresql.py
+-rw-r--r--   0        0        0     7620 2023-06-06 17:50:48.823399 watchmen_storage_postgresql-16.5.6/src/watchmen_storage_postgresql/storage_postgresql.py
+-rw-r--r--   0        0        0     2045 2023-06-06 17:50:48.823399 watchmen_storage_postgresql-16.5.6/src/watchmen_storage_postgresql/storage_postgresql_configuration.py
+-rw-r--r--   0        0        0     7816 2023-06-06 17:50:48.823399 watchmen_storage_postgresql-16.5.6/src/watchmen_storage_postgresql/table_creator.py
+-rw-r--r--   0        0        0    12688 2023-06-06 17:50:48.823399 watchmen_storage_postgresql-16.5.6/src/watchmen_storage_postgresql/where_build.py
+-rw-r--r--   0        0        0      546 1970-01-01 00:00:00.000000 watchmen_storage_postgresql-16.5.6/PKG-INFO
```

### Comparing `watchmen_storage_postgresql-16.5.5/LICENSE` & `watchmen_storage_postgresql-16.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_storage_postgresql-16.5.5/src/watchmen_storage_postgresql/data_source_postgresql.py` & `watchmen_storage_postgresql-16.5.6/src/watchmen_storage_postgresql/data_source_postgresql.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_postgresql-16.5.5/src/watchmen_storage_postgresql/script_builder_postgresql.py` & `watchmen_storage_postgresql-16.5.6/src/watchmen_storage_postgresql/script_builder_postgresql.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_postgresql-16.5.5/src/watchmen_storage_postgresql/storage_postgresql.py` & `watchmen_storage_postgresql-16.5.6/src/watchmen_storage_postgresql/storage_postgresql.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_postgresql-16.5.5/src/watchmen_storage_postgresql/storage_postgresql_configuration.py` & `watchmen_storage_postgresql-16.5.6/src/watchmen_storage_postgresql/storage_postgresql_configuration.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_postgresql-16.5.5/src/watchmen_storage_postgresql/table_creator.py` & `watchmen_storage_postgresql-16.5.6/src/watchmen_storage_postgresql/table_creator.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_postgresql-16.5.5/src/watchmen_storage_postgresql/where_build.py` & `watchmen_storage_postgresql-16.5.6/src/watchmen_storage_postgresql/where_build.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_postgresql-16.5.5/PKG-INFO` & `watchmen_storage_postgresql-16.5.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: watchmen-storage-postgresql
-Version: 16.5.5
+Version: 16.5.6
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
 Requires-Dist: psycopg2-binary (>=2.9.3,<3.0.0)
-Requires-Dist: watchmen-storage-rds (==16.5.5)
+Requires-Dist: watchmen-storage-rds (==16.5.6)
```

