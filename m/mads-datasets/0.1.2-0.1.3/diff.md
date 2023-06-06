# Comparing `tmp/mads_datasets-0.1.2.tar.gz` & `tmp/mads_datasets-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mads_datasets-0.1.2.tar", max compression
+gzip compressed data, was "mads_datasets-0.1.3.tar", max compression
```

## Comparing `mads_datasets-0.1.2.tar` & `mads_datasets-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2023-06-05 10:06:45.165441 mads_datasets-0.1.2/README.md
--rw-r--r--   0        0        0      164 2023-06-06 08:40:48.440388 mads_datasets-0.1.2/mads_datasets/__init__.py
--rw-r--r--   0        0        0    15296 2023-06-06 08:43:25.924558 mads_datasets-0.1.2/mads_datasets/datasetfactory.py
--rw-r--r--   0        0        0     4995 2023-06-05 19:39:01.314359 mads_datasets-0.1.2/mads_datasets/datasets.py
--rw-r--r--   0        0        0     4778 2023-06-05 10:37:07.673949 mads_datasets-0.1.2/mads_datasets/datatools.py
--rw-r--r--   0        0        0     3251 2023-06-06 08:42:57.768632 mads_datasets-0.1.2/mads_datasets/settings.py
--rw-r--r--   0        0        0      974 2023-06-06 08:44:13.499846 mads_datasets-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      778 1970-01-01 00:00:00.000000 mads_datasets-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-05 10:06:45.165441 mads_datasets-0.1.3/README.md
+-rw-r--r--   0        0        0      164 2023-06-06 08:40:48.440388 mads_datasets-0.1.3/mads_datasets/__init__.py
+-rw-r--r--   0        0        0    15323 2023-06-06 08:50:10.477115 mads_datasets-0.1.3/mads_datasets/datasetfactory.py
+-rw-r--r--   0        0        0     4995 2023-06-05 19:39:01.314359 mads_datasets-0.1.3/mads_datasets/datasets.py
+-rw-r--r--   0        0        0     4778 2023-06-05 10:37:07.673949 mads_datasets-0.1.3/mads_datasets/datatools.py
+-rw-r--r--   0        0        0     3251 2023-06-06 08:42:57.768632 mads_datasets-0.1.3/mads_datasets/settings.py
+-rw-r--r--   0        0        0      974 2023-06-06 08:52:16.930675 mads_datasets-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      778 1970-01-01 00:00:00.000000 mads_datasets-0.1.3/PKG-INFO
```

### Comparing `mads_datasets-0.1.2/mads_datasets/datasetfactory.py` & `mads_datasets-0.1.3/mads_datasets/datasetfactory.py`

 * *Files 0% similar despite different names*

```diff
@@ -389,15 +389,15 @@
         if dataset_type == DatasetType.FLOWERS:
             preprocessor = kwargs.get("preprocessor", BasePreprocessor)
             return FlowersDatasetFactory(
                 flowersdatasetsettings, preprocessor=preprocessor, **kwargs
             )
         if dataset_type == DatasetType.IMDB:
             preprocessor = kwargs.get("preprocessor", IMDBTokenizer)
-            return IMDBDatasetFactory(imdbdatasetsettings, **kwargs)
+            return IMDBDatasetFactory(imdbdatasetsettings, preprocessor=preprocessor, **kwargs)
         if dataset_type == DatasetType.GESTURES:
             preprocessor = kwargs.get("preprocessor", PaddedPreprocessor)
             return GesturesDatasetFactory(
                 gesturesdatasetsettings, preprocessor=preprocessor, **kwargs
             )
         if dataset_type == DatasetType.FASHION:
             preprocessor = kwargs.get("preprocessor", BasePreprocessor)
```

### Comparing `mads_datasets-0.1.2/mads_datasets/datasets.py` & `mads_datasets-0.1.3/mads_datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `mads_datasets-0.1.2/mads_datasets/datatools.py` & `mads_datasets-0.1.3/mads_datasets/datatools.py`

 * *Files identical despite different names*

### Comparing `mads_datasets-0.1.2/mads_datasets/settings.py` & `mads_datasets-0.1.3/mads_datasets/settings.py`

 * *Files identical despite different names*

### Comparing `mads_datasets-0.1.2/pyproject.toml` & `mads_datasets-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mads-datasets"
-version = "0.1.2"
+version = "0.1.3"
 description = "Datasets for the master applied data science"
 authors = ["Raoul Grouls <Raoul.Grouls@han.nl>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "mads_datasets"}]
 
 [tool.poetry.dependencies]
```

### Comparing `mads_datasets-0.1.2/PKG-INFO` & `mads_datasets-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mads-datasets
-Version: 0.1.2
+Version: 0.1.3
 Summary: Datasets for the master applied data science
 License: MIT
 Author: Raoul Grouls
 Author-email: Raoul.Grouls@han.nl
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

