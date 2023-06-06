# Comparing `tmp/SimpleShape-1.3.1.tar.gz` & `tmp/SimpleShape-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimpleShape-1.3.1.tar", last modified: Tue Jun  6 14:21:41 2023, max compression
+gzip compressed data, was "SimpleShape-1.3.2.tar", last modified: Tue Jun  6 15:36:37 2023, max compression
```

## Comparing `SimpleShape-1.3.1.tar` & `SimpleShape-1.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 14:21:41.393876 SimpleShape-1.3.1/
--rw-rw-rw-   0        0        0     1069 2023-06-03 17:41:01.000000 SimpleShape-1.3.1/License.txt
--rw-rw-rw-   0        0        0     4945 2023-06-06 14:21:41.393876 SimpleShape-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     4539 2023-06-06 12:50:04.000000 SimpleShape-1.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 14:21:41.378250 SimpleShape-1.3.1/SimpleShape/
--rw-rw-rw-   0        0        0      780 2023-06-06 06:03:25.000000 SimpleShape-1.3.1/SimpleShape/Example.py
--rw-rw-rw-   0        0        0    14010 2023-06-06 11:28:46.000000 SimpleShape-1.3.1/SimpleShape/SimpleShape.py
--rw-rw-rw-   0        0        0        2 2023-06-03 17:34:06.000000 SimpleShape-1.3.1/SimpleShape/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 14:21:41.393876 SimpleShape-1.3.1/SimpleShape.egg-info/
--rw-rw-rw-   0        0        0     4945 2023-06-06 14:21:41.000000 SimpleShape-1.3.1/SimpleShape.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      254 2023-06-06 14:21:41.000000 SimpleShape-1.3.1/SimpleShape.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 14:21:41.000000 SimpleShape-1.3.1/SimpleShape.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-06 14:21:41.000000 SimpleShape-1.3.1/SimpleShape.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2023-06-06 14:21:41.393876 SimpleShape-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0      974 2023-06-06 14:20:42.000000 SimpleShape-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 15:36:37.144811 SimpleShape-1.3.2/
+-rw-rw-rw-   0        0        0     1069 2023-06-03 17:41:01.000000 SimpleShape-1.3.2/License.txt
+-rw-rw-rw-   0        0        0     4945 2023-06-06 15:36:37.144811 SimpleShape-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4539 2023-06-06 12:50:04.000000 SimpleShape-1.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 15:36:37.129231 SimpleShape-1.3.2/SimpleShape/
+-rw-rw-rw-   0        0        0      780 2023-06-06 06:03:25.000000 SimpleShape-1.3.2/SimpleShape/Example.py
+-rw-rw-rw-   0        0        0    14010 2023-06-06 11:28:46.000000 SimpleShape-1.3.2/SimpleShape/SimpleShape.py
+-rw-rw-rw-   0        0        0        2 2023-06-03 17:34:06.000000 SimpleShape-1.3.2/SimpleShape/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 15:36:37.144811 SimpleShape-1.3.2/SimpleShape.egg-info/
+-rw-rw-rw-   0        0        0     4945 2023-06-06 15:36:36.000000 SimpleShape-1.3.2/SimpleShape.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2023-06-06 15:36:36.000000 SimpleShape-1.3.2/SimpleShape.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 15:36:36.000000 SimpleShape-1.3.2/SimpleShape.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-06 15:36:36.000000 SimpleShape-1.3.2/SimpleShape.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      115 2023-06-06 15:36:37.144811 SimpleShape-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      974 2023-06-06 15:24:47.000000 SimpleShape-1.3.2/setup.py
```

### Comparing `SimpleShape-1.3.1/License.txt` & `SimpleShape-1.3.2/License.txt`

 * *Files identical despite different names*

### Comparing `SimpleShape-1.3.1/PKG-INFO` & `SimpleShape-1.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpleShape
-Version: 1.3.1
+Version: 1.3.2
 Summary: A simple package for creating geometric objects
 Author: Tilen Žel
 Author-email: tilen.zel@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `SimpleShape-1.3.1/README.md` & `SimpleShape-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `SimpleShape-1.3.1/SimpleShape/Example.py` & `SimpleShape-1.3.2/SimpleShape/Example.py`

 * *Files identical despite different names*

### Comparing `SimpleShape-1.3.1/SimpleShape/SimpleShape.py` & `SimpleShape-1.3.2/SimpleShape/SimpleShape.py`

 * *Files identical despite different names*

### Comparing `SimpleShape-1.3.1/SimpleShape.egg-info/PKG-INFO` & `SimpleShape-1.3.2/SimpleShape.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpleShape
-Version: 1.3.1
+Version: 1.3.2
 Summary: A simple package for creating geometric objects
 Author: Tilen Žel
 Author-email: tilen.zel@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

