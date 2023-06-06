# Comparing `tmp/watchmen_inquiry_surface-16.5.3.tar.gz` & `tmp/watchmen_inquiry_surface-16.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_inquiry_surface-16.5.3.tar", max compression
+gzip compressed data, was "watchmen_inquiry_surface-16.5.4.tar", max compression
```

## Comparing `watchmen_inquiry_surface-16.5.3.tar` & `watchmen_inquiry_surface-16.5.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1061 2023-06-05 01:29:03.512123 watchmen_inquiry_surface-16.5.3/LICENSE
--rw-r--r--   0        0        0     1304 2023-06-05 01:29:03.512123 watchmen_inquiry_surface-16.5.3/pyproject.toml
--rw-r--r--   0        0        0       46 2023-06-05 01:29:03.512123 watchmen_inquiry_surface-16.5.3/src/watchmen_inquiry_surface/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 01:29:03.512123 watchmen_inquiry_surface-16.5.3/src/watchmen_inquiry_surface/data/__init__.py
--rw-r--r--   0        0        0     9998 2023-06-05 01:29:03.512123 watchmen_inquiry_surface-16.5.3/src/watchmen_inquiry_surface/data/data_router.py
--rw-r--r--   0        0        0      176 2023-06-05 01:29:03.512123 watchmen_inquiry_surface-16.5.3/src/watchmen_inquiry_surface/main.py
--rw-r--r--   0        0        0      476 2023-06-05 01:29:03.512123 watchmen_inquiry_surface-16.5.3/src/watchmen_inquiry_surface/settings.py
--rw-r--r--   0        0        0     1267 1970-01-01 00:00:00.000000 watchmen_inquiry_surface-16.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-06 01:45:59.129402 watchmen_inquiry_surface-16.5.4/LICENSE
+-rw-r--r--   0        0        0     1304 2023-06-06 01:45:59.129402 watchmen_inquiry_surface-16.5.4/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-06-06 01:45:59.129402 watchmen_inquiry_surface-16.5.4/src/watchmen_inquiry_surface/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 01:45:59.129402 watchmen_inquiry_surface-16.5.4/src/watchmen_inquiry_surface/data/__init__.py
+-rw-r--r--   0        0        0    10021 2023-06-06 01:45:59.129402 watchmen_inquiry_surface-16.5.4/src/watchmen_inquiry_surface/data/data_router.py
+-rw-r--r--   0        0        0      176 2023-06-06 01:45:59.129402 watchmen_inquiry_surface-16.5.4/src/watchmen_inquiry_surface/main.py
+-rw-r--r--   0        0        0      476 2023-06-06 01:45:59.129402 watchmen_inquiry_surface-16.5.4/src/watchmen_inquiry_surface/settings.py
+-rw-r--r--   0        0        0     1267 1970-01-01 00:00:00.000000 watchmen_inquiry_surface-16.5.4/PKG-INFO
```

### Comparing `watchmen_inquiry_surface-16.5.3/LICENSE` & `watchmen_inquiry_surface-16.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_surface-16.5.3/pyproject.toml` & `watchmen_inquiry_surface-16.5.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tool.poetry]
 name = "watchmen-inquiry-surface"
