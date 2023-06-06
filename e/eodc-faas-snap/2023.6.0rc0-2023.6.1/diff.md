# Comparing `tmp/eodc_faas_snap-2023.6.0rc0.tar.gz` & `tmp/eodc_faas_snap-2023.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodc_faas_snap-2023.6.0rc0.tar", max compression
+gzip compressed data, was "eodc_faas_snap-2023.6.1.tar", max compression
```

## Comparing `eodc_faas_snap-2023.6.0rc0.tar` & `eodc_faas_snap-2023.6.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       23 2023-05-31 09:46:10.507411 eodc_faas_snap-2023.6.0rc0/README.md
--rw-r--r--   0        0        0      694 2023-06-05 18:54:46.773222 eodc_faas_snap-2023.6.0rc0/pyproject.toml
--rw-r--r--   0        0        0       96 2023-06-05 18:54:39.633223 eodc_faas_snap-2023.6.0rc0/snap_processor_bindings/__init__.py
--rw-r--r--   0        0        0      937 2023-06-05 13:22:28.033203 eodc_faas_snap-2023.6.0rc0/snap_processor_bindings/model.py
--rw-r--r--   0        0        0     4743 2023-06-05 13:59:41.846970 eodc_faas_snap-2023.6.0rc0/snap_processor_bindings/workflows.py
--rw-r--r--   0        0        0      684 1970-01-01 00:00:00.000000 eodc_faas_snap-2023.6.0rc0/PKG-INFO
+-rw-r--r--   0        0        0       23 2023-06-01 09:43:57.267253 eodc_faas_snap-2023.6.1/README.md
+-rw-r--r--   0        0        0      689 2023-06-06 07:18:22.939253 eodc_faas_snap-2023.6.1/pyproject.toml
+-rw-r--r--   0        0        0       91 2023-06-06 07:18:22.939253 eodc_faas_snap-2023.6.1/snap_processor_bindings/__init__.py
+-rw-r--r--   0        0        0      937 2023-06-05 13:20:29.499253 eodc_faas_snap-2023.6.1/snap_processor_bindings/model.py
+-rw-r--r--   0        0        0     4743 2023-06-06 07:18:22.939253 eodc_faas_snap-2023.6.1/snap_processor_bindings/workflows.py
+-rw-r--r--   0        0        0      681 1970-01-01 00:00:00.000000 eodc_faas_snap-2023.6.1/PKG-INFO
```

### Comparing `eodc_faas_snap-2023.6.0rc0/pyproject.toml` & `eodc_faas_snap-2023.6.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eodc-faas-snap"
-version = "2023.6.0-rc.0"
+version = "2023.6.1"
 description = "Bindings for the snap processor exposed at EODC"
 authors = ["Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>", "Sean Hoyal <sean.hoyal@eodc.eu>", "Valentina Hutter <valentina.hutter@eodc.eu>"]
 readme = "README.md"
 packages = [{include = "snap_processor_bindings"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `eodc_faas_snap-2023.6.0rc0/snap_processor_bindings/model.py` & `eodc_faas_snap-2023.6.1/snap_processor_bindings/model.py`

 * *Files identical despite different names*

### Comparing `eodc_faas_snap-2023.6.0rc0/snap_processor_bindings/workflows.py` & `eodc_faas_snap-2023.6.1/snap_processor_bindings/workflows.py`

 * *Files identical despite different names*

### Comparing `eodc_faas_snap-2023.6.0rc0/PKG-INFO` & `eodc_faas_snap-2023.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eodc-faas-snap
-Version: 2023.6.0rc0
+Version: 2023.6.1
 Summary: Bindings for the snap processor exposed at EODC
 Author: Lukas Weidenholzer
 Author-email: lukas.weidenholzer@eodc.eu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

