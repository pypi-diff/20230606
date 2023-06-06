# Comparing `tmp/access_nri_intake-0.0.5.post1.tar.gz` & `tmp/access_nri_intake-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "access_nri_intake-0.0.5.post1.tar", last modified: Wed May 31 03:31:26 2023, max compression
+gzip compressed data, was "access_nri_intake-0.0.6.tar", last modified: Tue Jun  6 02:40:58 2023, max compression
```

## Comparing `access_nri_intake-0.0.5.post1.tar` & `access_nri_intake-0.0.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 03:31:26.114569 access_nri_intake-0.0.5.post1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-31 03:31:10.000000 access_nri_intake-0.0.5.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-31 03:31:26.114569 access_nri_intake-0.0.5.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-31 03:31:10.000000 access_nri_intake-0.0.5.post1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-31 03:31:10.000000 access_nri_intake-0.0.5.post1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 03:31:26.114569 access_nri_intake-0.0.5.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-31 03:31:10.000000 access_nri_intake-0.0.5.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 03:31:26.114569 access_nri_intake-0.0.5.post1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 03:31:26.114569 access_nri_intake-0.0.5.post1/src/access_nri_intake/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-31 03:31:10.000000 access_nri_intake-0.0.5.post1/src/access_nri_intake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-31 03:31:26.114569 access_nri_intake-0.0.5.post1/src/access_nri_intake/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 03:31:26.114569 access_nri_intake-0.0.5.post1/src/access_nri_intake/cat/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-31 03:31:10.000000 access_nri_intake-0.0.5.post1/src/access_nri_intake/cat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-31 03:31:10.000000 access_nri_intake-0.0.5.post1/src/access_nri_intake/cat/catalog.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-05-31 03:31:10.000000 access_nri_intake-0.0.5.post1/src/access_nri_intake/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 03:31:26.114569 access_nri_intake-0.0.5.post1/src/access_nri_intake/esmcat/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-31 03:31:10.000000 access_nri_intake-0.0.5.post1/src/access_nri_intake/esmcat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13197 2023-05-31 03:31:10.000000 access_nri_intake-0.0.5.post1/src/access_nri_intake/esmcat/builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-31 03:31:10.000000 access_nri_intake-0.0.5.post1/src/access_nri_intake/esmcat/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 03:31:26.114569 access_nri_intake-0.0.5.post1/src/access_nri_intake/metacat/
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-31 03:31:10.000000 access_nri_intake-0.0.5.post1/src/access_nri_intake/metacat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-05-31 03:31:10.000000 access_nri_intake-0.0.5.post1/src/access_nri_intake/metacat/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-05-31 03:31:10.000000 access_nri_intake-0.0.5.post1/src/access_nri_intake/metacat/translators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-05-31 03:31:10.000000 access_nri_intake-0.0.5.post1/src/access_nri_intake/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 03:31:26.114569 access_nri_intake-0.0.5.post1/src/access_nri_intake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-31 03:31:26.000000 access_nri_intake-0.0.5.post1/src/access_nri_intake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-31 03:31:26.000000 access_nri_intake-0.0.5.post1/src/access_nri_intake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 03:31:26.000000 access_nri_intake-0.0.5.post1/src/access_nri_intake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-31 03:31:26.000000 access_nri_intake-0.0.5.post1/src/access_nri_intake.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-31 03:31:26.000000 access_nri_intake-0.0.5.post1/src/access_nri_intake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-31 03:31:26.000000 access_nri_intake-0.0.5.post1/src/access_nri_intake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    83751 2023-05-31 03:31:10.000000 access_nri_intake-0.0.5.post1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:40:58.751484 access_nri_intake-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-06 02:40:44.000000 access_nri_intake-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-06 02:40:58.751484 access_nri_intake-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-06-06 02:40:44.000000 access_nri_intake-0.0.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-06 02:40:44.000000 access_nri_intake-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 02:40:58.751484 access_nri_intake-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-06 02:40:44.000000 access_nri_intake-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:40:58.747485 access_nri_intake-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:40:58.751484 access_nri_intake-0.0.6/src/access_nri_intake/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-06 02:40:44.000000 access_nri_intake-0.0.6/src/access_nri_intake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-06 02:40:58.751484 access_nri_intake-0.0.6/src/access_nri_intake/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:40:58.751484 access_nri_intake-0.0.6/src/access_nri_intake/cat/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-06 02:40:44.000000 access_nri_intake-0.0.6/src/access_nri_intake/cat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-06 02:40:44.000000 access_nri_intake-0.0.6/src/access_nri_intake/cat/catalog.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-06-06 02:40:44.000000 access_nri_intake-0.0.6/src/access_nri_intake/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:40:58.751484 access_nri_intake-0.0.6/src/access_nri_intake/esmcat/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-06 02:40:44.000000 access_nri_intake-0.0.6/src/access_nri_intake/esmcat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13197 2023-06-06 02:40:44.000000 access_nri_intake-0.0.6/src/access_nri_intake/esmcat/builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-06 02:40:44.000000 access_nri_intake-0.0.6/src/access_nri_intake/esmcat/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:40:58.751484 access_nri_intake-0.0.6/src/access_nri_intake/metacat/
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-06 02:40:44.000000 access_nri_intake-0.0.6/src/access_nri_intake/metacat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6922 2023-06-06 02:40:44.000000 access_nri_intake-0.0.6/src/access_nri_intake/metacat/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-06-06 02:40:44.000000 access_nri_intake-0.0.6/src/access_nri_intake/metacat/translators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-06 02:40:44.000000 access_nri_intake-0.0.6/src/access_nri_intake/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 02:40:58.751484 access_nri_intake-0.0.6/src/access_nri_intake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-06 02:40:58.000000 access_nri_intake-0.0.6/src/access_nri_intake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-06 02:40:58.000000 access_nri_intake-0.0.6/src/access_nri_intake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 02:40:58.000000 access_nri_intake-0.0.6/src/access_nri_intake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-06 02:40:58.000000 access_nri_intake-0.0.6/src/access_nri_intake.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-06 02:40:58.000000 access_nri_intake-0.0.6/src/access_nri_intake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-06 02:40:58.000000 access_nri_intake-0.0.6/src/access_nri_intake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    83751 2023-06-06 02:40:44.000000 access_nri_intake-0.0.6/versioneer.py
```

### Comparing `access_nri_intake-0.0.5.post1/LICENSE` & `access_nri_intake-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.5.post1/PKG-INFO` & `access_nri_intake-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: access_nri_intake
-Version: 0.0.5.post1
+Version: 0.0.6
 Summary: Intake catalog managed by ACCESS-NRI and associated tools
 Author: ACCESS-NRI
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,15 @@
 ------------
 
 +---------------+----------------------+
 | Documentation | |docs|               |
 +---------------+----------------------+
 | Package       | |pypi| |conda|       |
 +---------------+----------------------+
