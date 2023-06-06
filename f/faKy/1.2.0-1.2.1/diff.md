# Comparing `tmp/faKy-1.2.0.tar.gz` & `tmp/faKy-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faKy-1.2.0.tar", last modified: Tue Jun  6 10:53:53 2023, max compression
+gzip compressed data, was "faKy-1.2.1.tar", last modified: Tue Jun  6 11:12:50 2023, max compression
```

## Comparing `faKy-1.2.0.tar` & `faKy-1.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 10:53:53.357383 faKy-1.2.0/
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      719 2023-06-06 10:53:53.357090 faKy-1.2.0/PKG-INFO
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      488 2023-06-06 09:01:46.000000 faKy-1.2.0/README.md
-drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 10:53:53.354189 faKy-1.2.0/faKy/
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        1 2023-06-06 08:19:35.000000 faKy-1.2.0/faKy/__init__.py
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     8053 2023-06-06 08:14:25.000000 faKy-1.2.0/faKy/faKy.py
-drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 10:53:53.356616 faKy-1.2.0/faKy.egg-info/
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      719 2023-06-06 10:53:53.000000 faKy-1.2.0/faKy.egg-info/PKG-INFO
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      187 2023-06-06 10:53:53.000000 faKy-1.2.0/faKy.egg-info/SOURCES.txt
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        1 2023-06-06 10:53:53.000000 faKy-1.2.0/faKy.egg-info/dependency_links.txt
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      145 2023-06-06 10:53:53.000000 faKy-1.2.0/faKy.egg-info/requires.txt
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        5 2023-06-06 10:53:53.000000 faKy-1.2.0/faKy.egg-info/top_level.txt
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)       38 2023-06-06 10:53:53.357504 faKy-1.2.0/setup.cfg
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      693 2023-06-06 10:51:30.000000 faKy-1.2.0/setup.py
+drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 11:12:50.254754 faKy-1.2.1/
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      719 2023-06-06 11:12:50.254439 faKy-1.2.1/PKG-INFO
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      488 2023-06-06 09:01:46.000000 faKy-1.2.1/README.md
+drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 11:12:50.250928 faKy-1.2.1/faKy/
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        1 2023-06-06 08:19:35.000000 faKy-1.2.1/faKy/__init__.py
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     8053 2023-06-06 08:14:25.000000 faKy-1.2.1/faKy/faKy.py
+drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 11:12:50.253323 faKy-1.2.1/faKy.egg-info/
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      719 2023-06-06 11:12:50.000000 faKy-1.2.1/faKy.egg-info/PKG-INFO
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      187 2023-06-06 11:12:50.000000 faKy-1.2.1/faKy.egg-info/SOURCES.txt
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        1 2023-06-06 11:12:50.000000 faKy-1.2.1/faKy.egg-info/dependency_links.txt
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      143 2023-06-06 11:12:50.000000 faKy-1.2.1/faKy.egg-info/requires.txt
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        5 2023-06-06 11:12:50.000000 faKy-1.2.1/faKy.egg-info/top_level.txt
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)       38 2023-06-06 11:12:50.254871 faKy-1.2.1/setup.cfg
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      691 2023-06-06 11:12:44.000000 faKy-1.2.1/setup.py
```

### Comparing `faKy-1.2.0/PKG-INFO` & `faKy-1.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faKy
-Version: 1.2.0
+Version: 1.2.1
 Summary: Your library description
 Author: Sandro Barres Hamers
 Author-email: sbarreshamers@gmail.com
 Description-Content-Type: text/markdown
 Provides-Extra: vader
 Provides-Extra: en
```

### Comparing `faKy-1.2.0/faKy/faKy.py` & `faKy-1.2.1/faKy/faKy.py`

 * *Files identical despite different names*

### Comparing `faKy-1.2.0/faKy.egg-info/PKG-INFO` & `faKy-1.2.1/faKy.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faKy
-Version: 1.2.0
+Version: 1.2.1
 Summary: Your library description
 Author: Sandro Barres Hamers
 Author-email: sbarreshamers@gmail.com
 Description-Content-Type: text/markdown
 Provides-Extra: vader
 Provides-Extra: en
```

### Comparing `faKy-1.2.0/setup.py` & `faKy-1.2.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup
 
 with open('readme.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='faKy',
-    version='1.2.0',
+    version='1.2.1',
     description='Your library description',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Sandro Barres Hamers',
     author_email='sbarreshamers@gmail.com',
     packages=['faKy'],
     install_requires=[
         'numpy==1.24.2',
-        'spacy==3.0.0',
+        'spacy==2.3.9',
         'pandas==1.3.4',
         'spacy-readability==1.4.1',
-        'nltk==3.6.5',
+        'nltk==3.7',
         'vaderSentiment==3.3.2',
     ],
     extras_require={
         'vader': ['vaderSentiment'],
         'en': ['en_core_web_md'],
     },
 )
```

