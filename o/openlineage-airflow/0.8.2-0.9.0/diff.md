# Comparing `tmp/openlineage-airflow-0.8.2.tar.gz` & `tmp/openlineage-airflow-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/openlineage-airflow-0.8.2.tar", last modified: Thu May 19 20:00:16 2022, max compression
+gzip compressed data, was "dist/openlineage-airflow-0.9.0.tar", last modified: Fri Jun  3 23:03:16 2022, max compression
```

## Comparing `openlineage-airflow-0.8.2.tar` & `openlineage-airflow-0.9.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-05-19 20:00:16.000000 openlineage-airflow-0.8.2/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11740 2022-05-19 20:00:16.000000 openlineage-airflow-0.8.2/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9352 2022-05-19 20:00:10.000000 openlineage-airflow-0.8.2/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-05-19 20:00:16.000000 openlineage-airflow-0.8.2/openlineage/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-05-19 20:00:16.000000 openlineage-airflow-0.8.2/openlineage/airflow/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      341 2022-05-19 20:00:10.000000 openlineage-airflow-0.8.2/openlineage/airflow/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7317 2022-05-19 20:00:10.000000 openlineage-airflow-0.8.2/openlineage/airflow/adapter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8844 2022-05-19 20:00:10.000000 openlineage-airflow-0.8.2/openlineage/airflow/dag.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-05-19 20:00:16.000000 openlineage-airflow-0.8.2/openlineage/airflow/extractors/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      320 2022-05-19 20:00:10.000000 openlineage-airflow-0.8.2/openlineage/airflow/extractors/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2128 2022-05-19 20:00:10.000000 openlineage-airflow-0.8.2/openlineage/airflow/extractors/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1847 2022-05-19 20:00:10.000000 openlineage-airflow-0.8.2/openlineage/airflow/extractors/bash_extractor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5051 2022-05-19 20:00:10.000000 openlineage-airflow-0.8.2/openlineage/airflow/extractors/bigquery_extractor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      596 2022-05-19 20:00:10.000000 openlineage-airflow-0.8.2/openlineage/airflow/extractors/example_dag.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3329 2022-05-19 20:00:10.000000 openlineage-airflow-0.8.2/openlineage/airflow/extractors/extractors.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1539 2022-05-19 20:00:10.000000 openlineage-airflow-0.8.2/openlineage/airflow/extractors/great_expectations_extractor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3256 2022-05-19 20:00:10.000000 openlineage-airflow-0.8.2/openlineage/airflow/extractors/manager.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6355 2022-05-19 20:00:10.000000 openlineage-airflow-0.8.2/openlineage/airflow/extractors/mysql_extractor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7441 2022-05-19 20:00:10.000000 openlineage-airflow-0.8.2/openlineage/airflow/extractors/postgres_extractor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2522 2022-05-19 20:00:10.000000 openlineage-airflow-0.8.2/openlineage/airflow/extractors/python_extractor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2070 2022-05-19 20:00:10.000000 openlineage-airflow-0.8.2/openlineage/airflow/extractors/snowflake_extractor.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1276 2022-05-19 20:00:10.000000 openlineage-airflow-0.8.2/openlineage/airflow/facets.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4825 2022-05-19 20:00:10.000000 openlineage-airflow-0.8.2/openlineage/airflow/listener.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2170 2022-05-19 20:00:10.000000 openlineage-airflow-0.8.2/openlineage/airflow/macros.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      745 2022-05-19 20:00:10.000000 openlineage-airflow-0.8.2/openlineage/airflow/plugin.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8159 2022-05-19 20:00:10.000000 openlineage-airflow-0.8.2/openlineage/airflow/utils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-05-19 20:00:16.000000 openlineage-airflow-0.8.2/openlineage/lineage_backend/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3249 2022-05-19 20:00:10.000000 openlineage-airflow-0.8.2/openlineage/lineage_backend/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-05-19 20:00:16.000000 openlineage-airflow-0.8.2/openlineage_airflow.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11740 2022-05-19 20:00:16.000000 openlineage-airflow-0.8.2/openlineage_airflow.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1199 2022-05-19 20:00:16.000000 openlineage-airflow-0.8.2/openlineage_airflow.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-05-19 20:00:16.000000 openlineage-airflow-0.8.2/openlineage_airflow.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       84 2022-05-19 20:00:16.000000 openlineage-airflow-0.8.2/openlineage_airflow.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-05-19 20:00:16.000000 openlineage-airflow-0.8.2/openlineage_airflow.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)      732 2022-05-19 20:00:16.000000 openlineage-airflow-0.8.2/openlineage_airflow.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       12 2022-05-19 20:00:16.000000 openlineage-airflow-0.8.2/openlineage_airflow.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      554 2022-05-19 20:00:16.000000 openlineage-airflow-0.8.2/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2023 2022-05-19 20:00:10.000000 openlineage-airflow-0.8.2/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:16.000000 openlineage-airflow-0.9.0/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11740 2022-06-03 23:03:16.000000 openlineage-airflow-0.9.0/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9352 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:16.000000 openlineage-airflow-0.9.0/openlineage/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:16.000000 openlineage-airflow-0.9.0/openlineage/airflow/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      669 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/airflow/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7317 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/airflow/adapter.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8844 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/airflow/dag.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:16.000000 openlineage-airflow-0.9.0/openlineage/airflow/extractors/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      320 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/airflow/extractors/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2128 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/airflow/extractors/base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1847 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/airflow/extractors/bash_extractor.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3808 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/airflow/extractors/bigquery_extractor.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2731 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/airflow/extractors/dbapi_utils.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      596 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/airflow/extractors/example_dag.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3329 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/airflow/extractors/extractors.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1539 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/airflow/extractors/great_expectations_extractor.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3256 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/airflow/extractors/manager.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4319 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/airflow/extractors/mysql_extractor.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4282 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/airflow/extractors/postgres_extractor.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2522 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/airflow/extractors/python_extractor.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5621 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/airflow/extractors/snowflake_extractor.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1415 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/airflow/facets.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6374 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/airflow/listener.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2170 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/airflow/macros.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      874 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/airflow/plugin.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8648 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/airflow/utils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:16.000000 openlineage-airflow-0.9.0/openlineage/lineage_backend/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3428 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/openlineage/lineage_backend/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-06-03 23:03:16.000000 openlineage-airflow-0.9.0/openlineage_airflow.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11740 2022-06-03 23:03:16.000000 openlineage-airflow-0.9.0/openlineage_airflow.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1245 2022-06-03 23:03:16.000000 openlineage-airflow-0.9.0/openlineage_airflow.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-06-03 23:03:16.000000 openlineage-airflow-0.9.0/openlineage_airflow.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       84 2022-06-03 23:03:16.000000 openlineage-airflow-0.9.0/openlineage_airflow.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-06-03 23:03:16.000000 openlineage-airflow-0.9.0/openlineage_airflow.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      732 2022-06-03 23:03:16.000000 openlineage-airflow-0.9.0/openlineage_airflow.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       12 2022-06-03 23:03:16.000000 openlineage-airflow-0.9.0/openlineage_airflow.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      554 2022-06-03 23:03:16.000000 openlineage-airflow-0.9.0/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2023 2022-06-03 23:03:12.000000 openlineage-airflow-0.9.0/setup.py
```

### Comparing `openlineage-airflow-0.8.2/PKG-INFO` & `openlineage-airflow-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlineage-airflow
-Version: 0.8.2
+Version: 0.9.0
 Summary: OpenLineage integration with Airflow
 Home-page: UNKNOWN
 Author: OpenLineage
 License: UNKNOWN
 Description: <!-- SPDX-License-Identifier: Apache-2.0 -->
         
         # OpenLineage Airflow Integration
