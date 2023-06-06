# Comparing `tmp/alltime_athletics_python-0.7.0.tar.gz` & `tmp/alltime_athletics_python-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alltime_athletics_python-0.7.0.tar", max compression
+gzip compressed data, was "alltime_athletics_python-0.8.0.tar", max compression
```

## Comparing `alltime_athletics_python-0.7.0.tar` & `alltime_athletics_python-0.8.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1074 2023-06-01 06:57:21.506681 alltime_athletics_python-0.7.0/LICENSE
--rw-r--r--   0        0        0      299 2023-06-01 06:57:21.522140 alltime_athletics_python-0.7.0/alltime_athletics_python/__init__.py
--rw-r--r--   0        0        0     3205 2023-06-01 06:58:25.637564 alltime_athletics_python-0.7.0/alltime_athletics_python/get_content.py
--rw-r--r--   0        0        0     1915 2023-06-01 06:58:25.645679 alltime_athletics_python-0.7.0/alltime_athletics_python/get_content_urls.py
--rw-r--r--   0        0        0     3602 2023-06-05 09:07:54.851615 alltime_athletics_python-0.7.0/alltime_athletics_python/io.py
--rw-r--r--   0        0        0    11784 2023-06-05 09:05:25.415701 alltime_athletics_python-0.7.0/alltime_athletics_python/pipes.py
--rw-r--r--   0        0        0        0 2023-06-01 06:57:21.524099 alltime_athletics_python-0.7.0/alltime_athletics_python/utils/__init__.py
--rw-r--r--   0        0        0      600 2023-06-01 06:57:21.523437 alltime_athletics_python-0.7.0/alltime_athletics_python/utils/config.py
--rw-r--r--   0        0        0      736 2023-06-01 06:57:21.525381 alltime_athletics_python-0.7.0/alltime_athletics_python/utils/logger.py
--rw-r--r--   0        0        0      924 2023-06-05 09:08:51.365973 alltime_athletics_python-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      516 1970-01-01 00:00:00.000000 alltime_athletics_python-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-01 06:57:21.506681 alltime_athletics_python-0.8.0/LICENSE
+-rw-r--r--   0        0        0      299 2023-06-01 06:57:21.522140 alltime_athletics_python-0.8.0/alltime_athletics_python/__init__.py
+-rw-r--r--   0        0        0     3205 2023-06-01 06:58:25.637564 alltime_athletics_python-0.8.0/alltime_athletics_python/get_content.py
+-rw-r--r--   0        0        0     1915 2023-06-01 06:58:25.645679 alltime_athletics_python-0.8.0/alltime_athletics_python/get_content_urls.py
+-rw-r--r--   0        0        0     3602 2023-06-05 09:07:54.851615 alltime_athletics_python-0.8.0/alltime_athletics_python/io.py
+-rw-r--r--   0        0        0    11784 2023-06-05 09:05:25.415701 alltime_athletics_python-0.8.0/alltime_athletics_python/pipes.py
+-rw-r--r--   0        0        0        0 2023-06-01 06:57:21.524099 alltime_athletics_python-0.8.0/alltime_athletics_python/utils/__init__.py
+-rw-r--r--   0        0        0      600 2023-06-01 06:57:21.523437 alltime_athletics_python-0.8.0/alltime_athletics_python/utils/config.py
+-rw-r--r--   0        0        0      736 2023-06-01 06:57:21.525381 alltime_athletics_python-0.8.0/alltime_athletics_python/utils/logger.py
+-rw-r--r--   0        0        0     1077 2023-06-05 09:11:59.949022 alltime_athletics_python-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      668 1970-01-01 00:00:00.000000 alltime_athletics_python-0.8.0/PKG-INFO
```

### Comparing `alltime_athletics_python-0.7.0/LICENSE` & `alltime_athletics_python-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alltime_athletics_python-0.7.0/alltime_athletics_python/get_content.py` & `alltime_athletics_python-0.8.0/alltime_athletics_python/get_content.py`

 * *Files identical despite different names*

### Comparing `alltime_athletics_python-0.7.0/alltime_athletics_python/get_content_urls.py` & `alltime_athletics_python-0.8.0/alltime_athletics_python/get_content_urls.py`

 * *Files identical despite different names*

### Comparing `alltime_athletics_python-0.7.0/alltime_athletics_python/io.py` & `alltime_athletics_python-0.8.0/alltime_athletics_python/io.py`

 * *Files identical despite different names*

### Comparing `alltime_athletics_python-0.7.0/alltime_athletics_python/pipes.py` & `alltime_athletics_python-0.8.0/alltime_athletics_python/pipes.py`

 * *Files identical despite different names*

### Comparing `alltime_athletics_python-0.7.0/alltime_athletics_python/utils/config.py` & `alltime_athletics_python-0.8.0/alltime_athletics_python/utils/config.py`

 * *Files identical despite different names*

### Comparing `alltime_athletics_python-0.7.0/alltime_athletics_python/utils/logger.py` & `alltime_athletics_python-0.8.0/alltime_athletics_python/utils/logger.py`

 * *Files identical despite different names*

### Comparing `alltime_athletics_python-0.7.0/pyproject.toml` & `alltime_athletics_python-0.8.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [tool.poetry]
 name = "alltime_athletics_python"
-version = "0.7.0"
-description = ""
+version = "0.8.0"
+description = "Scrapes and post-processes data from Alltime Athletics (website by Peter Larsson)"
+homepage= "https://github.com/thomascamminady/alltime_athletics_python"
 authors = ["Thomas Camminady <0milieux_member@icloud.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pandas = "^2.0.2"
 lxml = "^4.9.2"
 html5lib = "^1.1"
```

### Comparing `alltime_athletics_python-0.7.0/PKG-INFO` & `alltime_athletics_python-0.8.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: alltime-athletics-python
-Version: 0.7.0
-Summary: 
+Version: 0.8.0
+Summary: Scrapes and post-processes data from Alltime Athletics (website by Peter Larsson)
+Home-page: https://github.com/thomascamminady/alltime_athletics_python
 Author: Thomas Camminady
 Author-email: 0milieux_member@icloud.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: html5lib (>=1.1,<2.0)
```

