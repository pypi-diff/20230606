# Comparing `tmp/triad-0.8.9.tar.gz` & `tmp/triad-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "triad-0.8.9.tar", last modified: Sat Jun  3 06:34:12 2023, max compression
+gzip compressed data, was "triad-0.9.0.tar", last modified: Tue Jun  6 07:04:41 2023, max compression
```

## Comparing `triad-0.8.9.tar` & `triad-0.9.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 06:34:12.801595 triad-0.8.9/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-03 06:33:22.000000 triad-0.8.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-06-03 06:34:12.801595 triad-0.8.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-06-03 06:33:22.000000 triad-0.8.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-03 06:34:12.801595 triad-0.8.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-03 06:33:22.000000 triad-0.8.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 06:34:12.789595 triad-0.8.9/triad/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-03 06:33:22.000000 triad-0.8.9/triad/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 06:34:12.793595 triad-0.8.9/triad/collections/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-03 06:33:22.000000 triad-0.8.9/triad/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-06-03 06:33:22.000000 triad-0.8.9/triad/collections/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     7044 2023-06-03 06:33:22.000000 triad-0.8.9/triad/collections/fs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11050 2023-06-03 06:33:22.000000 triad-0.8.9/triad/collections/function_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    19448 2023-06-03 06:33:22.000000 triad-0.8.9/triad/collections/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-03 06:33:22.000000 triad-0.8.9/triad/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-03 06:33:22.000000 triad-0.8.9/triad/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 06:34:12.801595 triad-0.8.9/triad/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-03 06:33:22.000000 triad-0.8.9/triad/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-03 06:33:22.000000 triad-0.8.9/triad/utils/assertion.py
--rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-06-03 06:33:22.000000 triad-0.8.9/triad/utils/batch_reslicers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-06-03 06:33:22.000000 triad-0.8.9/triad/utils/class_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)    17464 2023-06-03 06:33:22.000000 triad-0.8.9/triad/utils/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    11774 2023-06-03 06:33:22.000000 triad-0.8.9/triad/utils/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-03 06:33:22.000000 triad-0.8.9/triad/utils/entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-03 06:33:22.000000 triad-0.8.9/triad/utils/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     9352 2023-06-03 06:33:22.000000 triad-0.8.9/triad/utils/iter.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-03 06:33:22.000000 triad-0.8.9/triad/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    10649 2023-06-03 06:33:22.000000 triad-0.8.9/triad/utils/pandas_like.py
--rw-r--r--   0 runner    (1001) docker     (123)    29555 2023-06-03 06:33:22.000000 triad-0.8.9/triad/utils/pyarrow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-06-03 06:33:22.000000 triad-0.8.9/triad/utils/rename.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-06-03 06:33:22.000000 triad-0.8.9/triad/utils/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-03 06:33:22.000000 triad-0.8.9/triad/utils/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-06-03 06:33:22.000000 triad-0.8.9/triad/utils/threading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 06:34:12.793595 triad-0.8.9/triad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-06-03 06:34:12.000000 triad-0.8.9/triad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-03 06:34:12.000000 triad-0.8.9/triad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 06:34:12.000000 triad-0.8.9/triad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-03 06:34:12.000000 triad-0.8.9/triad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-03 06:34:12.000000 triad-0.8.9/triad.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 06:34:12.801595 triad-0.8.9/triad_version/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-03 06:33:22.000000 triad-0.8.9/triad_version/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:04:41.876869 triad-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-06 07:04:05.000000 triad-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-06-06 07:04:41.876869 triad-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-06 07:04:05.000000 triad-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-06 07:04:41.876869 triad-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-06 07:04:05.000000 triad-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:04:41.864869 triad-0.9.0/triad/
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-06 07:04:05.000000 triad-0.9.0/triad/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:04:41.868869 triad-0.9.0/triad/collections/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-06 07:04:05.000000 triad-0.9.0/triad/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-06-06 07:04:05.000000 triad-0.9.0/triad/collections/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7044 2023-06-06 07:04:05.000000 triad-0.9.0/triad/collections/fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11050 2023-06-06 07:04:05.000000 triad-0.9.0/triad/collections/function_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19448 2023-06-06 07:04:05.000000 triad-0.9.0/triad/collections/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-06 07:04:05.000000 triad-0.9.0/triad/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-06 07:04:05.000000 triad-0.9.0/triad/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:04:41.872869 triad-0.9.0/triad/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-06 07:04:05.000000 triad-0.9.0/triad/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-06 07:04:05.000000 triad-0.9.0/triad/utils/assertion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-06-06 07:04:05.000000 triad-0.9.0/triad/utils/batch_reslicers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-06-06 07:04:05.000000 triad-0.9.0/triad/utils/class_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17464 2023-06-06 07:04:05.000000 triad-0.9.0/triad/utils/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11774 2023-06-06 07:04:05.000000 triad-0.9.0/triad/utils/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-06 07:04:05.000000 triad-0.9.0/triad/utils/entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-06 07:04:05.000000 triad-0.9.0/triad/utils/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9352 2023-06-06 07:04:05.000000 triad-0.9.0/triad/utils/iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-06 07:04:05.000000 triad-0.9.0/triad/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17048 2023-06-06 07:04:05.000000 triad-0.9.0/triad/utils/pandas_like.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29555 2023-06-06 07:04:05.000000 triad-0.9.0/triad/utils/pyarrow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-06-06 07:04:05.000000 triad-0.9.0/triad/utils/rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-06-06 07:04:05.000000 triad-0.9.0/triad/utils/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-06 07:04:05.000000 triad-0.9.0/triad/utils/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-06-06 07:04:05.000000 triad-0.9.0/triad/utils/threading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:04:41.868869 triad-0.9.0/triad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-06-06 07:04:41.000000 triad-0.9.0/triad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-06 07:04:41.000000 triad-0.9.0/triad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 07:04:41.000000 triad-0.9.0/triad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-06 07:04:41.000000 triad-0.9.0/triad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-06 07:04:41.000000 triad-0.9.0/triad.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:04:41.872869 triad-0.9.0/triad_version/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-06 07:04:05.000000 triad-0.9.0/triad_version/__init__.py
```

### Comparing `triad-0.8.9/LICENSE` & `triad-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `triad-0.8.9/PKG-INFO` & `triad-0.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triad
-Version: 0.8.9
+Version: 0.9.0
 Summary: A collection of python utils for Fugue projects
 Home-page: http://github.com/fugue-project/triad
 Author: The Fugue Development Team
 Author-email: hello@fugue.ai
 License: Apache-2.0
 Description: # Triad
         
@@ -24,14 +24,18 @@
         ```bash
         pip install triad
         ```
         
         
         ## Release History
         
+        ### 0.9.0
+        
+        * Merge QPD pandas utils functions back to Triad
+        
         ### 0.8.9
         
         * Add batch reslicers
         * Fix package issue (exclude tests folder)
         
         ### 0.8.8
```

