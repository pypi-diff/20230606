# Comparing `tmp/krutils-0.20230607.13.tar.gz` & `tmp/krutils-0.20230607.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krutils-0.20230607.13.tar", last modified: Tue Jun  6 15:13:24 2023, max compression
+gzip compressed data, was "krutils-0.20230607.14.tar", last modified: Tue Jun  6 15:14:51 2023, max compression
```

## Comparing `krutils-0.20230607.13.tar` & `krutils-0.20230607.14.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 15:13:24.906435 krutils-0.20230607.13/
--rw-rw-rw-   0        0        0      524 2023-06-06 15:13:24.906435 krutils-0.20230607.13/PKG-INFO
--rw-rw-rw-   0        0        0      500 2023-05-25 04:35:41.000000 krutils-0.20230607.13/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 15:13:24.848536 krutils-0.20230607.13/krutils/
--rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230607.13/krutils/AppErr.py
--rw-rw-rw-   0        0        0     1741 2023-04-11 07:38:24.000000 krutils-0.20230607.13/krutils/CONST.py
--rw-rw-rw-   0        0        0      117 2023-06-06 09:13:37.000000 krutils-0.20230607.13/krutils/__init__.py
--rw-rw-rw-   0        0        0     5471 2023-04-11 07:45:04.000000 krutils-0.20230607.13/krutils/_dbmgr.py
--rw-rw-rw-   0        0        0     2721 2023-06-06 09:07:19.000000 krutils-0.20230607.13/krutils/futils.py
--rw-rw-rw-   0        0        0    12553 2023-05-22 05:02:22.000000 krutils-0.20230607.13/krutils/logger.py
--rw-rw-rw-   0        0        0      661 2023-05-24 07:15:43.000000 krutils-0.20230607.13/krutils/logger2.py
--rw-rw-rw-   0        0        0    18549 2023-06-06 14:41:02.000000 krutils-0.20230607.13/krutils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-06 15:13:24.903258 krutils-0.20230607.13/krutils.egg-info/
--rw-rw-rw-   0        0        0      524 2023-06-06 15:13:24.000000 krutils-0.20230607.13/krutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2023-06-06 15:13:24.000000 krutils-0.20230607.13/krutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 15:13:24.000000 krutils-0.20230607.13/krutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-06-06 15:13:24.000000 krutils-0.20230607.13/krutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-06 15:13:24.000000 krutils-0.20230607.13/krutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 15:13:24.906435 krutils-0.20230607.13/setup.cfg
--rw-rw-rw-   0        0        0      890 2023-06-06 15:13:23.000000 krutils-0.20230607.13/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-06 15:13:24.906435 krutils-0.20230607.13/test/
--rw-rw-rw-   0        0        0      349 2023-05-22 06:46:23.000000 krutils-0.20230607.13/test/test_futils.py
--rw-rw-rw-   0        0        0      347 2023-06-06 15:13:01.000000 krutils-0.20230607.13/test/test_logger.py
+drwxrwxrwx   0        0        0        0 2023-06-06 15:14:51.484974 krutils-0.20230607.14/
+-rw-rw-rw-   0        0        0      524 2023-06-06 15:14:51.479463 krutils-0.20230607.14/PKG-INFO
+-rw-rw-rw-   0        0        0      500 2023-05-25 04:35:41.000000 krutils-0.20230607.14/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 15:14:51.448070 krutils-0.20230607.14/krutils/
+-rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230607.14/krutils/AppErr.py
+-rw-rw-rw-   0        0        0     1741 2023-04-11 07:38:24.000000 krutils-0.20230607.14/krutils/CONST.py
+-rw-rw-rw-   0        0        0      117 2023-06-06 09:13:37.000000 krutils-0.20230607.14/krutils/__init__.py
+-rw-rw-rw-   0        0        0     5471 2023-04-11 07:45:04.000000 krutils-0.20230607.14/krutils/_dbmgr.py
+-rw-rw-rw-   0        0        0     2721 2023-06-06 09:07:19.000000 krutils-0.20230607.14/krutils/futils.py
+-rw-rw-rw-   0        0        0    12553 2023-05-22 05:02:22.000000 krutils-0.20230607.14/krutils/logger.py
+-rw-rw-rw-   0        0        0      661 2023-05-24 07:15:43.000000 krutils-0.20230607.14/krutils/logger2.py
+-rw-rw-rw-   0        0        0    18549 2023-06-06 14:41:02.000000 krutils-0.20230607.14/krutils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-06 15:14:51.479463 krutils-0.20230607.14/krutils.egg-info/
+-rw-rw-rw-   0        0        0      524 2023-06-06 15:14:51.000000 krutils-0.20230607.14/krutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-06-06 15:14:51.000000 krutils-0.20230607.14/krutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 15:14:51.000000 krutils-0.20230607.14/krutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-06-06 15:14:51.000000 krutils-0.20230607.14/krutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-06 15:14:51.000000 krutils-0.20230607.14/krutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 15:14:51.484974 krutils-0.20230607.14/setup.cfg
+-rw-rw-rw-   0        0        0      890 2023-06-06 15:14:50.000000 krutils-0.20230607.14/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 15:14:51.479463 krutils-0.20230607.14/test/
+-rw-rw-rw-   0        0        0      349 2023-05-22 06:46:23.000000 krutils-0.20230607.14/test/test_futils.py
+-rw-rw-rw-   0        0        0      347 2023-06-06 15:13:01.000000 krutils-0.20230607.14/test/test_logger.py
```

### Comparing `krutils-0.20230607.13/PKG-INFO` & `krutils-0.20230607.14/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krutils
-Version: 0.20230607.13
+Version: 0.20230607.14
 Summary: Some utils for me.
 Author: bonfireof
 Author-email: bonfireof@gmail.com
 Project-URL: Bug Tracker, https://github.com/bonfireof/krutils
 Project-URL: Documentation, https://github.com/bonfireof/krutils
 Project-URL: Source Code, https://github.com/bonfireof/krutils
 Classifier: Programming Language :: Python :: 3
