# Comparing `tmp/faKy-1.3.3.tar.gz` & `tmp/faKy-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faKy-1.3.3.tar", last modified: Tue Jun  6 13:06:36 2023, max compression
+gzip compressed data, was "faKy-1.4.0.tar", last modified: Tue Jun  6 13:22:33 2023, max compression
```

## Comparing `faKy-1.3.3.tar` & `faKy-1.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 13:06:36.891889 faKy-1.3.3/
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     4508 2023-06-06 13:06:36.891616 faKy-1.3.3/PKG-INFO
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     4295 2023-06-06 12:37:50.000000 faKy-1.3.3/README.md
-drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 13:06:36.882690 faKy-1.3.3/faKy/
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        1 2023-06-06 08:19:35.000000 faKy-1.3.3/faKy/__init__.py
-drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 13:06:36.889134 faKy-1.3.3/faKy/en_core_web_md-2.3.1/
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)       17 2023-06-06 11:41:49.000000 faKy-1.3.3/faKy/en_core_web_md-2.3.1/MANIFEST.in
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      362 2023-06-06 11:41:49.000000 faKy-1.3.3/faKy/en_core_web_md-2.3.1/PKG-INFO
-drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 13:06:36.890494 faKy-1.3.3/faKy/en_core_web_md-2.3.1/en_core_web_md/
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      291 2023-06-06 11:41:49.000000 faKy-1.3.3/faKy/en_core_web_md-2.3.1/en_core_web_md/__init__.py
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     9468 2023-06-06 11:41:50.000000 faKy-1.3.3/faKy/en_core_web_md-2.3.1/en_core_web_md/meta.json
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     9468 2023-06-06 11:41:50.000000 faKy-1.3.3/faKy/en_core_web_md-2.3.1/meta.json
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)       38 2023-06-06 11:41:50.000000 faKy-1.3.3/faKy/en_core_web_md-2.3.1/setup.cfg
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     1753 2023-06-06 11:41:50.000000 faKy-1.3.3/faKy/en_core_web_md-2.3.1/setup.py
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     8053 2023-06-06 11:30:30.000000 faKy-1.3.3/faKy/faKy.py
-drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 13:06:36.885646 faKy-1.3.3/faKy.egg-info/
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     4508 2023-06-06 13:06:36.000000 faKy-1.3.3/faKy.egg-info/PKG-INFO
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      471 2023-06-06 13:06:36.000000 faKy-1.3.3/faKy.egg-info/SOURCES.txt
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        1 2023-06-06 13:06:36.000000 faKy-1.3.3/faKy.egg-info/dependency_links.txt
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      122 2023-06-06 13:06:36.000000 faKy-1.3.3/faKy.egg-info/requires.txt
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        5 2023-06-06 13:06:36.000000 faKy-1.3.3/faKy.egg-info/top_level.txt
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)       38 2023-06-06 13:06:36.892007 faKy-1.3.3/setup.cfg
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      813 2023-06-06 13:06:32.000000 faKy-1.3.3/setup.py
+drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 13:22:33.438114 faKy-1.4.0/
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     4508 2023-06-06 13:22:33.437829 faKy-1.4.0/PKG-INFO
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     4295 2023-06-06 12:37:50.000000 faKy-1.4.0/README.md
+drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 13:22:33.427464 faKy-1.4.0/faKy/
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        1 2023-06-06 08:19:35.000000 faKy-1.4.0/faKy/__init__.py
+drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 13:22:33.435375 faKy-1.4.0/faKy/en_core_web_md-2.3.1/
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)       17 2023-06-06 11:41:49.000000 faKy-1.4.0/faKy/en_core_web_md-2.3.1/MANIFEST.in
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      362 2023-06-06 11:41:49.000000 faKy-1.4.0/faKy/en_core_web_md-2.3.1/PKG-INFO
+drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 13:22:33.436802 faKy-1.4.0/faKy/en_core_web_md-2.3.1/en_core_web_md/
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      291 2023-06-06 11:41:49.000000 faKy-1.4.0/faKy/en_core_web_md-2.3.1/en_core_web_md/__init__.py
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     9468 2023-06-06 11:41:50.000000 faKy-1.4.0/faKy/en_core_web_md-2.3.1/en_core_web_md/meta.json
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     9468 2023-06-06 11:41:50.000000 faKy-1.4.0/faKy/en_core_web_md-2.3.1/meta.json
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)       38 2023-06-06 11:41:50.000000 faKy-1.4.0/faKy/en_core_web_md-2.3.1/setup.cfg
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     1753 2023-06-06 11:41:50.000000 faKy-1.4.0/faKy/en_core_web_md-2.3.1/setup.py
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     8177 2023-06-06 13:21:51.000000 faKy-1.4.0/faKy/faKy.py
+drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 13:22:33.429649 faKy-1.4.0/faKy.egg-info/
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     4508 2023-06-06 13:22:33.000000 faKy-1.4.0/faKy.egg-info/PKG-INFO
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      471 2023-06-06 13:22:33.000000 faKy-1.4.0/faKy.egg-info/SOURCES.txt
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        1 2023-06-06 13:22:33.000000 faKy-1.4.0/faKy.egg-info/dependency_links.txt
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      122 2023-06-06 13:22:33.000000 faKy-1.4.0/faKy.egg-info/requires.txt
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        5 2023-06-06 13:22:33.000000 faKy-1.4.0/faKy.egg-info/top_level.txt
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)       38 2023-06-06 13:22:33.438224 faKy-1.4.0/setup.cfg
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      813 2023-06-06 13:22:13.000000 faKy-1.4.0/setup.py
```

### Comparing `faKy-1.3.3/PKG-INFO` & `faKy-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faKy
-Version: 1.3.3
+Version: 1.4.0
 Summary: Your library description
 Author: Sandro Barres Hamers
 Author-email: sbarreshamers@gmail.com
 Description-Content-Type: text/markdown
 Provides-Extra: vader
 
 # faKy
