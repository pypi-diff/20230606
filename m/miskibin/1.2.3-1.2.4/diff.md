# Comparing `tmp/miskibin-1.2.3.tar.gz` & `tmp/miskibin-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miskibin-1.2.3.tar", last modified: Tue Jun  6 11:24:50 2023, max compression
+gzip compressed data, was "miskibin-1.2.4.tar", last modified: Tue Jun  6 12:39:54 2023, max compression
```

## Comparing `miskibin-1.2.3.tar` & `miskibin-1.2.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:24:50.517864 miskibin-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-06 11:24:50.517864 miskibin-1.2.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:24:50.513864 miskibin-1.2.3/miskibin/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-06 11:24:40.000000 miskibin-1.2.3/miskibin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-06 11:24:40.000000 miskibin-1.2.3/miskibin/_logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-06-06 11:24:40.000000 miskibin-1.2.3/miskibin/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:24:50.517864 miskibin-1.2.3/miskibin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-06 11:24:50.000000 miskibin-1.2.3/miskibin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-06 11:24:50.000000 miskibin-1.2.3/miskibin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 11:24:50.000000 miskibin-1.2.3/miskibin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-06 11:24:50.000000 miskibin-1.2.3/miskibin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 11:24:50.517864 miskibin-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-06-06 11:24:40.000000 miskibin-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:39:54.344526 miskibin-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-06 12:39:54.344526 miskibin-1.2.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:39:54.344526 miskibin-1.2.4/miskibin/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-06 12:39:40.000000 miskibin-1.2.4/miskibin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-06 12:39:40.000000 miskibin-1.2.4/miskibin/_logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-06-06 12:39:40.000000 miskibin-1.2.4/miskibin/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:39:54.344526 miskibin-1.2.4/miskibin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-06 12:39:54.000000 miskibin-1.2.4/miskibin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-06 12:39:54.000000 miskibin-1.2.4/miskibin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 12:39:54.000000 miskibin-1.2.4/miskibin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-06 12:39:54.000000 miskibin-1.2.4/miskibin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 12:39:54.344526 miskibin-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-06-06 12:39:40.000000 miskibin-1.2.4/setup.py
```

### Comparing `miskibin-1.2.3/PKG-INFO` & `miskibin-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miskibin
-Version: 1.2.3
+Version: 1.2.4
 Summary: My personal package for colored logs. Highly customizable.
 Home-page: https://github.com/michalskibinski109/miskibin
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `miskibin-1.2.3/miskibin/_logging_utils.py` & `miskibin-1.2.4/miskibin/_logging_utils.py`

 * *Files identical despite different names*

### Comparing `miskibin-1.2.3/miskibin/utils.py` & `miskibin-1.2.4/miskibin/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,22 +31,22 @@
         Available configurations:
             simple: simple logger that works like print() but with colors
             proffesional: saves logs to file, displays time, filename line number and lvl
             default: default logger configuration
     Returns:
         Logger with colored logs and filter for ipynb cells.
     """
-    if type:
+    if predefined:
         try:
-            config = _LOGGERS[type]
+            config = _LOGGERS[predefined]
         except KeyError:
             raise FailedToLoadLoggingConfigException(
-                f"Failed to load predefined configuration: {type}"
+                f"Failed to load predefined configuration: {predefined}"
             )
-        type = None
+        predefined = None
         return get_logger(**config.__dict__)
     if disable_existing_loggers:
         logging.config.dictConfig(
             {
                 "version": 1,
                 "disable_existing_loggers": True,
             }
```

### Comparing `miskibin-1.2.3/miskibin.egg-info/PKG-INFO` & `miskibin-1.2.4/miskibin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miskibin
-Version: 1.2.3
+Version: 1.2.4
 Summary: My personal package for colored logs. Highly customizable.
 Home-page: https://github.com/michalskibinski109/miskibin
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `miskibin-1.2.3/setup.py` & `miskibin-1.2.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
 <img src="https://user-images.githubusercontent.com/77834536/201939466-228b110f-21de-4461-9c86-55f8f46652ef.png" width="500"/>
 
 """
 
 setuptools.setup(
     name="miskibin",
-    version="1.2.3",
+    version="1.2.4",
     author="Michał Skibiński",
     author_email="mskibinski109@gmail.com",
     description="My personal package for colored logs. Highly customizable.",
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     files_to_include=["miskibin"],
     url="https://github.com/michalskibinski109/miskibin",
```