-| CI/CD         | |cd|                 |
+| CI/CD         | |pre-commit| |cd|    |
 +---------------+----------------------+
 | Development   | |black|              |
 +---------------+----------------------+
 | License       | |license|            |
 +---------------+----------------------+
 
 .. |docs| image:: https://readthedocs.org/projects/access-nri-intake-catalog/badge/?version=latest
@@ -42,14 +42,18 @@
         :target: https://pypi.org/project/access-nri-intake/
         :alt: PyPI package
         
 .. |conda| image:: https://img.shields.io/conda/v/accessnri/access-nri-intake
         :target: https://anaconda.org/accessnri/access-nri-intake
         :alt: Conda package
 
+.. |pre-commit| image:: https://github.com/ACCESS-NRI/access-nri-intake-catalog/actions/workflows/pre-commit.yaml/badge.svg
+        :target: https://github.com/ACCESS-NRI/access-nri-intake-catalog/actions/workflows/pre-commit.yaml
+        :alt: Pre-commit status
+        
 .. |cd| image:: https://github.com/ACCESS-NRI/access-nri-intake-catalog/actions/workflows/cd.yml/badge.svg
         :target: https://github.com/ACCESS-NRI/access-nri-intake-catalog/actions/workflows/cd.yml
         :alt: Package CD status
         
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
         :target: https://github.com/python/black
         :alt: Black code formatter
