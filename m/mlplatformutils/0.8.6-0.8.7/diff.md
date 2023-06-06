# Comparing `tmp/mlplatformutils-0.8.6.tar.gz` & `tmp/mlplatformutils-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mlplatformutils-0.8.6.tar", last modified: Tue Jun  6 01:33:37 2023, max compression
+gzip compressed data, was "dist\mlplatformutils-0.8.7.tar", last modified: Tue Jun  6 02:58:52 2023, max compression
```

## Comparing `mlplatformutils-0.8.6.tar` & `mlplatformutils-0.8.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 01:33:37.145680 mlplatformutils-0.8.6/
--rw-rw-rw-   0        0        0     3055 2023-06-06 01:33:37.145680 mlplatformutils-0.8.6/PKG-INFO
--rw-rw-rw-   0        0        0      420 2023-06-04 22:07:41.000000 mlplatformutils-0.8.6/README.rst
--rw-rw-rw-   0        0        0      115 2023-06-06 01:33:37.148685 mlplatformutils-0.8.6/setup.cfg
--rw-rw-rw-   0        0        0      761 2023-06-06 01:32:45.000000 mlplatformutils-0.8.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-06 01:33:36.987702 mlplatformutils-0.8.6/src/
-drwxrwxrwx   0        0        0        0 2023-06-06 01:33:37.012698 mlplatformutils-0.8.6/src/mlplatformutils/
--rw-rw-rw-   0        0        0        0 2023-06-04 21:52:02.000000 mlplatformutils-0.8.6/src/mlplatformutils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 01:33:37.143674 mlplatformutils-0.8.6/src/mlplatformutils/core/
--rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.8.6/src/mlplatformutils/core/__init__.py
--rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.8.6/src/mlplatformutils/core/app_insights_logger.py
--rw-rw-rw-   0        0        0     8410 2023-06-05 20:57:54.000000 mlplatformutils-0.8.6/src/mlplatformutils/core/lineagegraph.py
--rw-rw-rw-   0        0        0     3611 2023-06-05 06:21:00.000000 mlplatformutils-0.8.6/src/mlplatformutils/core/pandasutils.py
--rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.8.6/src/mlplatformutils/core/platformutils.py
--rw-rw-rw-   0        0        0     7879 2023-06-06 01:32:24.000000 mlplatformutils-0.8.6/src/mlplatformutils/core/sparkutils.py
--rw-rw-rw-   0        0        0       21 2023-06-06 01:32:39.000000 mlplatformutils-0.8.6/src/mlplatformutils/core/version.py
-drwxrwxrwx   0        0        0        0 2023-06-06 01:33:37.048742 mlplatformutils-0.8.6/src/mlplatformutils.egg-info/
--rw-rw-rw-   0        0        0     3055 2023-06-06 01:33:36.000000 mlplatformutils-0.8.6/src/mlplatformutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      558 2023-06-06 01:33:36.000000 mlplatformutils-0.8.6/src/mlplatformutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 01:33:36.000000 mlplatformutils-0.8.6/src/mlplatformutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-06-06 01:33:36.000000 mlplatformutils-0.8.6/src/mlplatformutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-06 01:33:36.000000 mlplatformutils-0.8.6/src/mlplatformutils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 02:58:52.691068 mlplatformutils-0.8.7/
+-rw-rw-rw-   0        0        0     3055 2023-06-06 02:58:52.691068 mlplatformutils-0.8.7/PKG-INFO
+-rw-rw-rw-   0        0        0      420 2023-06-04 22:07:41.000000 mlplatformutils-0.8.7/README.rst
+-rw-rw-rw-   0        0        0      115 2023-06-06 02:58:52.693067 mlplatformutils-0.8.7/setup.cfg
+-rw-rw-rw-   0        0        0      761 2023-06-06 02:58:32.000000 mlplatformutils-0.8.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 02:58:52.511353 mlplatformutils-0.8.7/src/
+drwxrwxrwx   0        0        0        0 2023-06-06 02:58:52.537355 mlplatformutils-0.8.7/src/mlplatformutils/
+-rw-rw-rw-   0        0        0        0 2023-06-04 21:52:02.000000 mlplatformutils-0.8.7/src/mlplatformutils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 02:58:52.688070 mlplatformutils-0.8.7/src/mlplatformutils/core/
+-rw-rw-rw-   0        0        0        0 2023-06-03 20:39:09.000000 mlplatformutils-0.8.7/src/mlplatformutils/core/__init__.py
+-rw-rw-rw-   0        0        0     5868 2023-06-03 20:42:19.000000 mlplatformutils-0.8.7/src/mlplatformutils/core/app_insights_logger.py
+-rw-rw-rw-   0        0        0     8410 2023-06-05 20:57:54.000000 mlplatformutils-0.8.7/src/mlplatformutils/core/lineagegraph.py
+-rw-rw-rw-   0        0        0     5802 2023-06-06 02:57:46.000000 mlplatformutils-0.8.7/src/mlplatformutils/core/pandasutils.py
+-rw-rw-rw-   0        0        0     3129 2023-06-04 21:06:24.000000 mlplatformutils-0.8.7/src/mlplatformutils/core/platformutils.py
+-rw-rw-rw-   0        0        0     7879 2023-06-06 01:32:24.000000 mlplatformutils-0.8.7/src/mlplatformutils/core/sparkutils.py
+-rw-rw-rw-   0        0        0       21 2023-06-06 02:58:26.000000 mlplatformutils-0.8.7/src/mlplatformutils/core/version.py
+drwxrwxrwx   0        0        0        0 2023-06-06 02:58:52.576963 mlplatformutils-0.8.7/src/mlplatformutils.egg-info/
+-rw-rw-rw-   0        0        0     3055 2023-06-06 02:58:52.000000 mlplatformutils-0.8.7/src/mlplatformutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      558 2023-06-06 02:58:52.000000 mlplatformutils-0.8.7/src/mlplatformutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 02:58:52.000000 mlplatformutils-0.8.7/src/mlplatformutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-06-06 02:58:52.000000 mlplatformutils-0.8.7/src/mlplatformutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-06 02:58:52.000000 mlplatformutils-0.8.7/src/mlplatformutils.egg-info/top_level.txt
```

### Comparing `mlplatformutils-0.8.6/PKG-INFO` & `mlplatformutils-0.8.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.8.6
+Version: 0.8.7
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Keywords: mlplatformutils
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlplatformutils-0.8.6/setup.py` & `mlplatformutils-0.8.7/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 else:
     long_description="#DESC"
 
 setup(
     name='mlplatformutils',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.8.6',
+    version='0.8.7',
     license='MIT',
     classifiers=[
         'Programming Language :: Python :: 3.8'
     ],
     author='Keshav Singh',
     author_email='keshav_singh@hotmail.com',
     packages=find_packages('src'),
```

### Comparing `mlplatformutils-0.8.6/src/mlplatformutils/core/app_insights_logger.py` & `mlplatformutils-0.8.7/src/mlplatformutils/core/app_insights_logger.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.8.6/src/mlplatformutils/core/lineagegraph.py` & `mlplatformutils-0.8.7/src/mlplatformutils/core/lineagegraph.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.8.6/src/mlplatformutils/core/platformutils.py` & `mlplatformutils-0.8.7/src/mlplatformutils/core/platformutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.8.6/src/mlplatformutils/core/sparkutils.py` & `mlplatformutils-0.8.7/src/mlplatformutils/core/sparkutils.py`

 * *Files identical despite different names*

### Comparing `mlplatformutils-0.8.6/src/mlplatformutils.egg-info/PKG-INFO` & `mlplatformutils-0.8.7/src/mlplatformutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlplatformutils
-Version: 0.8.6
+Version: 0.8.7
 Author: Keshav Singh
 Author-email: keshav_singh@hotmail.com
 License: MIT
 Keywords: mlplatformutils
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `mlplatformutils-0.8.6/src/mlplatformutils.egg-info/SOURCES.txt` & `mlplatformutils-0.8.7/src/mlplatformutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

