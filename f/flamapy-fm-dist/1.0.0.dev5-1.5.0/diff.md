# Comparing `tmp/flamapy-fm-dist-1.0.0.dev5.tar.gz` & `tmp/flamapy-fm-dist-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flamapy-fm-dist-1.0.0.dev5.tar", last modified: Mon Jun  5 23:11:56 2023, max compression
+gzip compressed data, was "flamapy-fm-dist-1.5.0.tar", last modified: Tue Jun  6 09:28:09 2023, max compression
```

## Comparing `flamapy-fm-dist-1.0.0.dev5.tar` & `flamapy-fm-dist-1.5.0.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:11:56.566666 flamapy-fm-dist-1.0.0.dev5/
--rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-06-05 23:11:41.000000 flamapy-fm-dist-1.0.0.dev5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-06-05 23:11:56.566666 flamapy-fm-dist-1.0.0.dev5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-06-05 23:11:41.000000 flamapy-fm-dist-1.0.0.dev5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:11:56.562666 flamapy-fm-dist-1.0.0.dev5/flamapy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:11:56.562666 flamapy-fm-dist-1.0.0.dev5/flamapy/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 23:11:41.000000 flamapy-fm-dist-1.0.0.dev5/flamapy/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:11:56.562666 flamapy-fm-dist-1.0.0.dev5/flamapy/interfaces/command_line/
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-05 23:11:41.000000 flamapy-fm-dist-1.0.0.dev5/flamapy/interfaces/command_line/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:11:56.566666 flamapy-fm-dist-1.0.0.dev5/flamapy/interfaces/python/
--rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-06-05 23:11:41.000000 flamapy-fm-dist-1.0.0.dev5/flamapy/interfaces/python/FLAMAFeatureModel.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 23:11:41.000000 flamapy-fm-dist-1.0.0.dev5/flamapy/interfaces/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:11:56.566666 flamapy-fm-dist-1.0.0.dev5/flamapy_fm_dist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-06-05 23:11:56.000000 flamapy-fm-dist-1.0.0.dev5/flamapy_fm_dist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-05 23:11:56.000000 flamapy-fm-dist-1.0.0.dev5/flamapy_fm_dist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 23:11:56.000000 flamapy-fm-dist-1.0.0.dev5/flamapy_fm_dist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-05 23:11:56.000000 flamapy-fm-dist-1.0.0.dev5/flamapy_fm_dist.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-05 23:11:56.000000 flamapy-fm-dist-1.0.0.dev5/flamapy_fm_dist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 23:11:56.000000 flamapy-fm-dist-1.0.0.dev5/flamapy_fm_dist.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 23:11:56.566666 flamapy-fm-dist-1.0.0.dev5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-05 23:11:41.000000 flamapy-fm-dist-1.0.0.dev5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:28:09.882236 flamapy-fm-dist-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-06-06 09:27:54.000000 flamapy-fm-dist-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11596 2023-06-06 09:28:09.878236 flamapy-fm-dist-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10891 2023-06-06 09:27:54.000000 flamapy-fm-dist-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:28:09.878236 flamapy-fm-dist-1.5.0/flamapy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:28:09.878236 flamapy-fm-dist-1.5.0/flamapy/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 09:27:54.000000 flamapy-fm-dist-1.5.0/flamapy/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:28:09.878236 flamapy-fm-dist-1.5.0/flamapy/interfaces/command_line/
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-06 09:27:54.000000 flamapy-fm-dist-1.5.0/flamapy/interfaces/command_line/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:28:09.878236 flamapy-fm-dist-1.5.0/flamapy/interfaces/python/
+-rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-06-06 09:27:54.000000 flamapy-fm-dist-1.5.0/flamapy/interfaces/python/FLAMAFeatureModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 09:27:54.000000 flamapy-fm-dist-1.5.0/flamapy/interfaces/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:28:09.878236 flamapy-fm-dist-1.5.0/flamapy/interfaces/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)    10886 2023-06-06 09:27:54.000000 flamapy-fm-dist-1.5.0/flamapy/interfaces/rest/operations_routes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:28:09.878236 flamapy-fm-dist-1.5.0/flamapy_fm_dist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11596 2023-06-06 09:28:09.000000 flamapy-fm-dist-1.5.0/flamapy_fm_dist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-06 09:28:09.000000 flamapy-fm-dist-1.5.0/flamapy_fm_dist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 09:28:09.000000 flamapy-fm-dist-1.5.0/flamapy_fm_dist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-06 09:28:09.000000 flamapy-fm-dist-1.5.0/flamapy_fm_dist.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-06 09:28:09.000000 flamapy-fm-dist-1.5.0/flamapy_fm_dist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 09:28:09.000000 flamapy-fm-dist-1.5.0/flamapy_fm_dist.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 09:28:09.882236 flamapy-fm-dist-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-06 09:27:54.000000 flamapy-fm-dist-1.5.0/setup.py
```

### Comparing `flamapy-fm-dist-1.0.0.dev5/LICENSE` & `flamapy-fm-dist-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flamapy-fm-dist-1.0.0.dev5/flamapy/interfaces/command_line/__init__.py` & `flamapy-fm-dist-1.5.0/flamapy/interfaces/command_line/__init__.py`

 * *Files identical despite different names*

### Comparing `flamapy-fm-dist-1.0.0.dev5/flamapy/interfaces/python/FLAMAFeatureModel.py` & `flamapy-fm-dist-1.5.0/flamapy/interfaces/python/FLAMAFeatureModel.py`

 * *Files identical despite different names*

### Comparing `flamapy-fm-dist-1.0.0.dev5/setup.py` & `flamapy-fm-dist-1.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="flamapy-fm-dist",
-    version="1.0.0.dev5",
+    version="1.5.0",
     author="Flamapy",
     author_email="flamapy@us.es",
     description="Flamapy feature model is a distribution of the flama framework containing all plugins required to analyze feature models. It also offers a richier API and a complete command line interface and documentation.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/flamapy/flamapy-feature-model",
     packages=setuptools.find_namespace_packages(include=['flamapy.*']),
```

