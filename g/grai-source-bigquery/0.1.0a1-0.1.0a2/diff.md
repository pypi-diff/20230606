# Comparing `tmp/grai_source_bigquery-0.1.0a1.tar.gz` & `tmp/grai_source_bigquery-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_bigquery-0.1.0a1.tar", max compression
+gzip compressed data, was "grai_source_bigquery-0.1.0a2.tar", max compression
```

## Comparing `grai_source_bigquery-0.1.0a1.tar` & `grai_source_bigquery-0.1.0a2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      141 2023-05-02 08:01:59.695304 grai_source_bigquery-0.1.0a1/README.md
--rw-r--r--   0        0        0      971 2023-06-04 15:51:10.689502 grai_source_bigquery-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0      145 2023-02-14 12:06:39.088033 grai_source_bigquery-0.1.0a1/src/grai_source_bigquery/__init__.py
--rw-r--r--   0        0        0     8578 2023-06-02 08:26:06.787907 grai_source_bigquery-0.1.0a1/src/grai_source_bigquery/adapters.py
--rw-r--r--   0        0        0     2124 2023-06-04 15:50:44.843872 grai_source_bigquery-0.1.0a1/src/grai_source_bigquery/base.py
--rw-r--r--   0        0        0    12864 2023-06-04 15:50:44.997687 grai_source_bigquery-0.1.0a1/src/grai_source_bigquery/loader.py
--rw-r--r--   0        0        0     6120 2023-06-04 15:50:44.919123 grai_source_bigquery-0.1.0a1/src/grai_source_bigquery/models.py
--rw-r--r--   0        0        0      199 2023-06-02 08:26:06.789100 grai_source_bigquery-0.1.0a1/src/grai_source_bigquery/package_definitions.py
--rw-r--r--   0        0        0     1169 1970-01-01 00:00:00.000000 grai_source_bigquery-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0      141 2023-05-02 08:01:59.695304 grai_source_bigquery-0.1.0a2/README.md
+-rw-r--r--   0        0        0      971 2023-06-06 07:58:43.719920 grai_source_bigquery-0.1.0a2/pyproject.toml
+-rw-r--r--   0        0        0      145 2023-02-14 12:06:39.088033 grai_source_bigquery-0.1.0a2/src/grai_source_bigquery/__init__.py
+-rw-r--r--   0        0        0     8578 2023-06-02 08:26:06.787907 grai_source_bigquery-0.1.0a2/src/grai_source_bigquery/adapters.py
+-rw-r--r--   0        0        0     2124 2023-06-05 14:56:39.992488 grai_source_bigquery-0.1.0a2/src/grai_source_bigquery/base.py
+-rw-r--r--   0        0        0    13309 2023-06-05 17:43:32.597569 grai_source_bigquery-0.1.0a2/src/grai_source_bigquery/loader.py
+-rw-r--r--   0        0        0     6222 2023-06-05 17:34:49.806426 grai_source_bigquery-0.1.0a2/src/grai_source_bigquery/models.py
+-rw-r--r--   0        0        0      199 2023-06-02 08:26:06.789100 grai_source_bigquery-0.1.0a2/src/grai_source_bigquery/package_definitions.py
+-rw-r--r--   0        0        0     1169 1970-01-01 00:00:00.000000 grai_source_bigquery-0.1.0a2/PKG-INFO
```

### Comparing `grai_source_bigquery-0.1.0a1/pyproject.toml` & `grai_source_bigquery-0.1.0a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai_source_bigquery"
-version = "0.1.0-alpha1"
+version = "0.1.0-alpha2"
 description = ""
 authors = ["Edward Louth <edward@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_bigquery", from = "src" },
 ]
 readme = "README.md"
```

### Comparing `grai_source_bigquery-0.1.0a1/src/grai_source_bigquery/adapters.py` & `grai_source_bigquery-0.1.0a2/src/grai_source_bigquery/adapters.py`

 * *Files identical despite different names*

### Comparing `grai_source_bigquery-0.1.0a1/src/grai_source_bigquery/base.py` & `grai_source_bigquery-0.1.0a2/src/grai_source_bigquery/base.py`

 * *Files identical despite different names*

### Comparing `grai_source_bigquery-0.1.0a1/src/grai_source_bigquery/loader.py` & `grai_source_bigquery-0.1.0a2/src/grai_source_bigquery/loader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import os
 from datetime import datetime, timedelta, timezone
