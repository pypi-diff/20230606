# Comparing `tmp/audinterface-1.0.2.tar.gz` & `tmp/audinterface-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audinterface-1.0.2.tar", last modified: Mon May  8 12:54:47 2023, max compression
+gzip compressed data, was "audinterface-1.0.3.tar", last modified: Tue Jun  6 13:30:20 2023, max compression
```

## Comparing `audinterface-1.0.2.tar` & `audinterface-1.0.3.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:54:47.325755 audinterface-1.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:54:47.317754 audinterface-1.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:54:47.321755 audinterface-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-08 12:54:31.000000 audinterface-1.0.2/.github/workflows/flake8.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-08 12:54:31.000000 audinterface-1.0.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-05-08 12:54:31.000000 audinterface-1.0.2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-08 12:54:31.000000 audinterface-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-08 12:54:31.000000 audinterface-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     9453 2023-05-08 12:54:31.000000 audinterface-1.0.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-05-08 12:54:31.000000 audinterface-1.0.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-08 12:54:31.000000 audinterface-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15345 2023-05-08 12:54:47.325755 audinterface-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-08 12:54:31.000000 audinterface-1.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:54:47.321755 audinterface-1.0.2/audinterface/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-08 12:54:31.000000 audinterface-1.0.2/audinterface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:54:47.321755 audinterface-1.0.2/audinterface/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:54:31.000000 audinterface-1.0.2/audinterface/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32308 2023-05-08 12:54:31.000000 audinterface-1.0.2/audinterface/core/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)    30239 2023-05-08 12:54:31.000000 audinterface-1.0.2/audinterface/core/process.py
--rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-05-08 12:54:31.000000 audinterface-1.0.2/audinterface/core/process_with_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    19407 2023-05-08 12:54:31.000000 audinterface-1.0.2/audinterface/core/segment.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-08 12:54:31.000000 audinterface-1.0.2/audinterface/core/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)    14646 2023-05-08 12:54:31.000000 audinterface-1.0.2/audinterface/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:54:47.321755 audinterface-1.0.2/audinterface/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-08 12:54:31.000000 audinterface-1.0.2/audinterface/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:54:47.321755 audinterface-1.0.2/audinterface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15345 2023-05-08 12:54:46.000000 audinterface-1.0.2/audinterface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-08 12:54:47.000000 audinterface-1.0.2/audinterface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 12:54:46.000000 audinterface-1.0.2/audinterface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-08 12:54:46.000000 audinterface-1.0.2/audinterface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-08 12:54:46.000000 audinterface-1.0.2/audinterface.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:54:47.325755 audinterface-1.0.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:54:47.317754 audinterface-1.0.2/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:54:47.325755 audinterface-1.0.2/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-08 12:54:31.000000 audinterface-1.0.2/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-08 12:54:31.000000 audinterface-1.0.2/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-08 12:54:31.000000 audinterface-1.0.2/docs/_templates/autosummary/function.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:54:47.325755 audinterface-1.0.2/docs/api-src/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-08 12:54:31.000000 audinterface-1.0.2/docs/api-src/audinterface.rst
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-08 12:54:31.000000 audinterface-1.0.2/docs/api-src/audinterface.utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-08 12:54:31.000000 audinterface-1.0.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-08 12:54:31.000000 audinterface-1.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-08 12:54:31.000000 audinterface-1.0.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-08 12:54:31.000000 audinterface-1.0.2/docs/genindex.rst
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-08 12:54:31.000000 audinterface-1.0.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-08 12:54:31.000000 audinterface-1.0.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-08 12:54:31.000000 audinterface-1.0.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11457 2023-05-08 12:54:31.000000 audinterface-1.0.2/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:54:47.325755 audinterface-1.0.2/misc/
--rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-05-08 12:54:31.000000 audinterface-1.0.2/misc/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-08 12:54:31.000000 audinterface-1.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-08 12:54:47.325755 audinterface-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-08 12:54:31.000000 audinterface-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:54:47.325755 audinterface-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-08 12:54:31.000000 audinterface-1.0.2/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    29830 2023-05-08 12:54:31.000000 audinterface-1.0.2/tests/test_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)    39773 2023-05-08 12:54:31.000000 audinterface-1.0.2/tests/test_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-05-08 12:54:31.000000 audinterface-1.0.2/tests/test_process_with_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    12017 2023-05-08 12:54:31.000000 audinterface-1.0.2/tests/test_segment.py
--rw-r--r--   0 runner    (1001) docker     (123)    10481 2023-05-08 12:54:31.000000 audinterface-1.0.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:30:20.562342 audinterface-1.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:30:20.550342 audinterface-1.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:30:20.554342 audinterface-1.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-06 13:30:07.000000 audinterface-1.0.3/.github/workflows/flake8.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-06 13:30:07.000000 audinterface-1.0.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-06 13:30:07.000000 audinterface-1.0.3/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-06 13:30:07.000000 audinterface-1.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-06 13:30:07.000000 audinterface-1.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-06-06 13:30:07.000000 audinterface-1.0.3/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-06-06 13:30:07.000000 audinterface-1.0.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-06 13:30:07.000000 audinterface-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15537 2023-06-06 13:30:20.562342 audinterface-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-06 13:30:07.000000 audinterface-1.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:30:20.554342 audinterface-1.0.3/audinterface/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-06 13:30:07.000000 audinterface-1.0.3/audinterface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:30:20.558342 audinterface-1.0.3/audinterface/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 13:30:07.000000 audinterface-1.0.3/audinterface/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32308 2023-06-06 13:30:07.000000 audinterface-1.0.3/audinterface/core/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30238 2023-06-06 13:30:07.000000 audinterface-1.0.3/audinterface/core/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-06-06 13:30:07.000000 audinterface-1.0.3/audinterface/core/process_with_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20069 2023-06-06 13:30:07.000000 audinterface-1.0.3/audinterface/core/segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-06 13:30:07.000000 audinterface-1.0.3/audinterface/core/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14646 2023-06-06 13:30:07.000000 audinterface-1.0.3/audinterface/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:30:20.558342 audinterface-1.0.3/audinterface/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 13:30:07.000000 audinterface-1.0.3/audinterface/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:30:20.554342 audinterface-1.0.3/audinterface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15537 2023-06-06 13:30:20.000000 audinterface-1.0.3/audinterface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-06 13:30:20.000000 audinterface-1.0.3/audinterface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 13:30:20.000000 audinterface-1.0.3/audinterface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-06 13:30:20.000000 audinterface-1.0.3/audinterface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-06 13:30:20.000000 audinterface-1.0.3/audinterface.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:30:20.558342 audinterface-1.0.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:30:20.550342 audinterface-1.0.3/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:30:20.558342 audinterface-1.0.3/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-06 13:30:07.000000 audinterface-1.0.3/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-06 13:30:07.000000 audinterface-1.0.3/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-06 13:30:07.000000 audinterface-1.0.3/docs/_templates/autosummary/function.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:30:20.558342 audinterface-1.0.3/docs/api-src/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-06 13:30:07.000000 audinterface-1.0.3/docs/api-src/audinterface.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-06 13:30:07.000000 audinterface-1.0.3/docs/api-src/audinterface.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-06 13:30:07.000000 audinterface-1.0.3/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-06-06 13:30:07.000000 audinterface-1.0.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-06 13:30:07.000000 audinterface-1.0.3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-06 13:30:07.000000 audinterface-1.0.3/docs/genindex.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-06 13:30:07.000000 audinterface-1.0.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-06 13:30:07.000000 audinterface-1.0.3/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-06 13:30:07.000000 audinterface-1.0.3/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11457 2023-06-06 13:30:07.000000 audinterface-1.0.3/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:30:20.558342 audinterface-1.0.3/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-06-06 13:30:07.000000 audinterface-1.0.3/misc/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-06 13:30:07.000000 audinterface-1.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-06 13:30:20.562342 audinterface-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-06 13:30:07.000000 audinterface-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:30:20.562342 audinterface-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-06 13:30:07.000000 audinterface-1.0.3/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    29830 2023-06-06 13:30:07.000000 audinterface-1.0.3/tests/test_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39773 2023-06-06 13:30:07.000000 audinterface-1.0.3/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-06-06 13:30:07.000000 audinterface-1.0.3/tests/test_process_with_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12547 2023-06-06 13:30:07.000000 audinterface-1.0.3/tests/test_segment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10481 2023-06-06 13:30:07.000000 audinterface-1.0.3/tests/test_utils.py
```

### Comparing `audinterface-1.0.2/.github/workflows/publish.yml` & `audinterface-1.0.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.2/.github/workflows/test.yml` & `audinterface-1.0.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.2/CHANGELOG.rst` & `audinterface-1.0.3/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,21 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
 
