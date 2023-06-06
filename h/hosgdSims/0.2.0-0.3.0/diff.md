# Comparing `tmp/hosgdSims-0.2.0.tar.gz` & `tmp/hosgdSims-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hosgdSims-0.2.0.tar", last modified: Mon Jun  5 00:27:11 2023, max compression
+gzip compressed data, was "hosgdSims-0.3.0.tar", last modified: Tue Jun  6 05:08:27 2023, max compression
```

## Comparing `hosgdSims-0.2.0.tar` & `hosgdSims-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 jaru      (1000) users      (100)        0 2023-06-05 00:27:11.783589 hosgdSims-0.2.0/
--rw-r--r--   0 jaru      (1000) users      (100)       35 2023-06-04 19:15:40.000000 hosgdSims-0.2.0/AUTHORS
--rw-r--r--   0 jaru      (1000) users      (100)       11 2023-06-05 00:12:56.000000 hosgdSims-0.2.0/MANIFEST.in
--rw-r--r--   0 jaru      (1000) users      (100)      924 2023-06-05 00:27:11.783589 hosgdSims-0.2.0/PKG-INFO
--rw-r--r--   0 jaru      (1000) users      (100)      477 2023-06-04 21:16:25.000000 hosgdSims-0.2.0/README.md
-drwxr-xr-x   0 jaru      (1000) users      (100)        0 2023-06-05 00:27:11.783589 hosgdSims-0.2.0/hosgdSims/
--rw-r--r--   0 jaru      (1000) users      (100)     2227 2023-06-04 19:19:28.000000 hosgdSims-0.2.0/hosgdSims/HoSGDdefs.py
--rw-r--r--   0 jaru      (1000) users      (100)      283 2023-06-04 19:19:28.000000 hosgdSims-0.2.0/hosgdSims/HoSGDegAF.py
--rw-r--r--   0 jaru      (1000) users      (100)     9091 2023-06-04 19:19:28.000000 hosgdSims-0.2.0/hosgdSims/HoSGDlabAF.py
--rw-r--r--   0 jaru      (1000) users      (100)     6400 2023-06-04 19:19:28.000000 hosgdSims-0.2.0/hosgdSims/HoSGDlabAGD.py
--rw-r--r--   0 jaru      (1000) users      (100)     8333 2023-06-04 19:19:28.000000 hosgdSims-0.2.0/hosgdSims/HoSGDlabCG.py
--rw-r--r--   0 jaru      (1000) users      (100)     9502 2023-06-04 19:19:28.000000 hosgdSims-0.2.0/hosgdSims/HoSGDlabGD.py
--rw-r--r--   0 jaru      (1000) users      (100)    14694 2023-06-04 19:19:28.000000 hosgdSims-0.2.0/hosgdSims/HoSGDlabHL.py
--rw-r--r--   0 jaru      (1000) users      (100)     8058 2023-06-04 19:19:28.000000 hosgdSims-0.2.0/hosgdSims/HoSGDlabSGD.py
--rw-r--r--   0 jaru      (1000) users      (100)     7151 2023-06-04 19:19:28.000000 hosgdSims-0.2.0/hosgdSims/HoSGDlabSGDVariants.py
--rw-r--r--   0 jaru      (1000) users      (100)      150 2023-06-05 00:19:44.000000 hosgdSims-0.2.0/hosgdSims/__init__.py
-drwxr-xr-x   0 jaru      (1000) users      (100)        0 2023-06-05 00:27:11.783589 hosgdSims-0.2.0/hosgdSims.egg-info/
--rw-r--r--   0 jaru      (1000) users      (100)      924 2023-06-05 00:27:11.000000 hosgdSims-0.2.0/hosgdSims.egg-info/PKG-INFO
--rw-r--r--   0 jaru      (1000) users      (100)      466 2023-06-05 00:27:11.000000 hosgdSims-0.2.0/hosgdSims.egg-info/SOURCES.txt
--rw-r--r--   0 jaru      (1000) users      (100)        1 2023-06-05 00:27:11.000000 hosgdSims-0.2.0/hosgdSims.egg-info/dependency_links.txt
--rw-r--r--   0 jaru      (1000) users      (100)       45 2023-06-05 00:27:11.000000 hosgdSims-0.2.0/hosgdSims.egg-info/requires.txt
--rw-r--r--   0 jaru      (1000) users      (100)        1 2023-06-05 00:27:11.000000 hosgdSims-0.2.0/hosgdSims.egg-info/top_level.txt
--rw-r--r--   0 jaru      (1000) users      (100)       23 2023-06-04 21:09:24.000000 hosgdSims-0.2.0/requirements.txt
--rw-r--r--   0 jaru      (1000) users      (100)       38 2023-06-05 00:27:11.783589 hosgdSims-0.2.0/setup.cfg
--rw-r--r--   0 jaru      (1000) users      (100)      913 2023-06-05 00:19:27.000000 hosgdSims-0.2.0/setup.py
+drwxr-xr-x   0 jaru      (1000) users      (100)        0 2023-06-06 05:08:27.714021 hosgdSims-0.3.0/
+-rw-r--r--   0 jaru      (1000) users      (100)       35 2023-06-05 10:39:10.000000 hosgdSims-0.3.0/AUTHORS
+-rw-r--r--   0 jaru      (1000) users      (100)       11 2023-06-05 10:39:10.000000 hosgdSims-0.3.0/MANIFEST.in
+-rw-r--r--   0 jaru      (1000) users      (100)      924 2023-06-06 05:08:27.714021 hosgdSims-0.3.0/PKG-INFO
+-rw-r--r--   0 jaru      (1000) users      (100)      477 2023-06-05 10:39:10.000000 hosgdSims-0.3.0/README.md
+drwxr-xr-x   0 jaru      (1000) users      (100)        0 2023-06-06 05:08:27.714021 hosgdSims-0.3.0/hosgdSims/
+-rw-r--r--   0 jaru      (1000) users      (100)     2227 2023-06-05 10:39:10.000000 hosgdSims-0.3.0/hosgdSims/HoSGDdefs.py
+-rw-r--r--   0 jaru      (1000) users      (100)      283 2023-06-05 10:39:10.000000 hosgdSims-0.3.0/hosgdSims/HoSGDegAF.py
+-rw-r--r--   0 jaru      (1000) users      (100)     9091 2023-06-05 10:39:10.000000 hosgdSims-0.3.0/hosgdSims/HoSGDlabAF.py
+-rw-r--r--   0 jaru      (1000) users      (100)     6400 2023-06-05 10:39:10.000000 hosgdSims-0.3.0/hosgdSims/HoSGDlabAGD.py
+-rw-r--r--   0 jaru      (1000) users      (100)     9502 2023-06-05 10:39:10.000000 hosgdSims-0.3.0/hosgdSims/HoSGDlabGD.py
+-rw-r--r--   0 jaru      (1000) users      (100)    14694 2023-06-05 10:39:10.000000 hosgdSims-0.3.0/hosgdSims/HoSGDlabHL.py
+-rw-r--r--   0 jaru      (1000) users      (100)     8058 2023-06-05 10:39:10.000000 hosgdSims-0.3.0/hosgdSims/HoSGDlabSGD.py
+-rw-r--r--   0 jaru      (1000) users      (100)     7151 2023-06-05 10:39:10.000000 hosgdSims-0.3.0/hosgdSims/HoSGDlabSGDVariants.py
+-rw-r--r--   0 jaru      (1000) users      (100)      150 2023-06-06 05:01:25.000000 hosgdSims-0.3.0/hosgdSims/__init__.py
+drwxr-xr-x   0 jaru      (1000) users      (100)        0 2023-06-06 05:08:27.714021 hosgdSims-0.3.0/hosgdSims/__pycache__/
+-rw-r--r--   0 jaru      (1000) users      (100)     7961 2023-06-06 04:49:29.000000 hosgdSims-0.3.0/hosgdSims/__pycache__/HoSGDlabGD.cpython-39.pyc
+-rw-r--r--   0 jaru      (1000) users      (100)      346 2023-06-06 04:49:29.000000 hosgdSims-0.3.0/hosgdSims/__pycache__/__init__.cpython-39.pyc
+drwxr-xr-x   0 jaru      (1000) users      (100)        0 2023-06-06 05:08:27.714021 hosgdSims-0.3.0/hosgdSims.egg-info/
+-rw-r--r--   0 jaru      (1000) users      (100)      924 2023-06-06 05:08:27.000000 hosgdSims-0.3.0/hosgdSims.egg-info/PKG-INFO
+-rw-r--r--   0 jaru      (1000) users      (100)      536 2023-06-06 05:08:27.000000 hosgdSims-0.3.0/hosgdSims.egg-info/SOURCES.txt
+-rw-r--r--   0 jaru      (1000) users      (100)        1 2023-06-06 05:08:27.000000 hosgdSims-0.3.0/hosgdSims.egg-info/dependency_links.txt
+-rw-r--r--   0 jaru      (1000) users      (100)       45 2023-06-06 05:08:27.000000 hosgdSims-0.3.0/hosgdSims.egg-info/requires.txt
+-rw-r--r--   0 jaru      (1000) users      (100)        1 2023-06-06 05:08:27.000000 hosgdSims-0.3.0/hosgdSims.egg-info/top_level.txt
+-rw-r--r--   0 jaru      (1000) users      (100)       23 2023-06-05 10:39:10.000000 hosgdSims-0.3.0/requirements.txt
+-rw-r--r--   0 jaru      (1000) users      (100)       38 2023-06-06 05:08:27.714021 hosgdSims-0.3.0/setup.cfg
+-rw-r--r--   0 jaru      (1000) users      (100)      913 2023-06-06 05:01:11.000000 hosgdSims-0.3.0/setup.py
```

### Comparing `hosgdSims-0.2.0/PKG-INFO` & `hosgdSims-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hosgdSims
-Version: 0.2.0
+Version: 0.3.0
 Summary: Hands on SGD
 Home-page: https://gitlab.com/prodrig/hosgdsims
 Author: Paul Rodriguez
 Author-email: prodrig@pucp.edu.pe
 License: GNU General Public License v3 or later (GPLv3+)
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `hosgdSims-0.2.0/hosgdSims/HoSGDdefs.py` & `hosgdSims-0.3.0/hosgdSims/HoSGDdefs.py`

 * *Files identical despite different names*

