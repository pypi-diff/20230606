# Comparing `tmp/exampleproject_crida-0.2.2.tar.gz` & `tmp/exampleproject_crida-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exampleproject_crida-0.2.2.tar", max compression
+gzip compressed data, was "exampleproject_crida-0.2.3.tar", max compression
```

## Comparing `exampleproject_crida-0.2.2.tar` & `exampleproject_crida-0.2.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-06-05 08:42:00.330913 exampleproject_crida-0.2.2/exampleproject_crida/__init__.py
--rw-r--r--   0        0        0      502 2023-06-05 13:28:27.012013 exampleproject_crida-0.2.2/exampleproject_crida/example_usage.py
--rw-r--r--   0        0        0      311 2023-06-05 14:09:10.802628 exampleproject_crida-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      302 2023-06-05 14:07:57.148446 exampleproject_crida-0.2.2/README_repository.md
--rw-r--r--   0        0        0      644 1970-01-01 00:00:00.000000 exampleproject_crida-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-05 08:42:00.330913 exampleproject_crida-0.2.3/exampleproject_crida/__init__.py
+-rw-r--r--   0        0        0      502 2023-06-05 13:28:27.012013 exampleproject_crida-0.2.3/exampleproject_crida/example_usage.py
+-rw-r--r--   0        0        0      313 2023-06-06 16:57:12.762003 exampleproject_crida-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      302 2023-06-05 14:07:57.148446 exampleproject_crida-0.2.3/README_repository.md
+-rw-r--r--   0        0        0      644 1970-01-01 00:00:00.000000 exampleproject_crida-0.2.3/PKG-INFO
```

### Comparing `exampleproject_crida-0.2.2/PKG-INFO` & `exampleproject_crida-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exampleproject-crida
-Version: 0.2.2
+Version: 0.2.3
 Summary: 
 Author: Sergi Mas-Pujol
 Author-email: smas@e-crida.enaire.es
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

