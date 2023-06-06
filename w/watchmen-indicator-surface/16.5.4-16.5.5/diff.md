# Comparing `tmp/watchmen_indicator_surface-16.5.4.tar.gz` & `tmp/watchmen_indicator_surface-16.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_indicator_surface-16.5.4.tar", max compression
+gzip compressed data, was "watchmen_indicator_surface-16.5.5.tar", max compression
```

## Comparing `watchmen_indicator_surface-16.5.4.tar` & `watchmen_indicator_surface-16.5.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1025 2023-06-06 01:45:59.125402 watchmen_indicator_surface-16.5.4/pyproject.toml
--rw-r--r--   0        0        0       48 2023-06-06 01:45:59.125402 watchmen_indicator_surface-16.5.4/src/watchmen_indicator_surface/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 01:45:59.129402 watchmen_indicator_surface-16.5.4/src/watchmen_indicator_surface/data/__init__.py
--rw-r--r--   0        0        0     8936 2023-06-06 01:45:59.129402 watchmen_indicator_surface-16.5.4/src/watchmen_indicator_surface/data/objective_data_router.py
--rw-r--r--   0        0        0      541 2023-06-06 01:45:59.129402 watchmen_indicator_surface-16.5.4/src/watchmen_indicator_surface/main.py
--rw-r--r--   0        0        0        0 2023-06-06 01:45:59.129402 watchmen_indicator_surface-16.5.4/src/watchmen_indicator_surface/meta/__init__.py
--rw-r--r--   0        0        0     6015 2023-06-06 01:45:59.129402 watchmen_indicator_surface-16.5.4/src/watchmen_indicator_surface/meta/achievement_plugin_task_router.py
--rw-r--r--   0        0        0     7181 2023-06-06 01:45:59.129402 watchmen_indicator_surface-16.5.4/src/watchmen_indicator_surface/meta/bucket_router.py
--rw-r--r--   0        0        0     9156 2023-06-06 01:45:59.129402 watchmen_indicator_surface-16.5.4/src/watchmen_indicator_surface/meta/derived_objective_router.py
--rw-r--r--   0        0        0     7904 2023-06-06 01:45:59.129402 watchmen_indicator_surface-16.5.4/src/watchmen_indicator_surface/meta/indicator_router.py
--rw-r--r--   0        0        0    12699 2023-06-06 01:45:59.129402 watchmen_indicator_surface-16.5.4/src/watchmen_indicator_surface/meta/objective_router.py
--rw-r--r--   0        0        0     5673 2023-06-06 01:45:59.129402 watchmen_indicator_surface-16.5.4/src/watchmen_indicator_surface/meta/subject_router.py
--rw-r--r--   0        0        0      471 2023-06-06 01:45:59.129402 watchmen_indicator_surface-16.5.4/src/watchmen_indicator_surface/settings.py
--rw-r--r--   0        0        0       80 2023-06-06 01:45:59.129402 watchmen_indicator_surface-16.5.4/src/watchmen_indicator_surface/util/__init__.py
--rw-r--r--   0        0        0     2038 2023-06-06 01:45:59.129402 watchmen_indicator_surface-16.5.4/src/watchmen_indicator_surface/util/trans.py
--rw-r--r--   0        0        0     1016 1970-01-01 00:00:00.000000 watchmen_indicator_surface-16.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1025 2023-06-06 07:52:17.089011 watchmen_indicator_surface-16.5.5/pyproject.toml
+-rw-r--r--   0        0        0       48 2023-06-06 07:52:17.089011 watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 07:52:17.089011 watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/data/__init__.py
+-rw-r--r--   0        0        0     8936 2023-06-06 07:52:17.089011 watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/data/objective_data_router.py
+-rw-r--r--   0        0        0      541 2023-06-06 07:52:17.089011 watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/main.py
+-rw-r--r--   0        0        0        0 2023-06-06 07:52:17.089011 watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/meta/__init__.py
+-rw-r--r--   0        0        0     6015 2023-06-06 07:52:17.089011 watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/meta/achievement_plugin_task_router.py
+-rw-r--r--   0        0        0     7181 2023-06-06 07:52:17.089011 watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/meta/bucket_router.py
+-rw-r--r--   0        0        0     9156 2023-06-06 07:52:17.089011 watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/meta/derived_objective_router.py
+-rw-r--r--   0        0        0     7904 2023-06-06 07:52:17.089011 watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/meta/indicator_router.py
+-rw-r--r--   0        0        0    12699 2023-06-06 07:52:17.089011 watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/meta/objective_router.py
+-rw-r--r--   0        0        0     5673 2023-06-06 07:52:17.089011 watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/meta/subject_router.py
+-rw-r--r--   0        0        0      471 2023-06-06 07:52:17.089011 watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/settings.py
+-rw-r--r--   0        0        0       80 2023-06-06 07:52:17.089011 watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/util/__init__.py
+-rw-r--r--   0        0        0     2038 2023-06-06 07:52:17.089011 watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/util/trans.py
+-rw-r--r--   0        0        0     1016 1970-01-01 00:00:00.000000 watchmen_indicator_surface-16.5.5/PKG-INFO
```

### Comparing `watchmen_indicator_surface-16.5.4/pyproject.toml` & `watchmen_indicator_surface-16.5.5/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "watchmen-indicator-surface"
-version = "16.5.4"
+version = "16.5.5"
 description = ""
 authors = ["botlikes <75356972+botlikes456@users.noreply.github.com>"]
 license = "MIT"
 packages = [
     { include = "watchmen_indicator_surface", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-watchmen-indicator-kernel = "16.5.4"
-watchmen-rest = "16.5.4"
-watchmen-storage-mysql = { version = "16.5.4", optional = true }
-watchmen-storage-oracle = { version = "16.5.4", optional = true }
-watchmen-storage-mongodb = { version = "16.5.4", optional = true }
-watchmen-storage-mssql = { version = "16.5.4", optional = true }
-watchmen-storage-postgresql = { version = "16.5.4", optional = true }
+watchmen-indicator-kernel = "16.5.5"
+watchmen-rest = "16.5.5"
+watchmen-storage-mysql = { version = "16.5.5", optional = true }
+watchmen-storage-oracle = { version = "16.5.5", optional = true }
+watchmen-storage-mongodb = { version = "16.5.5", optional = true }
+watchmen-storage-mssql = { version = "16.5.5", optional = true }
+watchmen-storage-postgresql = { version = "16.5.5", optional = true }
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.extras]
 mysql = ["watchmen-storage-mysql"]
 oracle = ["watchmen-storage-oracle"]
 mongodb = ["watchmen-storage-mongodb"]
```

### Comparing `watchmen_indicator_surface-16.5.4/src/watchmen_indicator_surface/data/objective_data_router.py` & `watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/data/objective_data_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.5.4/src/watchmen_indicator_surface/main.py` & `watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/main.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.5.4/src/watchmen_indicator_surface/meta/achievement_plugin_task_router.py` & `watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/meta/achievement_plugin_task_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.5.4/src/watchmen_indicator_surface/meta/bucket_router.py` & `watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/meta/bucket_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.5.4/src/watchmen_indicator_surface/meta/derived_objective_router.py` & `watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/meta/derived_objective_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.5.4/src/watchmen_indicator_surface/meta/indicator_router.py` & `watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/meta/indicator_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.5.4/src/watchmen_indicator_surface/meta/objective_router.py` & `watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/meta/objective_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.5.4/src/watchmen_indicator_surface/meta/subject_router.py` & `watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/meta/subject_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.5.4/src/watchmen_indicator_surface/util/trans.py` & `watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/util/trans.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.5.4/PKG-INFO` & `watchmen_indicator_surface-16.5.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchmen-indicator-surface
-Version: 16.5.4
+Version: 16.5.5
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: mongodb
 Provides-Extra: mssql
 Provides-Extra: mysql
 Provides-Extra: oracle
 Provides-Extra: postgresql
-Requires-Dist: watchmen-indicator-kernel (==16.5.4)
-Requires-Dist: watchmen-rest (==16.5.4)
-Requires-Dist: watchmen-storage-mongodb (==16.5.4) ; extra == "mongodb"
-Requires-Dist: watchmen-storage-mssql (==16.5.4) ; extra == "mssql"
-Requires-Dist: watchmen-storage-mysql (==16.5.4) ; extra == "mysql"
-Requires-Dist: watchmen-storage-oracle (==16.5.4) ; extra == "oracle"
-Requires-Dist: watchmen-storage-postgresql (==16.5.4) ; extra == "postgresql"
+Requires-Dist: watchmen-indicator-kernel (==16.5.5)
+Requires-Dist: watchmen-rest (==16.5.5)
+Requires-Dist: watchmen-storage-mongodb (==16.5.5) ; extra == "mongodb"
+Requires-Dist: watchmen-storage-mssql (==16.5.5) ; extra == "mssql"
+Requires-Dist: watchmen-storage-mysql (==16.5.5) ; extra == "mysql"
+Requires-Dist: watchmen-storage-oracle (==16.5.5) ; extra == "oracle"
+Requires-Dist: watchmen-storage-postgresql (==16.5.5) ; extra == "postgresql"
```

