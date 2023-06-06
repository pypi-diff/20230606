# Comparing `tmp/UComp-1.0.20.tar.gz` & `tmp/UComp-1.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UComp-1.0.20.tar", last modified: Tue Jun  6 16:59:15 2023, max compression
+gzip compressed data, was "UComp-1.0.21.tar", last modified: Tue Jun  6 17:02:41 2023, max compression
```

## Comparing `UComp-1.0.20.tar` & `UComp-1.0.21.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 16:59:15.972877 UComp-1.0.20/
--rw-rw-rw-   0        0        0      233 2023-06-06 16:58:27.000000 UComp-1.0.20/MANIFEST.in
--rw-rw-rw-   0        0        0      304 2023-06-06 16:59:15.972877 UComp-1.0.20/PKG-INFO
--rw-rw-rw-   0        0        0       37 2023-05-19 10:25:10.000000 UComp-1.0.20/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 16:59:15.957254 UComp-1.0.20/UComp/
--rw-rw-rw-   0        0        0  1451960 2023-05-26 14:15:14.000000 UComp-1.0.20/UComp/ETSc.cpython-311-darwin.so
--rw-rw-rw-   0        0        0   573952 2023-05-19 09:06:21.000000 UComp-1.0.20/UComp/ETSc.pyd
--rw-rw-rw-   0        0        0  1631200 2023-05-26 14:18:31.000000 UComp-1.0.20/UComp/UCc.cpython-311-darwin.so
--rw-rw-rw-   0        0        0  1137664 2023-05-19 08:42:47.000000 UComp-1.0.20/UComp/UCc.pyd
--rw-rw-rw-   0        0        0    18991 2023-06-06 16:33:02.000000 UComp-1.0.20/UComp/UCmodule.py
--rw-rw-rw-   0        0        0       53 2023-06-06 16:51:47.000000 UComp-1.0.20/UComp/__init__.py
--rw-rw-rw-   0        0        0 32492623 2016-06-16 16:24:20.000000 UComp-1.0.20/UComp/libopenblas.dll
--rw-rw-rw-   0        0        0    28922 2023-06-06 14:31:28.000000 UComp-1.0.20/UComp/tools.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:59:15.972877 UComp-1.0.20/UComp.egg-info/
--rw-rw-rw-   0        0        0      304 2023-06-06 16:59:15.000000 UComp-1.0.20/UComp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      341 2023-06-06 16:59:15.000000 UComp-1.0.20/UComp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 16:59:15.000000 UComp-1.0.20/UComp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-06-06 16:59:15.000000 UComp-1.0.20/UComp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-06 16:59:15.000000 UComp-1.0.20/UComp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 16:59:15.972877 UComp-1.0.20/setup.cfg
--rw-rw-rw-   0        0        0      590 2023-06-06 16:58:44.000000 UComp-1.0.20/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 17:02:41.295403 UComp-1.0.21/
+-rw-rw-rw-   0        0        0      233 2023-06-06 16:58:27.000000 UComp-1.0.21/MANIFEST.in
+-rw-rw-rw-   0        0        0      304 2023-06-06 17:02:41.295403 UComp-1.0.21/PKG-INFO
+-rw-rw-rw-   0        0        0       37 2023-05-19 10:25:10.000000 UComp-1.0.21/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 17:02:41.279795 UComp-1.0.21/UComp/
+-rw-rw-rw-   0        0        0  1451960 2023-05-26 14:15:14.000000 UComp-1.0.21/UComp/ETSc.cpython-311-darwin.so
+-rw-rw-rw-   0        0        0   573952 2023-05-19 09:06:21.000000 UComp-1.0.21/UComp/ETSc.pyd
+-rw-rw-rw-   0        0        0  1631200 2023-05-26 14:18:31.000000 UComp-1.0.21/UComp/UCc.cpython-311-darwin.so
+-rw-rw-rw-   0        0        0  1137664 2023-05-19 08:42:47.000000 UComp-1.0.21/UComp/UCc.pyd
+-rw-rw-rw-   0        0        0    18991 2023-06-06 16:33:02.000000 UComp-1.0.21/UComp/UCmodule.py
+-rw-rw-rw-   0        0        0       57 2023-06-06 17:02:10.000000 UComp-1.0.21/UComp/__init__.py
+-rw-rw-rw-   0        0        0 32492623 2016-06-16 16:24:20.000000 UComp-1.0.21/UComp/libopenblas.dll
+-rw-rw-rw-   0        0        0    28922 2023-06-06 14:31:28.000000 UComp-1.0.21/UComp/tools.py
+drwxrwxrwx   0        0        0        0 2023-06-06 17:02:41.295403 UComp-1.0.21/UComp.egg-info/
+-rw-rw-rw-   0        0        0      304 2023-06-06 17:02:41.000000 UComp-1.0.21/UComp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2023-06-06 17:02:41.000000 UComp-1.0.21/UComp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 17:02:41.000000 UComp-1.0.21/UComp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-06-06 17:02:41.000000 UComp-1.0.21/UComp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-06 17:02:41.000000 UComp-1.0.21/UComp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 17:02:41.295403 UComp-1.0.21/setup.cfg
+-rw-rw-rw-   0        0        0      590 2023-06-06 17:02:35.000000 UComp-1.0.21/setup.py
```

### Comparing `UComp-1.0.20/UComp/ETSc.cpython-311-darwin.so` & `UComp-1.0.21/UComp/ETSc.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `UComp-1.0.20/UComp/UCc.cpython-311-darwin.so` & `UComp-1.0.21/UComp/UCc.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `UComp-1.0.20/UComp/UCmodule.py` & `UComp-1.0.21/UComp/UCmodule.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.20/UComp/libopenblas.dll` & `UComp-1.0.21/UComp/libopenblas.dll`

 * *Files identical despite different names*

### Comparing `UComp-1.0.20/UComp/tools.py` & `UComp-1.0.21/UComp/tools.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.20/setup.py` & `UComp-1.0.21/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='UComp',
-    version='1.0.20',
+    version='1.0.21',
     author='Diego J. Pedregal',
     author_email='diego.pedregal@uclm.es',
     description='Modelling and forecasting univariate time series',
     long_description='Modelling and forecasting univariate time series',
     url='https://github.com/djpedregal/UComp',
     packages=find_packages(),
     include_package_data=True,
```

