# Comparing `tmp/watchmen_storage-16.5.4.tar.gz` & `tmp/watchmen_storage-16.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_storage-16.5.4.tar", max compression
+gzip compressed data, was "watchmen_storage-16.5.5.tar", max compression
```

## Comparing `watchmen_storage-16.5.4.tar` & `watchmen_storage-16.5.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1061 2023-06-06 01:45:59.165403 watchmen_storage-16.5.4/LICENSE
--rw-r--r--   0        0        0      492 2023-06-06 01:45:59.165403 watchmen_storage-16.5.4/pyproject.toml
--rw-r--r--   0        0        0     2217 2023-06-06 01:45:59.165403 watchmen_storage-16.5.4/src/watchmen_storage/__init__.py
--rw-r--r--   0        0        0     4917 2023-06-06 01:45:59.165403 watchmen_storage-16.5.4/src/watchmen_storage/competitive_worker_id_generator.py
--rw-r--r--   0        0        0     5549 2023-06-06 01:45:59.165403 watchmen_storage-16.5.4/src/watchmen_storage/data_source_helper.py
--rw-r--r--   0        0        0     1819 2023-06-06 01:45:59.165403 watchmen_storage-16.5.4/src/watchmen_storage/free_storage_types.py
--rw-r--r--   0        0        0      211 2023-06-06 01:45:59.165403 watchmen_storage-16.5.4/src/watchmen_storage/secrets_manager.py
--rw-r--r--   0        0        0      730 2023-06-06 01:45:59.165403 watchmen_storage-16.5.4/src/watchmen_storage/secrets_manager_aws.py
--rw-r--r--   0        0        0     1096 2023-06-06 01:45:59.165403 watchmen_storage-16.5.4/src/watchmen_storage/settings.py
--rw-r--r--   0        0        0     2750 2023-06-06 01:45:59.165403 watchmen_storage-16.5.4/src/watchmen_storage/snowflake.py
--rw-r--r--   0        0        0      232 2023-06-06 01:45:59.165403 watchmen_storage-16.5.4/src/watchmen_storage/snowflake_worker_id_generator.py
--rw-r--r--   0        0        0        0 2023-06-06 01:45:59.165403 watchmen_storage-16.5.4/src/watchmen_storage/sql_analysis/__init__.py
--rw-r--r--   0        0        0    10191 2023-06-06 01:45:59.165403 watchmen_storage-16.5.4/src/watchmen_storage/sql_analysis/ast_vister.py
--rw-r--r--   0        0        0     2632 2023-06-06 01:45:59.165403 watchmen_storage-16.5.4/src/watchmen_storage/sql_analysis/parse_sql.py
--rw-r--r--   0        0        0      890 2023-06-06 01:45:59.165403 watchmen_storage-16.5.4/src/watchmen_storage/sql_analysis/query_performance_service.py
--rw-r--r--   0        0        0     1441 2023-06-06 01:45:59.165403 watchmen_storage-16.5.4/src/watchmen_storage/sql_analysis/topic_generator.py
--rw-r--r--   0        0        0     7259 2023-06-06 01:45:59.165403 watchmen_storage-16.5.4/src/watchmen_storage/storage_based_worker_id_generator.py
--rw-r--r--   0        0        0      721 2023-06-06 01:45:59.165403 watchmen_storage-16.5.4/src/watchmen_storage/storage_exception.py
--rw-r--r--   0        0        0     5998 2023-06-06 01:45:59.165403 watchmen_storage-16.5.4/src/watchmen_storage/storage_spi.py
--rw-r--r--   0        0        0     4717 2023-06-06 01:45:59.165403 watchmen_storage-16.5.4/src/watchmen_storage/storage_types.py
--rw-r--r--   0        0        0      630 2023-06-06 01:45:59.165403 watchmen_storage-16.5.4/src/watchmen_storage/topic_utils.py
--rw-r--r--   0        0        0      562 1970-01-01 00:00:00.000000 watchmen_storage-16.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-06 07:52:17.125012 watchmen_storage-16.5.5/LICENSE
+-rw-r--r--   0        0        0      443 2023-06-06 07:52:17.125012 watchmen_storage-16.5.5/pyproject.toml
+-rw-r--r--   0        0        0     2217 2023-06-06 07:52:17.125012 watchmen_storage-16.5.5/src/watchmen_storage/__init__.py
+-rw-r--r--   0        0        0     4917 2023-06-06 07:52:17.125012 watchmen_storage-16.5.5/src/watchmen_storage/competitive_worker_id_generator.py
+-rw-r--r--   0        0        0     5549 2023-06-06 07:52:17.125012 watchmen_storage-16.5.5/src/watchmen_storage/data_source_helper.py
+-rw-r--r--   0        0        0     1825 2023-06-06 07:52:17.125012 watchmen_storage-16.5.5/src/watchmen_storage/free_storage_types.py
+-rw-r--r--   0        0        0      211 2023-06-06 07:52:17.125012 watchmen_storage-16.5.5/src/watchmen_storage/secrets_manager.py
+-rw-r--r--   0        0        0      730 2023-06-06 07:52:17.125012 watchmen_storage-16.5.5/src/watchmen_storage/secrets_manager_aws.py
+-rw-r--r--   0        0        0     1096 2023-06-06 07:52:17.125012 watchmen_storage-16.5.5/src/watchmen_storage/settings.py
+-rw-r--r--   0        0        0     2750 2023-06-06 07:52:17.125012 watchmen_storage-16.5.5/src/watchmen_storage/snowflake.py
+-rw-r--r--   0        0        0      232 2023-06-06 07:52:17.125012 watchmen_storage-16.5.5/src/watchmen_storage/snowflake_worker_id_generator.py
+-rw-r--r--   0        0        0        0 2023-06-06 07:52:17.125012 watchmen_storage-16.5.5/src/watchmen_storage/sql_analysis/__init__.py
+-rw-r--r--   0        0        0    10961 2023-06-06 07:52:17.125012 watchmen_storage-16.5.5/src/watchmen_storage/sql_analysis/ast_vister.py
+-rw-r--r--   0        0        0     2832 2023-06-06 07:52:17.125012 watchmen_storage-16.5.5/src/watchmen_storage/sql_analysis/parse_sql.py
+-rw-r--r--   0        0        0      890 2023-06-06 07:52:17.125012 watchmen_storage-16.5.5/src/watchmen_storage/sql_analysis/query_performance_service.py
+-rw-r--r--   0        0        0     1441 2023-06-06 07:52:17.125012 watchmen_storage-16.5.5/src/watchmen_storage/sql_analysis/topic_generator.py
+-rw-r--r--   0        0        0     7259 2023-06-06 07:52:17.125012 watchmen_storage-16.5.5/src/watchmen_storage/storage_based_worker_id_generator.py
+-rw-r--r--   0        0        0      721 2023-06-06 07:52:17.125012 watchmen_storage-16.5.5/src/watchmen_storage/storage_exception.py
+-rw-r--r--   0        0        0     5998 2023-06-06 07:52:17.125012 watchmen_storage-16.5.5/src/watchmen_storage/storage_spi.py
+-rw-r--r--   0        0        0     4717 2023-06-06 07:52:17.125012 watchmen_storage-16.5.5/src/watchmen_storage/storage_types.py
+-rw-r--r--   0        0        0      630 2023-06-06 07:52:17.125012 watchmen_storage-16.5.5/src/watchmen_storage/topic_utils.py
+-rw-r--r--   0        0        0      521 1970-01-01 00:00:00.000000 watchmen_storage-16.5.5/PKG-INFO
```

### Comparing `watchmen_storage-16.5.4/LICENSE` & `watchmen_storage-16.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.4/src/watchmen_storage/__init__.py` & `watchmen_storage-16.5.5/src/watchmen_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.4/src/watchmen_storage/competitive_worker_id_generator.py` & `watchmen_storage-16.5.5/src/watchmen_storage/competitive_worker_id_generator.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.4/src/watchmen_storage/data_source_helper.py` & `watchmen_storage-16.5.5/src/watchmen_storage/data_source_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.4/src/watchmen_storage/free_storage_types.py` & `watchmen_storage-16.5.5/src/watchmen_storage/free_storage_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from typing import List, Optional, Callable
+from typing import Callable, List, Optional
 
 from watchmen_model.common import DataModel, Pageable
 from .sql_analysis.ast_vister import QueryPerformance
 from .storage_types import ColumnNameLiteral, EntityCriteria, EntitySortColumn, Literal
 
 
 class FreeAggregateArithmetic(str, Enum):
