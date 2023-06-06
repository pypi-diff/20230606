# Comparing `tmp/pypasskeeper-1.0.0.tar.gz` & `tmp/pypasskeeper-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypasskeeper-1.0.0.tar", last modified: Tue Jun  6 12:58:47 2023, max compression
+gzip compressed data, was "pypasskeeper-1.0.1.tar", last modified: Tue Jun  6 13:00:52 2023, max compression
```

## Comparing `pypasskeeper-1.0.0.tar` & `pypasskeeper-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-06 12:58:47.681357 pypasskeeper-1.0.0/
--rw-rw-r--   0 praveen   (1000) praveen   (1000)     6339 2023-06-06 12:58:47.681357 pypasskeeper-1.0.0/PKG-INFO
--rwxrwxr-x   0 praveen   (1000) praveen   (1000)     6084 2023-06-03 04:38:59.000000 pypasskeeper-1.0.0/README.md
-drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-06 12:58:47.681357 pypasskeeper-1.0.0/pypasskeeper.egg-info/
--rw-rw-r--   0 praveen   (1000) praveen   (1000)     6339 2023-06-06 12:58:47.000000 pypasskeeper-1.0.0/pypasskeeper.egg-info/PKG-INFO
--rw-rw-r--   0 praveen   (1000) praveen   (1000)      236 2023-06-06 12:58:47.000000 pypasskeeper-1.0.0/pypasskeeper.egg-info/SOURCES.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)        1 2023-06-06 12:58:47.000000 pypasskeeper-1.0.0/pypasskeeper.egg-info/dependency_links.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)       65 2023-06-06 12:58:47.000000 pypasskeeper-1.0.0/pypasskeeper.egg-info/entry_points.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)        8 2023-06-06 12:58:47.000000 pypasskeeper-1.0.0/pypasskeeper.egg-info/requires.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)        1 2023-06-06 12:58:47.000000 pypasskeeper-1.0.0/pypasskeeper.egg-info/top_level.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)       38 2023-06-06 12:58:47.681357 pypasskeeper-1.0.0/setup.cfg
--rw-rw-r--   0 praveen   (1000) praveen   (1000)      688 2023-06-06 12:56:14.000000 pypasskeeper-1.0.0/setup.py
+drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-06 13:00:52.277341 pypasskeeper-1.0.1/
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)     6339 2023-06-06 13:00:52.277341 pypasskeeper-1.0.1/PKG-INFO
+-rwxrwxr-x   0 praveen   (1000) praveen   (1000)     6084 2023-06-03 04:38:59.000000 pypasskeeper-1.0.1/README.md
+drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-06 13:00:52.277341 pypasskeeper-1.0.1/pypasskeeper.egg-info/
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)     6339 2023-06-06 13:00:52.000000 pypasskeeper-1.0.1/pypasskeeper.egg-info/PKG-INFO
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)      236 2023-06-06 13:00:52.000000 pypasskeeper-1.0.1/pypasskeeper.egg-info/SOURCES.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)        1 2023-06-06 13:00:52.000000 pypasskeeper-1.0.1/pypasskeeper.egg-info/dependency_links.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)       65 2023-06-06 13:00:52.000000 pypasskeeper-1.0.1/pypasskeeper.egg-info/entry_points.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)        8 2023-06-06 13:00:52.000000 pypasskeeper-1.0.1/pypasskeeper.egg-info/requires.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)        1 2023-06-06 13:00:52.000000 pypasskeeper-1.0.1/pypasskeeper.egg-info/top_level.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)       38 2023-06-06 13:00:52.277341 pypasskeeper-1.0.1/setup.cfg
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)      688 2023-06-06 13:00:45.000000 pypasskeeper-1.0.1/setup.py
```

### Comparing `pypasskeeper-1.0.0/PKG-INFO` & `pypasskeeper-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypasskeeper
-Version: 1.0.0
+Version: 1.0.1
 Summary: A simple password manager
 Home-page: UNKNOWN
 Author: M S Praveen Kumar
 Author-email: mspraveenkumar77@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pypasskeeper-1.0.0/README.md` & `pypasskeeper-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pypasskeeper-1.0.0/pypasskeeper.egg-info/PKG-INFO` & `pypasskeeper-1.0.1/pypasskeeper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypasskeeper
-Version: 1.0.0
+Version: 1.0.1
 Summary: A simple password manager
 Home-page: UNKNOWN
 Author: M S Praveen Kumar
 Author-email: mspraveenkumar77@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pypasskeeper-1.0.0/setup.py` & `pypasskeeper-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     required = f.read().splitlines()
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="pypasskeeper",
-    version="1.0.0",
+    version="1.0.1",
     author="M S Praveen Kumar",
     author_email="mspraveenkumar77@gmail.com",
     description="A simple password manager",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=required,
```

