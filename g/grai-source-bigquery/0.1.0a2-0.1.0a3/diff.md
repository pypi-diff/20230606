# Comparing `tmp/grai_source_bigquery-0.1.0a2.tar.gz` & `tmp/grai_source_bigquery-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grai_source_bigquery-0.1.0a2.tar", max compression
+gzip compressed data, was "grai_source_bigquery-0.1.0a3.tar", max compression
```

## Comparing `grai_source_bigquery-0.1.0a2.tar` & `grai_source_bigquery-0.1.0a3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      141 2023-05-02 08:01:59.695304 grai_source_bigquery-0.1.0a2/README.md
--rw-r--r--   0        0        0      971 2023-06-06 07:58:43.719920 grai_source_bigquery-0.1.0a2/pyproject.toml
--rw-r--r--   0        0        0      145 2023-02-14 12:06:39.088033 grai_source_bigquery-0.1.0a2/src/grai_source_bigquery/__init__.py
--rw-r--r--   0        0        0     8578 2023-06-02 08:26:06.787907 grai_source_bigquery-0.1.0a2/src/grai_source_bigquery/adapters.py
--rw-r--r--   0        0        0     2124 2023-06-05 14:56:39.992488 grai_source_bigquery-0.1.0a2/src/grai_source_bigquery/base.py
--rw-r--r--   0        0        0    13309 2023-06-05 17:43:32.597569 grai_source_bigquery-0.1.0a2/src/grai_source_bigquery/loader.py
--rw-r--r--   0        0        0     6222 2023-06-05 17:34:49.806426 grai_source_bigquery-0.1.0a2/src/grai_source_bigquery/models.py
--rw-r--r--   0        0        0      199 2023-06-02 08:26:06.789100 grai_source_bigquery-0.1.0a2/src/grai_source_bigquery/package_definitions.py
--rw-r--r--   0        0        0     1169 1970-01-01 00:00:00.000000 grai_source_bigquery-0.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0      141 2023-05-02 08:01:59.695304 grai_source_bigquery-0.1.0a3/README.md
+-rw-r--r--   0        0        0      971 2023-06-06 08:43:35.422679 grai_source_bigquery-0.1.0a3/pyproject.toml
+-rw-r--r--   0        0        0      145 2023-02-14 12:06:39.088033 grai_source_bigquery-0.1.0a3/src/grai_source_bigquery/__init__.py
+-rw-r--r--   0        0        0     8578 2023-06-02 08:26:06.787907 grai_source_bigquery-0.1.0a3/src/grai_source_bigquery/adapters.py
+-rw-r--r--   0        0        0     2106 2023-06-06 08:21:14.471667 grai_source_bigquery-0.1.0a3/src/grai_source_bigquery/base.py
+-rw-r--r--   0        0        0    13328 2023-06-06 08:42:13.747956 grai_source_bigquery-0.1.0a3/src/grai_source_bigquery/loader.py
+-rw-r--r--   0        0        0     6222 2023-06-06 08:19:27.554058 grai_source_bigquery-0.1.0a3/src/grai_source_bigquery/models.py
+-rw-r--r--   0        0        0      199 2023-06-02 08:26:06.789100 grai_source_bigquery-0.1.0a3/src/grai_source_bigquery/package_definitions.py
+-rw-r--r--   0        0        0     1169 1970-01-01 00:00:00.000000 grai_source_bigquery-0.1.0a3/PKG-INFO
```

### Comparing `grai_source_bigquery-0.1.0a2/pyproject.toml` & `grai_source_bigquery-0.1.0a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grai_source_bigquery"
-version = "0.1.0-alpha2"
+version = "0.1.0-alpha3"
 description = ""
 authors = ["Edward Louth <edward@grai.io>"]
 license = "Elastic-2.0"
 packages = [
     { include = "grai_source_bigquery", from = "src" },
 ]
 readme = "README.md"
```

### Comparing `grai_source_bigquery-0.1.0a2/src/grai_source_bigquery/adapters.py` & `grai_source_bigquery-0.1.0a3/src/grai_source_bigquery/adapters.py`

 * *Files identical despite different names*

### Comparing `grai_source_bigquery-0.1.0a2/src/grai_source_bigquery/base.py` & `grai_source_bigquery-0.1.0a3/src/grai_source_bigquery/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,53 +5,49 @@
 from grai_schemas.base import Edge, Node
 
 from grai_source_bigquery.adapters import adapt_to_client
 from grai_source_bigquery.loader import BigqueryConnector, LoggingConnector
 
 
 def get_nodes_and_edges(
-    connector: BigqueryConnector,
-    logging_connector: LoggingConnector = None,
-    version: Literal["v1"] = "v1",
+    connector: BigqueryConnector, version: Literal["v1"]
 ) -> Tuple[List[Node], List[Edge]]:
     """
 
     Args:
         connector (BigqueryConnector):
         version (Literal["v1"]):
 
     Returns:
 
     Raises:
 
     """
     if version != "v1":