@@ -35,15 +35,15 @@
 	type: Optional[FreeJoinType] = None
 
 
 class FreeFinder(DataModel):
 	columns: List[FreeColumn] = None
 	joins: List[FreeJoin] = None
 	criteria: Optional[EntityCriteria] = None
-	preExecutor: Optional[Callable[[QueryPerformance,bool],None]] = None
+	queryPfmMonitor: Optional[Callable[[QueryPerformance, bool], None]] = None
 
 
 class FreeAggregateColumn(DataModel):
 	name: str  # name must match free column's index, such as column_1, column_2 (starts from 1)
 	arithmetic: Optional[FreeAggregateArithmetic] = None
 	alias: Optional[str] = None
```

### Comparing `watchmen_storage-16.5.4/src/watchmen_storage/secrets_manager_aws.py` & `watchmen_storage-16.5.5/src/watchmen_storage/secrets_manager_aws.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.4/src/watchmen_storage/settings.py` & `watchmen_storage-16.5.5/src/watchmen_storage/settings.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.4/src/watchmen_storage/snowflake.py` & `watchmen_storage-16.5.5/src/watchmen_storage/snowflake.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.4/src/watchmen_storage/sql_analysis/ast_vister.py` & `watchmen_storage-16.5.5/src/watchmen_storage/sql_analysis/ast_vister.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from pydantic import BaseModel
-from sqlparse.sql import Token, Identifier, Parenthesis, Function, IdentifierList, Where, Comparison, Case
+from sqlparse.sql import Case, Comparison, Function, Identifier, IdentifierList, Parenthesis, Token, Where
 
 
 class SqlContext(BaseModel):
