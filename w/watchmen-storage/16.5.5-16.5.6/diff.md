# Comparing `tmp/watchmen_storage-16.5.5.tar.gz` & `tmp/watchmen_storage-16.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_storage-16.5.5.tar", max compression
+gzip compressed data, was "watchmen_storage-16.5.6.tar", max compression
```

## Comparing `watchmen_storage-16.5.5.tar` & `watchmen_storage-16.5.6.tar`

### file list

```diff
@@ -1,22 +1,21 @@
--rw-r--r--   0        0        0     1061 2023-06-06 07:52:17.125012 watchmen_storage-16.5.5/LICENSE
--rw-r--r--   0        0        0      443 2023-06-06 07:52:17.125012 watchmen_storage-16.5.5/pyproject.toml
--rw-r--r--   0        0        0     2217 2023-06-06 07:52:17.125012 watchmen_storage-16.5.5/src/watchmen_storage/__init__.py
--rw-r--r--   0        0        0     4917 2023-06-06 07:52:17.125012 watchmen_storage-16.5.5/src/watchmen_storage/competitive_worker_id_generator.py
--rw-r--r--   0        0        0     5549 2023-06-06 07:52:17.125012 watchmen_storage-16.5.5/src/watchmen_storage/data_source_helper.py
--rw-r--r--   0        0        0     1825 2023-06-06 07:52:17.125012 watchmen_storage-16.5.5/src/watchmen_storage/free_storage_types.py
--rw-r--r--   0        0        0      211 2023-06-06 07:52:17.125012 watchmen_storage-16.5.5/src/watchmen_storage/secrets_manager.py
--rw-r--r--   0        0        0      730 2023-06-06 07:52:17.125012 watchmen_storage-16.5.5/src/watchmen_storage/secrets_manager_aws.py
--rw-r--r--   0        0        0     1096 2023-06-06 07:52:17.125012 watchmen_storage-16.5.5/src/watchmen_storage/settings.py
--rw-r--r--   0        0        0     2750 2023-06-06 07:52:17.125012 watchmen_storage-16.5.5/src/watchmen_storage/snowflake.py
--rw-r--r--   0        0        0      232 2023-06-06 07:52:17.125012 watchmen_storage-16.5.5/src/watchmen_storage/snowflake_worker_id_generator.py
--rw-r--r--   0        0        0        0 2023-06-06 07:52:17.125012 watchmen_storage-16.5.5/src/watchmen_storage/sql_analysis/__init__.py
--rw-r--r--   0        0        0    10961 2023-06-06 07:52:17.125012 watchmen_storage-16.5.5/src/watchmen_storage/sql_analysis/ast_vister.py
--rw-r--r--   0        0        0     2832 2023-06-06 07:52:17.125012 watchmen_storage-16.5.5/src/watchmen_storage/sql_analysis/parse_sql.py
--rw-r--r--   0        0        0      890 2023-06-06 07:52:17.125012 watchmen_storage-16.5.5/src/watchmen_storage/sql_analysis/query_performance_service.py
--rw-r--r--   0        0        0     1441 2023-06-06 07:52:17.125012 watchmen_storage-16.5.5/src/watchmen_storage/sql_analysis/topic_generator.py
--rw-r--r--   0        0        0     7259 2023-06-06 07:52:17.125012 watchmen_storage-16.5.5/src/watchmen_storage/storage_based_worker_id_generator.py
--rw-r--r--   0        0        0      721 2023-06-06 07:52:17.125012 watchmen_storage-16.5.5/src/watchmen_storage/storage_exception.py
--rw-r--r--   0        0        0     5998 2023-06-06 07:52:17.125012 watchmen_storage-16.5.5/src/watchmen_storage/storage_spi.py
--rw-r--r--   0        0        0     4717 2023-06-06 07:52:17.125012 watchmen_storage-16.5.5/src/watchmen_storage/storage_types.py
--rw-r--r--   0        0        0      630 2023-06-06 07:52:17.125012 watchmen_storage-16.5.5/src/watchmen_storage/topic_utils.py
--rw-r--r--   0        0        0      521 1970-01-01 00:00:00.000000 watchmen_storage-16.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-06 17:50:48.823399 watchmen_storage-16.5.6/LICENSE
+-rw-r--r--   0        0        0      442 2023-06-06 17:50:48.827399 watchmen_storage-16.5.6/pyproject.toml
+-rw-r--r--   0        0        0     2261 2023-06-06 17:50:48.827399 watchmen_storage-16.5.6/src/watchmen_storage/__init__.py
+-rw-r--r--   0        0        0     4917 2023-06-06 17:50:48.827399 watchmen_storage-16.5.6/src/watchmen_storage/competitive_worker_id_generator.py
+-rw-r--r--   0        0        0     5549 2023-06-06 17:50:48.827399 watchmen_storage-16.5.6/src/watchmen_storage/data_source_helper.py
+-rw-r--r--   0        0        0     1853 2023-06-06 17:50:48.827399 watchmen_storage-16.5.6/src/watchmen_storage/free_storage_types.py
+-rw-r--r--   0        0        0      211 2023-06-06 17:50:48.827399 watchmen_storage-16.5.6/src/watchmen_storage/secrets_manager.py
+-rw-r--r--   0        0        0      730 2023-06-06 17:50:48.827399 watchmen_storage-16.5.6/src/watchmen_storage/secrets_manager_aws.py
+-rw-r--r--   0        0        0     1096 2023-06-06 17:50:48.827399 watchmen_storage-16.5.6/src/watchmen_storage/settings.py
+-rw-r--r--   0        0        0     2750 2023-06-06 17:50:48.827399 watchmen_storage-16.5.6/src/watchmen_storage/snowflake.py
+-rw-r--r--   0        0        0      232 2023-06-06 17:50:48.827399 watchmen_storage-16.5.6/src/watchmen_storage/snowflake_worker_id_generator.py
+-rw-r--r--   0        0        0       43 2023-06-06 17:50:48.827399 watchmen_storage-16.5.6/src/watchmen_storage/sql_analysis/__init__.py
+-rw-r--r--   0        0        0    10961 2023-06-06 17:50:48.827399 watchmen_storage-16.5.6/src/watchmen_storage/sql_analysis/ast_visitor.py
+-rw-r--r--   0        0        0     2833 2023-06-06 17:50:48.827399 watchmen_storage-16.5.6/src/watchmen_storage/sql_analysis/parse_sql.py
+-rw-r--r--   0        0        0     1441 2023-06-06 17:50:48.827399 watchmen_storage-16.5.6/src/watchmen_storage/sql_analysis/topic_generator.py
+-rw-r--r--   0        0        0     7259 2023-06-06 17:50:48.827399 watchmen_storage-16.5.6/src/watchmen_storage/storage_based_worker_id_generator.py
+-rw-r--r--   0        0        0      721 2023-06-06 17:50:48.827399 watchmen_storage-16.5.6/src/watchmen_storage/storage_exception.py
+-rw-r--r--   0        0        0     5998 2023-06-06 17:50:48.827399 watchmen_storage-16.5.6/src/watchmen_storage/storage_spi.py
+-rw-r--r--   0        0        0     4717 2023-06-06 17:50:48.827399 watchmen_storage-16.5.6/src/watchmen_storage/storage_types.py
+-rw-r--r--   0        0        0      630 2023-06-06 17:50:48.827399 watchmen_storage-16.5.6/src/watchmen_storage/topic_utils.py
+-rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 watchmen_storage-16.5.6/PKG-INFO
```

### Comparing `watchmen_storage-16.5.5/LICENSE` & `watchmen_storage-16.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.5/src/watchmen_storage/__init__.py` & `watchmen_storage-16.5.6/src/watchmen_storage/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from .competitive_worker_id_generator import competitive_worker_id, CompetitiveWorker, CompetitiveWorkerIdGenerator, \
 	CompetitiveWorkerRestarter, CompetitiveWorkerShutdownListener, CompetitiveWorkerShutdownSignal, get_host_ip, \
 	WorkerCreationException, WorkerDeclarationException, WorkerFirstDeclarationException
