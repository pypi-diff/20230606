# Comparing `tmp/steganodf-0.1.2.tar.gz` & `tmp/steganodf-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steganodf-0.1.2.tar", max compression
+gzip compressed data, was "steganodf-0.1.3.tar", max compression
```

## Comparing `steganodf-0.1.2.tar` & `steganodf-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      837 2023-05-29 22:52:55.771268 steganodf-0.1.2/README.md
--rw-r--r--   0        0        0      388 2023-06-05 22:34:29.974145 steganodf-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5967 2023-06-05 22:30:27.037481 steganodf-0.1.2/steganodf/__init__.py
--rw-r--r--   0        0        0       20 2023-05-29 22:48:26.964604 steganodf-0.1.2/steganodf/__main__.py
--rw-r--r--   0        0        0     1338 1970-01-01 00:00:00.000000 steganodf-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      837 2023-05-29 22:52:55.771268 steganodf-0.1.3/README.md
+-rw-r--r--   0        0        0      447 2023-06-05 23:36:54.384112 steganodf-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5967 2023-06-05 22:30:27.037481 steganodf-0.1.3/steganodf/__init__.py
+-rw-r--r--   0        0        0     2053 2023-06-05 23:29:15.344116 steganodf-0.1.3/steganodf/__main__.py
+-rw-r--r--   0        0        0     1338 1970-01-01 00:00:00.000000 steganodf-0.1.3/PKG-INFO
```

### Comparing `steganodf-0.1.2/README.md` & `steganodf-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `steganodf-0.1.2/steganodf/__init__.py` & `steganodf-0.1.3/steganodf/__init__.py`

 * *Files identical despite different names*

### Comparing `steganodf-0.1.2/PKG-INFO` & `steganodf-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: steganodf
-Version: 0.1.2
+Version: 0.1.3
 Summary: Functions to add steganographic message to a dataframe with row permutation
 Author: Sacha Schutz
 Author-email: sacha@labsquare.org
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