-from functools import cached_property
+from functools import cached_property, lru_cache
 from itertools import chain
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 from google.cloud import bigquery, logging
 from google.oauth2 import service_account
 
 from grai_source_bigquery.models import (
@@ -44,222 +44,39 @@
             f"Establishing bigquery connection requires a {label}. "
             f"Either pass a value explicitly or set a {env_key} environment value."
         )
         raise Exception(message)
     return result if validator is None else validator(result)
 
 
-class LoggingConnector:
-    """ """
-
-    def __init__(
-        self,
-        namespace: Optional[str] = None,
-        project: Optional[str] = None,
-        dataset: Optional[Union[str, List[str]]] = None,
-        credentials: Optional[str] = None,
-        window: Optional[int] = None,
-    ):
-        self.namespace = get_from_env("namespace", "default") if namespace is None else namespace
-        self.project = get_from_env("project", required=False) if project is None else project
-        self.dataset = get_from_env("dataset", required=False) if dataset is None else dataset
-        self.credentials = get_from_env("credentials", required=False) if credentials is None else credentials
-        self.window = int(get_from_env("window", required=False, default=7)) if window is None else window
-        self._connection: Optional[logging.Client] = None
-
-    def __enter__(self):
-        return self.connect()
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        self.close()
-
-    def connect(self) -> "LoggingConnector":
-        """
-
-        Args:
-
-        Returns:
-
-        Raises:
-
-        """
-        if self._connection is None:
-            credentials = None
-
-            if self.credentials:
-                json_acct_info = json.loads(self.credentials, strict=False)
-                credentials = service_account.Credentials.from_service_account_info(json_acct_info)
-
-            self._connection = logging.Client(credentials=credentials, project=self.project)
-        return self
-
-    @property
-    def connection(self) -> logging.Client:
-        """
-
-        Args:
-
-        Returns:
-
-        Raises:
-
-        """
-        if self._connection is None:
-            raise Exception("Not connected, call `.connect()")
-        return self._connection
-
-    def close(self) -> None:
-        """
-
-        Args:
-
-        Returns:
-
-        Raises:
-
-        """
-        self.connection.close()
-        self._connection = None
-
-    @cached_property
-    def logs(self) -> List[Any]:
-        """Create and return a list of dictionaries with the
-        schemas and names of tables in the database
-        connected to by the connection argument.
-
-        Args:
-
-        Returns:
-
-        Raises:
-
-        """
-
-        yesterday = datetime.now(timezone.utc) - timedelta(days=self.window)
-        time_format = "%Y-%m-%dT%H:%M:%S.%f%z"
-
-        filter_str = (
-            'protoPayload.serviceName="bigquery.googleapis.com"'
-            ' AND resource.type = "bigquery_project"'
-            ' AND protoPayload.methodName="google.cloud.bigquery.v2.JobService.InsertJob"'
-            f' AND timestamp>="{yesterday.strftime(time_format)}"'
-        )
-
-        return self.connection.list_entries(filter_=filter_str, page_size=1000)
-
-    def get_edges(self, existing_nodes) -> List[Edge]:
-        """
-
-        Args:
-
-        Returns:
-
-        Raises:
-
-        """
-
-        def table_string_to_table_id(table_string: str) -> Optional[TableID]:
-            table_string = table_string.split("/")
-
-            schema = table_string[3]
-            name = table_string[5]
-
-            if not any(node.name == name and node.table_schema == schema for node in existing_nodes):
-                return None
-
-            return TableID(
-                table_schema=schema,
-                name=name,
-                namespace=self.namespace,
-            )
-
-        edges = set()
-
-        for log in self.logs:
-            content = log.to_api_repr()
-
-            destination_table = (
-                content.get("protoPayload", {})
-                .get("metadata", {})
-                .get("jobChange", {})
-                .get("job", {})
-                .get("jobConfig", {})
-                .get("queryConfig", {})
-                .get("destinationTable")
-            ) or (
-                content.get("protoPayload", {})
-                .get("metadata", {})
-                .get("jobInsertion", {})
-                .get("job", {})
-                .get("jobConfig", {})
-                .get("queryConfig", {})
-                .get("destinationTable")
-            )
-
-            if destination_table is None:
-                continue
-
-            destination = table_string_to_table_id(destination_table)
-
-            if destination is None:
-                continue
-
-            referenced_tables = (
-                content.get("protoPayload", {})
-                .get("metadata", {})
-                .get("jobChange", {})
-                .get("job", {})
-                .get("jobStats", {})
-                .get("queryStats", {})
-                .get("referencedTables", [])
-            ) or (
-                content.get("protoPayload", {})
-                .get("metadata", {})
-                .get("jobInsertion", {})
-                .get("job", {})
-                .get("jobStats", {})
-                .get("queryStats", {})
-                .get("referencedTables", [])
-            )
-
-            for table in referenced_tables:
-                if destination_table == table:
-                    continue
-
-                source = table_string_to_table_id(table)
-
-                if source is None:
-                    continue
-
-                edges.add(
-                    Edge(
-                        constraint_type=Constraint("bqm"),
-                        source=source,
-                        destination=destination,
-                    )
-                )
-
-        return list(edges)
-
-
 class BigqueryConnector:
     """ """
 
     def __init__(
         self,
         namespace: Optional[str] = None,
         project: Optional[str] = None,
         dataset: Optional[Union[str, List[str]]] = None,
         credentials: Optional[str] = None,
         **kwargs,
     ):
