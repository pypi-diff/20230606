# Comparing `tmp/watchmen_storage_rds-16.5.5.tar.gz` & `tmp/watchmen_storage_rds-16.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_storage_rds-16.5.5.tar", max compression
+gzip compressed data, was "watchmen_storage_rds-16.5.6.tar", max compression
```

## Comparing `watchmen_storage_rds-16.5.5.tar` & `watchmen_storage_rds-16.5.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      455 2023-06-06 07:52:17.125012 watchmen_storage_rds-16.5.5/pyproject.toml
--rw-r--r--   0        0        0      643 2023-06-06 07:52:17.125012 watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/__init__.py
--rw-r--r--   0        0        0      652 2023-06-06 07:52:17.125012 watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/dbscript_builder.py
--rw-r--r--   0        0        0      518 2023-06-06 07:52:17.125012 watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/ext_types.py
--rw-r--r--   0        0        0      672 2023-06-06 07:52:17.125012 watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/settings.py
--rw-r--r--   0        0        0      941 2023-06-06 07:52:17.125012 watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/sort_build.py
--rw-r--r--   0        0        0    17832 2023-06-06 07:52:17.125012 watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/storage_rds.py
--rw-r--r--   0        0        0    22728 2023-06-06 07:52:17.125012 watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/table_defs.py
--rw-r--r--   0        0        0     2249 2023-06-06 07:52:17.125012 watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/table_defs_helper.py
--rw-r--r--   0        0        0    23204 2023-06-06 07:52:17.125012 watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/topic_data_storage_rds.py
--rw-r--r--   0        0        0     8191 2023-06-06 07:52:17.125012 watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/topic_table_generate.py
--rw-r--r--   0        0        0      916 2023-06-06 07:52:17.125012 watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/types.py
--rw-r--r--   0        0        0      524 1970-01-01 00:00:00.000000 watchmen_storage_rds-16.5.5/PKG-INFO
+-rw-r--r--   0        0        0      455 2023-06-06 17:50:48.823399 watchmen_storage_rds-16.5.6/pyproject.toml
+-rw-r--r--   0        0        0      643 2023-06-06 17:50:48.823399 watchmen_storage_rds-16.5.6/src/watchmen_storage_rds/__init__.py
+-rw-r--r--   0        0        0      652 2023-06-06 17:50:48.823399 watchmen_storage_rds-16.5.6/src/watchmen_storage_rds/dbscript_builder.py
+-rw-r--r--   0        0        0      518 2023-06-06 17:50:48.823399 watchmen_storage_rds-16.5.6/src/watchmen_storage_rds/ext_types.py
+-rw-r--r--   0        0        0      672 2023-06-06 17:50:48.823399 watchmen_storage_rds-16.5.6/src/watchmen_storage_rds/settings.py
+-rw-r--r--   0        0        0      941 2023-06-06 17:50:48.823399 watchmen_storage_rds-16.5.6/src/watchmen_storage_rds/sort_build.py
+-rw-r--r--   0        0        0    17832 2023-06-06 17:50:48.823399 watchmen_storage_rds-16.5.6/src/watchmen_storage_rds/storage_rds.py
+-rw-r--r--   0        0        0    22728 2023-06-06 17:50:48.823399 watchmen_storage_rds-16.5.6/src/watchmen_storage_rds/table_defs.py
+-rw-r--r--   0        0        0     2249 2023-06-06 17:50:48.823399 watchmen_storage_rds-16.5.6/src/watchmen_storage_rds/table_defs_helper.py
+-rw-r--r--   0        0        0    24063 2023-06-06 17:50:48.823399 watchmen_storage_rds-16.5.6/src/watchmen_storage_rds/topic_data_storage_rds.py
+-rw-r--r--   0        0        0     8191 2023-06-06 17:50:48.823399 watchmen_storage_rds-16.5.6/src/watchmen_storage_rds/topic_table_generate.py
+-rw-r--r--   0        0        0      916 2023-06-06 17:50:48.823399 watchmen_storage_rds-16.5.6/src/watchmen_storage_rds/types.py
+-rw-r--r--   0        0        0      524 1970-01-01 00:00:00.000000 watchmen_storage_rds-16.5.6/PKG-INFO
```

### Comparing `watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/__init__.py` & `watchmen_storage_rds-16.5.6/src/watchmen_storage_rds/__init__.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/dbscript_builder.py` & `watchmen_storage_rds-16.5.6/src/watchmen_storage_rds/dbscript_builder.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/ext_types.py` & `watchmen_storage_rds-16.5.6/src/watchmen_storage_rds/ext_types.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/settings.py` & `watchmen_storage_rds-16.5.6/src/watchmen_storage_rds/settings.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/sort_build.py` & `watchmen_storage_rds-16.5.6/src/watchmen_storage_rds/sort_build.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/storage_rds.py` & `watchmen_storage_rds-16.5.6/src/watchmen_storage_rds/storage_rds.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/table_defs.py` & `watchmen_storage_rds-16.5.6/src/watchmen_storage_rds/table_defs.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/table_defs_helper.py` & `watchmen_storage_rds-16.5.6/src/watchmen_storage_rds/table_defs_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/topic_data_storage_rds.py` & `watchmen_storage_rds-16.5.6/src/watchmen_storage_rds/topic_data_storage_rds.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from watchmen_model.admin import Factor, FactorType, Topic
 from watchmen_model.common import DataPage, TopicId
 from watchmen_storage import as_table_name, EntityHelper, FreeAggregateArithmetic, FreeAggregateColumn, \
 	FreeAggregatePager, FreeAggregator, FreeColumn, FreeFinder, FreeJoin, FreeJoinType, FreePager, Literal, \
 	NoFreeJoinException, TopicDataStorageSPI, UnexpectedStorageException
 from watchmen_storage.settings import ask_sql_analyzer_on
