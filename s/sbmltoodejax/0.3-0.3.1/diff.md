# Comparing `tmp/sbmltoodejax-0.3.tar.gz` & `tmp/sbmltoodejax-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbmltoodejax-0.3.tar", last modified: Tue Jun  6 15:07:25 2023, max compression
+gzip compressed data, was "sbmltoodejax-0.3.1.tar", last modified: Tue Jun  6 15:16:28 2023, max compression
```

## Comparing `sbmltoodejax-0.3.tar` & `sbmltoodejax-0.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 mayalen   (1001) mayalen   (1001)        0 2023-06-06 15:07:25.018816 sbmltoodejax-0.3/
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     2760 2023-06-06 15:00:48.000000 sbmltoodejax-0.3/LICENSE
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     5037 2023-06-06 15:07:25.014816 sbmltoodejax-0.3/PKG-INFO
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     4504 2023-06-06 15:00:48.000000 sbmltoodejax-0.3/README.md
-drwxrwxr-x   0 mayalen   (1001) mayalen   (1001)        0 2023-06-06 15:07:25.014816 sbmltoodejax-0.3/sbmltoodejax/
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)      344 2023-06-06 15:00:48.000000 sbmltoodejax-0.3/sbmltoodejax/__init__.py
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     6062 2023-06-06 15:00:48.000000 sbmltoodejax-0.3/sbmltoodejax/biomodels_api.py
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     2552 2023-06-06 15:00:48.000000 sbmltoodejax-0.3/sbmltoodejax/jaxfuncs.py
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)    25792 2023-06-06 15:00:48.000000 sbmltoodejax-0.3/sbmltoodejax/modulegeneration.py
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     2689 2023-06-06 15:00:48.000000 sbmltoodejax-0.3/sbmltoodejax/parse.py
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     3054 2023-06-06 15:00:48.000000 sbmltoodejax-0.3/sbmltoodejax/utils.py
-drwxrwxr-x   0 mayalen   (1001) mayalen   (1001)        0 2023-06-06 15:07:25.014816 sbmltoodejax-0.3/sbmltoodejax.egg-info/
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     5037 2023-06-06 15:07:24.000000 sbmltoodejax-0.3/sbmltoodejax.egg-info/PKG-INFO
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)      414 2023-06-06 15:07:24.000000 sbmltoodejax-0.3/sbmltoodejax.egg-info/SOURCES.txt
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)        1 2023-06-06 15:07:24.000000 sbmltoodejax-0.3/sbmltoodejax.egg-info/dependency_links.txt
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)       29 2023-06-06 15:07:24.000000 sbmltoodejax-0.3/sbmltoodejax.egg-info/requires.txt
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)       13 2023-06-06 15:07:24.000000 sbmltoodejax-0.3/sbmltoodejax.egg-info/top_level.txt
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)       38 2023-06-06 15:07:25.018816 sbmltoodejax-0.3/setup.cfg
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)      821 2023-06-06 15:07:18.000000 sbmltoodejax-0.3/setup.py
-drwxrwxr-x   0 mayalen   (1001) mayalen   (1001)        0 2023-06-06 15:07:25.014816 sbmltoodejax-0.3/test/
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     1641 2023-06-06 15:00:48.000000 sbmltoodejax-0.3/test/test_jaxfuncs.py
--rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     2461 2023-06-06 15:00:48.000000 sbmltoodejax-0.3/test/test_modulegeneration.py
+drwxrwxr-x   0 mayalen   (1001) mayalen   (1001)        0 2023-06-06 15:16:28.756468 sbmltoodejax-0.3.1/
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     2760 2023-06-06 15:00:48.000000 sbmltoodejax-0.3.1/LICENSE
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     5039 2023-06-06 15:16:28.756468 sbmltoodejax-0.3.1/PKG-INFO
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     4504 2023-06-06 15:00:48.000000 sbmltoodejax-0.3.1/README.md
+drwxrwxr-x   0 mayalen   (1001) mayalen   (1001)        0 2023-06-06 15:16:28.756468 sbmltoodejax-0.3.1/sbmltoodejax/
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)      346 2023-06-06 15:16:19.000000 sbmltoodejax-0.3.1/sbmltoodejax/__init__.py
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     6062 2023-06-06 15:00:48.000000 sbmltoodejax-0.3.1/sbmltoodejax/biomodels_api.py
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     2552 2023-06-06 15:00:48.000000 sbmltoodejax-0.3.1/sbmltoodejax/jaxfuncs.py
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)    25792 2023-06-06 15:00:48.000000 sbmltoodejax-0.3.1/sbmltoodejax/modulegeneration.py
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     2689 2023-06-06 15:00:48.000000 sbmltoodejax-0.3.1/sbmltoodejax/parse.py
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     3054 2023-06-06 15:00:48.000000 sbmltoodejax-0.3.1/sbmltoodejax/utils.py
+drwxrwxr-x   0 mayalen   (1001) mayalen   (1001)        0 2023-06-06 15:16:28.756468 sbmltoodejax-0.3.1/sbmltoodejax.egg-info/
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     5039 2023-06-06 15:16:28.000000 sbmltoodejax-0.3.1/sbmltoodejax.egg-info/PKG-INFO
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)      414 2023-06-06 15:16:28.000000 sbmltoodejax-0.3.1/sbmltoodejax.egg-info/SOURCES.txt
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)        1 2023-06-06 15:16:28.000000 sbmltoodejax-0.3.1/sbmltoodejax.egg-info/dependency_links.txt
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)       29 2023-06-06 15:16:28.000000 sbmltoodejax-0.3.1/sbmltoodejax.egg-info/requires.txt
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)       13 2023-06-06 15:16:28.000000 sbmltoodejax-0.3.1/sbmltoodejax.egg-info/top_level.txt
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)       38 2023-06-06 15:16:28.756468 sbmltoodejax-0.3.1/setup.cfg
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)      850 2023-06-06 15:14:35.000000 sbmltoodejax-0.3.1/setup.py
+drwxrwxr-x   0 mayalen   (1001) mayalen   (1001)        0 2023-06-06 15:16:28.756468 sbmltoodejax-0.3.1/test/
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     1641 2023-06-06 15:00:48.000000 sbmltoodejax-0.3.1/test/test_jaxfuncs.py
+-rw-rw-r--   0 mayalen   (1001) mayalen   (1001)     2461 2023-06-06 15:00:48.000000 sbmltoodejax-0.3.1/test/test_modulegeneration.py
```

### Comparing `sbmltoodejax-0.3/LICENSE` & `sbmltoodejax-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sbmltoodejax-0.3/PKG-INFO` & `sbmltoodejax-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbmltoodejax
-Version: 0.3
+Version: 0.3.1
 Summary: lightweight library that allows to automatically parse and convert SBML models into python models written end-to-end in JAX
 Home-page: https://github.com/flowersteam/sbmltoodejax
 Author: Mayalen Etcheverry
 Author-email: mayalen.etcheverry@inria.fr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sbmltoodejax-0.3/README.md` & `sbmltoodejax-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `sbmltoodejax-0.3/sbmltoodejax/biomodels_api.py` & `sbmltoodejax-0.3.1/sbmltoodejax/biomodels_api.py`

 * *Files identical despite different names*

