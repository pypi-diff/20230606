# Comparing `tmp/thsolver-1.1.3.tar.gz` & `tmp/thsolver-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thsolver-1.1.3.tar", last modified: Sat Jun  3 03:40:21 2023, max compression
+gzip compressed data, was "thsolver-1.1.4.tar", last modified: Tue Jun  6 03:28:24 2023, max compression
```

## Comparing `thsolver-1.1.3.tar` & `thsolver-1.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 wangps    (1001) wangps    (1001)        0 2023-06-03 03:40:21.684440 thsolver-1.1.3/
--rw-rw-r--   0 wangps    (1001) wangps    (1001)     1093 2022-10-25 12:13:18.000000 thsolver-1.1.3/LICENSE
--rw-rw-r--   0 wangps    (1001) wangps    (1001)      867 2023-06-03 03:40:21.684440 thsolver-1.1.3/PKG-INFO
--rw-rw-r--   0 wangps    (1001) wangps    (1001)      430 2023-06-01 09:42:54.000000 thsolver-1.1.3/README.md
--rw-rw-r--   0 wangps    (1001) wangps    (1001)      107 2023-06-03 03:40:21.684440 thsolver-1.1.3/setup.cfg
--rw-rw-r--   0 wangps    (1001) wangps    (1001)     1133 2023-06-03 03:13:18.000000 thsolver-1.1.3/setup.py
-drwxrwxr-x   0 wangps    (1001) wangps    (1001)        0 2023-06-03 03:40:21.684440 thsolver-1.1.3/thsolver/
--rw-rw-r--   0 wangps    (1001) wangps    (1001)      782 2023-06-01 09:42:51.000000 thsolver-1.1.3/thsolver/__init__.py
--rw-rw-r--   0 wangps    (1001) wangps    (1001)     7026 2023-06-03 03:14:22.000000 thsolver-1.1.3/thsolver/config.py
--rw-rw-r--   0 wangps    (1001) wangps    (1001)     2075 2023-06-01 09:42:51.000000 thsolver-1.1.3/thsolver/dataset.py
--rw-rw-r--   0 wangps    (1001) wangps    (1001)     2354 2022-10-25 12:13:18.000000 thsolver-1.1.3/thsolver/lr_scheduler.py
--rw-rw-r--   0 wangps    (1001) wangps    (1001)     1209 2023-06-01 09:51:14.000000 thsolver-1.1.3/thsolver/registry.py
--rw-rw-r--   0 wangps    (1001) wangps    (1001)     1555 2022-10-25 12:13:18.000000 thsolver-1.1.3/thsolver/sampler.py
--rw-rw-r--   0 wangps    (1001) wangps    (1001)    14718 2023-06-01 09:42:54.000000 thsolver-1.1.3/thsolver/solver.py
--rw-rw-r--   0 wangps    (1001) wangps    (1001)     3067 2023-06-01 09:42:54.000000 thsolver-1.1.3/thsolver/tracker.py
-drwxrwxr-x   0 wangps    (1001) wangps    (1001)        0 2023-06-03 03:40:21.684440 thsolver-1.1.3/thsolver.egg-info/
--rw-rw-r--   0 wangps    (1001) wangps    (1001)      867 2023-06-03 03:40:21.000000 thsolver-1.1.3/thsolver.egg-info/PKG-INFO
--rw-rw-r--   0 wangps    (1001) wangps    (1001)      391 2023-06-03 03:40:21.000000 thsolver-1.1.3/thsolver.egg-info/SOURCES.txt
--rw-rw-r--   0 wangps    (1001) wangps    (1001)        1 2023-06-03 03:40:21.000000 thsolver-1.1.3/thsolver.egg-info/dependency_links.txt
--rw-rw-r--   0 wangps    (1001) wangps    (1001)        1 2022-10-26 01:01:16.000000 thsolver-1.1.3/thsolver.egg-info/not-zip-safe
--rw-rw-r--   0 wangps    (1001) wangps    (1001)       22 2023-06-03 03:40:21.000000 thsolver-1.1.3/thsolver.egg-info/requires.txt
--rw-rw-r--   0 wangps    (1001) wangps    (1001)        9 2023-06-03 03:40:21.000000 thsolver-1.1.3/thsolver.egg-info/top_level.txt
+drwxrwxr-x   0 wangps    (1001) wangps    (1001)        0 2023-06-06 03:28:24.460970 thsolver-1.1.4/
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)     1093 2022-10-25 12:13:18.000000 thsolver-1.1.4/LICENSE
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)      867 2023-06-06 03:28:24.460970 thsolver-1.1.4/PKG-INFO
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)      430 2023-06-01 09:42:54.000000 thsolver-1.1.4/README.md
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)      107 2023-06-06 03:28:24.460970 thsolver-1.1.4/setup.cfg
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)     1133 2023-06-06 03:26:21.000000 thsolver-1.1.4/setup.py
+drwxrwxr-x   0 wangps    (1001) wangps    (1001)        0 2023-06-06 03:28:24.460970 thsolver-1.1.4/thsolver/
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)      782 2023-06-01 09:42:51.000000 thsolver-1.1.4/thsolver/__init__.py
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)     7026 2023-06-03 03:14:22.000000 thsolver-1.1.4/thsolver/config.py
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)     2075 2023-06-01 09:42:51.000000 thsolver-1.1.4/thsolver/dataset.py
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)     2354 2022-10-25 12:13:18.000000 thsolver-1.1.4/thsolver/lr_scheduler.py
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)     1209 2023-06-01 09:51:14.000000 thsolver-1.1.4/thsolver/registry.py
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)     1555 2022-10-25 12:13:18.000000 thsolver-1.1.4/thsolver/sampler.py
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)    14794 2023-06-05 14:26:07.000000 thsolver-1.1.4/thsolver/solver.py
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)     3067 2023-06-01 09:42:54.000000 thsolver-1.1.4/thsolver/tracker.py
+drwxrwxr-x   0 wangps    (1001) wangps    (1001)        0 2023-06-06 03:28:24.460970 thsolver-1.1.4/thsolver.egg-info/
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)      867 2023-06-06 03:28:24.000000 thsolver-1.1.4/thsolver.egg-info/PKG-INFO
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)      391 2023-06-06 03:28:24.000000 thsolver-1.1.4/thsolver.egg-info/SOURCES.txt
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)        1 2023-06-06 03:28:24.000000 thsolver-1.1.4/thsolver.egg-info/dependency_links.txt
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)        1 2022-10-26 01:01:16.000000 thsolver-1.1.4/thsolver.egg-info/not-zip-safe
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)       22 2023-06-06 03:28:24.000000 thsolver-1.1.4/thsolver.egg-info/requires.txt
+-rw-rw-r--   0 wangps    (1001) wangps    (1001)        9 2023-06-06 03:28:24.000000 thsolver-1.1.4/thsolver.egg-info/top_level.txt
```

### Comparing `thsolver-1.1.3/LICENSE` & `thsolver-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `thsolver-1.1.3/PKG-INFO` & `thsolver-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thsolver
-Version: 1.1.3
+Version: 1.1.4
 Summary: Solver for PyTorch
 Home-page: https://github.com/octree-nn/solver-pytorch
 Author: Peng-Shuai Wang
 Author-email: wangps@hotmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `thsolver-1.1.3/setup.py` & `thsolver-1.1.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright (c) 2022 Peng-Shuai Wang <wangps@hotmail.com>
 # Licensed under The MIT License [see LICENSE for details]
 # Written by Peng-Shuai Wang
 # --------------------------------------------------------
 
 from setuptools import setup, find_packages
 