+Version 1.0.3 (2023/06/06)
+--------------------------
+
+* Added: ``cache_root`` argument
+  to ``audinterface.Segment.process_index()``
+
+
 Version 1.0.2 (2023/05/08)
 --------------------------
 
 * Added: support for Python 3.11
 * Changed: require ``audformat>=1.0.1``
 * Fixed: ``*.process_index()``
   keeps precision of ``end`` values
```

### Comparing `audinterface-1.0.2/CONTRIBUTING.rst` & `audinterface-1.0.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.2/LICENSE` & `audinterface-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.2/PKG-INFO` & `audinterface-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: audinterface
-Version: 1.0.2
+Version: 1.0.3
 Summary: Generic interfaces for signal processing
 Home-page: https://github.com/audeering/audinterface/
 Author: Johannes Wagner, Hagen Wierstorf, Andreas Triantafyllopoulos
 Author-email: jwagner@audeering.com, hwierstorf@audeering.com, atriant@audeering.com
 License: MIT
 Project-URL: Documentation, https://audeering.github.io/audinterface/
 Description: ============
@@ -49,14 +49,21 @@
         
         All notable changes to this project will be documented in this file.
         
         The format is based on `Keep a Changelog`_,
         and this project adheres to `Semantic Versioning`_.
         
         
