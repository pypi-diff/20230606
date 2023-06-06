# Comparing `tmp/jsonQM-0.2.0.tar.gz` & `tmp/jsonQM-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/william/Documents/API Query language/dist/tmprafij20j/jsonQM-0.2.0.tar", last modified: Tue Jun  6 21:13:23 2023, max compression
+gzip compressed data, was "/home/william/Documents/API Query language/dist/tmpfnocn39a/jsonQM-0.2.1.tar", last modified: Tue Jun  6 21:22:46 2023, max compression
```

## Comparing `jsonQM-0.2.0.tar` & `jsonQM-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 william   (1000) william   (1000)        0 2023-06-06 21:13:23.000000 jsonQM-0.2.0/
-drwxrwxr-x   0 william   (1000) william   (1000)        0 2023-06-06 21:13:23.000000 jsonQM-0.2.0/jsonQM/
--rw-rw-r--   0 william   (1000) william   (1000)      620 2023-06-06 20:29:37.000000 jsonQM-0.2.0/jsonQM/Model.py
--rw-rw-r--   0 william   (1000) william   (1000)     1245 2023-06-06 20:30:54.000000 jsonQM-0.2.0/jsonQM/ModelSerializer.py
--rw-rw-r--   0 william   (1000) william   (1000)       68 2023-06-06 20:45:53.000000 jsonQM-0.2.0/jsonQM/__init__.py
--rw-rw-r--   0 william   (1000) william   (1000)       38 2023-06-06 21:13:23.000000 jsonQM-0.2.0/setup.cfg
-drwxrwxr-x   0 william   (1000) william   (1000)        0 2023-06-06 21:13:23.000000 jsonQM-0.2.0/jsonQM.egg-info/
--rw-rw-r--   0 william   (1000) william   (1000)      207 2023-06-06 21:13:23.000000 jsonQM-0.2.0/jsonQM.egg-info/SOURCES.txt
--rw-rw-r--   0 william   (1000) william   (1000)        7 2023-06-06 21:13:22.000000 jsonQM-0.2.0/jsonQM.egg-info/top_level.txt
--rw-rw-r--   0 william   (1000) william   (1000)      574 2023-06-06 21:13:22.000000 jsonQM-0.2.0/jsonQM.egg-info/PKG-INFO
--rw-rw-r--   0 william   (1000) william   (1000)        1 2023-06-06 21:13:22.000000 jsonQM-0.2.0/jsonQM.egg-info/dependency_links.txt
--rw-rw-r--   0 william   (1000) william   (1000)     1957 2023-06-06 21:05:46.000000 jsonQM-0.2.0/README.md
--rw-rw-r--   0 william   (1000) william   (1000)      574 2023-06-06 21:13:23.000000 jsonQM-0.2.0/PKG-INFO
--rw-rw-r--   0 william   (1000) william   (1000)     1061 2023-06-06 08:49:52.000000 jsonQM-0.2.0/LICENSE
--rw-rw-r--   0 william   (1000) william   (1000)     1008 2023-06-06 21:12:30.000000 jsonQM-0.2.0/setup.py
+drwxrwxr-x   0 william   (1000) william   (1000)        0 2023-06-06 21:22:46.000000 jsonQM-0.2.1/
+drwxrwxr-x   0 william   (1000) william   (1000)        0 2023-06-06 21:22:46.000000 jsonQM-0.2.1/jsonQM/
+-rw-rw-r--   0 william   (1000) william   (1000)      620 2023-06-06 20:29:37.000000 jsonQM-0.2.1/jsonQM/model.py
+-rw-rw-r--   0 william   (1000) william   (1000)     1245 2023-06-06 20:30:54.000000 jsonQM-0.2.1/jsonQM/modelserializer.py
+-rw-rw-r--   0 william   (1000) william   (1000)       68 2023-06-06 21:21:25.000000 jsonQM-0.2.1/jsonQM/__init__.py
+-rw-rw-r--   0 william   (1000) william   (1000)       38 2023-06-06 21:22:46.000000 jsonQM-0.2.1/setup.cfg
+drwxrwxr-x   0 william   (1000) william   (1000)        0 2023-06-06 21:22:46.000000 jsonQM-0.2.1/jsonQM.egg-info/
+-rw-rw-r--   0 william   (1000) william   (1000)      207 2023-06-06 21:22:46.000000 jsonQM-0.2.1/jsonQM.egg-info/SOURCES.txt
+-rw-rw-r--   0 william   (1000) william   (1000)        7 2023-06-06 21:22:46.000000 jsonQM-0.2.1/jsonQM.egg-info/top_level.txt
+-rw-rw-r--   0 william   (1000) william   (1000)      574 2023-06-06 21:22:46.000000 jsonQM-0.2.1/jsonQM.egg-info/PKG-INFO
+-rw-rw-r--   0 william   (1000) william   (1000)        1 2023-06-06 21:22:46.000000 jsonQM-0.2.1/jsonQM.egg-info/dependency_links.txt
+-rw-rw-r--   0 william   (1000) william   (1000)     1957 2023-06-06 21:05:46.000000 jsonQM-0.2.1/README.md
+-rw-rw-r--   0 william   (1000) william   (1000)      574 2023-06-06 21:22:46.000000 jsonQM-0.2.1/PKG-INFO
+-rw-rw-r--   0 william   (1000) william   (1000)     1061 2023-06-06 08:49:52.000000 jsonQM-0.2.1/LICENSE
+-rw-rw-r--   0 william   (1000) william   (1000)     1008 2023-06-06 21:22:22.000000 jsonQM-0.2.1/setup.py
```

### Comparing `jsonQM-0.2.0/jsonQM/Model.py` & `jsonQM-0.2.1/jsonQM/model.py`

 * *Files identical despite different names*

### Comparing `jsonQM-0.2.0/jsonQM/ModelSerializer.py` & `jsonQM-0.2.1/jsonQM/modelserializer.py`

 * *Files identical despite different names*

### Comparing `jsonQM-0.2.0/jsonQM.egg-info/PKG-INFO` & `jsonQM-0.2.1/jsonQM.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonQM
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple tool to easily make your API endpoint json queries more versatile.
 Home-page: UNKNOWN
 Author: William A. Lim
 Author-email: william.lim@csu.fullerton.edu
 License: UNKNOWN
 Keywords: python,json,request,query,model
 Platform: UNKNOWN
```

### Comparing `jsonQM-0.2.0/README.md` & `jsonQM-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `jsonQM-0.2.0/PKG-INFO` & `jsonQM-0.2.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonQM
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple tool to easily make your API endpoint json queries more versatile.
 Home-page: UNKNOWN
 Author: William A. Lim
 Author-email: william.lim@csu.fullerton.edu
 License: UNKNOWN
 Keywords: python,json,request,query,model
 Platform: UNKNOWN
```

### Comparing `jsonQM-0.2.0/LICENSE` & `jsonQM-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonQM-0.2.0/setup.py` & `jsonQM-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.2.0' 
+VERSION = '0.2.1' 
 DESCRIPTION = 'A simple tool to easily make your API endpoint json queries more versatile.'
 LONG_DESCRIPTION = 'This module allows you to make your API endpoints more versatile by binding response functions to different entries on your json request similar to GraphQL.'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="jsonQM",
```

