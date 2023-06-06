# Comparing `tmp/large-image-source-multi-1.22.2.dev4.tar.gz` & `tmp/large-image-source-multi-1.22.3.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-multi-1.22.2.dev4.tar", last modified: Mon Jun  5 19:13:28 2023, max compression
+gzip compressed data, was "large-image-source-multi-1.22.3.dev2.tar", last modified: Tue Jun  6 16:57:53 2023, max compression
```

## Comparing `large-image-source-multi-1.22.2.dev4.tar` & `large-image-source-multi-1.22.3.dev2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-05 19:13:28.268612 large-image-source-multi-1.22.2.dev4/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-06-05 19:13:28.000000 large-image-source-multi-1.22.2.dev4/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      966 2023-06-05 19:13:28.268612 large-image-source-multi-1.22.2.dev4/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-06-05 19:13:28.000000 large-image-source-multi-1.22.2.dev4/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-05 19:13:28.264612 large-image-source-multi-1.22.2.dev4/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3381 2023-06-05 19:12:22.000000 large-image-source-multi-1.22.2.dev4/docs/specification.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-05 19:13:28.264612 large-image-source-multi-1.22.2.dev4/large_image_source_multi/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    45193 2023-06-05 19:12:22.000000 large-image-source-multi-1.22.2.dev4/large_image_source_multi/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1356 2023-06-05 19:12:22.000000 large-image-source-multi-1.22.2.dev4/large_image_source_multi/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-05 19:13:28.264612 large-image-source-multi-1.22.2.dev4/large_image_source_multi.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      966 2023-06-05 19:13:28.000000 large-image-source-multi-1.22.2.dev4/large_image_source_multi.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      419 2023-06-05 19:13:28.000000 large-image-source-multi-1.22.2.dev4/large_image_source_multi.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-05 19:13:28.000000 large-image-source-multi-1.22.2.dev4/large_image_source_multi.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2023-06-05 19:13:28.000000 large-image-source-multi-1.22.2.dev4/large_image_source_multi.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      139 2023-06-05 19:13:28.000000 large-image-source-multi-1.22.2.dev4/large_image_source_multi.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-06-05 19:13:28.000000 large-image-source-multi-1.22.2.dev4/large_image_source_multi.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-06-05 19:13:28.268612 large-image-source-multi-1.22.2.dev4/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2637 2023-06-05 19:12:22.000000 large-image-source-multi-1.22.2.dev4/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-06 16:57:53.944736 large-image-source-multi-1.22.3.dev2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-06-06 16:57:53.000000 large-image-source-multi-1.22.3.dev2/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      966 2023-06-06 16:57:53.944736 large-image-source-multi-1.22.3.dev2/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-06-06 16:57:53.000000 large-image-source-multi-1.22.3.dev2/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-06 16:57:53.940736 large-image-source-multi-1.22.3.dev2/docs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3381 2023-06-06 16:56:44.000000 large-image-source-multi-1.22.3.dev2/docs/specification.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-06 16:57:53.940736 large-image-source-multi-1.22.3.dev2/large_image_source_multi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    45193 2023-06-06 16:56:44.000000 large-image-source-multi-1.22.3.dev2/large_image_source_multi/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1356 2023-06-06 16:56:44.000000 large-image-source-multi-1.22.3.dev2/large_image_source_multi/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-06 16:57:53.940736 large-image-source-multi-1.22.3.dev2/large_image_source_multi.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      966 2023-06-06 16:57:53.000000 large-image-source-multi-1.22.3.dev2/large_image_source_multi.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      419 2023-06-06 16:57:53.000000 large-image-source-multi-1.22.3.dev2/large_image_source_multi.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-06 16:57:53.000000 large-image-source-multi-1.22.3.dev2/large_image_source_multi.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2023-06-06 16:57:53.000000 large-image-source-multi-1.22.3.dev2/large_image_source_multi.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      139 2023-06-06 16:57:53.000000 large-image-source-multi-1.22.3.dev2/large_image_source_multi.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-06-06 16:57:53.000000 large-image-source-multi-1.22.3.dev2/large_image_source_multi.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-06-06 16:57:53.944736 large-image-source-multi-1.22.3.dev2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2637 2023-06-06 16:56:44.000000 large-image-source-multi-1.22.3.dev2/setup.py
```

### Comparing `large-image-source-multi-1.22.2.dev4/LICENSE` & `large-image-source-multi-1.22.3.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-multi-1.22.2.dev4/PKG-INFO` & `large-image-source-multi-1.22.3.dev2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-multi
-Version: 1.22.2.dev4
+Version: 1.22.3.dev2
 Summary: A tilesource for large_image to composite other tile sources
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-multi-1.22.2.dev4/README.rst` & `large-image-source-multi-1.22.3.dev2/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-multi-1.22.2.dev4/docs/specification.rst` & `large-image-source-multi-1.22.3.dev2/docs/specification.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-multi-1.22.2.dev4/large_image_source_multi/__init__.py` & `large-image-source-multi-1.22.3.dev2/large_image_source_multi/__init__.py`

 * *Files identical despite different names*

### Comparing `large-image-source-multi-1.22.2.dev4/large_image_source_multi/girder_source.py` & `large-image-source-multi-1.22.3.dev2/large_image_source_multi/girder_source.py`

 * *Files identical despite different names*

### Comparing `large-image-source-multi-1.22.2.dev4/large_image_source_multi.egg-info/PKG-INFO` & `large-image-source-multi-1.22.3.dev2/large_image_source_multi.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-multi
-Version: 1.22.2.dev4
+Version: 1.22.3.dev2
 Summary: A tilesource for large_image to composite other tile sources
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-multi-1.22.2.dev4/setup.py` & `large-image-source-multi-1.22.3.dev2/setup.py`

 * *Files identical despite different names*

