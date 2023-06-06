# Comparing `tmp/HomoglyphsCJK-0.1.3.tar.gz` & `tmp/HomoglyphsCJK-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HomoglyphsCJK-0.1.3.tar", last modified: Sat May 27 07:08:43 2023, max compression
+gzip compressed data, was "HomoglyphsCJK-0.1.4.tar", last modified: Tue Jun  6 05:44:35 2023, max compression
```

## Comparing `HomoglyphsCJK-0.1.3.tar` & `HomoglyphsCJK-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-27 07:08:43.211613 HomoglyphsCJK-0.1.3/
-drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-27 07:08:43.210469 HomoglyphsCJK-0.1.3/HomoglyphsCJK/
--rw-r--r--   0 yangxinmei   (501) staff       (20)      122 2023-05-27 06:49:16.000000 HomoglyphsCJK-0.1.3/HomoglyphsCJK/__init__.py
--rw-r--r--   0 yangxinmei   (501) staff       (20)    10932 2023-05-27 06:58:42.000000 HomoglyphsCJK-0.1.3/HomoglyphsCJK/hg_functions.py
--rw-r--r--   0 yangxinmei   (501) staff       (20)     2422 2023-05-13 13:49:58.000000 HomoglyphsCJK-0.1.3/HomoglyphsCJK/test_run.py
-drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-05-27 07:08:43.211313 HomoglyphsCJK-0.1.3/HomoglyphsCJK.egg-info/
--rw-r--r--   0 yangxinmei   (501) staff       (20)     4089 2023-05-27 07:08:43.000000 HomoglyphsCJK-0.1.3/HomoglyphsCJK.egg-info/PKG-INFO
--rw-r--r--   0 yangxinmei   (501) staff       (20)      284 2023-05-27 07:08:43.000000 HomoglyphsCJK-0.1.3/HomoglyphsCJK.egg-info/SOURCES.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)        1 2023-05-27 07:08:43.000000 HomoglyphsCJK-0.1.3/HomoglyphsCJK.egg-info/dependency_links.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)       44 2023-05-27 07:08:43.000000 HomoglyphsCJK-0.1.3/HomoglyphsCJK.egg-info/requires.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)       14 2023-05-27 07:08:43.000000 HomoglyphsCJK-0.1.3/HomoglyphsCJK.egg-info/top_level.txt
--rw-r--r--   0 yangxinmei   (501) staff       (20)     4089 2023-05-27 07:08:43.211480 HomoglyphsCJK-0.1.3/PKG-INFO
--rw-r--r--   0 yangxinmei   (501) staff       (20)     3545 2023-05-27 07:08:05.000000 HomoglyphsCJK-0.1.3/README.md
--rw-r--r--   0 yangxinmei   (501) staff       (20)       38 2023-05-27 07:08:43.211673 HomoglyphsCJK-0.1.3/setup.cfg
--rw-r--r--   0 yangxinmei   (501) staff       (20)      950 2023-05-27 07:08:29.000000 HomoglyphsCJK-0.1.3/setup.py
+drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-06-06 05:44:35.984540 HomoglyphsCJK-0.1.4/
+drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-06-06 05:44:35.982028 HomoglyphsCJK-0.1.4/HomoglyphsCJK/
+-rw-r--r--   0 yangxinmei   (501) staff       (20)      122 2023-05-27 07:13:42.000000 HomoglyphsCJK-0.1.4/HomoglyphsCJK/__init__.py
+-rw-r--r--   0 yangxinmei   (501) staff       (20)    10932 2023-05-27 06:58:42.000000 HomoglyphsCJK-0.1.4/HomoglyphsCJK/hg_functions.py
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     2422 2023-05-13 13:49:58.000000 HomoglyphsCJK-0.1.4/HomoglyphsCJK/test_run.py
+drwxr-xr-x   0 yangxinmei   (501) staff       (20)        0 2023-06-06 05:44:35.983818 HomoglyphsCJK-0.1.4/HomoglyphsCJK.egg-info/
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     4089 2023-06-06 05:44:35.000000 HomoglyphsCJK-0.1.4/HomoglyphsCJK.egg-info/PKG-INFO
+-rw-r--r--   0 yangxinmei   (501) staff       (20)      284 2023-06-06 05:44:35.000000 HomoglyphsCJK-0.1.4/HomoglyphsCJK.egg-info/SOURCES.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)        1 2023-06-06 05:44:35.000000 HomoglyphsCJK-0.1.4/HomoglyphsCJK.egg-info/dependency_links.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)       44 2023-06-06 05:44:35.000000 HomoglyphsCJK-0.1.4/HomoglyphsCJK.egg-info/requires.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)       14 2023-06-06 05:44:35.000000 HomoglyphsCJK-0.1.4/HomoglyphsCJK.egg-info/top_level.txt
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     4089 2023-06-06 05:44:35.984227 HomoglyphsCJK-0.1.4/PKG-INFO
+-rw-r--r--   0 yangxinmei   (501) staff       (20)     3545 2023-05-27 07:08:05.000000 HomoglyphsCJK-0.1.4/README.md
+-rw-r--r--   0 yangxinmei   (501) staff       (20)       38 2023-06-06 05:44:35.984635 HomoglyphsCJK-0.1.4/setup.cfg
+-rw-r--r--   0 yangxinmei   (501) staff       (20)      967 2023-06-06 05:43:27.000000 HomoglyphsCJK-0.1.4/setup.py
```

### Comparing `HomoglyphsCJK-0.1.3/HomoglyphsCJK/hg_functions.py` & `HomoglyphsCJK-0.1.4/HomoglyphsCJK/hg_functions.py`

 * *Files identical despite different names*

### Comparing `HomoglyphsCJK-0.1.3/HomoglyphsCJK/test_run.py` & `HomoglyphsCJK-0.1.4/HomoglyphsCJK/test_run.py`

 * *Files identical despite different names*

### Comparing `HomoglyphsCJK-0.1.3/HomoglyphsCJK.egg-info/PKG-INFO` & `HomoglyphsCJK-0.1.4/HomoglyphsCJK.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HomoglyphsCJK
-Version: 0.1.3
+Version: 0.1.4
 Summary: An easy Python package for fuzzy matching Chinese(simplified and traditional), Japanese and Korean, using character similarity trained from ViT transformer
 Home-page: https://github.com/dell-research-harvard/HomoglyphsCJK.git
 Author: HomoglyphsCJK Team
 Author-email: homoglyphscjk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `HomoglyphsCJK-0.1.3/PKG-INFO` & `HomoglyphsCJK-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HomoglyphsCJK
-Version: 0.1.3
+Version: 0.1.4
 Summary: An easy Python package for fuzzy matching Chinese(simplified and traditional), Japanese and Korean, using character similarity trained from ViT transformer
 Home-page: https://github.com/dell-research-harvard/HomoglyphsCJK.git
 Author: HomoglyphsCJK Team
 Author-email: homoglyphscjk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `HomoglyphsCJK-0.1.3/README.md` & `HomoglyphsCJK-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `HomoglyphsCJK-0.1.3/setup.py` & `HomoglyphsCJK-0.1.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 from setuptools import find_packages, setup
 
-with open("README.md","r") as fh:
+with open("README.md","r",encoding='utf-8') as fh:
     long_des = fh.read()
 
 setup(
     name="HomoglyphsCJK",
     packages=["HomoglyphsCJK"],
-    version="0.1.3",
+    version="0.1.4",
     author="HomoglyphsCJK Team",
     author_email="homoglyphscjk@gmail.com",
     description="An easy Python package for fuzzy matching Chinese(simplified and traditional), Japanese and Korean, using character similarity trained from ViT transformer",
     long_description=long_des,
     long_description_content_type="text/markdown",
     url="https://github.com/dell-research-harvard/HomoglyphsCJK.git",
     classifiers=[
```

