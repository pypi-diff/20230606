# Comparing `tmp/watchmen_pipeline_kernel-16.5.3.tar.gz` & `tmp/watchmen_pipeline_kernel-16.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_pipeline_kernel-16.5.3.tar", max compression
+gzip compressed data, was "watchmen_pipeline_kernel-16.5.4.tar", max compression
```

## Comparing `watchmen_pipeline_kernel-16.5.3.tar` & `watchmen_pipeline_kernel-16.5.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1061 2023-06-05 01:29:03.528123 watchmen_pipeline_kernel-16.5.3/LICENSE
--rw-r--r--   0        0        0     1165 2023-06-05 01:29:03.528123 watchmen_pipeline_kernel-16.5.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-05 01:29:03.528123 watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/__init__.py
--rw-r--r--   0        0        0       75 2023-06-05 01:29:03.528123 watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/boot/__init__.py
--rw-r--r--   0        0        0      643 2023-06-05 01:29:03.528123 watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/boot/boot.py
--rw-r--r--   0        0        0       40 2023-06-05 01:29:03.528123 watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/cache/__init__.py
--rw-r--r--   0        0        0      203 2023-06-05 01:29:03.528123 watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/cache/cache_service.py
--rw-r--r--   0        0        0     1626 2023-06-05 01:29:03.528123 watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/cache/compiled_pipeline_cache.py
--rw-r--r--   0        0        0      488 2023-06-05 01:29:03.528123 watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/common/__init__.py
--rw-r--r--   0        0        0       48 2023-06-05 01:29:03.528123 watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/common/exception.py
--rw-r--r--   0        0        0     2797 2023-06-05 01:29:03.528123 watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/common/settings.py
--rw-r--r--   0        0        0      335 2023-06-05 01:29:03.528123 watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/external_writer/__init__.py
--rw-r--r--   0        0        0      617 2023-06-05 01:29:03.528123 watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/external_writer/elastic_search_writer.py
--rw-r--r--   0        0        0      763 2023-06-05 01:29:03.528123 watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/external_writer/prebuilt_writers.py
--rw-r--r--   0        0        0     1895 2023-06-05 01:29:03.528123 watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/external_writer/standard_writer.py
--rw-r--r--   0        0        0       68 2023-06-05 01:29:03.528123 watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/monitor_log/__init__.py
--rw-r--r--   0        0        0     4938 2023-06-05 01:29:03.528123 watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/monitor_log/monitor_log_data_service.py
--rw-r--r--   0        0        0      200 2023-06-05 01:29:03.528123 watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/pipeline/__init__.py
--rw-r--r--   0        0        0     2094 2023-06-05 01:29:03.528123 watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/pipeline/monitor_log_invoker.py
--rw-r--r--   0        0        0     3124 2023-06-05 01:29:03.528123 watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/pipeline/pipeline_invoker.py
--rw-r--r--   0        0        0     6391 2023-06-05 01:29:03.528123 watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/pipeline/pipeline_trigger.py
--rw-r--r--   0        0        0     1261 2023-06-05 01:29:03.528123 watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/pipeline/pipelines_dispatcher.py
--rw-r--r--   0        0        0     1869 2023-06-05 01:29:03.532124 watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/pipeline/sql_performance_invoker.py
--rw-r--r--   0        0        0       53 2023-06-05 01:29:03.532124 watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/pipeline_schema/__init__.py
--rw-r--r--   0        0        0    40015 2023-06-05 01:29:03.532124 watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/pipeline_schema/compiled_action.py
--rw-r--r--   0        0        0     7260 2023-06-05 01:29:03.532124 watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/pipeline_schema/compiled_pipeline.py
--rw-r--r--   0        0        0     3967 2023-06-05 01:29:03.532124 watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/pipeline_schema/compiled_single_unit.py
--rw-r--r--   0        0        0     3395 2023-06-05 01:29:03.532124 watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/pipeline_schema/compiled_stage.py
--rw-r--r--   0        0        0     4440 2023-06-05 01:29:03.532124 watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/pipeline_schema/compiled_unit.py
--rw-r--r--   0        0        0     7884 2023-06-05 01:29:03.532124 watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/pipeline_schema/distributed_compiled_unit.py
--rw-r--r--   0        0        0     2206 2023-06-05 01:29:03.532124 watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/pipeline_schema/pipeline_context.py
--rw-r--r--   0        0        0      191 2023-06-05 01:29:03.532124 watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/pipeline_schema_interface/__init__.py
--rw-r--r--   0        0        0      804 2023-06-05 01:29:03.532124 watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/pipeline_schema_interface/compiled_pipeline.py
--rw-r--r--   0        0        0      208 2023-06-05 01:29:03.532124 watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/pipeline_schema_interface/create_queue_pipeline.py
--rw-r--r--   0        0        0      428 2023-06-05 01:29:03.532124 watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/pipeline_schema_interface/pipeline_context.py
--rw-r--r--   0        0        0      292 2023-06-05 01:29:03.532124 watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/pipeline_schema_interface/topic_storages.py
--rw-r--r--   0        0        0       47 2023-06-05 01:29:03.532124 watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/topic/__init__.py
--rw-r--r--   0        0        0     1378 2023-06-05 01:29:03.532124 watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/topic/topic_helper.py
--rw-r--r--   0        0        0      412 2023-06-05 01:29:03.532124 watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/topic_snapshot/__init__.py
--rw-r--r--   0        0        0     5023 2023-06-05 01:29:03.532124 watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/topic_snapshot/scheduler_launcher.py
--rw-r--r--   0        0        0     1907 2023-06-05 01:29:03.532124 watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/topic_snapshot/scheduler_registrar.py
--rw-r--r--   0        0        0    13921 2023-06-05 01:29:03.532124 watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/topic_snapshot/scheduler_runner.py
--rw-r--r--   0        0        0     6352 2023-06-05 01:29:03.532124 watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/topic_snapshot/utils.py
--rw-r--r--   0        0        0     1247 1970-01-01 00:00:00.000000 watchmen_pipeline_kernel-16.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-06 01:45:59.137402 watchmen_pipeline_kernel-16.5.4/LICENSE
+-rw-r--r--   0        0        0     1165 2023-06-06 01:45:59.141403 watchmen_pipeline_kernel-16.5.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-06 01:45:59.141403 watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/__init__.py
+-rw-r--r--   0        0        0       75 2023-06-06 01:45:59.141403 watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/boot/__init__.py
+-rw-r--r--   0        0        0      643 2023-06-06 01:45:59.141403 watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/boot/boot.py
+-rw-r--r--   0        0        0       40 2023-06-06 01:45:59.141403 watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/cache/__init__.py
+-rw-r--r--   0        0        0      203 2023-06-06 01:45:59.141403 watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/cache/cache_service.py
+-rw-r--r--   0        0        0     1626 2023-06-06 01:45:59.141403 watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/cache/compiled_pipeline_cache.py
+-rw-r--r--   0        0        0      488 2023-06-06 01:45:59.141403 watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/common/__init__.py
+-rw-r--r--   0        0        0       48 2023-06-06 01:45:59.141403 watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/common/exception.py
+-rw-r--r--   0        0        0     2902 2023-06-06 01:45:59.141403 watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/common/settings.py
+-rw-r--r--   0        0        0      335 2023-06-06 01:45:59.141403 watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/external_writer/__init__.py
+-rw-r--r--   0        0        0      617 2023-06-06 01:45:59.141403 watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/external_writer/elastic_search_writer.py
+-rw-r--r--   0        0        0      763 2023-06-06 01:45:59.141403 watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/external_writer/prebuilt_writers.py
+-rw-r--r--   0        0        0     1895 2023-06-06 01:45:59.141403 watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/external_writer/standard_writer.py
+-rw-r--r--   0        0        0       68 2023-06-06 01:45:59.141403 watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/monitor_log/__init__.py
+-rw-r--r--   0        0        0     4938 2023-06-06 01:45:59.141403 watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/monitor_log/monitor_log_data_service.py
+-rw-r--r--   0        0        0      200 2023-06-06 01:45:59.141403 watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/pipeline/__init__.py
+-rw-r--r--   0        0        0     2094 2023-06-06 01:45:59.141403 watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/pipeline/monitor_log_invoker.py
+-rw-r--r--   0        0        0     3124 2023-06-06 01:45:59.141403 watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/pipeline/pipeline_invoker.py
+-rw-r--r--   0        0        0     6391 2023-06-06 01:45:59.141403 watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/pipeline/pipeline_trigger.py
+-rw-r--r--   0        0        0     1261 2023-06-06 01:45:59.141403 watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/pipeline/pipelines_dispatcher.py
+-rw-r--r--   0        0        0     2087 2023-06-06 01:45:59.141403 watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/pipeline/sql_performance_invoker.py
+-rw-r--r--   0        0        0       53 2023-06-06 01:45:59.141403 watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/pipeline_schema/__init__.py
+-rw-r--r--   0        0        0    40015 2023-06-06 01:45:59.141403 watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/pipeline_schema/compiled_action.py
+-rw-r--r--   0        0        0     7260 2023-06-06 01:45:59.141403 watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/pipeline_schema/compiled_pipeline.py
+-rw-r--r--   0        0        0     3967 2023-06-06 01:45:59.141403 watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/pipeline_schema/compiled_single_unit.py
+-rw-r--r--   0        0        0     3395 2023-06-06 01:45:59.141403 watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/pipeline_schema/compiled_stage.py
+-rw-r--r--   0        0        0     4440 2023-06-06 01:45:59.141403 watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/pipeline_schema/compiled_unit.py
+-rw-r--r--   0        0        0     7884 2023-06-06 01:45:59.141403 watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/pipeline_schema/distributed_compiled_unit.py
+-rw-r--r--   0        0        0     2206 2023-06-06 01:45:59.141403 watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/pipeline_schema/pipeline_context.py
+-rw-r--r--   0        0        0      191 2023-06-06 01:45:59.141403 watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/pipeline_schema_interface/__init__.py
+-rw-r--r--   0        0        0      804 2023-06-06 01:45:59.141403 watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/pipeline_schema_interface/compiled_pipeline.py
+-rw-r--r--   0        0        0      208 2023-06-06 01:45:59.141403 watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/pipeline_schema_interface/create_queue_pipeline.py
+-rw-r--r--   0        0        0      428 2023-06-06 01:45:59.141403 watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/pipeline_schema_interface/pipeline_context.py
+-rw-r--r--   0        0        0      292 2023-06-06 01:45:59.141403 watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/pipeline_schema_interface/topic_storages.py
+-rw-r--r--   0        0        0       47 2023-06-06 01:45:59.141403 watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/topic/__init__.py
+-rw-r--r--   0        0        0     1378 2023-06-06 01:45:59.141403 watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/topic/topic_helper.py
+-rw-r--r--   0        0        0      412 2023-06-06 01:45:59.141403 watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/topic_snapshot/__init__.py
+-rw-r--r--   0        0        0     5023 2023-06-06 01:45:59.141403 watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/topic_snapshot/scheduler_launcher.py
+-rw-r--r--   0        0        0     1907 2023-06-06 01:45:59.141403 watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/topic_snapshot/scheduler_registrar.py
+-rw-r--r--   0        0        0    13921 2023-06-06 01:45:59.141403 watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/topic_snapshot/scheduler_runner.py
+-rw-r--r--   0        0        0     6352 2023-06-06 01:45:59.141403 watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/topic_snapshot/utils.py
+-rw-r--r--   0        0        0     1247 1970-01-01 00:00:00.000000 watchmen_pipeline_kernel-16.5.4/PKG-INFO
```

### Comparing `watchmen_pipeline_kernel-16.5.3/LICENSE` & `watchmen_pipeline_kernel-16.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.5.3/pyproject.toml` & `watchmen_pipeline_kernel-16.5.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "watchmen-pipeline-kernel"
-version = "16.5.3"
+version = "16.5.4"
 description = ""
 authors = ["botlikes <75356972+botlikes456@users.noreply.github.com>"]
 license = "MIT"
 packages = [
     { include = "watchmen_pipeline_kernel", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 dask = "^2022.9.1"
 distributed = "^2022.9.1"
 APScheduler = "^3.9.1"
-watchmen-data-kernel = "16.5.3"
-watchmen-storage-mysql = { version = "16.5.3", optional = true }
-watchmen-storage-oracle = { version = "16.5.3", optional = true }
-watchmen-storage-mongodb = { version = "16.5.3", optional = true }
-watchmen-storage-mssql = { version = "16.5.3", optional = true }
-watchmen-storage-postgresql = { version = "16.5.3", optional = true }
+watchmen-data-kernel = "16.5.4"
+watchmen-storage-mysql = { version = "16.5.4", optional = true }
+watchmen-storage-oracle = { version = "16.5.4", optional = true }
+watchmen-storage-mongodb = { version = "16.5.4", optional = true }
+watchmen-storage-mssql = { version = "16.5.4", optional = true }
+watchmen-storage-postgresql = { version = "16.5.4", optional = true }
 requests = { version = "^2.27.1", optional = true }
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.extras]
 mysql = ["watchmen-storage-mysql"]
 oracle = ["watchmen-storage-oracle"]
```

### Comparing `watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/boot/boot.py` & `watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/boot/boot.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/cache/compiled_pipeline_cache.py` & `watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/cache/compiled_pipeline_cache.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/common/settings.py` & `watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/common/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 	PIPELINE_STANDARD_EXTERNAL_WRITER: bool = True
 	PIPELINE_ELASTIC_SEARCH_EXTERNAL_WRITER: bool = False
 	PIPELINE_UPDATE_RETRY: bool = True  # enable pipeline update retry if it is failed on optimistic lock
 	PIPELINE_UPDATE_RETRY_TIMES: int = 3  # optimistic lock retry times
 	PIPELINE_UPDATE_RETRY_INTERVAL: int = 10  # retry interval in milliseconds
 	PIPELINE_UPDATE_RETRY_FORCE: bool = True  # enable force retry after all retries failed
 	PIPELINE_ASYNC_HANDLE_MONITOR_LOG: bool = True  # handle monitor log (might with pipelines) asynchronized
+	QUERY_MONITOR_LOG:bool = False
 
 	class Config:
 		# secrets_dir = '/var/run'
 		env_file = '.env'
 		env_file_encoding = 'utf-8'
 		case_sensitive = True
 
@@ -85,7 +86,11 @@
 
 def ask_pipeline_update_retry_force() -> bool:
 	return settings.PIPELINE_UPDATE_RETRY_FORCE
 
 
 def ask_async_handle_monitor_log() -> bool:
 	return settings.PIPELINE_ASYNC_HANDLE_MONITOR_LOG
+
+
+def ask_query_monitor_log()->bool  :
+	return settings.QUERY_MONITOR_LOG
```

### Comparing `watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/external_writer/elastic_search_writer.py` & `watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/external_writer/elastic_search_writer.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/external_writer/prebuilt_writers.py` & `watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/external_writer/prebuilt_writers.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/external_writer/standard_writer.py` & `watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/external_writer/standard_writer.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/monitor_log/monitor_log_data_service.py` & `watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/monitor_log/monitor_log_data_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/pipeline/monitor_log_invoker.py` & `watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/pipeline/monitor_log_invoker.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/pipeline/pipeline_invoker.py` & `watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/pipeline/pipeline_invoker.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/pipeline/pipeline_trigger.py` & `watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/pipeline/pipeline_trigger.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/pipeline/pipelines_dispatcher.py` & `watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/pipeline/pipelines_dispatcher.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/pipeline/sql_performance_invoker.py` & `watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/pipeline/sql_performance_invoker.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from watchmen_data_kernel.topic_schema import TopicSchema
 from watchmen_model.admin import PipelineTriggerType
 from watchmen_model.pipeline_kernel import PipelineTriggerTraceId
 from watchmen_pipeline_kernel.common import PipelineKernelException
 from watchmen_storage.sql_analysis.ast_vister import QueryPerformance
 from . import create_monitor_log_pipeline_invoker
 from .pipeline_trigger import PipelineTrigger
+from ..common.settings import ask_query_monitor_log
 
 logger = getLogger(__name__)
 
 def get_topic_service(principal_service: PrincipalService) -> TopicService:
 	return TopicService(principal_service)
 
 
@@ -41,8 +42,14 @@
 			asynchronized=asynchronized,
 			handle_monitor_log=create_monitor_log_pipeline_invoker(trace_id, principal_service)
 		)
 
 		asyncio.create_task(trigger.invoke())
 
 
