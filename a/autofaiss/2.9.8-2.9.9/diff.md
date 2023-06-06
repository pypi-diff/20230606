# Comparing `tmp/autofaiss-2.9.8.tar.gz` & `tmp/autofaiss-2.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/autofaiss-2.9.8.tar", last modified: Tue Feb 22 08:41:11 2022, max compression
+gzip compressed data, was "dist/autofaiss-2.9.9.tar", last modified: Wed Feb 23 15:22:12 2022, max compression
```

## Comparing `autofaiss-2.9.8.tar` & `autofaiss-2.9.9.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 08:41:11.000000 autofaiss-2.9.8/
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-02-22 08:40:43.000000 autofaiss-2.9.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1751 2022-02-22 08:40:43.000000 autofaiss-2.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 08:41:11.000000 autofaiss-2.9.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 08:41:11.000000 autofaiss-2.9.8/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-02-22 08:40:43.000000 autofaiss-2.9.8/tests/unit/test_np_quantize.py
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-02-22 08:40:43.000000 autofaiss-2.9.8/tests/unit/test_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     9093 2022-02-22 08:40:43.000000 autofaiss-2.9.8/tests/unit/test_quantize.py
--rw-r--r--   0 runner    (1001) docker     (121)     8248 2022-02-22 08:40:43.000000 autofaiss-2.9.8/tests/unit/test_embeddings_iterators.py
--rw-r--r--   0 runner    (1001) docker     (121)     3995 2022-02-22 08:40:43.000000 autofaiss-2.9.8/tests/unit/test_optimize.py
--rw-r--r--   0 runner    (1001) docker     (121)      345 2022-02-22 08:40:43.000000 autofaiss-2.9.8/tests/unit/test_scoring_tuning.py
--rw-r--r--   0 runner    (1001) docker     (121)      942 2022-02-22 08:40:43.000000 autofaiss-2.9.8/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-22 08:40:43.000000 autofaiss-2.9.8/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2821 2022-02-22 08:40:43.000000 autofaiss-2.9.8/tests/unit/test_mem_efficient_flat_index.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-22 08:40:43.000000 autofaiss-2.9.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-22 08:41:11.000000 autofaiss-2.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)    14864 2022-02-22 08:41:11.000000 autofaiss-2.9.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 08:41:11.000000 autofaiss-2.9.8/autofaiss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-02-22 08:41:09.000000 autofaiss-2.9.8/autofaiss.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    14864 2022-02-22 08:41:09.000000 autofaiss-2.9.8/autofaiss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1386 2022-02-22 08:41:11.000000 autofaiss-2.9.8/autofaiss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-02-22 08:41:09.000000 autofaiss-2.9.8/autofaiss.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-02-22 08:41:09.000000 autofaiss-2.9.8/autofaiss.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-22 08:41:09.000000 autofaiss-2.9.8/autofaiss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)    12907 2022-02-22 08:40:43.000000 autofaiss-2.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 08:41:11.000000 autofaiss-2.9.8/autofaiss/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 08:41:11.000000 autofaiss-2.9.8/autofaiss/readers/
--rw-r--r--   0 runner    (1001) docker     (121)    15757 2022-02-22 08:40:43.000000 autofaiss-2.9.8/autofaiss/readers/embeddings_iterators.py
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-02-22 08:40:43.000000 autofaiss-2.9.8/autofaiss/readers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 08:41:11.000000 autofaiss-2.9.8/autofaiss/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      704 2022-02-22 08:40:43.000000 autofaiss-2.9.8/autofaiss/utils/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (121)     2700 2022-02-22 08:40:43.000000 autofaiss-2.9.8/autofaiss/utils/cast.py
--rw-r--r--   0 runner    (1001) docker     (121)     2158 2022-02-22 08:40:43.000000 autofaiss-2.9.8/autofaiss/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)      448 2022-02-22 08:40:43.000000 autofaiss-2.9.8/autofaiss/utils/array_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-02-22 08:40:43.000000 autofaiss-2.9.8/autofaiss/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 08:41:11.000000 autofaiss-2.9.8/autofaiss/metrics/
--rw-r--r--   0 runner    (1001) docker     (121)     3619 2022-02-22 08:40:43.000000 autofaiss-2.9.8/autofaiss/metrics/recalls.py
--rw-r--r--   0 runner    (1001) docker     (121)     4215 2022-02-22 08:40:43.000000 autofaiss-2.9.8/autofaiss/metrics/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-02-22 08:40:43.000000 autofaiss-2.9.8/autofaiss/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      792 2022-02-22 08:40:43.000000 autofaiss-2.9.8/autofaiss/metrics/reconstruction.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 08:41:11.000000 autofaiss-2.9.8/autofaiss/indices/
--rw-r--r--   0 runner    (1001) docker     (121)    10743 2022-02-22 08:40:43.000000 autofaiss-2.9.8/autofaiss/indices/memory_efficient_flat_index.py
--rw-r--r--   0 runner    (1001) docker     (121)      441 2022-02-22 08:40:43.000000 autofaiss-2.9.8/autofaiss/indices/search.py
--rw-r--r--   0 runner    (1001) docker     (121)     4379 2022-02-22 08:40:43.000000 autofaiss-2.9.8/autofaiss/indices/index_factory.py
--rw-r--r--   0 runner    (1001) docker     (121)     2280 2022-02-22 08:40:43.000000 autofaiss-2.9.8/autofaiss/indices/faiss_index_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)     4186 2022-02-22 08:40:43.000000 autofaiss-2.9.8/autofaiss/indices/index_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-02-22 08:40:43.000000 autofaiss-2.9.8/autofaiss/indices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14319 2022-02-22 08:40:43.000000 autofaiss-2.9.8/autofaiss/indices/distributed.py
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-02-22 08:40:43.000000 autofaiss-2.9.8/autofaiss/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-22 08:41:11.000000 autofaiss-2.9.8/autofaiss/external/
--rw-r--r--   0 runner    (1001) docker     (121)     5660 2022-02-22 08:40:43.000000 autofaiss-2.9.8/autofaiss/external/scores.py
--rw-r--r--   0 runner    (1001) docker     (121)     4318 2022-02-22 08:40:43.000000 autofaiss-2.9.8/autofaiss/external/descriptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     9424 2022-02-22 08:40:43.000000 autofaiss-2.9.8/autofaiss/external/build.py
--rw-r--r--   0 runner    (1001) docker     (121)    18881 2022-02-22 08:40:43.000000 autofaiss-2.9.8/autofaiss/external/quantize.py
--rw-r--r--   0 runner    (1001) docker     (121)     8215 2022-02-22 08:40:43.000000 autofaiss-2.9.8/autofaiss/external/metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)    15220 2022-02-22 08:40:43.000000 autofaiss-2.9.8/autofaiss/external/optimize.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-22 08:40:43.000000 autofaiss-2.9.8/autofaiss/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-02-22 08:40:43.000000 autofaiss-2.9.8/autofaiss/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 15:22:12.000000 autofaiss-2.9.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      147 2022-02-23 15:21:51.000000 autofaiss-2.9.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1751 2022-02-23 15:21:51.000000 autofaiss-2.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 15:22:12.000000 autofaiss-2.9.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 15:22:12.000000 autofaiss-2.9.9/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (121)      231 2022-02-23 15:21:51.000000 autofaiss-2.9.9/tests/unit/test_np_quantize.py
+-rw-r--r--   0 runner    (1001) docker     (121)      196 2022-02-23 15:21:51.000000 autofaiss-2.9.9/tests/unit/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9093 2022-02-23 15:21:51.000000 autofaiss-2.9.9/tests/unit/test_quantize.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8248 2022-02-23 15:21:51.000000 autofaiss-2.9.9/tests/unit/test_embeddings_iterators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3995 2022-02-23 15:21:51.000000 autofaiss-2.9.9/tests/unit/test_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (121)      345 2022-02-23 15:21:51.000000 autofaiss-2.9.9/tests/unit/test_scoring_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (121)      942 2022-02-23 15:21:51.000000 autofaiss-2.9.9/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-23 15:21:51.000000 autofaiss-2.9.9/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2821 2022-02-23 15:21:51.000000 autofaiss-2.9.9/tests/unit/test_mem_efficient_flat_index.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-23 15:21:51.000000 autofaiss-2.9.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-23 15:22:12.000000 autofaiss-2.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)    14864 2022-02-23 15:22:12.000000 autofaiss-2.9.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 15:22:12.000000 autofaiss-2.9.9/autofaiss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-02-23 15:22:12.000000 autofaiss-2.9.9/autofaiss.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    14864 2022-02-23 15:22:12.000000 autofaiss-2.9.9/autofaiss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1386 2022-02-23 15:22:12.000000 autofaiss-2.9.9/autofaiss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      148 2022-02-23 15:22:12.000000 autofaiss-2.9.9/autofaiss.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-02-23 15:22:12.000000 autofaiss-2.9.9/autofaiss.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-23 15:22:12.000000 autofaiss-2.9.9/autofaiss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    12907 2022-02-23 15:21:51.000000 autofaiss-2.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 15:22:12.000000 autofaiss-2.9.9/autofaiss/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 15:22:12.000000 autofaiss-2.9.9/autofaiss/readers/
+-rw-r--r--   0 runner    (1001) docker     (121)    15757 2022-02-23 15:21:51.000000 autofaiss-2.9.9/autofaiss/readers/embeddings_iterators.py
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2022-02-23 15:21:51.000000 autofaiss-2.9.9/autofaiss/readers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 15:22:12.000000 autofaiss-2.9.9/autofaiss/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)      704 2022-02-23 15:21:51.000000 autofaiss-2.9.9/autofaiss/utils/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2700 2022-02-23 15:21:51.000000 autofaiss-2.9.9/autofaiss/utils/cast.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2158 2022-02-23 15:21:51.000000 autofaiss-2.9.9/autofaiss/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (121)      448 2022-02-23 15:21:51.000000 autofaiss-2.9.9/autofaiss/utils/array_functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2022-02-23 15:21:51.000000 autofaiss-2.9.9/autofaiss/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 15:22:12.000000 autofaiss-2.9.9/autofaiss/metrics/
+-rw-r--r--   0 runner    (1001) docker     (121)     3619 2022-02-23 15:21:51.000000 autofaiss-2.9.9/autofaiss/metrics/recalls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4215 2022-02-23 15:21:51.000000 autofaiss-2.9.9/autofaiss/metrics/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2022-02-23 15:21:51.000000 autofaiss-2.9.9/autofaiss/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      792 2022-02-23 15:21:51.000000 autofaiss-2.9.9/autofaiss/metrics/reconstruction.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 15:22:12.000000 autofaiss-2.9.9/autofaiss/indices/
+-rw-r--r--   0 runner    (1001) docker     (121)    10743 2022-02-23 15:21:51.000000 autofaiss-2.9.9/autofaiss/indices/memory_efficient_flat_index.py
+-rw-r--r--   0 runner    (1001) docker     (121)      441 2022-02-23 15:21:51.000000 autofaiss-2.9.9/autofaiss/indices/search.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4379 2022-02-23 15:21:51.000000 autofaiss-2.9.9/autofaiss/indices/index_factory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2280 2022-02-23 15:21:51.000000 autofaiss-2.9.9/autofaiss/indices/faiss_index_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4186 2022-02-23 15:21:51.000000 autofaiss-2.9.9/autofaiss/indices/index_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2022-02-23 15:21:51.000000 autofaiss-2.9.9/autofaiss/indices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14321 2022-02-23 15:21:51.000000 autofaiss-2.9.9/autofaiss/indices/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (121)      183 2022-02-23 15:21:51.000000 autofaiss-2.9.9/autofaiss/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-23 15:22:12.000000 autofaiss-2.9.9/autofaiss/external/
+-rw-r--r--   0 runner    (1001) docker     (121)     5660 2022-02-23 15:21:51.000000 autofaiss-2.9.9/autofaiss/external/scores.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4318 2022-02-23 15:21:51.000000 autofaiss-2.9.9/autofaiss/external/descriptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9424 2022-02-23 15:21:51.000000 autofaiss-2.9.9/autofaiss/external/build.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18881 2022-02-23 15:21:51.000000 autofaiss-2.9.9/autofaiss/external/quantize.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8215 2022-02-23 15:21:51.000000 autofaiss-2.9.9/autofaiss/external/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15220 2022-02-23 15:21:51.000000 autofaiss-2.9.9/autofaiss/external/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-02-23 15:21:51.000000 autofaiss-2.9.9/autofaiss/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      171 2022-02-23 15:21:51.000000 autofaiss-2.9.9/autofaiss/version.py
```

### Comparing `autofaiss-2.9.8/setup.py` & `autofaiss-2.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `autofaiss-2.9.8/tests/unit/test_quantize.py` & `autofaiss-2.9.9/tests/unit/test_quantize.py`

 * *Files identical despite different names*

