# Comparing `tmp/pyoptmat-1.3.0.tar.gz` & `tmp/pyoptmat-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyoptmat-1.3.0.tar", last modified: Wed May 10 19:50:08 2023, max compression
+gzip compressed data, was "pyoptmat-1.3.1.tar", last modified: Tue Jun  6 18:09:45 2023, max compression
```

## Comparing `pyoptmat-1.3.0.tar` & `pyoptmat-1.3.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:50:08.541592 pyoptmat-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-10 19:50:08.541592 pyoptmat-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:50:08.541592 pyoptmat-1.3.0/pyoptmat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/pyoptmat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21760 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/pyoptmat/chunktime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/pyoptmat/damage.py
--rw-r--r--   0 runner    (1001) docker     (123)    18369 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/pyoptmat/experiments.py
--rw-r--r--   0 runner    (1001) docker     (123)    46061 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/pyoptmat/flowrules.py
--rw-r--r--   0 runner    (1001) docker     (123)    35630 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/pyoptmat/hardening.py
--rw-r--r--   0 runner    (1001) docker     (123)    15812 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/pyoptmat/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/pyoptmat/neuralode.py
--rw-r--r--   0 runner    (1001) docker     (123)    24843 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/pyoptmat/ode.py
--rw-r--r--   0 runner    (1001) docker     (123)    19718 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/pyoptmat/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/pyoptmat/scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)    12202 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/pyoptmat/solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18011 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/pyoptmat/temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)    14860 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/pyoptmat/utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:50:08.541592 pyoptmat-1.3.0/pyoptmat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-10 19:50:08.000000 pyoptmat-1.3.0/pyoptmat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-10 19:50:08.000000 pyoptmat-1.3.0/pyoptmat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 19:50:08.000000 pyoptmat-1.3.0/pyoptmat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-10 19:50:08.000000 pyoptmat-1.3.0/pyoptmat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-10 19:50:08.000000 pyoptmat-1.3.0/pyoptmat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 19:50:08.000000 pyoptmat-1.3.0/pyoptmat.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-10 19:50:08.541592 pyoptmat-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 19:50:08.541592 pyoptmat-1.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)    13085 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/test/test_adjoint_gradients.py
--rw-r--r--   0 runner    (1001) docker     (123)    35434 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/test/test_batch_gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/test/test_chunktime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/test/test_damage.py
--rw-r--r--   0 runner    (1001) docker     (123)    20725 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/test/test_flowrules.py
--rw-r--r--   0 runner    (1001) docker     (123)    18620 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/test/test_hardening.py
--rw-r--r--   0 runner    (1001) docker     (123)    13211 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/test/test_model_gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)    16944 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/test/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9162 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/test/test_ode.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/test/test_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/test/test_solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16483 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/test/test_temperature_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-05-10 19:50:04.000000 pyoptmat-1.3.0/test/test_utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:09:45.462954 pyoptmat-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-06-06 18:09:45.462954 pyoptmat-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:09:45.462954 pyoptmat-1.3.1/pyoptmat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/pyoptmat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21760 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/pyoptmat/chunktime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/pyoptmat/damage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18369 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/pyoptmat/experiments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46061 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/pyoptmat/flowrules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35630 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/pyoptmat/hardening.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15812 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/pyoptmat/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/pyoptmat/neuralode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24843 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/pyoptmat/ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19718 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/pyoptmat/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/pyoptmat/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12202 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/pyoptmat/solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18011 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/pyoptmat/temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14860 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/pyoptmat/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:09:45.462954 pyoptmat-1.3.1/pyoptmat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-06-06 18:09:45.000000 pyoptmat-1.3.1/pyoptmat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-06 18:09:45.000000 pyoptmat-1.3.1/pyoptmat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 18:09:45.000000 pyoptmat-1.3.1/pyoptmat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-06 18:09:45.000000 pyoptmat-1.3.1/pyoptmat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-06 18:09:45.000000 pyoptmat-1.3.1/pyoptmat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 18:09:45.000000 pyoptmat-1.3.1/pyoptmat.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-06 18:09:45.462954 pyoptmat-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:09:45.462954 pyoptmat-1.3.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    13085 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/test/test_adjoint_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35434 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/test/test_batch_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/test/test_chunktime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/test/test_damage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20725 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/test/test_flowrules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18620 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/test/test_hardening.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13211 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/test/test_model_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16944 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/test/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9162 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/test/test_ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/test/test_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/test/test_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16483 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/test/test_temperature_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7769 2023-06-06 18:09:41.000000 pyoptmat-1.3.1/test/test_utility.py
```

### Comparing `pyoptmat-1.3.0/LICENSE` & `pyoptmat-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.0/PKG-INFO` & `pyoptmat-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyoptmat
-Version: 1.3.0
+Version: 1.3.1
 Summary: Statistical inference for material models
 Home-page: https://github.com/Argonne-National-Laboratory/pyoptmat
 Author: Argonne National Laboratory
 Author-email: messner@anl.gov
 License: UNKNOWN
 Keywords: materials inference modeling
 Platform: UNKNOWN