-        raise NotImplementedError(f"No available implementation for client version {version}")
+        raise NotImplementedError(
+            f"No available implementation for client version {version}"
+        )
 
     with connector.connect() as conn:
         nodes, edges = conn.get_nodes_and_edges()
 
-    log_edges = []
-
-    if logging_connector is not None:
-        with logging_connector.connect() as conn:
-            log_edges = conn.get_edges(nodes)
-
     nodes = adapt_to_client(nodes, version)
-    edges = adapt_to_client(edges + log_edges, version)
+    edges = adapt_to_client(edges, version)
 
     return nodes, edges
 
 
 def update_server(
     client: BaseClient,
     namespace: Optional[str] = None,
     project: Optional[str] = None,
     dataset: Optional[Union[str, List[str]]] = None,
     credentials: Optional[str] = None,
+    log_parsing: Optional[bool] = False,
+    log_parsing_window: Optional[int] = 7,
 ) -> None:
     """
 
     Args:
         client (BaseClient):
         namespace (Optional[str], optional):  (Default value = None)
         project (Optional[str], optional):  (Default value = None)
@@ -59,23 +55,28 @@
         credentials (Optional[str], optional):  (Default value = None)
 
     Returns:
 
     Raises:
 
     """
-    conn = BigqueryConnector(
-        project=project,
-        namespace=namespace,
-        dataset=dataset,
-        credentials=credentials,
-    )
-    logging_conn = LoggingConnector(
-        project=project,
-        namespace=namespace,
-        dataset=dataset,
-        credentials=credentials,
+    conn = (
+        BigqueryConnector(
+            project=project,
+            namespace=namespace,
+            dataset=dataset,
+            credentials=credentials,
+        )
+        if not log_parsing
+        else LoggingConnector(
+            project=project,
+            namespace=namespace,
+            dataset=dataset,
+            credentials=credentials,
+            window=log_parsing_window,
+        )
     )
 
-    nodes, edges = get_nodes_and_edges(conn, logging_conn, client.id)
+    nodes, edges = get_nodes_and_edges(conn, client.id)
+
     update(client, nodes)
     update(client, edges)
```

### Comparing `grai_source_bigquery-0.1.0a2/src/grai_source_bigquery/loader.py` & `grai_source_bigquery-0.1.0a3/src/grai_source_bigquery/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -418,15 +418,15 @@
             ' AND resource.type = "bigquery_project"'
             ' AND protoPayload.methodName="google.cloud.bigquery.v2.JobService.InsertJob"'
             f' AND timestamp>="{yesterday.strftime(time_format)}"'
         )
 
         return self.logging_connection.list_entries(filter_=filter_str, page_size=1000)
 
-    def get_edges(self, existing_nodes) -> List[Edge]:
+    def get_bigquery_edges(self, existing_nodes: List[BigqueryNode]) -> List[Edge]:
         """
 
         Args:
 
         Returns:
 
         Raises:
@@ -516,13 +516,12 @@
                         destination=destination,
                     )
                 )
 
         return list(edges)
 
     def get_nodes_and_edges(self) -> Tuple[List[BigqueryNode], List[Edge]]:
-        nodes = super().get_nodes()
-        edges = super().get_edges()
+        nodes, edges = super().get_nodes_and_edges()
 
-        bigquery_edges = self.get_edges(nodes)
+        bigquery_edges = self.get_bigquery_edges(nodes)
 
         return nodes, edges + bigquery_edges
```

### Comparing `grai_source_bigquery-0.1.0a2/src/grai_source_bigquery/models.py` & `grai_source_bigquery-0.1.0a3/src/grai_source_bigquery/models.py`

 * *Files identical despite different names*

### Comparing `grai_source_bigquery-0.1.0a2/PKG-INFO` & `grai_source_bigquery-0.1.0a3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grai-source-bigquery
-Version: 0.1.0a2
+Version: 0.1.0a3
 Summary: 
 Home-page: https://www.grai.io/
 License: Elastic-2.0
 Author: Edward Louth
 Author-email: edward@grai.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
```

