# Comparing `tmp/cpquant-0.0.2.tar.gz` & `tmp/cpquant-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpquant-0.0.2.tar", last modified: Mon Jun  5 22:22:42 2023, max compression
+gzip compressed data, was "cpquant-0.0.3.tar", last modified: Mon Jun  5 22:21:42 2023, max compression
```

## Comparing `cpquant-0.0.2.tar` & `cpquant-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 charlieray   (501) staff       (20)        0 2023-06-05 22:22:42.821817 cpquant-0.0.2/
--rw-r--r--   0 charlieray   (501) staff       (20)     1076 2023-06-05 20:27:13.000000 cpquant-0.0.2/LICENSE
--rw-r--r--   0 charlieray   (501) staff       (20)      522 2023-06-05 22:22:42.821663 cpquant-0.0.2/PKG-INFO
--rw-r--r--   0 charlieray   (501) staff       (20)       80 2023-06-05 20:27:13.000000 cpquant-0.0.2/README.md
-drwxr-xr-x   0 charlieray   (501) staff       (20)        0 2023-06-05 22:22:42.820690 cpquant-0.0.2/cpquant/
--rw-r--r--   0 charlieray   (501) staff       (20)       19 2023-06-05 22:22:39.000000 cpquant-0.0.2/cpquant/__init__.py
--rw-r--r--   0 charlieray   (501) staff       (20)       65 2023-06-05 22:10:54.000000 cpquant-0.0.2/cpquant/data.py
-drwxr-xr-x   0 charlieray   (501) staff       (20)        0 2023-06-05 22:22:42.821456 cpquant-0.0.2/cpquant.egg-info/
--rw-r--r--   0 charlieray   (501) staff       (20)      522 2023-06-05 22:22:42.000000 cpquant-0.0.2/cpquant.egg-info/PKG-INFO
--rw-r--r--   0 charlieray   (501) staff       (20)      186 2023-06-05 22:22:42.000000 cpquant-0.0.2/cpquant.egg-info/SOURCES.txt
--rw-r--r--   0 charlieray   (501) staff       (20)        1 2023-06-05 22:22:42.000000 cpquant-0.0.2/cpquant.egg-info/dependency_links.txt
--rw-r--r--   0 charlieray   (501) staff       (20)        8 2023-06-05 22:22:42.000000 cpquant-0.0.2/cpquant.egg-info/top_level.txt
--rw-r--r--   0 charlieray   (501) staff       (20)       38 2023-06-05 22:22:42.821863 cpquant-0.0.2/setup.cfg
--rw-r--r--   0 charlieray   (501) staff       (20)      651 2023-06-05 22:22:17.000000 cpquant-0.0.2/setup.py
+drwxr-xr-x   0 charlieray   (501) staff       (20)        0 2023-06-05 22:21:42.298558 cpquant-0.0.3/
+-rw-r--r--   0 charlieray   (501) staff       (20)     1076 2023-06-05 20:27:13.000000 cpquant-0.0.3/LICENSE
+-rw-r--r--   0 charlieray   (501) staff       (20)      522 2023-06-05 22:21:42.298380 cpquant-0.0.3/PKG-INFO
+-rw-r--r--   0 charlieray   (501) staff       (20)       80 2023-06-05 20:27:13.000000 cpquant-0.0.3/README.md
+drwxr-xr-x   0 charlieray   (501) staff       (20)        0 2023-06-05 22:21:42.296080 cpquant-0.0.3/cpquant/
+-rw-r--r--   0 charlieray   (501) staff       (20)       14 2023-06-05 20:36:17.000000 cpquant-0.0.3/cpquant/__init__.py
+-rw-r--r--   0 charlieray   (501) staff       (20)       65 2023-06-05 22:10:54.000000 cpquant-0.0.3/cpquant/data.py
+drwxr-xr-x   0 charlieray   (501) staff       (20)        0 2023-06-05 22:21:42.298157 cpquant-0.0.3/cpquant.egg-info/
+-rw-r--r--   0 charlieray   (501) staff       (20)      522 2023-06-05 22:21:42.000000 cpquant-0.0.3/cpquant.egg-info/PKG-INFO
+-rw-r--r--   0 charlieray   (501) staff       (20)      186 2023-06-05 22:21:42.000000 cpquant-0.0.3/cpquant.egg-info/SOURCES.txt
+-rw-r--r--   0 charlieray   (501) staff       (20)        1 2023-06-05 22:21:42.000000 cpquant-0.0.3/cpquant.egg-info/dependency_links.txt
+-rw-r--r--   0 charlieray   (501) staff       (20)        8 2023-06-05 22:21:42.000000 cpquant-0.0.3/cpquant.egg-info/top_level.txt
+-rw-r--r--   0 charlieray   (501) staff       (20)       38 2023-06-05 22:21:42.298606 cpquant-0.0.3/setup.cfg
+-rw-r--r--   0 charlieray   (501) staff       (20)      651 2023-06-05 22:21:39.000000 cpquant-0.0.3/setup.py
```

### Comparing `cpquant-0.0.2/LICENSE` & `cpquant-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cpquant-0.0.2/PKG-INFO` & `cpquant-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpquant
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package containing common functions for CP Quant Club
 Home-page: https://github.com/Cal-Poly-Quant-Club/cpquant
 Author: Charlie Ray
 Author-email: charlie.ray320@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cpquant-0.0.2/cpquant.egg-info/PKG-INFO` & `cpquant-0.0.3/cpquant.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpquant
-Version: 0.0.2
+Version: 0.0.3
 Summary: A package containing common functions for CP Quant Club
 Home-page: https://github.com/Cal-Poly-Quant-Club/cpquant
 Author: Charlie Ray
 Author-email: charlie.ray320@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cpquant-0.0.2/setup.py` & `cpquant-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cpquant",
-    version="0.0.2",
+    version="0.0.3",
     author="Charlie Ray",
     author_email="charlie.ray320@gmail.com",
     description="A package containing common functions for CP Quant Club",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Cal-Poly-Quant-Club/cpquant",
     packages=setuptools.find_packages(),
```

