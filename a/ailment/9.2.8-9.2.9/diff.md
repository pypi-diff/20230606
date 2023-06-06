# Comparing `tmp/ailment-9.2.8.tar.gz` & `tmp/ailment-9.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ailment-9.2.8.tar", last modified: Tue Jun 28 17:02:53 2022, max compression
+gzip compressed data, was "ailment-9.2.9.tar", last modified: Tue Jul  5 17:02:34 2022, max compression
```

## Comparing `ailment-9.2.8.tar` & `ailment-9.2.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:02:53.206723 ailment-9.2.8/
--rw-r--r--   0 vsts      (1001) docker     (121)     1327 2022-06-28 17:01:18.000000 ailment-9.2.8/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (121)      442 2022-06-28 17:02:53.206723 ailment-9.2.8/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)       49 2022-06-28 17:01:18.000000 ailment-9.2.8/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:02:53.206723 ailment-9.2.8/ailment/
--rw-r--r--   0 vsts      (1001) docker     (121)     1534 2022-06-28 17:01:35.000000 ailment-9.2.8/ailment/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1856 2022-06-28 17:01:18.000000 ailment-9.2.8/ailment/block.py
--rw-r--r--   0 vsts      (1001) docker     (121)      146 2022-06-28 17:01:18.000000 ailment-9.2.8/ailment/converter_common.py
--rw-r--r--   0 vsts      (1001) docker     (121)    19521 2022-06-28 17:01:18.000000 ailment-9.2.8/ailment/converter_pcode.py
--rw-r--r--   0 vsts      (1001) docker     (121)    21275 2022-06-28 17:01:18.000000 ailment-9.2.8/ailment/converter_vex.py
--rw-r--r--   0 vsts      (1001) docker     (121)    24974 2022-06-28 17:01:18.000000 ailment-9.2.8/ailment/expression.py
--rw-r--r--   0 vsts      (1001) docker     (121)      702 2022-06-28 17:01:18.000000 ailment-9.2.8/ailment/manager.py
--rw-r--r--   0 vsts      (1001) docker     (121)    16439 2022-06-28 17:01:18.000000 ailment-9.2.8/ailment/statement.py
--rw-r--r--   0 vsts      (1001) docker     (121)      936 2022-06-28 17:01:18.000000 ailment-9.2.8/ailment/tagged_object.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2665 2022-06-28 17:01:18.000000 ailment-9.2.8/ailment/utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:02:53.206723 ailment-9.2.8/ailment.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (121)      442 2022-06-28 17:02:52.000000 ailment-9.2.8/ailment.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)      387 2022-06-28 17:02:53.000000 ailment-9.2.8/ailment.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-06-28 17:02:52.000000 ailment-9.2.8/ailment.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        8 2022-06-28 17:02:53.000000 ailment-9.2.8/ailment.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       98 2022-06-28 17:01:35.000000 ailment-9.2.8/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (121)      497 2022-06-28 17:02:53.206723 ailment-9.2.8/setup.cfg
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:02:34.225067 ailment-9.2.9/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1327 2022-07-05 17:01:22.000000 ailment-9.2.9/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (121)      442 2022-07-05 17:02:34.225067 ailment-9.2.9/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)       49 2022-07-05 17:01:22.000000 ailment-9.2.9/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:02:34.225067 ailment-9.2.9/ailment/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1534 2022-07-05 17:01:34.000000 ailment-9.2.9/ailment/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1856 2022-07-05 17:01:22.000000 ailment-9.2.9/ailment/block.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      146 2022-07-05 17:01:22.000000 ailment-9.2.9/ailment/converter_common.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    19521 2022-07-05 17:01:22.000000 ailment-9.2.9/ailment/converter_pcode.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    21275 2022-07-05 17:01:22.000000 ailment-9.2.9/ailment/converter_vex.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    24974 2022-07-05 17:01:22.000000 ailment-9.2.9/ailment/expression.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      702 2022-07-05 17:01:22.000000 ailment-9.2.9/ailment/manager.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    16439 2022-07-05 17:01:22.000000 ailment-9.2.9/ailment/statement.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      936 2022-07-05 17:01:22.000000 ailment-9.2.9/ailment/tagged_object.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     2665 2022-07-05 17:01:22.000000 ailment-9.2.9/ailment/utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:02:34.225067 ailment-9.2.9/ailment.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (121)      442 2022-07-05 17:02:34.000000 ailment-9.2.9/ailment.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)      387 2022-07-05 17:02:34.000000 ailment-9.2.9/ailment.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-07-05 17:02:34.000000 ailment-9.2.9/ailment.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        8 2022-07-05 17:02:34.000000 ailment-9.2.9/ailment.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)       98 2022-07-05 17:01:34.000000 ailment-9.2.9/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (121)      497 2022-07-05 17:02:34.225067 ailment-9.2.9/setup.cfg
```

### Comparing `ailment-9.2.8/LICENSE` & `ailment-9.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ailment-9.2.8/ailment/__init__.py` & `ailment-9.2.9/ailment/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "9.2.8"
+__version__ = "9.2.9"
 
 import logging
 from typing import Set
 
 from .block import Block
 from . import statement as Stmt
 from . import expression as Expr
```

### Comparing `ailment-9.2.8/ailment/block.py` & `ailment-9.2.9/ailment/block.py`

 * *Files identical despite different names*

### Comparing `ailment-9.2.8/ailment/converter_pcode.py` & `ailment-9.2.9/ailment/converter_pcode.py`

 * *Files identical despite different names*

### Comparing `ailment-9.2.8/ailment/converter_vex.py` & `ailment-9.2.9/ailment/converter_vex.py`

 * *Files identical despite different names*

### Comparing `ailment-9.2.8/ailment/expression.py` & `ailment-9.2.9/ailment/expression.py`

 * *Files identical despite different names*

### Comparing `ailment-9.2.8/ailment/manager.py` & `ailment-9.2.9/ailment/manager.py`

 * *Files identical despite different names*

### Comparing `ailment-9.2.8/ailment/statement.py` & `ailment-9.2.9/ailment/statement.py`

 * *Files identical despite different names*

### Comparing `ailment-9.2.8/ailment/tagged_object.py` & `ailment-9.2.9/ailment/tagged_object.py`

 * *Files identical despite different names*

### Comparing `ailment-9.2.8/ailment/utils.py` & `ailment-9.2.9/ailment/utils.py`

 * *Files identical despite different names*