### Comparing `autofaiss-2.9.8/tests/unit/test_embeddings_iterators.py` & `autofaiss-2.9.9/tests/unit/test_embeddings_iterators.py`

 * *Files identical despite different names*

### Comparing `autofaiss-2.9.8/tests/unit/test_optimize.py` & `autofaiss-2.9.9/tests/unit/test_optimize.py`

 * *Files identical despite different names*

### Comparing `autofaiss-2.9.8/tests/unit/test_utils.py` & `autofaiss-2.9.9/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `autofaiss-2.9.8/tests/unit/test_mem_efficient_flat_index.py` & `autofaiss-2.9.9/tests/unit/test_mem_efficient_flat_index.py`

 * *Files identical despite different names*

### Comparing `autofaiss-2.9.8/PKG-INFO` & `autofaiss-2.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autofaiss
-Version: 2.9.8
+Version: 2.9.9
 Summary: # AutoFaiss
 Home-page: https://github.com/criteo/autofaiss
 Author: Criteo
 License: UNKNOWN
 Description: # AutoFaiss
         
         [![pypi](https://img.shields.io/pypi/v/autofaiss.svg)](https://pypi.python.org/pypi/autofaiss)
```

### Comparing `autofaiss-2.9.8/autofaiss.egg-info/PKG-INFO` & `autofaiss-2.9.9/autofaiss.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autofaiss
-Version: 2.9.8
+Version: 2.9.9
 Summary: # AutoFaiss
 Home-page: https://github.com/criteo/autofaiss
 Author: Criteo
 License: UNKNOWN
 Description: # AutoFaiss
         
         [![pypi](https://img.shields.io/pypi/v/autofaiss.svg)](https://pypi.python.org/pypi/autofaiss)
```

### Comparing `autofaiss-2.9.8/autofaiss.egg-info/SOURCES.txt` & `autofaiss-2.9.9/autofaiss.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autofaiss-2.9.8/README.md` & `autofaiss-2.9.9/README.md`

 * *Files identical despite different names*

### Comparing `autofaiss-2.9.8/autofaiss/readers/embeddings_iterators.py` & `autofaiss-2.9.9/autofaiss/readers/embeddings_iterators.py`

 * *Files identical despite different names*

### Comparing `autofaiss-2.9.8/autofaiss/utils/algorithms.py` & `autofaiss-2.9.9/autofaiss/utils/algorithms.py`

 * *Files identical despite different names*

### Comparing `autofaiss-2.9.8/autofaiss/utils/cast.py` & `autofaiss-2.9.9/autofaiss/utils/cast.py`

 * *Files identical despite different names*

### Comparing `autofaiss-2.9.8/autofaiss/utils/decorators.py` & `autofaiss-2.9.9/autofaiss/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `autofaiss-2.9.8/autofaiss/metrics/recalls.py` & `autofaiss-2.9.9/autofaiss/metrics/recalls.py`

 * *Files identical despite different names*

### Comparing `autofaiss-2.9.8/autofaiss/metrics/benchmark.py` & `autofaiss-2.9.9/autofaiss/metrics/benchmark.py`

 * *Files identical despite different names*

### Comparing `autofaiss-2.9.8/autofaiss/metrics/reconstruction.py` & `autofaiss-2.9.9/autofaiss/metrics/reconstruction.py`

 * *Files identical despite different names*

### Comparing `autofaiss-2.9.8/autofaiss/indices/memory_efficient_flat_index.py` & `autofaiss-2.9.9/autofaiss/indices/memory_efficient_flat_index.py`

 * *Files identical despite different names*

### Comparing `autofaiss-2.9.8/autofaiss/indices/index_factory.py` & `autofaiss-2.9.9/autofaiss/indices/index_factory.py`

 * *Files identical despite different names*

### Comparing `autofaiss-2.9.8/autofaiss/indices/faiss_index_wrapper.py` & `autofaiss-2.9.9/autofaiss/indices/faiss_index_wrapper.py`

 * *Files identical despite different names*

### Comparing `autofaiss-2.9.8/autofaiss/indices/index_utils.py` & `autofaiss-2.9.9/autofaiss/indices/index_utils.py`

 * *Files identical despite different names*

### Comparing `autofaiss-2.9.8/autofaiss/indices/distributed.py` & `autofaiss-2.9.9/autofaiss/indices/distributed.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,22 +38,22 @@
 ):
     """Lazy load a batch of embeddings."""
     if isinstance(file_system, PyArrowHDFS):
         file_system = get_filesystem_class("hdfs")()
     cur_start = cur_end = 0
     for chunk_size, file_path in zip(chunk_sizes, embeddings_paths):
         cur_end += chunk_size
-        if cur_end < start:
+        if cur_end <= start:
             cur_start += chunk_size
             continue
         slice_start = max(0, start - cur_start)
         slice_end = min(chunk_size, end - cur_start)
         with get_matrix_reader(file_format, file_system, file_path, embedding_column_name, id_columns) as matrix_reader:
             yield matrix_reader.get_lazy_array().get_rows(start=slice_start, end=slice_end)
-        if cur_end > end:
+        if cur_end >= end:
             break
         cur_start += chunk_size
 
 
 def _generate_small_index_file_name(batch_id: int, nb_batches: int) -> str:
     suffix_width = int(math.log10(nb_batches)) + 1
     return "index_" + str(batch_id).zfill(suffix_width)
```

### Comparing `autofaiss-2.9.8/autofaiss/external/scores.py` & `autofaiss-2.9.9/autofaiss/external/scores.py`

 * *Files identical despite different names*

### Comparing `autofaiss-2.9.8/autofaiss/external/descriptions.py` & `autofaiss-2.9.9/autofaiss/external/descriptions.py`

 * *Files identical despite different names*

### Comparing `autofaiss-2.9.8/autofaiss/external/build.py` & `autofaiss-2.9.9/autofaiss/external/build.py`

 * *Files identical despite different names*

### Comparing `autofaiss-2.9.8/autofaiss/external/quantize.py` & `autofaiss-2.9.9/autofaiss/external/quantize.py`

 * *Files identical despite different names*

### Comparing `autofaiss-2.9.8/autofaiss/external/metadata.py` & `autofaiss-2.9.9/autofaiss/external/metadata.py`

 * *Files identical despite different names*

### Comparing `autofaiss-2.9.8/autofaiss/external/optimize.py` & `autofaiss-2.9.9/autofaiss/external/optimize.py`

 * *Files identical despite different names*