-        self.namespace = get_from_env("namespace", "default") if namespace is None else namespace
-        self.project = get_from_env("project", required=False) if project is None else project
-        self.dataset = get_from_env("dataset", required=False) if dataset is None else dataset
-        self.credentials = get_from_env("credentials", required=False) if credentials is None else credentials
+        self.namespace = (
+            get_from_env("namespace", "default") if namespace is None else namespace
+        )
+        self.project = (
+            get_from_env("project", required=False) if project is None else project
+        )
+        self.dataset = (
+            get_from_env("dataset", required=False) if dataset is None else dataset
+        )
+        self.credentials = (
+            get_from_env("credentials", required=False)
+            if credentials is None
+            else credentials
+        )
         self._connection: Optional[bigquery.connector.BigqueryConnection] = None
 
         self._tables: Optional[List[Table]] = None
         self._foreign_keys: Optional[List[Edge]] = None
 
     def __enter__(self):
         return self.connect()
@@ -278,17 +95,21 @@
 
         """
         if self._connection is None:
             credentials = None
 
             if self.credentials:
                 json_acct_info = json.loads(self.credentials, strict=False)
-                credentials = service_account.Credentials.from_service_account_info(json_acct_info)
+                credentials = service_account.Credentials.from_service_account_info(
+                    json_acct_info
+                )
 
-            self._connection = bigquery.Client(credentials=credentials, project=self.project)
+            self._connection = bigquery.Client(
+                credentials=credentials, project=self.project
+            )
         return self
 
     @property
     def connection(self) -> bigquery.Client:
         """
 
         Args:
@@ -325,166 +146,383 @@
         Returns:
 
         Raises:
 
         """
         return self.connection.query(query)
 
-    @cached_property
-    def tables(self) -> List[Table]:
+    @lru_cache
+    def tables(self, dataset: str) -> List[Table]:
         """Create and return a list of dictionaries with the
         schemas and names of tables in the database
         connected to by the connection argument.
 
         Args:
 
         Returns:
 
         Raises:
 
         """
         query = f"""
             SELECT table_schema, table_name, table_type
-            FROM {self.project}.{self.dataset}.INFORMATION_SCHEMA.TABLES
+            FROM {self.project}.{dataset}.INFORMATION_SCHEMA.TABLES
             WHERE table_schema != 'INFORMATION_SCHEMA'
             ORDER BY table_schema, table_name
         """
-        res = ({k.lower(): v for k, v in result.items()} for result in self.query_runner(query))
+        res = (
+            {k.lower(): v for k, v in result.items()}
+            for result in self.query_runner(query)
+        )
 
         additional_args = {
             "namespace": self.namespace,
-            "table_dataset": self.dataset,
+            "table_dataset": dataset,
         }
 
         tables = [Table(**result, **additional_args) for result in res]
         for table in tables:
-            table.columns = self.get_table_columns(table)
+            table.columns = self.get_table_columns(table, dataset)
         return tables
 
-    @cached_property
-    def columns(self) -> List[Column]:
+    @lru_cache
+    def columns(self, dataset: str) -> List[Column]:
         """Creates and returns a list of dictionaries for the specified
         schema.table in the database connected to.
 
         Args:
 
         Returns:
 
         Raises:
 
         """
 
         query = f"""
             SELECT column_name, data_type, is_nullable, column_default, table_schema, table_name
