# Comparing `tmp/krutils-0.20230607.136.tar.gz` & `tmp/krutils-0.20230607.140.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krutils-0.20230607.136.tar", last modified: Tue Jun  6 16:36:29 2023, max compression
+gzip compressed data, was "krutils-0.20230607.140.tar", last modified: Tue Jun  6 16:40:42 2023, max compression
```

## Comparing `krutils-0.20230607.136.tar` & `krutils-0.20230607.140.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 16:36:29.650610 krutils-0.20230607.136/
--rw-rw-rw-   0        0        0      525 2023-06-06 16:36:29.648168 krutils-0.20230607.136/PKG-INFO
--rw-rw-rw-   0        0        0      500 2023-05-25 04:35:41.000000 krutils-0.20230607.136/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 16:36:29.578963 krutils-0.20230607.136/krutils/
--rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230607.136/krutils/AppErr.py
--rw-rw-rw-   0        0        0     1741 2023-04-11 07:38:24.000000 krutils-0.20230607.136/krutils/CONST.py
--rw-rw-rw-   0        0        0       94 2023-06-06 15:37:21.000000 krutils-0.20230607.136/krutils/__init__.py
--rw-rw-rw-   0        0        0     5471 2023-04-11 07:45:04.000000 krutils-0.20230607.136/krutils/_dbmgr.py
--rw-rw-rw-   0        0        0     2721 2023-06-06 09:07:19.000000 krutils-0.20230607.136/krutils/futils.py
--rw-rw-rw-   0        0        0    12553 2023-06-06 15:58:45.000000 krutils-0.20230607.136/krutils/logger.py
--rw-rw-rw-   0        0        0      661 2023-05-24 07:15:43.000000 krutils-0.20230607.136/krutils/logger2.py
--rw-rw-rw-   0        0        0    18541 2023-06-06 16:33:34.000000 krutils-0.20230607.136/krutils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:36:29.627049 krutils-0.20230607.136/krutils.egg-info/
--rw-rw-rw-   0        0        0      525 2023-06-06 16:36:29.000000 krutils-0.20230607.136/krutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2023-06-06 16:36:29.000000 krutils-0.20230607.136/krutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 16:36:29.000000 krutils-0.20230607.136/krutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-06-06 16:36:29.000000 krutils-0.20230607.136/krutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-06 16:36:29.000000 krutils-0.20230607.136/krutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 16:36:29.650610 krutils-0.20230607.136/setup.cfg
--rw-rw-rw-   0        0        0      890 2023-06-06 16:36:28.000000 krutils-0.20230607.136/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:36:29.644483 krutils-0.20230607.136/test/
--rw-rw-rw-   0        0        0      349 2023-05-22 06:46:23.000000 krutils-0.20230607.136/test/test_futils.py
--rw-rw-rw-   0        0        0      367 2023-06-06 16:15:09.000000 krutils-0.20230607.136/test/test_logger.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:40:42.489992 krutils-0.20230607.140/
+-rw-rw-rw-   0        0        0      525 2023-06-06 16:40:42.483505 krutils-0.20230607.140/PKG-INFO
+-rw-rw-rw-   0        0        0      500 2023-05-25 04:35:41.000000 krutils-0.20230607.140/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 16:40:42.411170 krutils-0.20230607.140/krutils/
+-rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230607.140/krutils/AppErr.py
+-rw-rw-rw-   0        0        0     1741 2023-04-11 07:38:24.000000 krutils-0.20230607.140/krutils/CONST.py
+-rw-rw-rw-   0        0        0       94 2023-06-06 15:37:21.000000 krutils-0.20230607.140/krutils/__init__.py
+-rw-rw-rw-   0        0        0     5471 2023-04-11 07:45:04.000000 krutils-0.20230607.140/krutils/_dbmgr.py
+-rw-rw-rw-   0        0        0     2721 2023-06-06 09:07:19.000000 krutils-0.20230607.140/krutils/futils.py
+-rw-rw-rw-   0        0        0    12556 2023-06-06 16:39:50.000000 krutils-0.20230607.140/krutils/logger.py
+-rw-rw-rw-   0        0        0      661 2023-05-24 07:15:43.000000 krutils-0.20230607.140/krutils/logger2.py
+-rw-rw-rw-   0        0        0    18551 2023-06-06 16:40:24.000000 krutils-0.20230607.140/krutils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:40:42.444203 krutils-0.20230607.140/krutils.egg-info/
+-rw-rw-rw-   0        0        0      525 2023-06-06 16:40:41.000000 krutils-0.20230607.140/krutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-06-06 16:40:42.000000 krutils-0.20230607.140/krutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 16:40:41.000000 krutils-0.20230607.140/krutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-06-06 16:40:41.000000 krutils-0.20230607.140/krutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-06 16:40:42.000000 krutils-0.20230607.140/krutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 16:40:42.491010 krutils-0.20230607.140/setup.cfg
+-rw-rw-rw-   0        0        0      890 2023-06-06 16:40:40.000000 krutils-0.20230607.140/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:40:42.473962 krutils-0.20230607.140/test/
+-rw-rw-rw-   0        0        0      349 2023-05-22 06:46:23.000000 krutils-0.20230607.140/test/test_futils.py
+-rw-rw-rw-   0        0        0      367 2023-06-06 16:15:09.000000 krutils-0.20230607.140/test/test_logger.py
```

### Comparing `krutils-0.20230607.136/PKG-INFO` & `krutils-0.20230607.140/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krutils
-Version: 0.20230607.136
+Version: 0.20230607.140
 Summary: Some utils for me.
 Author: bonfireof
 Author-email: bonfireof@gmail.com
 Project-URL: Bug Tracker, https://github.com/bonfireof/krutils
 Project-URL: Documentation, https://github.com/bonfireof/krutils
 Project-URL: Source Code, https://github.com/bonfireof/krutils
 Classifier: Programming Language :: Python :: 3