```

### Comparing `openlineage-airflow-0.8.2/README.md` & `openlineage-airflow-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-0.8.2/openlineage/airflow/adapter.py` & `openlineage-airflow-0.9.0/openlineage/airflow/adapter.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-0.8.2/openlineage/airflow/dag.py` & `openlineage-airflow-0.9.0/openlineage/airflow/dag.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-0.8.2/openlineage/airflow/extractors/base.py` & `openlineage-airflow-0.9.0/openlineage/airflow/extractors/base.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-0.8.2/openlineage/airflow/extractors/bash_extractor.py` & `openlineage-airflow-0.9.0/openlineage/airflow/extractors/bash_extractor.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-0.8.2/openlineage/airflow/extractors/bigquery_extractor.py` & `openlineage-airflow-0.9.0/openlineage/airflow/extractors/bigquery_extractor.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,44 @@
 # SPDX-License-Identifier: Apache-2.0.
 
-import json
 import logging
 import traceback
 from typing import Optional, List
 from airflow.version import version as AIRFLOW_VERSION
 
-import attr
 from pkg_resources import parse_version
 
 from openlineage.client.facet import SqlJobFacet
 from openlineage.common.provider.bigquery import BigQueryDatasetsProvider, BigQueryErrorRunFacet
-from openlineage.common.sql import parse
 
 from openlineage.airflow.extractors.base import (
     BaseExtractor,
     TaskMetadata
 )
 from openlineage.airflow.utils import get_job_name, try_import_from_string
 from google.cloud.bigquery import Client
 
 _BIGQUERY_CONN_URL = 'bigquery'
 
 log = logging.getLogger(__name__)
 
 