-from .data_source_helper import DataSourceHelper, ask_datasource_name
+from .data_source_helper import ask_datasource_name, DataSourceHelper
 from .free_storage_types import FreeAggregateArithmetic, FreeAggregateColumn, FreeAggregatePager, FreeAggregator, \
 	FreeColumn, FreeFinder, FreeJoin, FreeJoinType, FreePager
 from .settings import ask_decimal_fraction_digits, ask_decimal_integral_digits, ask_disable_compiled_cache, \
 	ask_object_storage_need_date_directory, ask_store_json_in_clob
 from .snowflake import InvalidSystemClockException, SnowflakeGenerator
 from .snowflake_worker_id_generator import immutable_worker_id, WorkerIdGenerator
+# from .sql_analysis import QueryPerformance
 from .storage_based_worker_id_generator import COMPETITIVE_WORKER_SHAPER, CompetitiveWorkerShaper, \
 	SNOWFLAKE_WORKER_ID_TABLE, StorageBasedWorkerIdGenerator
 from .storage_exception import EntityNotFoundException, InsertConflictException, NoCriteriaForUpdateException, \
 	NoFreeJoinException, OptimisticLockException, TooManyEntitiesFoundException, UnexpectedStorageException, \
 	UnsupportedComputationException, UnsupportedCriteriaException, UnsupportedSortMethodException, \
 	UnsupportedStraightColumnException
 from .storage_spi import StorageSPI, TopicDataStorageSPI, TransactionalStorageSPI
