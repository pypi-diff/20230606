# Comparing `tmp/mootdx-0.9.8.tar.gz` & `tmp/mootdx-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mootdx-0.9.8.tar", last modified: Mon Nov 28 12:33:58 2022, max compression
+gzip compressed data, was "mootdx-0.9.9.tar", last modified: Mon Nov 28 15:33:26 2022, max compression
```

## Comparing `mootdx-0.9.8.tar` & `mootdx-0.9.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 bopo       (501) staff       (20)        0 2022-11-28 12:33:58.196891 mootdx-0.9.8/
--rwxr-xr-x   0 bopo       (501) staff       (20)       86 2022-08-03 11:50:47.000000 mootdx-0.9.8/AUTHORS.rst
--rwxr-xr-x   0 bopo       (501) staff       (20)     1023 2022-08-03 11:50:47.000000 mootdx-0.9.8/HISTORY.rst
--rwxr-xr-x   0 bopo       (501) staff       (20)     1065 2022-08-03 11:50:47.000000 mootdx-0.9.8/LICENSE
--rwxr-xr-x   0 bopo       (501) staff       (20)      335 2022-08-03 11:50:47.000000 mootdx-0.9.8/MANIFEST.in
--rw-r--r--   0 bopo       (501) staff       (20)     3944 2022-11-28 12:33:58.196956 mootdx-0.9.8/PKG-INFO
--rwxr-xr-x   0 bopo       (501) staff       (20)     3248 2022-11-24 04:26:33.000000 mootdx-0.9.8/README.rst
-drwxr-xr-x   0 bopo       (501) staff       (20)        0 2022-11-28 12:33:58.194440 mootdx-0.9.8/mootdx/
--rw-r--r--   0 bopo       (501) staff       (20)      269 2022-11-28 12:33:55.000000 mootdx-0.9.8/mootdx/__init__.py
--rw-r--r--   0 bopo       (501) staff       (20)     7361 2022-11-24 04:26:33.000000 mootdx-0.9.8/mootdx/__main__.py
--rw-r--r--   0 bopo       (501) staff       (20)     3060 2022-11-28 11:24:25.000000 mootdx-0.9.8/mootdx/affair.py
--rw-r--r--   0 bopo       (501) staff       (20)     2213 2022-11-24 04:26:33.000000 mootdx-0.9.8/mootdx/config.py
--rw-r--r--   0 bopo       (501) staff       (20)     3951 2022-11-28 12:20:32.000000 mootdx-0.9.8/mootdx/consts.py
-drwxr-xr-x   0 bopo       (501) staff       (20)        0 2022-11-28 12:33:58.195626 mootdx-0.9.8/mootdx/contrib/
--rw-r--r--   0 bopo       (501) staff       (20)       90 2022-08-03 11:50:47.000000 mootdx-0.9.8/mootdx/contrib/__init__.py
--rw-r--r--   0 bopo       (501) staff       (20)     2441 2022-11-12 16:35:15.000000 mootdx-0.9.8/mootdx/contrib/adjust.py
--rw-r--r--   0 bopo       (501) staff       (20)     4616 2022-11-12 16:35:15.000000 mootdx-0.9.8/mootdx/contrib/compat.py
--rw-r--r--   0 bopo       (501) staff       (20)     7291 2022-11-24 04:26:33.000000 mootdx-0.9.8/mootdx/contrib/fuquan.py
--rw-r--r--   0 bopo       (501) staff       (20)      752 2022-11-24 04:26:33.000000 mootdx-0.9.8/mootdx/exceptions.py
-drwxr-xr-x   0 bopo       (501) staff       (20)        0 2022-11-28 12:33:58.196059 mootdx-0.9.8/mootdx/financial/
--rw-r--r--   0 bopo       (501) staff       (20)        0 2022-08-03 11:50:47.000000 mootdx-0.9.8/mootdx/financial/__init__.py
--rw-r--r--   0 bopo       (501) staff       (20)     2727 2022-11-24 04:26:33.000000 mootdx-0.9.8/mootdx/financial/base.py
--rw-r--r--   0 bopo       (501) staff       (20)    17603 2022-11-12 16:35:15.000000 mootdx-0.9.8/mootdx/financial/columns.py
--rw-r--r--   0 bopo       (501) staff       (20)     6589 2022-11-24 04:26:33.000000 mootdx-0.9.8/mootdx/financial/financial.py
--rw-r--r--   0 bopo       (501) staff       (20)      294 2022-11-28 12:24:09.000000 mootdx-0.9.8/mootdx/logger.py
--rw-r--r--   0 bopo       (501) staff       (20)     1738 2022-11-24 04:26:33.000000 mootdx-0.9.8/mootdx/parse.py
--rw-r--r--   0 bopo       (501) staff       (20)    25631 2022-11-28 12:25:01.000000 mootdx-0.9.8/mootdx/quotes.py
--rw-r--r--   0 bopo       (501) staff       (20)     5585 2022-11-24 04:26:33.000000 mootdx-0.9.8/mootdx/reader.py
--rw-r--r--   0 bopo       (501) staff       (20)     5308 2022-11-28 12:26:30.000000 mootdx-0.9.8/mootdx/server.py
-drwxr-xr-x   0 bopo       (501) staff       (20)        0 2022-11-28 12:33:58.196470 mootdx-0.9.8/mootdx/tools/
--rw-r--r--   0 bopo       (501) staff       (20)       60 2022-08-03 11:50:47.000000 mootdx-0.9.8/mootdx/tools/__init__.py
--rw-r--r--   0 bopo       (501) staff       (20)     6350 2022-11-24 04:26:33.000000 mootdx-0.9.8/mootdx/tools/customize.py
--rw-r--r--   0 bopo       (501) staff       (20)     3986 2022-11-12 16:35:15.000000 mootdx-0.9.8/mootdx/tools/reversion.py
--rw-r--r--   0 bopo       (501) staff       (20)     1736 2022-11-12 16:35:15.000000 mootdx-0.9.8/mootdx/tools/tdx2csv.py
-drwxr-xr-x   0 bopo       (501) staff       (20)        0 2022-11-28 12:33:58.196772 mootdx-0.9.8/mootdx/utils/
--rw-r--r--   0 bopo       (501) staff       (20)     6836 2022-11-24 04:26:33.000000 mootdx-0.9.8/mootdx/utils/__init__.py
--rw-r--r--   0 bopo       (501) staff       (20)     5343 2022-11-12 16:35:15.000000 mootdx-0.9.8/mootdx/utils/adjust.py
--rw-r--r--   0 bopo       (501) staff       (20)    14561 2022-11-24 04:26:33.000000 mootdx-0.9.8/mootdx/utils/holiday.py
-drwxr-xr-x   0 bopo       (501) staff       (20)        0 2022-11-28 12:33:58.195184 mootdx-0.9.8/mootdx.egg-info/
--rw-r--r--   0 bopo       (501) staff       (20)     3944 2022-11-28 12:33:58.000000 mootdx-0.9.8/mootdx.egg-info/PKG-INFO
--rw-r--r--   0 bopo       (501) staff       (20)      897 2022-11-28 12:33:58.000000 mootdx-0.9.8/mootdx.egg-info/SOURCES.txt
--rw-r--r--   0 bopo       (501) staff       (20)        1 2022-11-28 12:33:58.000000 mootdx-0.9.8/mootdx.egg-info/dependency_links.txt
--rw-r--r--   0 bopo       (501) staff       (20)       49 2022-11-28 12:33:58.000000 mootdx-0.9.8/mootdx.egg-info/entry_points.txt
--rw-r--r--   0 bopo       (501) staff       (20)        1 2022-11-28 12:33:58.000000 mootdx-0.9.8/mootdx.egg-info/not-zip-safe
--rw-r--r--   0 bopo       (501) staff       (20)       65 2022-11-28 12:33:58.000000 mootdx-0.9.8/mootdx.egg-info/requires.txt
--rw-r--r--   0 bopo       (501) staff       (20)        7 2022-11-28 12:33:58.000000 mootdx-0.9.8/mootdx.egg-info/top_level.txt
--rw-r--r--   0 bopo       (501) staff       (20)      540 2022-11-28 12:33:55.000000 mootdx-0.9.8/pyproject.toml
--rwxr-xr-x   0 bopo       (501) staff       (20)       65 2022-11-28 11:24:25.000000 mootdx-0.9.8/requirements.txt
--rwxr-xr-x   0 bopo       (501) staff       (20)      758 2022-11-28 12:33:58.197231 mootdx-0.9.8/setup.cfg
--rwxr-xr-x   0 bopo       (501) staff       (20)     1732 2022-11-28 12:33:55.000000 mootdx-0.9.8/setup.py
+drwxr-xr-x   0 bopo       (501) staff       (20)        0 2022-11-28 15:33:26.577481 mootdx-0.9.9/
+-rwxr-xr-x   0 bopo       (501) staff       (20)       86 2022-08-03 11:50:47.000000 mootdx-0.9.9/AUTHORS.rst
+-rwxr-xr-x   0 bopo       (501) staff       (20)     1023 2022-08-03 11:50:47.000000 mootdx-0.9.9/HISTORY.rst
+-rwxr-xr-x   0 bopo       (501) staff       (20)     1065 2022-08-03 11:50:47.000000 mootdx-0.9.9/LICENSE
+-rwxr-xr-x   0 bopo       (501) staff       (20)      335 2022-08-03 11:50:47.000000 mootdx-0.9.9/MANIFEST.in
+-rw-r--r--   0 bopo       (501) staff       (20)     4046 2022-11-28 15:33:26.577553 mootdx-0.9.9/PKG-INFO
+-rwxr-xr-x   0 bopo       (501) staff       (20)     3248 2022-11-24 04:26:33.000000 mootdx-0.9.9/README.rst
+drwxr-xr-x   0 bopo       (501) staff       (20)        0 2022-11-28 15:33:26.575099 mootdx-0.9.9/mootdx/
+-rw-r--r--   0 bopo       (501) staff       (20)      269 2022-11-28 15:33:22.000000 mootdx-0.9.9/mootdx/__init__.py
+-rw-r--r--   0 bopo       (501) staff       (20)     7361 2022-11-28 15:30:48.000000 mootdx-0.9.9/mootdx/__main__.py
+-rw-r--r--   0 bopo       (501) staff       (20)     3060 2022-11-28 12:42:41.000000 mootdx-0.9.9/mootdx/affair.py
+-rw-r--r--   0 bopo       (501) staff       (20)     2213 2022-11-24 04:26:33.000000 mootdx-0.9.9/mootdx/config.py
+-rw-r--r--   0 bopo       (501) staff       (20)     3951 2022-11-28 12:42:41.000000 mootdx-0.9.9/mootdx/consts.py
+drwxr-xr-x   0 bopo       (501) staff       (20)        0 2022-11-28 15:33:26.576240 mootdx-0.9.9/mootdx/contrib/
+-rw-r--r--   0 bopo       (501) staff       (20)       90 2022-08-03 11:50:47.000000 mootdx-0.9.9/mootdx/contrib/__init__.py
+-rw-r--r--   0 bopo       (501) staff       (20)     2441 2022-11-12 16:35:15.000000 mootdx-0.9.9/mootdx/contrib/adjust.py
+-rw-r--r--   0 bopo       (501) staff       (20)     4616 2022-11-12 16:35:15.000000 mootdx-0.9.9/mootdx/contrib/compat.py
+-rw-r--r--   0 bopo       (501) staff       (20)     7291 2022-11-24 04:26:33.000000 mootdx-0.9.9/mootdx/contrib/fuquan.py
+-rw-r--r--   0 bopo       (501) staff       (20)      752 2022-11-24 04:26:33.000000 mootdx-0.9.9/mootdx/exceptions.py
+drwxr-xr-x   0 bopo       (501) staff       (20)        0 2022-11-28 15:33:26.576662 mootdx-0.9.9/mootdx/financial/
+-rw-r--r--   0 bopo       (501) staff       (20)        0 2022-08-03 11:50:47.000000 mootdx-0.9.9/mootdx/financial/__init__.py
+-rw-r--r--   0 bopo       (501) staff       (20)     2727 2022-11-24 04:26:33.000000 mootdx-0.9.9/mootdx/financial/base.py
+-rw-r--r--   0 bopo       (501) staff       (20)    17603 2022-11-12 16:35:15.000000 mootdx-0.9.9/mootdx/financial/columns.py
+-rw-r--r--   0 bopo       (501) staff       (20)     6589 2022-11-24 04:26:33.000000 mootdx-0.9.9/mootdx/financial/financial.py
+-rw-r--r--   0 bopo       (501) staff       (20)      294 2022-11-28 12:24:09.000000 mootdx-0.9.9/mootdx/logger.py
+-rw-r--r--   0 bopo       (501) staff       (20)     1738 2022-11-24 04:26:33.000000 mootdx-0.9.9/mootdx/parse.py
+-rw-r--r--   0 bopo       (501) staff       (20)    25631 2022-11-28 12:42:41.000000 mootdx-0.9.9/mootdx/quotes.py
+-rw-r--r--   0 bopo       (501) staff       (20)     5585 2022-11-24 04:26:33.000000 mootdx-0.9.9/mootdx/reader.py
+-rw-r--r--   0 bopo       (501) staff       (20)     5308 2022-11-28 12:42:41.000000 mootdx-0.9.9/mootdx/server.py
+drwxr-xr-x   0 bopo       (501) staff       (20)        0 2022-11-28 15:33:26.577075 mootdx-0.9.9/mootdx/tools/
+-rw-r--r--   0 bopo       (501) staff       (20)       60 2022-08-03 11:50:47.000000 mootdx-0.9.9/mootdx/tools/__init__.py
+-rw-r--r--   0 bopo       (501) staff       (20)     6350 2022-11-24 04:26:33.000000 mootdx-0.9.9/mootdx/tools/customize.py
+-rw-r--r--   0 bopo       (501) staff       (20)     3986 2022-11-12 16:35:15.000000 mootdx-0.9.9/mootdx/tools/reversion.py
+-rw-r--r--   0 bopo       (501) staff       (20)     1736 2022-11-12 16:35:15.000000 mootdx-0.9.9/mootdx/tools/tdx2csv.py
+drwxr-xr-x   0 bopo       (501) staff       (20)        0 2022-11-28 15:33:26.577386 mootdx-0.9.9/mootdx/utils/
+-rw-r--r--   0 bopo       (501) staff       (20)     6836 2022-11-24 04:26:33.000000 mootdx-0.9.9/mootdx/utils/__init__.py
+-rw-r--r--   0 bopo       (501) staff       (20)     5343 2022-11-12 16:35:15.000000 mootdx-0.9.9/mootdx/utils/adjust.py
+-rw-r--r--   0 bopo       (501) staff       (20)    14561 2022-11-24 04:26:33.000000 mootdx-0.9.9/mootdx/utils/holiday.py
+drwxr-xr-x   0 bopo       (501) staff       (20)        0 2022-11-28 15:33:26.575819 mootdx-0.9.9/mootdx.egg-info/
+-rw-r--r--   0 bopo       (501) staff       (20)     4046 2022-11-28 15:33:26.000000 mootdx-0.9.9/mootdx.egg-info/PKG-INFO
+-rw-r--r--   0 bopo       (501) staff       (20)      897 2022-11-28 15:33:26.000000 mootdx-0.9.9/mootdx.egg-info/SOURCES.txt
+-rw-r--r--   0 bopo       (501) staff       (20)        1 2022-11-28 15:33:26.000000 mootdx-0.9.9/mootdx.egg-info/dependency_links.txt
+-rw-r--r--   0 bopo       (501) staff       (20)       49 2022-11-28 15:33:26.000000 mootdx-0.9.9/mootdx.egg-info/entry_points.txt
+-rw-r--r--   0 bopo       (501) staff       (20)        1 2022-11-28 15:33:26.000000 mootdx-0.9.9/mootdx.egg-info/not-zip-safe
+-rw-r--r--   0 bopo       (501) staff       (20)       65 2022-11-28 15:33:26.000000 mootdx-0.9.9/mootdx.egg-info/requires.txt
+-rw-r--r--   0 bopo       (501) staff       (20)        7 2022-11-28 15:33:26.000000 mootdx-0.9.9/mootdx.egg-info/top_level.txt
+-rw-r--r--   0 bopo       (501) staff       (20)      541 2022-11-28 15:33:22.000000 mootdx-0.9.9/pyproject.toml
+-rwxr-xr-x   0 bopo       (501) staff       (20)       65 2022-11-28 12:42:41.000000 mootdx-0.9.9/requirements.txt
+-rwxr-xr-x   0 bopo       (501) staff       (20)      758 2022-11-28 15:33:26.577866 mootdx-0.9.9/setup.cfg
+-rwxr-xr-x   0 bopo       (501) staff       (20)     1832 2022-11-28 15:33:22.000000 mootdx-0.9.9/setup.py
```

### Comparing `mootdx-0.9.8/HISTORY.rst` & `mootdx-0.9.9/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `mootdx-0.9.8/LICENSE` & `mootdx-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mootdx-0.9.8/PKG-INFO` & `mootdx-0.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mootdx
-Version: 0.9.8
+Version: 0.9.9
 Summary: 通达信数据读取接口.
 Home-page: https://github.com/mootdx/mootdx
 Author: bopo.wang
 Author-email: ibopo@126.com
 License: MIT license
 Keywords: mootdx
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -12,14 +12,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 通达信数据读取接口
 ==================
 
 .. image:: https://badge.fury.io/py/mootdx.svg
```

