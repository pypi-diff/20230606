# Comparing `tmp/watchmen_lineage-16.5.3.tar.gz` & `tmp/watchmen_lineage-16.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_lineage-16.5.3.tar", max compression
+gzip compressed data, was "watchmen_lineage-16.5.4.tar", max compression
```

## Comparing `watchmen_lineage-16.5.3.tar` & `watchmen_lineage-16.5.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1061 2023-06-05 01:29:03.516123 watchmen_lineage-16.5.3/LICENSE
--rw-r--r--   0        0        0       46 2023-06-05 01:29:03.516123 watchmen_lineage-16.5.3/README.md
--rw-r--r--   0        0        0      633 2023-06-05 01:29:03.516123 watchmen_lineage-16.5.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-05 01:29:03.516123 watchmen_lineage-16.5.3/src/watchmen_lineage/__init__.py
--rw-r--r--   0        0        0     1369 2023-06-05 01:29:03.516123 watchmen_lineage-16.5.3/src/watchmen_lineage/index.py
--rw-r--r--   0        0        0      548 2023-06-05 01:29:03.516123 watchmen_lineage-16.5.3/src/watchmen_lineage/lineage_setting.py
--rw-r--r--   0        0        0        0 2023-06-05 01:29:03.516123 watchmen_lineage-16.5.3/src/watchmen_lineage/ml/__init__.py
--rw-r--r--   0        0        0      911 2023-06-05 01:29:03.516123 watchmen_lineage-16.5.3/src/watchmen_lineage/ml/mapping_similar.py
--rw-r--r--   0        0        0        0 2023-06-05 01:29:03.516123 watchmen_lineage-16.5.3/src/watchmen_lineage/model/__init__.py
--rw-r--r--   0        0        0      676 2023-06-05 01:29:03.516123 watchmen_lineage-16.5.3/src/watchmen_lineage/model/ast.py
--rw-r--r--   0        0        0     5521 2023-06-05 01:29:03.516123 watchmen_lineage-16.5.3/src/watchmen_lineage/model/lineage.py
--rw-r--r--   0        0        0        0 2023-06-05 01:29:03.516123 watchmen_lineage-16.5.3/src/watchmen_lineage/router/__init__.py
--rw-r--r--   0        0        0     1564 2023-06-05 01:29:03.516123 watchmen_lineage-16.5.3/src/watchmen_lineage/router/lineage_router.py
--rw-r--r--   0        0        0        0 2023-06-05 01:29:03.516123 watchmen_lineage-16.5.3/src/watchmen_lineage/service/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 01:29:03.516123 watchmen_lineage-16.5.3/src/watchmen_lineage/service/builder/__init__.py
--rw-r--r--   0        0        0     4777 2023-06-05 01:29:03.516123 watchmen_lineage-16.5.3/src/watchmen_lineage/service/builder/graphic_builder.py
--rw-r--r--   0        0        0     1179 2023-06-05 01:29:03.516123 watchmen_lineage-16.5.3/src/watchmen_lineage/service/builder/index.py
--rw-r--r--   0        0        0     5696 2023-06-05 01:29:03.516123 watchmen_lineage-16.5.3/src/watchmen_lineage/service/builder/indicator_lineage.py
--rw-r--r--   0        0        0      581 2023-06-05 01:29:03.516123 watchmen_lineage-16.5.3/src/watchmen_lineage/service/builder/loader.py
--rw-r--r--   0        0        0    10390 2023-06-05 01:29:03.516123 watchmen_lineage-16.5.3/src/watchmen_lineage/service/builder/objective_lineage.py
--rw-r--r--   0        0        0     7469 2023-06-05 01:29:03.516123 watchmen_lineage-16.5.3/src/watchmen_lineage/service/builder/pipeline_lineage.py
--rw-r--r--   0        0        0     6522 2023-06-05 01:29:03.516123 watchmen_lineage-16.5.3/src/watchmen_lineage/service/builder/subject_lineage.py
--rw-r--r--   0        0        0     2896 2023-06-05 01:29:03.516123 watchmen_lineage-16.5.3/src/watchmen_lineage/service/builder/topic_lineage.py
--rw-r--r--   0        0        0      291 2023-06-05 01:29:03.516123 watchmen_lineage-16.5.3/src/watchmen_lineage/service/compute_service.py
--rw-r--r--   0        0        0     1027 2023-06-05 01:29:03.516123 watchmen_lineage-16.5.3/src/watchmen_lineage/service/lineage_cache.py
--rw-r--r--   0        0        0    12850 2023-06-05 01:29:03.516123 watchmen_lineage-16.5.3/src/watchmen_lineage/service/lineage_service.py
--rw-r--r--   0        0        0        0 2023-06-05 01:29:03.516123 watchmen_lineage-16.5.3/src/watchmen_lineage/service/memory/__init__.py
--rw-r--r--   0        0        0      141 2023-06-05 01:29:03.516123 watchmen_lineage-16.5.3/src/watchmen_lineage/service/memory/memory_compute_service.py
--rw-r--r--   0        0        0        0 2023-06-05 01:29:03.516123 watchmen_lineage-16.5.3/src/watchmen_lineage/service/table/__init__.py
--rw-r--r--   0        0        0      140 2023-06-05 01:29:03.516123 watchmen_lineage-16.5.3/src/watchmen_lineage/service/table/table_compute_service.py
--rw-r--r--   0        0        0        0 2023-06-05 01:29:03.516123 watchmen_lineage-16.5.3/src/watchmen_lineage/storage/__init__.py
--rw-r--r--   0        0        0      247 2023-06-05 01:29:03.516123 watchmen_lineage-16.5.3/src/watchmen_lineage/storage/lineage_storage.py
--rw-r--r--   0        0        0        0 2023-06-05 01:29:03.516123 watchmen_lineage-16.5.3/src/watchmen_lineage/utils/__init__.py
--rw-r--r--   0        0        0     7971 2023-06-05 01:29:03.516123 watchmen_lineage-16.5.3/src/watchmen_lineage/utils/constant_utils.py
--rw-r--r--   0        0        0     1991 2023-06-05 01:29:03.516123 watchmen_lineage-16.5.3/src/watchmen_lineage/utils/id_utils.py
--rw-r--r--   0        0        0     1453 2023-06-05 01:29:03.516123 watchmen_lineage-16.5.3/src/watchmen_lineage/utils/size_utils.py
--rw-r--r--   0        0        0    11880 2023-06-05 01:29:03.516123 watchmen_lineage-16.5.3/src/watchmen_lineage/utils/utils.py
--rw-r--r--   0        0        0      782 1970-01-01 00:00:00.000000 watchmen_lineage-16.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/LICENSE
+-rw-r--r--   0        0        0       46 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/README.md
+-rw-r--r--   0        0        0      633 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/src/watchmen_lineage/__init__.py
+-rw-r--r--   0        0        0     1369 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/src/watchmen_lineage/index.py
+-rw-r--r--   0        0        0      548 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/src/watchmen_lineage/lineage_setting.py
+-rw-r--r--   0        0        0        0 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/src/watchmen_lineage/ml/__init__.py
+-rw-r--r--   0        0        0      911 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/src/watchmen_lineage/ml/mapping_similar.py
+-rw-r--r--   0        0        0        0 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/src/watchmen_lineage/model/__init__.py
+-rw-r--r--   0        0        0      676 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/src/watchmen_lineage/model/ast.py
+-rw-r--r--   0        0        0     5521 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/src/watchmen_lineage/model/lineage.py
+-rw-r--r--   0        0        0        0 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/src/watchmen_lineage/router/__init__.py
+-rw-r--r--   0        0        0     1564 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/src/watchmen_lineage/router/lineage_router.py
+-rw-r--r--   0        0        0        0 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/src/watchmen_lineage/service/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/src/watchmen_lineage/service/builder/__init__.py
+-rw-r--r--   0        0        0     4777 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/src/watchmen_lineage/service/builder/graphic_builder.py
+-rw-r--r--   0        0        0     1179 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/src/watchmen_lineage/service/builder/index.py
+-rw-r--r--   0        0        0     5696 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/src/watchmen_lineage/service/builder/indicator_lineage.py
+-rw-r--r--   0        0        0      581 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/src/watchmen_lineage/service/builder/loader.py
+-rw-r--r--   0        0        0    10390 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/src/watchmen_lineage/service/builder/objective_lineage.py
+-rw-r--r--   0        0        0     7469 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/src/watchmen_lineage/service/builder/pipeline_lineage.py
+-rw-r--r--   0        0        0     6522 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/src/watchmen_lineage/service/builder/subject_lineage.py
+-rw-r--r--   0        0        0     2896 2023-06-06 01:45:59.129402 watchmen_lineage-16.5.4/src/watchmen_lineage/service/builder/topic_lineage.py
+-rw-r--r--   0        0        0      291 2023-06-06 01:45:59.133402 watchmen_lineage-16.5.4/src/watchmen_lineage/service/compute_service.py
+-rw-r--r--   0        0        0     1027 2023-06-06 01:45:59.133402 watchmen_lineage-16.5.4/src/watchmen_lineage/service/lineage_cache.py
+-rw-r--r--   0        0        0    12850 2023-06-06 01:45:59.133402 watchmen_lineage-16.5.4/src/watchmen_lineage/service/lineage_service.py
+-rw-r--r--   0        0        0        0 2023-06-06 01:45:59.133402 watchmen_lineage-16.5.4/src/watchmen_lineage/service/memory/__init__.py
+-rw-r--r--   0        0        0      141 2023-06-06 01:45:59.133402 watchmen_lineage-16.5.4/src/watchmen_lineage/service/memory/memory_compute_service.py
+-rw-r--r--   0        0        0        0 2023-06-06 01:45:59.133402 watchmen_lineage-16.5.4/src/watchmen_lineage/service/table/__init__.py
+-rw-r--r--   0        0        0      140 2023-06-06 01:45:59.133402 watchmen_lineage-16.5.4/src/watchmen_lineage/service/table/table_compute_service.py
+-rw-r--r--   0        0        0        0 2023-06-06 01:45:59.133402 watchmen_lineage-16.5.4/src/watchmen_lineage/storage/__init__.py
+-rw-r--r--   0        0        0      247 2023-06-06 01:45:59.133402 watchmen_lineage-16.5.4/src/watchmen_lineage/storage/lineage_storage.py
+-rw-r--r--   0        0        0        0 2023-06-06 01:45:59.133402 watchmen_lineage-16.5.4/src/watchmen_lineage/utils/__init__.py
+-rw-r--r--   0        0        0     7971 2023-06-06 01:45:59.133402 watchmen_lineage-16.5.4/src/watchmen_lineage/utils/constant_utils.py
+-rw-r--r--   0        0        0     1991 2023-06-06 01:45:59.133402 watchmen_lineage-16.5.4/src/watchmen_lineage/utils/id_utils.py
+-rw-r--r--   0        0        0     1453 2023-06-06 01:45:59.133402 watchmen_lineage-16.5.4/src/watchmen_lineage/utils/size_utils.py
+-rw-r--r--   0        0        0    11880 2023-06-06 01:45:59.133402 watchmen_lineage-16.5.4/src/watchmen_lineage/utils/utils.py
+-rw-r--r--   0        0        0      782 1970-01-01 00:00:00.000000 watchmen_lineage-16.5.4/PKG-INFO
```

### Comparing `watchmen_lineage-16.5.3/LICENSE` & `watchmen_lineage-16.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.3/src/watchmen_lineage/index.py` & `watchmen_lineage-16.5.4/src/watchmen_lineage/index.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.3/src/watchmen_lineage/lineage_setting.py` & `watchmen_lineage-16.5.4/src/watchmen_lineage/lineage_setting.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.3/src/watchmen_lineage/ml/mapping_similar.py` & `watchmen_lineage-16.5.4/src/watchmen_lineage/ml/mapping_similar.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.3/src/watchmen_lineage/model/ast.py` & `watchmen_lineage-16.5.4/src/watchmen_lineage/model/ast.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.3/src/watchmen_lineage/model/lineage.py` & `watchmen_lineage-16.5.4/src/watchmen_lineage/model/lineage.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.3/src/watchmen_lineage/router/lineage_router.py` & `watchmen_lineage-16.5.4/src/watchmen_lineage/router/lineage_router.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.3/src/watchmen_lineage/service/builder/graphic_builder.py` & `watchmen_lineage-16.5.4/src/watchmen_lineage/service/builder/graphic_builder.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.3/src/watchmen_lineage/service/builder/index.py` & `watchmen_lineage-16.5.4/src/watchmen_lineage/service/builder/index.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.3/src/watchmen_lineage/service/builder/indicator_lineage.py` & `watchmen_lineage-16.5.4/src/watchmen_lineage/service/builder/indicator_lineage.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.3/src/watchmen_lineage/service/builder/loader.py` & `watchmen_lineage-16.5.4/src/watchmen_lineage/service/builder/loader.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.3/src/watchmen_lineage/service/builder/objective_lineage.py` & `watchmen_lineage-16.5.4/src/watchmen_lineage/service/builder/objective_lineage.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.3/src/watchmen_lineage/service/builder/pipeline_lineage.py` & `watchmen_lineage-16.5.4/src/watchmen_lineage/service/builder/pipeline_lineage.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.3/src/watchmen_lineage/service/builder/subject_lineage.py` & `watchmen_lineage-16.5.4/src/watchmen_lineage/service/builder/subject_lineage.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.3/src/watchmen_lineage/service/builder/topic_lineage.py` & `watchmen_lineage-16.5.4/src/watchmen_lineage/service/builder/topic_lineage.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.3/src/watchmen_lineage/service/lineage_cache.py` & `watchmen_lineage-16.5.4/src/watchmen_lineage/service/lineage_cache.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.3/src/watchmen_lineage/service/lineage_service.py` & `watchmen_lineage-16.5.4/src/watchmen_lineage/service/lineage_service.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.3/src/watchmen_lineage/utils/constant_utils.py` & `watchmen_lineage-16.5.4/src/watchmen_lineage/utils/constant_utils.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.3/src/watchmen_lineage/utils/id_utils.py` & `watchmen_lineage-16.5.4/src/watchmen_lineage/utils/id_utils.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.3/src/watchmen_lineage/utils/size_utils.py` & `watchmen_lineage-16.5.4/src/watchmen_lineage/utils/size_utils.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.3/src/watchmen_lineage/utils/utils.py` & `watchmen_lineage-16.5.4/src/watchmen_lineage/utils/utils.py`

 * *Files identical despite different names*

### Comparing `watchmen_lineage-16.5.3/PKG-INFO` & `watchmen_lineage-16.5.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: watchmen-lineage
-Version: 16.5.3
+Version: 16.5.4
 Summary: 
 Author: luke0623
 Author-email: luke0623@outlook.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: networkx (>=2.8.8,<3.0.0)
-Requires-Dist: watchmen-data-surface (==16.5.3)
-Requires-Dist: watchmen-indicator-surface (==16.5.3)
-Requires-Dist: watchmen-inquiry-surface (==16.5.3)
-Requires-Dist: watchmen-inquiry-trino (==16.5.3)
-Requires-Dist: watchmen-pipeline-surface (==16.5.3)
-Requires-Dist: watchmen-storage-mysql (==16.5.3)
+Requires-Dist: watchmen-data-surface (==16.5.4)
+Requires-Dist: watchmen-indicator-surface (==16.5.4)
+Requires-Dist: watchmen-inquiry-surface (==16.5.4)
+Requires-Dist: watchmen-inquiry-trino (==16.5.4)
+Requires-Dist: watchmen-pipeline-surface (==16.5.4)
+Requires-Dist: watchmen-storage-mysql (==16.5.4)
 Description-Content-Type: text/markdown
 
 # Watchmen Lineage
 
 Lineage of _**Watchmen**_.
```