@@ -19,8 +20,7 @@
 	EntityColumnAggregateArithmetic, EntityColumnName, EntityColumnValue, EntityCriteria, EntityCriteriaExpression, \
 	EntityCriteriaJoint, EntityCriteriaJointConjunction, EntityCriteriaOperator, EntityCriteriaStatement, \
 	EntityDeleter, EntityDistinctValuesFinder, EntityFinder, EntityHelper, EntityId, EntityIdHelper, EntityList, \
 	EntityName, EntityPager, EntityRow, EntityShaper, EntitySort, EntitySortColumn, EntitySortMethod, \
 	EntityStraightAggregateColumn, EntityStraightColumn, EntityStraightValuesFinder, EntityUpdate, EntityUpdater, \
 	Literal, EntityColumnType, EntityLimitedFinder
 from .topic_utils import as_table_name
-
```

### Comparing `watchmen_storage-16.5.5/src/watchmen_storage/competitive_worker_id_generator.py` & `watchmen_storage-16.5.6/src/watchmen_storage/competitive_worker_id_generator.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.5/src/watchmen_storage/data_source_helper.py` & `watchmen_storage-16.5.6/src/watchmen_storage/data_source_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.5/src/watchmen_storage/free_storage_types.py` & `watchmen_storage-16.5.6/src/watchmen_storage/free_storage_types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from enum import Enum
 from typing import Callable, List, Optional
 
 from watchmen_model.common import DataModel, Pageable
-from .sql_analysis.ast_vister import QueryPerformance
+from .sql_analysis.ast_visitor import QueryPerformance
 from .storage_types import ColumnNameLiteral, EntityCriteria, EntitySortColumn, Literal
 
 
 class FreeAggregateArithmetic(str, Enum):
 	NONE = 'none'
 	DISTINCT_COUNT = 'distinct_count'
 	COUNT = 'count'
@@ -35,14 +35,15 @@
 	type: Optional[FreeJoinType] = None
 
 
 class FreeFinder(DataModel):
 	columns: List[FreeColumn] = None
 	joins: List[FreeJoin] = None
 	criteria: Optional[EntityCriteria] = None
+	commandOnly: bool = False
 	queryPfmMonitor: Optional[Callable[[QueryPerformance, bool], None]] = None
 
 
 class FreeAggregateColumn(DataModel):
 	name: str  # name must match free column's index, such as column_1, column_2 (starts from 1)
 	arithmetic: Optional[FreeAggregateArithmetic] = None
 	alias: Optional[str] = None
```

### Comparing `watchmen_storage-16.5.5/src/watchmen_storage/secrets_manager_aws.py` & `watchmen_storage-16.5.6/src/watchmen_storage/secrets_manager_aws.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.5/src/watchmen_storage/settings.py` & `watchmen_storage-16.5.6/src/watchmen_storage/settings.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.5/src/watchmen_storage/snowflake.py` & `watchmen_storage-16.5.6/src/watchmen_storage/snowflake.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.5/src/watchmen_storage/sql_analysis/ast_vister.py` & `watchmen_storage-16.5.6/src/watchmen_storage/sql_analysis/ast_visitor.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.5/src/watchmen_storage/sql_analysis/parse_sql.py` & `watchmen_storage-16.5.6/src/watchmen_storage/sql_analysis/parse_sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sqlparse
 
-from watchmen_storage.sql_analysis.ast_vister import CaseVisitor, ComparisonVisitor, FunctionVisitor, \
+from watchmen_storage.sql_analysis.ast_visitor import CaseVisitor, ComparisonVisitor, FunctionVisitor, \
 	IdentifierListVisitor, IdentifierVisitor, ParenthesisVisitor, QueryPerformance, SqlColumn, SqlContext, TokenVisitor, \
 	WhereVisitor
 
 
 class SqlParser:
 	def __init__(self):
 		self.visitors = [
```

### Comparing `watchmen_storage-16.5.5/src/watchmen_storage/sql_analysis/topic_generator.py` & `watchmen_storage-16.5.6/src/watchmen_storage/sql_analysis/topic_generator.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.5/src/watchmen_storage/storage_based_worker_id_generator.py` & `watchmen_storage-16.5.6/src/watchmen_storage/storage_based_worker_id_generator.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.5/src/watchmen_storage/storage_exception.py` & `watchmen_storage-16.5.6/src/watchmen_storage/storage_exception.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.5/src/watchmen_storage/storage_spi.py` & `watchmen_storage-16.5.6/src/watchmen_storage/storage_spi.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.5/src/watchmen_storage/storage_types.py` & `watchmen_storage-16.5.6/src/watchmen_storage/storage_types.py`

 * *Files identical despite different names*

### Comparing `watchmen_storage-16.5.5/src/watchmen_storage/topic_utils.py` & `watchmen_storage-16.5.6/src/watchmen_storage/topic_utils.py`

 * *Files identical despite different names*

