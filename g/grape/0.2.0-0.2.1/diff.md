# Comparing `tmp/grape-0.2.0.tar.gz` & `tmp/grape-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grape-0.2.0.tar", last modified: Tue Jun  6 08:45:20 2023, max compression
+gzip compressed data, was "dist/grape-0.2.1.tar", last modified: Tue Jun  6 13:05:20 2023, max compression
```

## Comparing `grape-0.2.0.tar` & `grape-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 luca      (1001) luca      (1003)        0 2023-06-06 08:45:20.095202 grape-0.2.0/
--rw-r--r--   0 luca      (1001) luca      (1003)     1090 2023-05-14 14:45:38.000000 grape-0.2.0/LICENSE
--rw-r--r--   0 luca      (1001) luca      (1003)    12754 2023-06-06 08:45:20.095202 grape-0.2.0/PKG-INFO
--rw-r--r--   0 luca      (1001) luca      (1003)    12156 2023-05-21 21:27:34.000000 grape-0.2.0/README.rst
-drwxr-xr-x   0 luca      (1001) luca      (1003)        0 2023-06-06 08:45:20.095202 grape-0.2.0/grape/
--rw-r--r--   0 luca      (1001) luca      (1003)     2538 2023-05-14 14:45:38.000000 grape-0.2.0/grape/__init__.py
--rw-r--r--   0 luca      (1001) luca      (1003)       62 2023-06-06 08:44:21.000000 grape-0.2.0/grape/__version__.py
-drwxr-xr-x   0 luca      (1001) luca      (1003)        0 2023-06-06 08:45:20.095202 grape-0.2.0/grape.egg-info/
--rw-r--r--   0 luca      (1001) luca      (1003)    12754 2023-06-06 08:45:20.000000 grape-0.2.0/grape.egg-info/PKG-INFO
--rw-r--r--   0 luca      (1001) luca      (1003)      210 2023-06-06 08:45:20.000000 grape-0.2.0/grape.egg-info/SOURCES.txt
--rw-r--r--   0 luca      (1001) luca      (1003)        1 2023-06-06 08:45:20.000000 grape-0.2.0/grape.egg-info/dependency_links.txt
--rw-r--r--   0 luca      (1001) luca      (1003)       71 2023-06-06 08:45:20.000000 grape-0.2.0/grape.egg-info/requires.txt
--rw-r--r--   0 luca      (1001) luca      (1003)        6 2023-06-06 08:45:20.000000 grape-0.2.0/grape.egg-info/top_level.txt
--rw-r--r--   0 luca      (1001) luca      (1003)       38 2023-06-06 08:45:20.095202 grape-0.2.0/setup.cfg
--rw-r--r--   0 luca      (1001) luca      (1003)     1924 2023-06-06 08:44:35.000000 grape-0.2.0/setup.py
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2023-06-06 13:05:20.000000 grape-0.2.1/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     1090 2021-09-06 15:24:55.000000 grape-0.2.1/LICENSE
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)    12734 2023-06-06 13:05:20.000000 grape-0.2.1/PKG-INFO
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)    12156 2023-06-06 08:46:56.000000 grape-0.2.1/README.rst
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2023-06-06 13:05:20.000000 grape-0.2.1/grape/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     2538 2022-08-21 09:09:13.000000 grape-0.2.1/grape/__init__.py
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)       62 2023-06-06 13:04:51.000000 grape-0.2.1/grape/__version__.py
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2023-06-06 13:05:20.000000 grape-0.2.1/grape.egg-info/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)    12734 2023-06-06 13:05:20.000000 grape-0.2.1/grape.egg-info/PKG-INFO
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      232 2023-06-06 13:05:20.000000 grape-0.2.1/grape.egg-info/SOURCES.txt
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)        1 2023-06-06 13:05:20.000000 grape-0.2.1/grape.egg-info/dependency_links.txt
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)       71 2023-06-06 13:05:20.000000 grape-0.2.1/grape.egg-info/requires.txt
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)        6 2023-06-06 13:05:20.000000 grape-0.2.1/grape.egg-info/top_level.txt
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)       38 2023-06-06 13:05:20.000000 grape-0.2.1/setup.cfg
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)     1924 2023-06-06 13:04:57.000000 grape-0.2.1/setup.py
+drwxr-xr-x   0 lucacappelletti   (501) staff       (20)        0 2023-06-06 13:05:20.000000 grape-0.2.1/tests/
+-rw-r--r--   0 lucacappelletti   (501) staff       (20)      198 2022-06-07 11:36:25.000000 grape-0.2.1/tests/test_imports.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `grape-0.2.0/LICENSE` & `grape-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `grape-0.2.0/PKG-INFO` & `grape-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: grape
-Version: 0.2.0
+Version: 0.2.1
 Summary: 🍇 GRAPE is a Rust/Python Graph Representation Learning library for Predictions and Evaluations.
 Home-page: https://github.com/AnacletoLAB/grape
 Author: Luca Cappelletti, Tommaso Fontana, Vida Ravanmehr, Peter Robinson
 Author-email: luca.cappelletti1@unimi.it, tommaso.fontana@mail.polimi.it, vida.ravanmehr@jax.org, peter.robinson@jax.org
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
 🍇 GRAPE
 ===================================
@@ -217,9 +216,7 @@
 .. |discord| image:: https://badges.aleen42.com/src/discord.svg
     :target: https://discord.gg/Nda2cqYvTN
     :alt: Discord Server
 
 .. |logo| image:: images/grape_logo.png
     :target: https://github.com/AnacletoLAB/grape
     :width:  80
-
-
```

### Comparing `grape-0.2.0/README.rst` & `grape-0.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `grape-0.2.0/grape/__init__.py` & `grape-0.2.1/grape/__init__.py`

 * *Files identical despite different names*

### Comparing `grape-0.2.0/grape.egg-info/PKG-INFO` & `grape-0.2.1/grape.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: grape
-Version: 0.2.0
+Version: 0.2.1
 Summary: 🍇 GRAPE is a Rust/Python Graph Representation Learning library for Predictions and Evaluations.
 Home-page: https://github.com/AnacletoLAB/grape
 Author: Luca Cappelletti, Tommaso Fontana, Vida Ravanmehr, Peter Robinson
 Author-email: luca.cappelletti1@unimi.it, tommaso.fontana@mail.polimi.it, vida.ravanmehr@jax.org, peter.robinson@jax.org
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
 🍇 GRAPE
 ===================================
@@ -217,9 +216,7 @@
 .. |discord| image:: https://badges.aleen42.com/src/discord.svg
     :target: https://discord.gg/Nda2cqYvTN
     :alt: Discord Server
 
 .. |logo| image:: images/grape_logo.png
     :target: https://github.com/AnacletoLAB/grape
     :width:  80
-
-
```

### Comparing `grape-0.2.0/setup.py` & `grape-0.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,10 +60,10 @@
     packages=find_packages(exclude=['contrib', 'docs', 'tests*']),
     tests_require=test_deps,
     install_requires=[
         "downloaders",
         "bioregistry",
         "py-cpuinfo",
         "ensmallen>=0.8.60",
-        "embiggen>=0.11.54",
+        "embiggen>=0.11.56",
     ]
 )
```