+        Version 1.0.3 (2023/06/06)
+        --------------------------
+        
+        * Added: ``cache_root`` argument
+          to ``audinterface.Segment.process_index()``
+        
+        
         Version 1.0.2 (2023/05/08)
         --------------------------
         
         * Added: support for Python 3.11
         * Changed: require ``audformat>=1.0.1``
         * Fixed: ``*.process_index()``
           keeps precision of ``end`` values
```

### Comparing `audinterface-1.0.2/README.rst` & `audinterface-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.2/audinterface/__init__.py` & `audinterface-1.0.3/audinterface/__init__.py`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.2/audinterface/core/feature.py` & `audinterface-1.0.3/audinterface/core/feature.py`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.2/audinterface/core/process.py` & `audinterface-1.0.3/audinterface/core/process.py`

 * *Files 0% similar despite different names*

```diff
@@ -505,15 +505,15 @@
 
         If ``cache_root`` is not ``None``,
         a hash value is created from the index
         using :func:`audformat.utils.hash` and
         the result is stored as
         ``<cache_root>/<hash>.pkl``.
         When called again with the same index,
-        features will be read from the cached file.
+        results will be read from the cached file.
 
         Args:
             index: index with segment information
             preserve_index: if ``True``
                 and :attr:`audinterface.Process.segment` is ``None``
                 the returned index
                 will be of same type
```

### Comparing `audinterface-1.0.2/audinterface/core/process_with_context.py` & `audinterface-1.0.3/audinterface/core/process_with_context.py`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.2/audinterface/core/segment.py` & `audinterface-1.0.3/audinterface/core/segment.py`

 * *Files 2% similar despite different names*

```diff
@@ -370,20 +370,30 @@
         return self.process_files(files)
 
     def process_index(
             self,
             index: pd.Index,
             *,
             root: str = None,
+            cache_root: str = None,
     ) -> pd.Index:
         r"""Segment files or segments from an index.
 
+        If ``cache_root`` is not ``None``,
+        a hash value is created from the index
+        using :func:`audformat.utils.hash` and
+        the result is stored as
+        ``<cache_root>/<hash>.pkl``.
+        When called again with the same index,
+        results will be read from the cached file.
+
         Args:
             index: index conform to audformat_
             root: root folder to expand relative file paths
+            cache_root: cache folder (see description)
 
         Returns:
             Segmented index conform to audformat_
 
         Raises:
             RuntimeError: if sampling rates do not match
             RuntimeError: if channel selection is invalid
@@ -393,21 +403,31 @@
         """
         index = audformat.utils.to_segmented_index(index)
         utils.assert_index(index)
 
         if index.empty:
             return index
 
-        return self.process_files(
-            index.get_level_values('file'),
-            starts=index.get_level_values('start'),
-            ends=index.get_level_values('end'),
+        y = self.process.process_index(
+            index,
+            preserve_index=False,
             root=root,
+            cache_root=cache_root,
         )
 
+        files = []
+        starts = []
+        ends = []
+        for (file, start, _), index in y.items():
+            files.extend([file] * len(index))
+            starts.extend(index.levels[0] + start)
+            ends.extend(index.levels[1] + start)
+
+        return audformat.segmented_index(files, starts, ends)
+
     def process_signal(
             self,
             signal: np.ndarray,
             sampling_rate: int,
             *,
             file: str = None,
             start: Timestamp = None,
```