### Comparing `mootdx-0.9.8/README.rst` & `mootdx-0.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `mootdx-0.9.8/mootdx/__main__.py` & `mootdx-0.9.9/mootdx/__main__.py`

 * *Files identical despite different names*

### Comparing `mootdx-0.9.8/mootdx/affair.py` & `mootdx-0.9.9/mootdx/affair.py`

 * *Files identical despite different names*

### Comparing `mootdx-0.9.8/mootdx/config.py` & `mootdx-0.9.9/mootdx/config.py`

 * *Files identical despite different names*

### Comparing `mootdx-0.9.8/mootdx/consts.py` & `mootdx-0.9.9/mootdx/consts.py`

 * *Files identical despite different names*

### Comparing `mootdx-0.9.8/mootdx/contrib/adjust.py` & `mootdx-0.9.9/mootdx/contrib/adjust.py`

 * *Files identical despite different names*

### Comparing `mootdx-0.9.8/mootdx/contrib/compat.py` & `mootdx-0.9.9/mootdx/contrib/compat.py`

 * *Files identical despite different names*

### Comparing `mootdx-0.9.8/mootdx/contrib/fuquan.py` & `mootdx-0.9.9/mootdx/contrib/fuquan.py`

 * *Files identical despite different names*

### Comparing `mootdx-0.9.8/mootdx/exceptions.py` & `mootdx-0.9.9/mootdx/exceptions.py`

 * *Files identical despite different names*

