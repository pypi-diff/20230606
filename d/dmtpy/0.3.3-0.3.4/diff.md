# Comparing `tmp/dmtpy-0.3.3.tar.gz` & `tmp/dmtpy-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmtpy-0.3.3.tar", last modified: Mon Apr 17 08:55:33 2023, max compression
+gzip compressed data, was "dmtpy-0.3.4.tar", last modified: Tue Jun  6 10:58:56 2023, max compression
```

## Comparing `dmtpy-0.3.3.tar` & `dmtpy-0.3.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:55:33.717674 dmtpy-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-04-17 08:55:12.000000 dmtpy-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-17 08:55:33.717674 dmtpy-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-17 08:55:12.000000 dmtpy-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 08:55:33.717674 dmtpy-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-17 08:55:12.000000 dmtpy-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:55:33.713674 dmtpy-0.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:55:33.717674 dmtpy-0.3.3/src/dmt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 08:55:12.000000 dmtpy-0.3.3/src/dmt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-04-17 08:55:12.000000 dmtpy-0.3.3/src/dmt/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-17 08:55:12.000000 dmtpy-0.3.3/src/dmt/blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-17 08:55:12.000000 dmtpy-0.3.3/src/dmt/blueprint_attribute.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:55:33.717674 dmtpy-0.3.3/src/dmt/blueprints/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 08:55:12.000000 dmtpy-0.3.3/src/dmt/blueprints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-04-17 08:55:12.000000 dmtpy-0.3.3/src/dmt/blueprints/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-17 08:55:12.000000 dmtpy-0.3.3/src/dmt/blueprints/namedentity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-04-17 08:55:12.000000 dmtpy-0.3.3/src/dmt/copier.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-17 08:55:12.000000 dmtpy-0.3.3/src/dmt/dimension.py
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-04-17 08:55:12.000000 dmtpy-0.3.3/src/dmt/dmt_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-04-17 08:55:12.000000 dmtpy-0.3.3/src/dmt/dmt_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-04-17 08:55:12.000000 dmtpy-0.3.3/src/dmt/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-17 08:55:12.000000 dmtpy-0.3.3/src/dmt/enum_attribute.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:55:33.717674 dmtpy-0.3.3/src/dmt/h5/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 08:55:12.000000 dmtpy-0.3.3/src/dmt/h5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-04-17 08:55:12.000000 dmtpy-0.3.3/src/dmt/h5/h5_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-17 08:55:12.000000 dmtpy-0.3.3/src/dmt/h5/h5_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-17 08:55:12.000000 dmtpy-0.3.3/src/dmt/namedentity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 08:55:33.717674 dmtpy-0.3.3/src/dmtpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-04-17 08:55:33.000000 dmtpy-0.3.3/src/dmtpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-17 08:55:33.000000 dmtpy-0.3.3/src/dmtpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 08:55:33.000000 dmtpy-0.3.3/src/dmtpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-17 08:55:33.000000 dmtpy-0.3.3/src/dmtpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-17 08:55:33.000000 dmtpy-0.3.3/src/dmtpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:58:56.359512 dmtpy-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-06 10:58:39.000000 dmtpy-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-06 10:58:56.359512 dmtpy-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-06 10:58:39.000000 dmtpy-0.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 10:58:56.359512 dmtpy-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-06 10:58:39.000000 dmtpy-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:58:56.359512 dmtpy-0.3.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:58:56.359512 dmtpy-0.3.4/src/dmt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 10:58:39.000000 dmtpy-0.3.4/src/dmt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-06 10:58:39.000000 dmtpy-0.3.4/src/dmt/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-06 10:58:39.000000 dmtpy-0.3.4/src/dmt/blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-06 10:58:39.000000 dmtpy-0.3.4/src/dmt/blueprint_attribute.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:58:56.359512 dmtpy-0.3.4/src/dmt/blueprints/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 10:58:39.000000 dmtpy-0.3.4/src/dmt/blueprints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-06 10:58:39.000000 dmtpy-0.3.4/src/dmt/blueprints/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-06 10:58:39.000000 dmtpy-0.3.4/src/dmt/blueprints/namedentity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-06-06 10:58:39.000000 dmtpy-0.3.4/src/dmt/copier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-06 10:58:39.000000 dmtpy-0.3.4/src/dmt/dimension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-06-06 10:58:39.000000 dmtpy-0.3.4/src/dmt/dmt_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-06-06 10:58:39.000000 dmtpy-0.3.4/src/dmt/dmt_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-06-06 10:58:39.000000 dmtpy-0.3.4/src/dmt/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-06 10:58:39.000000 dmtpy-0.3.4/src/dmt/enum_attribute.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:58:56.359512 dmtpy-0.3.4/src/dmt/h5/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 10:58:39.000000 dmtpy-0.3.4/src/dmt/h5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-06-06 10:58:39.000000 dmtpy-0.3.4/src/dmt/h5/h5_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-06-06 10:58:39.000000 dmtpy-0.3.4/src/dmt/h5/h5_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-06 10:58:39.000000 dmtpy-0.3.4/src/dmt/namedentity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 10:58:56.359512 dmtpy-0.3.4/src/dmtpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-06 10:58:56.000000 dmtpy-0.3.4/src/dmtpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-06 10:58:56.000000 dmtpy-0.3.4/src/dmtpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 10:58:56.000000 dmtpy-0.3.4/src/dmtpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-06 10:58:56.000000 dmtpy-0.3.4/src/dmtpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-06 10:58:56.000000 dmtpy-0.3.4/src/dmtpy.egg-info/top_level.txt
```

### Comparing `dmtpy-0.3.3/LICENSE` & `dmtpy-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dmtpy-0.3.3/PKG-INFO` & `dmtpy-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmtpy
-Version: 0.3.3
+Version: 0.3.4
 Summary: Python runtime library for SIMOS based DMT models
 Home-page: https://github.com/SINTEF/dmtpy
 Author: SINTEF Ocean
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `dmtpy-0.3.3/setup.py` & `dmtpy-0.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # Remove build and dist folders
 shutil.rmtree(Path("build"), ignore_errors=True)
 shutil.rmtree(Path("dist"), ignore_errors=True)
 
 setup(
     name="dmtpy",
-    version="0.3.3",
+    version="0.3.4",
     author="SINTEF Ocean",
     description="Python runtime library for SIMOS based DMT models",
     url="https://github.com/SINTEF/dmtpy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_dir={"": "src"},
     packages=find_packages(where="src", exclude=["tests"]),
```

