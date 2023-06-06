# Comparing `tmp/encoded_core-0.0.0.1b2.tar.gz` & `tmp/encoded_core-0.0.0.1b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encoded_core-0.0.0.1b2.tar", max compression
+gzip compressed data, was "encoded_core-0.0.0.1b4.tar", max compression
```

## Comparing `encoded_core-0.0.0.1b2.tar` & `encoded_core-0.0.0.1b4.tar`

### file list

```diff
@@ -1,54 +1,57 @@
--rw-r--r--   0        0        0     1083 2023-04-28 13:49:44.781887 encoded_core-0.0.0.1b2/LICENSE
--rw-r--r--   0        0        0      174 2023-04-28 13:50:12.674541 encoded_core-0.0.0.1b2/README.rst
--rw-r--r--   0        0        0     3671 2023-05-09 14:51:36.163703 encoded_core-0.0.0.1b2/pyproject.toml
--rw-r--r--   0        0        0     2378 2023-05-01 18:24:20.274258 encoded_core-0.0.0.1b2/src/encoded_core/__init__.py
--rw-r--r--   0        0        0     4847 2023-04-28 17:14:35.491425 encoded_core-0.0.0.1b2/src/encoded_core/local_roles.py
--rw-r--r--   0        0        0     1915 2023-04-28 13:50:12.708994 encoded_core-0.0.0.1b2/src/encoded_core/schemas/document.json
--rw-r--r--   0        0        0    18925 2023-05-02 19:21:41.656041 encoded_core-0.0.0.1b2/src/encoded_core/schemas/file.json
--rw-r--r--   0        0        0     5070 2023-04-28 13:50:12.701442 encoded_core-0.0.0.1b2/src/encoded_core/schemas/file_format.json
--rw-r--r--   0        0        0     6170 2023-04-28 13:50:12.706416 encoded_core-0.0.0.1b2/src/encoded_core/schemas/file_processed.json
--rw-r--r--   0        0        0     2336 2023-04-28 13:50:12.710774 encoded_core-0.0.0.1b2/src/encoded_core/schemas/file_reference.json
--rw-r--r--   0        0        0     1331 2023-04-28 13:50:12.712368 encoded_core-0.0.0.1b2/src/encoded_core/schemas/file_submitted.json
--rw-r--r--   0        0        0     1831 2023-04-28 13:50:12.715563 encoded_core-0.0.0.1b2/src/encoded_core/schemas/higlass_view_config.json
--rw-r--r--   0        0        0     1528 2023-04-28 13:50:12.714806 encoded_core-0.0.0.1b2/src/encoded_core/schemas/image.json
--rw-r--r--   0        0        0    18352 2023-04-28 13:50:12.707283 encoded_core-0.0.0.1b2/src/encoded_core/schemas/meta_workflow.json
--rw-r--r--   0        0        0    14409 2023-04-28 13:50:12.713194 encoded_core-0.0.0.1b2/src/encoded_core/schemas/meta_workflow_run.json
--rw-r--r--   0        0        0    17295 2023-04-28 13:50:12.702288 encoded_core-0.0.0.1b2/src/encoded_core/schemas/mixins.json
--rw-r--r--   0        0        0     4581 2023-04-28 13:50:12.716243 encoded_core-0.0.0.1b2/src/encoded_core/schemas/page.json
--rw-r--r--   0        0        0     1454 2023-05-05 17:13:08.190163 encoded_core-0.0.0.1b2/src/encoded_core/schemas/quality_metric.json
--rw-r--r--   0        0        0     3228 2023-05-02 19:21:00.959543 encoded_core-0.0.0.1b2/src/encoded_core/schemas/quality_metric_generic.json
--rw-r--r--   0        0        0     5715 2023-04-28 13:50:12.713992 encoded_core-0.0.0.1b2/src/encoded_core/schemas/software.json
--rw-r--r--   0        0        0     5010 2023-04-28 13:50:12.708092 encoded_core-0.0.0.1b2/src/encoded_core/schemas/static_section.json
--rw-r--r--   0        0        0    20411 2023-04-28 13:50:12.700669 encoded_core-0.0.0.1b2/src/encoded_core/schemas/tracking_item.json
--rw-r--r--   0        0        0     3749 2023-04-28 13:50:12.703052 encoded_core-0.0.0.1b2/src/encoded_core/schemas/user_content.json
--rw-r--r--   0        0        0    28089 2023-05-02 19:08:31.618837 encoded_core-0.0.0.1b2/src/encoded_core/schemas/workflow.json
--rw-r--r--   0        0        0    10491 2023-05-02 19:07:38.780580 encoded_core-0.0.0.1b2/src/encoded_core/schemas/workflow_run.json
--rw-r--r--   0        0        0     1908 2023-04-28 13:50:12.703919 encoded_core-0.0.0.1b2/src/encoded_core/schemas/workflow_run_awsem.json
--rw-r--r--   0        0        0        0 2023-04-28 17:30:49.756296 encoded_core-0.0.0.1b2/src/encoded_core/tests/__init__.py
--rw-r--r--   0        0        0    14046 2023-05-05 16:55:24.908128 encoded_core-0.0.0.1b2/src/encoded_core/tests/conftest.py
--rw-r--r--   0        0        0     1873 2023-05-01 15:51:03.342243 encoded_core-0.0.0.1b2/src/encoded_core/tests/conftest_settings.py
--rw-r--r--   0        0        0     7765 2023-05-02 19:39:48.058091 encoded_core-0.0.0.1b2/src/encoded_core/tests/datafixtures.py
--rw-r--r--   0        0        0    10832 2023-05-02 19:39:17.806355 encoded_core-0.0.0.1b2/src/encoded_core/tests/test_types_file.py
--rw-r--r--   0        0        0      262 2023-05-02 19:36:28.328655 encoded_core-0.0.0.1b2/src/encoded_core/tests/test_types_file_format.py
--rw-r--r--   0        0        0      239 2023-05-02 19:39:17.802109 encoded_core-0.0.0.1b2/src/encoded_core/tests/test_types_meta_workflow.py
--rw-r--r--   0        0        0      212 2023-05-02 19:39:17.799579 encoded_core-0.0.0.1b2/src/encoded_core/tests/test_types_software.py
--rw-r--r--   0        0        0      502 2023-05-02 19:39:54.040945 encoded_core-0.0.0.1b2/src/encoded_core/tests/test_types_workflow.py
--rw-r--r--   0        0        0       70 2023-04-28 13:50:12.688855 encoded_core-0.0.0.1b2/src/encoded_core/types/__init__.py
--rw-r--r--   0        0        0     1290 2023-04-28 18:02:48.783979 encoded_core-0.0.0.1b2/src/encoded_core/types/document.py
--rw-r--r--   0        0        0    41353 2023-04-28 18:02:48.769257 encoded_core-0.0.0.1b2/src/encoded_core/types/file.py
--rw-r--r--   0        0        0      870 2023-04-28 18:02:48.776599 encoded_core-0.0.0.1b2/src/encoded_core/types/file_format.py
--rw-r--r--   0        0        0     2352 2023-04-28 18:02:48.779024 encoded_core-0.0.0.1b2/src/encoded_core/types/file_processed.py
--rw-r--r--   0        0        0      517 2023-04-28 18:02:48.786571 encoded_core-0.0.0.1b2/src/encoded_core/types/file_reference.py
--rw-r--r--   0        0        0     2025 2023-04-28 18:02:48.765168 encoded_core-0.0.0.1b2/src/encoded_core/types/file_submitted.py
--rw-r--r--   0        0        0      607 2023-04-28 18:02:48.793746 encoded_core-0.0.0.1b2/src/encoded_core/types/higlass_view_config.py
--rw-r--r--   0        0        0     1046 2023-04-28 18:02:48.788942 encoded_core-0.0.0.1b2/src/encoded_core/types/image.py
--rw-r--r--   0        0        0     3191 2023-04-28 18:02:48.781565 encoded_core-0.0.0.1b2/src/encoded_core/types/meta_workflow.py
--rw-r--r--   0        0        0    13688 2023-05-09 14:53:19.136309 encoded_core-0.0.0.1b2/src/encoded_core/types/page.py
--rw-r--r--   0        0        0     5824 2023-05-02 19:21:22.853435 encoded_core-0.0.0.1b2/src/encoded_core/types/quality_metric.py
--rw-r--r--   0        0        0     2750 2023-05-01 15:51:03.333411 encoded_core-0.0.0.1b2/src/encoded_core/types/software.py
--rw-r--r--   0        0        0     3895 2023-04-28 18:02:48.791425 encoded_core-0.0.0.1b2/src/encoded_core/types/tracking_item.py
--rw-r--r--   0        0        0     5468 2023-05-01 15:51:03.338160 encoded_core-0.0.0.1b2/src/encoded_core/types/user_content.py
--rw-r--r--   0        0        0    12886 2023-05-01 15:51:03.346409 encoded_core-0.0.0.1b2/src/encoded_core/types/workflow.py
--rw-r--r--   0        0        0     1316 2023-04-28 17:00:24.678007 encoded_core-0.0.0.1b2/src/encoded_core/upgrade.py
--rw-r--r--   0        0        0     2601 1970-01-01 00:00:00.000000 encoded_core-0.0.0.1b2/setup.py
--rw-r--r--   0        0        0     2585 1970-01-01 00:00:00.000000 encoded_core-0.0.0.1b2/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-04-28 13:49:44.781887 encoded_core-0.0.0.1b4/LICENSE
+-rw-r--r--   0        0        0      174 2023-04-28 13:50:12.674541 encoded_core-0.0.0.1b4/README.rst
+-rw-r--r--   0        0        0     3671 2023-06-06 14:44:57.006111 encoded_core-0.0.0.1b4/pyproject.toml
+-rw-r--r--   0        0        0     2378 2023-05-01 18:24:20.274258 encoded_core-0.0.0.1b4/src/encoded_core/__init__.py
+-rw-r--r--   0        0        0    21571 2023-06-02 16:48:49.923493 encoded_core-0.0.0.1b4/src/encoded_core/file_views.py
+-rw-r--r--   0        0        0     4847 2023-04-28 17:14:35.491425 encoded_core-0.0.0.1b4/src/encoded_core/local_roles.py
+-rw-r--r--   0        0        0    12807 2023-06-02 15:59:02.987015 encoded_core-0.0.0.1b4/src/encoded_core/page_views.py
+-rw-r--r--   0        0        0     2490 2023-06-02 16:08:48.657524 encoded_core-0.0.0.1b4/src/encoded_core/qc_views.py
+-rw-r--r--   0        0        0     1915 2023-04-28 13:50:12.708994 encoded_core-0.0.0.1b4/src/encoded_core/schemas/document.json
+-rw-r--r--   0        0        0    18925 2023-05-02 19:21:41.656041 encoded_core-0.0.0.1b4/src/encoded_core/schemas/file.json
+-rw-r--r--   0        0        0     5070 2023-04-28 13:50:12.701442 encoded_core-0.0.0.1b4/src/encoded_core/schemas/file_format.json
+-rw-r--r--   0        0        0     6170 2023-04-28 13:50:12.706416 encoded_core-0.0.0.1b4/src/encoded_core/schemas/file_processed.json
+-rw-r--r--   0        0        0     2336 2023-04-28 13:50:12.710774 encoded_core-0.0.0.1b4/src/encoded_core/schemas/file_reference.json
+-rw-r--r--   0        0        0     1334 2023-05-11 17:27:14.435690 encoded_core-0.0.0.1b4/src/encoded_core/schemas/file_submitted.json
+-rw-r--r--   0        0        0     1831 2023-04-28 13:50:12.715563 encoded_core-0.0.0.1b4/src/encoded_core/schemas/higlass_view_config.json
+-rw-r--r--   0        0        0     1528 2023-04-28 13:50:12.714806 encoded_core-0.0.0.1b4/src/encoded_core/schemas/image.json
+-rw-r--r--   0        0        0    18352 2023-04-28 13:50:12.707283 encoded_core-0.0.0.1b4/src/encoded_core/schemas/meta_workflow.json
+-rw-r--r--   0        0        0    14409 2023-04-28 13:50:12.713194 encoded_core-0.0.0.1b4/src/encoded_core/schemas/meta_workflow_run.json
+-rw-r--r--   0        0        0    17295 2023-04-28 13:50:12.702288 encoded_core-0.0.0.1b4/src/encoded_core/schemas/mixins.json
+-rw-r--r--   0        0        0     4581 2023-04-28 13:50:12.716243 encoded_core-0.0.0.1b4/src/encoded_core/schemas/page.json
+-rw-r--r--   0        0        0     1454 2023-05-05 17:13:08.190163 encoded_core-0.0.0.1b4/src/encoded_core/schemas/quality_metric.json
+-rw-r--r--   0        0        0     3228 2023-05-02 19:21:00.959543 encoded_core-0.0.0.1b4/src/encoded_core/schemas/quality_metric_generic.json
+-rw-r--r--   0        0        0     5715 2023-04-28 13:50:12.713992 encoded_core-0.0.0.1b4/src/encoded_core/schemas/software.json
+-rw-r--r--   0        0        0     5010 2023-04-28 13:50:12.708092 encoded_core-0.0.0.1b4/src/encoded_core/schemas/static_section.json
+-rw-r--r--   0        0        0    20411 2023-04-28 13:50:12.700669 encoded_core-0.0.0.1b4/src/encoded_core/schemas/tracking_item.json
+-rw-r--r--   0        0        0     3749 2023-04-28 13:50:12.703052 encoded_core-0.0.0.1b4/src/encoded_core/schemas/user_content.json
+-rw-r--r--   0        0        0    28089 2023-05-02 19:08:31.618837 encoded_core-0.0.0.1b4/src/encoded_core/schemas/workflow.json
+-rw-r--r--   0        0        0    10491 2023-05-02 19:07:38.780580 encoded_core-0.0.0.1b4/src/encoded_core/schemas/workflow_run.json
+-rw-r--r--   0        0        0     1908 2023-04-28 13:50:12.703919 encoded_core-0.0.0.1b4/src/encoded_core/schemas/workflow_run_awsem.json
+-rw-r--r--   0        0        0        0 2023-04-28 17:30:49.756296 encoded_core-0.0.0.1b4/src/encoded_core/tests/__init__.py
+-rw-r--r--   0        0        0    14046 2023-05-05 16:55:24.908128 encoded_core-0.0.0.1b4/src/encoded_core/tests/conftest.py
+-rw-r--r--   0        0        0     1873 2023-05-01 15:51:03.342243 encoded_core-0.0.0.1b4/src/encoded_core/tests/conftest_settings.py
+-rw-r--r--   0        0        0     7765 2023-05-02 19:39:48.058091 encoded_core-0.0.0.1b4/src/encoded_core/tests/datafixtures.py
+-rw-r--r--   0        0        0    10832 2023-05-02 19:39:17.806355 encoded_core-0.0.0.1b4/src/encoded_core/tests/test_types_file.py
+-rw-r--r--   0        0        0      262 2023-05-02 19:36:28.328655 encoded_core-0.0.0.1b4/src/encoded_core/tests/test_types_file_format.py
+-rw-r--r--   0        0        0      239 2023-05-02 19:39:17.802109 encoded_core-0.0.0.1b4/src/encoded_core/tests/test_types_meta_workflow.py
+-rw-r--r--   0        0        0      212 2023-05-02 19:39:17.799579 encoded_core-0.0.0.1b4/src/encoded_core/tests/test_types_software.py
+-rw-r--r--   0        0        0      502 2023-05-02 19:39:54.040945 encoded_core-0.0.0.1b4/src/encoded_core/tests/test_types_workflow.py
+-rw-r--r--   0        0        0       70 2023-04-28 13:50:12.688855 encoded_core-0.0.0.1b4/src/encoded_core/types/__init__.py
+-rw-r--r--   0        0        0     1284 2023-06-02 13:39:14.666319 encoded_core-0.0.0.1b4/src/encoded_core/types/document.py
+-rw-r--r--   0        0        0    20058 2023-06-02 15:54:47.022313 encoded_core-0.0.0.1b4/src/encoded_core/types/file.py
+-rw-r--r--   0        0        0      789 2023-06-02 13:42:53.807665 encoded_core-0.0.0.1b4/src/encoded_core/types/file_format.py
+-rw-r--r--   0        0        0     2325 2023-06-06 14:44:48.692867 encoded_core-0.0.0.1b4/src/encoded_core/types/file_processed.py
+-rw-r--r--   0        0        0      490 2023-06-06 14:44:48.696157 encoded_core-0.0.0.1b4/src/encoded_core/types/file_reference.py
+-rw-r--r--   0        0        0     1998 2023-06-06 14:44:41.314893 encoded_core-0.0.0.1b4/src/encoded_core/types/file_submitted.py
+-rw-r--r--   0        0        0      584 2023-06-02 13:43:41.158990 encoded_core-0.0.0.1b4/src/encoded_core/types/higlass_view_config.py
+-rw-r--r--   0        0        0     1040 2023-06-02 13:39:14.669360 encoded_core-0.0.0.1b4/src/encoded_core/types/image.py
+-rw-r--r--   0        0        0     3136 2023-06-06 14:40:02.762803 encoded_core-0.0.0.1b4/src/encoded_core/types/meta_workflow.py
+-rw-r--r--   0        0        0      858 2023-06-02 16:00:14.279429 encoded_core-0.0.0.1b4/src/encoded_core/types/page.py
+-rw-r--r--   0        0        0     1705 2023-06-02 16:07:00.928971 encoded_core-0.0.0.1b4/src/encoded_core/types/quality_metric.py
+-rw-r--r--   0        0        0     2750 2023-05-01 15:51:03.333411 encoded_core-0.0.0.1b4/src/encoded_core/types/software.py
+-rw-r--r--   0        0        0     3847 2023-06-02 13:41:24.973582 encoded_core-0.0.0.1b4/src/encoded_core/types/tracking_item.py
+-rw-r--r--   0        0        0     5468 2023-05-01 15:51:03.338160 encoded_core-0.0.0.1b4/src/encoded_core/types/user_content.py
+-rw-r--r--   0        0        0    12886 2023-05-01 15:51:03.346409 encoded_core-0.0.0.1b4/src/encoded_core/types/workflow.py
+-rw-r--r--   0        0        0     1316 2023-04-28 17:00:24.678007 encoded_core-0.0.0.1b4/src/encoded_core/upgrade.py
+-rw-r--r--   0        0        0     2601 1970-01-01 00:00:00.000000 encoded_core-0.0.0.1b4/setup.py
+-rw-r--r--   0        0        0     2585 1970-01-01 00:00:00.000000 encoded_core-0.0.0.1b4/PKG-INFO
```

### Comparing `encoded_core-0.0.0.1b2/LICENSE` & `encoded_core-0.0.0.1b4/LICENSE`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b2/pyproject.toml` & `encoded_core-0.0.0.1b4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "encoded-core"
-version = "0.0.0.1b2"  # to become 0.0.1
+version = "0.0.0.1b4"  # to become 0.0.1
 description = "Core data models for Park Lab ENCODE based projects"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/smaht-dac/encoded-core"
 repository = "https://github.com/smaht-dac/encoded-core"
 documentation = "https://github.com/smaht-dac/encoded-core"
```