### Comparing `mootdx-0.9.8/mootdx/financial/base.py` & `mootdx-0.9.9/mootdx/financial/base.py`

 * *Files identical despite different names*

### Comparing `mootdx-0.9.8/mootdx/financial/columns.py` & `mootdx-0.9.9/mootdx/financial/columns.py`

 * *Files identical despite different names*

### Comparing `mootdx-0.9.8/mootdx/financial/financial.py` & `mootdx-0.9.9/mootdx/financial/financial.py`

 * *Files identical despite different names*

### Comparing `mootdx-0.9.8/mootdx/parse.py` & `mootdx-0.9.9/mootdx/parse.py`

 * *Files identical despite different names*

### Comparing `mootdx-0.9.8/mootdx/quotes.py` & `mootdx-0.9.9/mootdx/quotes.py`

 * *Files identical despite different names*

### Comparing `mootdx-0.9.8/mootdx/reader.py` & `mootdx-0.9.9/mootdx/reader.py`

 * *Files identical despite different names*

### Comparing `mootdx-0.9.8/mootdx/server.py` & `mootdx-0.9.9/mootdx/server.py`

 * *Files identical despite different names*

### Comparing `mootdx-0.9.8/mootdx/tools/customize.py` & `mootdx-0.9.9/mootdx/tools/customize.py`

 * *Files identical despite different names*

