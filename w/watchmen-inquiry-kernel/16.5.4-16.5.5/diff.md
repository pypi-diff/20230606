# Comparing `tmp/watchmen_inquiry_kernel-16.5.4.tar.gz` & `tmp/watchmen_inquiry_kernel-16.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_inquiry_kernel-16.5.4.tar", max compression
+gzip compressed data, was "watchmen_inquiry_kernel-16.5.5.tar", max compression
```

## Comparing `watchmen_inquiry_kernel-16.5.4.tar` & `watchmen_inquiry_kernel-16.5.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1061 2023-06-06 01:45:59.129402 watchmen_inquiry_kernel-16.5.4/LICENSE
--rw-r--r--   0        0        0     1274 2023-06-06 01:45:59.129402 watchmen_inquiry_kernel-16.5.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-06 01:45:59.129402 watchmen_inquiry_kernel-16.5.4/src/watchmen_inquiry_kernel/__init__.py
--rw-r--r--   0        0        0      112 2023-06-06 01:45:59.129402 watchmen_inquiry_kernel-16.5.4/src/watchmen_inquiry_kernel/common/__init__.py
--rw-r--r--   0        0        0       47 2023-06-06 01:45:59.129402 watchmen_inquiry_kernel-16.5.4/src/watchmen_inquiry_kernel/common/exception.py
--rw-r--r--   0        0        0      620 2023-06-06 01:45:59.129402 watchmen_inquiry_kernel-16.5.4/src/watchmen_inquiry_kernel/common/settings.py
--rw-r--r--   0        0        0       86 2023-06-06 01:45:59.129402 watchmen_inquiry_kernel-16.5.4/src/watchmen_inquiry_kernel/meta/__init__.py
--rw-r--r--   0        0        0     1847 2023-06-06 01:45:59.129402 watchmen_inquiry_kernel-16.5.4/src/watchmen_inquiry_kernel/meta/enum_service.py
--rw-r--r--   0        0        0     1404 2023-06-06 01:45:59.129402 watchmen_inquiry_kernel-16.5.4/src/watchmen_inquiry_kernel/meta/report_service.py
--rw-r--r--   0        0        0     2358 2023-06-06 01:45:59.129402 watchmen_inquiry_kernel-16.5.4/src/watchmen_inquiry_kernel/meta/subject_service.py
--rw-r--r--   0        0        0       82 2023-06-06 01:45:59.129402 watchmen_inquiry_kernel-16.5.4/src/watchmen_inquiry_kernel/schema/__init__.py
--rw-r--r--   0        0        0     2178 2023-06-06 01:45:59.129402 watchmen_inquiry_kernel-16.5.4/src/watchmen_inquiry_kernel/schema/report_schema.py
--rw-r--r--   0        0        0    12544 2023-06-06 01:45:59.129402 watchmen_inquiry_kernel-16.5.4/src/watchmen_inquiry_kernel/schema/subject_schema.py
--rw-r--r--   0        0        0      104 2023-06-06 01:45:59.129402 watchmen_inquiry_kernel-16.5.4/src/watchmen_inquiry_kernel/storage/__init__.py
--rw-r--r--   0        0        0     1544 2023-06-06 01:45:59.129402 watchmen_inquiry_kernel-16.5.4/src/watchmen_inquiry_kernel/storage/report_data_service.py
--rw-r--r--   0        0        0     1228 2023-06-06 01:45:59.129402 watchmen_inquiry_kernel-16.5.4/src/watchmen_inquiry_kernel/storage/subject_data_service.py
--rw-r--r--   0        0        0    54334 2023-06-06 01:45:59.129402 watchmen_inquiry_kernel-16.5.4/src/watchmen_inquiry_kernel/storage/subject_storage.py
--rw-r--r--   0        0        0     1223 1970-01-01 00:00:00.000000 watchmen_inquiry_kernel-16.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-06 07:52:17.089011 watchmen_inquiry_kernel-16.5.5/LICENSE
+-rw-r--r--   0        0        0     1275 2023-06-06 07:52:17.089011 watchmen_inquiry_kernel-16.5.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-06 07:52:17.089011 watchmen_inquiry_kernel-16.5.5/src/watchmen_inquiry_kernel/__init__.py
+-rw-r--r--   0        0        0      112 2023-06-06 07:52:17.089011 watchmen_inquiry_kernel-16.5.5/src/watchmen_inquiry_kernel/common/__init__.py
+-rw-r--r--   0        0        0       47 2023-06-06 07:52:17.089011 watchmen_inquiry_kernel-16.5.5/src/watchmen_inquiry_kernel/common/exception.py
+-rw-r--r--   0        0        0      620 2023-06-06 07:52:17.089011 watchmen_inquiry_kernel-16.5.5/src/watchmen_inquiry_kernel/common/settings.py
+-rw-r--r--   0        0        0       86 2023-06-06 07:52:17.089011 watchmen_inquiry_kernel-16.5.5/src/watchmen_inquiry_kernel/meta/__init__.py
+-rw-r--r--   0        0        0     1847 2023-06-06 07:52:17.089011 watchmen_inquiry_kernel-16.5.5/src/watchmen_inquiry_kernel/meta/enum_service.py
+-rw-r--r--   0        0        0     1404 2023-06-06 07:52:17.089011 watchmen_inquiry_kernel-16.5.5/src/watchmen_inquiry_kernel/meta/report_service.py
+-rw-r--r--   0        0        0     2358 2023-06-06 07:52:17.089011 watchmen_inquiry_kernel-16.5.5/src/watchmen_inquiry_kernel/meta/subject_service.py
+-rw-r--r--   0        0        0       82 2023-06-06 07:52:17.089011 watchmen_inquiry_kernel-16.5.5/src/watchmen_inquiry_kernel/schema/__init__.py
+-rw-r--r--   0        0        0     2178 2023-06-06 07:52:17.089011 watchmen_inquiry_kernel-16.5.5/src/watchmen_inquiry_kernel/schema/report_schema.py
+-rw-r--r--   0        0        0    12544 2023-06-06 07:52:17.089011 watchmen_inquiry_kernel-16.5.5/src/watchmen_inquiry_kernel/schema/subject_schema.py
+-rw-r--r--   0        0        0      104 2023-06-06 07:52:17.089011 watchmen_inquiry_kernel-16.5.5/src/watchmen_inquiry_kernel/storage/__init__.py
+-rw-r--r--   0        0        0     1769 2023-06-06 07:52:17.089011 watchmen_inquiry_kernel-16.5.5/src/watchmen_inquiry_kernel/storage/report_data_service.py
+-rw-r--r--   0        0        0     1496 2023-06-06 07:52:17.089011 watchmen_inquiry_kernel-16.5.5/src/watchmen_inquiry_kernel/storage/subject_data_service.py
+-rw-r--r--   0        0        0    54423 2023-06-06 07:52:17.089011 watchmen_inquiry_kernel-16.5.5/src/watchmen_inquiry_kernel/storage/subject_storage.py
+-rw-r--r--   0        0        0     1223 1970-01-01 00:00:00.000000 watchmen_inquiry_kernel-16.5.5/PKG-INFO
```

### Comparing `watchmen_inquiry_kernel-16.5.4/LICENSE` & `watchmen_inquiry_kernel-16.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.5.4/pyproject.toml` & `watchmen_inquiry_kernel-16.5.5/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [tool.poetry]
 name = "watchmen-inquiry-kernel"