```

### Comparing `faKy-1.3.3/README.md` & `faKy-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `faKy-1.3.3/faKy/en_core_web_md-2.3.1/en_core_web_md/meta.json` & `faKy-1.4.0/faKy/en_core_web_md-2.3.1/en_core_web_md/meta.json`

 * *Files identical despite different names*

### Comparing `faKy-1.3.3/faKy/en_core_web_md-2.3.1/meta.json` & `faKy-1.4.0/faKy/en_core_web_md-2.3.1/meta.json`

 * *Files identical despite different names*

### Comparing `faKy-1.3.3/faKy/en_core_web_md-2.3.1/setup.py` & `faKy-1.4.0/faKy/en_core_web_md-2.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `faKy-1.3.3/faKy/faKy.py` & `faKy-1.4.0/faKy/faKy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import pandas as pd 
 import numpy as np
 import sys
 import gzip
 import spacy
+import os
 from spacy.tokens import Doc
 from spacy_readability import Readability
 import nltk
 from vaderSentiment.vaderSentiment import SentimentIntensityAnalyzer
 
 
 
 nltk.download('vader_lexicon')
-nlp = spacy.load('en_core_web_md')
+current_dir = os.path.dirname(os.path.abspath(__file__))
+model_path = os.path.join(current_dir, 'en_core_web_md-2.3.1')
+nlp = spacy.load(model_path)
 
 
 '''
  The function readability_computation computes the Flesch-Kincaid Reading Ease score for a spaCy document using the Readability class. 
  It returns the original document object. 
  It is added to the spaCy pipeline using nlp.add_pipe with last=True.
 '''
```

### Comparing `faKy-1.3.3/faKy.egg-info/PKG-INFO` & `faKy-1.4.0/faKy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faKy
-Version: 1.3.3
+Version: 1.4.0
 Summary: Your library description
 Author: Sandro Barres Hamers
 Author-email: sbarreshamers@gmail.com
 Description-Content-Type: text/markdown
 Provides-Extra: vader
 
 # faKy
```

### Comparing `faKy-1.3.3/setup.py` & `faKy-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('readme.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='faKy',
-    version='1.3.3',
+    version='1.4.0',
     description='Your library description',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Sandro Barres Hamers',
     author_email='sbarreshamers@gmail.com',
     packages=['faKy'],
     install_requires=[
```

