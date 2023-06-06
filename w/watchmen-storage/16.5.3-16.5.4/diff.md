# Comparing `tmp/watchmen_storage-16.5.3.tar.gz` & `tmp/watchmen_storage-16.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_storage-16.5.3.tar", max compression
+gzip compressed data, was "watchmen_storage-16.5.4.tar", max compression
```

## Comparing `watchmen_storage-16.5.3.tar` & `watchmen_storage-16.5.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1061 2023-06-05 01:29:03.568124 watchmen_storage-16.5.3/LICENSE
--rw-r--r--   0        0        0      492 2023-06-05 01:29:03.568124 watchmen_storage-16.5.3/pyproject.toml
--rw-r--r--   0        0        0     2217 2023-06-05 01:29:03.568124 watchmen_storage-16.5.3/src/watchmen_storage/__init__.py
--rw-r--r--   0        0        0     4917 2023-06-05 01:29:03.568124 watchmen_storage-16.5.3/src/watchmen_storage/competitive_worker_id_generator.py
--rw-r--r--   0        0        0     5549 2023-06-05 01:29:03.568124 watchmen_storage-16.5.3/src/watchmen_storage/data_source_helper.py
--rw-r--r--   0        0        0     1819 2023-06-05 01:29:03.568124 watchmen_storage-16.5.3/src/watchmen_storage/free_storage_types.py
--rw-r--r--   0        0        0      211 2023-06-05 01:29:03.568124 watchmen_storage-16.5.3/src/watchmen_storage/secrets_manager.py
--rw-r--r--   0        0        0      730 2023-06-05 01:29:03.568124 watchmen_storage-16.5.3/src/watchmen_storage/secrets_manager_aws.py
--rw-r--r--   0        0        0     1096 2023-06-05 01:29:03.568124 watchmen_storage-16.5.3/src/watchmen_storage/settings.py
--rw-r--r--   0        0        0     2750 2023-06-05 01:29:03.568124 watchmen_storage-16.5.3/src/watchmen_storage/snowflake.py
--rw-r--r--   0        0        0      232 2023-06-05 01:29:03.568124 watchmen_storage-16.5.3/src/watchmen_storage/snowflake_worker_id_generator.py
--rw-r--r--   0        0        0        0 2023-06-05 01:29:03.568124 watchmen_storage-16.5.3/src/watchmen_storage/sql_analysis/__init__.py
--rw-r--r--   0        0        0    10150 2023-06-05 01:29:03.568124 watchmen_storage-16.5.3/src/watchmen_storage/sql_analysis/ast_vister.py
--rw-r--r--   0        0        0     2632 2023-06-05 01:29:03.568124 watchmen_storage-16.5.3/src/watchmen_storage/sql_analysis/parse_sql.py
--rw-r--r--   0        0        0      890 2023-06-05 01:29:03.568124 watchmen_storage-16.5.3/src/watchmen_storage/sql_analysis/query_performance_service.py
--rw-r--r--   0        0        0     1441 2023-06-05 01:29:03.568124 watchmen_storage-16.5.3/src/watchmen_storage/sql_analysis/topic_generator.py
--rw-r--r--   0        0        0     7259 2023-06-05 01:29:03.568124 watchmen_storage-16.5.3/src/watchmen_storage/storage_based_worker_id_generator.py
--rw-r--r--   0        0        0      721 2023-06-05 01:29:03.568124 watchmen_storage-16.5.3/src/watchmen_storage/storage_exception.py
--rw-r--r--   0        0        0     5998 2023-06-05 01:29:03.568124 watchmen_storage-16.5.3/src/watchmen_storage/storage_spi.py
--rw-r--r--   0        0        0     4717 2023-06-05 01:29:03.568124 watchmen_storage-16.5.3/src/watchmen_storage/storage_types.py
--rw-r--r--   0        0        0      630 2023-06-05 01:29:03.568124 watchmen_storage-16.5.3/src/watchmen_storage/topic_utils.py
--rw-r--r--   0        0        0      562 1970-01-01 00:00:00.000000 watchmen_storage-16.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-06 01:45:59.165403 watchmen_storage-16.5.4/LICENSE
+-rw-r--r--   0        0        0      492 2023-06-06 01:45:59.165403 watchmen_storage-16.5.4/pyproject.toml
+-rw-r--r--   0        0        0     2217 2023-06-06 01:45:59.165403 watchmen_storage-16.5.4/src/watchmen_storage/__init__.py
+-rw-r--r--   0        0        0     4917 2023-06-06 01:45:59.165403 watchmen_storage-16.5.4/src/watchmen_storage/competitive_worker_id_generator.py
+-rw-r--r--   0        0        0     5549 2023-06-06 01:45:59.165403 watchmen_storage-16.5.4/src/watchmen_storage/data_source_helper.py
+-rw-r--r--   0        0        0     1819 2023-06-06 01:45:59.165403 watchmen_storage-16.5.4/src/watchmen_storage/free_storage_types.py
+-rw-r--r--   0        0        0      211 2023-06-06 01:45:59.165403 watchmen_storage-16.5.4/src/watchmen_storage/secrets_manager.py
+-rw-r--r--   0        0        0      730 2023-06-06 01:45:59.165403 watchmen_storage-16.5.4/src/watchmen_storage/secrets_manager_aws.py
+-rw-r--r--   0        0        0     1096 2023-06-06 01:45:59.165403 watchmen_storage-16.5.4/src/watchmen_storage/settings.py
+-rw-r--r--   0        0        0     2750 2023-06-06 01:45:59.165403 watchmen_storage-16.5.4/src/watchmen_storage/snowflake.py
+-rw-r--r--   0        0        0      232 2023-06-06 01:45:59.165403 watchmen_storage-16.5.4/src/watchmen_storage/snowflake_worker_id_generator.py
+-rw-r--r--   0        0        0        0 2023-06-06 01:45:59.165403 watchmen_storage-16.5.4/src/watchmen_storage/sql_analysis/__init__.py
+-rw-r--r--   0        0        0    10191 2023-06-06 01:45:59.165403 watchmen_storage-16.5.4/src/watchmen_storage/sql_analysis/ast_vister.py
+-rw-r--r--   0        0        0     2632 2023-06-06 01:45:59.165403 watchmen_storage-16.5.4/src/watchmen_storage/sql_analysis/parse_sql.py
+-rw-r--r--   0        0        0      890 2023-06-06 01:45:59.165403 watchmen_storage-16.5.4/src/watchmen_storage/sql_analysis/query_performance_service.py
+-rw-r--r--   0        0        0     1441 2023-06-06 01:45:59.165403 watchmen_storage-16.5.4/src/watchmen_storage/sql_analysis/topic_generator.py
+-rw-r--r--   0        0        0     7259 2023-06-06 01:45:59.165403 watchmen_storage-16.5.4/src/watchmen_storage/storage_based_worker_id_generator.py
+-rw-r--r--   0        0        0      721 2023-06-06 01:45:59.165403 watchmen_storage-16.5.4/src/watchmen_storage/storage_exception.py
+-rw-r--r--   0        0        0     5998 2023-06-06 01:45:59.165403 watchmen_storage-16.5.4/src/watchmen_storage/storage_spi.py
+-rw-r--r--   0        0        0     4717 2023-06-06 01:45:59.165403 watchmen_storage-16.5.4/src/watchmen_storage/storage_types.py
+-rw-r--r--   0        0        0      630 2023-06-06 01:45:59.165403 watchmen_storage-16.5.4/src/watchmen_storage/topic_utils.py
+-rw-r--r--   0        0        0      562 1970-01-01 00:00:00.000000 watchmen_storage-16.5.4/PKG-INFO
```

### Comparing `watchmen_storage-16.5.3/LICENSE` & `watchmen_storage-16.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.3/src/watchmen_storage/__init__.py` & `watchmen_storage-16.5.4/src/watchmen_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.3/src/watchmen_storage/competitive_worker_id_generator.py` & `watchmen_storage-16.5.4/src/watchmen_storage/competitive_worker_id_generator.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.3/src/watchmen_storage/data_source_helper.py` & `watchmen_storage-16.5.4/src/watchmen_storage/data_source_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.3/src/watchmen_storage/free_storage_types.py` & `watchmen_storage-16.5.4/src/watchmen_storage/free_storage_types.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.3/src/watchmen_storage/secrets_manager_aws.py` & `watchmen_storage-16.5.4/src/watchmen_storage/secrets_manager_aws.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.3/src/watchmen_storage/settings.py` & `watchmen_storage-16.5.4/src/watchmen_storage/settings.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.3/src/watchmen_storage/snowflake.py` & `watchmen_storage-16.5.4/src/watchmen_storage/snowflake.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.3/src/watchmen_storage/sql_analysis/ast_vister.py` & `watchmen_storage-16.5.4/src/watchmen_storage/sql_analysis/ast_vister.py`

 * *Files 2% similar despite different names*

```diff
@@ -306,18 +306,20 @@
 	            next_token: Token = None):
 		if context.status == "case" and context.sub_status == "WHEN":
 			left_table, left = token.left.normalized.split(".")
 			add_column_topic(context, left_table)
 			add_column(context, left)
 
 		elif context.status == "where":
