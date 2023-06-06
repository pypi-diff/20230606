# Comparing `tmp/utilsbox-0.0.8.tar.gz` & `tmp/utilsbox-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utilsbox-0.0.8.tar", last modified: Sat Aug  6 06:01:58 2022, max compression
+gzip compressed data, was "utilsbox-0.0.9.tar", last modified: Sat Aug  6 06:08:13 2022, max compression
```

## Comparing `utilsbox-0.0.8.tar` & `utilsbox-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 vikas     (1000) vikas     (1000)        0 2022-08-06 06:01:57.994204 utilsbox-0.0.8/
--rw-rw-r--   0 vikas     (1000) vikas     (1000)      665 2022-08-06 06:01:57.994204 utilsbox-0.0.8/PKG-INFO
--rw-rw-r--   0 vikas     (1000) vikas     (1000)       89 2022-07-24 18:14:04.000000 utilsbox-0.0.8/README.md
--rw-rw-r--   0 vikas     (1000) vikas     (1000)       38 2022-08-06 06:01:57.994204 utilsbox-0.0.8/setup.cfg
--rw-rw-r--   0 vikas     (1000) vikas     (1000)      944 2022-08-06 06:01:47.000000 utilsbox-0.0.8/setup.py
-drwxrwxr-x   0 vikas     (1000) vikas     (1000)        0 2022-08-06 06:01:57.994204 utilsbox-0.0.8/utilsbox/
--rw-rw-r--   0 vikas     (1000) vikas     (1000)        0 2022-07-24 18:08:51.000000 utilsbox-0.0.8/utilsbox/__init__.py
--rw-rw-r--   0 vikas     (1000) vikas     (1000)     8916 2022-08-06 06:00:17.000000 utilsbox-0.0.8/utilsbox/utils.py
-drwxrwxr-x   0 vikas     (1000) vikas     (1000)        0 2022-08-06 06:01:57.994204 utilsbox-0.0.8/utilsbox.egg-info/
--rw-rw-r--   0 vikas     (1000) vikas     (1000)      665 2022-08-06 06:01:57.000000 utilsbox-0.0.8/utilsbox.egg-info/PKG-INFO
--rw-rw-r--   0 vikas     (1000) vikas     (1000)      216 2022-08-06 06:01:57.000000 utilsbox-0.0.8/utilsbox.egg-info/SOURCES.txt
--rw-rw-r--   0 vikas     (1000) vikas     (1000)        1 2022-08-06 06:01:57.000000 utilsbox-0.0.8/utilsbox.egg-info/dependency_links.txt
--rw-rw-r--   0 vikas     (1000) vikas     (1000)        6 2022-08-06 06:01:57.000000 utilsbox-0.0.8/utilsbox.egg-info/requires.txt
--rw-rw-r--   0 vikas     (1000) vikas     (1000)        9 2022-08-06 06:01:57.000000 utilsbox-0.0.8/utilsbox.egg-info/top_level.txt
+drwxrwxr-x   0 vikas     (1000) vikas     (1000)        0 2022-08-06 06:08:13.136235 utilsbox-0.0.9/
+-rw-rw-r--   0 vikas     (1000) vikas     (1000)      665 2022-08-06 06:08:13.136235 utilsbox-0.0.9/PKG-INFO
+-rw-rw-r--   0 vikas     (1000) vikas     (1000)       89 2022-07-24 18:14:04.000000 utilsbox-0.0.9/README.md
+-rw-rw-r--   0 vikas     (1000) vikas     (1000)       38 2022-08-06 06:08:13.136235 utilsbox-0.0.9/setup.cfg
+-rw-rw-r--   0 vikas     (1000) vikas     (1000)      969 2022-08-06 06:07:42.000000 utilsbox-0.0.9/setup.py
+drwxrwxr-x   0 vikas     (1000) vikas     (1000)        0 2022-08-06 06:08:13.136235 utilsbox-0.0.9/utilsbox/
+-rw-rw-r--   0 vikas     (1000) vikas     (1000)        0 2022-07-24 18:08:51.000000 utilsbox-0.0.9/utilsbox/__init__.py
+-rw-rw-r--   0 vikas     (1000) vikas     (1000)     8926 2022-08-06 06:07:05.000000 utilsbox-0.0.9/utilsbox/utils.py
+drwxrwxr-x   0 vikas     (1000) vikas     (1000)        0 2022-08-06 06:08:13.136235 utilsbox-0.0.9/utilsbox.egg-info/
+-rw-rw-r--   0 vikas     (1000) vikas     (1000)      665 2022-08-06 06:08:13.000000 utilsbox-0.0.9/utilsbox.egg-info/PKG-INFO
+-rw-rw-r--   0 vikas     (1000) vikas     (1000)      216 2022-08-06 06:08:13.000000 utilsbox-0.0.9/utilsbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 vikas     (1000) vikas     (1000)        1 2022-08-06 06:08:13.000000 utilsbox-0.0.9/utilsbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 vikas     (1000) vikas     (1000)       28 2022-08-06 06:08:13.000000 utilsbox-0.0.9/utilsbox.egg-info/requires.txt
+-rw-rw-r--   0 vikas     (1000) vikas     (1000)        9 2022-08-06 06:08:13.000000 utilsbox-0.0.9/utilsbox.egg-info/top_level.txt
```

### Comparing `utilsbox-0.0.8/PKG-INFO` & `utilsbox-0.0.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilsbox
-Version: 0.0.8
+Version: 0.0.9
 Summary: Contains useful functions and classes
 Home-page: UNKNOWN
 Author: Vikas Sanwal
 Author-email: <vikassnwl@gmail.com>
 License: UNKNOWN
 Description: 
         This package contains module named utils.py which contains useful functions and classes.
```

### Comparing `utilsbox-0.0.8/setup.py` & `utilsbox-0.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'Contains useful functions and classes'
 
 # Setting up
 setup(
     name="utilsbox",
     version=VERSION,
     author="Vikas Sanwal",
     author_email="<vikassnwl@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=['scipy'],
+    install_requires=['scipy', 'opencv-contrib-python'],
     keywords=['python'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

### Comparing `utilsbox-0.0.8/utilsbox/utils.py` & `utilsbox-0.0.9/utilsbox/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from scipy.spatial import distance
 import re
 import cv2
 import numpy as np
+import os
 
 
 
 def greet(name):
     """This function prints the string saying Hello to the name passed as argument.
 
     Args:
```

### Comparing `utilsbox-0.0.8/utilsbox.egg-info/PKG-INFO` & `utilsbox-0.0.9/utilsbox.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilsbox
-Version: 0.0.8
+Version: 0.0.9
 Summary: Contains useful functions and classes
 Home-page: UNKNOWN
 Author: Vikas Sanwal
 Author-email: <vikassnwl@gmail.com>
 License: UNKNOWN
 Description: 
         This package contains module named utils.py which contains useful functions and classes.
```

