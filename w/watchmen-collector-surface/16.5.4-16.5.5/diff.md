# Comparing `tmp/watchmen_collector_surface-16.5.4.tar.gz` & `tmp/watchmen_collector_surface-16.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_collector_surface-16.5.4.tar", max compression
+gzip compressed data, was "watchmen_collector_surface-16.5.5.tar", max compression
```

## Comparing `watchmen_collector_surface-16.5.4.tar` & `watchmen_collector_surface-16.5.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1061 2023-06-06 01:45:59.117402 watchmen_collector_surface-16.5.4/LICENSE
--rw-r--r--   0        0        0     1247 2023-06-06 01:45:59.117402 watchmen_collector_surface-16.5.4/pyproject.toml
--rw-r--r--   0        0        0      106 2023-06-06 01:45:59.117402 watchmen_collector_surface-16.5.4/src/watchmen_collector_surface/__init__.py
--rw-r--r--   0        0        0      188 2023-06-06 01:45:59.117402 watchmen_collector_surface-16.5.4/src/watchmen_collector_surface/cdc/__init__.py
--rw-r--r--   0        0        0     5306 2023-06-06 01:45:59.117402 watchmen_collector_surface-16.5.4/src/watchmen_collector_surface/cdc/monitor_event.py
--rw-r--r--   0        0        0    11506 2023-06-06 01:45:59.117402 watchmen_collector_surface-16.5.4/src/watchmen_collector_surface/cdc/post_json.py
--rw-r--r--   0        0        0    10062 2023-06-06 01:45:59.117402 watchmen_collector_surface-16.5.4/src/watchmen_collector_surface/cdc/record_to_json.py
--rw-r--r--   0        0        0     7551 2023-06-06 01:45:59.117402 watchmen_collector_surface-16.5.4/src/watchmen_collector_surface/cdc/table_extractor.py
--rw-r--r--   0        0        0       65 2023-06-06 01:45:59.117402 watchmen_collector_surface-16.5.4/src/watchmen_collector_surface/connects/__init__.py
--rw-r--r--   0        0        0     4829 2023-06-06 01:45:59.117402 watchmen_collector_surface-16.5.4/src/watchmen_collector_surface/connects/s3_connector.py
--rw-r--r--   0        0        0        0 2023-06-06 01:45:59.117402 watchmen_collector_surface-16.5.4/src/watchmen_collector_surface/data/__init__.py
--rw-r--r--   0        0        0     3988 2023-06-06 01:45:59.117402 watchmen_collector_surface-16.5.4/src/watchmen_collector_surface/data/config_router.py
--rw-r--r--   0        0        0     2034 2023-06-06 01:45:59.117402 watchmen_collector_surface-16.5.4/src/watchmen_collector_surface/data/task_router.py
--rw-r--r--   0        0        0     1450 2023-06-06 01:45:59.117402 watchmen_collector_surface-16.5.4/src/watchmen_collector_surface/data/trigger_router.py
--rw-r--r--   0        0        0      258 2023-06-06 01:45:59.117402 watchmen_collector_surface-16.5.4/src/watchmen_collector_surface/main.py
--rw-r--r--   0        0        0     1716 2023-06-06 01:45:59.117402 watchmen_collector_surface-16.5.4/src/watchmen_collector_surface/settings.py
--rw-r--r--   0        0        0     1230 2023-06-06 01:45:59.117402 watchmen_collector_surface-16.5.4/src/watchmen_collector_surface/surface.py
--rw-r--r--   0        0        0       46 2023-06-06 01:45:59.117402 watchmen_collector_surface-16.5.4/src/watchmen_collector_surface/task/__init__.py
--rw-r--r--   0        0        0     2329 2023-06-06 01:45:59.117402 watchmen_collector_surface-16.5.4/src/watchmen_collector_surface/task/handler.py
--rw-r--r--   0        0        0     2737 2023-06-06 01:45:59.117402 watchmen_collector_surface-16.5.4/src/watchmen_collector_surface/task/task_listener.py
--rw-r--r--   0        0        0     1232 1970-01-01 00:00:00.000000 watchmen_collector_surface-16.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-06 07:52:17.077011 watchmen_collector_surface-16.5.5/LICENSE
+-rw-r--r--   0        0        0     1247 2023-06-06 07:52:17.081011 watchmen_collector_surface-16.5.5/pyproject.toml
+-rw-r--r--   0        0        0      106 2023-06-06 07:52:17.081011 watchmen_collector_surface-16.5.5/src/watchmen_collector_surface/__init__.py
+-rw-r--r--   0        0        0      188 2023-06-06 07:52:17.081011 watchmen_collector_surface-16.5.5/src/watchmen_collector_surface/cdc/__init__.py
+-rw-r--r--   0        0        0     5306 2023-06-06 07:52:17.081011 watchmen_collector_surface-16.5.5/src/watchmen_collector_surface/cdc/monitor_event.py
+-rw-r--r--   0        0        0    11506 2023-06-06 07:52:17.081011 watchmen_collector_surface-16.5.5/src/watchmen_collector_surface/cdc/post_json.py
+-rw-r--r--   0        0        0    10062 2023-06-06 07:52:17.081011 watchmen_collector_surface-16.5.5/src/watchmen_collector_surface/cdc/record_to_json.py
+-rw-r--r--   0        0        0     7551 2023-06-06 07:52:17.081011 watchmen_collector_surface-16.5.5/src/watchmen_collector_surface/cdc/table_extractor.py
+-rw-r--r--   0        0        0       65 2023-06-06 07:52:17.081011 watchmen_collector_surface-16.5.5/src/watchmen_collector_surface/connects/__init__.py
+-rw-r--r--   0        0        0     4829 2023-06-06 07:52:17.081011 watchmen_collector_surface-16.5.5/src/watchmen_collector_surface/connects/s3_connector.py
+-rw-r--r--   0        0        0        0 2023-06-06 07:52:17.081011 watchmen_collector_surface-16.5.5/src/watchmen_collector_surface/data/__init__.py
+-rw-r--r--   0        0        0     3988 2023-06-06 07:52:17.081011 watchmen_collector_surface-16.5.5/src/watchmen_collector_surface/data/config_router.py
+-rw-r--r--   0        0        0     2034 2023-06-06 07:52:17.081011 watchmen_collector_surface-16.5.5/src/watchmen_collector_surface/data/task_router.py
+-rw-r--r--   0        0        0     1450 2023-06-06 07:52:17.081011 watchmen_collector_surface-16.5.5/src/watchmen_collector_surface/data/trigger_router.py
+-rw-r--r--   0        0        0      258 2023-06-06 07:52:17.081011 watchmen_collector_surface-16.5.5/src/watchmen_collector_surface/main.py
+-rw-r--r--   0        0        0     1716 2023-06-06 07:52:17.081011 watchmen_collector_surface-16.5.5/src/watchmen_collector_surface/settings.py
+-rw-r--r--   0        0        0     1230 2023-06-06 07:52:17.081011 watchmen_collector_surface-16.5.5/src/watchmen_collector_surface/surface.py
+-rw-r--r--   0        0        0       46 2023-06-06 07:52:17.081011 watchmen_collector_surface-16.5.5/src/watchmen_collector_surface/task/__init__.py
+-rw-r--r--   0        0        0     2329 2023-06-06 07:52:17.081011 watchmen_collector_surface-16.5.5/src/watchmen_collector_surface/task/handler.py
+-rw-r--r--   0        0        0     2737 2023-06-06 07:52:17.081011 watchmen_collector_surface-16.5.5/src/watchmen_collector_surface/task/task_listener.py
+-rw-r--r--   0        0        0     1232 1970-01-01 00:00:00.000000 watchmen_collector_surface-16.5.5/PKG-INFO
```

### Comparing `watchmen_collector_surface-16.5.4/LICENSE` & `watchmen_collector_surface-16.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_collector_surface-16.5.4/pyproject.toml` & `watchmen_collector_surface-16.5.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tool.poetry]
 name = "watchmen-collector-surface"
