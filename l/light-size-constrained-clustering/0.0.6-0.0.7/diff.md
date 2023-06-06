# Comparing `tmp/light_size_constrained_clustering-0.0.6.tar.gz` & `tmp/light_size_constrained_clustering-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "light_size_constrained_clustering-0.0.6.tar", last modified: Mon May 29 08:48:16 2023, max compression
+gzip compressed data, was "light_size_constrained_clustering-0.0.7.tar", last modified: Tue Jun  6 14:22:58 2023, max compression
```

## Comparing `light_size_constrained_clustering-0.0.6.tar` & `light_size_constrained_clustering-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 i0365030   (502) staff       (20)        0 2023-05-29 08:48:16.492337 light_size_constrained_clustering-0.0.6/
--rw-r--r--   0 i0365030   (502) staff       (20)     1074 2023-05-24 18:28:58.000000 light_size_constrained_clustering-0.0.6/LICENSE
--rw-r--r--   0 i0365030   (502) staff       (20)     3646 2023-05-29 08:48:16.492120 light_size_constrained_clustering-0.0.6/PKG-INFO
--rw-r--r--   0 i0365030   (502) staff       (20)     3299 2023-05-25 17:12:16.000000 light_size_constrained_clustering-0.0.6/README.md
-drwxr-xr-x   0 i0365030   (502) staff       (20)        0 2023-05-29 08:48:16.490894 light_size_constrained_clustering-0.0.6/light_size_constrained_clustering/
--rw-r--r--   0 i0365030   (502) staff       (20)      106 2023-05-25 16:50:29.000000 light_size_constrained_clustering-0.0.6/light_size_constrained_clustering/__init__.py
--rw-r--r--   0 i0365030   (502) staff       (20)     6178 2023-05-25 16:50:29.000000 light_size_constrained_clustering-0.0.6/light_size_constrained_clustering/base.py
--rw-r--r--   0 i0365030   (502) staff       (20)     9292 2023-05-29 08:46:59.000000 light_size_constrained_clustering-0.0.6/light_size_constrained_clustering/da.py
-drwxr-xr-x   0 i0365030   (502) staff       (20)        0 2023-05-29 08:48:16.491761 light_size_constrained_clustering-0.0.6/light_size_constrained_clustering.egg-info/
--rw-r--r--   0 i0365030   (502) staff       (20)     3646 2023-05-29 08:48:16.000000 light_size_constrained_clustering-0.0.6/light_size_constrained_clustering.egg-info/PKG-INFO
--rw-r--r--   0 i0365030   (502) staff       (20)      455 2023-05-29 08:48:16.000000 light_size_constrained_clustering-0.0.6/light_size_constrained_clustering.egg-info/SOURCES.txt
--rw-r--r--   0 i0365030   (502) staff       (20)        1 2023-05-29 08:48:16.000000 light_size_constrained_clustering-0.0.6/light_size_constrained_clustering.egg-info/dependency_links.txt
--rw-r--r--   0 i0365030   (502) staff       (20)      106 2023-05-29 08:48:16.000000 light_size_constrained_clustering-0.0.6/light_size_constrained_clustering.egg-info/requires.txt
--rw-r--r--   0 i0365030   (502) staff       (20)       34 2023-05-29 08:48:16.000000 light_size_constrained_clustering-0.0.6/light_size_constrained_clustering.egg-info/top_level.txt
--rw-r--r--   0 i0365030   (502) staff       (20)       38 2023-05-29 08:48:16.492406 light_size_constrained_clustering-0.0.6/setup.cfg
--rw-r--r--   0 i0365030   (502) staff       (20)     1140 2023-05-29 08:47:37.000000 light_size_constrained_clustering-0.0.6/setup.py
-drwxr-xr-x   0 i0365030   (502) staff       (20)        0 2023-05-29 08:48:16.491891 light_size_constrained_clustering-0.0.6/tests/
--rw-r--r--   0 i0365030   (502) staff       (20)     1341 2023-05-25 16:50:29.000000 light_size_constrained_clustering-0.0.6/tests/test_da.py
+drwxr-xr-x   0 i0365030   (502) staff       (20)        0 2023-06-06 14:22:58.654576 light_size_constrained_clustering-0.0.7/
+-rw-r--r--   0 i0365030   (502) staff       (20)     1074 2023-05-24 18:28:58.000000 light_size_constrained_clustering-0.0.7/LICENSE
+-rw-r--r--   0 i0365030   (502) staff       (20)     3646 2023-06-06 14:22:58.654421 light_size_constrained_clustering-0.0.7/PKG-INFO
+-rw-r--r--   0 i0365030   (502) staff       (20)     3299 2023-05-25 17:12:16.000000 light_size_constrained_clustering-0.0.7/README.md
+drwxr-xr-x   0 i0365030   (502) staff       (20)        0 2023-06-06 14:22:58.652869 light_size_constrained_clustering-0.0.7/light_size_constrained_clustering/
+-rw-r--r--   0 i0365030   (502) staff       (20)      106 2023-05-25 16:50:29.000000 light_size_constrained_clustering-0.0.7/light_size_constrained_clustering/__init__.py
+-rw-r--r--   0 i0365030   (502) staff       (20)     6178 2023-05-25 16:50:29.000000 light_size_constrained_clustering-0.0.7/light_size_constrained_clustering/base.py
+-rw-r--r--   0 i0365030   (502) staff       (20)     9292 2023-05-29 08:46:59.000000 light_size_constrained_clustering-0.0.7/light_size_constrained_clustering/da.py
+drwxr-xr-x   0 i0365030   (502) staff       (20)        0 2023-06-06 14:22:58.653997 light_size_constrained_clustering-0.0.7/light_size_constrained_clustering.egg-info/
+-rw-r--r--   0 i0365030   (502) staff       (20)     3646 2023-06-06 14:22:58.000000 light_size_constrained_clustering-0.0.7/light_size_constrained_clustering.egg-info/PKG-INFO
+-rw-r--r--   0 i0365030   (502) staff       (20)      455 2023-06-06 14:22:58.000000 light_size_constrained_clustering-0.0.7/light_size_constrained_clustering.egg-info/SOURCES.txt
+-rw-r--r--   0 i0365030   (502) staff       (20)        1 2023-06-06 14:22:58.000000 light_size_constrained_clustering-0.0.7/light_size_constrained_clustering.egg-info/dependency_links.txt
+-rw-r--r--   0 i0365030   (502) staff       (20)      106 2023-06-06 14:22:58.000000 light_size_constrained_clustering-0.0.7/light_size_constrained_clustering.egg-info/requires.txt
+-rw-r--r--   0 i0365030   (502) staff       (20)       34 2023-06-06 14:22:58.000000 light_size_constrained_clustering-0.0.7/light_size_constrained_clustering.egg-info/top_level.txt
+-rw-r--r--   0 i0365030   (502) staff       (20)       38 2023-06-06 14:22:58.654616 light_size_constrained_clustering-0.0.7/setup.cfg
+-rw-r--r--   0 i0365030   (502) staff       (20)     1140 2023-06-06 14:22:01.000000 light_size_constrained_clustering-0.0.7/setup.py
+drwxr-xr-x   0 i0365030   (502) staff       (20)        0 2023-06-06 14:22:58.654142 light_size_constrained_clustering-0.0.7/tests/
+-rw-r--r--   0 i0365030   (502) staff       (20)     1341 2023-05-25 16:50:29.000000 light_size_constrained_clustering-0.0.7/tests/test_da.py
```

### Comparing `light_size_constrained_clustering-0.0.6/LICENSE` & `light_size_constrained_clustering-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `light_size_constrained_clustering-0.0.6/PKG-INFO` & `light_size_constrained_clustering-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: light_size_constrained_clustering
-Version: 0.0.6
+Version: 0.0.7
 Summary: Size Constrained Clustering solver
 Home-page: https://github.com/AlbertPlaPlanas/size_constrained_clustering
 Author: Albert Pla
 Author-email: plaalbert@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `light_size_constrained_clustering-0.0.6/README.md` & `light_size_constrained_clustering-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `light_size_constrained_clustering-0.0.6/light_size_constrained_clustering/base.py` & `light_size_constrained_clustering-0.0.7/light_size_constrained_clustering/base.py`

 * *Files identical despite different names*

