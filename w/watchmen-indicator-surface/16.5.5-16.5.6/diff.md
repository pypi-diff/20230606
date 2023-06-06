# Comparing `tmp/watchmen_indicator_surface-16.5.5.tar.gz` & `tmp/watchmen_indicator_surface-16.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_indicator_surface-16.5.5.tar", max compression
+gzip compressed data, was "watchmen_indicator_surface-16.5.6.tar", max compression
```

## Comparing `watchmen_indicator_surface-16.5.5.tar` & `watchmen_indicator_surface-16.5.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1025 2023-06-06 07:52:17.089011 watchmen_indicator_surface-16.5.5/pyproject.toml
--rw-r--r--   0        0        0       48 2023-06-06 07:52:17.089011 watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 07:52:17.089011 watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/data/__init__.py
--rw-r--r--   0        0        0     8936 2023-06-06 07:52:17.089011 watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/data/objective_data_router.py
--rw-r--r--   0        0        0      541 2023-06-06 07:52:17.089011 watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/main.py
--rw-r--r--   0        0        0        0 2023-06-06 07:52:17.089011 watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/meta/__init__.py
--rw-r--r--   0        0        0     6015 2023-06-06 07:52:17.089011 watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/meta/achievement_plugin_task_router.py
--rw-r--r--   0        0        0     7181 2023-06-06 07:52:17.089011 watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/meta/bucket_router.py
--rw-r--r--   0        0        0     9156 2023-06-06 07:52:17.089011 watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/meta/derived_objective_router.py
--rw-r--r--   0        0        0     7904 2023-06-06 07:52:17.089011 watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/meta/indicator_router.py
--rw-r--r--   0        0        0    12699 2023-06-06 07:52:17.089011 watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/meta/objective_router.py
--rw-r--r--   0        0        0     5673 2023-06-06 07:52:17.089011 watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/meta/subject_router.py
--rw-r--r--   0        0        0      471 2023-06-06 07:52:17.089011 watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/settings.py
--rw-r--r--   0        0        0       80 2023-06-06 07:52:17.089011 watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/util/__init__.py
--rw-r--r--   0        0        0     2038 2023-06-06 07:52:17.089011 watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/util/trans.py
--rw-r--r--   0        0        0     1016 1970-01-01 00:00:00.000000 watchmen_indicator_surface-16.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1025 2023-06-06 17:50:48.787399 watchmen_indicator_surface-16.5.6/pyproject.toml
+-rw-r--r--   0        0        0       48 2023-06-06 17:50:48.787399 watchmen_indicator_surface-16.5.6/src/watchmen_indicator_surface/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 17:50:48.787399 watchmen_indicator_surface-16.5.6/src/watchmen_indicator_surface/data/__init__.py
+-rw-r--r--   0        0        0     9264 2023-06-06 17:50:48.787399 watchmen_indicator_surface-16.5.6/src/watchmen_indicator_surface/data/objective_data_router.py
+-rw-r--r--   0        0        0      541 2023-06-06 17:50:48.787399 watchmen_indicator_surface-16.5.6/src/watchmen_indicator_surface/main.py
+-rw-r--r--   0        0        0        0 2023-06-06 17:50:48.787399 watchmen_indicator_surface-16.5.6/src/watchmen_indicator_surface/meta/__init__.py
+-rw-r--r--   0        0        0     6015 2023-06-06 17:50:48.787399 watchmen_indicator_surface-16.5.6/src/watchmen_indicator_surface/meta/achievement_plugin_task_router.py
+-rw-r--r--   0        0        0     7181 2023-06-06 17:50:48.787399 watchmen_indicator_surface-16.5.6/src/watchmen_indicator_surface/meta/bucket_router.py
+-rw-r--r--   0        0        0     9156 2023-06-06 17:50:48.787399 watchmen_indicator_surface-16.5.6/src/watchmen_indicator_surface/meta/derived_objective_router.py
+-rw-r--r--   0        0        0     7904 2023-06-06 17:50:48.787399 watchmen_indicator_surface-16.5.6/src/watchmen_indicator_surface/meta/indicator_router.py
+-rw-r--r--   0        0        0    12699 2023-06-06 17:50:48.787399 watchmen_indicator_surface-16.5.6/src/watchmen_indicator_surface/meta/objective_router.py
+-rw-r--r--   0        0        0     5673 2023-06-06 17:50:48.791399 watchmen_indicator_surface-16.5.6/src/watchmen_indicator_surface/meta/subject_router.py
+-rw-r--r--   0        0        0      471 2023-06-06 17:50:48.791399 watchmen_indicator_surface-16.5.6/src/watchmen_indicator_surface/settings.py
+-rw-r--r--   0        0        0       80 2023-06-06 17:50:48.791399 watchmen_indicator_surface-16.5.6/src/watchmen_indicator_surface/util/__init__.py
+-rw-r--r--   0        0        0     2038 2023-06-06 17:50:48.791399 watchmen_indicator_surface-16.5.6/src/watchmen_indicator_surface/util/trans.py
+-rw-r--r--   0        0        0     1016 1970-01-01 00:00:00.000000 watchmen_indicator_surface-16.5.6/PKG-INFO
```

### Comparing `watchmen_indicator_surface-16.5.5/pyproject.toml` & `watchmen_indicator_surface-16.5.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "watchmen-indicator-surface"
-version = "16.5.5"
+version = "16.5.6"
 description = ""
 authors = ["botlikes <75356972+botlikes456@users.noreply.github.com>"]
 license = "MIT"
 packages = [
     { include = "watchmen_indicator_surface", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-watchmen-indicator-kernel = "16.5.5"
-watchmen-rest = "16.5.5"
-watchmen-storage-mysql = { version = "16.5.5", optional = true }
-watchmen-storage-oracle = { version = "16.5.5", optional = true }
-watchmen-storage-mongodb = { version = "16.5.5", optional = true }
-watchmen-storage-mssql = { version = "16.5.5", optional = true }
-watchmen-storage-postgresql = { version = "16.5.5", optional = true }
+watchmen-indicator-kernel = "16.5.6"
+watchmen-rest = "16.5.6"
+watchmen-storage-mysql = { version = "16.5.6", optional = true }
+watchmen-storage-oracle = { version = "16.5.6", optional = true }
+watchmen-storage-mongodb = { version = "16.5.6", optional = true }
+watchmen-storage-mssql = { version = "16.5.6", optional = true }
+watchmen-storage-postgresql = { version = "16.5.6", optional = true }
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.extras]
 mysql = ["watchmen-storage-mysql"]
 oracle = ["watchmen-storage-oracle"]
 mongodb = ["watchmen-storage-mongodb"]
```

### Comparing `watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/data/objective_data_router.py` & `watchmen_indicator_surface-16.5.6/src/watchmen_indicator_surface/data/objective_data_router.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,17 +14,18 @@
 from watchmen_indicator_kernel.meta import IndicatorService
 from watchmen_meta.common import ask_meta_storage, ask_snowflake_generator
 from watchmen_model.admin import UserRole
 from watchmen_model.common import DataResult
 from watchmen_model.indicator import Indicator, Objective, ObjectiveFactorOnIndicator, ObjectiveTimeFrame, \
 	ObjectiveTimeFrameKind, ObjectiveTarget, ComputedObjectiveParameter
 from watchmen_model.indicator.derived_objective import BreakdownTarget
+from watchmen_model.indicator.objective_report import ObjectiveReport, CellTargetValue
 from watchmen_rest import get_admin_principal
 from watchmen_rest.util import raise_400, raise_403
-from watchmen_utilities import is_blank, ArrayHelper
+from watchmen_utilities import is_blank
 
 logger = getLogger(__name__)
 router = APIRouter()
 
 
 class ObjectiveBreakdownRequest(BaseModel):
 	objective: Objective = None
@@ -206,7 +207,21 @@
 			row.currentValue = data[0]
 		elif value_type == BreakdownValueType.PreviousCycle:
 			row.previousValue = data[0]
 		elif value_type == BreakdownValueType.ChainCycle:
 			row.chainValue = data[0]
 		objective_target_breakdown.data.append(row)
 	return objective_target_breakdown
+
+
+
+def build_dataset_with_objectives(objective_report:ObjectiveReport)->DataResult:
+	cell_list: List[CellTargetValue] = objective_report.cells
+
+	## find objective
+
+	## build objective data service
+
+
+	## get target and compute value for each target
+
+	pass
```

### Comparing `watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/main.py` & `watchmen_indicator_surface-16.5.6/src/watchmen_indicator_surface/main.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/meta/achievement_plugin_task_router.py` & `watchmen_indicator_surface-16.5.6/src/watchmen_indicator_surface/meta/achievement_plugin_task_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/meta/bucket_router.py` & `watchmen_indicator_surface-16.5.6/src/watchmen_indicator_surface/meta/bucket_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/meta/derived_objective_router.py` & `watchmen_indicator_surface-16.5.6/src/watchmen_indicator_surface/meta/derived_objective_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/meta/indicator_router.py` & `watchmen_indicator_surface-16.5.6/src/watchmen_indicator_surface/meta/indicator_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/meta/objective_router.py` & `watchmen_indicator_surface-16.5.6/src/watchmen_indicator_surface/meta/objective_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/meta/subject_router.py` & `watchmen_indicator_surface-16.5.6/src/watchmen_indicator_surface/meta/subject_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.5.5/src/watchmen_indicator_surface/util/trans.py` & `watchmen_indicator_surface-16.5.6/src/watchmen_indicator_surface/util/trans.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_surface-16.5.5/PKG-INFO` & `watchmen_indicator_surface-16.5.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchmen-indicator-surface
-Version: 16.5.5
+Version: 16.5.6
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
-Requires-Dist: watchmen-indicator-kernel (==16.5.5)
-Requires-Dist: watchmen-rest (==16.5.5)
-Requires-Dist: watchmen-storage-mongodb (==16.5.5) ; extra == "mongodb"
-Requires-Dist: watchmen-storage-mssql (==16.5.5) ; extra == "mssql"
-Requires-Dist: watchmen-storage-mysql (==16.5.5) ; extra == "mysql"
-Requires-Dist: watchmen-storage-oracle (==16.5.5) ; extra == "oracle"
-Requires-Dist: watchmen-storage-postgresql (==16.5.5) ; extra == "postgresql"
+Requires-Dist: watchmen-indicator-kernel (==16.5.6)
+Requires-Dist: watchmen-rest (==16.5.6)
+Requires-Dist: watchmen-storage-mongodb (==16.5.6) ; extra == "mongodb"
+Requires-Dist: watchmen-storage-mssql (==16.5.6) ; extra == "mssql"
+Requires-Dist: watchmen-storage-mysql (==16.5.6) ; extra == "mysql"
+Requires-Dist: watchmen-storage-oracle (==16.5.6) ; extra == "oracle"
+Requires-Dist: watchmen-storage-postgresql (==16.5.6) ; extra == "postgresql"
```

