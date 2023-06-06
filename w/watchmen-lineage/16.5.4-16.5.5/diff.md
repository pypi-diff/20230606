# Comparing `tmp/watchmen_lineage-16.5.4.tar.gz` & `tmp/watchmen_lineage-16.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_lineage-16.5.4.tar", max compression
+gzip compressed data, was "watchmen_lineage-16.5.5.tar", max compression
```

## Comparing `watchmen_lineage-16.5.4.tar` & `watchmen_lineage-16.5.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1061 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/LICENSE
--rw-r--r--   0        0        0       46 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/README.md
--rw-r--r--   0        0        0      633 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/src/watchmen_lineage/__init__.py
--rw-r--r--   0        0        0     1369 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/src/watchmen_lineage/index.py
--rw-r--r--   0        0        0      548 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/src/watchmen_lineage/lineage_setting.py
--rw-r--r--   0        0        0        0 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/src/watchmen_lineage/ml/__init__.py
--rw-r--r--   0        0        0      911 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/src/watchmen_lineage/ml/mapping_similar.py
--rw-r--r--   0        0        0        0 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/src/watchmen_lineage/model/__init__.py
--rw-r--r--   0        0        0      676 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/src/watchmen_lineage/model/ast.py
--rw-r--r--   0        0        0     5521 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/src/watchmen_lineage/model/lineage.py
--rw-r--r--   0        0        0        0 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/src/watchmen_lineage/router/__init__.py
--rw-r--r--   0        0        0     1564 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/src/watchmen_lineage/router/lineage_router.py
--rw-r--r--   0        0        0        0 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/src/watchmen_lineage/service/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/src/watchmen_lineage/service/builder/__init__.py
--rw-r--r--   0        0        0     4777 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/src/watchmen_lineage/service/builder/graphic_builder.py
--rw-r--r--   0        0        0     1179 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/src/watchmen_lineage/service/builder/index.py
--rw-r--r--   0        0        0     5696 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/src/watchmen_lineage/service/builder/indicator_lineage.py
--rw-r--r--   0        0        0      581 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/src/watchmen_lineage/service/builder/loader.py
--rw-r--r--   0        0        0    10390 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/src/watchmen_lineage/service/builder/objective_lineage.py
--rw-r--r--   0        0        0     7469 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/src/watchmen_lineage/service/builder/pipeline_lineage.py
--rw-r--r--   0        0        0     6522 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/src/watchmen_lineage/service/builder/subject_lineage.py
--rw-r--r--   0        0        0     2896 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/src/watchmen_lineage/service/builder/topic_lineage.py
--rw-r--r--   0        0        0      291 2023-06-06 01:45:59.133402 watchmen_lineage-16.5.4/src/watchmen_lineage/service/compute_service.py
--rw-r--r--   0        0        0     1027 2023-06-06 01:45:59.133402 watchmen_lineage-16.5.4/src/watchmen_lineage/service/lineage_cache.py
--rw-r--r--   0        0        0    12850 2023-06-06 01:45:59.133402 watchmen_lineage-16.5.4/src/watchmen_lineage/service/lineage_service.py
--rw-r--r--   0        0        0        0 2023-06-06 01:45:59.133402 watchmen_lineage-16.5.4/src/watchmen_lineage/service/memory/__init__.py
--rw-r--r--   0        0        0      141 2023-06-06 01:45:59.133402 watchmen_lineage-16.5.4/src/watchmen_lineage/service/memory/memory_compute_service.py
--rw-r--r--   0        0        0        0 2023-06-06 01:45:59.133402 watchmen_lineage-16.5.4/src/watchmen_lineage/service/table/__init__.py
--rw-r--r--   0        0        0      140 2023-06-06 01:45:59.133402 watchmen_lineage-16.5.4/src/watchmen_lineage/service/table/table_compute_service.py
--rw-r--r--   0        0        0        0 2023-06-06 01:45:59.133402 watchmen_lineage-16.5.4/src/watchmen_lineage/storage/__init__.py
--rw-r--r--   0        0        0      247 2023-06-06 01:45:59.133402 watchmen_lineage-16.5.4/src/watchmen_lineage/storage/lineage_storage.py
--rw-r--r--   0        0        0        0 2023-06-06 01:45:59.133402 watchmen_lineage-16.5.4/src/watchmen_lineage/utils/__init__.py
--rw-r--r--   0        0        0     7971 2023-06-06 01:45:59.133402 watchmen_lineage-16.5.4/src/watchmen_lineage/utils/constant_utils.py
--rw-r--r--   0        0        0     1991 2023-06-06 01:45:59.133402 watchmen_lineage-16.5.4/src/watchmen_lineage/utils/id_utils.py
--rw-r--r--   0        0        0     1453 2023-06-06 01:45:59.133402 watchmen_lineage-16.5.4/src/watchmen_lineage/utils/size_utils.py
--rw-r--r--   0        0        0    11880 2023-06-06 01:45:59.133402 watchmen_lineage-16.5.4/src/watchmen_lineage/utils/utils.py
--rw-r--r--   0        0        0      782 1970-01-01 00:00:00.000000 watchmen_lineage-16.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-06 07:52:17.089011 watchmen_lineage-16.5.5/LICENSE
+-rw-r--r--   0        0        0       46 2023-06-06 07:52:17.093011 watchmen_lineage-16.5.5/README.md
+-rw-r--r--   0        0        0      633 2023-06-06 07:52:17.093011 watchmen_lineage-16.5.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-06 07:52:17.093011 watchmen_lineage-16.5.5/src/watchmen_lineage/__init__.py
+-rw-r--r--   0        0        0     1371 2023-06-06 07:52:17.093011 watchmen_lineage-16.5.5/src/watchmen_lineage/index.py
+-rw-r--r--   0        0        0      548 2023-06-06 07:52:17.093011 watchmen_lineage-16.5.5/src/watchmen_lineage/lineage_setting.py
+-rw-r--r--   0        0        0        0 2023-06-06 07:52:17.093011 watchmen_lineage-16.5.5/src/watchmen_lineage/ml/__init__.py
+-rw-r--r--   0        0        0      911 2023-06-06 07:52:17.093011 watchmen_lineage-16.5.5/src/watchmen_lineage/ml/mapping_similar.py
+-rw-r--r--   0        0        0        0 2023-06-06 07:52:17.093011 watchmen_lineage-16.5.5/src/watchmen_lineage/model/__init__.py
+-rw-r--r--   0        0        0      676 2023-06-06 07:52:17.093011 watchmen_lineage-16.5.5/src/watchmen_lineage/model/ast.py
+-rw-r--r--   0        0        0     5521 2023-06-06 07:52:17.093011 watchmen_lineage-16.5.5/src/watchmen_lineage/model/lineage.py
+-rw-r--r--   0        0        0        0 2023-06-06 07:52:17.093011 watchmen_lineage-16.5.5/src/watchmen_lineage/router/__init__.py
+-rw-r--r--   0        0        0     1564 2023-06-06 07:52:17.093011 watchmen_lineage-16.5.5/src/watchmen_lineage/router/lineage_router.py
+-rw-r--r--   0        0        0        0 2023-06-06 07:52:17.093011 watchmen_lineage-16.5.5/src/watchmen_lineage/service/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 07:52:17.093011 watchmen_lineage-16.5.5/src/watchmen_lineage/service/builder/__init__.py
+-rw-r--r--   0        0        0     4777 2023-06-06 07:52:17.093011 watchmen_lineage-16.5.5/src/watchmen_lineage/service/builder/graphic_builder.py
+-rw-r--r--   0        0        0     1179 2023-06-06 07:52:17.093011 watchmen_lineage-16.5.5/src/watchmen_lineage/service/builder/index.py
+-rw-r--r--   0        0        0     5696 2023-06-06 07:52:17.093011 watchmen_lineage-16.5.5/src/watchmen_lineage/service/builder/indicator_lineage.py
+-rw-r--r--   0        0        0      581 2023-06-06 07:52:17.093011 watchmen_lineage-16.5.5/src/watchmen_lineage/service/builder/loader.py
+-rw-r--r--   0        0        0    10390 2023-06-06 07:52:17.093011 watchmen_lineage-16.5.5/src/watchmen_lineage/service/builder/objective_lineage.py
+-rw-r--r--   0        0        0     7469 2023-06-06 07:52:17.093011 watchmen_lineage-16.5.5/src/watchmen_lineage/service/builder/pipeline_lineage.py
+-rw-r--r--   0        0        0     6522 2023-06-06 07:52:17.093011 watchmen_lineage-16.5.5/src/watchmen_lineage/service/builder/subject_lineage.py
+-rw-r--r--   0        0        0     2896 2023-06-06 07:52:17.093011 watchmen_lineage-16.5.5/src/watchmen_lineage/service/builder/topic_lineage.py
+-rw-r--r--   0        0        0      291 2023-06-06 07:52:17.093011 watchmen_lineage-16.5.5/src/watchmen_lineage/service/compute_service.py
+-rw-r--r--   0        0        0     1027 2023-06-06 07:52:17.093011 watchmen_lineage-16.5.5/src/watchmen_lineage/service/lineage_cache.py
+-rw-r--r--   0        0        0    12852 2023-06-06 07:52:17.093011 watchmen_lineage-16.5.5/src/watchmen_lineage/service/lineage_service.py
+-rw-r--r--   0        0        0        0 2023-06-06 07:52:17.093011 watchmen_lineage-16.5.5/src/watchmen_lineage/service/memory/__init__.py
+-rw-r--r--   0        0        0      141 2023-06-06 07:52:17.093011 watchmen_lineage-16.5.5/src/watchmen_lineage/service/memory/memory_compute_service.py
+-rw-r--r--   0        0        0        0 2023-06-06 07:52:17.093011 watchmen_lineage-16.5.5/src/watchmen_lineage/service/table/__init__.py
+-rw-r--r--   0        0        0      140 2023-06-06 07:52:17.093011 watchmen_lineage-16.5.5/src/watchmen_lineage/service/table/table_compute_service.py
+-rw-r--r--   0        0        0        0 2023-06-06 07:52:17.093011 watchmen_lineage-16.5.5/src/watchmen_lineage/storage/__init__.py
+-rw-r--r--   0        0        0      247 2023-06-06 07:52:17.093011 watchmen_lineage-16.5.5/src/watchmen_lineage/storage/lineage_storage.py
+-rw-r--r--   0        0        0        0 2023-06-06 07:52:17.093011 watchmen_lineage-16.5.5/src/watchmen_lineage/utils/__init__.py
+-rw-r--r--   0        0        0     7971 2023-06-06 07:52:17.093011 watchmen_lineage-16.5.5/src/watchmen_lineage/utils/constant_utils.py
+-rw-r--r--   0        0        0     1991 2023-06-06 07:52:17.093011 watchmen_lineage-16.5.5/src/watchmen_lineage/utils/id_utils.py
+-rw-r--r--   0        0        0     1453 2023-06-06 07:52:17.093011 watchmen_lineage-16.5.5/src/watchmen_lineage/utils/size_utils.py
+-rw-r--r--   0        0        0    11880 2023-06-06 07:52:17.093011 watchmen_lineage-16.5.5/src/watchmen_lineage/utils/utils.py
+-rw-r--r--   0        0        0      782 1970-01-01 00:00:00.000000 watchmen_lineage-16.5.5/PKG-INFO
```

### Comparing `watchmen_lineage-16.5.4/LICENSE` & `watchmen_lineage-16.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.4/pyproject.toml` & `watchmen_lineage-16.5.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "watchmen-lineage"
-version = "16.5.4"
+version = "16.5.5"
 description = ""
 authors = ["luke0623 <luke0623@outlook.com>"]
 readme = "README.md"
 packages = [
     { include = "watchmen_lineage", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-watchmen-data-surface = "16.5.4"
-watchmen-pipeline-surface = "16.5.4"
-watchmen-inquiry-surface = "16.5.4"
-watchmen-inquiry-trino = { version = "16.5.4", optional = true }
-watchmen-indicator-surface = "16.5.4"
-watchmen-storage-mysql = { version = "16.5.4", optional = true }
+watchmen-data-surface = "16.5.5"
+watchmen-pipeline-surface = "16.5.5"
+watchmen-inquiry-surface = "16.5.5"
+watchmen-inquiry-trino = { version = "16.5.5", optional = true }
+watchmen-indicator-surface = "16.5.5"
+watchmen-storage-mysql = { version = "16.5.5", optional = true }
 networkx = "^2.8.8"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `watchmen_lineage-16.5.4/src/watchmen_lineage/index.py` & `watchmen_lineage-16.5.5/src/watchmen_lineage/index.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 principal_service: PrincipalService = fake_tenant_admin("1047472206839607296")
 
 lineage_service.init_tenant_all_lineage_data(principal_service)
 
 lineage_service.graph_json(principal_service)
 
 
-print(lineage_service.load_relevant_indicators("1078711287888358400",principal_service))
+# print(lineage_service.load_relevant_indicators("1078711287888358400",principal_service))
 
 # result = lineage_service.fine_lineage_by_factor("963837989900259328", "6270b3713bee4d1db483db37c8734ff0",
 #                                                 principal_service)
```

### Comparing `watchmen_lineage-16.5.4/src/watchmen_lineage/lineage_setting.py` & `watchmen_lineage-16.5.5/src/watchmen_lineage/lineage_setting.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.4/src/watchmen_lineage/ml/mapping_similar.py` & `watchmen_lineage-16.5.5/src/watchmen_lineage/ml/mapping_similar.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.4/src/watchmen_lineage/model/ast.py` & `watchmen_lineage-16.5.5/src/watchmen_lineage/model/ast.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.4/src/watchmen_lineage/model/lineage.py` & `watchmen_lineage-16.5.5/src/watchmen_lineage/model/lineage.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.4/src/watchmen_lineage/router/lineage_router.py` & `watchmen_lineage-16.5.5/src/watchmen_lineage/router/lineage_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.4/src/watchmen_lineage/service/builder/graphic_builder.py` & `watchmen_lineage-16.5.5/src/watchmen_lineage/service/builder/graphic_builder.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.4/src/watchmen_lineage/service/builder/index.py` & `watchmen_lineage-16.5.5/src/watchmen_lineage/service/builder/index.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.4/src/watchmen_lineage/service/builder/indicator_lineage.py` & `watchmen_lineage-16.5.5/src/watchmen_lineage/service/builder/indicator_lineage.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.4/src/watchmen_lineage/service/builder/loader.py` & `watchmen_lineage-16.5.5/src/watchmen_lineage/service/builder/loader.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.4/src/watchmen_lineage/service/builder/objective_lineage.py` & `watchmen_lineage-16.5.5/src/watchmen_lineage/service/builder/objective_lineage.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.4/src/watchmen_lineage/service/builder/pipeline_lineage.py` & `watchmen_lineage-16.5.5/src/watchmen_lineage/service/builder/pipeline_lineage.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.4/src/watchmen_lineage/service/builder/subject_lineage.py` & `watchmen_lineage-16.5.5/src/watchmen_lineage/service/builder/subject_lineage.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.4/src/watchmen_lineage/service/builder/topic_lineage.py` & `watchmen_lineage-16.5.5/src/watchmen_lineage/service/builder/topic_lineage.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.4/src/watchmen_lineage/service/lineage_cache.py` & `watchmen_lineage-16.5.5/src/watchmen_lineage/service/lineage_cache.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.4/src/watchmen_lineage/service/lineage_service.py` & `watchmen_lineage-16.5.5/src/watchmen_lineage/service/lineage_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,15 +231,15 @@
 	@staticmethod
 	def __get_node(graphic: MultiDiGraph, node_id: str):
 		return graphic.nodes[node_id]
 
 	def graph_json(self, principal_service: PrincipalService):
 		graphic = self.get_graph_by_tenant(principal_service)
 		graph_json = nx.node_link_data(graphic)
-		print(graph_json)
+		# print(graph_json)
 		return graph_json
 
 	def build_partial_lineage(self, model: BaseModel, lineage_type: LineageType, principal_service: PrincipalService):
 
 		tenant_node_graph: MultiDiGraph = self.get_graph_by_tenant(principal_service)
 		builder: LineageBuilder = get_builder(lineage_type)
 		builder.build_partial(tenant_node_graph, model)
```

### Comparing `watchmen_lineage-16.5.4/src/watchmen_lineage/utils/constant_utils.py` & `watchmen_lineage-16.5.5/src/watchmen_lineage/utils/constant_utils.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.4/src/watchmen_lineage/utils/id_utils.py` & `watchmen_lineage-16.5.5/src/watchmen_lineage/utils/id_utils.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.4/src/watchmen_lineage/utils/size_utils.py` & `watchmen_lineage-16.5.5/src/watchmen_lineage/utils/size_utils.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.4/src/watchmen_lineage/utils/utils.py` & `watchmen_lineage-16.5.5/src/watchmen_lineage/utils/utils.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.4/PKG-INFO` & `watchmen_lineage-16.5.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: watchmen-lineage
-Version: 16.5.4
+Version: 16.5.5
 Summary: 
 Author: luke0623
 Author-email: luke0623@outlook.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: networkx (>=2.8.8,<3.0.0)
-Requires-Dist: watchmen-data-surface (==16.5.4)
-Requires-Dist: watchmen-indicator-surface (==16.5.4)
-Requires-Dist: watchmen-inquiry-surface (==16.5.4)
-Requires-Dist: watchmen-inquiry-trino (==16.5.4)
-Requires-Dist: watchmen-pipeline-surface (==16.5.4)
-Requires-Dist: watchmen-storage-mysql (==16.5.4)
+Requires-Dist: watchmen-data-surface (==16.5.5)
+Requires-Dist: watchmen-indicator-surface (==16.5.5)
+Requires-Dist: watchmen-inquiry-surface (==16.5.5)
+Requires-Dist: watchmen-inquiry-trino (==16.5.5)
+Requires-Dist: watchmen-pipeline-surface (==16.5.5)
+Requires-Dist: watchmen-storage-mysql (==16.5.5)
 Description-Content-Type: text/markdown
 
 # Watchmen Lineage
 
 Lineage of _**Watchmen**_.
```

