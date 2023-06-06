# Comparing `tmp/faKy-1.2.1.tar.gz` & `tmp/faKy-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faKy-1.2.1.tar", last modified: Tue Jun  6 11:12:50 2023, max compression
+gzip compressed data, was "faKy-1.2.3.tar", last modified: Tue Jun  6 11:20:46 2023, max compression
```

## Comparing `faKy-1.2.1.tar` & `faKy-1.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 11:12:50.254754 faKy-1.2.1/
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      719 2023-06-06 11:12:50.254439 faKy-1.2.1/PKG-INFO
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      488 2023-06-06 09:01:46.000000 faKy-1.2.1/README.md
-drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 11:12:50.250928 faKy-1.2.1/faKy/
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        1 2023-06-06 08:19:35.000000 faKy-1.2.1/faKy/__init__.py
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     8053 2023-06-06 08:14:25.000000 faKy-1.2.1/faKy/faKy.py
-drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 11:12:50.253323 faKy-1.2.1/faKy.egg-info/
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      719 2023-06-06 11:12:50.000000 faKy-1.2.1/faKy.egg-info/PKG-INFO
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      187 2023-06-06 11:12:50.000000 faKy-1.2.1/faKy.egg-info/SOURCES.txt
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        1 2023-06-06 11:12:50.000000 faKy-1.2.1/faKy.egg-info/dependency_links.txt
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      143 2023-06-06 11:12:50.000000 faKy-1.2.1/faKy.egg-info/requires.txt
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        5 2023-06-06 11:12:50.000000 faKy-1.2.1/faKy.egg-info/top_level.txt
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)       38 2023-06-06 11:12:50.254871 faKy-1.2.1/setup.cfg
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      691 2023-06-06 11:12:44.000000 faKy-1.2.1/setup.py
+drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 11:20:46.194816 faKy-1.2.3/
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      719 2023-06-06 11:20:46.194532 faKy-1.2.3/PKG-INFO
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      488 2023-06-06 09:01:46.000000 faKy-1.2.3/README.md
+drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 11:20:46.191902 faKy-1.2.3/faKy/
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        1 2023-06-06 08:19:35.000000 faKy-1.2.3/faKy/__init__.py
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     8053 2023-06-06 08:14:25.000000 faKy-1.2.3/faKy/faKy.py
+drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 11:20:46.194073 faKy-1.2.3/faKy.egg-info/
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      719 2023-06-06 11:20:46.000000 faKy-1.2.3/faKy.egg-info/PKG-INFO
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      187 2023-06-06 11:20:46.000000 faKy-1.2.3/faKy.egg-info/SOURCES.txt
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        1 2023-06-06 11:20:46.000000 faKy-1.2.3/faKy.egg-info/dependency_links.txt
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      143 2023-06-06 11:20:46.000000 faKy-1.2.3/faKy.egg-info/requires.txt
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        5 2023-06-06 11:20:46.000000 faKy-1.2.3/faKy.egg-info/top_level.txt
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)       38 2023-06-06 11:20:46.194932 faKy-1.2.3/setup.cfg
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      691 2023-06-06 11:20:41.000000 faKy-1.2.3/setup.py
```

### Comparing `faKy-1.2.1/PKG-INFO` & `faKy-1.2.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faKy
-Version: 1.2.1
+Version: 1.2.3
 Summary: Your library description
 Author: Sandro Barres Hamers
 Author-email: sbarreshamers@gmail.com
 Description-Content-Type: text/markdown
 Provides-Extra: vader
 Provides-Extra: en
```

### Comparing `faKy-1.2.1/faKy/faKy.py` & `faKy-1.2.3/faKy/faKy.py`

 * *Files identical despite different names*

### Comparing `faKy-1.2.1/faKy.egg-info/PKG-INFO` & `faKy-1.2.3/faKy.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faKy
-Version: 1.2.1
+Version: 1.2.3
 Summary: Your library description
 Author: Sandro Barres Hamers
 Author-email: sbarreshamers@gmail.com
 Description-Content-Type: text/markdown
 Provides-Extra: vader
 Provides-Extra: en
```

### Comparing `faKy-1.2.1/setup.py` & `faKy-1.2.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('readme.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='faKy',
-    version='1.2.1',
+    version='1.2.3',
     description='Your library description',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Sandro Barres Hamers',
     author_email='sbarreshamers@gmail.com',
     packages=['faKy'],
     install_requires=[
```