### Comparing `sbmltoodejax-0.3/sbmltoodejax/jaxfuncs.py` & `sbmltoodejax-0.3.1/sbmltoodejax/jaxfuncs.py`

 * *Files identical despite different names*

### Comparing `sbmltoodejax-0.3/sbmltoodejax/modulegeneration.py` & `sbmltoodejax-0.3.1/sbmltoodejax/modulegeneration.py`

 * *Files identical despite different names*

### Comparing `sbmltoodejax-0.3/sbmltoodejax/parse.py` & `sbmltoodejax-0.3.1/sbmltoodejax/parse.py`

 * *Files identical despite different names*

### Comparing `sbmltoodejax-0.3/sbmltoodejax/utils.py` & `sbmltoodejax-0.3.1/sbmltoodejax/utils.py`

 * *Files identical despite different names*

### Comparing `sbmltoodejax-0.3/sbmltoodejax.egg-info/PKG-INFO` & `sbmltoodejax-0.3.1/sbmltoodejax.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbmltoodejax
-Version: 0.3
+Version: 0.3.1
 Summary: lightweight library that allows to automatically parse and convert SBML models into python models written end-to-end in JAX
 Home-page: https://github.com/flowersteam/sbmltoodejax
 Author: Mayalen Etcheverry
 Author-email: mayalen.etcheverry@inria.fr
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sbmltoodejax-0.3/test/test_jaxfuncs.py` & `sbmltoodejax-0.3.1/test/test_jaxfuncs.py`

 * *Files identical despite different names*

### Comparing `sbmltoodejax-0.3/test/test_modulegeneration.py` & `sbmltoodejax-0.3.1/test/test_modulegeneration.py`

 * *Files identical despite different names*

