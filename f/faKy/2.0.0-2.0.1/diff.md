# Comparing `tmp/faKy-2.0.0.tar.gz` & `tmp/faKy-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faKy-2.0.0.tar", last modified: Tue Jun  6 14:06:52 2023, max compression
+gzip compressed data, was "faKy-2.0.1.tar", last modified: Tue Jun  6 14:11:05 2023, max compression
```

## Comparing `faKy-2.0.0.tar` & `faKy-2.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 14:06:52.332484 faKy-2.0.0/
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     4486 2023-06-06 14:06:52.332142 faKy-2.0.0/PKG-INFO
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     4273 2023-06-06 13:52:24.000000 faKy-2.0.0/README.md
-drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 14:06:52.324863 faKy-2.0.0/faKy/
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        1 2023-06-06 08:19:35.000000 faKy-2.0.0/faKy/__init__.py
-drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 14:06:52.329909 faKy-2.0.0/faKy/en_core_web_md-2.3.1/
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)       17 2023-06-06 11:41:49.000000 faKy-2.0.0/faKy/en_core_web_md-2.3.1/MANIFEST.in
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      362 2023-06-06 11:41:49.000000 faKy-2.0.0/faKy/en_core_web_md-2.3.1/PKG-INFO
-drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 14:06:52.330993 faKy-2.0.0/faKy/en_core_web_md-2.3.1/en_core_web_md/
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      291 2023-06-06 11:41:49.000000 faKy-2.0.0/faKy/en_core_web_md-2.3.1/en_core_web_md/__init__.py
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     9468 2023-06-06 11:41:50.000000 faKy-2.0.0/faKy/en_core_web_md-2.3.1/en_core_web_md/meta.json
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     9468 2023-06-06 11:41:50.000000 faKy-2.0.0/faKy/en_core_web_md-2.3.1/meta.json
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)       38 2023-06-06 11:41:50.000000 faKy-2.0.0/faKy/en_core_web_md-2.3.1/setup.cfg
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     1753 2023-06-06 11:41:50.000000 faKy-2.0.0/faKy/en_core_web_md-2.3.1/setup.py
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     8256 2023-06-06 14:05:57.000000 faKy-2.0.0/faKy/faKy.py
-drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 14:06:52.326760 faKy-2.0.0/faKy.egg-info/
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     4486 2023-06-06 14:06:52.000000 faKy-2.0.0/faKy.egg-info/PKG-INFO
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      471 2023-06-06 14:06:52.000000 faKy-2.0.0/faKy.egg-info/SOURCES.txt
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        1 2023-06-06 14:06:52.000000 faKy-2.0.0/faKy.egg-info/dependency_links.txt
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      122 2023-06-06 14:06:52.000000 faKy-2.0.0/faKy.egg-info/requires.txt
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        5 2023-06-06 14:06:52.000000 faKy-2.0.0/faKy.egg-info/top_level.txt
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)       38 2023-06-06 14:06:52.332648 faKy-2.0.0/setup.cfg
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      759 2023-06-06 14:06:13.000000 faKy-2.0.0/setup.py
+drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 14:11:05.711001 faKy-2.0.1/
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     4486 2023-06-06 14:11:05.710632 faKy-2.0.1/PKG-INFO
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     4273 2023-06-06 13:52:24.000000 faKy-2.0.1/README.md
+drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 14:11:05.701789 faKy-2.0.1/faKy/
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        1 2023-06-06 08:19:35.000000 faKy-2.0.1/faKy/__init__.py
+drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 14:11:05.707563 faKy-2.0.1/faKy/en_core_web_md-2.3.1/
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)       17 2023-06-06 11:41:49.000000 faKy-2.0.1/faKy/en_core_web_md-2.3.1/MANIFEST.in
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      362 2023-06-06 11:41:49.000000 faKy-2.0.1/faKy/en_core_web_md-2.3.1/PKG-INFO
+drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 14:11:05.709637 faKy-2.0.1/faKy/en_core_web_md-2.3.1/en_core_web_md/
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      291 2023-06-06 11:41:49.000000 faKy-2.0.1/faKy/en_core_web_md-2.3.1/en_core_web_md/__init__.py
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     9468 2023-06-06 11:41:50.000000 faKy-2.0.1/faKy/en_core_web_md-2.3.1/en_core_web_md/meta.json
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     9468 2023-06-06 11:41:50.000000 faKy-2.0.1/faKy/en_core_web_md-2.3.1/meta.json
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)       38 2023-06-06 11:41:50.000000 faKy-2.0.1/faKy/en_core_web_md-2.3.1/setup.cfg
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     1753 2023-06-06 11:41:50.000000 faKy-2.0.1/faKy/en_core_web_md-2.3.1/setup.py
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     8158 2023-06-06 14:10:42.000000 faKy-2.0.1/faKy/faKy.py
+drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 14:11:05.703735 faKy-2.0.1/faKy.egg-info/
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     4486 2023-06-06 14:11:05.000000 faKy-2.0.1/faKy.egg-info/PKG-INFO
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      471 2023-06-06 14:11:05.000000 faKy-2.0.1/faKy.egg-info/SOURCES.txt
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        1 2023-06-06 14:11:05.000000 faKy-2.0.1/faKy.egg-info/dependency_links.txt
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      122 2023-06-06 14:11:05.000000 faKy-2.0.1/faKy.egg-info/requires.txt
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        5 2023-06-06 14:11:05.000000 faKy-2.0.1/faKy.egg-info/top_level.txt
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)       38 2023-06-06 14:11:05.711122 faKy-2.0.1/setup.cfg
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      759 2023-06-06 14:11:00.000000 faKy-2.0.1/setup.py
```

### Comparing `faKy-2.0.0/PKG-INFO` & `faKy-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faKy
-Version: 2.0.0
+Version: 2.0.1
 Summary: Your library description
 Author: Sandro Barres Hamers
 Author-email: sbarreshamers@gmail.com
 Description-Content-Type: text/markdown
 Provides-Extra: vader
 
 # faKy