```

### Comparing `krutils-0.20230607.13/krutils/CONST.py` & `krutils-0.20230607.14/krutils/CONST.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230607.13/krutils/_dbmgr.py` & `krutils-0.20230607.14/krutils/_dbmgr.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230607.13/krutils/futils.py` & `krutils-0.20230607.14/krutils/futils.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230607.13/krutils/logger.py` & `krutils-0.20230607.14/krutils/logger.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230607.13/krutils/logger2.py` & `krutils-0.20230607.14/krutils/logger2.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230607.13/krutils/utils.py` & `krutils-0.20230607.14/krutils/utils.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230607.13/krutils.egg-info/PKG-INFO` & `krutils-0.20230607.14/krutils.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krutils
-Version: 0.20230607.13
+Version: 0.20230607.14
 Summary: Some utils for me.
 Author: bonfireof
 Author-email: bonfireof@gmail.com
 Project-URL: Bug Tracker, https://github.com/bonfireof/krutils
 Project-URL: Documentation, https://github.com/bonfireof/krutils
 Project-URL: Source Code, https://github.com/bonfireof/krutils
 Classifier: Programming Language :: Python :: 3
```

### Comparing `krutils-0.20230607.13/setup.py` & `krutils-0.20230607.14/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="krutils",
-    version="0.20230607.0013",
+    version="0.20230607.0014",
     author="bonfireof",
     author_email="bonfireof@gmail.com",
     description="Some utils for me.",
     project_urls={
         "Bug Tracker": "https://github.com/bonfireof/krutils",
         "Documentation": "https://github.com/bonfireof/krutils",
         "Source Code": "https://github.com/bonfireof/krutils",
```