-            FROM {self.project}.{self.dataset}.INFORMATION_SCHEMA.COLUMNS
+            FROM {self.project}.{dataset}.INFORMATION_SCHEMA.COLUMNS
         """
 
-        res = [{k.lower(): v for k, v in result.items()} for result in self.query_runner(query)]
+        res = [
+            {k.lower(): v for k, v in result.items()}
+            for result in self.query_runner(query)
+        ]
         for item in res:
             item.update(
                 {
                     "table": item["table_name"],
                     "column_schema": item["table_schema"],
                 }
             )
 
         addtl_args = {
             "namespace": self.namespace,
         }
         return [Column(**result, **addtl_args) for result in res]
 
-    @cached_property
-    def column_map(self) -> Dict[Tuple[str, str], List[Column]]:
+    @lru_cache
+    def column_map(self, dataset: str) -> Dict[Tuple[str, str], List[Column]]:
         """
 
         Args:
 
         Returns:
 
         Raises:
 
         """
         result_map: Dict[Tuple[str, str], List[Column]] = {}
-        for col in self.columns:
+        for col in self.columns(dataset):
             table_id = (col.column_schema, col.table)
             result_map.setdefault(table_id, [])
             result_map[table_id].append(col)
         return result_map
 
-    def get_table_columns(self, table: Table) -> List[Column]:
+    def get_table_columns(self, table: Table, dataset: str) -> List[Column]:
         """
 
         Args:
             table (Table):
 
         Returns:
 
         Raises:
 
         """
         table_id = (table.table_schema, table.name)
-        if table_id in self.column_map:
-            return self.column_map[table_id]
+
+        column_map = self.column_map(dataset)
+
+        if table_id in column_map:
+            return column_map[table_id]
 
         schema = table_id[0]
         name = table_id[1]
         table_id = (schema, name)
-        if table_id in self.column_map:
-            return self.column_map[table_id]
+        if table_id in column_map:
+            return column_map[table_id]
         else:
-            raise Exception(f"No columns found for table with schema={schema} and name={name}")
+            raise Exception(
+                f"No columns found for table with schema={schema} and name={name}"
+            )
 
-    def get_nodes(self) -> List[BigqueryNode]:
+    def get_nodes(self, dataset: str) -> List[BigqueryNode]:
         """
 
         Args:
 
         Returns:
 
         Raises:
 
         """
-        return list(chain(self.tables, self.columns))
+        return list(chain(self.tables(dataset), self.columns(dataset)))
 
-    def get_edges(self) -> List[Edge]:
+    def get_edges(self, dataset: str) -> List[Edge]:
         """
 
         Args:
 
         Returns:
 
         Raises:
 
         """
-        return [item for item in chain(*[t.get_edges() for t in self.tables]) if item is not None]
+        return [
+            item
+            for item in chain(*[t.get_edges() for t in self.tables(dataset)])
+            if item is not None
+        ]
 
-    def _get_nodes_and_edges(self) -> Tuple[List[BigqueryNode], List[Edge]]:
+    def get_nodes_and_edges(self) -> Tuple[List[BigqueryNode], List[Edge]]:
         """
 
         Args:
 
         Returns:
 
         Raises:
 
         """
-        nodes = self.get_nodes()
-        edges = self.get_edges()
-        return nodes, edges
-
-    def get_nodes_and_edges(self) -> Tuple[List[BigqueryNode], List[Edge]]:
         datasets = [self.dataset] if isinstance(self.dataset, str) else self.dataset
 
         nodes = []
         edges = []
 
         for dataset in datasets:
-            self.dataset = dataset
-            n, e = self._get_nodes_and_edges()
-            nodes.extend(n)
-            edges.extend(e)
-
-            del self.tables
-            del self.columns
-            del self.column_map
+            nodes.extend(self.get_nodes(dataset))
+            edges.extend(self.get_edges(dataset))
 
         return nodes, edges
+
+
+class LoggingConnector(BigqueryConnector):
+    """ """
+
+    def __init__(
+        self,
+        namespace: Optional[str] = None,
+        project: Optional[str] = None,
+        dataset: Optional[Union[str, List[str]]] = None,
+        credentials: Optional[str] = None,
+        window: Optional[int] = None,
+    ):
+        super().__init__(namespace, project, dataset, credentials)
+
+        self.window = (
+            int(get_from_env("window", required=False, default=7))
+            if window is None
+            else window
+        )
+        self._logging_connection: Optional[logging.Client] = None
+
+    def __enter__(self):
+        super().__enter__()
+
+        return self.logging_connect()
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        super().__exit__(exc_type, exc_val, exc_tb)
+        self.logging_close()
+
+    def logging_connect(self) -> "LoggingConnector":
+        """
+
+        Args:
+
+        Returns:
+
+        Raises:
+
+        """
+        if self._logging_connection is None:
+            credentials = None
+
+            if self.credentials:
+                json_acct_info = json.loads(self.credentials, strict=False)
+                credentials = service_account.Credentials.from_service_account_info(
+                    json_acct_info
+                )
+
+            self._logging_connection = logging.Client(
+                credentials=credentials, project=self.project
+            )
+        return self
+
+    @property
+    def logging_connection(self) -> logging.Client:
+        """
+
+        Args:
+
+        Returns:
+
+        Raises:
+
+        """
+        if self._logging_connection is None:
+            raise Exception("Not connected, call `.connect()")
+        return self._logging_connection
+
+    def logging_close(self) -> None:
+        """
+
+        Args:
+
+        Returns:
+
+        Raises:
+
+        """
+        self.logging_connection.close()
+        self._logging_connection = None
+
+    @cached_property
+    def logs(self) -> List[Any]:
+        """Create and return a list of dictionaries with the
+        schemas and names of tables in the database
+        connected to by the connection argument.
+
+        Args:
+
+        Returns:
+
+        Raises:
+
+        """
+
+        yesterday = datetime.now(timezone.utc) - timedelta(days=self.window)
+        time_format = "%Y-%m-%dT%H:%M:%S.%f%z"
+
+        filter_str = (
+            'protoPayload.serviceName="bigquery.googleapis.com"'
+            ' AND resource.type = "bigquery_project"'
+            ' AND protoPayload.methodName="google.cloud.bigquery.v2.JobService.InsertJob"'
+            f' AND timestamp>="{yesterday.strftime(time_format)}"'
+        )
+
+        return self.logging_connection.list_entries(filter_=filter_str, page_size=1000)
+
+    def get_edges(self, existing_nodes) -> List[Edge]:
+        """
+
+        Args:
+
+        Returns:
+
+        Raises:
+
+        """
+
+        def table_string_to_table_id(table_string: str) -> Optional[TableID]:
+            table_string = table_string.split("/")
+
+            schema = table_string[3]
+            name = table_string[5]
+
+            if not any(
+                node.name == name and node.table_schema == schema
+                for node in existing_nodes
+            ):
+                return None
+
+            return TableID(
+                table_schema=schema,
+                name=name,
+                namespace=self.namespace,
+            )
+
+        edges = set()
+
+        for log in self.logs:
+            content = log.to_api_repr()
+
+            destination_table = (
+                content.get("protoPayload", {})
+                .get("metadata", {})
+                .get("jobChange", {})
+                .get("job", {})
+                .get("jobConfig", {})
+                .get("queryConfig", {})
+                .get("destinationTable")
+            ) or (
+                content.get("protoPayload", {})
+                .get("metadata", {})
+                .get("jobInsertion", {})
+                .get("job", {})
+                .get("jobConfig", {})
+                .get("queryConfig", {})
+                .get("destinationTable")
+            )
+
+            if destination_table is None:
+                continue
+
+            destination = table_string_to_table_id(destination_table)
+
+            if destination is None:
+                continue
+
+            referenced_tables = (
+                content.get("protoPayload", {})
+                .get("metadata", {})
+                .get("jobChange", {})
+                .get("job", {})
+                .get("jobStats", {})
+                .get("queryStats", {})
+                .get("referencedTables", [])
+            ) or (
+                content.get("protoPayload", {})
+                .get("metadata", {})
+                .get("jobInsertion", {})
+                .get("job", {})
+                .get("jobStats", {})
+                .get("queryStats", {})
+                .get("referencedTables", [])
+            )
+
+            for table in referenced_tables:
+                if destination_table == table:
+                    continue
+
+                source = table_string_to_table_id(table)
+
+                if source is None:
+                    continue
+
+                edges.add(
+                    Edge(
+                        constraint_type=Constraint("bqm"),
+                        source=source,
+                        destination=destination,
+                    )
+                )
+
+        return list(edges)
+
+    def get_nodes_and_edges(self) -> Tuple[List[BigqueryNode], List[Edge]]:
+        nodes = super().get_nodes()
+        edges = super().get_edges()
+
+        bigquery_edges = self.get_edges(nodes)
+
+        return nodes, edges + bigquery_edges
```

### Comparing `grai_source_bigquery-0.1.0a1/src/grai_source_bigquery/models.py` & `grai_source_bigquery-0.1.0a2/src/grai_source_bigquery/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,15 +160,20 @@
         """
 
         Returns:
 
         Raises:
 
         """
-        return hash((self.source.full_name, self.destination.full_name, self.constraint_type))
+        return hash(
+            (
+                (self.source.namespace, self.source.full_name),
+                (self.destination.namespace, self.destination.full_name),
+            )
+        )
 
 
 class TableType(str, Enum):
     """ """
 
     Table = "BASE TABLE"
     Clone = "CLONE"
```

### Comparing `grai_source_bigquery-0.1.0a1/PKG-INFO` & `grai_source_bigquery-0.1.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grai-source-bigquery
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Edward Louth
 Author-email: edward@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