### Comparing `encoded_core-0.0.0.1b2/src/encoded_core/__init__.py` & `encoded_core-0.0.0.1b4/src/encoded_core/__init__.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b2/src/encoded_core/local_roles.py` & `encoded_core-0.0.0.1b4/src/encoded_core/local_roles.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b2/src/encoded_core/schemas/document.json` & `encoded_core-0.0.0.1b4/src/encoded_core/schemas/document.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b2/src/encoded_core/schemas/file.json` & `encoded_core-0.0.0.1b4/src/encoded_core/schemas/file.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b2/src/encoded_core/schemas/file_format.json` & `encoded_core-0.0.0.1b4/src/encoded_core/schemas/file_format.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b2/src/encoded_core/schemas/file_processed.json` & `encoded_core-0.0.0.1b4/src/encoded_core/schemas/file_processed.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b2/src/encoded_core/schemas/file_reference.json` & `encoded_core-0.0.0.1b4/src/encoded_core/schemas/file_reference.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b2/src/encoded_core/schemas/file_submitted.json` & `encoded_core-0.0.0.1b4/src/encoded_core/schemas/file_submitted.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'description'": "'File submitted to ENCODED'"}*

```diff
@@ -1,11 +1,11 @@
 {
     "$schema": "http://json-schema.org/draft-04/schema#",
     "additionalProperties": false,
-    "description": "File submitted to CGAP",
+    "description": "File submitted to ENCODED",
     "id": "/profiles/file_submitted.json",
     "identifyingProperties": [
         "uuid",
         "accession",
         "aliases"
     ],
     "mixinColumns": [
```