### Comparing `mootdx-0.9.8/mootdx/tools/reversion.py` & `mootdx-0.9.9/mootdx/tools/reversion.py`

 * *Files identical despite different names*

### Comparing `mootdx-0.9.8/mootdx/tools/tdx2csv.py` & `mootdx-0.9.9/mootdx/tools/tdx2csv.py`

 * *Files identical despite different names*

### Comparing `mootdx-0.9.8/mootdx/utils/__init__.py` & `mootdx-0.9.9/mootdx/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mootdx-0.9.8/mootdx/utils/adjust.py` & `mootdx-0.9.9/mootdx/utils/adjust.py`

 * *Files identical despite different names*

### Comparing `mootdx-0.9.8/mootdx/utils/holiday.py` & `mootdx-0.9.9/mootdx/utils/holiday.py`

 * *Files identical despite different names*

### Comparing `mootdx-0.9.8/mootdx.egg-info/PKG-INFO` & `mootdx-0.9.9/mootdx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mootdx
-Version: 0.9.8
+Version: 0.9.9
 Summary: 通达信数据读取接口.
 Home-page: https://github.com/mootdx/mootdx
 Author: bopo.wang
 Author-email: ibopo@126.com
 License: MIT license
 Keywords: mootdx
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -12,14 +12,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 License-File: LICENSE
 License-File: AUTHORS.rst
 
 通达信数据读取接口
 ==================
 
 .. image:: https://badge.fury.io/py/mootdx.svg