-	status: str =None
-	sub_status: str =None
-	table: list =[]
+	status: str = None
+	sub_status: str = None
+	table: list = []
 	group_by: list = []
-	joins: list =[]
+	joins: list = []
 	where: list = []
-	columns: dict ={"level_0":[],"level_1":[],"level_2":[]}
-	function:list = []
-	level:int = -1
+	columns: dict = {"level_0": [], "level_1": [], "level_2": []}
+	function: list = []
+	level: int = -1
+
 
 class SqlColumn(BaseModel):
 	"""
 	Represents a column in a sql select statement
 	"""
 	name: str = None
 	alias: str = None
@@ -51,21 +52,22 @@
 	alias: str = None
 	table: str = None
 	operator: str = None
 	value: str = None
 
 
 class QueryPerformance(BaseModel):
-	topic_dimensions:str = None
-	column_dimensions:str = None
-	execution_time:int = None
-	data_volume:int = None
-	join_dimensions:str = None
-	where_dimensions:str = None
-	group_by_dimensions:str = None
+	topic_dimensions: str = None
+	column_dimensions: str = None
+	execution_time: int = None
+	data_volume: int = None
+	join_dimensions: str = None
+	where_dimensions: str = None
+	group_by_dimensions: str = None
+	sql: str = None
 
 
 def build_function(name):
 	if value_is_function(name):
 		return name
 	else:
 		return None
@@ -89,15 +91,15 @@
 		column = column_dict[key][-1]
 		column.name = value
 	else:
 		column = SqlColumn(name=value)
 		column_dict[key].append(column)
 
 
-def add_column_as(context:SqlContext, value):
+def add_column_as(context: SqlContext, value):
 	if context.level == 0:
 		column_dict = context.columns
 		column = column_dict["level_0"][-1]
 		column.alias = value
 	elif context.level == 1:
 		column_dict = context.columns
 		column = column_dict["level_1"][-1]