### Comparing `encoded_core-0.0.0.1b2/src/encoded_core/schemas/higlass_view_config.json` & `encoded_core-0.0.0.1b4/src/encoded_core/schemas/higlass_view_config.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b2/src/encoded_core/schemas/image.json` & `encoded_core-0.0.0.1b4/src/encoded_core/schemas/image.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b2/src/encoded_core/schemas/meta_workflow.json` & `encoded_core-0.0.0.1b4/src/encoded_core/schemas/meta_workflow.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b2/src/encoded_core/schemas/meta_workflow_run.json` & `encoded_core-0.0.0.1b4/src/encoded_core/schemas/meta_workflow_run.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b2/src/encoded_core/schemas/mixins.json` & `encoded_core-0.0.0.1b4/src/encoded_core/schemas/mixins.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b2/src/encoded_core/schemas/page.json` & `encoded_core-0.0.0.1b4/src/encoded_core/schemas/page.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b2/src/encoded_core/schemas/quality_metric.json` & `encoded_core-0.0.0.1b4/src/encoded_core/schemas/quality_metric.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b2/src/encoded_core/schemas/quality_metric_generic.json` & `encoded_core-0.0.0.1b4/src/encoded_core/schemas/quality_metric_generic.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b2/src/encoded_core/schemas/software.json` & `encoded_core-0.0.0.1b4/src/encoded_core/schemas/software.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b2/src/encoded_core/schemas/static_section.json` & `encoded_core-0.0.0.1b4/src/encoded_core/schemas/static_section.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b2/src/encoded_core/schemas/tracking_item.json` & `encoded_core-0.0.0.1b4/src/encoded_core/schemas/tracking_item.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b2/src/encoded_core/schemas/user_content.json` & `encoded_core-0.0.0.1b4/src/encoded_core/schemas/user_content.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b2/src/encoded_core/schemas/workflow.json` & `encoded_core-0.0.0.1b4/src/encoded_core/schemas/workflow.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b2/src/encoded_core/schemas/workflow_run.json` & `encoded_core-0.0.0.1b4/src/encoded_core/schemas/workflow_run.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b2/src/encoded_core/schemas/workflow_run_awsem.json` & `encoded_core-0.0.0.1b4/src/encoded_core/schemas/workflow_run_awsem.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b2/src/encoded_core/tests/conftest.py` & `encoded_core-0.0.0.1b4/src/encoded_core/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b2/src/encoded_core/tests/conftest_settings.py` & `encoded_core-0.0.0.1b4/src/encoded_core/tests/conftest_settings.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b2/src/encoded_core/tests/datafixtures.py` & `encoded_core-0.0.0.1b4/src/encoded_core/tests/datafixtures.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b2/src/encoded_core/tests/test_types_file.py` & `encoded_core-0.0.0.1b4/src/encoded_core/tests/test_types_file.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b2/src/encoded_core/types/document.py` & `encoded_core-0.0.0.1b4/src/encoded_core/types/document.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 @collection(
     name='documents',
     properties={
         'title': 'Documents',
         'description': 'Listing of Documents',
     })
