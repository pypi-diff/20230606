# Comparing `tmp/datascope-experiments-0.0.8.tar.gz` & `tmp/datascope-experiments-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datascope-experiments-0.0.8.tar", last modified: Fri Jan  6 22:33:29 2023, max compression
+gzip compressed data, was "datascope-experiments-0.0.9.tar", last modified: Sat Jan  7 11:55:37 2023, max compression
```

## Comparing `datascope-experiments-0.0.8.tar` & `datascope-experiments-0.0.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 22:33:29.252649 datascope-experiments-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-01-06 22:32:30.000000 datascope-experiments-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-01-06 22:33:29.252649 datascope-experiments-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-01-06 22:32:30.000000 datascope-experiments-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 22:33:29.248649 datascope-experiments-0.0.8/datascope/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-01-06 22:32:30.000000 datascope-experiments-0.0.8/datascope/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 22:33:29.248649 datascope-experiments-0.0.8/datascope/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-01-06 22:32:30.000000 datascope-experiments-0.0.8/datascope/experiments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-01-06 22:32:30.000000 datascope-experiments-0.0.8/datascope/experiments/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-01-06 22:32:30.000000 datascope-experiments-0.0.8/datascope/experiments/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 22:33:29.248649 datascope-experiments-0.0.8/datascope/experiments/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-01-06 22:32:30.000000 datascope-experiments-0.0.8/datascope/experiments/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42998 2023-01-06 22:32:30.000000 datascope-experiments-0.0.8/datascope/experiments/datasets/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9320 2023-01-06 22:32:30.000000 datascope-experiments-0.0.8/datascope/experiments/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 22:33:29.252649 datascope-experiments-0.0.8/datascope/experiments/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-01-06 22:32:30.000000 datascope-experiments-0.0.8/datascope/experiments/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-01-06 22:32:30.000000 datascope-experiments-0.0.8/datascope/experiments/pipelines/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-01-06 22:32:30.000000 datascope-experiments-0.0.8/datascope/experiments/pipelines/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 22:33:29.252649 datascope-experiments-0.0.8/datascope/experiments/reports/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-06 22:32:30.000000 datascope-experiments-0.0.8/datascope/experiments/reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36299 2023-01-06 22:32:30.000000 datascope-experiments-0.0.8/datascope/experiments/reports/aggregate_plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 22:33:29.252649 datascope-experiments-0.0.8/datascope/experiments/scenarios/
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-01-06 22:32:30.000000 datascope-experiments-0.0.8/datascope/experiments/scenarios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46851 2023-01-06 22:32:30.000000 datascope-experiments-0.0.8/datascope/experiments/scenarios/base.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6636 2023-01-06 22:32:30.000000 datascope-experiments-0.0.8/datascope/experiments/scenarios/compute_time.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17443 2023-01-06 22:32:30.000000 datascope-experiments-0.0.8/datascope/experiments/scenarios/data_discard.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11379 2023-01-06 22:32:30.000000 datascope-experiments-0.0.8/datascope/experiments/scenarios/datascope_scenario.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18395 2023-01-06 22:32:30.000000 datascope-experiments-0.0.8/datascope/experiments/scenarios/label_repair.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-06 22:32:30.000000 datascope-experiments-0.0.8/datascope/experiments/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-06 22:33:29.252649 datascope-experiments-0.0.8/datascope_experiments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-01-06 22:33:29.000000 datascope-experiments-0.0.8/datascope_experiments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-01-06 22:33:29.000000 datascope-experiments-0.0.8/datascope_experiments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-06 22:33:29.000000 datascope-experiments-0.0.8/datascope_experiments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-01-06 22:33:29.000000 datascope-experiments-0.0.8/datascope_experiments.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-01-06 22:33:29.000000 datascope-experiments-0.0.8/datascope_experiments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-06 22:33:29.000000 datascope-experiments-0.0.8/datascope_experiments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-01-06 22:32:30.000000 datascope-experiments-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-06 22:33:29.252649 datascope-experiments-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-01-06 22:32:30.000000 datascope-experiments-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 11:55:37.116194 datascope-experiments-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-01-07 11:55:37.116194 datascope-experiments-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 11:55:37.112194 datascope-experiments-0.0.9/datascope/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 11:55:37.112194 datascope-experiments-0.0.9/datascope/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 11:55:37.116194 datascope-experiments-0.0.9/datascope/experiments/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42998 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/datasets/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9320 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 11:55:37.116194 datascope-experiments-0.0.9/datascope/experiments/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7725 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/pipelines/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/pipelines/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 11:55:37.116194 datascope-experiments-0.0.9/datascope/experiments/reports/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36299 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/reports/aggregate_plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 11:55:37.116194 datascope-experiments-0.0.9/datascope/experiments/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/scenarios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46851 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/scenarios/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6636 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/scenarios/compute_time.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17443 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/scenarios/data_discard.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11559 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/scenarios/datascope_scenario.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18395 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/scenarios/label_repair.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/datascope/experiments/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 11:55:37.116194 datascope-experiments-0.0.9/datascope_experiments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-01-07 11:55:37.000000 datascope-experiments-0.0.9/datascope_experiments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-01-07 11:55:37.000000 datascope-experiments-0.0.9/datascope_experiments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-07 11:55:37.000000 datascope-experiments-0.0.9/datascope_experiments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-01-07 11:55:37.000000 datascope-experiments-0.0.9/datascope_experiments.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-01-07 11:55:37.000000 datascope-experiments-0.0.9/datascope_experiments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-07 11:55:37.000000 datascope-experiments-0.0.9/datascope_experiments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-07 11:55:37.116194 datascope-experiments-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-01-07 11:54:30.000000 datascope-experiments-0.0.9/setup.py
```

### Comparing `datascope-experiments-0.0.8/PKG-INFO` & `datascope-experiments-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datascope-experiments
-Version: 0.0.8
+Version: 0.0.9
 Summary: Module for running experiments on top of datascope.
 Home-page: https://ease.ml/datascope/
 Author-email: easeml@ds3lab.com
 License: MIT
 Description: # Experimental toolkit for ease.ml/datascope
         
         [![PyPI version](https://badge.fury.io/py/datascope-experiments.svg)](https://badge.fury.io/py/datascope-experiments)
```

### Comparing `datascope-experiments-0.0.8/datascope/experiments/base.py` & `datascope-experiments-0.0.9/datascope/experiments/base.py`

 * *Files identical despite different names*

### Comparing `datascope-experiments-0.0.8/datascope/experiments/datasets/__init__.py` & `datascope-experiments-0.0.9/datascope/experiments/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `datascope-experiments-0.0.8/datascope/experiments/datasets/base.py` & `datascope-experiments-0.0.9/datascope/experiments/datasets/base.py`

 * *Files identical despite different names*

### Comparing `datascope-experiments-0.0.8/datascope/experiments/main.py` & `datascope-experiments-0.0.9/datascope/experiments/main.py`

 * *Files identical despite different names*

### Comparing `datascope-experiments-0.0.8/datascope/experiments/pipelines/__init__.py` & `datascope-experiments-0.0.9/datascope/experiments/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `datascope-experiments-0.0.8/datascope/experiments/pipelines/base.py` & `datascope-experiments-0.0.9/datascope/experiments/pipelines/base.py`

 * *Files identical despite different names*

### Comparing `datascope-experiments-0.0.8/datascope/experiments/pipelines/models.py` & `datascope-experiments-0.0.9/datascope/experiments/pipelines/models.py`

 * *Files identical despite different names*

### Comparing `datascope-experiments-0.0.8/datascope/experiments/reports/aggregate_plot.py` & `datascope-experiments-0.0.9/datascope/experiments/reports/aggregate_plot.py`

 * *Files identical despite different names*

### Comparing `datascope-experiments-0.0.8/datascope/experiments/scenarios/__init__.py` & `datascope-experiments-0.0.9/datascope/experiments/scenarios/__init__.py`

 * *Files identical despite different names*

### Comparing `datascope-experiments-0.0.8/datascope/experiments/scenarios/base.py` & `datascope-experiments-0.0.9/datascope/experiments/scenarios/base.py`

 * *Files identical despite different names*

### Comparing `datascope-experiments-0.0.8/datascope/experiments/scenarios/compute_time.py` & `datascope-experiments-0.0.9/datascope/experiments/scenarios/compute_time.py`

 * *Files identical despite different names*

### Comparing `datascope-experiments-0.0.8/datascope/experiments/scenarios/data_discard.py` & `datascope-experiments-0.0.9/datascope/experiments/scenarios/data_discard.py`

 * *Files identical despite different names*

### Comparing `datascope-experiments-0.0.8/datascope/experiments/scenarios/datascope_scenario.py` & `datascope-experiments-0.0.9/datascope/experiments/scenarios/datascope_scenario.py`

 * *Files 2% similar despite different names*

```diff
@@ -312,14 +312,19 @@
 
     @property
     def dataframe(self) -> DataFrame:
         result = self._evolution.assign(
             id=self.id,
             dataset=self.dataset,
             pipeline=self.pipeline,
+            model=self.model,
+            providers=self.providers,
+            mc_timeout=self.mc_timeout,
+            mc_tolerance=self.mc_tolerance,
+            nn_k=self.nn_k,
             method=self.method,
             utility=self.utility,
             iteration=self.iteration,
         )
         if "importance_cputime" not in result.columns and self._importance_cputime is not None:
             result = result.assign(importance_cputime=self._importance_cputime)
         return result
```

### Comparing `datascope-experiments-0.0.8/datascope/experiments/scenarios/label_repair.py` & `datascope-experiments-0.0.9/datascope/experiments/scenarios/label_repair.py`

 * *Files identical despite different names*

### Comparing `datascope-experiments-0.0.8/datascope_experiments.egg-info/PKG-INFO` & `datascope-experiments-0.0.9/datascope_experiments.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datascope-experiments
-Version: 0.0.8
+Version: 0.0.9
 Summary: Module for running experiments on top of datascope.
 Home-page: https://ease.ml/datascope/
 Author-email: easeml@ds3lab.com
 License: MIT
 Description: # Experimental toolkit for ease.ml/datascope
         
         [![PyPI version](https://badge.fury.io/py/datascope-experiments.svg)](https://badge.fury.io/py/datascope-experiments)
```

### Comparing `datascope-experiments-0.0.8/datascope_experiments.egg-info/SOURCES.txt` & `datascope-experiments-0.0.9/datascope_experiments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datascope-experiments-0.0.8/setup.py` & `datascope-experiments-0.0.9/setup.py`

 * *Files identical despite different names*

