# Comparing `tmp/watchmen_rest_dqc-16.5.4.tar.gz` & `tmp/watchmen_rest_dqc-16.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_rest_dqc-16.5.4.tar", max compression
+gzip compressed data, was "watchmen_rest_dqc-16.5.5.tar", max compression
```

## Comparing `watchmen_rest_dqc-16.5.4.tar` & `watchmen_rest_dqc-16.5.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1061 2023-06-06 01:45:59.145403 watchmen_rest_dqc-16.5.4/LICENSE
--rw-r--r--   0        0        0     1331 2023-06-06 01:45:59.145403 watchmen_rest_dqc-16.5.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-06 01:45:59.149403 watchmen_rest_dqc-16.5.4/src/watchmen_rest_dqc/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 01:45:59.149403 watchmen_rest_dqc-16.5.4/src/watchmen_rest_dqc/admin/__init__.py
--rw-r--r--   0        0        0     5943 2023-06-06 01:45:59.149403 watchmen_rest_dqc-16.5.4/src/watchmen_rest_dqc/admin/catalog_router.py
--rw-r--r--   0        0        0     3051 2023-06-06 01:45:59.149403 watchmen_rest_dqc-16.5.4/src/watchmen_rest_dqc/admin/monitor_rules_router.py
--rw-r--r--   0        0        0      861 2023-06-06 01:45:59.149403 watchmen_rest_dqc-16.5.4/src/watchmen_rest_dqc/dqc.py
--rw-r--r--   0        0        0      544 2023-06-06 01:45:59.149403 watchmen_rest_dqc-16.5.4/src/watchmen_rest_dqc/main.py
--rw-r--r--   0        0        0        0 2023-06-06 01:45:59.149403 watchmen_rest_dqc-16.5.4/src/watchmen_rest_dqc/monitor/__init__.py
--rw-r--r--   0        0        0     5292 2023-06-06 01:45:59.149403 watchmen_rest_dqc-16.5.4/src/watchmen_rest_dqc/monitor/topic_monitor_router.py
--rw-r--r--   0        0        0      106 2023-06-06 01:45:59.149403 watchmen_rest_dqc-16.5.4/src/watchmen_rest_dqc/settings.py
--rw-r--r--   0        0        0        0 2023-06-06 01:45:59.149403 watchmen_rest_dqc-16.5.4/src/watchmen_rest_dqc/topic_profile/__init__.py
--rw-r--r--   0        0        0     1289 2023-06-06 01:45:59.149403 watchmen_rest_dqc-16.5.4/src/watchmen_rest_dqc/topic_profile/topic_profile_router.py
--rw-r--r--   0        0        0       80 2023-06-06 01:45:59.149403 watchmen_rest_dqc-16.5.4/src/watchmen_rest_dqc/util/__init__.py
--rw-r--r--   0        0        0     2068 2023-06-06 01:45:59.149403 watchmen_rest_dqc-16.5.4/src/watchmen_rest_dqc/util/trans.py
--rw-r--r--   0        0        0     1240 1970-01-01 00:00:00.000000 watchmen_rest_dqc-16.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-06 07:52:17.109012 watchmen_rest_dqc-16.5.5/LICENSE
+-rw-r--r--   0        0        0     1331 2023-06-06 07:52:17.109012 watchmen_rest_dqc-16.5.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-06 07:52:17.109012 watchmen_rest_dqc-16.5.5/src/watchmen_rest_dqc/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 07:52:17.109012 watchmen_rest_dqc-16.5.5/src/watchmen_rest_dqc/admin/__init__.py
+-rw-r--r--   0        0        0     5943 2023-06-06 07:52:17.109012 watchmen_rest_dqc-16.5.5/src/watchmen_rest_dqc/admin/catalog_router.py
+-rw-r--r--   0        0        0     3051 2023-06-06 07:52:17.109012 watchmen_rest_dqc-16.5.5/src/watchmen_rest_dqc/admin/monitor_rules_router.py
+-rw-r--r--   0        0        0      861 2023-06-06 07:52:17.109012 watchmen_rest_dqc-16.5.5/src/watchmen_rest_dqc/dqc.py
+-rw-r--r--   0        0        0      544 2023-06-06 07:52:17.109012 watchmen_rest_dqc-16.5.5/src/watchmen_rest_dqc/main.py
+-rw-r--r--   0        0        0        0 2023-06-06 07:52:17.109012 watchmen_rest_dqc-16.5.5/src/watchmen_rest_dqc/monitor/__init__.py
+-rw-r--r--   0        0        0     5292 2023-06-06 07:52:17.109012 watchmen_rest_dqc-16.5.5/src/watchmen_rest_dqc/monitor/topic_monitor_router.py
+-rw-r--r--   0        0        0      106 2023-06-06 07:52:17.109012 watchmen_rest_dqc-16.5.5/src/watchmen_rest_dqc/settings.py
+-rw-r--r--   0        0        0        0 2023-06-06 07:52:17.109012 watchmen_rest_dqc-16.5.5/src/watchmen_rest_dqc/topic_profile/__init__.py
+-rw-r--r--   0        0        0     1289 2023-06-06 07:52:17.109012 watchmen_rest_dqc-16.5.5/src/watchmen_rest_dqc/topic_profile/topic_profile_router.py
+-rw-r--r--   0        0        0       80 2023-06-06 07:52:17.109012 watchmen_rest_dqc-16.5.5/src/watchmen_rest_dqc/util/__init__.py
+-rw-r--r--   0        0        0     2068 2023-06-06 07:52:17.109012 watchmen_rest_dqc-16.5.5/src/watchmen_rest_dqc/util/trans.py
+-rw-r--r--   0        0        0     1240 1970-01-01 00:00:00.000000 watchmen_rest_dqc-16.5.5/PKG-INFO
```

### Comparing `watchmen_rest_dqc-16.5.4/LICENSE` & `watchmen_rest_dqc-16.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_rest_dqc-16.5.4/pyproject.toml` & `watchmen_rest_dqc-16.5.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tool.poetry]
 name = "watchmen-rest-dqc"