```

### Comparing `krutils-0.20230607.136/krutils/CONST.py` & `krutils-0.20230607.140/krutils/CONST.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230607.136/krutils/_dbmgr.py` & `krutils-0.20230607.140/krutils/_dbmgr.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230607.136/krutils/futils.py` & `krutils-0.20230607.140/krutils/futils.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230607.136/krutils/logger.py` & `krutils-0.20230607.140/krutils/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -284,15 +284,15 @@
             pass
 
 
 
 ######################
 # logger 클래스 메인
 #   1. 설정파일을 찾아 적용한다. 없으면 기본값으로 적용한다.
-class logger(_logging):
+class getlogger(_logging):
     '''
     My favorite log format maker.
     [LEVEL] [TIME] [SOURCE] contents...
 
     sample>
         logger = krutils.logger(__file__)
```

### Comparing `krutils-0.20230607.136/krutils/logger2.py` & `krutils-0.20230607.140/krutils/logger2.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230607.136/krutils/utils.py` & `krutils-0.20230607.140/krutils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -693,15 +693,15 @@
 
     caller_path = ____file__
 
     if is_empty(caller_path) == True:
         caller_path = __file__
 
     from krutils import logger
-    return logger(caller_path)
+    return logger.getlogger(caller_path)
```

### Comparing `krutils-0.20230607.136/krutils.egg-info/PKG-INFO` & `krutils-0.20230607.140/krutils.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krutils
-Version: 0.20230607.136
+Version: 0.20230607.140
 Summary: Some utils for me.
 Author: bonfireof
 Author-email: bonfireof@gmail.com
 Project-URL: Bug Tracker, https://github.com/bonfireof/krutils
 Project-URL: Documentation, https://github.com/bonfireof/krutils
 Project-URL: Source Code, https://github.com/bonfireof/krutils
 Classifier: Programming Language :: Python :: 3
```

### Comparing `krutils-0.20230607.136/setup.py` & `krutils-0.20230607.140/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="krutils",
-    version="0.20230607.0136",
+    version="0.20230607.0140",
     author="bonfireof",
     author_email="bonfireof@gmail.com",
     description="Some utils for me.",
     project_urls={
         "Bug Tracker": "https://github.com/bonfireof/krutils",
         "Documentation": "https://github.com/bonfireof/krutils",
         "Source Code": "https://github.com/bonfireof/krutils",
```