### Comparing `triad-0.8.9/README.md` & `triad-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,18 @@
 ```bash
 pip install triad
 ```
 
 
 ## Release History
 
+### 0.9.0
+
+* Merge QPD pandas utils functions back to Triad
+
 ### 0.8.9
 
 * Add batch reslicers
 * Fix package issue (exclude tests folder)
 
 ### 0.8.8
```

### Comparing `triad-0.8.9/setup.py` & `triad-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.9/triad/collections/dict.py` & `triad-0.9.0/triad/collections/dict.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.9/triad/collections/fs.py` & `triad-0.9.0/triad/collections/fs.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.9/triad/collections/function_wrapper.py` & `triad-0.9.0/triad/collections/function_wrapper.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.9/triad/collections/schema.py` & `triad-0.9.0/triad/collections/schema.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.9/triad/utils/assertion.py` & `triad-0.9.0/triad/utils/assertion.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.9/triad/utils/batch_reslicers.py` & `triad-0.9.0/triad/utils/batch_reslicers.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.9/triad/utils/class_extension.py` & `triad-0.9.0/triad/utils/class_extension.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.9/triad/utils/convert.py` & `triad-0.9.0/triad/utils/convert.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.9/triad/utils/dispatcher.py` & `triad-0.9.0/triad/utils/dispatcher.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.9/triad/utils/entry_points.py` & `triad-0.9.0/triad/utils/entry_points.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.9/triad/utils/hash.py` & `triad-0.9.0/triad/utils/hash.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.9/triad/utils/iter.py` & `triad-0.9.0/triad/utils/iter.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.9/triad/utils/json.py` & `triad-0.9.0/triad/utils/json.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.9/triad/utils/pyarrow.py` & `triad-0.9.0/triad/utils/pyarrow.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.9/triad/utils/rename.py` & `triad-0.9.0/triad/utils/rename.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.9/triad/utils/schema.py` & `triad-0.9.0/triad/utils/schema.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.9/triad/utils/string.py` & `triad-0.9.0/triad/utils/string.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.9/triad/utils/threading.py` & `triad-0.9.0/triad/utils/threading.py`

 * *Files identical despite different names*

### Comparing `triad-0.8.9/triad.egg-info/PKG-INFO` & `triad-0.9.0/triad.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triad
-Version: 0.8.9
+Version: 0.9.0
 Summary: A collection of python utils for Fugue projects
 Home-page: http://github.com/fugue-project/triad
 Author: The Fugue Development Team
 Author-email: hello@fugue.ai
 License: Apache-2.0
 Description: # Triad
         
@@ -24,14 +24,18 @@
         ```bash
         pip install triad
         ```
         
         
         ## Release History
         
+        ### 0.9.0
+        
+        * Merge QPD pandas utils functions back to Triad
+        
         ### 0.8.9
         
         * Add batch reslicers
         * Fix package issue (exclude tests folder)
         
         ### 0.8.8
```

### Comparing `triad-0.8.9/triad.egg-info/SOURCES.txt` & `triad-0.9.0/triad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

