# Comparing `tmp/encoded_core-0.0.0.1b4.tar.gz` & `tmp/encoded_core-0.0.0.1b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encoded_core-0.0.0.1b4.tar", max compression
+gzip compressed data, was "encoded_core-0.0.0.1b5.tar", max compression
```

## Comparing `encoded_core-0.0.0.1b4.tar` & `encoded_core-0.0.0.1b5.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0     1083 2023-04-28 13:49:44.781887 encoded_core-0.0.0.1b4/LICENSE
--rw-r--r--   0        0        0      174 2023-04-28 13:50:12.674541 encoded_core-0.0.0.1b4/README.rst
--rw-r--r--   0        0        0     3671 2023-06-06 14:44:57.006111 encoded_core-0.0.0.1b4/pyproject.toml
--rw-r--r--   0        0        0     2378 2023-05-01 18:24:20.274258 encoded_core-0.0.0.1b4/src/encoded_core/__init__.py
--rw-r--r--   0        0        0    21571 2023-06-02 16:48:49.923493 encoded_core-0.0.0.1b4/src/encoded_core/file_views.py
--rw-r--r--   0        0        0     4847 2023-04-28 17:14:35.491425 encoded_core-0.0.0.1b4/src/encoded_core/local_roles.py
--rw-r--r--   0        0        0    12807 2023-06-02 15:59:02.987015 encoded_core-0.0.0.1b4/src/encoded_core/page_views.py
--rw-r--r--   0        0        0     2490 2023-06-02 16:08:48.657524 encoded_core-0.0.0.1b4/src/encoded_core/qc_views.py
--rw-r--r--   0        0        0     1915 2023-04-28 13:50:12.708994 encoded_core-0.0.0.1b4/src/encoded_core/schemas/document.json
--rw-r--r--   0        0        0    18925 2023-05-02 19:21:41.656041 encoded_core-0.0.0.1b4/src/encoded_core/schemas/file.json
--rw-r--r--   0        0        0     5070 2023-04-28 13:50:12.701442 encoded_core-0.0.0.1b4/src/encoded_core/schemas/file_format.json
--rw-r--r--   0        0        0     6170 2023-04-28 13:50:12.706416 encoded_core-0.0.0.1b4/src/encoded_core/schemas/file_processed.json
--rw-r--r--   0        0        0     2336 2023-04-28 13:50:12.710774 encoded_core-0.0.0.1b4/src/encoded_core/schemas/file_reference.json
--rw-r--r--   0        0        0     1334 2023-05-11 17:27:14.435690 encoded_core-0.0.0.1b4/src/encoded_core/schemas/file_submitted.json
--rw-r--r--   0        0        0     1831 2023-04-28 13:50:12.715563 encoded_core-0.0.0.1b4/src/encoded_core/schemas/higlass_view_config.json
--rw-r--r--   0        0        0     1528 2023-04-28 13:50:12.714806 encoded_core-0.0.0.1b4/src/encoded_core/schemas/image.json
--rw-r--r--   0        0        0    18352 2023-04-28 13:50:12.707283 encoded_core-0.0.0.1b4/src/encoded_core/schemas/meta_workflow.json
--rw-r--r--   0        0        0    14409 2023-04-28 13:50:12.713194 encoded_core-0.0.0.1b4/src/encoded_core/schemas/meta_workflow_run.json
--rw-r--r--   0        0        0    17295 2023-04-28 13:50:12.702288 encoded_core-0.0.0.1b4/src/encoded_core/schemas/mixins.json
--rw-r--r--   0        0        0     4581 2023-04-28 13:50:12.716243 encoded_core-0.0.0.1b4/src/encoded_core/schemas/page.json
--rw-r--r--   0        0        0     1454 2023-05-05 17:13:08.190163 encoded_core-0.0.0.1b4/src/encoded_core/schemas/quality_metric.json
--rw-r--r--   0        0        0     3228 2023-05-02 19:21:00.959543 encoded_core-0.0.0.1b4/src/encoded_core/schemas/quality_metric_generic.json
--rw-r--r--   0        0        0     5715 2023-04-28 13:50:12.713992 encoded_core-0.0.0.1b4/src/encoded_core/schemas/software.json
--rw-r--r--   0        0        0     5010 2023-04-28 13:50:12.708092 encoded_core-0.0.0.1b4/src/encoded_core/schemas/static_section.json
--rw-r--r--   0        0        0    20411 2023-04-28 13:50:12.700669 encoded_core-0.0.0.1b4/src/encoded_core/schemas/tracking_item.json
--rw-r--r--   0        0        0     3749 2023-04-28 13:50:12.703052 encoded_core-0.0.0.1b4/src/encoded_core/schemas/user_content.json
--rw-r--r--   0        0        0    28089 2023-05-02 19:08:31.618837 encoded_core-0.0.0.1b4/src/encoded_core/schemas/workflow.json
--rw-r--r--   0        0        0    10491 2023-05-02 19:07:38.780580 encoded_core-0.0.0.1b4/src/encoded_core/schemas/workflow_run.json
--rw-r--r--   0        0        0     1908 2023-04-28 13:50:12.703919 encoded_core-0.0.0.1b4/src/encoded_core/schemas/workflow_run_awsem.json
--rw-r--r--   0        0        0        0 2023-04-28 17:30:49.756296 encoded_core-0.0.0.1b4/src/encoded_core/tests/__init__.py
--rw-r--r--   0        0        0    14046 2023-05-05 16:55:24.908128 encoded_core-0.0.0.1b4/src/encoded_core/tests/conftest.py
--rw-r--r--   0        0        0     1873 2023-05-01 15:51:03.342243 encoded_core-0.0.0.1b4/src/encoded_core/tests/conftest_settings.py
--rw-r--r--   0        0        0     7765 2023-05-02 19:39:48.058091 encoded_core-0.0.0.1b4/src/encoded_core/tests/datafixtures.py
--rw-r--r--   0        0        0    10832 2023-05-02 19:39:17.806355 encoded_core-0.0.0.1b4/src/encoded_core/tests/test_types_file.py
--rw-r--r--   0        0        0      262 2023-05-02 19:36:28.328655 encoded_core-0.0.0.1b4/src/encoded_core/tests/test_types_file_format.py
--rw-r--r--   0        0        0      239 2023-05-02 19:39:17.802109 encoded_core-0.0.0.1b4/src/encoded_core/tests/test_types_meta_workflow.py
--rw-r--r--   0        0        0      212 2023-05-02 19:39:17.799579 encoded_core-0.0.0.1b4/src/encoded_core/tests/test_types_software.py
--rw-r--r--   0        0        0      502 2023-05-02 19:39:54.040945 encoded_core-0.0.0.1b4/src/encoded_core/tests/test_types_workflow.py
--rw-r--r--   0        0        0       70 2023-04-28 13:50:12.688855 encoded_core-0.0.0.1b4/src/encoded_core/types/__init__.py
--rw-r--r--   0        0        0     1284 2023-06-02 13:39:14.666319 encoded_core-0.0.0.1b4/src/encoded_core/types/document.py
--rw-r--r--   0        0        0    20058 2023-06-02 15:54:47.022313 encoded_core-0.0.0.1b4/src/encoded_core/types/file.py
--rw-r--r--   0        0        0      789 2023-06-02 13:42:53.807665 encoded_core-0.0.0.1b4/src/encoded_core/types/file_format.py
--rw-r--r--   0        0        0     2325 2023-06-06 14:44:48.692867 encoded_core-0.0.0.1b4/src/encoded_core/types/file_processed.py
--rw-r--r--   0        0        0      490 2023-06-06 14:44:48.696157 encoded_core-0.0.0.1b4/src/encoded_core/types/file_reference.py
--rw-r--r--   0        0        0     1998 2023-06-06 14:44:41.314893 encoded_core-0.0.0.1b4/src/encoded_core/types/file_submitted.py
--rw-r--r--   0        0        0      584 2023-06-02 13:43:41.158990 encoded_core-0.0.0.1b4/src/encoded_core/types/higlass_view_config.py
--rw-r--r--   0        0        0     1040 2023-06-02 13:39:14.669360 encoded_core-0.0.0.1b4/src/encoded_core/types/image.py
--rw-r--r--   0        0        0     3136 2023-06-06 14:40:02.762803 encoded_core-0.0.0.1b4/src/encoded_core/types/meta_workflow.py
--rw-r--r--   0        0        0      858 2023-06-02 16:00:14.279429 encoded_core-0.0.0.1b4/src/encoded_core/types/page.py
--rw-r--r--   0        0        0     1705 2023-06-02 16:07:00.928971 encoded_core-0.0.0.1b4/src/encoded_core/types/quality_metric.py
--rw-r--r--   0        0        0     2750 2023-05-01 15:51:03.333411 encoded_core-0.0.0.1b4/src/encoded_core/types/software.py
--rw-r--r--   0        0        0     3847 2023-06-02 13:41:24.973582 encoded_core-0.0.0.1b4/src/encoded_core/types/tracking_item.py
--rw-r--r--   0        0        0     5468 2023-05-01 15:51:03.338160 encoded_core-0.0.0.1b4/src/encoded_core/types/user_content.py
--rw-r--r--   0        0        0    12886 2023-05-01 15:51:03.346409 encoded_core-0.0.0.1b4/src/encoded_core/types/workflow.py
--rw-r--r--   0        0        0     1316 2023-04-28 17:00:24.678007 encoded_core-0.0.0.1b4/src/encoded_core/upgrade.py
--rw-r--r--   0        0        0     2601 1970-01-01 00:00:00.000000 encoded_core-0.0.0.1b4/setup.py
--rw-r--r--   0        0        0     2585 1970-01-01 00:00:00.000000 encoded_core-0.0.0.1b4/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-04-28 13:49:44.781887 encoded_core-0.0.0.1b5/LICENSE
+-rw-r--r--   0        0        0      174 2023-04-28 13:50:12.674541 encoded_core-0.0.0.1b5/README.rst
+-rw-r--r--   0        0        0     3671 2023-06-06 15:07:52.928550 encoded_core-0.0.0.1b5/pyproject.toml
+-rw-r--r--   0        0        0     2378 2023-05-01 18:24:20.274258 encoded_core-0.0.0.1b5/src/encoded_core/__init__.py
+-rw-r--r--   0        0        0    21571 2023-06-02 16:48:49.923493 encoded_core-0.0.0.1b5/src/encoded_core/file_views.py
+-rw-r--r--   0        0        0     4847 2023-04-28 17:14:35.491425 encoded_core-0.0.0.1b5/src/encoded_core/local_roles.py
+-rw-r--r--   0        0        0    12807 2023-06-02 15:59:02.987015 encoded_core-0.0.0.1b5/src/encoded_core/page_views.py
+-rw-r--r--   0        0        0     2490 2023-06-02 16:08:48.657524 encoded_core-0.0.0.1b5/src/encoded_core/qc_views.py
+-rw-r--r--   0        0        0     1915 2023-04-28 13:50:12.708994 encoded_core-0.0.0.1b5/src/encoded_core/schemas/document.json
+-rw-r--r--   0        0        0    18925 2023-05-02 19:21:41.656041 encoded_core-0.0.0.1b5/src/encoded_core/schemas/file.json
+-rw-r--r--   0        0        0     5070 2023-04-28 13:50:12.701442 encoded_core-0.0.0.1b5/src/encoded_core/schemas/file_format.json
+-rw-r--r--   0        0        0     6170 2023-04-28 13:50:12.706416 encoded_core-0.0.0.1b5/src/encoded_core/schemas/file_processed.json
+-rw-r--r--   0        0        0     2336 2023-04-28 13:50:12.710774 encoded_core-0.0.0.1b5/src/encoded_core/schemas/file_reference.json
+-rw-r--r--   0        0        0     1334 2023-05-11 17:27:14.435690 encoded_core-0.0.0.1b5/src/encoded_core/schemas/file_submitted.json
+-rw-r--r--   0        0        0     1831 2023-04-28 13:50:12.715563 encoded_core-0.0.0.1b5/src/encoded_core/schemas/higlass_view_config.json
+-rw-r--r--   0        0        0     1528 2023-04-28 13:50:12.714806 encoded_core-0.0.0.1b5/src/encoded_core/schemas/image.json
+-rw-r--r--   0        0        0    18352 2023-04-28 13:50:12.707283 encoded_core-0.0.0.1b5/src/encoded_core/schemas/meta_workflow.json
+-rw-r--r--   0        0        0    14409 2023-04-28 13:50:12.713194 encoded_core-0.0.0.1b5/src/encoded_core/schemas/meta_workflow_run.json
+-rw-r--r--   0        0        0    17295 2023-04-28 13:50:12.702288 encoded_core-0.0.0.1b5/src/encoded_core/schemas/mixins.json
+-rw-r--r--   0        0        0     4581 2023-04-28 13:50:12.716243 encoded_core-0.0.0.1b5/src/encoded_core/schemas/page.json
+-rw-r--r--   0        0        0     1454 2023-05-05 17:13:08.190163 encoded_core-0.0.0.1b5/src/encoded_core/schemas/quality_metric.json
+-rw-r--r--   0        0        0     3228 2023-05-02 19:21:00.959543 encoded_core-0.0.0.1b5/src/encoded_core/schemas/quality_metric_generic.json
+-rw-r--r--   0        0        0     5715 2023-04-28 13:50:12.713992 encoded_core-0.0.0.1b5/src/encoded_core/schemas/software.json
+-rw-r--r--   0        0        0     5010 2023-04-28 13:50:12.708092 encoded_core-0.0.0.1b5/src/encoded_core/schemas/static_section.json
+-rw-r--r--   0        0        0    20411 2023-04-28 13:50:12.700669 encoded_core-0.0.0.1b5/src/encoded_core/schemas/tracking_item.json
+-rw-r--r--   0        0        0     3749 2023-04-28 13:50:12.703052 encoded_core-0.0.0.1b5/src/encoded_core/schemas/user_content.json
+-rw-r--r--   0        0        0    28089 2023-05-02 19:08:31.618837 encoded_core-0.0.0.1b5/src/encoded_core/schemas/workflow.json
+-rw-r--r--   0        0        0    10491 2023-05-02 19:07:38.780580 encoded_core-0.0.0.1b5/src/encoded_core/schemas/workflow_run.json
+-rw-r--r--   0        0        0     1908 2023-04-28 13:50:12.703919 encoded_core-0.0.0.1b5/src/encoded_core/schemas/workflow_run_awsem.json
+-rw-r--r--   0        0        0        0 2023-04-28 17:30:49.756296 encoded_core-0.0.0.1b5/src/encoded_core/tests/__init__.py
+-rw-r--r--   0        0        0    14046 2023-05-05 16:55:24.908128 encoded_core-0.0.0.1b5/src/encoded_core/tests/conftest.py
+-rw-r--r--   0        0        0     1873 2023-05-01 15:51:03.342243 encoded_core-0.0.0.1b5/src/encoded_core/tests/conftest_settings.py
+-rw-r--r--   0        0        0     7765 2023-05-02 19:39:48.058091 encoded_core-0.0.0.1b5/src/encoded_core/tests/datafixtures.py
+-rw-r--r--   0        0        0    10832 2023-05-02 19:39:17.806355 encoded_core-0.0.0.1b5/src/encoded_core/tests/test_types_file.py
+-rw-r--r--   0        0        0      262 2023-05-02 19:36:28.328655 encoded_core-0.0.0.1b5/src/encoded_core/tests/test_types_file_format.py
+-rw-r--r--   0        0        0      239 2023-05-02 19:39:17.802109 encoded_core-0.0.0.1b5/src/encoded_core/tests/test_types_meta_workflow.py
+-rw-r--r--   0        0        0      212 2023-05-02 19:39:17.799579 encoded_core-0.0.0.1b5/src/encoded_core/tests/test_types_software.py
+-rw-r--r--   0        0        0      502 2023-05-02 19:39:54.040945 encoded_core-0.0.0.1b5/src/encoded_core/tests/test_types_workflow.py
+-rw-r--r--   0        0        0       70 2023-04-28 13:50:12.688855 encoded_core-0.0.0.1b5/src/encoded_core/types/__init__.py
+-rw-r--r--   0        0        0     1284 2023-06-02 13:39:14.666319 encoded_core-0.0.0.1b5/src/encoded_core/types/document.py
+-rw-r--r--   0        0        0    20031 2023-06-06 15:06:52.700127 encoded_core-0.0.0.1b5/src/encoded_core/types/file.py
+-rw-r--r--   0        0        0      789 2023-06-02 13:42:53.807665 encoded_core-0.0.0.1b5/src/encoded_core/types/file_format.py
+-rw-r--r--   0        0        0     2297 2023-06-06 14:57:52.832401 encoded_core-0.0.0.1b5/src/encoded_core/types/file_processed.py
+-rw-r--r--   0        0        0      462 2023-06-06 14:57:52.835614 encoded_core-0.0.0.1b5/src/encoded_core/types/file_reference.py
+-rw-r--r--   0        0        0     1970 2023-06-06 14:55:50.259426 encoded_core-0.0.0.1b5/src/encoded_core/types/file_submitted.py
+-rw-r--r--   0        0        0      584 2023-06-02 13:43:41.158990 encoded_core-0.0.0.1b5/src/encoded_core/types/higlass_view_config.py
+-rw-r--r--   0        0        0     1040 2023-06-02 13:39:14.669360 encoded_core-0.0.0.1b5/src/encoded_core/types/image.py
+-rw-r--r--   0        0        0     3136 2023-06-06 14:40:02.762803 encoded_core-0.0.0.1b5/src/encoded_core/types/meta_workflow.py
+-rw-r--r--   0        0        0      858 2023-06-02 16:00:14.279429 encoded_core-0.0.0.1b5/src/encoded_core/types/page.py
+-rw-r--r--   0        0        0     1705 2023-06-02 16:07:00.928971 encoded_core-0.0.0.1b5/src/encoded_core/types/quality_metric.py
+-rw-r--r--   0        0        0     2750 2023-05-01 15:51:03.333411 encoded_core-0.0.0.1b5/src/encoded_core/types/software.py
+-rw-r--r--   0        0        0     3847 2023-06-02 13:41:24.973582 encoded_core-0.0.0.1b5/src/encoded_core/types/tracking_item.py
+-rw-r--r--   0        0        0     5468 2023-05-01 15:51:03.338160 encoded_core-0.0.0.1b5/src/encoded_core/types/user_content.py
+-rw-r--r--   0        0        0    12886 2023-05-01 15:51:03.346409 encoded_core-0.0.0.1b5/src/encoded_core/types/workflow.py
+-rw-r--r--   0        0        0     1316 2023-04-28 17:00:24.678007 encoded_core-0.0.0.1b5/src/encoded_core/upgrade.py
+-rw-r--r--   0        0        0     2601 1970-01-01 00:00:00.000000 encoded_core-0.0.0.1b5/setup.py
+-rw-r--r--   0        0        0     2585 1970-01-01 00:00:00.000000 encoded_core-0.0.0.1b5/PKG-INFO
```

### Comparing `encoded_core-0.0.0.1b4/LICENSE` & `encoded_core-0.0.0.1b5/LICENSE`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b4/pyproject.toml` & `encoded_core-0.0.0.1b5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "encoded-core"
-version = "0.0.0.1b4"  # to become 0.0.1
+version = "0.0.0.1b5"  # to become 0.0.1
 description = "Core data models for Park Lab ENCODE based projects"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/smaht-dac/encoded-core"
 repository = "https://github.com/smaht-dac/encoded-core"
 documentation = "https://github.com/smaht-dac/encoded-core"
```

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/__init__.py` & `encoded_core-0.0.0.1b5/src/encoded_core/__init__.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/file_views.py` & `encoded_core-0.0.0.1b5/src/encoded_core/file_views.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/local_roles.py` & `encoded_core-0.0.0.1b5/src/encoded_core/local_roles.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/page_views.py` & `encoded_core-0.0.0.1b5/src/encoded_core/page_views.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/qc_views.py` & `encoded_core-0.0.0.1b5/src/encoded_core/qc_views.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/schemas/document.json` & `encoded_core-0.0.0.1b5/src/encoded_core/schemas/document.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/schemas/file.json` & `encoded_core-0.0.0.1b5/src/encoded_core/schemas/file.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/schemas/file_format.json` & `encoded_core-0.0.0.1b5/src/encoded_core/schemas/file_format.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/schemas/file_processed.json` & `encoded_core-0.0.0.1b5/src/encoded_core/schemas/file_processed.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/schemas/file_reference.json` & `encoded_core-0.0.0.1b5/src/encoded_core/schemas/file_reference.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/schemas/file_submitted.json` & `encoded_core-0.0.0.1b5/src/encoded_core/schemas/file_submitted.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/schemas/higlass_view_config.json` & `encoded_core-0.0.0.1b5/src/encoded_core/schemas/higlass_view_config.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/schemas/image.json` & `encoded_core-0.0.0.1b5/src/encoded_core/schemas/image.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/schemas/meta_workflow.json` & `encoded_core-0.0.0.1b5/src/encoded_core/schemas/meta_workflow.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/schemas/meta_workflow_run.json` & `encoded_core-0.0.0.1b5/src/encoded_core/schemas/meta_workflow_run.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/schemas/mixins.json` & `encoded_core-0.0.0.1b5/src/encoded_core/schemas/mixins.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/schemas/page.json` & `encoded_core-0.0.0.1b5/src/encoded_core/schemas/page.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/schemas/quality_metric.json` & `encoded_core-0.0.0.1b5/src/encoded_core/schemas/quality_metric.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/schemas/quality_metric_generic.json` & `encoded_core-0.0.0.1b5/src/encoded_core/schemas/quality_metric_generic.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/schemas/software.json` & `encoded_core-0.0.0.1b5/src/encoded_core/schemas/software.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/schemas/static_section.json` & `encoded_core-0.0.0.1b5/src/encoded_core/schemas/static_section.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/schemas/tracking_item.json` & `encoded_core-0.0.0.1b5/src/encoded_core/schemas/tracking_item.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/schemas/user_content.json` & `encoded_core-0.0.0.1b5/src/encoded_core/schemas/user_content.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/schemas/workflow.json` & `encoded_core-0.0.0.1b5/src/encoded_core/schemas/workflow.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/schemas/workflow_run.json` & `encoded_core-0.0.0.1b5/src/encoded_core/schemas/workflow_run.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/schemas/workflow_run_awsem.json` & `encoded_core-0.0.0.1b5/src/encoded_core/schemas/workflow_run_awsem.json`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/tests/conftest.py` & `encoded_core-0.0.0.1b5/src/encoded_core/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/tests/conftest_settings.py` & `encoded_core-0.0.0.1b5/src/encoded_core/tests/conftest_settings.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/tests/datafixtures.py` & `encoded_core-0.0.0.1b5/src/encoded_core/tests/datafixtures.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/tests/test_types_file.py` & `encoded_core-0.0.0.1b5/src/encoded_core/tests/test_types_file.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/types/document.py` & `encoded_core-0.0.0.1b5/src/encoded_core/types/document.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/types/file.py` & `encoded_core-0.0.0.1b5/src/encoded_core/types/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,14 @@
     })
 class File(Item):
     """Collection for individual files."""
     item_type = 'file'
     base_types = ['File'] + Item.base_types
     schema = load_schema('encoded_core:schemas/file.json')
     embedded_list = _build_file_embedded_list()
-    name_key = 'accession'
 
     @calculated_property(schema={
         "title": "Display Title",
         "description": "Name of this File",
         "type": "string"
     })
     def display_title(self, request, file_format, accession=None, external_accession=None):
```

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/types/file_format.py` & `encoded_core-0.0.0.1b5/src/encoded_core/types/file_format.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/types/file_processed.py` & `encoded_core-0.0.0.1b5/src/encoded_core/types/file_processed.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,14 @@
     load_schema,
 )
 from .file import File, file_workflow_run_embeds
 
 
 @collection(
     name='files-processed',
-    unique_key='accession',
     properties={
         'title': 'Processed Files',
         'description': 'Listing of Processed Files',
     })
 class FileProcessed(File):
     """Collection for individual processed files."""
     item_type = 'file_processed'