```

### Comparing `access_nri_intake-0.0.5.post1/README.rst` & `access_nri_intake-0.0.6/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 ------------
 
 +---------------+----------------------+
 | Documentation | |docs|               |
 +---------------+----------------------+
 | Package       | |pypi| |conda|       |
 +---------------+----------------------+
-| CI/CD         | |cd|                 |
+| CI/CD         | |pre-commit| |cd|    |
 +---------------+----------------------+
 | Development   | |black|              |
 +---------------+----------------------+
 | License       | |license|            |
 +---------------+----------------------+
 
 .. |docs| image:: https://readthedocs.org/projects/access-nri-intake-catalog/badge/?version=latest
@@ -28,14 +28,18 @@
         :target: https://pypi.org/project/access-nri-intake/
         :alt: PyPI package
         
 .. |conda| image:: https://img.shields.io/conda/v/accessnri/access-nri-intake
         :target: https://anaconda.org/accessnri/access-nri-intake
         :alt: Conda package
 
+.. |pre-commit| image:: https://github.com/ACCESS-NRI/access-nri-intake-catalog/actions/workflows/pre-commit.yaml/badge.svg
+        :target: https://github.com/ACCESS-NRI/access-nri-intake-catalog/actions/workflows/pre-commit.yaml
+        :alt: Pre-commit status
+        
 .. |cd| image:: https://github.com/ACCESS-NRI/access-nri-intake-catalog/actions/workflows/cd.yml/badge.svg
         :target: https://github.com/ACCESS-NRI/access-nri-intake-catalog/actions/workflows/cd.yml
         :alt: Package CD status
         
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
         :target: https://github.com/python/black
         :alt: Black code formatter
```

### Comparing `access_nri_intake-0.0.5.post1/pyproject.toml` & `access_nri_intake-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.5.post1/src/access_nri_intake/cli.py` & `access_nri_intake-0.0.6/src/access_nri_intake/cli.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.5.post1/src/access_nri_intake/esmcat/__init__.py` & `access_nri_intake-0.0.6/src/access_nri_intake/esmcat/__init__.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.5.post1/src/access_nri_intake/esmcat/builders.py` & `access_nri_intake-0.0.6/src/access_nri_intake/esmcat/builders.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.5.post1/src/access_nri_intake/esmcat/utils.py` & `access_nri_intake-0.0.6/src/access_nri_intake/esmcat/utils.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.5.post1/src/access_nri_intake/metacat/__init__.py` & `access_nri_intake-0.0.6/src/access_nri_intake/metacat/__init__.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.5.post1/src/access_nri_intake/metacat/manager.py` & `access_nri_intake-0.0.6/src/access_nri_intake/metacat/manager.py`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.5.post1/src/access_nri_intake/metacat/translators.py` & `access_nri_intake-0.0.6/src/access_nri_intake/metacat/translators.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,16 @@
         else:
             len_df = 1
 
         if hasattr(self.cat, column):
             val = getattr(self.cat, column)
         elif column in self.cat.metadata:
             val = self.cat.metadata[column]
+            if isinstance(val, list):
+                val = tuple(val)
         else:
             raise TranslatorError(
                 f"Could not translate '{column}' from {self.cat.name} using {self.__class__.__name__}"
             )
 
         return pd.Series([val] * len_df)
```

