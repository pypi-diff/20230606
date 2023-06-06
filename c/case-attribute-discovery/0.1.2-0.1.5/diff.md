# Comparing `tmp/case_attribute_discovery-0.1.2.tar.gz` & `tmp/case_attribute_discovery-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "case_attribute_discovery-0.1.2.tar", max compression
+gzip compressed data, was "case_attribute_discovery-0.1.5.tar", max compression
```

## Comparing `case_attribute_discovery-0.1.2.tar` & `case_attribute_discovery-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2023-06-06 09:54:19.022540 case_attribute_discovery-0.1.2/LICENSE
--rw-r--r--   0        0        0     2049 2023-06-06 10:09:14.745854 case_attribute_discovery-0.1.2/README.md
--rw-r--r--   0        0        0      571 2023-06-06 10:47:13.969693 case_attribute_discovery-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-06 09:54:19.023038 case_attribute_discovery-0.1.2/src/case_attribute_discovery/__init__.py
--rw-r--r--   0        0        0      476 2023-06-06 09:54:19.023190 case_attribute_discovery-0.1.2/src/case_attribute_discovery/config.py
--rw-r--r--   0        0        0     4180 2023-06-06 10:00:16.489132 case_attribute_discovery-0.1.2/src/case_attribute_discovery/discovery.py
--rw-r--r--   0        0        0     2610 1970-01-01 00:00:00.000000 case_attribute_discovery-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-06 11:07:30.121601 case_attribute_discovery-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2049 2023-06-06 11:07:30.121601 case_attribute_discovery-0.1.5/README.md
+-rw-r--r--   0        0        0      571 2023-06-06 11:07:30.121601 case_attribute_discovery-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-06 11:07:30.121601 case_attribute_discovery-0.1.5/src/case_attribute_discovery/__init__.py
+-rw-r--r--   0        0        0      476 2023-06-06 11:07:30.121601 case_attribute_discovery-0.1.5/src/case_attribute_discovery/config.py
+-rw-r--r--   0        0        0     4180 2023-06-06 11:07:30.121601 case_attribute_discovery-0.1.5/src/case_attribute_discovery/discovery.py
+-rw-r--r--   0        0        0     2610 1970-01-01 00:00:00.000000 case_attribute_discovery-0.1.5/PKG-INFO
```

### Comparing `case_attribute_discovery-0.1.2/LICENSE` & `case_attribute_discovery-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `case_attribute_discovery-0.1.2/README.md` & `case_attribute_discovery-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `case_attribute_discovery-0.1.2/pyproject.toml` & `case_attribute_discovery-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "case-attribute-discovery"
-version = "0.1.2"
+version = "0.1.5"
 description = ""
 authors = ["David Chapela de la Campa <david.chapela.delacampa@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "case_attribute_discovery", from = "src" }]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
```

### Comparing `case_attribute_discovery-0.1.2/src/case_attribute_discovery/discovery.py` & `case_attribute_discovery-0.1.5/src/case_attribute_discovery/discovery.py`

 * *Files identical despite different names*

### Comparing `case_attribute_discovery-0.1.2/PKG-INFO` & `case_attribute_discovery-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: case-attribute-discovery
-Version: 0.1.2
+Version: 0.1.5
 Summary: 
 Author: David Chapela de la Campa
 Author-email: david.chapela.delacampa@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

