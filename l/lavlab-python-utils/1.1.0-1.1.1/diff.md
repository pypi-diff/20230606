# Comparing `tmp/lavlab-python-utils-1.1.0.tar.gz` & `tmp/lavlab-python-utils-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavlab-python-utils-1.1.0.tar", last modified: Tue Jun  6 11:46:16 2023, max compression
+gzip compressed data, was "lavlab-python-utils-1.1.1.tar", last modified: Tue Jun  6 11:56:20 2023, max compression
```

## Comparing `lavlab-python-utils-1.1.0.tar` & `lavlab-python-utils-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:46:16.204936 lavlab-python-utils-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-06 11:46:16.204936 lavlab-python-utils-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-06 11:46:04.000000 lavlab-python-utils-1.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-06 11:46:04.000000 lavlab-python-utils-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 11:46:16.204936 lavlab-python-utils-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:46:16.204936 lavlab-python-utils-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:46:16.204936 lavlab-python-utils-1.1.0/src/lavlab/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-06 11:46:04.000000 lavlab-python-utils-1.1.0/src/lavlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-06-06 11:46:04.000000 lavlab-python-utils-1.1.0/src/lavlab/omero_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)    27776 2023-06-06 11:46:04.000000 lavlab-python-utils-1.1.0/src/lavlab/omero_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-06-06 11:46:04.000000 lavlab-python-utils-1.1.0/src/lavlab/python_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:46:16.204936 lavlab-python-utils-1.1.0/src/lavlab_python_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-06 11:46:16.000000 lavlab-python-utils-1.1.0/src/lavlab_python_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-06 11:46:16.000000 lavlab-python-utils-1.1.0/src/lavlab_python_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 11:46:16.000000 lavlab-python-utils-1.1.0/src/lavlab_python_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-06 11:46:16.000000 lavlab-python-utils-1.1.0/src/lavlab_python_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-06 11:46:16.000000 lavlab-python-utils-1.1.0/src/lavlab_python_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:46:16.204936 lavlab-python-utils-1.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-06-06 11:46:04.000000 lavlab-python-utils-1.1.0/test/test_omero_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-06-06 11:46:04.000000 lavlab-python-utils-1.1.0/test/test_python_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:56:20.677699 lavlab-python-utils-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-06 11:56:20.677699 lavlab-python-utils-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-06 11:56:07.000000 lavlab-python-utils-1.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-06 11:56:07.000000 lavlab-python-utils-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 11:56:20.677699 lavlab-python-utils-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:56:20.673699 lavlab-python-utils-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:56:20.677699 lavlab-python-utils-1.1.1/src/lavlab/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-06 11:56:07.000000 lavlab-python-utils-1.1.1/src/lavlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-06-06 11:56:07.000000 lavlab-python-utils-1.1.1/src/lavlab/omero_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27768 2023-06-06 11:56:07.000000 lavlab-python-utils-1.1.1/src/lavlab/omero_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-06-06 11:56:07.000000 lavlab-python-utils-1.1.1/src/lavlab/python_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:56:20.677699 lavlab-python-utils-1.1.1/src/lavlab_python_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-06 11:56:20.000000 lavlab-python-utils-1.1.1/src/lavlab_python_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-06 11:56:20.000000 lavlab-python-utils-1.1.1/src/lavlab_python_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 11:56:20.000000 lavlab-python-utils-1.1.1/src/lavlab_python_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-06 11:56:20.000000 lavlab-python-utils-1.1.1/src/lavlab_python_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-06 11:56:20.000000 lavlab-python-utils-1.1.1/src/lavlab_python_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:56:20.677699 lavlab-python-utils-1.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-06-06 11:56:07.000000 lavlab-python-utils-1.1.1/test/test_omero_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-06-06 11:56:07.000000 lavlab-python-utils-1.1.1/test/test_python_utils.py
```

### Comparing `lavlab-python-utils-1.1.0/PKG-INFO` & `lavlab-python-utils-1.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavlab-python-utils
-Version: 1.1.0
+Version: 1.1.1
 Summary: LaViolette Lab utility package
 Author-email: Michael Barrett <mjbarrett@mcw.edu>
 Project-URL: Homepage, https://github.com/laviolette-lab/lavlab-python-utils
 Project-URL: Bug Tracker, https://github.com/laviolette-lab/lavlab-python-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lavlab-python-utils-1.1.0/pyproject.toml` & `lavlab-python-utils-1.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "lavlab-python-utils"
 description = "LaViolette Lab utility package"
-version = "1.1.0"
+version = "1.1.1"
 
 authors = [
   { name="Michael Barrett", email="mjbarrett@mcw.edu" },
 ]
 
 readme = "README.rst"
 classifiers = [
```

### Comparing `lavlab-python-utils-1.1.0/src/lavlab/omero_asyncio.py` & `lavlab-python-utils-1.1.1/src/lavlab/omero_asyncio.py`

 * *Files identical despite different names*

### Comparing `lavlab-python-utils-1.1.0/src/lavlab/omero_util.py` & `lavlab-python-utils-1.1.1/src/lavlab/omero_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
 
     # create parallel raw pixels stores
     jobs=[]
     for chunk in chunkify(tiles, PARALLEL_STORE_COUNT):
         jobs.append(work(img.getPrimaryPixels().getId(), chunk, resLvl))
     return merge_async_iters(*jobs)
 
-def getDownsampledXYDimensions(img: ImageWrapper, downsample_factor: int) -> tuple[float,float]:
+def getDownsampledXYDimensions(img: ImageWrapper, downsample_factor: int) -> tuple[int,int]:
     """
 Returns XY (rows,columns) dimensions of given image at the downsample.
 
 Parameters
 ----------
 img: omero.gateway.ImageWrapper
     Omero Image object from conn.getObjects().
@@ -169,15 +169,15 @@
 Returns
 -------
 float 
     img.getSizeX() / downsample_factor
 float
     img.getSizeY() / downsample_factor
 """
-    return (float(img.getSizeX() / downsample_factor), float(img.getSizeY() / downsample_factor))
+    return (int(img.getSizeX() / downsample_factor), int(img.getSizeY() / downsample_factor))
 
 def getDownsampleFromDimensions(base_shape:tuple[int,...], sample_shape:tuple[int,...]) -> tuple[float,...]:
     """
 Essentially an alias for np.divide().
 
 Finds the ratio between a base array shape and a sample array shape by dividing each axis.
```

### Comparing `lavlab-python-utils-1.1.0/src/lavlab/python_util.py` & `lavlab-python-utils-1.1.1/src/lavlab/python_util.py`

 * *Files identical despite different names*

### Comparing `lavlab-python-utils-1.1.0/src/lavlab_python_utils.egg-info/PKG-INFO` & `lavlab-python-utils-1.1.1/src/lavlab_python_utils.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavlab-python-utils
-Version: 1.1.0
+Version: 1.1.1
 Summary: LaViolette Lab utility package
 Author-email: Michael Barrett <mjbarrett@mcw.edu>
 Project-URL: Homepage, https://github.com/laviolette-lab/lavlab-python-utils
 Project-URL: Bug Tracker, https://github.com/laviolette-lab/lavlab-python-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lavlab-python-utils-1.1.0/test/test_omero_util.py` & `lavlab-python-utils-1.1.1/test/test_omero_util.py`

 * *Files identical despite different names*

### Comparing `lavlab-python-utils-1.1.0/test/test_python_utils.py` & `lavlab-python-utils-1.1.1/test/test_python_utils.py`

 * *Files identical despite different names*