-class Document(ItemWithAttachment, Item):
+class Document(ItemWithAttachment):
     """Document class."""
 
     item_type = 'document'
     schema = load_schema('encoded_core:schemas/document.json')
     embedded_list = []
     mimetype_map = {'application/proband+xml': ['text/plain']}
```

### Comparing `encoded_core-0.0.0.1b2/src/encoded_core/types/file_format.py` & `encoded_core-0.0.0.1b4/src/encoded_core/types/file_format.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 from snovault import (
     calculated_property,
     collection,
     load_schema,
 )
 from snovault.attachment import ItemWithAttachment
-from snovault.types.base import (
-    Item
-)
 
 
 @collection(
     name='file-formats',
     unique_key='file_format:file_format',
-    lookup_key='file_format',
     properties={
         'title': 'File Formats',
         'description': 'Listing of file formats used by 4DN'
     }
 )
-class FileFormat(Item, ItemWithAttachment):
+class FileFormat(ItemWithAttachment):
     """The class to store information about 4DN file formats"""
     item_type = 'file_format'
     schema = load_schema('encoded_core:schemas/file_format.json')
     name_key = 'file_format'
 
     @calculated_property(schema={
         "title": "Display Title",
```

### Comparing `encoded_core-0.0.0.1b2/src/encoded_core/types/file_processed.py` & `encoded_core-0.0.0.1b4/src/encoded_core/types/file_processed.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
         'description': 'Listing of Processed Files',
     })
 class FileProcessed(File):
     """Collection for individual processed files."""
     item_type = 'file_processed'
     schema = load_schema('encoded_core:schemas/file_processed.json')
     embedded_list = File.embedded_list + file_workflow_run_embeds
