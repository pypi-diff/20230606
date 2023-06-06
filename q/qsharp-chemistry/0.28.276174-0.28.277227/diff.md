# Comparing `tmp/qsharp-chemistry-0.28.276174.tar.gz` & `tmp/qsharp-chemistry-0.28.277227.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qsharp-chemistry-0.28.276174.tar", last modified: Fri Jun  2 00:31:57 2023, max compression
+gzip compressed data, was "qsharp-chemistry-0.28.277227.tar", last modified: Mon Jun  5 21:41:56 2023, max compression
```

## Comparing `qsharp-chemistry-0.28.276174.tar` & `qsharp-chemistry-0.28.277227.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 00:31:57.657759 qsharp-chemistry-0.28.276174/
--rw-rw-rw-   0        0        0     2898 2023-06-02 00:31:57.657759 qsharp-chemistry-0.28.276174/PKG-INFO
--rw-rw-rw-   0        0        0     2432 2023-06-02 00:12:27.000000 qsharp-chemistry-0.28.276174/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 00:31:57.642148 qsharp-chemistry-0.28.276174/qsharp/
-drwxrwxrwx   0        0        0        0 2023-06-02 00:31:57.657759 qsharp-chemistry-0.28.276174/qsharp/chemistry/
--rw-rw-rw-   0        0        0     7166 2023-06-02 00:12:27.000000 qsharp-chemistry-0.28.276174/qsharp/chemistry/__init__.py
--rw-rw-rw-   0        0        0      268 2023-06-02 00:31:56.000000 qsharp-chemistry-0.28.276174/qsharp/chemistry/version.py
-drwxrwxrwx   0        0        0        0 2023-06-02 00:31:57.657759 qsharp-chemistry-0.28.276174/qsharp/tests/
--rw-rw-rw-   0        0        0        0 2023-06-02 00:12:27.000000 qsharp-chemistry-0.28.276174/qsharp/tests/__init__.py
--rw-rw-rw-   0        0        0     2768 2023-06-02 00:12:27.000000 qsharp-chemistry-0.28.276174/qsharp/tests/test_chemistry.py
-drwxrwxrwx   0        0        0        0 2023-06-02 00:31:57.657759 qsharp-chemistry-0.28.276174/qsharp_chemistry.egg-info/
--rw-rw-rw-   0        0        0     2898 2023-06-02 00:31:57.000000 qsharp-chemistry-0.28.276174/qsharp_chemistry.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      330 2023-06-02 00:31:57.000000 qsharp-chemistry-0.28.276174/qsharp_chemistry.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 00:31:57.000000 qsharp-chemistry-0.28.276174/qsharp_chemistry.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-06-02 00:31:57.000000 qsharp-chemistry-0.28.276174/qsharp_chemistry.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-02 00:31:57.000000 qsharp-chemistry-0.28.276174/qsharp_chemistry.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 00:31:57.657759 qsharp-chemistry-0.28.276174/setup.cfg
--rw-rw-rw-   0        0        0     2148 2023-06-02 00:12:27.000000 qsharp-chemistry-0.28.276174/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 21:41:56.944831 qsharp-chemistry-0.28.277227/
+-rw-rw-rw-   0        0        0     2898 2023-06-05 21:41:56.944831 qsharp-chemistry-0.28.277227/PKG-INFO
+-rw-rw-rw-   0        0        0     2432 2023-06-05 21:23:52.000000 qsharp-chemistry-0.28.277227/README.md
+drwxrwxrwx   0        0        0        0 2023-06-05 21:41:56.944831 qsharp-chemistry-0.28.277227/qsharp/
+drwxrwxrwx   0        0        0        0 2023-06-05 21:41:56.944831 qsharp-chemistry-0.28.277227/qsharp/chemistry/
+-rw-rw-rw-   0        0        0     7166 2023-06-05 21:23:52.000000 qsharp-chemistry-0.28.277227/qsharp/chemistry/__init__.py
+-rw-rw-rw-   0        0        0      268 2023-06-05 21:41:56.000000 qsharp-chemistry-0.28.277227/qsharp/chemistry/version.py
+drwxrwxrwx   0        0        0        0 2023-06-05 21:41:56.944831 qsharp-chemistry-0.28.277227/qsharp/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-05 21:23:52.000000 qsharp-chemistry-0.28.277227/qsharp/tests/__init__.py
+-rw-rw-rw-   0        0        0     2768 2023-06-05 21:23:52.000000 qsharp-chemistry-0.28.277227/qsharp/tests/test_chemistry.py
+drwxrwxrwx   0        0        0        0 2023-06-05 21:41:56.944831 qsharp-chemistry-0.28.277227/qsharp_chemistry.egg-info/
+-rw-rw-rw-   0        0        0     2898 2023-06-05 21:41:56.000000 qsharp-chemistry-0.28.277227/qsharp_chemistry.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      330 2023-06-05 21:41:56.000000 qsharp-chemistry-0.28.277227/qsharp_chemistry.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 21:41:56.000000 qsharp-chemistry-0.28.277227/qsharp_chemistry.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-06-05 21:41:56.000000 qsharp-chemistry-0.28.277227/qsharp_chemistry.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-05 21:41:56.000000 qsharp-chemistry-0.28.277227/qsharp_chemistry.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-05 21:41:56.944831 qsharp-chemistry-0.28.277227/setup.cfg
+-rw-rw-rw-   0        0        0     2148 2023-06-05 21:23:52.000000 qsharp-chemistry-0.28.277227/setup.py
```

### Comparing `qsharp-chemistry-0.28.276174/PKG-INFO` & `qsharp-chemistry-0.28.277227/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsharp-chemistry
-Version: 0.28.276174
+Version: 0.28.277227
 Summary: Python chemistry libraries for Q#.
 Home-page: https://github.com/microsoft/QuantumLibraries
 Author: Microsoft
 Author-email: que-contacts@microsoft.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `qsharp-chemistry-0.28.276174/README.md` & `qsharp-chemistry-0.28.277227/README.md`

 * *Files identical despite different names*

### Comparing `qsharp-chemistry-0.28.276174/qsharp/chemistry/__init__.py` & `qsharp-chemistry-0.28.277227/qsharp/chemistry/__init__.py`

 * *Files identical despite different names*

### Comparing `qsharp-chemistry-0.28.276174/qsharp/tests/test_chemistry.py` & `qsharp-chemistry-0.28.277227/qsharp/tests/test_chemistry.py`

 * *Files identical despite different names*

### Comparing `qsharp-chemistry-0.28.276174/qsharp_chemistry.egg-info/PKG-INFO` & `qsharp-chemistry-0.28.277227/qsharp_chemistry.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsharp-chemistry
-Version: 0.28.276174
+Version: 0.28.277227
 Summary: Python chemistry libraries for Q#.
 Home-page: https://github.com/microsoft/QuantumLibraries
 Author: Microsoft
 Author-email: que-contacts@microsoft.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `qsharp-chemistry-0.28.276174/setup.py` & `qsharp-chemistry-0.28.277227/setup.py`

 * *Files identical despite different names*