```

### Comparing `faKy-2.0.0/README.md` & `faKy-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `faKy-2.0.0/faKy/en_core_web_md-2.3.1/en_core_web_md/meta.json` & `faKy-2.0.1/faKy/en_core_web_md-2.3.1/en_core_web_md/meta.json`

 * *Files identical despite different names*

### Comparing `faKy-2.0.0/faKy/en_core_web_md-2.3.1/meta.json` & `faKy-2.0.1/faKy/en_core_web_md-2.3.1/meta.json`

 * *Files identical despite different names*

### Comparing `faKy-2.0.0/faKy/en_core_web_md-2.3.1/setup.py` & `faKy-2.0.1/faKy/en_core_web_md-2.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `faKy-2.0.0/faKy/faKy.py` & `faKy-2.0.1/faKy/faKy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,18 @@
-import spacy.util
+import spacy
 
-# Load the 'en_core_web_md' model
 try:
     nlp = spacy.load('en_core_web_md')
 except OSError:
-    # Download the model if it's not found
-    spacy.util.download('en_core_web_md')
-    nlp = spacy.load('en_core_web_md')
+    print("Model not found. Please make sure 'en_core_web_md' is installed.")
 
 import pandas as pd 
 import numpy as np
 import sys
 import gzip
-import spacy
 from spacy.tokens import Doc
 from spacy_readability import Readability
 import nltk
 from vaderSentiment.vaderSentiment import SentimentIntensityAnalyzer
```

### Comparing `faKy-2.0.0/faKy.egg-info/PKG-INFO` & `faKy-2.0.1/faKy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faKy
-Version: 2.0.0
+Version: 2.0.1
 Summary: Your library description
 Author: Sandro Barres Hamers
 Author-email: sbarreshamers@gmail.com
 Description-Content-Type: text/markdown
 Provides-Extra: vader
 
 # faKy
```

### Comparing `faKy-2.0.0/setup.py` & `faKy-2.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('readme.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='faKy',
-    version='2.0.0',
+    version='2.0.1',
     description='Your library description',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Sandro Barres Hamers',
     author_email='sbarreshamers@gmail.com',
     packages=['faKy'],
     install_requires=[
```

