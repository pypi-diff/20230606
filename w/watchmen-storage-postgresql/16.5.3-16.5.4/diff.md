# Comparing `tmp/watchmen_storage_postgresql-16.5.3.tar.gz` & `tmp/watchmen_storage_postgresql-16.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_storage_postgresql-16.5.3.tar", max compression
+gzip compressed data, was "watchmen_storage_postgresql-16.5.4.tar", max compression
```

## Comparing `watchmen_storage_postgresql-16.5.3.tar` & `watchmen_storage_postgresql-16.5.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1061 2023-06-05 01:29:03.560124 watchmen_storage_postgresql-16.5.3/LICENSE
--rw-r--r--   0        0        0      478 2023-06-05 01:29:03.564124 watchmen_storage_postgresql-16.5.3/pyproject.toml
--rw-r--r--   0        0        0      309 2023-06-05 01:29:03.564124 watchmen_storage_postgresql-16.5.3/src/watchmen_storage_postgresql/__init__.py
--rw-r--r--   0        0        0     3557 2023-06-05 01:29:03.564124 watchmen_storage_postgresql-16.5.3/src/watchmen_storage_postgresql/data_source_postgresql.py
--rw-r--r--   0        0        0     2485 2023-06-05 01:29:03.564124 watchmen_storage_postgresql-16.5.3/src/watchmen_storage_postgresql/script_builder_postgresql.py
--rw-r--r--   0        0        0     7620 2023-06-05 01:29:03.564124 watchmen_storage_postgresql-16.5.3/src/watchmen_storage_postgresql/storage_postgresql.py
--rw-r--r--   0        0        0     2045 2023-06-05 01:29:03.564124 watchmen_storage_postgresql-16.5.3/src/watchmen_storage_postgresql/storage_postgresql_configuration.py
--rw-r--r--   0        0        0     7816 2023-06-05 01:29:03.564124 watchmen_storage_postgresql-16.5.3/src/watchmen_storage_postgresql/table_creator.py
--rw-r--r--   0        0        0    12688 2023-06-05 01:29:03.564124 watchmen_storage_postgresql-16.5.3/src/watchmen_storage_postgresql/where_build.py
--rw-r--r--   0        0        0      546 1970-01-01 00:00:00.000000 watchmen_storage_postgresql-16.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-06 01:45:59.161403 watchmen_storage_postgresql-16.5.4/LICENSE
+-rw-r--r--   0        0        0      478 2023-06-06 01:45:59.165403 watchmen_storage_postgresql-16.5.4/pyproject.toml
+-rw-r--r--   0        0        0      309 2023-06-06 01:45:59.165403 watchmen_storage_postgresql-16.5.4/src/watchmen_storage_postgresql/__init__.py
+-rw-r--r--   0        0        0     3557 2023-06-06 01:45:59.165403 watchmen_storage_postgresql-16.5.4/src/watchmen_storage_postgresql/data_source_postgresql.py
+-rw-r--r--   0        0        0     2485 2023-06-06 01:45:59.165403 watchmen_storage_postgresql-16.5.4/src/watchmen_storage_postgresql/script_builder_postgresql.py
+-rw-r--r--   0        0        0     7620 2023-06-06 01:45:59.165403 watchmen_storage_postgresql-16.5.4/src/watchmen_storage_postgresql/storage_postgresql.py
+-rw-r--r--   0        0        0     2045 2023-06-06 01:45:59.165403 watchmen_storage_postgresql-16.5.4/src/watchmen_storage_postgresql/storage_postgresql_configuration.py
+-rw-r--r--   0        0        0     7816 2023-06-06 01:45:59.165403 watchmen_storage_postgresql-16.5.4/src/watchmen_storage_postgresql/table_creator.py
+-rw-r--r--   0        0        0    12688 2023-06-06 01:45:59.165403 watchmen_storage_postgresql-16.5.4/src/watchmen_storage_postgresql/where_build.py
+-rw-r--r--   0        0        0      546 1970-01-01 00:00:00.000000 watchmen_storage_postgresql-16.5.4/PKG-INFO
```

### Comparing `watchmen_storage_postgresql-16.5.3/LICENSE` & `watchmen_storage_postgresql-16.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_storage_postgresql-16.5.3/src/watchmen_storage_postgresql/data_source_postgresql.py` & `watchmen_storage_postgresql-16.5.4/src/watchmen_storage_postgresql/data_source_postgresql.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_postgresql-16.5.3/src/watchmen_storage_postgresql/script_builder_postgresql.py` & `watchmen_storage_postgresql-16.5.4/src/watchmen_storage_postgresql/script_builder_postgresql.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_postgresql-16.5.3/src/watchmen_storage_postgresql/storage_postgresql.py` & `watchmen_storage_postgresql-16.5.4/src/watchmen_storage_postgresql/storage_postgresql.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_postgresql-16.5.3/src/watchmen_storage_postgresql/storage_postgresql_configuration.py` & `watchmen_storage_postgresql-16.5.4/src/watchmen_storage_postgresql/storage_postgresql_configuration.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_postgresql-16.5.3/src/watchmen_storage_postgresql/table_creator.py` & `watchmen_storage_postgresql-16.5.4/src/watchmen_storage_postgresql/table_creator.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_postgresql-16.5.3/src/watchmen_storage_postgresql/where_build.py` & `watchmen_storage_postgresql-16.5.4/src/watchmen_storage_postgresql/where_build.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_postgresql-16.5.3/PKG-INFO` & `watchmen_storage_postgresql-16.5.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: watchmen-storage-postgresql
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
 Requires-Dist: psycopg2-binary (>=2.9.3,<3.0.0)
-Requires-Dist: watchmen-storage-rds (==16.5.3)
+Requires-Dist: watchmen-storage-rds (==16.5.4)
```