-version = "16.5.4"
+version = "16.5.5"
 description = ""
 authors = ["botlikes <75356972+botlikes456@users.noreply.github.com>"]
 license = "MIT"
 packages = [
     { include = "watchmen_inquiry_kernel", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-watchmen-data-kernel = "16.5.4"
-watchmen-inquiry-trino = { version = "16.5.4", optional = true }
-watchmen-storage-mysql = { version = "16.5.4", optional = true }
-watchmen-storage-oracle = { version = "16.5.4", optional = true }
-watchmen-storage-mongodb = { version = "16.5.4", optional = true }
-watchmen-storage-mssql = { version = "16.5.4", optional = true }
-watchmen-storage-postgresql = { version = "16.5.4", optional = true }
-watchmen-storage-oss = { version = "16.5.4", optional = true }
-watchmen-storage-s3 = { version = "16.5.4", optional = true }
+watchmen-data-kernel = "16.5.5"
+watchmen-inquiry-trino = { version = "16.5.5", optional = true }
+watchmen-storage-mysql = { version = "16.5.5", optional = true }
+watchmen-storage-oracle = { version = "16.5.5", optional = true }
+watchmen-storage-mongodb = { version = "16.5.5", optional = true }
+watchmen-storage-mssql = { version = "16.5.5", optional = true }
+watchmen-storage-postgresql = { version = "16.5.5", optional = true }
+watchmen-storage-oss = { version = "16.5.5", optional = true }
+watchmen-storage-s3 = { version = "16.5.5", optional = true }
+
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.extras]
 mysql = ["watchmen-storage-mysql"]
 oracle = ["watchmen-storage-oracle"]
 mongodb = ["watchmen-storage-mongodb"]
```

### Comparing `watchmen_inquiry_kernel-16.5.4/src/watchmen_inquiry_kernel/common/settings.py` & `watchmen_inquiry_kernel-16.5.5/src/watchmen_inquiry_kernel/common/settings.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.5.4/src/watchmen_inquiry_kernel/meta/enum_service.py` & `watchmen_inquiry_kernel-16.5.5/src/watchmen_inquiry_kernel/meta/enum_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.5.4/src/watchmen_inquiry_kernel/meta/report_service.py` & `watchmen_inquiry_kernel-16.5.5/src/watchmen_inquiry_kernel/meta/report_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.5.4/src/watchmen_inquiry_kernel/meta/subject_service.py` & `watchmen_inquiry_kernel-16.5.5/src/watchmen_inquiry_kernel/meta/subject_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.5.4/src/watchmen_inquiry_kernel/schema/report_schema.py` & `watchmen_inquiry_kernel-16.5.5/src/watchmen_inquiry_kernel/schema/report_schema.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.5.4/src/watchmen_inquiry_kernel/schema/subject_schema.py` & `watchmen_inquiry_kernel-16.5.5/src/watchmen_inquiry_kernel/schema/subject_schema.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_kernel-16.5.4/src/watchmen_inquiry_kernel/storage/report_data_service.py` & `watchmen_inquiry_kernel-16.5.5/src/watchmen_inquiry_kernel/storage/report_data_service.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,26 +14,35 @@
 
 	def get_schema(self) -> ReportSchema:
 		return self.schema
 
 	def get_report(self) -> Report:
 		return self.schema.get_report()
 
-	def find(self) -> DataResult:
+	def create_subject_storage(self) -> SubjectStorage:
 		subject_schema = self.subject_data_service.get_schema()
 		principal_service = self.subject_data_service.get_principal_service()
-		storage = SubjectStorage(subject_schema, principal_service)
+		return SubjectStorage(subject_schema, principal_service)
+
+	def find(self) -> DataResult:
+		storage = self.create_subject_storage()
 		data = storage.aggregate_find(self.get_schema())
 
 		return DataResult(
 			columns=self.get_schema().get_result_columns(),
 			data=self.get_schema().translate_to_array_table(data)
 		)
 
+	def find_sql(self) -> str:
+		storage = self.create_subject_storage()
+		return storage.aggregate_find_sql(self.get_schema())
+
 	def page(self, pageable: Pageable) -> DataPage:
-		subject_schema = self.subject_data_service.get_schema()
-		principal_service = self.subject_data_service.get_principal_service()
-		storage = SubjectStorage(subject_schema, principal_service)
+		storage = self.create_subject_storage()
 		page = storage.aggregate_page(self.get_schema(), pageable)
 		# translate to a data table
 		page.data = self.get_schema().translate_to_array_table(page.data)
 		return page
+
+	def page_sql(self, pageable: Pageable) -> str:
+		storage = self.create_subject_storage()
+		return storage.aggregate_page_sql(self.get_schema(), pageable)
```

### Comparing `watchmen_inquiry_kernel-16.5.4/src/watchmen_inquiry_kernel/storage/subject_storage.py` & `watchmen_inquiry_kernel-16.5.5/src/watchmen_inquiry_kernel/storage/subject_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from abc import abstractmethod
 from datetime import date
 from decimal import Decimal
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
+from watchmen_pipeline_kernel.pipeline.sql_performance_invoker import create_sql_performance_pipeline_invoker
+
 from watchmen_auth import PrincipalService
 from watchmen_data_kernel.common import ask_all_date_formats, ask_time_formats
 from watchmen_data_kernel.service import ask_topic_storage
 from watchmen_data_kernel.storage_bridge import ask_topic_data_entity_helper, parse_condition_for_storage, \
 	parse_parameter_for_storage, ParsedStorageCondition, PipelineVariables, PossibleParameterType
 from watchmen_data_kernel.topic_schema import TopicSchema
 from watchmen_data_kernel.utils import MightAVariable, parse_function_in_variable, parse_move_date_pattern, \
@@ -22,15 +24,14 @@
 from watchmen_model.common import ComputedParameter, ConstantParameter, DataModel, DataPage, FactorId, Pageable, \
 	Parameter, ParameterComputeType, ParameterCondition, ParameterExpression, ParameterExpressionOperator, \
 	ParameterJoint, ParameterJointType, SubjectDatasetColumnId, TopicFactorParameter, TopicId, \
 	VariablePredefineFunctions
 from watchmen_model.console import ConnectedSpace, ReportDimension, ReportFunnel, ReportFunnelType, ReportIndicator, \
 	ReportIndicatorArithmetic, SubjectDatasetColumn, SubjectDatasetJoin, SubjectJoinType
 from watchmen_model.console.subject import Subject, SubjectColumnArithmetic
-from watchmen_pipeline_kernel.pipeline.sql_performance_invoker import create_sql_performance_pipeline_invoker
 from watchmen_storage import ColumnNameLiteral, ComputedLiteral, ComputedLiteralOperator, EntityCriteria, \
 	EntityCriteriaExpression, EntityCriteriaJoint, EntityCriteriaJointConjunction, EntityCriteriaOperator, \
 	EntityCriteriaStatement, EntitySortColumn, EntitySortMethod, FreeAggregateArithmetic, FreeAggregateColumn, \
 	FreeAggregatePager, FreeAggregator, FreeColumn, FreeFinder, FreeJoin, FreeJoinType, FreePager, Literal, \
 	TopicDataStorageSPI
 from watchmen_utilities import ArrayHelper, date_might_with_prefix, get_current_time_in_seconds, is_blank, is_date, \
 	is_decimal, is_not_blank, is_time, month_diff, move_date, translate_date_format_to_memory, truncate_time, year_diff
@@ -314,37 +315,46 @@
 			)]
 		else:
 			joins = ArrayHelper(dataset.joins).map(lambda x: self.build_join(x, available_schemas)).to_list()
 
 		storage = ask_topic_storage(self.schema.get_primary_topic_schema(), self.principalService)
 		# register topic, in case of it is not registered yet
 		ArrayHelper(available_schemas).each(lambda x: storage.register_topic(x.get_topic()))