-			left_table, left = token.left.normalized.split(".")
-			operator = find_operator(token)
-			value = token.right.value
-			context.where.append(WhereColumn(table=left_table, name=left, operator=operator, value=value))
+			if "." in token.left.normalized:
+				left_table, left = token.left.normalized.split(".")
+				operator = find_operator(token)
+				value = token.right.value
+				context.where.append(WhereColumn(table=left_table, name=left, operator=operator, value=value))
+
 
 		elif token.is_group and token.left and token.right and not context.status == "case":
 			left_table, left = token.left.normalized.split(".")
 			right_table, right = token.right.normalized.split(".")
 			operator = find_operator(token)
 			context.joins.append(
 				JoinColumn(leftTable=left_table, left=left, rightTable=right_table, right=right, operator=operator))
```

### Comparing `watchmen_storage-16.5.3/src/watchmen_storage/sql_analysis/parse_sql.py` & `watchmen_storage-16.5.4/src/watchmen_storage/sql_analysis/parse_sql.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.3/src/watchmen_storage/sql_analysis/query_performance_service.py` & `watchmen_storage-16.5.4/src/watchmen_storage/sql_analysis/query_performance_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.3/src/watchmen_storage/sql_analysis/topic_generator.py` & `watchmen_storage-16.5.4/src/watchmen_storage/sql_analysis/topic_generator.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.3/src/watchmen_storage/storage_based_worker_id_generator.py` & `watchmen_storage-16.5.4/src/watchmen_storage/storage_based_worker_id_generator.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.3/src/watchmen_storage/storage_exception.py` & `watchmen_storage-16.5.4/src/watchmen_storage/storage_exception.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.3/src/watchmen_storage/storage_spi.py` & `watchmen_storage-16.5.4/src/watchmen_storage/storage_spi.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.3/src/watchmen_storage/storage_types.py` & `watchmen_storage-16.5.4/src/watchmen_storage/storage_types.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.3/src/watchmen_storage/topic_utils.py` & `watchmen_storage-16.5.4/src/watchmen_storage/topic_utils.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.3/PKG-INFO` & `watchmen_storage-16.5.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: watchmen-storage
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
 Requires-Dist: boto3 (>=1.24.20,<2.0.0)
 Requires-Dist: sqlparse (>=0.4.4,<0.5.0)
-Requires-Dist: watchmen-model (==16.5.3)
+Requires-Dist: watchmen-model (==16.5.4)
```