```

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/types/file_submitted.py` & `encoded_core-0.0.0.1b5/src/encoded_core/types/file_submitted.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
         "quality_metric.Sequence length",
         "quality_metric.url",
     ]
 
 
 @collection(
     name="files-submitted",
-    unique_key="accession",
     properties={
         "title": "Submitted Files",
         "description": "Listing of Submitted Files",
     })
 class FileSubmitted(File):
     """Collection for individual submitted files."""
     item_type = 'file_submitted'
```

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/types/higlass_view_config.py` & `encoded_core-0.0.0.1b5/src/encoded_core/types/higlass_view_config.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/types/image.py` & `encoded_core-0.0.0.1b5/src/encoded_core/types/image.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/types/meta_workflow.py` & `encoded_core-0.0.0.1b5/src/encoded_core/types/meta_workflow.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/types/page.py` & `encoded_core-0.0.0.1b5/src/encoded_core/types/page.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/types/quality_metric.py` & `encoded_core-0.0.0.1b5/src/encoded_core/types/quality_metric.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/types/software.py` & `encoded_core-0.0.0.1b5/src/encoded_core/types/software.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/types/tracking_item.py` & `encoded_core-0.0.0.1b5/src/encoded_core/types/tracking_item.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/types/user_content.py` & `encoded_core-0.0.0.1b5/src/encoded_core/types/user_content.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/types/workflow.py` & `encoded_core-0.0.0.1b5/src/encoded_core/types/workflow.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b4/src/encoded_core/upgrade.py` & `encoded_core-0.0.0.1b5/src/encoded_core/upgrade.py`

 * *Files identical despite different names*

### Comparing `encoded_core-0.0.0.1b4/setup.py` & `encoded_core-0.0.0.1b5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
                      'show-image-manifest = '
                      'dcicutils.ecr_scripts:show_image_manifest_main',
                      'unrelease-most-recent-image = '
                      'dcicutils.ecr_scripts:unrelease_most_recent_image_main']}
 
 setup_kwargs = {
     'name': 'encoded-core',
-    'version': '0.0.0.1b4',
+    'version': '0.0.0.1b5',
     'description': 'Core data models for Park Lab ENCODE based projects',
     'long_description': '============\nencoded-core\n============\n\n\nWelcome to ``encoded-core``!\n\nThis library contains common data models used across ENCODE style projects\nimplemented by the Park Lab.',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/smaht-dac/encoded-core',
```

### Comparing `encoded_core-0.0.0.1b4/PKG-INFO` & `encoded_core-0.0.0.1b5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encoded-core
-Version: 0.0.0.1b4
+Version: 0.0.0.1b5
 Summary: Core data models for Park Lab ENCODE based projects
 Home-page: https://github.com/smaht-dac/encoded-core
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.8.1,<3.10
 Classifier: Development Status :: 3 - Alpha
```

