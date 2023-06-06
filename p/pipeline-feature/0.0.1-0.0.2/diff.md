# Comparing `tmp/pipeline-feature-0.0.1.tar.gz` & `tmp/pipeline-feature-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipeline-feature-0.0.1.tar", last modified: Tue Jun  6 05:17:14 2023, max compression
+gzip compressed data, was "pipeline-feature-0.0.2.tar", last modified: Tue Jun  6 05:25:23 2023, max compression
```

## Comparing `pipeline-feature-0.0.1.tar` & `pipeline-feature-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 gaohn      (501) staff       (20)        0 2023-06-06 05:17:14.043032 pipeline-feature-0.0.1/
--rw-r--r--   0 gaohn      (501) staff       (20)     1072 2023-06-06 02:49:04.000000 pipeline-feature-0.0.1/LICENSE
--rw-r--r--   0 gaohn      (501) staff       (20)      589 2023-06-06 05:17:14.042911 pipeline-feature-0.0.1/PKG-INFO
--rw-r--r--   0 gaohn      (501) staff       (20)       20 2023-06-06 03:10:35.000000 pipeline-feature-0.0.1/README.md
-drwxr-xr-x   0 gaohn      (501) staff       (20)        0 2023-06-06 05:17:14.041378 pipeline-feature-0.0.1/mlops_pipeline_feature_v1/
-drwxr-xr-x   0 gaohn      (501) staff       (20)        0 2023-06-06 05:17:14.042730 pipeline-feature-0.0.1/mlops_pipeline_feature_v1/pipeline_feature.egg-info/
--rw-r--r--   0 gaohn      (501) staff       (20)      589 2023-06-06 05:17:14.000000 pipeline-feature-0.0.1/mlops_pipeline_feature_v1/pipeline_feature.egg-info/PKG-INFO
--rw-r--r--   0 gaohn      (501) staff       (20)      361 2023-06-06 05:17:14.000000 pipeline-feature-0.0.1/mlops_pipeline_feature_v1/pipeline_feature.egg-info/SOURCES.txt
--rw-r--r--   0 gaohn      (501) staff       (20)        1 2023-06-06 05:17:14.000000 pipeline-feature-0.0.1/mlops_pipeline_feature_v1/pipeline_feature.egg-info/dependency_links.txt
--rw-r--r--   0 gaohn      (501) staff       (20)      106 2023-06-06 05:17:14.000000 pipeline-feature-0.0.1/mlops_pipeline_feature_v1/pipeline_feature.egg-info/requires.txt
--rw-r--r--   0 gaohn      (501) staff       (20)        1 2023-06-06 05:17:14.000000 pipeline-feature-0.0.1/mlops_pipeline_feature_v1/pipeline_feature.egg-info/top_level.txt
--rw-r--r--   0 gaohn      (501) staff       (20)      983 2023-06-06 03:28:19.000000 pipeline-feature-0.0.1/pyproject.toml
--rw-r--r--   0 gaohn      (501) staff       (20)       38 2023-06-06 05:17:14.043072 pipeline-feature-0.0.1/setup.cfg
+drwxr-xr-x   0 gaohn      (501) staff       (20)        0 2023-06-06 05:25:23.363769 pipeline-feature-0.0.2/
+-rw-r--r--   0 gaohn      (501) staff       (20)     1072 2023-06-06 02:49:04.000000 pipeline-feature-0.0.2/LICENSE
+-rw-r--r--   0 gaohn      (501) staff       (20)      589 2023-06-06 05:25:23.363642 pipeline-feature-0.0.2/PKG-INFO
+-rw-r--r--   0 gaohn      (501) staff       (20)       20 2023-06-06 03:10:35.000000 pipeline-feature-0.0.2/README.md
+drwxr-xr-x   0 gaohn      (501) staff       (20)        0 2023-06-06 05:25:23.361957 pipeline-feature-0.0.2/mlops_pipeline_feature_v1/
+drwxr-xr-x   0 gaohn      (501) staff       (20)        0 2023-06-06 05:25:23.363469 pipeline-feature-0.0.2/mlops_pipeline_feature_v1/pipeline_feature.egg-info/
+-rw-r--r--   0 gaohn      (501) staff       (20)      589 2023-06-06 05:25:23.000000 pipeline-feature-0.0.2/mlops_pipeline_feature_v1/pipeline_feature.egg-info/PKG-INFO
+-rw-r--r--   0 gaohn      (501) staff       (20)      361 2023-06-06 05:25:23.000000 pipeline-feature-0.0.2/mlops_pipeline_feature_v1/pipeline_feature.egg-info/SOURCES.txt
+-rw-r--r--   0 gaohn      (501) staff       (20)        1 2023-06-06 05:25:23.000000 pipeline-feature-0.0.2/mlops_pipeline_feature_v1/pipeline_feature.egg-info/dependency_links.txt
+-rw-r--r--   0 gaohn      (501) staff       (20)      106 2023-06-06 05:25:23.000000 pipeline-feature-0.0.2/mlops_pipeline_feature_v1/pipeline_feature.egg-info/requires.txt
+-rw-r--r--   0 gaohn      (501) staff       (20)        1 2023-06-06 05:25:23.000000 pipeline-feature-0.0.2/mlops_pipeline_feature_v1/pipeline_feature.egg-info/top_level.txt
+-rw-r--r--   0 gaohn      (501) staff       (20)      983 2023-06-06 05:25:17.000000 pipeline-feature-0.0.2/pyproject.toml
+-rw-r--r--   0 gaohn      (501) staff       (20)       38 2023-06-06 05:25:23.363807 pipeline-feature-0.0.2/setup.cfg
```

### Comparing `pipeline-feature-0.0.1/LICENSE` & `pipeline-feature-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pipeline-feature-0.0.1/PKG-INFO` & `pipeline-feature-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipeline-feature
-Version: 0.0.1
+Version: 0.0.2
 Summary: Feature Pipeline of MLOps Pipeline Version 1
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/mlops-pipeline-v1
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/mlops-pipeline-v1/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pipeline-feature-0.0.1/mlops_pipeline_feature_v1/pipeline_feature.egg-info/PKG-INFO` & `pipeline-feature-0.0.2/mlops_pipeline_feature_v1/pipeline_feature.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipeline-feature
-Version: 0.0.1
+Version: 0.0.2
 Summary: Feature Pipeline of MLOps Pipeline Version 1
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/mlops-pipeline-v1
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/mlops-pipeline-v1/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pipeline-feature-0.0.1/pyproject.toml` & `pipeline-feature-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pipeline-feature"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Gao Hongnan", email="hongnangao@gmail.com" },
 ]
 description = "Feature Pipeline of MLOps Pipeline Version 1"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

