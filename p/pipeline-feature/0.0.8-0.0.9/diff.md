# Comparing `tmp/pipeline-feature-0.0.8.tar.gz` & `tmp/pipeline-feature-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipeline-feature-0.0.8.tar", last modified: Tue Jun  6 08:19:09 2023, max compression
+gzip compressed data, was "pipeline-feature-0.0.9.tar", last modified: Tue Jun  6 08:26:01 2023, max compression
```

## Comparing `pipeline-feature-0.0.8.tar` & `pipeline-feature-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 gaohn      (501) staff       (20)        0 2023-06-06 08:19:09.640824 pipeline-feature-0.0.8/
--rw-r--r--   0 gaohn      (501) staff       (20)     1072 2023-06-06 02:49:04.000000 pipeline-feature-0.0.8/LICENSE
--rw-r--r--   0 gaohn      (501) staff       (20)      589 2023-06-06 08:19:09.640655 pipeline-feature-0.0.8/PKG-INFO
--rw-r--r--   0 gaohn      (501) staff       (20)       20 2023-06-06 03:10:35.000000 pipeline-feature-0.0.8/README.md
-drwxr-xr-x   0 gaohn      (501) staff       (20)        0 2023-06-06 08:19:09.639502 pipeline-feature-0.0.8/mlops_pipeline_feature_v1/
--rw-r--r--   0 gaohn      (501) staff       (20)        0 2023-06-06 03:26:48.000000 pipeline-feature-0.0.8/mlops_pipeline_feature_v1/__init__.py
--rw-r--r--   0 gaohn      (501) staff       (20)    10219 2023-06-06 08:16:20.000000 pipeline-feature-0.0.8/mlops_pipeline_feature_v1/pipeline.py
-drwxr-xr-x   0 gaohn      (501) staff       (20)        0 2023-06-06 08:19:09.640318 pipeline-feature-0.0.8/pipeline_feature.egg-info/
--rw-r--r--   0 gaohn      (501) staff       (20)      589 2023-06-06 08:19:09.000000 pipeline-feature-0.0.8/pipeline_feature.egg-info/PKG-INFO
--rw-r--r--   0 gaohn      (501) staff       (20)      307 2023-06-06 08:19:09.000000 pipeline-feature-0.0.8/pipeline_feature.egg-info/SOURCES.txt
--rw-r--r--   0 gaohn      (501) staff       (20)        1 2023-06-06 08:19:09.000000 pipeline-feature-0.0.8/pipeline_feature.egg-info/dependency_links.txt
--rw-r--r--   0 gaohn      (501) staff       (20)      120 2023-06-06 08:19:09.000000 pipeline-feature-0.0.8/pipeline_feature.egg-info/requires.txt
--rw-r--r--   0 gaohn      (501) staff       (20)       49 2023-06-06 08:19:09.000000 pipeline-feature-0.0.8/pipeline_feature.egg-info/top_level.txt
--rw-r--r--   0 gaohn      (501) staff       (20)      980 2023-06-06 08:19:01.000000 pipeline-feature-0.0.8/pyproject.toml
--rw-r--r--   0 gaohn      (501) staff       (20)       38 2023-06-06 08:19:09.640885 pipeline-feature-0.0.8/setup.cfg
+drwxr-xr-x   0 gaohn      (501) staff       (20)        0 2023-06-06 08:26:01.787322 pipeline-feature-0.0.9/
+-rw-r--r--   0 gaohn      (501) staff       (20)     1072 2023-06-06 02:49:04.000000 pipeline-feature-0.0.9/LICENSE
+-rw-r--r--   0 gaohn      (501) staff       (20)      589 2023-06-06 08:26:01.787209 pipeline-feature-0.0.9/PKG-INFO
+-rw-r--r--   0 gaohn      (501) staff       (20)       20 2023-06-06 03:10:35.000000 pipeline-feature-0.0.9/README.md
+drwxr-xr-x   0 gaohn      (501) staff       (20)        0 2023-06-06 08:26:01.786218 pipeline-feature-0.0.9/mlops_pipeline_feature_v1/
+-rw-r--r--   0 gaohn      (501) staff       (20)        0 2023-06-06 03:26:48.000000 pipeline-feature-0.0.9/mlops_pipeline_feature_v1/__init__.py
+-rw-r--r--   0 gaohn      (501) staff       (20)    10219 2023-06-06 08:16:20.000000 pipeline-feature-0.0.9/mlops_pipeline_feature_v1/pipeline.py
+drwxr-xr-x   0 gaohn      (501) staff       (20)        0 2023-06-06 08:26:01.787024 pipeline-feature-0.0.9/pipeline_feature.egg-info/
+-rw-r--r--   0 gaohn      (501) staff       (20)      589 2023-06-06 08:26:01.000000 pipeline-feature-0.0.9/pipeline_feature.egg-info/PKG-INFO
+-rw-r--r--   0 gaohn      (501) staff       (20)      307 2023-06-06 08:26:01.000000 pipeline-feature-0.0.9/pipeline_feature.egg-info/SOURCES.txt
+-rw-r--r--   0 gaohn      (501) staff       (20)        1 2023-06-06 08:26:01.000000 pipeline-feature-0.0.9/pipeline_feature.egg-info/dependency_links.txt
+-rw-r--r--   0 gaohn      (501) staff       (20)      130 2023-06-06 08:26:01.000000 pipeline-feature-0.0.9/pipeline_feature.egg-info/requires.txt
+-rw-r--r--   0 gaohn      (501) staff       (20)       49 2023-06-06 08:26:01.000000 pipeline-feature-0.0.9/pipeline_feature.egg-info/top_level.txt
+-rw-r--r--   0 gaohn      (501) staff       (20)      997 2023-06-06 08:25:49.000000 pipeline-feature-0.0.9/pyproject.toml
+-rw-r--r--   0 gaohn      (501) staff       (20)       38 2023-06-06 08:26:01.787359 pipeline-feature-0.0.9/setup.cfg
```

### Comparing `pipeline-feature-0.0.8/LICENSE` & `pipeline-feature-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pipeline-feature-0.0.8/PKG-INFO` & `pipeline-feature-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipeline-feature
-Version: 0.0.8
+Version: 0.0.9
 Summary: Feature Pipeline of MLOps Pipeline Version 1
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/mlops-pipeline-v1
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/mlops-pipeline-v1/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pipeline-feature-0.0.8/mlops_pipeline_feature_v1/pipeline.py` & `pipeline-feature-0.0.9/mlops_pipeline_feature_v1/pipeline.py`

 * *Files identical despite different names*

### Comparing `pipeline-feature-0.0.8/pipeline_feature.egg-info/PKG-INFO` & `pipeline-feature-0.0.9/pipeline_feature.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipeline-feature
-Version: 0.0.8
+Version: 0.0.9
 Summary: Feature Pipeline of MLOps Pipeline Version 1
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/mlops-pipeline-v1
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/mlops-pipeline-v1/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pipeline-feature-0.0.8/pyproject.toml` & `pipeline-feature-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pipeline-feature"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Gao Hongnan", email="hongnangao@gmail.com" },
 ]
 description = "Feature Pipeline of MLOps Pipeline Version 1"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -19,14 +19,15 @@
 dependencies = [
     "numpy",
     "requests",
     "prettytable",
     "rich",
     "pydantic",
     "python-dotenv",
+    "db_dtypes",
     "gaohn-common-utils==0.0.23"
 ]
 
 [project.optional-dependencies]
 dev = ["black", "pylint", "isort", "pytest", "mypy"]
 
 [tool.setuptools.packages.find]
```