### Comparing `dmtpy-0.3.3/src/dmt/attribute.py` & `dmtpy-0.3.4/src/dmt/attribute.py`

 * *Files identical despite different names*

### Comparing `dmtpy-0.3.3/src/dmt/blueprint.py` & `dmtpy-0.3.4/src/dmt/blueprint.py`

 * *Files identical despite different names*

### Comparing `dmtpy-0.3.3/src/dmt/blueprint_attribute.py` & `dmtpy-0.3.4/src/dmt/blueprint_attribute.py`

 * *Files identical despite different names*

### Comparing `dmtpy-0.3.3/src/dmt/copier.py` & `dmtpy-0.3.4/src/dmt/copier.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Sequence
 from dmt.blueprint import Blueprint
 from dmt.blueprint_attribute import BlueprintAttribute
 from .entity import Entity
 
 class Copier:
 
-    def __init__(self,keep_uncontained_references=False):
+    def __init__(self,keep_uncontained_references=True):
         """Create a copier
         keep_uncontained_references: If True, uncontained references will be copied as well, otherwise they will be removed
         """
         self.__copies = {}
         self.keep_uncontained_references = keep_uncontained_references
 
     def copy(self, entity: Entity) -> Entity:
```

### Comparing `dmtpy-0.3.3/src/dmt/dmt_reader.py` & `dmtpy-0.3.4/src/dmt/dmt_reader.py`

 * *Files identical despite different names*

### Comparing `dmtpy-0.3.3/src/dmt/dmt_writer.py` & `dmtpy-0.3.4/src/dmt/dmt_writer.py`

 * *Files identical despite different names*

### Comparing `dmtpy-0.3.3/src/dmt/entity.py` & `dmtpy-0.3.4/src/dmt/entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,11 +85,11 @@
                         yield child
                         yield from child.all_content()
                 else:
                     child: Entity = value
                     yield child
                     yield from child.all_content()
 
-    def copy(self: E,keep_uncontained_references=False) -> E:
+    def copy(self: E,keep_uncontained_references=True) -> E:
         """"Copy the entity"""
         from .copier import Copier
         return Copier(keep_uncontained_references).copy(self)
```

### Comparing `dmtpy-0.3.3/src/dmt/enum_attribute.py` & `dmtpy-0.3.4/src/dmt/enum_attribute.py`

 * *Files identical despite different names*

### Comparing `dmtpy-0.3.3/src/dmt/h5/h5_reader.py` & `dmtpy-0.3.4/src/dmt/h5/h5_reader.py`

 * *Files identical despite different names*

### Comparing `dmtpy-0.3.3/src/dmt/h5/h5_writer.py` & `dmtpy-0.3.4/src/dmt/h5/h5_writer.py`

 * *Files identical despite different names*

### Comparing `dmtpy-0.3.3/src/dmt/namedentity.py` & `dmtpy-0.3.4/src/dmt/namedentity.py`

 * *Files identical despite different names*

### Comparing `dmtpy-0.3.3/src/dmtpy.egg-info/PKG-INFO` & `dmtpy-0.3.4/src/dmtpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmtpy
-Version: 0.3.3
+Version: 0.3.4
 Summary: Python runtime library for SIMOS based DMT models
 Home-page: https://github.com/SINTEF/dmtpy
 Author: SINTEF Ocean
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `dmtpy-0.3.3/src/dmtpy.egg-info/SOURCES.txt` & `dmtpy-0.3.4/src/dmtpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