```

### Comparing `mootdx-0.9.8/mootdx.egg-info/SOURCES.txt` & `mootdx-0.9.9/mootdx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mootdx-0.9.8/pyproject.toml` & `mootdx-0.9.9/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "mootdx"
-version = "0.9.8"
+version = "0.9.9"
 description = ""
 authors = ["bopo <ibopo@126.com>"]
-readme = "README.md"
+readme = "README.rst"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 click = "^8.1.3"
 httpx = "^0.23.1"
 pandas = "^1.5.2"
 prettytable = "^3.5.0"
```

### Comparing `mootdx-0.9.8/setup.cfg` & `mootdx-0.9.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.9.8
+current_version = 0.9.9
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `mootdx-0.9.8/setup.py` & `mootdx-0.9.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 requirements = parse_requirements("requirements.txt")
 test_requirements = requirements
 # test_requirements.append('pytest')
 
 setup(
     name="mootdx",
-    version="0.9.8",
+    version="0.9.9",
     description="通达信数据读取接口.",
     long_description=readme,
     author="bopo.wang",
     author_email="ibopo@126.com",
     url="https://github.com/mootdx/mootdx",
     packages=find_packages(include=["mootdx", "mootdx.*"]),
     # include_package_data=True,
@@ -47,12 +47,14 @@
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     test_suite="tests",
     tests_require=test_requirements,
     setup_requires=requirements,
 )
```