-		return FreeFinder(columns=columns, joins=joins, criteria=criteria,
-		                  preExecutor=create_sql_performance_pipeline_invoker(str(ask_snowflake_generator().next_id()),
-		                                                                      self.principalService)), possible_types_list
+		return FreeFinder(
+			columns=columns, joins=joins, criteria=criteria,
+			queryPfmMonitor=create_sql_performance_pipeline_invoker(
+				str(ask_snowflake_generator().next_id()), self.principalService)), possible_types_list
 
 	def find(self) -> List[Dict[str, Any]]:
 		finder, _ = self.ask_storage_finder()
 		return self.find_data(lambda agent: agent.free_find(finder))
 
+	def find_sql(self) -> str:
+		# TODO
+		pass
+
 	def ask_storage_pager(self, pageable: Pageable) -> FreePager:
 		finder, _ = self.ask_storage_finder()
 		return FreePager(
 			columns=finder.columns,
 			joins=finder.joins,
 			criteria=finder.criteria,
 			pageable=pageable,
-			preExecutor=create_sql_performance_pipeline_invoker(str(ask_snowflake_generator().next_id()),
-			                                                    self.principalService)
+			queryPfmMonitor=create_sql_performance_pipeline_invoker(
+				str(ask_snowflake_generator().next_id()), self.principalService)
 		)
 
 	def page(self, pageable: Pageable) -> DataPage:
 		return self.find_data(
 			lambda agent: agent.free_page(self.ask_storage_pager(pageable)))
 