@@ -106,21 +108,25 @@
 		column_dict = context.columns
 		column = column_dict["level_2"][-1]
 		column.alias = value
 
 
 def find_operator(token: Token):
 	"""
-
 	:param token:
 	:return:
 	"""
 	for sub_token in token.tokens:
 		if isinstance(sub_token, Token):
-			if sub_token.normalized == "=" or sub_token.normalized == ">" or sub_token.normalized == "<" or sub_token.normalized == ">=" or sub_token.normalized == "<=" or sub_token.normalized == "!=":
+			if sub_token.normalized == "=" \
+					or sub_token.normalized == ">" \
+					or sub_token.normalized == "<" \
+					or sub_token.normalized == ">=" \
+					or sub_token.normalized == "<=" \
+					or sub_token.normalized == "!=":
 				return sub_token.normalized
 
 
 def add_column_topic(context, value):
 	"""
 	:param context:
 	:param value:
@@ -136,15 +142,15 @@
 		column_dict["level_1"].append(column)
 	elif context.level == 2:
 		column_dict = context.columns
 		column = SqlColumn(table=value)
 		column_dict["level_2"].append(column)
 
 
-def set_status(context:SqlContext, token: Token):
+def set_status(context: SqlContext, token: Token):
 	if token.is_keyword and token.value.upper() == 'SELECT':
 		context.status = "select"
 		context.level = context.level + 1
 	elif token.is_keyword and token.value.upper() == 'FROM':
 		context.status = "from"
 	elif token.is_keyword and token.value.upper() == "AS":
 		if context.status == "from":
@@ -160,42 +166,50 @@
 	# elif token.value == "IN" or token.value == "NOT IN" or token.value == "EXISTS" or token.value == "NOT EXISTS":
 	elif context.status == "case":
 		context.sub_status = token.value
 	elif token.is_keyword or value_is_function(token.value):
 		function = build_function(token.value)
 		context.function.append(function)
 
+
 def get_current_column(context):
 	column_dict = context.columns
 	level = context.level
 	key = "level_" + str(level)
 	return column_dict[key][-1]
 
 
-class TokenVister:
-
+class TokenVisitor:
+	# noinspection PyMethodMayBeStatic
 	def support(self, ast):
 		return isinstance(ast, Token)
 
+	# noinspection PyUnusedLocal
 	def process(self, token: Token, context, visitor_list, previous_token: Token = None, next_token: Token = None):
 		if self.ignore_value(token):
 			return None
 		elif token.value == ")":
 			if context.sub_status == "start_function":
 				self.process_end_function(context)
 			else:
 				return None
 		elif token.is_keyword or value_is_function(token.value):
 			set_status(context, token)
-
-		elif not token.is_keyword and not token.is_group and not token.is_whitespace and not token.value.startswith(
-				"anon"):
+		elif not token.is_keyword \
+				and not token.is_group \
+				and not token.is_whitespace \
+				and not token.value.startswith("anon"):
 			if token.value == ".":
 				context.status = "dot"
-			elif (context.sub_status == "IN" or context.sub_status == "THEN" or context.sub_status=="ELSE" or context.sub_status=="END") and context.status == "case":
+			elif (
+					context.sub_status == "IN"
+					or context.sub_status == "THEN"
+					or context.sub_status == "ELSE"
+					or context.sub_status == "END") \
+					and context.status == "case":
 				return None
 			elif token.value == "IN" and context.status == "case":
 				context.sub_status = "IN"
 			elif context.status == "from" or context.status == "join":
 				context.table.append(token.value)
 			elif context.status == "group_by":
 				context.group_by.append(token.value)
@@ -204,115 +218,133 @@
 				context.status = None
 			elif context.status == "case" and context.sub_status == "when":
 				if token.value.startswith("topic_"):
 					add_column_topic(context, token.value)
 				else:
 					add_column(context, token.value)
 			else:
-				if token.value.startswith("topic_") and not context.status == "where"  :
+				if token.value.startswith("topic_") and not context.status == "where":
 					add_column_topic(context, token.value)
 				else:
 					add_column(context, token.value)
 
+	# noinspection PyMethodMayBeStatic
 	def process_end_function(self, context):
 		context.sub_status = "end_function"
 		function_list = context.function
 		column = get_current_column(context)
 		column.function = function_list
 		context.function = []
 
+	# noinspection PyMethodMayBeStatic
 	def ignore_value(self, token):
-		return token.is_whitespace or token.value == "(" or token.value == "." or token.value == "," or token.value == ";" or token.value == "##"
-
+		return token.is_whitespace \
+			or token.value == "(" \
+			or token.value == "." \
+			or token.value == "," \
+			or token.value == ";" \
+			or token.value == "##"
 
-class IdentifierVister:
 
+class IdentifierVisitor:
+	# noinspection PyMethodMayBeStatic
 	def support(self, ast):
 		return isinstance(ast, Identifier)
 
+	# noinspection PyMethodMayBeStatic
 	def process(self, token: Identifier, context, visitor_list, previous_token: Token = None, next_token: Token = None):
 		if token.is_group:
 			for sub_token in token.tokens:
 				visitor = find_visitor(visitor_list, sub_token)
 				if visitor:
 					visitor.process(sub_token, context, visitor_list, previous_token, next_token)
 
 
-class ParenthesisVister:
+class ParenthesisVisitor:
+	# noinspection PyMethodMayBeStatic
 	def support(self, ast):
 		return isinstance(ast, Parenthesis)
 
-	def process(self, token: Parenthesis, context, visitor_list, previous_token: Token = None,
-	            next_token: Token = None):
+	# noinspection PyMethodMayBeStatic
+	def process(
+			self, token: Parenthesis, context, visitor_list, previous_token: Token = None,
+			next_token: Token = None):
 		if context.sub_status == "function":
 			context.sub_status = "start_function"
-		if (context.sub_status == "IN" or context.sub_status=="THEN")and context.status=="case" :
+		if (context.sub_status == "IN" or context.sub_status == "THEN") and context.status == "case":
 			return None
 		if token.M_OPEN and token.M_CLOSE:
 			for sub_token in token.tokens:
 				visitor = find_visitor(visitor_list, sub_token)
 				if visitor:
 					visitor.process(sub_token, context, visitor_list, previous_token, next_token)
 
 
-class FunctionVister:
-
+class FunctionVisitor:
+	# noinspection PyMethodMayBeStatic
 	def support(self, ast):
 		return isinstance(ast, Function)
 
+	# noinspection PyMethodMayBeStatic
 	def process(self, token: Function, context, visitor_list, previous_token: Token = None, next_token: Token = None):
 		# if context.status == "select":
 		context.sub_status = "function"
 		if token.is_group:
 			for sub_token in token.tokens:
 				visitor = find_visitor(visitor_list, sub_token)
 				if visitor:
 					visitor.process(sub_token, context, visitor_list, previous_token, next_token)
 
 
-class IdentifierListVister:
-
+class IdentifierListVisitor:
+	# noinspection PyMethodMayBeStatic
 	def support(self, ast):
 		return isinstance(ast, IdentifierList)
 
-	def process(self, token: IdentifierList, context, visitor_list, previous_token: Token = None,
-	            next_token: Token = None):
+	# noinspection PyMethodMayBeStatic
+	def process(
+			self, token: IdentifierList, context, visitor_list, previous_token: Token = None,
+			next_token: Token = None):
 		if token.is_group:
 			for sub_token in token.tokens:
 				visitor = find_visitor(visitor_list, sub_token)
 				if visitor:
 					visitor.process(sub_token, context, visitor_list, previous_token, next_token)
 
 
-class WhereVister:
-
+class WhereVisitor:
+	# noinspection PyMethodMayBeStatic
 	def support(self, ast):
 		return isinstance(ast, Where)
 
-	def process(self, token: IdentifierList, context, visitor_list, previous_token: Token = None,
-	            next_token: Token = None):
+	# noinspection PyMethodMayBeStatic
+	def process(
+			self, token: IdentifierList, context, visitor_list, previous_token: Token = None,
+			next_token: Token = None):
 		context.status = "where"
 		if token.is_group:
 			for sub_token in token.tokens:
 				visitor = find_visitor(visitor_list, sub_token)
 				if visitor:
 					visitor.process(sub_token, context, visitor_list, previous_token, next_token)
 
 
 class ComparisonVisitor:
+	# noinspection PyMethodMayBeStatic
 	def support(self, ast):
 		return isinstance(ast, Comparison)
 
-	def process(self, token: Comparison, context:SqlContext, visitor_list, previous_token: Token = None,
-	            next_token: Token = None):
+	# noinspection PyMethodMayBeStatic, PyUnusedLocal
+	def process(
+			self, token: Comparison, context: SqlContext, visitor_list, previous_token: Token = None,
+			next_token: Token = None):
 		if context.status == "case" and context.sub_status == "WHEN":
 			left_table, left = token.left.normalized.split(".")
 			add_column_topic(context, left_table)
 			add_column(context, left)
-
 		elif context.status == "where":
 			if "." in token.left.normalized:
 				left_table, left = token.left.normalized.split(".")
 				operator = find_operator(token)
 				value = token.right.value
 				context.where.append(WhereColumn(table=left_table, name=left, operator=operator, value=value))
 
@@ -322,20 +354,21 @@
 			right_table, right = token.right.normalized.split(".")
 			operator = find_operator(token)
 			context.joins.append(
 				JoinColumn(leftTable=left_table, left=left, rightTable=right_table, right=right, operator=operator))
 
 
 class CaseVisitor:
+	# noinspection PyMethodMayBeStatic
 	def support(self, ast):
 		return isinstance(ast, Case)
 
-	def process(self, token: Case, context, visitor_list, previous_token: Token = None,
-	            next_token: Token = None):
+	# noinspection PyMethodMayBeStatic
+	def process(
+			self, token: Case, context, visitor_list, previous_token: Token = None,
+			next_token: Token = None):
 		context.status = "case"
 		if token.is_group:
 			for sub_token in token.tokens:
-
-
 				visitor = find_visitor(visitor_list, sub_token)
 				if visitor:
-					visitor.process(sub_token, context, visitor_list, previous_token, next_token)
+					visitor.process(sub_token, context, visitor_list, previous_token, next_token)
```

### Comparing `watchmen_storage-16.5.4/src/watchmen_storage/sql_analysis/parse_sql.py` & `watchmen_storage-16.5.5/src/watchmen_storage/sql_analysis/parse_sql.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,46 @@
 import sqlparse
 
-from watchmen_storage.sql_analysis.ast_vister import IdentifierListVister, FunctionVister, IdentifierVister, \
-	ParenthesisVister, ComparisonVisitor, WhereVister, CaseVisitor, TokenVister, SqlContext, SqlColumn, QueryPerformance
+from watchmen_storage.sql_analysis.ast_vister import CaseVisitor, ComparisonVisitor, FunctionVisitor, \
+	IdentifierListVisitor, IdentifierVisitor, ParenthesisVisitor, QueryPerformance, SqlColumn, SqlContext, TokenVisitor, \
+	WhereVisitor
 
 
 class SqlParser:
-
 	def __init__(self):
-		self.visiters = [IdentifierListVister(), FunctionVister(), IdentifierVister(), ParenthesisVister(),
-		                 ComparisonVisitor(), WhereVister(), CaseVisitor(), TokenVister()]
+		self.visitors = [
+			IdentifierListVisitor(), FunctionVisitor(), IdentifierVisitor(), ParenthesisVisitor(),
+			ComparisonVisitor(), WhereVisitor(), CaseVisitor(), TokenVisitor()
+		]
 
 	def find_visitor(self, ast):
-		for v in self.visiters:
+		for v in self.visitors:
 			if v.support(ast):
 				return v
 
 	def start(self):
 		pass
 
 	def parse(self, sql: str) -> QueryPerformance:
 		context = SqlContext()
 		statements = sqlparse.split(sql)
 		for statement in statements:
 			tokens = sqlparse.parse(statement)[0].tokens
 			for index, token in enumerate(tokens):
 				visitor = self.find_visitor(token)
 				if visitor:
-					previous = self.get_previous(index, tokens)
-					next = self.get_next(index, tokens)
-					visitor.process(token, context, self.visiters, previous, next)
-
-		return self.process_context_result(context)
+					previous_one = self.get_previous(index, tokens)
+					next_one = self.get_next(index, tokens)
+					visitor.process(token, context, self.visitors, previous_one, next_one)
+
+		qp = self.process_context_result(context)
+		qp.sql = sql
+		return qp
 
+	# noinspection PyMethodMayBeStatic
 	def remove_duplicate(self, current_column_list):
 		result = []
 		last_name = None
 		for column in current_column_list:
 			if last_name != column.name:
 				result.append(column)
 				last_name = column.name
@@ -44,14 +49,15 @@
 	def process_context_result(self, context: SqlContext):
 		query_performance = QueryPerformance()
 		column_dimensions = self.build_column_dimension(context)
 		query_performance.column_dimensions = column_dimensions
 		query_performance.topic_dimensions = self.build_table_dimension(context)
 		return query_performance
 
+	# noinspection PyMethodMayBeStatic
 	def build_table_dimension(self, context: SqlContext):
 		tables = context.table
 		tables_value = ""
 		for table in tables:
 			if tables_value == "":
 				tables_value = table
 			else:
@@ -59,27 +65,30 @@
 		return tables_value
 
 	def build_column_dimension(self, context: SqlContext):
 		column_dict = context.columns
 		level = context.level
 		current_column_list = column_dict["level_" + str(level)]
 		dimension_value = ""
-		sort_current_column_list = self.remove_duplicate(sorted(current_column_list, key=lambda column: column.name))
+		sort_current_column_list = self.remove_duplicate(
+			sorted(current_column_list, key=lambda a_column: a_column.name))
 		for column in sort_current_column_list:
 			column: SqlColumn = column
-			if dimension_value =="":
+			if dimension_value == "":
 				dimension_value = column.name
 			else:
-				dimension_value = dimension_value + "_"+ column.name
+				dimension_value = dimension_value + "_" + column.name
 		return dimension_value
 
+	# noinspection PyMethodMayBeStatic
 	def get_previous(self, index, tokens):
 		if index > 0:
 			return tokens[index - 1]
 		else:
 			return None
 
+	# noinspection PyMethodMayBeStatic
 	def get_next(self, index, tokens):
 		if index < len(tokens) - 1:
 			return tokens[index + 1]
 		else:
 			return None
```

### Comparing `watchmen_storage-16.5.4/src/watchmen_storage/sql_analysis/query_performance_service.py` & `watchmen_storage-16.5.5/src/watchmen_storage/sql_analysis/query_performance_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.4/src/watchmen_storage/sql_analysis/topic_generator.py` & `watchmen_storage-16.5.5/src/watchmen_storage/sql_analysis/topic_generator.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.4/src/watchmen_storage/storage_based_worker_id_generator.py` & `watchmen_storage-16.5.5/src/watchmen_storage/storage_based_worker_id_generator.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.4/src/watchmen_storage/storage_exception.py` & `watchmen_storage-16.5.5/src/watchmen_storage/storage_exception.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.4/src/watchmen_storage/storage_spi.py` & `watchmen_storage-16.5.5/src/watchmen_storage/storage_spi.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.4/src/watchmen_storage/storage_types.py` & `watchmen_storage-16.5.5/src/watchmen_storage/storage_types.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.4/src/watchmen_storage/topic_utils.py` & `watchmen_storage-16.5.5/src/watchmen_storage/topic_utils.py`

 * *Files identical despite different names*

