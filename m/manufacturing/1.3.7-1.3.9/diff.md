# Comparing `tmp/manufacturing-1.3.7.tar.gz` & `tmp/manufacturing-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "manufacturing-1.3.7.tar", max compression
+gzip compressed data, was "manufacturing-1.3.9.tar", max compression
```

## Comparing `manufacturing-1.3.7.tar` & `manufacturing-1.3.9.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0      918 2022-10-17 18:21:41.939884 manufacturing-1.3.7/manufacturing/__init__.py
--rw-r--r--   0        0        0     5098 2022-10-17 18:21:41.939884 manufacturing-1.3.7/manufacturing/alt_analysis.py
--rw-r--r--   0        0        0    17338 2022-10-17 18:21:41.939884 manufacturing-1.3.7/manufacturing/alt_vis.py
--rw-r--r--   0        0        0    19440 2022-10-17 18:21:41.939884 manufacturing-1.3.7/manufacturing/analysis.py
--rw-r--r--   0        0        0     3289 2022-10-17 18:21:41.939884 manufacturing-1.3.7/manufacturing/data_import.py
--rw-r--r--   0        0        0     4510 2022-10-17 18:21:41.939884 manufacturing-1.3.7/manufacturing/lookup_tables.py
--rw-r--r--   0        0        0     4391 2022-10-17 18:21:41.939884 manufacturing-1.3.7/manufacturing/report.py
--rw-r--r--   0        0        0     2242 2022-10-17 18:21:41.939884 manufacturing-1.3.7/manufacturing/util.py
--rw-r--r--   0        0        0    56476 2022-10-17 18:21:41.943884 manufacturing-1.3.7/manufacturing/visual.py
--rw-r--r--   0        0        0      611 2022-10-17 18:21:41.943884 manufacturing-1.3.7/pyproject.toml
--rw-r--r--   0        0        0     3010 2022-10-17 18:21:41.943884 manufacturing-1.3.7/readme.md
--rw-r--r--   0        0        0     3860 1970-01-01 00:00:00.000000 manufacturing-1.3.7/setup.py
--rw-r--r--   0        0        0     3718 1970-01-01 00:00:00.000000 manufacturing-1.3.7/PKG-INFO
+-rw-r--r--   0        0        0      918 2023-06-06 15:17:14.950840 manufacturing-1.3.9/manufacturing/__init__.py
+-rw-r--r--   0        0        0     5098 2023-06-06 15:17:14.950840 manufacturing-1.3.9/manufacturing/alt_analysis.py
+-rw-r--r--   0        0        0    17338 2023-06-06 15:17:14.950840 manufacturing-1.3.9/manufacturing/alt_vis.py
+-rw-r--r--   0        0        0    19440 2023-06-06 15:17:14.950840 manufacturing-1.3.9/manufacturing/analysis.py
+-rw-r--r--   0        0        0     3289 2023-06-06 15:17:14.950840 manufacturing-1.3.9/manufacturing/data_import.py
+-rw-r--r--   0        0        0     4510 2023-06-06 15:17:14.950840 manufacturing-1.3.9/manufacturing/lookup_tables.py
+-rw-r--r--   0        0        0     4391 2023-06-06 15:17:14.950840 manufacturing-1.3.9/manufacturing/report.py
+-rw-r--r--   0        0        0     2242 2023-06-06 15:17:14.950840 manufacturing-1.3.9/manufacturing/util.py
+-rw-r--r--   0        0        0    56472 2023-06-06 15:17:14.950840 manufacturing-1.3.9/manufacturing/visual.py
+-rw-r--r--   0        0        0      611 2023-06-06 15:17:14.950840 manufacturing-1.3.9/pyproject.toml
+-rw-r--r--   0        0        0     3010 2023-06-06 15:17:14.954840 manufacturing-1.3.9/readme.md
+-rw-r--r--   0        0        0     3718 1970-01-01 00:00:00.000000 manufacturing-1.3.9/PKG-INFO
```

### Comparing `manufacturing-1.3.7/manufacturing/__init__.py` & `manufacturing-1.3.9/manufacturing/__init__.py`

 * *Files identical despite different names*

### Comparing `manufacturing-1.3.7/manufacturing/alt_analysis.py` & `manufacturing-1.3.9/manufacturing/alt_analysis.py`

 * *Files identical despite different names*

### Comparing `manufacturing-1.3.7/manufacturing/alt_vis.py` & `manufacturing-1.3.9/manufacturing/alt_vis.py`

 * *Files identical despite different names*

### Comparing `manufacturing-1.3.7/manufacturing/analysis.py` & `manufacturing-1.3.9/manufacturing/analysis.py`

 * *Files identical despite different names*

### Comparing `manufacturing-1.3.7/manufacturing/data_import.py` & `manufacturing-1.3.9/manufacturing/data_import.py`

 * *Files identical despite different names*

### Comparing `manufacturing-1.3.7/manufacturing/lookup_tables.py` & `manufacturing-1.3.9/manufacturing/lookup_tables.py`

 * *Files identical despite different names*

### Comparing `manufacturing-1.3.7/manufacturing/report.py` & `manufacturing-1.3.9/manufacturing/report.py`

 * *Files identical despite different names*

### Comparing `manufacturing-1.3.7/manufacturing/util.py` & `manufacturing-1.3.9/manufacturing/util.py`

 * *Files identical despite different names*

### Comparing `manufacturing-1.3.7/manufacturing/visual.py` & `manufacturing-1.3.9/manufacturing/visual.py`

 * *Files 0% similar despite different names*

```diff
@@ -476,15 +476,15 @@
                 edgecolor="red",
                 zorder=zorder,
             )
             diameter += diameter_inc
             zorder -= 1
             show_legend = True
 
-            for i, v in beyond_limits_violations.iteritems():
+            for i, v in beyond_limits_violations.items():
                 ax.axvline(i, color='red', alpha=0.4)
 
     if highlight_zone_a:
         zone_a_violations = control_zone_a(
             data=data,
             upper_control_limit=upper_control_limit,
             lower_control_limit=lower_control_limit,
```

### Comparing `manufacturing-1.3.7/pyproject.toml` & `manufacturing-1.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "manufacturing"
-version = "1.3.7"
+version = "1.3.9"
 description = "Six-Sigma based analysis of manufacturing data"
 readme = 'readme.md'
 authors = ["Jason R. Jones <slightlynybbled@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
```

### Comparing `manufacturing-1.3.7/readme.md` & `manufacturing-1.3.9/readme.md`

 * *Files identical despite different names*

### Comparing `manufacturing-1.3.7/PKG-INFO` & `manufacturing-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: manufacturing
-Version: 1.3.7
+Version: 1.3.9
 Summary: Six-Sigma based analysis of manufacturing data
 License: MIT
 Author: Jason R. Jones
 Author-email: slightlynybbled@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

