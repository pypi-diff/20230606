# Comparing `tmp/smriprep-docker-0.9.1.tar.gz` & `tmp/smriprep-docker-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/smriprep-docker-0.9.1.tar", last modified: Thu Jul 14 19:49:15 2022, max compression
+gzip compressed data, was "dist/smriprep-docker-0.9.2.tar", last modified: Thu Jul 21 02:08:28 2022, max compression
```

## Comparing `smriprep-docker-0.9.1.tar` & `smriprep-docker-0.9.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-07-14 19:49:15.266975 smriprep-docker-0.9.1/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1841 2022-07-14 19:49:15.266975 smriprep-docker-0.9.1/PKG-INFO
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)      900 2022-07-14 19:49:02.000000 smriprep-docker-0.9.1/README.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      941 2022-07-14 19:49:15.266975 smriprep-docker-0.9.1/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)      538 2022-07-14 19:49:02.000000 smriprep-docker-0.9.1/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-07-14 19:49:15.266975 smriprep-docker-0.9.1/smriprep_docker.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1841 2022-07-14 19:49:15.000000 smriprep-docker-0.9.1/smriprep_docker.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2022-07-14 19:49:15.000000 smriprep-docker-0.9.1/smriprep_docker.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-07-14 19:49:15.000000 smriprep-docker-0.9.1/smriprep_docker.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       58 2022-07-14 19:49:15.000000 smriprep-docker-0.9.1/smriprep_docker.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       16 2022-07-14 19:49:15.000000 smriprep-docker-0.9.1/smriprep_docker.egg-info/top_level.txt
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)    14717 2022-07-14 19:49:14.000000 smriprep-docker-0.9.1/smriprep_docker.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-07-21 02:08:28.764479 smriprep-docker-0.9.2/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1841 2022-07-21 02:08:28.764479 smriprep-docker-0.9.2/PKG-INFO
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)      900 2022-07-21 02:08:16.000000 smriprep-docker-0.9.2/README.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      941 2022-07-21 02:08:28.764479 smriprep-docker-0.9.2/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      538 2022-07-21 02:08:16.000000 smriprep-docker-0.9.2/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-07-21 02:08:28.764479 smriprep-docker-0.9.2/smriprep_docker.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1841 2022-07-21 02:08:28.000000 smriprep-docker-0.9.2/smriprep_docker.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      246 2022-07-21 02:08:28.000000 smriprep-docker-0.9.2/smriprep_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-07-21 02:08:28.000000 smriprep-docker-0.9.2/smriprep_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       58 2022-07-21 02:08:28.000000 smriprep-docker-0.9.2/smriprep_docker.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       16 2022-07-21 02:08:28.000000 smriprep-docker-0.9.2/smriprep_docker.egg-info/top_level.txt
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)    14717 2022-07-21 02:08:28.000000 smriprep-docker-0.9.2/smriprep_docker.py
```

### Comparing `smriprep-docker-0.9.1/PKG-INFO` & `smriprep-docker-0.9.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smriprep-docker
-Version: 0.9.1
+Version: 0.9.2
 Summary: A wrapper for generating Docker commands using regular sMRIPrep syntax
 Home-page: https://github.com/nipreps/smriprep
 Author: The NiPreps developers
 Author-email: nipreps@gmail.com
 Maintainer: Christopher J. Markiewicz
 Maintainer-email: nipreps@gmail.com
 License: 3-clause BSD
```

### Comparing `smriprep-docker-0.9.1/README.rst` & `smriprep-docker-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `smriprep-docker-0.9.1/setup.cfg` & `smriprep-docker-0.9.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `smriprep-docker-0.9.1/setup.py` & `smriprep-docker-0.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `smriprep-docker-0.9.1/smriprep_docker.egg-info/PKG-INFO` & `smriprep-docker-0.9.2/smriprep_docker.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smriprep-docker
-Version: 0.9.1
+Version: 0.9.2
 Summary: A wrapper for generating Docker commands using regular sMRIPrep syntax
 Home-page: https://github.com/nipreps/smriprep
 Author: The NiPreps developers
 Author-email: nipreps@gmail.com
 Maintainer: Christopher J. Markiewicz
 Maintainer-email: nipreps@gmail.com
 License: 3-clause BSD
```

### Comparing `smriprep-docker-0.9.1/smriprep_docker.py` & `smriprep-docker-0.9.2/smriprep_docker.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 """
 import sys
 import os
 import re
 import subprocess
 from warnings import warn
 
-__version__ = "0.9.1"
+__version__ = "0.9.2"
 __copyright__ = (
     "Copyright 2019, Center for Reproducible Neuroscience, Stanford University"
 )
 __credits__ = [
     "Oscar Esteban",
     "Chris Gorgolewski",
     "Christopher J. Markiewicz",
```