### Comparing `audinterface-1.0.2/audinterface/core/utils.py` & `audinterface-1.0.3/audinterface/core/utils.py`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.2/audinterface.egg-info/PKG-INFO` & `audinterface-1.0.3/audinterface.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: audinterface
-Version: 1.0.2
+Version: 1.0.3
 Summary: Generic interfaces for signal processing
 Home-page: https://github.com/audeering/audinterface/
 Author: Johannes Wagner, Hagen Wierstorf, Andreas Triantafyllopoulos
 Author-email: jwagner@audeering.com, hwierstorf@audeering.com, atriant@audeering.com
 License: MIT
 Project-URL: Documentation, https://audeering.github.io/audinterface/
 Description: ============
@@ -49,14 +49,21 @@
         
         All notable changes to this project will be documented in this file.
         
         The format is based on `Keep a Changelog`_,
         and this project adheres to `Semantic Versioning`_.
         
         
+        Version 1.0.3 (2023/06/06)
+        --------------------------
+        
+        * Added: ``cache_root`` argument
+          to ``audinterface.Segment.process_index()``
+        
+        
         Version 1.0.2 (2023/05/08)
         --------------------------
         
         * Added: support for Python 3.11
         * Changed: require ``audformat>=1.0.1``
         * Fixed: ``*.process_index()``
           keeps precision of ``end`` values
```

### Comparing `audinterface-1.0.2/audinterface.egg-info/SOURCES.txt` & `audinterface-1.0.3/audinterface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.2/docs/_templates/autosummary/class.rst` & `audinterface-1.0.3/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.2/docs/api-src/audinterface.rst` & `audinterface-1.0.3/docs/api-src/audinterface.rst`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.2/docs/conf.py` & `audinterface-1.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.2/docs/index.rst` & `audinterface-1.0.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.2/docs/usage.rst` & `audinterface-1.0.3/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.2/misc/logo.png` & `audinterface-1.0.3/misc/logo.png`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.2/setup.cfg` & `audinterface-1.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.2/tests/test_feature.py` & `audinterface-1.0.3/tests/test_feature.py`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.2/tests/test_process.py` & `audinterface-1.0.3/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.2/tests/test_process_with_context.py` & `audinterface-1.0.3/tests/test_process_with_context.py`

 * *Files identical despite different names*

### Comparing `audinterface-1.0.2/tests/test_segment.py` & `audinterface-1.0.3/tests/test_segment.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,14 +211,33 @@
     index = pd.Index([file], name='file')
     expected = audformat.segmented_index(file, '0.1s', '2.9s')
     result = segment.process_index(index, root=root)
     pd.testing.assert_index_equal(result, expected)
     result = segment.process_signal_from_index(signal, sampling_rate, index)
     pd.testing.assert_index_equal(result, expected)
 
+    # empty index returned by process func
+
+    def process_func(x, sr):
+        return audinterface.utils.signal_index()
+
+    segment = audinterface.Segment(
+        process_func=process_func,
+        sampling_rate=None,
+        resample=False,
+        num_workers=num_workers,
+        multiprocessing=multiprocessing,
+        verbose=False,
+    )
+
+    index = pd.Index([path], name='file')
+    expected = audformat.segmented_index()
+    result = segment.process_index(index)
+    pd.testing.assert_index_equal(result, expected)
+
 
 @pytest.mark.parametrize(
     'signal, sampling_rate, segment_func, result',
     [
         (
             SIGNAL,
             SAMPLING_RATE,
```

### Comparing `audinterface-1.0.2/tests/test_utils.py` & `audinterface-1.0.3/tests/test_utils.py`

 * *Files identical despite different names*

