# Comparing `tmp/commodplot-1.6.2.tar.gz` & `tmp/commodplot-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commodplot-1.6.2.tar", last modified: Mon Jun  5 11:43:08 2023, max compression
+gzip compressed data, was "commodplot-1.6.3.tar", last modified: Tue Jun  6 12:03:01 2023, max compression
```

## Comparing `commodplot-1.6.2.tar` & `commodplot-1.6.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:43:08.051389 commodplot-1.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-05 11:43:08.051389 commodplot-1.6.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:43:08.051389 commodplot-1.6.2/commodplot/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 11:42:57.000000 commodplot-1.6.2/commodplot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16416 2023-06-05 11:42:57.000000 commodplot-1.6.2/commodplot/commodplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-06-05 11:42:57.000000 commodplot-1.6.2/commodplot/commodplottable.py
--rw-r--r--   0 runner    (1001) docker     (123)    13925 2023-06-05 11:42:57.000000 commodplot-1.6.2/commodplot/commodplottrace.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-05 11:42:57.000000 commodplot-1.6.2/commodplot/commodplottransform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-06-05 11:42:57.000000 commodplot-1.6.2/commodplot/commodplotutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-06-05 11:42:57.000000 commodplot-1.6.2/commodplot/jinjautils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-06-05 11:42:57.000000 commodplot-1.6.2/commodplot/messaging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:43:08.051389 commodplot-1.6.2/commodplot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-05 11:43:07.000000 commodplot-1.6.2/commodplot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-05 11:43:08.000000 commodplot-1.6.2/commodplot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 11:43:07.000000 commodplot-1.6.2/commodplot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-05 11:43:07.000000 commodplot-1.6.2/commodplot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-05 11:43:07.000000 commodplot-1.6.2/commodplot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-05 11:43:08.051389 commodplot-1.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-05 11:42:57.000000 commodplot-1.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 11:43:08.051389 commodplot-1.6.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 11:42:57.000000 commodplot-1.6.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9355 2023-06-05 11:42:57.000000 commodplot-1.6.2/test/test_commodplot.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-05 11:42:57.000000 commodplot-1.6.2/test/test_commodplottable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-05 11:42:57.000000 commodplot-1.6.2/test/test_commodplottrace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-05 11:42:57.000000 commodplot-1.6.2/test/test_commodplotutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-05 11:42:57.000000 commodplot-1.6.2/test/test_jinjautils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-05 11:42:57.000000 commodplot-1.6.2/test/test_messaging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:03:01.383042 commodplot-1.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-06 12:03:01.383042 commodplot-1.6.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:03:01.379042 commodplot-1.6.3/commodplot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:50.000000 commodplot-1.6.3/commodplot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16416 2023-06-06 12:02:50.000000 commodplot-1.6.3/commodplot/commodplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-06-06 12:02:50.000000 commodplot-1.6.3/commodplot/commodplottable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13925 2023-06-06 12:02:50.000000 commodplot-1.6.3/commodplot/commodplottrace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-06 12:02:50.000000 commodplot-1.6.3/commodplot/commodplottransform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5444 2023-06-06 12:02:50.000000 commodplot-1.6.3/commodplot/commodplotutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-06-06 12:02:50.000000 commodplot-1.6.3/commodplot/jinjautils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-06-06 12:02:50.000000 commodplot-1.6.3/commodplot/messaging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:03:01.383042 commodplot-1.6.3/commodplot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-06 12:03:01.000000 commodplot-1.6.3/commodplot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-06 12:03:01.000000 commodplot-1.6.3/commodplot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 12:03:01.000000 commodplot-1.6.3/commodplot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-06 12:03:01.000000 commodplot-1.6.3/commodplot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-06 12:03:01.000000 commodplot-1.6.3/commodplot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-06 12:03:01.383042 commodplot-1.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-06 12:02:50.000000 commodplot-1.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:03:01.383042 commodplot-1.6.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 12:02:50.000000 commodplot-1.6.3/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9355 2023-06-06 12:02:50.000000 commodplot-1.6.3/test/test_commodplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-06 12:02:50.000000 commodplot-1.6.3/test/test_commodplottable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-06 12:02:50.000000 commodplot-1.6.3/test/test_commodplottrace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-06 12:02:50.000000 commodplot-1.6.3/test/test_commodplotutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-06 12:02:50.000000 commodplot-1.6.3/test/test_jinjautils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-06 12:02:50.000000 commodplot-1.6.3/test/test_messaging.py
```

### Comparing `commodplot-1.6.2/commodplot/commodplot.py` & `commodplot-1.6.3/commodplot/commodplot.py`

 * *Files identical despite different names*

### Comparing `commodplot-1.6.2/commodplot/commodplottable.py` & `commodplot-1.6.3/commodplot/commodplottable.py`

 * *Files identical despite different names*

### Comparing `commodplot-1.6.2/commodplot/commodplottrace.py` & `commodplot-1.6.3/commodplot/commodplottrace.py`

 * *Files identical despite different names*

### Comparing `commodplot-1.6.2/commodplot/commodplottransform.py` & `commodplot-1.6.3/commodplot/commodplottransform.py`

 * *Files identical despite different names*

### Comparing `commodplot-1.6.2/commodplot/commodplotutil.py` & `commodplot-1.6.3/commodplot/commodplotutil.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     symb = "+" if delta > 0.0 else ""
 
     if precision_format:
         val1, delta = precision_format.format(val1), precision_format.format(delta)
     else:
         val1 = val1.round(2)
 
-    s = "{}   △: {}{}".format(val1, symb, delta)
+    s = "{}   \u0394: {}{}".format(val1, symb, delta)
     return s
 
 
 def format_date_col(col, date_format="%d-%b"):
     """
     Format a column heading as a data
     :param col:
```

### Comparing `commodplot-1.6.2/commodplot/jinjautils.py` & `commodplot-1.6.3/commodplot/jinjautils.py`

 * *Files identical despite different names*

### Comparing `commodplot-1.6.2/commodplot/messaging.py` & `commodplot-1.6.3/commodplot/messaging.py`

 * *Files identical despite different names*

### Comparing `commodplot-1.6.2/commodplot.egg-info/SOURCES.txt` & `commodplot-1.6.3/commodplot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `commodplot-1.6.2/setup.py` & `commodplot-1.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="commodplot",
-    version="1.6.2",
+    version="1.6.3",
     author="aeorxc",
     author_email="author@example.com",
     description="common commodity plotting including seasonal charts using plotly",
     url="https://github.com/aeorxc/commodplot",
     project_urls={
         "Source": "https://github.com/aeorxc/commodplot",
     },
```

### Comparing `commodplot-1.6.2/test/test_commodplot.py` & `commodplot-1.6.3/test/test_commodplot.py`

 * *Files identical despite different names*

### Comparing `commodplot-1.6.2/test/test_commodplottable.py` & `commodplot-1.6.3/test/test_commodplottable.py`

 * *Files identical despite different names*

### Comparing `commodplot-1.6.2/test/test_commodplottrace.py` & `commodplot-1.6.3/test/test_commodplottrace.py`

 * *Files identical despite different names*

### Comparing `commodplot-1.6.2/test/test_commodplotutil.py` & `commodplot-1.6.3/test/test_commodplotutil.py`

 * *Files identical despite different names*

### Comparing `commodplot-1.6.2/test/test_jinjautils.py` & `commodplot-1.6.3/test/test_jinjautils.py`

 * *Files identical despite different names*

### Comparing `commodplot-1.6.2/test/test_messaging.py` & `commodplot-1.6.3/test/test_messaging.py`

 * *Files identical despite different names*

