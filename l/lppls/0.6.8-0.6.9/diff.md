# Comparing `tmp/lppls-0.6.8.tar.gz` & `tmp/lppls-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lppls-0.6.8.tar", last modified: Thu Mar 23 04:23:35 2023, max compression
+gzip compressed data, was "lppls-0.6.9.tar", last modified: Tue Jun  6 05:09:23 2023, max compression
```

## Comparing `lppls-0.6.8.tar` & `lppls-0.6.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 04:23:35.861576 lppls-0.6.8/
--rw-r--r--   0 runner    (1001) docker     (123)     9162 2023-03-23 04:23:35.861576 lppls-0.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-03-23 04:23:23.000000 lppls-0.6.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 04:23:35.857576 lppls-0.6.8/lppls/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 04:23:35.861576 lppls-0.6.8/lppls/data/
--rw-r--r--   0 runner    (1001) docker     (123)   124809 2023-03-23 04:23:23.000000 lppls-0.6.8/lppls/data/nasdaq_dotcom.csv
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-03-23 04:23:23.000000 lppls-0.6.8/lppls/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    21575 2023-03-23 04:23:23.000000 lppls-0.6.8/lppls/lppls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-03-23 04:23:23.000000 lppls-0.6.8/lppls/lppls_cmaes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 04:23:35.861576 lppls-0.6.8/lppls.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9162 2023-03-23 04:23:35.000000 lppls-0.6.8/lppls.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-03-23 04:23:35.000000 lppls-0.6.8/lppls.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 04:23:35.000000 lppls-0.6.8/lppls.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 04:23:35.000000 lppls-0.6.8/lppls.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-23 04:23:35.000000 lppls-0.6.8/lppls.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-23 04:23:35.000000 lppls-0.6.8/lppls.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-23 04:23:35.861576 lppls-0.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-03-23 04:23:23.000000 lppls-0.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 05:09:23.663106 lppls-0.6.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     7156 2023-06-06 05:09:23.663106 lppls-0.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6850 2023-06-06 05:09:11.000000 lppls-0.6.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 05:09:23.659106 lppls-0.6.9/lppls/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 05:09:23.663106 lppls-0.6.9/lppls/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   124809 2023-06-06 05:09:11.000000 lppls-0.6.9/lppls/data/nasdaq_dotcom.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-06 05:09:11.000000 lppls-0.6.9/lppls/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21575 2023-06-06 05:09:11.000000 lppls-0.6.9/lppls/lppls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-06-06 05:09:11.000000 lppls-0.6.9/lppls/lppls_cmaes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 05:09:23.663106 lppls-0.6.9/lppls.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7156 2023-06-06 05:09:23.000000 lppls-0.6.9/lppls.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-06 05:09:23.000000 lppls-0.6.9/lppls.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 05:09:23.000000 lppls-0.6.9/lppls.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 05:09:23.000000 lppls-0.6.9/lppls.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-06 05:09:23.000000 lppls-0.6.9/lppls.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-06 05:09:23.000000 lppls-0.6.9/lppls.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-06 05:09:23.663106 lppls-0.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-06 05:09:11.000000 lppls-0.6.9/setup.py
```

### Comparing `lppls-0.6.8/lppls/data/nasdaq_dotcom.csv` & `lppls-0.6.9/lppls/data/nasdaq_dotcom.csv`

 * *Files identical despite different names*

### Comparing `lppls-0.6.8/lppls/data_loader.py` & `lppls-0.6.9/lppls/data_loader.py`

 * *Files identical despite different names*

### Comparing `lppls-0.6.8/lppls/lppls.py` & `lppls-0.6.9/lppls/lppls.py`

 * *Files identical despite different names*

### Comparing `lppls-0.6.8/lppls/lppls_cmaes.py` & `lppls-0.6.9/lppls/lppls_cmaes.py`

 * *Files identical despite different names*

### Comparing `lppls-0.6.8/setup.py` & `lppls-0.6.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(name='lppls',
-      version='0.6.8',
+      version='0.6.9',
       description='A Python module for fitting the LPPLS model to data.',
       packages=['lppls'],
       author='Josh Nielsen',
       author_email='josh@boulderinvestment.tech',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/Boulder-Investment-Technologies/lppls',
```