-    name_key = 'accession'
     rev = dict(File.rev, **{
         'workflow_run_inputs': ('WorkflowRun', 'input_files.value'),
         'workflow_run_outputs': ('WorkflowRun', 'output_files.value'),
     })
     aggregated_items = {
         "last_modified": [
             "date_modified"
```

### Comparing `encoded_core-0.0.0.1b2/src/encoded_core/types/file_submitted.py` & `encoded_core-0.0.0.1b4/src/encoded_core/types/file_submitted.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,14 @@
         "description": "Listing of Submitted Files",
     })
 class FileSubmitted(File):
     """Collection for individual submitted files."""
     item_type = 'file_submitted'
     schema = load_schema('encoded_core:schemas/file_submitted.json')
     embedded_list = _build_file_submitted_embedded_list()
-    name_key = 'accession'
     rev = dict(File.rev, **{
         'workflow_run_inputs': ('WorkflowRun', 'input_files.value'),
         'workflow_run_outputs': ('WorkflowRun', 'output_files.value'),
     })
 
     @calculated_property(schema={
         "title": "Input of Workflow Runs",
```

### Comparing `encoded_core-0.0.0.1b2/src/encoded_core/types/higlass_view_config.py` & `encoded_core-0.0.0.1b4/src/encoded_core/types/higlass_view_config.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from snovault import collection, load_schema
 from snovault.types.base import Item
 
 
 @collection(
     name='higlass-view-configs',
-    unique_key='higlass_view_config:uuid',
-    lookup_key='name',
+    unique_key='higlass_view_config:name',
     properties={
         'title': 'HiGlass Displays',
         'description': 'Displays and view configurations for HiGlass',
     })
 class HiglassViewConfig(Item):
     """
     Item type which contains a `view_config` property and other metadata.
```

### Comparing `encoded_core-0.0.0.1b2/src/encoded_core/types/image.py` & `encoded_core-0.0.0.1b4/src/encoded_core/types/image.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 @collection(
     name='images',
     unique_key='image:filename',
     properties={
         'title': 'Image',
         'description': 'Listing of portal images',
     })
-class Image(ItemWithAttachment, Item):
+class Image(ItemWithAttachment):
     """Class image,defines accepted file types."""
 
     item_type = 'image'
     schema = load_schema('encoded_core:schemas/image.json')
     schema['properties']['attachment']['properties']['type']['enum'] = [
         'image/png',
         'image/jpeg',
```

### Comparing `encoded_core-0.0.0.1b2/src/encoded_core/types/meta_workflow.py` & `encoded_core-0.0.0.1b4/src/encoded_core/types/meta_workflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,22 +52,20 @@
         "workflow_runs.workflow_run.output_files.*",
         # "workflow_runs.workflow_run.output_files.value.workflow_run_outputs.@id"
     ]
 
 
 @collection(
     name='meta-workflows',
-    unique_key='accession',
     properties={
         'title': 'MetaWorkflows',
         'description': 'Listing of MetaWorkflows',
     })
 class MetaWorkflow(Item):
     item_type = 'meta_workflow'
-    name_key = 'accession'
     schema = load_schema('encoded_core:schemas/meta_workflow.json')
 
 
 @collection(
     name='meta-workflow-runs',
     properties={
         'title': 'MetaWorkflowRuns',
```

### Comparing `encoded_core-0.0.0.1b2/src/encoded_core/types/page.py` & `encoded_core-0.0.0.1b4/src/encoded_core/page_views.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,53 @@
-"""
-The type file for the collection Pages.  Which is used for static pages on the portal
-"""
-
 from dcicutils.misc_utils import filtered_warnings
-from pyramid.httpexceptions import ( # 301-307 redirect code response
+from pyramid.httpexceptions import (  # 301-307 redirect code response
     HTTPMovedPermanently,
     HTTPFound,
     HTTPSeeOther,
     HTTPTemporaryRedirect
 )
 from pyramid.view import view_config
-from snovault import collection, load_schema, COLLECTIONS, CONNECTION
+from snovault import COLLECTIONS, CONNECTION
 from snovault.resource_views import item_view_page
 from snovault.util import debug_log
 from snovault.validators import (
     validate_item_content_post,
     validate_item_content_put,
     validate_item_content_patch,
     validate_item_content_in_place,
     no_validate_item_content_post,
     no_validate_item_content_put,
     no_validate_item_content_patch
 )
 from urllib.parse import urlparse, urlencode
 from snovault.search.search import get_iterable_search_results
-from snovault.types.base import Item, collection_add, item_edit
-# from .user_content import StaticSection
+from snovault.types.base import collection_add, item_edit
+from .types.page import Page
+
+
+def includeme(config):
+    with filtered_warnings("ignore", category=DeprecationWarning):
+        config.add_route(
+            'staticpage',
+            '/*subpath',
+            # TODO: Replace custom_predicates=[is_static_page] with something more modern.
+            # The custom_predicates needs to be rewritten.
+            # Although there is a complex rewrite using .add_route_predicate,
+            # the simpler case of just using .add_static_view may bypass a lot of complexity.
+            # But this needs more study to get right. For now this code will work and
+            # we're just going to suppress the warning.  -kmp 16-May-2020
+            # Refs:
+            #  - https://stackoverflow.com/questions/30102767/custom-route-predicates-in-pyramid
+            #  - https://docs.pylonsproject.org/projects/pyramid/en/latest/_modules/pyramid/config/routes.html
+            #  - https://docs.pylonsproject.org/projects/pyramid/en/master/narr/hooks.html#view-and-route-predicates
+            #  - https://docs.pylonsproject.org/projects/pyramid/en/latest/api/config.html
+            custom_predicates=[is_static_page],
+            request_method="GET"
+        )
+    config.add_view(static_page, route_name='staticpage')
 
 
 def get_pyramid_http_exception_for_redirect_code(code):
     code_dict = {
         301 : HTTPMovedPermanently,
         302 : HTTPFound,
         303 : HTTPSeeOther,
@@ -124,15 +142,14 @@
             new_children.append(add_sibling_parent_relations_to_tree(new_child))
         new_node = node.copy()
         new_node['children'] = new_children
         return new_node
     return node
 
 
-
 def is_static_page(info, request):
     page_name = "/".join(info.get('match', {}).get('subpath'))
     if '@@' in page_name:
         return False
 
     path_parts = page_name.split('/')
     if path_parts[0] != "pages" and path_parts[0] in request.registry[COLLECTIONS].keys():
@@ -143,63 +160,14 @@
 
     if request._static_page_model:
         return True
     else:
         return False
 
 
-def includeme(config):
-    with filtered_warnings("ignore", category=DeprecationWarning):
-        config.add_route(
-            'staticpage',
-            '/*subpath',
-            # TODO: Replace custom_predicates=[is_static_page] with something more modern.
-            # The custom_predicates needs to be rewritten.
-            # Although there is a complex rewrite using .add_route_predicate,
-            # the simpler case of just using .add_static_view may bypass a lot of complexity.
-            # But this needs more study to get right. For now this code will work and
-            # we're just going to suppress the warning.  -kmp 16-May-2020
-            # Refs:
-            #  - https://stackoverflow.com/questions/30102767/custom-route-predicates-in-pyramid
-            #  - https://docs.pylonsproject.org/projects/pyramid/en/latest/_modules/pyramid/config/routes.html
-            #  - https://docs.pylonsproject.org/projects/pyramid/en/master/narr/hooks.html#view-and-route-predicates
-            #  - https://docs.pylonsproject.org/projects/pyramid/en/latest/api/config.html
-            custom_predicates=[is_static_page],
-            request_method="GET"
-        )
-    config.add_view(static_page, route_name='staticpage')
-
-
-@collection(
-    name='pages',
-    lookup_key='name',
-    properties={
-        'title': 'Pages',
-        'description': 'Static Pages for the Portal',
-    })
-class Page(Item):
-    """Links to StaticSections"""
-    item_type = 'page'
-    schema = load_schema('encoded_core:schemas/page.json')
-    embedded_list = ['content.*']
-
-    # STATUS_ACL = StaticSection.STATUS_ACL
-
-    class Collection(Item.Collection):
-        pass
-
-
-for field in ['display_title', 'name', 'description', 'content.name']:
-    Page.embedded_list = Page.embedded_list + [
-        'children.' + field, 'children.children.' + field, 'children.children.children.' + field
-    ]
-
-
-#### Must add validators for add/edit since 'name' path is now lookup_key, not unique_key
-
 def validate_unique_page_name(context, request):
     '''validator to ensure page 'name' lookup_key is unique
     '''
     data = request.json
     # name is required; validate_item_content_post/put/patch will handle missing field
     if 'name' in data:
         lookup_res = request.registry[CONNECTION].storage.get_by_json('name', data['name'], 'page')
@@ -310,8 +278,8 @@
             item['previous'] =  remove_relations_in_tree(curr_node['previous'])
         if curr_node.get('parent'):
             item['parent'] =    remove_relations_in_tree(curr_node['parent'], keep="parent")
         if curr_node.get('sibling_length') is not None:
             item['sibling_length'] = curr_node['sibling_length']
             item['sibling_position'] = curr_node['sibling_position']
 
-    return item
+    return item
```

### Comparing `encoded_core-0.0.0.1b2/src/encoded_core/types/software.py` & `encoded_core-0.0.0.1b4/src/encoded_core/types/software.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b2/src/encoded_core/types/tracking_item.py` & `encoded_core-0.0.0.1b4/src/encoded_core/types/tracking_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,28 +15,27 @@
 )
 
 
 @collection(
     name='tracking-items',
     properties={
         'title': 'TrackingItem',
-        'description': 'For internal tracking of Fourfront events',
+        'description': 'For internal tracking of ENCODED events',
     })
 class TrackingItem(Item):
     """tracking-item class."""
 
     item_type = 'tracking_item'
     schema = load_schema('encoded_core:schemas/tracking_item.json')
     embedded_list = []
-    STATUS_ACL = Item.STATUS_ACL.copy()
-    STATUS_ACL.update({
+    STATUS_ACL = {
         'released': ONLY_ADMIN_VIEW_ACL,
         'deleted': DELETED_ACL,
         'draft': ONLY_ADMIN_VIEW_ACL
-    })
+    }
 
     @classmethod
     def create_and_commit(cls, request, properties, clean_headers=False):
         """
         Create a TrackingItem with a given request and properties, committing
         it directly to the DB. This works by manually committing the
         transaction, which may cause issues if this function is called as
```

### Comparing `encoded_core-0.0.0.1b2/src/encoded_core/types/user_content.py` & `encoded_core-0.0.0.1b4/src/encoded_core/types/user_content.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b2/src/encoded_core/types/workflow.py` & `encoded_core-0.0.0.1b4/src/encoded_core/types/workflow.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b2/src/encoded_core/upgrade.py` & `encoded_core-0.0.0.1b4/src/encoded_core/upgrade.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b2/setup.py` & `encoded_core-0.0.0.1b4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
                      'show-image-manifest = '
                      'dcicutils.ecr_scripts:show_image_manifest_main',
                      'unrelease-most-recent-image = '
                      'dcicutils.ecr_scripts:unrelease_most_recent_image_main']}
 
 setup_kwargs = {
     'name': 'encoded-core',
-    'version': '0.0.0.1b2',
+    'version': '0.0.0.1b4',
     'description': 'Core data models for Park Lab ENCODE based projects',
     'long_description': '============\nencoded-core\n============\n\n\nWelcome to ``encoded-core``!\n\nThis library contains common data models used across ENCODE style projects\nimplemented by the Park Lab.',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/smaht-dac/encoded-core',
```

### Comparing `encoded_core-0.0.0.1b2/PKG-INFO` & `encoded_core-0.0.0.1b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encoded-core
-Version: 0.0.0.1b2
+Version: 0.0.0.1b4
 Summary: Core data models for Park Lab ENCODE based projects
 Home-page: https://github.com/smaht-dac/encoded-core
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.8.1,<3.10
 Classifier: Development Status :: 3 - Alpha
```

