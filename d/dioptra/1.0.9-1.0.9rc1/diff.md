# Comparing `tmp/dioptra-1.0.9.tar.gz` & `tmp/dioptra-1.0.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dioptra-1.0.9.tar", last modified: Thu Apr 13 18:56:06 2023, max compression
+gzip compressed data, was "dioptra-1.0.9rc1.tar", last modified: Thu Apr 13 04:32:02 2023, max compression
```

## Comparing `dioptra-1.0.9.tar` & `dioptra-1.0.9rc1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 18:56:06.115201 dioptra-1.0.9/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1471 2023-04-13 18:56:05.000000 dioptra-1.0.9/LICENSE.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2159 2023-04-13 18:56:06.115201 dioptra-1.0.9/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1106 2023-04-13 18:56:05.000000 dioptra-1.0.9/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 18:56:06.111200 dioptra-1.0.9/dioptra/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       22 2023-04-13 18:56:05.000000 dioptra-1.0.9/dioptra/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 18:56:06.111200 dioptra-1.0.9/dioptra/inference/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-13 18:56:05.000000 dioptra-1.0.9/dioptra/inference/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1637 2023-04-13 18:56:05.000000 dioptra-1.0.9/dioptra/inference/inference_runner.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 18:56:06.111200 dioptra-1.0.9/dioptra/inference/tf/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-13 18:56:05.000000 dioptra-1.0.9/dioptra/inference/tf/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5707 2023-04-13 18:56:05.000000 dioptra-1.0.9/dioptra/inference/tf/tf_runner.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 18:56:06.111200 dioptra-1.0.9/dioptra/inference/torch/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-13 18:56:05.000000 dioptra-1.0.9/dioptra/inference/torch/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6900 2023-04-13 18:56:05.000000 dioptra-1.0.9/dioptra/inference/torch/torch_runner.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 18:56:06.115201 dioptra-1.0.9/dioptra/lake/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-13 18:56:05.000000 dioptra-1.0.9/dioptra/lake/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8352 2023-04-13 18:56:05.000000 dioptra-1.0.9/dioptra/lake/datasets.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 18:56:06.115201 dioptra-1.0.9/dioptra/lake/torch/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-13 18:56:05.000000 dioptra-1.0.9/dioptra/lake/torch/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4545 2023-04-13 18:56:05.000000 dioptra-1.0.9/dioptra/lake/torch/object_store_datasets.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    29031 2023-04-13 18:56:05.000000 dioptra-1.0.9/dioptra/lake/utils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 18:56:06.115201 dioptra-1.0.9/dioptra/miners/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      416 2023-04-13 18:56:05.000000 dioptra-1.0.9/dioptra/miners/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3151 2023-04-13 18:56:05.000000 dioptra-1.0.9/dioptra/miners/activation_miner.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4382 2023-04-13 18:56:05.000000 dioptra-1.0.9/dioptra/miners/base_miner.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3533 2023-04-13 18:56:05.000000 dioptra-1.0.9/dioptra/miners/coreset_miner.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2105 2023-04-13 18:56:05.000000 dioptra-1.0.9/dioptra/miners/entropy_miner.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3511 2023-04-13 18:56:05.000000 dioptra-1.0.9/dioptra/miners/knn_miner.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2090 2023-04-13 18:56:05.000000 dioptra-1.0.9/dioptra/miners/random_miner.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2107 2023-04-13 18:56:05.000000 dioptra-1.0.9/dioptra/miners/variance_miner.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 18:56:06.111200 dioptra-1.0.9/dioptra.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2159 2023-04-13 18:56:06.000000 dioptra-1.0.9/dioptra.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      808 2023-04-13 18:56:06.000000 dioptra-1.0.9/dioptra.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-13 18:56:06.000000 dioptra-1.0.9/dioptra.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      229 2023-04-13 18:56:06.000000 dioptra-1.0.9/dioptra.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        8 2023-04-13 18:56:06.000000 dioptra-1.0.9/dioptra.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-04-13 18:56:06.115201 dioptra-1.0.9/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1656 2023-04-13 18:56:05.000000 dioptra-1.0.9/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 04:32:02.184200 dioptra-1.0.9rc1/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1471 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/LICENSE.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2162 2023-04-13 04:32:02.184200 dioptra-1.0.9rc1/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1106 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 04:32:02.180200 dioptra-1.0.9rc1/dioptra/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       25 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/dioptra/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 04:32:02.180200 dioptra-1.0.9rc1/dioptra/inference/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/dioptra/inference/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1637 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/dioptra/inference/inference_runner.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 04:32:02.180200 dioptra-1.0.9rc1/dioptra/inference/tf/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/dioptra/inference/tf/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5707 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/dioptra/inference/tf/tf_runner.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 04:32:02.180200 dioptra-1.0.9rc1/dioptra/inference/torch/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/dioptra/inference/torch/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6900 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/dioptra/inference/torch/torch_runner.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 04:32:02.184200 dioptra-1.0.9rc1/dioptra/lake/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/dioptra/lake/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8352 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/dioptra/lake/datasets.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 04:32:02.184200 dioptra-1.0.9rc1/dioptra/lake/torch/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/dioptra/lake/torch/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4545 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/dioptra/lake/torch/object_store_datasets.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    29031 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/dioptra/lake/utils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 04:32:02.184200 dioptra-1.0.9rc1/dioptra/miners/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      416 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/dioptra/miners/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3151 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/dioptra/miners/activation_miner.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4382 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/dioptra/miners/base_miner.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3533 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/dioptra/miners/coreset_miner.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2105 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/dioptra/miners/entropy_miner.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3511 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/dioptra/miners/knn_miner.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2090 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/dioptra/miners/random_miner.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2107 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/dioptra/miners/variance_miner.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-13 04:32:02.180200 dioptra-1.0.9rc1/dioptra.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2162 2023-04-13 04:32:02.000000 dioptra-1.0.9rc1/dioptra.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      808 2023-04-13 04:32:02.000000 dioptra-1.0.9rc1/dioptra.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-13 04:32:02.000000 dioptra-1.0.9rc1/dioptra.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      229 2023-04-13 04:32:02.000000 dioptra-1.0.9rc1/dioptra.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        8 2023-04-13 04:32:02.000000 dioptra-1.0.9rc1/dioptra.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-04-13 04:32:02.184200 dioptra-1.0.9rc1/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1656 2023-04-13 04:32:01.000000 dioptra-1.0.9rc1/setup.py
```

### Comparing `dioptra-1.0.9/LICENSE.md` & `dioptra-1.0.9rc1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.9/PKG-INFO` & `dioptra-1.0.9rc1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dioptra
-Version: 1.0.9
+Version: 1.0.9rc1
 Summary: Client library to log data to Dioptra API
 Home-page: https://github.com/dioptra-ai/collector-py
 Author: dioptra.ai
 Author-email: info@dioptra.ai
 License: BSD
 Project-URL: dioptra.ai, https://www.dioptra.ai
 Description: <div align="center">