-	return handle_sql_performance_log
+	def ignore_performance_log(sql_performance_log: QueryPerformance, asynchronized: bool):
+		pass
+
+	if ask_query_monitor_log():
+		return handle_sql_performance_log
+	else:
+		return ignore_performance_log
```

### Comparing `watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/pipeline_schema/compiled_action.py` & `watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/pipeline_schema/compiled_action.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/pipeline_schema/compiled_pipeline.py` & `watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/pipeline_schema/compiled_pipeline.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/pipeline_schema/compiled_single_unit.py` & `watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/pipeline_schema/compiled_single_unit.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/pipeline_schema/compiled_stage.py` & `watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/pipeline_schema/compiled_stage.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/pipeline_schema/compiled_unit.py` & `watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/pipeline_schema/compiled_unit.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/pipeline_schema/distributed_compiled_unit.py` & `watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/pipeline_schema/distributed_compiled_unit.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/pipeline_schema/pipeline_context.py` & `watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/pipeline_schema/pipeline_context.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/pipeline_schema_interface/compiled_pipeline.py` & `watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/pipeline_schema_interface/compiled_pipeline.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/topic/topic_helper.py` & `watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/topic/topic_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/topic_snapshot/scheduler_launcher.py` & `watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/topic_snapshot/scheduler_launcher.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/topic_snapshot/scheduler_registrar.py` & `watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/topic_snapshot/scheduler_registrar.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/topic_snapshot/scheduler_runner.py` & `watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/topic_snapshot/scheduler_runner.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.5.3/src/watchmen_pipeline_kernel/topic_snapshot/utils.py` & `watchmen_pipeline_kernel-16.5.4/src/watchmen_pipeline_kernel/topic_snapshot/utils.py`

 * *Files identical despite different names*

### Comparing `watchmen_pipeline_kernel-16.5.3/PKG-INFO` & `watchmen_pipeline_kernel-16.5.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchmen-pipeline-kernel
-Version: 16.5.3
+Version: 16.5.4
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,13 +18,13 @@
 Provides-Extra: oracle
 Provides-Extra: postgresql
 Provides-Extra: standard-ext-writer
 Requires-Dist: APScheduler (>=3.9.1,<4.0.0)
 Requires-Dist: dask (>=2022.9.1,<2023.0.0)
 Requires-Dist: distributed (>=2022.9.1,<2023.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0) ; extra == "standard-ext-writer"
-Requires-Dist: watchmen-data-kernel (==16.5.3)
-Requires-Dist: watchmen-storage-mongodb (==16.5.3) ; extra == "mongodb"
-Requires-Dist: watchmen-storage-mssql (==16.5.3) ; extra == "mssql"
-Requires-Dist: watchmen-storage-mysql (==16.5.3) ; extra == "mysql"
-Requires-Dist: watchmen-storage-oracle (==16.5.3) ; extra == "oracle"
-Requires-Dist: watchmen-storage-postgresql (==16.5.3) ; extra == "postgresql"
+Requires-Dist: watchmen-data-kernel (==16.5.4)
+Requires-Dist: watchmen-storage-mongodb (==16.5.4) ; extra == "mongodb"
+Requires-Dist: watchmen-storage-mssql (==16.5.4) ; extra == "mssql"
+Requires-Dist: watchmen-storage-mysql (==16.5.4) ; extra == "mysql"
+Requires-Dist: watchmen-storage-oracle (==16.5.4) ; extra == "oracle"
+Requires-Dist: watchmen-storage-postgresql (==16.5.4) ; extra == "postgresql"
```

