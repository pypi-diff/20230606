# Comparing `tmp/cdnmon-0.2.4.tar.gz` & `tmp/cdnmon-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdnmon-0.2.4.tar", max compression
+gzip compressed data, was "cdnmon-0.2.5.tar", max compression
```

## Comparing `cdnmon-0.2.4.tar` & `cdnmon-0.2.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      934 2023-06-06 08:00:30.901968 cdnmon-0.2.4/README.md
--rw-r--r--   0        0        0      516 2023-06-06 08:00:30.901968 cdnmon-0.2.4/cdnmon/__init__.py
--rw-r--r--   0        0        0      256 2023-06-06 08:00:30.901968 cdnmon-0.2.4/cdnmon/config.py
--rw-r--r--   0        0        0       32 2023-06-06 08:00:30.901968 cdnmon-0.2.4/cdnmon/settings.py
--rw-r--r--   0        0        0      382 2023-06-06 08:00:30.901968 cdnmon-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     1455 1970-01-01 00:00:00.000000 cdnmon-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      934 2023-06-06 08:04:02.732516 cdnmon-0.2.5/README.md
+-rw-r--r--   0        0        0      516 2023-06-06 08:04:02.732516 cdnmon-0.2.5/cdnmon/__init__.py
+-rw-r--r--   0        0        0      404 2023-06-06 08:04:02.732516 cdnmon-0.2.5/cdnmon/config.py
+-rw-r--r--   0        0        0       32 2023-06-06 08:04:02.732516 cdnmon-0.2.5/cdnmon/settings.py
+-rw-r--r--   0        0        0      382 2023-06-06 08:04:02.732516 cdnmon-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     1455 1970-01-01 00:00:00.000000 cdnmon-0.2.5/PKG-INFO
```

### Comparing `cdnmon-0.2.4/README.md` & `cdnmon-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `cdnmon-0.2.4/cdnmon/__init__.py` & `cdnmon-0.2.5/cdnmon/__init__.py`

 * *Files identical despite different names*

### Comparing `cdnmon-0.2.4/PKG-INFO` & `cdnmon-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdnmon
-Version: 0.2.4
+Version: 0.2.5
 Summary: 
 Author: Yihang Wang
 Author-email: wangyihanger@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