-version = "16.5.4"
+version = "16.5.5"
 description = ""
 authors = ["botlikes <75356972+botlikes456@users.noreply.github.com>"]
 license = "MIT"
 packages = [
     { include = "watchmen_rest_dqc", from = "src" }
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.9"
-watchmen-dqc = "16.5.4"
-watchmen-rest = "16.5.4"
-watchmen-storage-mysql = { version = "16.5.4", optional = true }
-watchmen-storage-oracle = { version = "16.5.4", optional = true }
-watchmen-storage-mongodb = { version = "16.5.4", optional = true }
-watchmen-storage-mssql = { version = "16.5.4", optional = true }
-watchmen-storage-postgresql = { version = "16.5.4", optional = true }
-watchmen-storage-oss = { version = "16.5.4", optional = true }
-watchmen-storage-s3 = { version = "16.5.4", optional = true }
+watchmen-dqc = "16.5.5"
+watchmen-rest = "16.5.5"
+watchmen-storage-mysql = { version = "16.5.5", optional = true }
+watchmen-storage-oracle = { version = "16.5.5", optional = true }
+watchmen-storage-mongodb = { version = "16.5.5", optional = true }
+watchmen-storage-mssql = { version = "16.5.5", optional = true }
+watchmen-storage-postgresql = { version = "16.5.5", optional = true }
+watchmen-storage-oss = { version = "16.5.5", optional = true }
+watchmen-storage-s3 = { version = "16.5.5", optional = true }
 boto3 = {version = "^1.24.20", optional = true }
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.extras]
 mysql = ["watchmen-storage-mysql"]
 oracle = ["watchmen-storage-oracle"]
```

### Comparing `watchmen_rest_dqc-16.5.4/src/watchmen_rest_dqc/admin/catalog_router.py` & `watchmen_rest_dqc-16.5.5/src/watchmen_rest_dqc/admin/catalog_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_dqc-16.5.4/src/watchmen_rest_dqc/admin/monitor_rules_router.py` & `watchmen_rest_dqc-16.5.5/src/watchmen_rest_dqc/admin/monitor_rules_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_dqc-16.5.4/src/watchmen_rest_dqc/dqc.py` & `watchmen_rest_dqc-16.5.5/src/watchmen_rest_dqc/dqc.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_dqc-16.5.4/src/watchmen_rest_dqc/main.py` & `watchmen_rest_dqc-16.5.5/src/watchmen_rest_dqc/main.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_dqc-16.5.4/src/watchmen_rest_dqc/monitor/topic_monitor_router.py` & `watchmen_rest_dqc-16.5.5/src/watchmen_rest_dqc/monitor/topic_monitor_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_dqc-16.5.4/src/watchmen_rest_dqc/topic_profile/topic_profile_router.py` & `watchmen_rest_dqc-16.5.5/src/watchmen_rest_dqc/topic_profile/topic_profile_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_dqc-16.5.4/src/watchmen_rest_dqc/util/trans.py` & `watchmen_rest_dqc-16.5.5/src/watchmen_rest_dqc/util/trans.py`

 * *Files identical despite different names*

### Comparing `watchmen_rest_dqc-16.5.4/PKG-INFO` & `watchmen_rest_dqc-16.5.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchmen-rest-dqc
-Version: 16.5.4
+Version: 16.5.5
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,16 +16,16 @@
 Provides-Extra: mssql
 Provides-Extra: mysql
 Provides-Extra: oracle
 Provides-Extra: oss
 Provides-Extra: postgresql
 Provides-Extra: s3
 Requires-Dist: boto3 (>=1.24.20,<2.0.0) ; extra == "boto3"
-Requires-Dist: watchmen-dqc (==16.5.4)
-Requires-Dist: watchmen-rest (==16.5.4)
-Requires-Dist: watchmen-storage-mongodb (==16.5.4) ; extra == "mongodb"
-Requires-Dist: watchmen-storage-mssql (==16.5.4) ; extra == "mssql"
-Requires-Dist: watchmen-storage-mysql (==16.5.4) ; extra == "mysql"
-Requires-Dist: watchmen-storage-oracle (==16.5.4) ; extra == "oracle"
-Requires-Dist: watchmen-storage-oss (==16.5.4) ; extra == "oss"
-Requires-Dist: watchmen-storage-postgresql (==16.5.4) ; extra == "postgresql"
-Requires-Dist: watchmen-storage-s3 (==16.5.4) ; extra == "s3"
+Requires-Dist: watchmen-dqc (==16.5.5)
+Requires-Dist: watchmen-rest (==16.5.5)
+Requires-Dist: watchmen-storage-mongodb (==16.5.5) ; extra == "mongodb"
+Requires-Dist: watchmen-storage-mssql (==16.5.5) ; extra == "mssql"
+Requires-Dist: watchmen-storage-mysql (==16.5.5) ; extra == "mysql"
+Requires-Dist: watchmen-storage-oracle (==16.5.5) ; extra == "oracle"
+Requires-Dist: watchmen-storage-oss (==16.5.5) ; extra == "oss"
+Requires-Dist: watchmen-storage-postgresql (==16.5.5) ; extra == "postgresql"
+Requires-Dist: watchmen-storage-s3 (==16.5.5) ; extra == "s3"
```

