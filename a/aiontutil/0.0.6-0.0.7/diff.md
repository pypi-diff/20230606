# Comparing `tmp/aiontutil-0.0.6.tar.gz` & `tmp/aiontutil-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiontutil-0.0.6.tar", max compression
+gzip compressed data, was "aiontutil-0.0.7.tar", max compression
```

## Comparing `aiontutil-0.0.6.tar` & `aiontutil-0.0.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      283 2023-05-08 08:27:47.285958 aiontutil-0.0.6/README.md
--rw-r--r--   0        0        0       22 2023-05-08 07:09:03.272254 aiontutil-0.0.6/aiontutil/__init__.py
--rw-r--r--   0        0        0     5234 2023-05-16 02:19:08.832054 aiontutil-0.0.6/aiontutil/signal.py
--rw-r--r--   0        0        0      355 2023-05-16 02:21:52.085449 aiontutil-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 aiontutil-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      283 2023-05-08 08:27:47.285958 aiontutil-0.0.7/README.md
+-rw-r--r--   0        0        0       22 2023-05-08 07:09:03.272254 aiontutil-0.0.7/aiontutil/__init__.py
+-rw-r--r--   0        0        0     7874 2023-06-06 06:15:36.062162 aiontutil-0.0.7/aiontutil/signal.py
+-rw-r--r--   0        0        0      355 2023-06-06 06:17:50.317571 aiontutil-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 aiontutil-0.0.7/PKG-INFO
```

### Comparing `aiontutil-0.0.6/PKG-INFO` & `aiontutil-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiontutil
-Version: 0.0.6
+Version: 0.0.7
 Summary: aiont utility package
 Author: jlan
 Author-email: jlan@aiont.io
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