```

### Comparing `pyoptmat-1.3.0/README.md` & `pyoptmat-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.0/pyoptmat/chunktime.py` & `pyoptmat-1.3.1/pyoptmat/chunktime.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.0/pyoptmat/damage.py` & `pyoptmat-1.3.1/pyoptmat/damage.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.0/pyoptmat/experiments.py` & `pyoptmat-1.3.1/pyoptmat/experiments.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.0/pyoptmat/flowrules.py` & `pyoptmat-1.3.1/pyoptmat/flowrules.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.0/pyoptmat/hardening.py` & `pyoptmat-1.3.1/pyoptmat/hardening.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.0/pyoptmat/models.py` & `pyoptmat-1.3.1/pyoptmat/models.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.0/pyoptmat/neuralode.py` & `pyoptmat-1.3.1/pyoptmat/neuralode.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.0/pyoptmat/ode.py` & `pyoptmat-1.3.1/pyoptmat/ode.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.0/pyoptmat/optimize.py` & `pyoptmat-1.3.1/pyoptmat/optimize.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.0/pyoptmat/scaling.py` & `pyoptmat-1.3.1/pyoptmat/scaling.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.0/pyoptmat/solvers.py` & `pyoptmat-1.3.1/pyoptmat/solvers.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.0/pyoptmat/temperature.py` & `pyoptmat-1.3.1/pyoptmat/temperature.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.0/pyoptmat/utility.py` & `pyoptmat-1.3.1/pyoptmat/utility.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.0/pyoptmat.egg-info/PKG-INFO` & `pyoptmat-1.3.1/pyoptmat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyoptmat
-Version: 1.3.0
+Version: 1.3.1
 Summary: Statistical inference for material models
 Home-page: https://github.com/Argonne-National-Laboratory/pyoptmat
 Author: Argonne National Laboratory
 Author-email: messner@anl.gov
 License: UNKNOWN
 Keywords: materials inference modeling
 Platform: UNKNOWN
```

### Comparing `pyoptmat-1.3.0/pyoptmat.egg-info/SOURCES.txt` & `pyoptmat-1.3.1/pyoptmat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.0/setup.py` & `pyoptmat-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 with open(os.path.join(this_directory, 'README.md'), encoding = 'utf-8') as f:
   long_description = f.read()
 
 setup (
     # Name of the project
     name = 'pyoptmat',
     # Version
-    version = '1.3.0',
+    version = '1.3.1',
     # One line-description
     description = "Statistical inference for material models",
     # README
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     # Project webpage
     url='https://github.com/Argonne-National-Laboratory/pyoptmat',
```

### Comparing `pyoptmat-1.3.0/test/test_adjoint_gradients.py` & `pyoptmat-1.3.1/test/test_adjoint_gradients.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.0/test/test_batch_gradient.py` & `pyoptmat-1.3.1/test/test_batch_gradient.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.0/test/test_chunktime.py` & `pyoptmat-1.3.1/test/test_chunktime.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.0/test/test_damage.py` & `pyoptmat-1.3.1/test/test_damage.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.0/test/test_flowrules.py` & `pyoptmat-1.3.1/test/test_flowrules.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.0/test/test_hardening.py` & `pyoptmat-1.3.1/test/test_hardening.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.0/test/test_model_gradient.py` & `pyoptmat-1.3.1/test/test_model_gradient.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.0/test/test_models.py` & `pyoptmat-1.3.1/test/test_models.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.0/test/test_ode.py` & `pyoptmat-1.3.1/test/test_ode.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.0/test/test_scaling.py` & `pyoptmat-1.3.1/test/test_scaling.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.0/test/test_solvers.py` & `pyoptmat-1.3.1/test/test_solvers.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.0/test/test_temperature_scaling.py` & `pyoptmat-1.3.1/test/test_temperature_scaling.py`

 * *Files identical despite different names*

### Comparing `pyoptmat-1.3.0/test/test_utility.py` & `pyoptmat-1.3.1/test/test_utility.py`

 * *Files identical despite different names*