### Comparing `light_size_constrained_clustering-0.0.6/light_size_constrained_clustering/da.py` & `light_size_constrained_clustering-0.0.7/light_size_constrained_clustering/da.py`

 * *Files identical despite different names*

### Comparing `light_size_constrained_clustering-0.0.6/light_size_constrained_clustering.egg-info/PKG-INFO` & `light_size_constrained_clustering-0.0.7/light_size_constrained_clustering.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: light-size-constrained-clustering
-Version: 0.0.6
+Version: 0.0.7
 Summary: Size Constrained Clustering solver
 Home-page: https://github.com/AlbertPlaPlanas/size_constrained_clustering
 Author: Albert Pla
 Author-email: plaalbert@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `light_size_constrained_clustering-0.0.6/setup.py` & `light_size_constrained_clustering-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 path = os.path.dirname(os.path.abspath(__file__))
 
 with open(os.path.join(path, "requirements.txt")) as fp:
     install_requires = fp.read().strip().split("\n")
 
 
-VERSION = "0.0.6"
+VERSION = "0.0.7"
 LICENSE = "MIT"
 setup(
     #ext_modules=extensions,
     version=VERSION,
     setup_requires=["numpy"],
     install_requires=install_requires,
     name="light_size_constrained_clustering",
```

### Comparing `light_size_constrained_clustering-0.0.6/tests/test_da.py` & `light_size_constrained_clustering-0.0.7/tests/test_da.py`

 * *Files identical despite different names*

