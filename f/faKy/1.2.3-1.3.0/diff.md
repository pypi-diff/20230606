# Comparing `tmp/faKy-1.2.3.tar.gz` & `tmp/faKy-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faKy-1.2.3.tar", last modified: Tue Jun  6 11:20:46 2023, max compression
+gzip compressed data, was "faKy-1.3.0.tar", last modified: Tue Jun  6 11:43:28 2023, max compression
```

## Comparing `faKy-1.2.3.tar` & `faKy-1.3.0.tar`

### file list

```diff
@@ -1,14 +1,20 @@
-drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 11:20:46.194816 faKy-1.2.3/
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      719 2023-06-06 11:20:46.194532 faKy-1.2.3/PKG-INFO
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      488 2023-06-06 09:01:46.000000 faKy-1.2.3/README.md
-drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 11:20:46.191902 faKy-1.2.3/faKy/
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        1 2023-06-06 08:19:35.000000 faKy-1.2.3/faKy/__init__.py
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     8053 2023-06-06 08:14:25.000000 faKy-1.2.3/faKy/faKy.py
-drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 11:20:46.194073 faKy-1.2.3/faKy.egg-info/
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      719 2023-06-06 11:20:46.000000 faKy-1.2.3/faKy.egg-info/PKG-INFO
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      187 2023-06-06 11:20:46.000000 faKy-1.2.3/faKy.egg-info/SOURCES.txt
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        1 2023-06-06 11:20:46.000000 faKy-1.2.3/faKy.egg-info/dependency_links.txt
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      143 2023-06-06 11:20:46.000000 faKy-1.2.3/faKy.egg-info/requires.txt
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        5 2023-06-06 11:20:46.000000 faKy-1.2.3/faKy.egg-info/top_level.txt
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)       38 2023-06-06 11:20:46.194932 faKy-1.2.3/setup.cfg
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      691 2023-06-06 11:20:41.000000 faKy-1.2.3/setup.py
+drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 11:43:28.403264 faKy-1.3.0/
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      700 2023-06-06 11:43:28.402961 faKy-1.3.0/PKG-INFO
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      488 2023-06-06 09:01:46.000000 faKy-1.3.0/README.md
+drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 11:43:28.396565 faKy-1.3.0/faKy/
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        1 2023-06-06 08:19:35.000000 faKy-1.3.0/faKy/__init__.py
+drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 11:43:28.402140 faKy-1.3.0/faKy/en_core_web_md-2.3.1/
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)       17 2023-06-06 11:41:49.000000 faKy-1.3.0/faKy/en_core_web_md-2.3.1/MANIFEST.in
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      362 2023-06-06 11:41:49.000000 faKy-1.3.0/faKy/en_core_web_md-2.3.1/PKG-INFO
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     9468 2023-06-06 11:41:50.000000 faKy-1.3.0/faKy/en_core_web_md-2.3.1/meta.json
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)       38 2023-06-06 11:41:50.000000 faKy-1.3.0/faKy/en_core_web_md-2.3.1/setup.cfg
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     1753 2023-06-06 11:41:50.000000 faKy-1.3.0/faKy/en_core_web_md-2.3.1/setup.py
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     8053 2023-06-06 11:30:30.000000 faKy-1.3.0/faKy/faKy.py
+drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 11:43:28.398877 faKy-1.3.0/faKy.egg-info/
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      700 2023-06-06 11:43:28.000000 faKy-1.3.0/faKy.egg-info/PKG-INFO
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      367 2023-06-06 11:43:28.000000 faKy-1.3.0/faKy.egg-info/SOURCES.txt
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        1 2023-06-06 11:43:28.000000 faKy-1.3.0/faKy.egg-info/dependency_links.txt
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      122 2023-06-06 11:43:28.000000 faKy-1.3.0/faKy.egg-info/requires.txt
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        5 2023-06-06 11:43:28.000000 faKy-1.3.0/faKy.egg-info/top_level.txt
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)       38 2023-06-06 11:43:28.403387 faKy-1.3.0/setup.cfg
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      727 2023-06-06 11:43:23.000000 faKy-1.3.0/setup.py
```

### Comparing `faKy-1.2.3/PKG-INFO` & `faKy-1.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: faKy
-Version: 1.2.3
+Version: 1.3.0
 Summary: Your library description
 Author: Sandro Barres Hamers
 Author-email: sbarreshamers@gmail.com
 Description-Content-Type: text/markdown
 Provides-Extra: vader
-Provides-Extra: en
 
 # faKy
 
 This library provides functionality for analyzing text using various techniques and models. It includes functions for calculating readability scores, sentiment analysis using VADER, counting named entities, analyzing part-of-speech tags, and more.
 
 ## Installation
```

### Comparing `faKy-1.2.3/faKy/faKy.py` & `faKy-1.3.0/faKy/faKy.py`

 * *Files identical despite different names*

### Comparing `faKy-1.2.3/faKy.egg-info/PKG-INFO` & `faKy-1.3.0/faKy.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: faKy
-Version: 1.2.3
+Version: 1.3.0
 Summary: Your library description
 Author: Sandro Barres Hamers
 Author-email: sbarreshamers@gmail.com
 Description-Content-Type: text/markdown
 Provides-Extra: vader
-Provides-Extra: en
 
 # faKy
 
 This library provides functionality for analyzing text using various techniques and models. It includes functions for calculating readability scores, sentiment analysis using VADER, counting named entities, analyzing part-of-speech tags, and more.
 
 ## Installation
```

### Comparing `faKy-1.2.3/setup.py` & `faKy-1.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('readme.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='faKy',
-    version='1.2.3',
+    version='1.3.0',
     description='Your library description',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Sandro Barres Hamers',
     author_email='sbarreshamers@gmail.com',
     packages=['faKy'],
     install_requires=[
@@ -18,10 +18,12 @@
         'pandas==1.3.4',
         'spacy-readability==1.4.1',
         'nltk==3.7',
         'vaderSentiment==3.3.2',
     ],
     extras_require={
         'vader': ['vaderSentiment'],
-        'en': ['en_core_web_md'],
+    },
+    package_data={
+        'faKy': ['en_core_web_md-2.3.1/*'],
     },
 )
```