```

### Comparing `dioptra-1.0.9/README.md` & `dioptra-1.0.9rc1/README.md`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.9/dioptra/inference/inference_runner.py` & `dioptra-1.0.9rc1/dioptra/inference/inference_runner.py`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.9/dioptra/inference/tf/tf_runner.py` & `dioptra-1.0.9rc1/dioptra/inference/tf/tf_runner.py`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.9/dioptra/inference/torch/torch_runner.py` & `dioptra-1.0.9rc1/dioptra/inference/torch/torch_runner.py`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.9/dioptra/lake/datasets.py` & `dioptra-1.0.9rc1/dioptra/lake/datasets.py`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.9/dioptra/lake/torch/object_store_datasets.py` & `dioptra-1.0.9rc1/dioptra/lake/torch/object_store_datasets.py`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.9/dioptra/lake/utils.py` & `dioptra-1.0.9rc1/dioptra/lake/utils.py`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.9/dioptra/miners/activation_miner.py` & `dioptra-1.0.9rc1/dioptra/miners/activation_miner.py`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.9/dioptra/miners/base_miner.py` & `dioptra-1.0.9rc1/dioptra/miners/base_miner.py`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.9/dioptra/miners/coreset_miner.py` & `dioptra-1.0.9rc1/dioptra/miners/coreset_miner.py`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.9/dioptra/miners/entropy_miner.py` & `dioptra-1.0.9rc1/dioptra/miners/entropy_miner.py`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.9/dioptra/miners/knn_miner.py` & `dioptra-1.0.9rc1/dioptra/miners/knn_miner.py`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.9/dioptra/miners/random_miner.py` & `dioptra-1.0.9rc1/dioptra/miners/random_miner.py`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.9/dioptra/miners/variance_miner.py` & `dioptra-1.0.9rc1/dioptra/miners/variance_miner.py`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.9/dioptra.egg-info/PKG-INFO` & `dioptra-1.0.9rc1/dioptra.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dioptra
-Version: 1.0.9
+Version: 1.0.9rc1
 Summary: Client library to log data to Dioptra API
 Home-page: https://github.com/dioptra-ai/collector-py
 Author: dioptra.ai
 Author-email: info@dioptra.ai
 License: BSD
 Project-URL: dioptra.ai, https://www.dioptra.ai
 Description: <div align="center">
```

### Comparing `dioptra-1.0.9/dioptra.egg-info/SOURCES.txt` & `dioptra-1.0.9rc1/dioptra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dioptra-1.0.9/setup.py` & `dioptra-1.0.9rc1/setup.py`

 * *Files identical despite different names*