-version = "16.5.4"
+version = "16.5.5"
 description = ""
 authors = ["botlikes <75356972+botlikes456@users.noreply.github.com>"]
 license = "MIT"
 packages = [
     { include = "watchmen_collector_surface", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-watchmen-collector-kernel = "16.5.4"
-watchmen-pipeline-kernel = "16.5.4"
-watchmen-rest = "16.5.4"
-watchmen-storage-mysql = { version = "16.5.4", optional = true }
-watchmen-storage-oracle = { version = "16.5.4", optional = true }
-watchmen-storage-mongodb = { version = "16.5.4", optional = true }
-watchmen-storage-mssql = { version = "16.5.4", optional = true }
-watchmen-storage-postgresql = { version = "16.5.4", optional = true }
-watchmen-storage-oss = { version = "16.5.4", optional = true }
-watchmen-storage-s3 = { version = "16.5.4", optional = true }
+watchmen-collector-kernel = "16.5.5"
+watchmen-pipeline-kernel = "16.5.5"
+watchmen-rest = "16.5.5"
+watchmen-storage-mysql = { version = "16.5.5", optional = true }
+watchmen-storage-oracle = { version = "16.5.5", optional = true }
+watchmen-storage-mongodb = { version = "16.5.5", optional = true }
+watchmen-storage-mssql = { version = "16.5.5", optional = true }
+watchmen-storage-postgresql = { version = "16.5.5", optional = true }
+watchmen-storage-oss = { version = "16.5.5", optional = true }
+watchmen-storage-s3 = { version = "16.5.5", optional = true }
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.extras]
 mysql = ["watchmen-storage-mysql"]
 oracle = ["watchmen-storage-oracle"]
 mongodb = ["watchmen-storage-mongodb"]
```

### Comparing `watchmen_collector_surface-16.5.4/src/watchmen_collector_surface/cdc/monitor_event.py` & `watchmen_collector_surface-16.5.5/src/watchmen_collector_surface/cdc/monitor_event.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_surface-16.5.4/src/watchmen_collector_surface/cdc/post_json.py` & `watchmen_collector_surface-16.5.5/src/watchmen_collector_surface/cdc/post_json.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_surface-16.5.4/src/watchmen_collector_surface/cdc/record_to_json.py` & `watchmen_collector_surface-16.5.5/src/watchmen_collector_surface/cdc/record_to_json.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_surface-16.5.4/src/watchmen_collector_surface/cdc/table_extractor.py` & `watchmen_collector_surface-16.5.5/src/watchmen_collector_surface/cdc/table_extractor.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_surface-16.5.4/src/watchmen_collector_surface/connects/s3_connector.py` & `watchmen_collector_surface-16.5.5/src/watchmen_collector_surface/connects/s3_connector.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_surface-16.5.4/src/watchmen_collector_surface/data/config_router.py` & `watchmen_collector_surface-16.5.5/src/watchmen_collector_surface/data/config_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_surface-16.5.4/src/watchmen_collector_surface/data/task_router.py` & `watchmen_collector_surface-16.5.5/src/watchmen_collector_surface/data/task_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_surface-16.5.4/src/watchmen_collector_surface/data/trigger_router.py` & `watchmen_collector_surface-16.5.5/src/watchmen_collector_surface/data/trigger_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_surface-16.5.4/src/watchmen_collector_surface/settings.py` & `watchmen_collector_surface-16.5.5/src/watchmen_collector_surface/settings.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_surface-16.5.4/src/watchmen_collector_surface/surface.py` & `watchmen_collector_surface-16.5.5/src/watchmen_collector_surface/surface.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_surface-16.5.4/src/watchmen_collector_surface/task/handler.py` & `watchmen_collector_surface-16.5.5/src/watchmen_collector_surface/task/handler.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_surface-16.5.4/src/watchmen_collector_surface/task/task_listener.py` & `watchmen_collector_surface-16.5.5/src/watchmen_collector_surface/task/task_listener.py`

 * *Files identical despite different names*

### Comparing `watchmen_collector_surface-16.5.4/PKG-INFO` & `watchmen_collector_surface-16.5.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchmen-collector-surface
-Version: 16.5.4
+Version: 16.5.5
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -14,17 +14,17 @@
 Provides-Extra: mongodb
 Provides-Extra: mssql
 Provides-Extra: mysql
 Provides-Extra: oracle
 Provides-Extra: oss
 Provides-Extra: postgresql
 Provides-Extra: s3
-Requires-Dist: watchmen-collector-kernel (==16.5.4)
-Requires-Dist: watchmen-pipeline-kernel (==16.5.4)
-Requires-Dist: watchmen-rest (==16.5.4)
-Requires-Dist: watchmen-storage-mongodb (==16.5.4) ; extra == "mongodb"
-Requires-Dist: watchmen-storage-mssql (==16.5.4) ; extra == "mssql"
-Requires-Dist: watchmen-storage-mysql (==16.5.4) ; extra == "mysql"
-Requires-Dist: watchmen-storage-oracle (==16.5.4) ; extra == "oracle"
-Requires-Dist: watchmen-storage-oss (==16.5.4) ; extra == "oss"
-Requires-Dist: watchmen-storage-postgresql (==16.5.4) ; extra == "postgresql"
-Requires-Dist: watchmen-storage-s3 (==16.5.4) ; extra == "s3"
+Requires-Dist: watchmen-collector-kernel (==16.5.5)
+Requires-Dist: watchmen-pipeline-kernel (==16.5.5)
+Requires-Dist: watchmen-rest (==16.5.5)
+Requires-Dist: watchmen-storage-mongodb (==16.5.5) ; extra == "mongodb"
+Requires-Dist: watchmen-storage-mssql (==16.5.5) ; extra == "mssql"
+Requires-Dist: watchmen-storage-mysql (==16.5.5) ; extra == "mysql"
+Requires-Dist: watchmen-storage-oracle (==16.5.5) ; extra == "oracle"
+Requires-Dist: watchmen-storage-oss (==16.5.5) ; extra == "oss"
+Requires-Dist: watchmen-storage-postgresql (==16.5.5) ; extra == "postgresql"
+Requires-Dist: watchmen-storage-s3 (==16.5.5) ; extra == "s3"
```