-from watchmen_storage.sql_analysis.ast_vister import QueryPerformance
+from watchmen_storage.sql_analysis.ast_visitor import QueryPerformance
 from watchmen_storage.sql_analysis.parse_sql import SqlParser
 from watchmen_utilities import ArrayHelper, is_not_blank
 from .storage_rds import StorageRDS
 from .table_defs import register_table
 from .types import SQLAlchemyStatement
 
 logger = getLogger(__name__)
@@ -411,18 +411,24 @@
 			sql = str(sql_query)
 			sql_parser = SqlParser()
 			return sql_parser.parse(sql)
 
 	def free_find(self, finder: FreeFinder) -> List[Dict[str, Any]]:
 		data_statement = self.build_free_find_statement(finder)
 		# print("----------")
-		# noinspection DuplicatedCode
 		sql = data_statement.compile(dialect=self.connection.dialect, compile_kwargs={"literal_binds": True})
 		query_performance = self.extract_sql(sql)
+		if finder.commandOnly:
+			query_performance.execution_time = 0
+			query_performance.data_volume = 0
+			if finder.queryPfmMonitor:
+				finder.queryPfmMonitor(query_performance, True)
+			return []
 
+		# noinspection DuplicatedCode
 		start = timer()
 		# noinspection DuplicatedCode
 		results = self.connection.execute(data_statement).mappings().all()
 		end = timer()
 
 		query_performance.execution_time = end - start
 		query_performance.data_volume = len(results)
@@ -462,14 +468,20 @@
 		page_number, max_page_number = self.compute_page(count, page_size, pager.pageable.pageNumber)
 		data_statement = self.build_offset_for_statement(data_statement, page_size, page_number)
 
 		# print("----------")
 		sql = data_statement.compile(dialect=self.connection.dialect, compile_kwargs={"literal_binds": True})
 		query_performance = self.extract_sql(sql)
 		# print("----------")
+		if pager.commandOnly:
+			query_performance.execution_time = 0
+			query_performance.data_volume = 0
+			if pager.queryPfmMonitor:
+				pager.queryPfmMonitor(query_performance, True)
+			return self.create_empty_page(page_size)
 
 		start = timer()
 		results = self.connection.execute(data_statement).mappings().all()
 		end = timer()
 
 		query_performance.execution_time = end - start
 		query_performance.data_volume = len(results)
@@ -494,14 +506,21 @@
 		data_statement = self.build_sort_for_statement(data_statement, aggregator.highOrderSortColumns)
 		if aggregator.highOrderTruncation is not None and aggregator.highOrderTruncation > 0:
 			data_statement = data_statement.limit(aggregator.highOrderTruncation)
 
 		# noinspection DuplicatedCode
 		sql = data_statement.compile(dialect=self.connection.dialect, compile_kwargs={"literal_binds": True})
 		query_performance = self.extract_sql(sql)
+		if aggregator.commandOnly:
+			query_performance.execution_time = 0
+			query_performance.data_volume = 0
+			if aggregator.queryPfmMonitor:
+				aggregator.queryPfmMonitor(query_performance, True)
+			return []
+
 		start = timer()
 		# print("-----adad-----")
 		results = self.connection.execute(data_statement).mappings().all()
 		end = timer()
 		# print("-------asdadd---")
 		query_performance.execution_time = end - start
 		query_performance.data_volume = len(results)
@@ -533,14 +552,21 @@
 
 		data_statement = self.build_sort_for_statement(data_statement, pager.highOrderSortColumns)
 		page_number, max_page_number = self.compute_page(count, page_size, pager.pageable.pageNumber)
 		data_statement = self.build_offset_for_statement(data_statement, page_size, page_number)
 		# print("----------")
 		sql = data_statement.compile(dialect=self.connection.dialect, compile_kwargs={"literal_binds": True})
 		query_performance = self.extract_sql(sql)
+		if pager.commandOnly:
+			query_performance.execution_time = 0
+			query_performance.data_volume = 0
+			if pager.queryPfmMonitor:
+				pager.queryPfmMonitor(query_performance, True)
+			return self.create_empty_page(page_size)
+
 		# print("----------")
 		start = timer()
 		results = self.connection.execute(data_statement).mappings().all()
 		end = timer()
 		query_performance.execution_time = end - start
 		query_performance.data_volume = len(results)
 		# print(query_performance)
```

### Comparing `watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/topic_table_generate.py` & `watchmen_storage_rds-16.5.6/src/watchmen_storage_rds/topic_table_generate.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/types.py` & `watchmen_storage_rds-16.5.6/src/watchmen_storage_rds/types.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.5.5/PKG-INFO` & `watchmen_storage_rds-16.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: watchmen-storage-rds
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
 Requires-Dist: SQLAlchemy (==1.4.35)
-Requires-Dist: watchmen-storage (==16.5.5)
+Requires-Dist: watchmen-storage (==16.5.6)
```