-version = "16.5.3"
+version = "16.5.4"
 description = ""
 authors = ["botlikes <75356972+botlikes456@users.noreply.github.com>"]
 license = "MIT"
 packages = [
     { include = "watchmen_inquiry_surface", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-watchmen-inquiry-kernel = "16.5.3"
-watchmen-rest = "16.5.3"
-watchmen-inquiry-trino = { version = "16.5.3", optional = true }
-watchmen-storage-mysql = { version = "16.5.3", optional = true }
-watchmen-storage-oracle = { version = "16.5.3", optional = true }
-watchmen-storage-mongodb = { version = "16.5.3", optional = true }
-watchmen-storage-mssql = { version = "16.5.3", optional = true }
-watchmen-storage-postgresql = { version = "16.5.3", optional = true }
-watchmen-storage-oss = { version = "16.5.3", optional = true }
-watchmen-storage-s3 = { version = "16.5.3", optional = true }
+watchmen-inquiry-kernel = "16.5.4"
+watchmen-rest = "16.5.4"
+watchmen-inquiry-trino = { version = "16.5.4", optional = true }
+watchmen-storage-mysql = { version = "16.5.4", optional = true }
+watchmen-storage-oracle = { version = "16.5.4", optional = true }
+watchmen-storage-mongodb = { version = "16.5.4", optional = true }
+watchmen-storage-mssql = { version = "16.5.4", optional = true }
+watchmen-storage-postgresql = { version = "16.5.4", optional = true }
+watchmen-storage-oss = { version = "16.5.4", optional = true }
+watchmen-storage-s3 = { version = "16.5.4", optional = true }
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.extras]
 trino = ["watchmen-inquiry-trino"]
 mysql = ["watchmen-storage-mysql"]
 oracle = ["watchmen-storage-oracle"]
```

### Comparing `watchmen_inquiry_surface-16.5.3/src/watchmen_inquiry_surface/data/data_router.py` & `watchmen_inquiry_surface-16.5.4/src/watchmen_inquiry_surface/data/data_router.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,21 +116,21 @@
 		subject: Optional[Subject] = get_subject_service(principal_service).find_by_id(subject_id)
 	else:
 		subject: Optional[Subject] = get_subject_service(principal_service).find_by_name(subject_name)
 	if subject is None:
 		raise_400(f'Subject not found by given criteria[id={subject_id}, name={subject_name}].')
 
 	subject_column_map: Dict[str, SubjectDatasetColumn] = ArrayHelper(subject.dataset.columns) \
-		.to_map(lambda x: x.alias, lambda x: x)
+		.to_map(lambda x: x.columnId, lambda x: x)
 
 	def to_report_indicator(indicator: SubjectDatasetCriteriaIndicator) -> ReportIndicator:
-		name = indicator.name
-		dataset_column = subject_column_map.get(name)
+		columnId = indicator.columnId
+		dataset_column = subject_column_map.get(columnId)
 		if dataset_column is None:
-			raise_400(f'Cannot find column[name={name}] from subject.')
+			raise_400(f'Cannot find column[columnId={columnId}] from subject.')
 
 		arithmetic = ReportIndicatorArithmetic.NONE
 		if indicator.arithmetic == SubjectDatasetCriteriaIndicatorArithmetic.COUNT:
 			arithmetic = ReportIndicatorArithmetic.COUNT
 		elif indicator.arithmetic == SubjectDatasetCriteriaIndicatorArithmetic.DISTINCT_COUNT:
 			arithmetic = ReportIndicatorArithmetic.DISTINCT_COUNT
 		elif indicator.arithmetic == SubjectDatasetCriteriaIndicatorArithmetic.SUMMARY:
```

### Comparing `watchmen_inquiry_surface-16.5.3/PKG-INFO` & `watchmen_inquiry_surface-16.5.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchmen-inquiry-surface
-Version: 16.5.3
+Version: 16.5.4
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,17 +15,17 @@
 Provides-Extra: mssql
 Provides-Extra: mysql
 Provides-Extra: oracle
 Provides-Extra: oss
 Provides-Extra: postgresql
 Provides-Extra: s3
 Provides-Extra: trino
-Requires-Dist: watchmen-inquiry-kernel (==16.5.3)
-Requires-Dist: watchmen-inquiry-trino (==16.5.3) ; extra == "trino"
-Requires-Dist: watchmen-rest (==16.5.3)
-Requires-Dist: watchmen-storage-mongodb (==16.5.3) ; extra == "mongodb"
-Requires-Dist: watchmen-storage-mssql (==16.5.3) ; extra == "mssql"
-Requires-Dist: watchmen-storage-mysql (==16.5.3) ; extra == "mysql"
-Requires-Dist: watchmen-storage-oracle (==16.5.3) ; extra == "oracle"
-Requires-Dist: watchmen-storage-oss (==16.5.3) ; extra == "oss"
-Requires-Dist: watchmen-storage-postgresql (==16.5.3) ; extra == "postgresql"
-Requires-Dist: watchmen-storage-s3 (==16.5.3) ; extra == "s3"
+Requires-Dist: watchmen-inquiry-kernel (==16.5.4)
+Requires-Dist: watchmen-inquiry-trino (==16.5.4) ; extra == "trino"
+Requires-Dist: watchmen-rest (==16.5.4)
+Requires-Dist: watchmen-storage-mongodb (==16.5.4) ; extra == "mongodb"
+Requires-Dist: watchmen-storage-mssql (==16.5.4) ; extra == "mssql"
+Requires-Dist: watchmen-storage-mysql (==16.5.4) ; extra == "mysql"
+Requires-Dist: watchmen-storage-oracle (==16.5.4) ; extra == "oracle"
+Requires-Dist: watchmen-storage-oss (==16.5.4) ; extra == "oss"
+Requires-Dist: watchmen-storage-postgresql (==16.5.4) ; extra == "postgresql"
+Requires-Dist: watchmen-storage-s3 (==16.5.4) ; extra == "s3"
```