+	def page_sql(self, pageable: Pageable) -> str:
+		# TODO
+		pass
+
 	# noinspection PyMethodMayBeStatic
 	def build_aggregate_column_by_indicator(
 			self, indicator: ReportIndicator, indicator_index: int,
 			subject_column_map: Dict[SubjectDatasetColumnId, int], report_schema: ReportSchema
 	) -> FreeAggregateColumn:
 		column_id = indicator.columnId
 		index = subject_column_map.get(column_id)
@@ -1155,41 +1165,50 @@
 			columns=finder.columns,
 			joins=finder.joins,
 			criteria=finder.criteria,
 			highOrderAggregateColumns=self.build_aggregate_columns(report_schema),
 			highOrderCriteria=self.build_high_order_criteria(report_schema, possible_types_list),
 			highOrderSortColumns=self.build_sort_columns(report_schema),
 			highOrderTruncation=report_schema.get_truncation_count(),
-			preExecutor=create_sql_performance_pipeline_invoker(str(ask_snowflake_generator().next_id()),
-			                                                    self.principalService)
+			queryPfmMonitor=create_sql_performance_pipeline_invoker(
+				str(ask_snowflake_generator().next_id()), self.principalService)
 		)
 
 	def aggregate_find(self, report_schema: ReportSchema) -> List[Dict[str, Any]]:
-		return self.find_data(lambda agent: agent.free_aggregate_find(self.ask_storage_aggregator(report_schema)))
+		return self.find_data(
+			lambda agent: agent.free_aggregate_find(self.ask_storage_aggregator(report_schema)))
+
+	def aggregate_find_sql(self, report_schema: ReportSchema) -> str:
+		# TODO
+		pass
 
 	def ask_storage_aggregate_pager(
 			self, report_schema: ReportSchema, pageable: Pageable) -> FreeAggregatePager:
 		aggregator = self.ask_storage_aggregator(report_schema)
 		return FreeAggregatePager(
 			columns=aggregator.columns,
 			joins=aggregator.joins,
 			criteria=aggregator.criteria,
 			highOrderAggregateColumns=aggregator.highOrderAggregateColumns,
 			highOrderCriteria=aggregator.highOrderCriteria,
 			highOrderSortColumns=aggregator.highOrderSortColumns,
 			highOrderTruncation=aggregator.highOrderTruncation,
 			pageable=pageable,
-			preExecutor=create_sql_performance_pipeline_invoker(str(ask_snowflake_generator().next_id()),
-			                                                    self.principalService)
+			queryPfmMonitor=create_sql_performance_pipeline_invoker(
+				str(ask_snowflake_generator().next_id()), self.principalService)
 		)
 
 	def aggregate_page(self, report_schema: ReportSchema, pageable: Pageable) -> DataPage:
 		return self.find_data(
 			lambda agent: agent.free_aggregate_page(self.ask_storage_aggregate_pager(report_schema, pageable)))
 
+	def aggregate_page_sql(self, report_schema: ReportSchema, pageable: Pageable) -> str:
+		# TODO
+		pass
+
 	# noinspection PyMethodMayBeStatic
 	def do_find(
 			self, find_agent: FindAgent, find: Callable[[FindAgent], Union[List[Dict[str, Any]], DataPage]]
 	) -> Union[List[Dict[str, Any]], DataPage]:
 		try:
 			find_agent.connect()
 			return find(find_agent)
```

### Comparing `watchmen_inquiry_kernel-16.5.4/PKG-INFO` & `watchmen_inquiry_kernel-16.5.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchmen-inquiry-kernel
-Version: 16.5.4
+Version: 16.5.5
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
-Requires-Dist: watchmen-data-kernel (==16.5.4)
-Requires-Dist: watchmen-inquiry-trino (==16.5.4) ; extra == "trino"
-Requires-Dist: watchmen-storage-mongodb (==16.5.4) ; extra == "mongodb"
-Requires-Dist: watchmen-storage-mssql (==16.5.4) ; extra == "mssql"
-Requires-Dist: watchmen-storage-mysql (==16.5.4) ; extra == "mysql"
-Requires-Dist: watchmen-storage-oracle (==16.5.4) ; extra == "oracle"
-Requires-Dist: watchmen-storage-oss (==16.5.4) ; extra == "oss"
-Requires-Dist: watchmen-storage-postgresql (==16.5.4) ; extra == "postgresql"
-Requires-Dist: watchmen-storage-s3 (==16.5.4) ; extra == "s3"
+Requires-Dist: watchmen-data-kernel (==16.5.5)
+Requires-Dist: watchmen-inquiry-trino (==16.5.5) ; extra == "trino"
+Requires-Dist: watchmen-storage-mongodb (==16.5.5) ; extra == "mongodb"
+Requires-Dist: watchmen-storage-mssql (==16.5.5) ; extra == "mssql"
+Requires-Dist: watchmen-storage-mysql (==16.5.5) ; extra == "mysql"
+Requires-Dist: watchmen-storage-oracle (==16.5.5) ; extra == "oracle"
+Requires-Dist: watchmen-storage-oss (==16.5.5) ; extra == "oss"
+Requires-Dist: watchmen-storage-postgresql (==16.5.5) ; extra == "postgresql"
+Requires-Dist: watchmen-storage-s3 (==16.5.5) ; extra == "s3"
```

