# Comparing `tmp/watchmen_storage_rds-16.5.4.tar.gz` & `tmp/watchmen_storage_rds-16.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_storage_rds-16.5.4.tar", max compression
+gzip compressed data, was "watchmen_storage_rds-16.5.5.tar", max compression
```

## Comparing `watchmen_storage_rds-16.5.4.tar` & `watchmen_storage_rds-16.5.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      455 2023-06-06 01:45:59.165403 watchmen_storage_rds-16.5.4/pyproject.toml
--rw-r--r--   0        0        0      643 2023-06-06 01:45:59.165403 watchmen_storage_rds-16.5.4/src/watchmen_storage_rds/__init__.py
--rw-r--r--   0        0        0      652 2023-06-06 01:45:59.165403 watchmen_storage_rds-16.5.4/src/watchmen_storage_rds/dbscript_builder.py
--rw-r--r--   0        0        0      518 2023-06-06 01:45:59.165403 watchmen_storage_rds-16.5.4/src/watchmen_storage_rds/ext_types.py
--rw-r--r--   0        0        0      672 2023-06-06 01:45:59.165403 watchmen_storage_rds-16.5.4/src/watchmen_storage_rds/settings.py
--rw-r--r--   0        0        0      941 2023-06-06 01:45:59.165403 watchmen_storage_rds-16.5.4/src/watchmen_storage_rds/sort_build.py
--rw-r--r--   0        0        0    17832 2023-06-06 01:45:59.165403 watchmen_storage_rds-16.5.4/src/watchmen_storage_rds/storage_rds.py
--rw-r--r--   0        0        0    22728 2023-06-06 01:45:59.165403 watchmen_storage_rds-16.5.4/src/watchmen_storage_rds/table_defs.py
--rw-r--r--   0        0        0     2249 2023-06-06 01:45:59.165403 watchmen_storage_rds-16.5.4/src/watchmen_storage_rds/table_defs_helper.py
--rw-r--r--   0        0        0    22999 2023-06-06 01:45:59.165403 watchmen_storage_rds-16.5.4/src/watchmen_storage_rds/topic_data_storage_rds.py
--rw-r--r--   0        0        0     8191 2023-06-06 01:45:59.165403 watchmen_storage_rds-16.5.4/src/watchmen_storage_rds/topic_table_generate.py
--rw-r--r--   0        0        0      916 2023-06-06 01:45:59.165403 watchmen_storage_rds-16.5.4/src/watchmen_storage_rds/types.py
--rw-r--r--   0        0        0      524 1970-01-01 00:00:00.000000 watchmen_storage_rds-16.5.4/PKG-INFO
+-rw-r--r--   0        0        0      455 2023-06-06 07:52:17.125012 watchmen_storage_rds-16.5.5/pyproject.toml
+-rw-r--r--   0        0        0      643 2023-06-06 07:52:17.125012 watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/__init__.py
+-rw-r--r--   0        0        0      652 2023-06-06 07:52:17.125012 watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/dbscript_builder.py
+-rw-r--r--   0        0        0      518 2023-06-06 07:52:17.125012 watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/ext_types.py
+-rw-r--r--   0        0        0      672 2023-06-06 07:52:17.125012 watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/settings.py
+-rw-r--r--   0        0        0      941 2023-06-06 07:52:17.125012 watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/sort_build.py
+-rw-r--r--   0        0        0    17832 2023-06-06 07:52:17.125012 watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/storage_rds.py
+-rw-r--r--   0        0        0    22728 2023-06-06 07:52:17.125012 watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/table_defs.py
+-rw-r--r--   0        0        0     2249 2023-06-06 07:52:17.125012 watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/table_defs_helper.py
+-rw-r--r--   0        0        0    23204 2023-06-06 07:52:17.125012 watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/topic_data_storage_rds.py
+-rw-r--r--   0        0        0     8191 2023-06-06 07:52:17.125012 watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/topic_table_generate.py
+-rw-r--r--   0        0        0      916 2023-06-06 07:52:17.125012 watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/types.py
+-rw-r--r--   0        0        0      524 1970-01-01 00:00:00.000000 watchmen_storage_rds-16.5.5/PKG-INFO
```

### Comparing `watchmen_storage_rds-16.5.4/src/watchmen_storage_rds/__init__.py` & `watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/__init__.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.5.4/src/watchmen_storage_rds/dbscript_builder.py` & `watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/dbscript_builder.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.5.4/src/watchmen_storage_rds/ext_types.py` & `watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/ext_types.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.5.4/src/watchmen_storage_rds/settings.py` & `watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/settings.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.5.4/src/watchmen_storage_rds/sort_build.py` & `watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/sort_build.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.5.4/src/watchmen_storage_rds/storage_rds.py` & `watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/storage_rds.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.5.4/src/watchmen_storage_rds/table_defs.py` & `watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/table_defs.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.5.4/src/watchmen_storage_rds/table_defs_helper.py` & `watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/table_defs_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.5.4/src/watchmen_storage_rds/topic_data_storage_rds.py` & `watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/topic_data_storage_rds.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from watchmen_model.admin import Factor, FactorType, Topic
 from watchmen_model.common import DataPage, TopicId
 from watchmen_storage import as_table_name, EntityHelper, FreeAggregateArithmetic, FreeAggregateColumn, \
 	FreeAggregatePager, FreeAggregator, FreeColumn, FreeFinder, FreeJoin, FreeJoinType, FreePager, Literal, \
 	NoFreeJoinException, TopicDataStorageSPI, UnexpectedStorageException
 from watchmen_storage.settings import ask_sql_analyzer_on