-@attr.s
-class SqlContext:
-    """Internal SQL context for holding query parser results"""
-    sql: str = attr.ib()
-    inputs: Optional[str] = attr.ib(default=None)
-    outputs: Optional[str] = attr.ib(default=None)
-    parser_error: Optional[str] = attr.ib(default=None)
-
-
 class BigQueryExtractor(BaseExtractor):
     def __init__(self, operator):
         super().__init__(operator)
 
     @classmethod
     def get_operator_classnames(cls) -> List[str]:
         return ['BigQueryOperator', 'BigQueryExecuteQueryOperator']
 
     def extract(self) -> Optional[TaskMetadata]:
         return None
 
     def extract_on_complete(self, task_instance) -> Optional[TaskMetadata]:
         log.debug(f"extract_on_complete({task_instance})")
-        context = self.parse_sql_context()
 
         try:
             bigquery_job_id = self._get_xcom_bigquery_job_id(task_instance)
             if bigquery_job_id is None:
                 raise Exception(
                     "Xcom could not resolve BigQuery job id. Job may have failed."
                 )
@@ -60,27 +47,26 @@
                 f"Cannot retrieve job details from BigQuery.Client. {e}", exc_info=True
             )
             return TaskMetadata(
                 name=get_job_name(task=self.operator),
                 run_facets={
                     "bigQuery_error": BigQueryErrorRunFacet(
                         clientError=f"{e}: {traceback.format_exc()}",
-                        parserError=context.parser_error
                     )
                 }
             )
 
         client = self._get_client()
 
         stats = BigQueryDatasetsProvider(client=client).get_facets(bigquery_job_id)
         inputs = stats.inputs
         output = stats.output
         run_facets = stats.run_facets
         job_facets = {
-            "sql": SqlJobFacet(context.sql)
+            "sql": SqlJobFacet(self.operator.sql)
         }
 
         return TaskMetadata(
             name=get_job_name(task=self.operator),
             inputs=[ds.to_openlineage_dataset() for ds in inputs],
             outputs=[output.to_openlineage_dataset()] if output else [],
             run_facets=run_facets,
@@ -115,28 +101,7 @@
 
     def _get_xcom_bigquery_job_id(self, task_instance):
         bigquery_job_id = task_instance.xcom_pull(
             task_ids=task_instance.task_id, key='job_id')
 
         log.debug(f"bigquery_job_id: {bigquery_job_id}")
         return bigquery_job_id
-
-    def parse_sql_context(self) -> SqlContext:
-        try:
-            sql_meta = parse(self.operator.sql, dialect='bigquery')
-            log.debug(f"bigquery sql parsed and obtained meta: {sql_meta}")
-            return SqlContext(
-                sql=self.operator.sql,
-                inputs=json.dumps(
-                    [in_table.name for in_table in sql_meta.in_tables]
-                ),
-                outputs=json.dumps(
-                    [out_table.name for out_table in sql_meta.out_tables]
-                )
-            )
-        except Exception as e:
-            log.error(f"Cannot parse sql query. {e}",
-                      exc_info=True)
-            return SqlContext(
-                sql=self.operator.sql,
-                parser_error=f'{e}: {traceback.format_exc()}'
-            )
```

### Comparing `openlineage-airflow-0.8.2/openlineage/airflow/extractors/example_dag.py` & `openlineage-airflow-0.9.0/openlineage/airflow/extractors/example_dag.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-0.8.2/openlineage/airflow/extractors/extractors.py` & `openlineage-airflow-0.9.0/openlineage/airflow/extractors/extractors.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-0.8.2/openlineage/airflow/extractors/great_expectations_extractor.py` & `openlineage-airflow-0.9.0/openlineage/airflow/extractors/great_expectations_extractor.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-0.8.2/openlineage/airflow/extractors/manager.py` & `openlineage-airflow-0.9.0/openlineage/airflow/extractors/manager.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-0.8.2/openlineage/airflow/extractors/mysql_extractor.py` & `openlineage-airflow-0.9.0/openlineage/airflow/extractors/snowflake_extractor.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,189 +1,156 @@
-# SPDX-License-Identifier: Apache-2.0.
+# SPDX-License-Identifier: Apache-2.0
+
 import logging
-from contextlib import closing
-from typing import Optional, List
-from urllib.parse import urlparse
-
-from openlineage.airflow.utils import (
-    get_connection_uri,
-    get_connection, safe_import_airflow
-)
-from openlineage.airflow.extractors.base import (
-    BaseExtractor,
-    TaskMetadata
-)
-from openlineage.client.facet import SqlJobFacet
-from openlineage.common.models import (
-    DbTableSchema,
-    DbColumn
-)
+from typing import List, TYPE_CHECKING, Optional
+
+from openlineage.airflow.extractors.base import BaseExtractor, TaskMetadata
+from openlineage.airflow.extractors.dbapi_utils import get_table_schemas
+from openlineage.airflow.utils import get_connection_uri, get_connection  # noqa
+from openlineage.client.facet import SqlJobFacet, ExternalQueryRunFacet
+from openlineage.common.dataset import Source
 from openlineage.common.sql import SqlMeta, parse, DbTableMeta
-from openlineage.common.dataset import Source, Dataset
 
-_TABLE_SCHEMA = 0
-_TABLE_NAME = 1
-_COLUMN_NAME = 2
-_ORDINAL_POSITION = 3
-_COLUMN_TYPE = 4
 
-logger = logging.getLogger(__name__)
+if TYPE_CHECKING:
+    from airflow.models import Connection
+
 
+logger = logging.getLogger(__file__)
 
-class MySqlExtractor(BaseExtractor):
-    default_schema = None
+
+class SnowflakeExtractor(BaseExtractor):
+    source_type = 'SNOWFLAKE'
+    default_schema = 'PUBLIC'
 
     def __init__(self, operator):
         super().__init__(operator)
-        self.conn = None
+        self.conn: "Connection" = None
+        self.hook = None
 
     @classmethod
     def get_operator_classnames(cls) -> List[str]:
-        return ['MySqlOperator']
+        return ['SnowflakeOperator']
 
     def extract(self) -> TaskMetadata:
+        task_name = f"{self.operator.dag_id}.{self.operator.task_id}"
+        run_facets = {}
+        job_facets = {
+            'sql': SqlJobFacet(self.operator.sql)
+        }
+
         # (1) Parse sql statement to obtain input / output tables.
-        sql_meta: SqlMeta = parse(self.operator.sql, self.default_schema)
+        logger.debug(f"Sending SQL to parser: {self.operator.sql}")
+        sql_meta: Optional[SqlMeta] = parse(self.operator.sql, self.default_schema)
+        logger.debug(f"Got meta {sql_meta}")
+
+        if not sql_meta:
+            return TaskMetadata(
+                name=task_name,
+                inputs=[],
+                outputs=[],
+                run_facets=run_facets,
+                job_facets=job_facets
+            )
 
-        # (2) Get database connection
+        # (2) Get Airflow connection
         self.conn = get_connection(self._conn_id())
 
         # (3) Default all inputs / outputs to current connection.
         # NOTE: We'll want to look into adding support for the `database`
         # property that is used to override the one defined in the connection.
         source = Source(
-            scheme=self._get_scheme(),
+            scheme='snowflake',
             authority=self._get_authority(),
             connection_url=self._get_connection_uri()
         )
 
         database = self.operator.database
         if not database:
             database = self._get_database()
 
         # (4) Map input / output tables to dataset objects with source set
         # as the current connection. We need to also fetch the schema for the
         # input tables to format the dataset name as:
         # {schema_name}.{table_name}
-        inputs = [
-            Dataset.from_table(
-                source=source,
-                table_name=in_table_schema.table_name.name,
-                schema_name=in_table_schema.schema_name,
-                database_name=database
-            ) for in_table_schema in self._get_table_schemas(
-                sql_meta.in_tables
+        inputs, outputs = get_table_schemas(
+            self._get_hook(),
+            source,
+            database,
+            self._information_schema_query(sql_meta.in_tables) if sql_meta.in_tables else None,
+            self._information_schema_query(sql_meta.out_tables) if sql_meta.out_tables else None
+        )
+
+        query_ids = self._get_query_ids()
+        if len(query_ids) == 1:
+            run_facets['externalQuery'] = ExternalQueryRunFacet(
+                externalQueryId=query_ids[0],
+                source=source.name
             )
-        ]
-        outputs = [
-            Dataset.from_table_schema(
-                source=source,
-                table_schema=out_table_schema,
-                database_name=database
-            ) for out_table_schema in self._get_table_schemas(
-                sql_meta.out_tables
+        elif len(query_ids) > 1:
+            logger.warning(
+                f"Found more than one query id for task {task_name}: {query_ids} "
+                "This might indicate that this task might be better as multiple jobs"
             )
-        ]
-
-        task_name = f"{self.operator.dag_id}.{self.operator.task_id}"
-        run_facets = {}
-        job_facets = {
-            'sql': SqlJobFacet(self.operator.sql)
-        }
 
         return TaskMetadata(
             name=task_name,
             inputs=[ds.to_openlineage_dataset() for ds in inputs],
             outputs=[ds.to_openlineage_dataset() for ds in outputs],
             run_facets=run_facets,
             job_facets=job_facets
         )
 
-    def _get_connection_uri(self):
-        return get_connection_uri(self.conn)
-
-    def _get_scheme(self):
-        return 'mysql'
+    def _information_schema_query(self, tables: List[DbTableMeta]) -> str:
+        table_names = ",".join(map(
+            lambda name: f"'{self._normalize_identifiers(name.name)}'", tables
+        ))
+        database = self.operator.database
+        if not database:
+            database = self._get_database()
+        sql = f"""
+        SELECT table_schema,
+               table_name,
+               column_name,
+               ordinal_position,
+               data_type
+          FROM {database}.information_schema.columns
+         WHERE table_name IN ({table_names});
+        """
+        return sql
 
     def _get_database(self) -> str:
-        if self.conn.schema:
-            return self.conn.schema
-        else:
-            parsed = urlparse(self.conn.get_uri())
-            return f'{parsed.path}'
+        if hasattr(self.operator, 'database') and self.operator.database is not None:
+            return self.operator.database
+        return self.conn.extra_dejson.get('extra__snowflake__database', '') \
+            or self.conn.extra_dejson.get('database', '')
 
     def _get_authority(self) -> str:
-        if self.conn.host and self.conn.port:
-            return f'{self.conn.host}:{self.conn.port}'
+        if hasattr(self.operator, 'account') and self.operator.account is not None:
+            return self.operator.account
+        return self.conn.extra_dejson.get('extra__snowflake__account', '') \
+            or self.conn.extra_dejson.get('account', '')
+
+    def _get_hook(self):
+        if hasattr(self.operator, 'get_db_hook'):
+            return self.operator.get_db_hook()
         else:
-            parsed = urlparse(self.conn.get_uri())
-            return f'{parsed.hostname}:{parsed.port}'
+            return self.operator.get_hook()
 
     def _conn_id(self):
-        return self.operator.mysql_conn_id
+        return self.operator.snowflake_conn_id
 
-    def _information_schema_query(self, table_names: str) -> str:
-        return f"""
-        SELECT table_schema,
-        table_name,
-        column_name,
-        ordinal_position,
-        column_type
-        FROM information_schema.columns
-        WHERE table_name IN ({table_names});
+    def _normalize_identifiers(self, table: str):
         """
+        Snowflake keeps it's table names in uppercase, so we need to normalize
+        them before use: see
+        https://community.snowflake.com/s/question/0D50Z00009SDHEoSAP/is-there-case-insensitivity-for-table-name-or-column-names  # noqa
+        """
+        return table.upper()
 
-    def _get_hook(self):
-        MySqlHook = safe_import_airflow(
-            airflow_1_path="airflow.hooks.mysql_hook.MySqlHook",
-            airflow_2_path="airflow.providers.mysql.hooks.mysql.MySqlHook"
-        )
-        return MySqlHook(
-            mysql_conn_id=self.operator.mysql_conn_id,
-            schema=self.operator.database
-        )
-
-    def _get_table_schemas(
-            self, table_names: [DbTableMeta]
-    ) -> [DbTableSchema]:
-        # Avoid querying mysql by returning an empty array
-        # if no table names have been provided.
-        if not table_names:
-            return []
-
-        # Keeps tack of the schema by table.
-        schemas_by_table = {}
-
-        hook = self._get_hook()
-        with closing(hook.get_conn()) as conn:
-            with closing(conn.cursor()) as cursor:
-                table_names_as_str = ",".join(map(
-                    lambda name: f"'{name.name}'", table_names
-                ))
-                cursor.execute(
-                    self._information_schema_query(table_names_as_str)
-                )
-                for row in cursor.fetchall():
-                    table_schema_name: str = row[_TABLE_SCHEMA]
-                    table_name: DbTableMeta = DbTableMeta(row[_TABLE_NAME])
-                    table_column: DbColumn = DbColumn(
-                        name=row[_COLUMN_NAME],
-                        type=row[_COLUMN_TYPE],
-                        ordinal_position=row[_ORDINAL_POSITION]
-                    )
-
-                    # Attempt to get table schema
-                    table_key: str = f"{table_schema_name}.{table_name}"
-                    table_schema: Optional[DbTableSchema] = schemas_by_table.get(table_key)
-
-                    if table_schema:
-                        # Add column to existing table schema.
-                        schemas_by_table[table_key].columns.append(table_column)
-                    else:
-                        # Create new table schema with column.
-                        schemas_by_table[table_key] = DbTableSchema(
-                            schema_name=table_schema_name,
-                            table_name=table_name,
-                            columns=[table_column]
-                        )
+    def _get_connection_uri(self):
+        return get_connection_uri(self.conn)
 
-        return list(schemas_by_table.values())
+    def _get_query_ids(self) -> List[str]:
+        if hasattr(self.operator, 'query_ids'):
+            return self.operator.query_ids
+        return []
```

### Comparing `openlineage-airflow-0.8.2/openlineage/airflow/extractors/python_extractor.py` & `openlineage-airflow-0.9.0/openlineage/airflow/extractors/python_extractor.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-0.8.2/openlineage/airflow/facets.py` & `openlineage-airflow-0.9.0/openlineage/airflow/facets.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,36 +13,41 @@
     operator: str = attr.ib()
     taskInfo: str = attr.ib()
     airflowVersion: str = attr.ib()
     openlineageAirflowVersion: str = attr.ib()
 
     @classmethod
     def from_task(cls, task):
+        # task.__dict__ may contain values uncastable to str
+        from openlineage.airflow.utils import SafeStrDict
         return cls(
-            f'{task.__class__.__module__}.{task.__class__.__name__}',
-            str(task.__dict__),
+            f"{task.__class__.__module__}.{task.__class__.__name__}",
+            str(SafeStrDict(task.__dict__)),
             AIRFLOW_VERSION,
-            OPENLINEAGE_AIRFLOW_VERSION
+            OPENLINEAGE_AIRFLOW_VERSION,
         )
 
 
 @attr.s
 class AirflowRunArgsRunFacet(BaseFacet):
     externalTrigger: bool = attr.ib(default=False)
 
 
 @attr.s
 class UnknownOperatorInstance:
     """
-    Describes an unknown operator - specifies the (class) name of the operator and its properties
+    Describes an unknown operator - specifies the (class) name of the operator
+    and its properties
     """
+
     name: str = attr.ib()
     properties: Dict[str, object] = attr.ib()
     type: str = attr.ib(default="operator")
 
 
 @attr.s
 class UnknownOperatorAttributeRunFacet(BaseFacet):
     """
     RunFacet that describes unknown operators in an Airflow DAG
     """
+
     unknownItems: List[UnknownOperatorInstance] = attr.ib()
```

### Comparing `openlineage-airflow-0.8.2/openlineage/airflow/macros.py` & `openlineage-airflow-0.9.0/openlineage/airflow/macros.py`

 * *Files identical despite different names*

### Comparing `openlineage-airflow-0.8.2/openlineage/airflow/utils.py` & `openlineage-airflow-0.9.0/openlineage/airflow/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 # SPDX-License-Identifier: Apache-2.0.
 import importlib
 import json
 import logging
 import os
 import subprocess
+from typing import TYPE_CHECKING
 from uuid import uuid4
 from urllib.parse import urlparse, urlunparse, parse_qs, urlencode
 
 from airflow.version import version as AIRFLOW_VERSION
 
 from pkg_resources import parse_version
 
 from openlineage.airflow.facets import AirflowVersionRunFacet, AirflowRunArgsRunFacet
 from pendulum import from_timestamp
 
+
+if TYPE_CHECKING:
+    from airflow.models import Connection
+
+
 log = logging.getLogger(__name__)
 _NOMINAL_TIME_FORMAT = "%Y-%m-%dT%H:%M:%S.%fZ"
 
 
 def openlineage_job_name(dag_id: str, task_id: str) -> str:
     return f'{dag_id}.{task_id}'
 
@@ -54,14 +60,26 @@
                 return None
 
     @staticmethod
     def make_key(job_name, run_id):
         return "openlineage_id_mapping-{}-{}".format(job_name, run_id)
 
 
+class SafeStrDict(dict):
+    def __str__(self):
+        castable = list()
+        for attr, val in self.items():
+            try:
+                str(attr), str(val)
+                castable.append((attr, val))
+            except (TypeError, NotImplementedError):
+                continue
+        return str(dict(castable))
+
+
 def url_to_https(url) -> str:
     # Ensure URL exists
     if not url:
         return None
 
     base_url = None
     if url.startswith('git@'):
@@ -131,15 +149,16 @@
     the Airflow's connection table.
     """
 
     conn_uri = conn.get_uri()
     parsed = urlparse(conn_uri)
 
     # Remove username and password
-    parsed = parsed._replace(netloc=f'{parsed.hostname}:{parsed.port}')
+    netloc = f'{parsed.hostname}' + (f':{parsed.port}' if parsed.port else "")
+    parsed = parsed._replace(netloc=netloc)
     query_dict = parse_qs(parsed.query)
     filtered_qs = {k: query_dict[k]
                    for k in query_dict.keys()
                    if not _filtered_query_params(k)}
     parsed = parsed._replace(query=urlencode(filtered_qs))
     return urlunparse(parsed)
 
@@ -163,15 +182,15 @@
     """
     uri = get_connection_uri(conn)
     if uri.startswith('postgresql'):
         uri = uri.replace('postgresql', 'postgres', 1)
     return uri
 
 
-def get_connection(conn_id):
+def get_connection(conn_id) -> "Connection":
     # TODO: We may want to throw an exception if the connection
     # does not exist (ex: AirflowConnectionException). The connection
     # URI is required when collecting metadata for a data source.
     from airflow.models import Connection
     conn_uri = os.environ.get('AIRFLOW_CONN_' + conn_id.upper())
     if conn_uri:
         conn = Connection()
```

### Comparing `openlineage-airflow-0.8.2/openlineage/lineage_backend/__init__.py` & `openlineage-airflow-0.9.0/openlineage/lineage_backend/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: Apache-2.0
-
+import os
 import uuid
 import time
 
 from pkg_resources import parse_version
 
 from airflow.lineage.backend import LineageBackend
 from airflow.version import version as AIRFLOW_VERSION
@@ -84,10 +84,13 @@
     backend: Backend = None
 
     @classmethod
     def send_lineage(cls, *args, **kwargs):
         # Do not use LineageBackend approach when we can use plugins
         if parse_version(AIRFLOW_VERSION) >= parse_version("2.3.0.dev0"):
             return
+        # Make this method a noop if OPENLINEAGE_DISABLED is set to true
+        if os.getenv("OPENLINEAGE_DISABLED", None) in [True, 'true', "True"]:
+            return
         if not cls.backend:
             cls.backend = Backend()
         return cls.backend.send_lineage(*args, **kwargs)
```

### Comparing `openlineage-airflow-0.8.2/openlineage_airflow.egg-info/PKG-INFO` & `openlineage-airflow-0.9.0/openlineage_airflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlineage-airflow
-Version: 0.8.2
+Version: 0.9.0
 Summary: OpenLineage integration with Airflow
 Home-page: UNKNOWN
 Author: OpenLineage
 License: UNKNOWN
 Description: <!-- SPDX-License-Identifier: Apache-2.0 -->
         
         # OpenLineage Airflow Integration
```

### Comparing `openlineage-airflow-0.8.2/openlineage_airflow.egg-info/SOURCES.txt` & `openlineage-airflow-0.9.0/openlineage_airflow.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 openlineage/airflow/macros.py
 openlineage/airflow/plugin.py
 openlineage/airflow/utils.py
 openlineage/airflow/extractors/__init__.py
 openlineage/airflow/extractors/base.py
 openlineage/airflow/extractors/bash_extractor.py
 openlineage/airflow/extractors/bigquery_extractor.py
+openlineage/airflow/extractors/dbapi_utils.py
 openlineage/airflow/extractors/example_dag.py
 openlineage/airflow/extractors/extractors.py
 openlineage/airflow/extractors/great_expectations_extractor.py
 openlineage/airflow/extractors/manager.py
 openlineage/airflow/extractors/mysql_extractor.py
 openlineage/airflow/extractors/postgres_extractor.py
 openlineage/airflow/extractors/python_extractor.py
```

### Comparing `openlineage-airflow-0.8.2/setup.cfg` & `openlineage-airflow-0.9.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.8.2
+current_version = 0.9.0
 commit = False
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?P<rc>.*)
 serialize = 
 	{major}.{minor}.{patch}{rc}
 	{major}.{minor}.{patch}
```

### Comparing `openlineage-airflow-0.8.2/setup.py` & `openlineage-airflow-0.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import setup, find_namespace_packages
 
 with open("README.md") as readme_file:
     readme = readme_file.read()
 
-__version__ = "0.8.2"
+__version__ = "0.9.0"
 
 requirements = [
     "attrs>=19.3",
     "requests>=2.20.0",
     "sqlparse>=0.3.1",
     f"openlineage-integration-common=={__version__}",
     f"openlineage-python=={__version__}",
```

