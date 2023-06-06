# Comparing `tmp/securepassmanager-1.0.0.tar.gz` & `tmp/securepassmanager-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "securepassmanager-1.0.0.tar", last modified: Tue Jun  6 13:37:30 2023, max compression
+gzip compressed data, was "securepassmanager-1.0.1.tar", last modified: Tue Jun  6 13:42:02 2023, max compression
```

## Comparing `securepassmanager-1.0.0.tar` & `securepassmanager-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-06 13:37:30.880706 securepassmanager-1.0.0/
--rw-rw-r--   0 praveen   (1000) praveen   (1000)     6344 2023-06-06 13:37:30.880706 securepassmanager-1.0.0/PKG-INFO
--rwxrwxr-x   0 praveen   (1000) praveen   (1000)     6084 2023-06-03 04:38:59.000000 securepassmanager-1.0.0/README.md
-drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-06 13:37:30.880706 securepassmanager-1.0.0/securepassmanager.egg-info/
--rw-rw-r--   0 praveen   (1000) praveen   (1000)     6344 2023-06-06 13:37:30.000000 securepassmanager-1.0.0/securepassmanager.egg-info/PKG-INFO
--rw-rw-r--   0 praveen   (1000) praveen   (1000)      266 2023-06-06 13:37:30.000000 securepassmanager-1.0.0/securepassmanager.egg-info/SOURCES.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)        1 2023-06-06 13:37:30.000000 securepassmanager-1.0.0/securepassmanager.egg-info/dependency_links.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)       74 2023-06-06 13:37:30.000000 securepassmanager-1.0.0/securepassmanager.egg-info/entry_points.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)        8 2023-06-06 13:37:30.000000 securepassmanager-1.0.0/securepassmanager.egg-info/requires.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)        1 2023-06-06 13:37:30.000000 securepassmanager-1.0.0/securepassmanager.egg-info/top_level.txt
--rw-rw-r--   0 praveen   (1000) praveen   (1000)       38 2023-06-06 13:37:30.880706 securepassmanager-1.0.0/setup.cfg
--rw-rw-r--   0 praveen   (1000) praveen   (1000)      702 2023-06-06 13:37:29.000000 securepassmanager-1.0.0/setup.py
+drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-06 13:42:02.066232 securepassmanager-1.0.1/
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)     6344 2023-06-06 13:42:02.066232 securepassmanager-1.0.1/PKG-INFO
+-rwxrwxr-x   0 praveen   (1000) praveen   (1000)     6084 2023-06-03 04:38:59.000000 securepassmanager-1.0.1/README.md
+drwxrwxr-x   0 praveen   (1000) praveen   (1000)        0 2023-06-06 13:42:02.066232 securepassmanager-1.0.1/securepassmanager.egg-info/
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)     6344 2023-06-06 13:42:02.000000 securepassmanager-1.0.1/securepassmanager.egg-info/PKG-INFO
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)      266 2023-06-06 13:42:02.000000 securepassmanager-1.0.1/securepassmanager.egg-info/SOURCES.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)        1 2023-06-06 13:42:02.000000 securepassmanager-1.0.1/securepassmanager.egg-info/dependency_links.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)       78 2023-06-06 13:42:02.000000 securepassmanager-1.0.1/securepassmanager.egg-info/entry_points.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)        8 2023-06-06 13:42:02.000000 securepassmanager-1.0.1/securepassmanager.egg-info/requires.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)        1 2023-06-06 13:42:02.000000 securepassmanager-1.0.1/securepassmanager.egg-info/top_level.txt
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)       38 2023-06-06 13:42:02.066232 securepassmanager-1.0.1/setup.cfg
+-rw-rw-r--   0 praveen   (1000) praveen   (1000)      706 2023-06-06 13:41:25.000000 securepassmanager-1.0.1/setup.py
```

### Comparing `securepassmanager-1.0.0/PKG-INFO` & `securepassmanager-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: securepassmanager
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

### Comparing `securepassmanager-1.0.0/README.md` & `securepassmanager-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `securepassmanager-1.0.0/securepassmanager.egg-info/PKG-INFO` & `securepassmanager-1.0.1/securepassmanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: securepassmanager
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

### Comparing `securepassmanager-1.0.0/setup.py` & `securepassmanager-1.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,21 +5,21 @@
     required = f.read().splitlines()
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="securepassmanager",
-    version="1.0.0",
+    version="1.0.1",
     author="M S Praveen Kumar",
     author_email="mspraveenkumar77@gmail.com",
     description="A simple password manager",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=required,
     entry_points={
         "console_scripts": [
-            "passwordmanager = passwordmanager.passwordmanager:main",
+            "securepassmanager = passwordmanager.securepassmanager:main",
         ]
     },
 )
```

