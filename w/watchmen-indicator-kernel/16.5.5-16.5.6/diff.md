# Comparing `tmp/watchmen_indicator_kernel-16.5.5.tar.gz` & `tmp/watchmen_indicator_kernel-16.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_indicator_kernel-16.5.5.tar", max compression
+gzip compressed data, was "watchmen_indicator_kernel-16.5.6.tar", max compression
```

## Comparing `watchmen_indicator_kernel-16.5.5.tar` & `watchmen_indicator_kernel-16.5.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1281 2023-06-06 07:52:17.085011 watchmen_indicator_kernel-16.5.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-06 07:52:17.085011 watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/__init__.py
--rw-r--r--   0        0        0       86 2023-06-06 07:52:17.085011 watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/common/__init__.py
--rw-r--r--   0        0        0       49 2023-06-06 07:52:17.085011 watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/common/exception.py
--rw-r--r--   0        0        0      329 2023-06-06 07:52:17.085011 watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/common/settings.py
--rw-r--r--   0        0        0      286 2023-06-06 07:52:17.085011 watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/data/__init__.py
--rw-r--r--   0        0        0      140 2023-06-06 07:52:17.085011 watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/data/objective/__init__.py
--rw-r--r--   0        0        0      313 2023-06-06 07:52:17.085011 watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/data/objective/data_helper.py
--rw-r--r--   0        0        0    27145 2023-06-06 07:52:17.085011 watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/data/objective/data_service.py
--rw-r--r--   0        0        0       59 2023-06-06 07:52:17.085011 watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/data/objective_factor/__init__.py
--rw-r--r--   0        0        0     2678 2023-06-06 07:52:17.085011 watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/data/objective_factor/data_helper.py
--rw-r--r--   0        0        0    11941 2023-06-06 07:52:17.085011 watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/data/objective_factor/data_service.py
--rw-r--r--   0        0        0    21400 2023-06-06 07:52:17.085011 watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/data/objective_factor/objective_criteria_service.py
--rw-r--r--   0        0        0    10799 2023-06-06 07:52:17.085011 watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/data/objective_factor/subject_base_service.py
--rw-r--r--   0        0        0     8341 2023-06-06 07:52:17.085011 watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/data/objective_factor/topic_base_service.py
--rw-r--r--   0        0        0      397 2023-06-06 07:52:17.085011 watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/data/utils/__init__.py
--rw-r--r--   0        0        0     1088 2023-06-06 07:52:17.089011 watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/data/utils/bucket.py
--rw-r--r--   0        0        0      979 2023-06-06 07:52:17.089011 watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/data/utils/derived_objective.py
--rw-r--r--   0        0        0     1051 2023-06-06 07:52:17.089011 watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/data/utils/enum.py
--rw-r--r--   0        0        0      284 2023-06-06 07:52:17.089011 watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/data/utils/factor.py
--rw-r--r--   0        0        0     1330 2023-06-06 07:52:17.089011 watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/data/utils/indicator.py
--rw-r--r--   0        0        0     3110 2023-06-06 07:52:17.089011 watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/data/utils/parameter.py
--rw-r--r--   0        0        0      786 2023-06-06 07:52:17.089011 watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/data/utils/subject.py
--rw-r--r--   0        0        0    12305 2023-06-06 07:52:17.089011 watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/data/utils/time_frame.py
--rw-r--r--   0        0        0     1074 2023-06-06 07:52:17.089011 watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/data/utils/topic.py
--rw-r--r--   0        0        0      268 2023-06-06 07:52:17.089011 watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/meta/__init__.py
--rw-r--r--   0        0        0     1762 2023-06-06 07:52:17.089011 watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/meta/achievement_task_service.py
--rw-r--r--   0        0        0     8647 2023-06-06 07:52:17.089011 watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/meta/bucket_service.py
--rw-r--r--   0        0        0     4960 2023-06-06 07:52:17.089011 watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/meta/derived_objective_service.py
--rw-r--r--   0        0        0     6695 2023-06-06 07:52:17.089011 watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/meta/indicator_service.py
--rw-r--r--   0        0        0     5783 2023-06-06 07:52:17.089011 watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/meta/objective_service.py
--rw-r--r--   0        0        0       46 2023-06-06 07:52:17.089011 watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/plugin/__init__.py
--rw-r--r--   0        0        0      678 2023-06-06 07:52:17.089011 watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/plugin/connector.py
--rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 watchmen_indicator_kernel-16.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1281 2023-06-06 17:50:48.787399 watchmen_indicator_kernel-16.5.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-06 17:50:48.787399 watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/__init__.py
+-rw-r--r--   0        0        0       86 2023-06-06 17:50:48.787399 watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/common/__init__.py
+-rw-r--r--   0        0        0       49 2023-06-06 17:50:48.787399 watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/common/exception.py
+-rw-r--r--   0        0        0      329 2023-06-06 17:50:48.787399 watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/common/settings.py
+-rw-r--r--   0        0        0      286 2023-06-06 17:50:48.787399 watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/data/__init__.py
+-rw-r--r--   0        0        0      140 2023-06-06 17:50:48.787399 watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/data/objective/__init__.py
+-rw-r--r--   0        0        0      313 2023-06-06 17:50:48.787399 watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/data/objective/data_helper.py
+-rw-r--r--   0        0        0    27145 2023-06-06 17:50:48.787399 watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/data/objective/data_service.py
+-rw-r--r--   0        0        0       59 2023-06-06 17:50:48.787399 watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/data/objective_factor/__init__.py
+-rw-r--r--   0        0        0     2678 2023-06-06 17:50:48.787399 watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/data/objective_factor/data_helper.py
+-rw-r--r--   0        0        0    11941 2023-06-06 17:50:48.787399 watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/data/objective_factor/data_service.py
+-rw-r--r--   0        0        0    21400 2023-06-06 17:50:48.787399 watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/data/objective_factor/objective_criteria_service.py
+-rw-r--r--   0        0        0    10799 2023-06-06 17:50:48.787399 watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/data/objective_factor/subject_base_service.py
+-rw-r--r--   0        0        0     8341 2023-06-06 17:50:48.787399 watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/data/objective_factor/topic_base_service.py
+-rw-r--r--   0        0        0      397 2023-06-06 17:50:48.787399 watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/data/utils/__init__.py
+-rw-r--r--   0        0        0     1088 2023-06-06 17:50:48.787399 watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/data/utils/bucket.py
+-rw-r--r--   0        0        0      979 2023-06-06 17:50:48.787399 watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/data/utils/derived_objective.py
+-rw-r--r--   0        0        0     1051 2023-06-06 17:50:48.787399 watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/data/utils/enum.py
+-rw-r--r--   0        0        0      284 2023-06-06 17:50:48.787399 watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/data/utils/factor.py
+-rw-r--r--   0        0        0     1330 2023-06-06 17:50:48.787399 watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/data/utils/indicator.py
+-rw-r--r--   0        0        0     3110 2023-06-06 17:50:48.787399 watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/data/utils/parameter.py
+-rw-r--r--   0        0        0      786 2023-06-06 17:50:48.787399 watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/data/utils/subject.py
+-rw-r--r--   0        0        0    12305 2023-06-06 17:50:48.787399 watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/data/utils/time_frame.py
+-rw-r--r--   0        0        0     1074 2023-06-06 17:50:48.787399 watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/data/utils/topic.py
+-rw-r--r--   0        0        0      268 2023-06-06 17:50:48.787399 watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/meta/__init__.py
+-rw-r--r--   0        0        0     1762 2023-06-06 17:50:48.787399 watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/meta/achievement_task_service.py
+-rw-r--r--   0        0        0     8647 2023-06-06 17:50:48.787399 watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/meta/bucket_service.py
+-rw-r--r--   0        0        0     4960 2023-06-06 17:50:48.787399 watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/meta/derived_objective_service.py
+-rw-r--r--   0        0        0     6695 2023-06-06 17:50:48.787399 watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/meta/indicator_service.py
+-rw-r--r--   0        0        0     5783 2023-06-06 17:50:48.787399 watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/meta/objective_service.py
+-rw-r--r--   0        0        0       46 2023-06-06 17:50:48.787399 watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/plugin/__init__.py
+-rw-r--r--   0        0        0      678 2023-06-06 17:50:48.787399 watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/plugin/connector.py
+-rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 watchmen_indicator_kernel-16.5.6/PKG-INFO
```

### Comparing `watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/data/objective/data_service.py` & `watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/data/objective/data_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/data/objective_factor/data_helper.py` & `watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/data/objective_factor/data_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/data/objective_factor/data_service.py` & `watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/data/objective_factor/data_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/data/objective_factor/objective_criteria_service.py` & `watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/data/objective_factor/objective_criteria_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/data/objective_factor/subject_base_service.py` & `watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/data/objective_factor/subject_base_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/data/objective_factor/topic_base_service.py` & `watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/data/objective_factor/topic_base_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/data/utils/bucket.py` & `watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/data/utils/bucket.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/data/utils/derived_objective.py` & `watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/data/utils/derived_objective.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/data/utils/enum.py` & `watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/data/utils/enum.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/data/utils/indicator.py` & `watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/data/utils/indicator.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/data/utils/parameter.py` & `watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/data/utils/parameter.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/data/utils/subject.py` & `watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/data/utils/subject.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/data/utils/time_frame.py` & `watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/data/utils/time_frame.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/data/utils/topic.py` & `watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/data/utils/topic.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/meta/achievement_task_service.py` & `watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/meta/achievement_task_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/meta/bucket_service.py` & `watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/meta/bucket_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/meta/derived_objective_service.py` & `watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/meta/derived_objective_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/meta/indicator_service.py` & `watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/meta/indicator_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/meta/objective_service.py` & `watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/meta/objective_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.5/src/watchmen_indicator_kernel/plugin/connector.py` & `watchmen_indicator_kernel-16.5.6/src/watchmen_indicator_kernel/plugin/connector.py`

 * *Files identical despite different names*

### Comparing `watchmen_indicator_kernel-16.5.5/PKG-INFO` & `watchmen_indicator_kernel-16.5.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchmen-indicator-kernel
-Version: 16.5.5
+Version: 16.5.6
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,16 +15,16 @@
 Provides-Extra: mssql
 Provides-Extra: mysql
 Provides-Extra: oracle
 Provides-Extra: oss
 Provides-Extra: postgresql
 Provides-Extra: s3
 Provides-Extra: trino