-__version__ = '1.1.3'
+__version__ = '1.1.4'
 
 with open("README.md", "r", encoding="utf-8") as fid:
   long_description = fid.read()
 
 setup(
     name='thsolver',
     version=__version__,
```

### Comparing `thsolver-1.1.3/thsolver/__init__.py` & `thsolver-1.1.4/thsolver/__init__.py`

 * *Files identical despite different names*

### Comparing `thsolver-1.1.3/thsolver/config.py` & `thsolver-1.1.4/thsolver/config.py`

 * *Files identical despite different names*

### Comparing `thsolver-1.1.3/thsolver/dataset.py` & `thsolver-1.1.4/thsolver/dataset.py`

 * *Files identical despite different names*

### Comparing `thsolver-1.1.3/thsolver/lr_scheduler.py` & `thsolver-1.1.4/thsolver/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `thsolver-1.1.3/thsolver/registry.py` & `thsolver-1.1.4/thsolver/registry.py`

 * *Files identical despite different names*

### Comparing `thsolver-1.1.3/thsolver/sampler.py` & `thsolver-1.1.4/thsolver/sampler.py`

 * *Files identical despite different names*

### Comparing `thsolver-1.1.3/thsolver/solver.py` & `thsolver-1.1.4/thsolver/solver.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,15 +217,16 @@
       batch['iter_num'] = it
       batch['epoch'] = epoch
       with torch.no_grad():
         self.eval_step(batch)
 
   def save_best_checkpoint(self, tracker: AverageTracker, epoch: int):
     best_val = self.FLAGS.SOLVER.best_val
-    if not best_val: return  # return if best_val is empty
+    if not (best_val and self.FLAGS.SOLVER.run == 'train'):
+      return  # return if best_val is empty or it is not in the train mode
 
     compare, key = best_val.split(':')
     key = 'test/' + key
     assert compare in ['max', 'min']
     operator = lambda x, y: x > y if compare == 'max' else x < y
 
     if key in tracker.value:
```

### Comparing `thsolver-1.1.3/thsolver/tracker.py` & `thsolver-1.1.4/thsolver/tracker.py`

 * *Files identical despite different names*

### Comparing `thsolver-1.1.3/thsolver.egg-info/PKG-INFO` & `thsolver-1.1.4/thsolver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thsolver
-Version: 1.1.3
+Version: 1.1.4
 Summary: Solver for PyTorch
 Home-page: https://github.com/octree-nn/solver-pytorch
 Author: Peng-Shuai Wang
 Author-email: wangps@hotmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

