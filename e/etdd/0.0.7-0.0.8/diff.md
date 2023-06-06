# Comparing `tmp/etdd-0.0.7.tar.gz` & `tmp/etdd-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etdd-0.0.7.tar", last modified: Tue Jun  6 11:53:49 2023, max compression
+gzip compressed data, was "etdd-0.0.8.tar", last modified: Tue Jun  6 12:15:32 2023, max compression
```

## Comparing `etdd-0.0.7.tar` & `etdd-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-06 11:53:49.681840 etdd-0.0.7/
--rw-rw-r--   0 user      (1000) user      (1000)     1516 2023-06-05 11:53:50.000000 etdd-0.0.7/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)     1080 2023-06-06 11:53:49.681840 etdd-0.0.7/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      431 2023-06-06 11:49:15.000000 etdd-0.0.7/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-06 11:53:49.681840 etdd-0.0.7/etdd/
--rwxrwxr-x   0 user      (1000) user      (1000)       38 2023-06-06 11:48:09.000000 etdd-0.0.7/etdd/__init__.py
--rwxrwxr-x   0 user      (1000) user      (1000)    16709 2023-06-06 11:47:58.000000 etdd-0.0.7/etdd/core.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-06 11:53:49.681840 etdd-0.0.7/etdd.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     1080 2023-06-06 11:53:49.000000 etdd-0.0.7/etdd.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      195 2023-06-06 11:53:49.000000 etdd-0.0.7/etdd.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-06 11:53:49.000000 etdd-0.0.7/etdd.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       46 2023-06-06 11:53:49.000000 etdd-0.0.7/etdd.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        5 2023-06-06 11:53:49.000000 etdd-0.0.7/etdd.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-06 11:53:49.681840 etdd-0.0.7/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1111 2023-06-06 11:53:48.000000 etdd-0.0.7/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-06 12:15:32.105376 etdd-0.0.8/
+-rw-rw-r--   0 user      (1000) user      (1000)     1516 2023-06-05 11:53:50.000000 etdd-0.0.8/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)     1636 2023-06-06 12:15:32.105376 etdd-0.0.8/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      987 2023-06-06 12:15:13.000000 etdd-0.0.8/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-06 12:15:32.101376 etdd-0.0.8/etdd/
+-rwxrwxr-x   0 user      (1000) user      (1000)       38 2023-06-06 11:48:09.000000 etdd-0.0.8/etdd/__init__.py
+-rwxrwxr-x   0 user      (1000) user      (1000)    16709 2023-06-06 11:47:58.000000 etdd-0.0.8/etdd/core.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-06 12:15:32.101376 etdd-0.0.8/etdd.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     1636 2023-06-06 12:15:32.000000 etdd-0.0.8/etdd.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      195 2023-06-06 12:15:32.000000 etdd-0.0.8/etdd.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-06 12:15:32.000000 etdd-0.0.8/etdd.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       53 2023-06-06 12:15:32.000000 etdd-0.0.8/etdd.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        5 2023-06-06 12:15:32.000000 etdd-0.0.8/etdd.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-06 12:15:32.105376 etdd-0.0.8/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1131 2023-06-06 12:15:29.000000 etdd-0.0.8/setup.py
```

### Comparing `etdd-0.0.7/LICENSE` & `etdd-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `etdd-0.0.7/etdd/core.py` & `etdd-0.0.8/etdd/core.py`

 * *Files identical despite different names*

### Comparing `etdd-0.0.7/setup.py` & `etdd-0.0.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='etdd',
-    version='0.0.7',
+    version='0.0.8',
     description='eTDD framework',
     packages=['etdd'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Topic :: Software Development :: Libraries :: Python Modules",
@@ -28,9 +28,10 @@
     # ]},
     install_requires=[
         'pathlib'
         , 'jinja2'
         , 'colorama'
         , 'tabulate'
         , 'console-menu'
+        , 'lizard'
     ]
 )
```

