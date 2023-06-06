# Comparing `tmp/pypasskeeper-1.0.2.tar.gz` & `tmp/pypasskeeper-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypasskeeper-1.0.2.tar", last modified: Tue Jun  6 13:14:09 2023, max compression
+gzip compressed data, was "pypasskeeper-1.0.3.tar", last modified: Tue Jun  6 13:16:33 2023, max compression
```

## Comparing `pypasskeeper-1.0.2.tar` & `pypasskeeper-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-06 13:14:09.920628 pypasskeeper-1.0.2/
--rw-rw-r--   0 praveen   (1000) praveen   (1000)     6339 2023-06-06 13:14:09.920628 pypasskeeper-1.0.2/PKG-INFO
--rwxrwxr-x   0 praveen   (1000) praveen   (1000)     6084 2023-06-03 04:38:59.000000 pypasskeeper-1.0.2/README.md
-drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-06 13:14:09.920628 pypasskeeper-1.0.2/pypasskeeper.egg-info/
--rw-rw-r--   0 praveen   (1000) praveen   (1000)     6339 2023-06-06 13:14:09.000000 pypasskeeper-1.0.2/pypasskeeper.egg-info/PKG-INFO
--rw-rw-r--   0 praveen   (1000) praveen   (1000)      236 2023-06-06 13:14:09.000000 pypasskeeper-1.0.2/pypasskeeper.egg-info/SOURCES.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)        1 2023-06-06 13:14:09.000000 pypasskeeper-1.0.2/pypasskeeper.egg-info/dependency_links.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)       65 2023-06-06 13:14:09.000000 pypasskeeper-1.0.2/pypasskeeper.egg-info/entry_points.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)        8 2023-06-06 13:14:09.000000 pypasskeeper-1.0.2/pypasskeeper.egg-info/requires.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)        1 2023-06-06 13:14:09.000000 pypasskeeper-1.0.2/pypasskeeper.egg-info/top_level.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)       38 2023-06-06 13:14:09.920628 pypasskeeper-1.0.2/setup.cfg
--rw-rw-r--   0 praveen   (1000) praveen   (1000)      688 2023-06-06 13:14:07.000000 pypasskeeper-1.0.2/setup.py
+drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-06 13:16:33.412936 pypasskeeper-1.0.3/
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)     6339 2023-06-06 13:16:33.412936 pypasskeeper-1.0.3/PKG-INFO
+-rwxrwxr-x   0 praveen   (1000) praveen   (1000)     6084 2023-06-03 04:38:59.000000 pypasskeeper-1.0.3/README.md
+drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-06 13:16:33.412936 pypasskeeper-1.0.3/pypasskeeper.egg-info/
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)     6339 2023-06-06 13:16:33.000000 pypasskeeper-1.0.3/pypasskeeper.egg-info/PKG-INFO
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)      236 2023-06-06 13:16:33.000000 pypasskeeper-1.0.3/pypasskeeper.egg-info/SOURCES.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)        1 2023-06-06 13:16:33.000000 pypasskeeper-1.0.3/pypasskeeper.egg-info/dependency_links.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)       74 2023-06-06 13:16:33.000000 pypasskeeper-1.0.3/pypasskeeper.egg-info/entry_points.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)        8 2023-06-06 13:16:33.000000 pypasskeeper-1.0.3/pypasskeeper.egg-info/requires.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)        1 2023-06-06 13:16:33.000000 pypasskeeper-1.0.3/pypasskeeper.egg-info/top_level.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)       38 2023-06-06 13:16:33.412936 pypasskeeper-1.0.3/setup.cfg
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)      697 2023-06-06 13:16:29.000000 pypasskeeper-1.0.3/setup.py
```

### Comparing `pypasskeeper-1.0.2/PKG-INFO` & `pypasskeeper-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypasskeeper
-Version: 1.0.2
+Version: 1.0.3
 Summary: A simple password manager
 Home-page: UNKNOWN
 Author: M S Praveen Kumar
 Author-email: mspraveenkumar77@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pypasskeeper-1.0.2/README.md` & `pypasskeeper-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pypasskeeper-1.0.2/pypasskeeper.egg-info/PKG-INFO` & `pypasskeeper-1.0.3/pypasskeeper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypasskeeper
-Version: 1.0.2
+Version: 1.0.3
 Summary: A simple password manager
 Home-page: UNKNOWN
 Author: M S Praveen Kumar
 Author-email: mspraveenkumar77@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pypasskeeper-1.0.2/setup.py` & `pypasskeeper-1.0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,21 +5,21 @@
     required = f.read().splitlines()
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="pypasskeeper",
-    version="1.0.2",
+    version="1.0.3",
     author="M S Praveen Kumar",
     author_email="mspraveenkumar77@gmail.com",
     description="A simple password manager",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=required,
     entry_points={
         "console_scripts": [
-            "pypasskeeper = pypasskeeper.pypasskeeper:main",
+            "passwordmanager = passwordmanager.passwordmanager:main",
         ]
     },
 )
```