-Requires-Dist: watchmen-inquiry-kernel (==16.5.5)
-Requires-Dist: watchmen-inquiry-trino (==16.5.5) ; extra == "trino"
-Requires-Dist: watchmen-storage-mongodb (==16.5.5) ; extra == "mongodb"
-Requires-Dist: watchmen-storage-mssql (==16.5.5) ; extra == "mssql"
-Requires-Dist: watchmen-storage-mysql (==16.5.5) ; extra == "mysql"
-Requires-Dist: watchmen-storage-oracle (==16.5.5) ; extra == "oracle"
-Requires-Dist: watchmen-storage-oss (==16.5.5) ; extra == "oss"
-Requires-Dist: watchmen-storage-postgresql (==16.5.5) ; extra == "postgresql"
-Requires-Dist: watchmen-storage-s3 (==16.5.5) ; extra == "s3"
+Requires-Dist: watchmen-inquiry-kernel (==16.5.6)
+Requires-Dist: watchmen-inquiry-trino (==16.5.6) ; extra == "trino"
+Requires-Dist: watchmen-storage-mongodb (==16.5.6) ; extra == "mongodb"
+Requires-Dist: watchmen-storage-mssql (==16.5.6) ; extra == "mssql"
+Requires-Dist: watchmen-storage-mysql (==16.5.6) ; extra == "mysql"
+Requires-Dist: watchmen-storage-oracle (==16.5.6) ; extra == "oracle"
+Requires-Dist: watchmen-storage-oss (==16.5.6) ; extra == "oss"
+Requires-Dist: watchmen-storage-postgresql (==16.5.6) ; extra == "postgresql"
+Requires-Dist: watchmen-storage-s3 (==16.5.6) ; extra == "s3"
```

