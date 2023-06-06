# Comparing `tmp/jsonQM-0.2.2.tar.gz` & `tmp/jsonQM-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/william/Documents/API Query language/dist/tmpzg71u05j/jsonQM-0.2.2.tar", last modified: Tue Jun  6 21:31:38 2023, max compression
+gzip compressed data, was "/home/william/Documents/API Query language/dist/tmp11wlu70y/jsonQM-0.2.3.tar", last modified: Tue Jun  6 21:44:13 2023, max compression
```

## Comparing `jsonQM-0.2.2.tar` & `jsonQM-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 william   (1000) william   (1000)        0 2023-06-06 21:31:38.000000 jsonQM-0.2.2/
-drwxrwxr-x   0 william   (1000) william   (1000)        0 2023-06-06 21:31:38.000000 jsonQM-0.2.2/jsonQM/
--rw-rw-r--   0 william   (1000) william   (1000)      620 2023-06-06 20:29:37.000000 jsonQM-0.2.2/jsonQM/model.py
--rw-rw-r--   0 william   (1000) william   (1000)     1245 2023-06-06 21:30:30.000000 jsonQM-0.2.2/jsonQM/modelserializer.py
--rw-rw-r--   0 william   (1000) william   (1000)       68 2023-06-06 21:21:25.000000 jsonQM-0.2.2/jsonQM/__init__.py
--rw-rw-r--   0 william   (1000) william   (1000)       38 2023-06-06 21:31:38.000000 jsonQM-0.2.2/setup.cfg
-drwxrwxr-x   0 william   (1000) william   (1000)        0 2023-06-06 21:31:38.000000 jsonQM-0.2.2/jsonQM.egg-info/
--rw-rw-r--   0 william   (1000) william   (1000)      207 2023-06-06 21:31:38.000000 jsonQM-0.2.2/jsonQM.egg-info/SOURCES.txt
--rw-rw-r--   0 william   (1000) william   (1000)        7 2023-06-06 21:31:38.000000 jsonQM-0.2.2/jsonQM.egg-info/top_level.txt
--rw-rw-r--   0 william   (1000) william   (1000)      574 2023-06-06 21:31:38.000000 jsonQM-0.2.2/jsonQM.egg-info/PKG-INFO
--rw-rw-r--   0 william   (1000) william   (1000)        1 2023-06-06 21:31:38.000000 jsonQM-0.2.2/jsonQM.egg-info/dependency_links.txt
--rw-rw-r--   0 william   (1000) william   (1000)     1957 2023-06-06 21:05:46.000000 jsonQM-0.2.2/README.md
--rw-rw-r--   0 william   (1000) william   (1000)      574 2023-06-06 21:31:38.000000 jsonQM-0.2.2/PKG-INFO
--rw-rw-r--   0 william   (1000) william   (1000)     1061 2023-06-06 08:49:52.000000 jsonQM-0.2.2/LICENSE
--rw-rw-r--   0 william   (1000) william   (1000)     1008 2023-06-06 21:30:20.000000 jsonQM-0.2.2/setup.py
+drwxrwxr-x   0 william   (1000) william   (1000)        0 2023-06-06 21:44:13.000000 jsonQM-0.2.3/
+drwxrwxr-x   0 william   (1000) william   (1000)        0 2023-06-06 21:44:13.000000 jsonQM-0.2.3/jsonQM/
+-rw-rw-r--   0 william   (1000) william   (1000)      620 2023-06-06 20:29:37.000000 jsonQM-0.2.3/jsonQM/model.py
+-rw-rw-r--   0 william   (1000) william   (1000)     1246 2023-06-06 21:42:47.000000 jsonQM-0.2.3/jsonQM/modelserializer.py
+-rw-rw-r--   0 william   (1000) william   (1000)       70 2023-06-06 21:42:40.000000 jsonQM-0.2.3/jsonQM/__init__.py
+-rw-rw-r--   0 william   (1000) william   (1000)       38 2023-06-06 21:44:13.000000 jsonQM-0.2.3/setup.cfg
+drwxrwxr-x   0 william   (1000) william   (1000)        0 2023-06-06 21:44:13.000000 jsonQM-0.2.3/jsonQM.egg-info/
+-rw-rw-r--   0 william   (1000) william   (1000)      207 2023-06-06 21:44:13.000000 jsonQM-0.2.3/jsonQM.egg-info/SOURCES.txt
+-rw-rw-r--   0 william   (1000) william   (1000)        7 2023-06-06 21:44:13.000000 jsonQM-0.2.3/jsonQM.egg-info/top_level.txt
+-rw-rw-r--   0 william   (1000) william   (1000)      574 2023-06-06 21:44:13.000000 jsonQM-0.2.3/jsonQM.egg-info/PKG-INFO
+-rw-rw-r--   0 william   (1000) william   (1000)        1 2023-06-06 21:44:13.000000 jsonQM-0.2.3/jsonQM.egg-info/dependency_links.txt
+-rw-rw-r--   0 william   (1000) william   (1000)     1957 2023-06-06 21:05:46.000000 jsonQM-0.2.3/README.md
+-rw-rw-r--   0 william   (1000) william   (1000)      574 2023-06-06 21:44:13.000000 jsonQM-0.2.3/PKG-INFO
+-rw-rw-r--   0 william   (1000) william   (1000)     1061 2023-06-06 08:49:52.000000 jsonQM-0.2.3/LICENSE
+-rw-rw-r--   0 william   (1000) william   (1000)     1008 2023-06-06 21:43:12.000000 jsonQM-0.2.3/setup.py
```

### Comparing `jsonQM-0.2.2/jsonQM/model.py` & `jsonQM-0.2.3/jsonQM/model.py`

 * *Files identical despite different names*

### Comparing `jsonQM-0.2.2/jsonQM/modelserializer.py` & `jsonQM-0.2.3/jsonQM/modelserializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Union
-from model import Model
+from .model import Model
 
 #this is the decorator that serializes the Model
 class ModelSerializer:
     def __init__(self) -> None:
         """
         Each Model requires a new `ModelSerializer`.
         """
```

### Comparing `jsonQM-0.2.2/jsonQM.egg-info/PKG-INFO` & `jsonQM-0.2.3/jsonQM.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonQM
-Version: 0.2.2
+Version: 0.2.3
 Summary: A simple tool to easily make your API endpoint json queries more versatile.
 Home-page: UNKNOWN
 Author: William A. Lim
 Author-email: william.lim@csu.fullerton.edu
 License: UNKNOWN
 Keywords: python,json,request,query,model
 Platform: UNKNOWN
```

### Comparing `jsonQM-0.2.2/README.md` & `jsonQM-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `jsonQM-0.2.2/PKG-INFO` & `jsonQM-0.2.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonQM
-Version: 0.2.2
+Version: 0.2.3
 Summary: A simple tool to easily make your API endpoint json queries more versatile.
 Home-page: UNKNOWN
 Author: William A. Lim
 Author-email: william.lim@csu.fullerton.edu
 License: UNKNOWN
 Keywords: python,json,request,query,model
 Platform: UNKNOWN
```

### Comparing `jsonQM-0.2.2/LICENSE` & `jsonQM-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonQM-0.2.2/setup.py` & `jsonQM-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2.2' 
+VERSION = '0.2.3' 
 DESCRIPTION = 'A simple tool to easily make your API endpoint json queries more versatile.'
 LONG_DESCRIPTION = 'This module allows you to make your API endpoints more versatile by binding response functions to different entries on your json request similar to GraphQL.'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="jsonQM",
```