### Comparing `access_nri_intake-0.0.5.post1/src/access_nri_intake/utils.py` & `access_nri_intake-0.0.6/src/access_nri_intake/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     catalog_schema["required"] = req
 
     return schema, catalog_schema
 
 
 def load_metadata_yaml(path):
     """
-    Load a metadata.yaml file, leaving dates as strings and loading arrays as tuples
+    Load a metadata.yaml file, leaving dates as strings
 
     Parameters
     ----------
     paths: str
         The path to the metadata.yaml
     """
 
@@ -69,27 +69,15 @@
                 cls.yaml_implicit_resolvers = cls.yaml_implicit_resolvers.copy()
 
             for first_letter, mappings in cls.yaml_implicit_resolvers.items():
                 cls.yaml_implicit_resolvers[first_letter] = [
                     (tag, regexp) for tag, regexp in mappings if tag != tag_to_remove
                 ]
 
-    def tuple_constructor(self, node):
-        """
-        yaml constructor to make leaf sequences into tuples
-
-        See https://stackoverflow.com/questions/39553008/how-to-read-a-python-tuple-using-pyyaml
-        """
-        seq = self.construct_sequence(node)
-        if seq and isinstance(seq[0], (list, tuple)):
-            return seq
-        return tuple(seq)
-
     NoDatesSafeLoader.remove_implicit_resolver("tag:yaml.org,2002:timestamp")
-    NoDatesSafeLoader.add_constructor("tag:yaml.org,2002:seq", tuple_constructor)
 
     with open(path) as fpath:
         metadata = yaml.load(fpath, Loader=NoDatesSafeLoader)
 
     return metadata
```

### Comparing `access_nri_intake-0.0.5.post1/src/access_nri_intake.egg-info/PKG-INFO` & `access_nri_intake-0.0.6/src/access_nri_intake.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: access-nri-intake
-Version: 0.0.5.post1
+Version: 0.0.6
 Summary: Intake catalog managed by ACCESS-NRI and associated tools
 Author: ACCESS-NRI
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,15 @@
 ------------
 
 +---------------+----------------------+
 | Documentation | |docs|               |
 +---------------+----------------------+
 | Package       | |pypi| |conda|       |
 +---------------+----------------------+
-| CI/CD         | |cd|                 |
+| CI/CD         | |pre-commit| |cd|    |
 +---------------+----------------------+
 | Development   | |black|              |
 +---------------+----------------------+
 | License       | |license|            |
 +---------------+----------------------+
 
 .. |docs| image:: https://readthedocs.org/projects/access-nri-intake-catalog/badge/?version=latest
@@ -42,14 +42,18 @@
         :target: https://pypi.org/project/access-nri-intake/
         :alt: PyPI package
         
 .. |conda| image:: https://img.shields.io/conda/v/accessnri/access-nri-intake
         :target: https://anaconda.org/accessnri/access-nri-intake
         :alt: Conda package
 
+.. |pre-commit| image:: https://github.com/ACCESS-NRI/access-nri-intake-catalog/actions/workflows/pre-commit.yaml/badge.svg
+        :target: https://github.com/ACCESS-NRI/access-nri-intake-catalog/actions/workflows/pre-commit.yaml
+        :alt: Pre-commit status
+        
 .. |cd| image:: https://github.com/ACCESS-NRI/access-nri-intake-catalog/actions/workflows/cd.yml/badge.svg
         :target: https://github.com/ACCESS-NRI/access-nri-intake-catalog/actions/workflows/cd.yml
         :alt: Package CD status
         
 .. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
         :target: https://github.com/python/black
         :alt: Black code formatter
```

### Comparing `access_nri_intake-0.0.5.post1/src/access_nri_intake.egg-info/SOURCES.txt` & `access_nri_intake-0.0.6/src/access_nri_intake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `access_nri_intake-0.0.5.post1/versioneer.py` & `access_nri_intake-0.0.6/versioneer.py`

 * *Files identical despite different names*