### Comparing `hosgdSims-0.2.0/hosgdSims/HoSGDlabAF.py` & `hosgdSims-0.3.0/hosgdSims/HoSGDlabAF.py`

 * *Files identical despite different names*

### Comparing `hosgdSims-0.2.0/hosgdSims/HoSGDlabAGD.py` & `hosgdSims-0.3.0/hosgdSims/HoSGDlabAGD.py`

 * *Files identical despite different names*

### Comparing `hosgdSims-0.2.0/hosgdSims/HoSGDlabGD.py` & `hosgdSims-0.3.0/hosgdSims/HoSGDlabGD.py`

 * *Files identical despite different names*

### Comparing `hosgdSims-0.2.0/hosgdSims/HoSGDlabHL.py` & `hosgdSims-0.3.0/hosgdSims/HoSGDlabHL.py`

 * *Files identical despite different names*

### Comparing `hosgdSims-0.2.0/hosgdSims/HoSGDlabSGD.py` & `hosgdSims-0.3.0/hosgdSims/HoSGDlabSGD.py`

 * *Files identical despite different names*

### Comparing `hosgdSims-0.2.0/hosgdSims/HoSGDlabSGDVariants.py` & `hosgdSims-0.3.0/hosgdSims/HoSGDlabSGDVariants.py`

 * *Files identical despite different names*

### Comparing `hosgdSims-0.2.0/hosgdSims.egg-info/PKG-INFO` & `hosgdSims-0.3.0/hosgdSims.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hosgdSims
-Version: 0.2.0
+Version: 0.3.0
 Summary: Hands on SGD
 Home-page: https://gitlab.com/prodrig/hosgdsims
 Author: Paul Rodriguez
 Author-email: prodrig@pucp.edu.pe
 License: GNU General Public License v3 or later (GPLv3+)
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `hosgdSims-0.2.0/setup.py` & `hosgdSims-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="hosgdSims",
-    version="0.2.0",
+    version="0.3.0",
     description="Hands on SGD",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/prodrig/hosgdsims",
     author="Paul Rodriguez",
     author_email="prodrig@pucp.edu.pe",
     license="GNU General Public License v3 or later (GPLv3+)",
```