-from watchmen_storage.sql_analysis.ast_vister import SqlContext, QueryPerformance
+from watchmen_storage.sql_analysis.ast_vister import QueryPerformance
 from watchmen_storage.sql_analysis.parse_sql import SqlParser
 from watchmen_utilities import ArrayHelper, is_not_blank
 from .storage_rds import StorageRDS
 from .table_defs import register_table
 from .types import SQLAlchemyStatement
 
 logger = getLogger(__name__)
@@ -51,15 +51,15 @@
 		raise UnexpectedStorageException('Method[ask_synonym_columns_sql] does not support by rds storage.')
 
 	@abstractmethod
 	def schema_column_data_type_to_factor_type(self, schema_column_data_type: str) -> Tuple[FactorType, Optional[str]]:
 		raise UnexpectedStorageException(
 			'Method[schema_column_data_type_to_factor_type] does not support by rds storage.')
 
-
+	# noinspection PyMethodMayBeStatic
 	def get_value_from_row_data(self, row: Dict[str, Any], key: str) -> Any:
 		return row.get(key) or row.get(key.lower())
 
 	def schema_column_to_factor(self, column: Dict[str, Any], index: int) -> Factor:
 		factor_type, factor_precision = \
 			self.schema_column_data_type_to_factor_type(self.get_value_from_row_data(column, 'COLUMN_TYPE'))
 		return Factor(
@@ -401,38 +401,39 @@
 		data_statement = self.build_criteria_for_statement(tables, data_statement, finder.criteria)
 		# build aggregate query
 		data_statement = self.build_fake_aggregation_statement(finder.columns, data_statement)
 		# build when recalculate columns existing
 		data_statement = self.build_recalculate_columns(finder.columns, data_statement)
 		return data_statement
 
-	def extract_sql(self,sql_query)->QueryPerformance:
+	# noinspection PyMethodMayBeStatic
+	def extract_sql(self, sql_query) -> QueryPerformance:
 		if ask_sql_analyzer_on():
 			sql = str(sql_query)
 			sql_parser = SqlParser()
 			return sql_parser.parse(sql)
 
-
 	def free_find(self, finder: FreeFinder) -> List[Dict[str, Any]]:
 		data_statement = self.build_free_find_statement(finder)
-		print("----------")
+		# print("----------")
+		# noinspection DuplicatedCode
 		sql = data_statement.compile(dialect=self.connection.dialect, compile_kwargs={"literal_binds": True})
-		query_performance =  self.extract_sql(sql)
-
+		query_performance = self.extract_sql(sql)
 
 		start = timer()
+		# noinspection DuplicatedCode
 		results = self.connection.execute(data_statement).mappings().all()
 		end = timer()
 
 		query_performance.execution_time = end - start
 		query_performance.data_volume = len(results)
-		print(query_performance)
+		# print(query_performance)
 
-		if finder.preExecutor:
-			finder.preExecutor(query_performance, True)
+		if finder.queryPfmMonitor:
+			finder.queryPfmMonitor(query_performance, True)
 
 		return ArrayHelper(results) \
 			.map(lambda x: self.deserialize_from_auto_generated_columns(x, finder.columns)) \
 			.to_list()
 
 	# noinspection DuplicatedCode
 	def free_page(self, pager: FreePager) -> DataPage:
@@ -454,33 +455,31 @@
 		else:
 			sub_query = data_statement.subquery()
 			count_statement = select(func.count()).select_from(sub_query)
 			count, empty_page = self.execute_page_count(count_statement, page_size)
 			if count == 0:
 				return empty_page
 
-
 		page_number, max_page_number = self.compute_page(count, page_size, pager.pageable.pageNumber)
 		data_statement = self.build_offset_for_statement(data_statement, page_size, page_number)
 
-		print("----------")
-		sql = data_statement.compile(dialect=self.connection.dialect,compile_kwargs={"literal_binds": True})
+		# print("----------")
+		sql = data_statement.compile(dialect=self.connection.dialect, compile_kwargs={"literal_binds": True})
 		query_performance = self.extract_sql(sql)
-		print("----------")
+		# print("----------")
 
 		start = timer()
 		results = self.connection.execute(data_statement).mappings().all()
 		end = timer()
 
 		query_performance.execution_time = end - start
 		query_performance.data_volume = len(results)
-		print(query_performance)
-		if pager.preExecutor:
-			pager.preExecutor(query_performance,True)
-
+		# print(query_performance)
+		if pager.queryPfmMonitor:
+			pager.queryPfmMonitor(query_performance, True)
 
 		results = ArrayHelper(results) \
 			.map(lambda x: self.deserialize_from_auto_generated_columns(x, pager.columns)) \
 			.to_list()
 
 		return DataPage(
 			data=results,
@@ -492,33 +491,31 @@
 
 	def free_aggregate_find(self, aggregator: FreeAggregator) -> List[Dict[str, Any]]:
 		_, data_statement = self.build_aggregate_statement(aggregator)
 		data_statement = self.build_sort_for_statement(data_statement, aggregator.highOrderSortColumns)
 		if aggregator.highOrderTruncation is not None and aggregator.highOrderTruncation > 0:
 			data_statement = data_statement.limit(aggregator.highOrderTruncation)
 
+		# noinspection DuplicatedCode
 		sql = data_statement.compile(dialect=self.connection.dialect, compile_kwargs={"literal_binds": True})
 		query_performance = self.extract_sql(sql)
 		start = timer()
-		print("-----adad-----")
+		# print("-----adad-----")
 		results = self.connection.execute(data_statement).mappings().all()
 		end = timer()
-		print("-------asdadd---")
+		# print("-------asdadd---")
 		query_performance.execution_time = end - start
 		query_performance.data_volume = len(results)
-		print(query_performance)
-		if aggregator.preExecutor:
-			aggregator.preExecutor(query_performance, False)
-
+		# print(query_performance)
+		if aggregator.queryPfmMonitor:
+			aggregator.queryPfmMonitor(query_performance, False)
 
 		def deserialize(row: Dict[str, Any]) -> Dict[str, Any]:
 			return self.deserialize_from_auto_generated_aggregate_columns(row, aggregator.highOrderAggregateColumns)
 
-
-
 		return ArrayHelper(results).map(lambda x: deserialize(x)).to_list()
 
 	# noinspection DuplicatedCode
 	def free_aggregate_page(self, pager: FreeAggregatePager) -> DataPage:
 		page_size = pager.pageable.pageSize
 
 		_, data_statement = self.build_aggregate_statement(pager)
@@ -533,28 +530,27 @@
 			count, empty_page = self.execute_page_count(count_statement, page_size)
 			if count == 0:
 				return empty_page
 
 		data_statement = self.build_sort_for_statement(data_statement, pager.highOrderSortColumns)
 		page_number, max_page_number = self.compute_page(count, page_size, pager.pageable.pageNumber)
 		data_statement = self.build_offset_for_statement(data_statement, page_size, page_number)
-		print("----------")
-		sql  = data_statement.compile(dialect=self.connection.dialect, compile_kwargs={"literal_binds": True})
+		# print("----------")
+		sql = data_statement.compile(dialect=self.connection.dialect, compile_kwargs={"literal_binds": True})
 		query_performance = self.extract_sql(sql)
-		print("----------")
+		# print("----------")
 		start = timer()
 		results = self.connection.execute(data_statement).mappings().all()
 		end = timer()
 		query_performance.execution_time = end - start
 		query_performance.data_volume = len(results)
-		print(query_performance)
-
-		if pager.preExecutor:
-			pager.preExecutor(query_performance,True)
+		# print(query_performance)
 
+		if pager.queryPfmMonitor:
+			pager.queryPfmMonitor(query_performance, True)
 
 		def deserialize(row: Dict[str, Any]) -> Dict[str, Any]:
 			return self.deserialize_from_auto_generated_aggregate_columns(row, pager.highOrderAggregateColumns)
 
 		results = ArrayHelper(results).map(lambda x: deserialize(x)).to_list()
 
 		return DataPage(
```

### Comparing `watchmen_storage_rds-16.5.4/src/watchmen_storage_rds/topic_table_generate.py` & `watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/topic_table_generate.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.5.4/src/watchmen_storage_rds/types.py` & `watchmen_storage_rds-16.5.5/src/watchmen_storage_rds/types.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage_rds-16.5.4/PKG-INFO` & `watchmen_storage_rds-16.5.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: watchmen-storage-rds
-Version: 16.5.4
+Version: 16.5.5
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
-Requires-Dist: watchmen-storage (==16.5.4)
+Requires-Dist: watchmen-storage (==16.5.5)
```

