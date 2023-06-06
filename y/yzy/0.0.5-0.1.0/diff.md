# Comparing `tmp/yzy-0.0.5.tar.gz` & `tmp/yzy-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yzy-0.0.5.tar", last modified: Tue Jun  6 10:21:50 2023, max compression
+gzip compressed data, was "yzy-0.1.0.tar", last modified: Tue Jun  6 11:49:34 2023, max compression
```

## Comparing `yzy-0.0.5.tar` & `yzy-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 10:21:50.797742 yzy-0.0.5/
--rw-rw-rw-   0        0        0     1073 2023-04-02 11:39:35.000000 yzy-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      805 2023-06-06 10:21:50.797742 yzy-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      288 2023-04-09 03:08:26.000000 yzy-0.0.5/README.md
--rw-rw-rw-   0        0        0      608 2023-06-06 10:20:52.000000 yzy-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-06 10:21:50.797742 yzy-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-06 10:21:50.777740 yzy-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-06-06 10:21:50.788740 yzy-0.0.5/src/yzy/
--rw-rw-rw-   0        0        0        0 2023-04-02 11:41:50.000000 yzy-0.0.5/src/yzy/__init__.py
--rw-rw-rw-   0        0        0     5660 2023-06-06 09:19:07.000000 yzy-0.0.5/src/yzy/arxiv.py
--rw-rw-rw-   0        0        0     2500 2023-06-06 09:17:59.000000 yzy-0.0.5/src/yzy/file2md.py
--rw-rw-rw-   0        0        0     1973 2023-06-06 09:18:22.000000 yzy-0.0.5/src/yzy/id2md.py
-drwxrwxrwx   0        0        0        0 2023-06-06 10:21:50.796740 yzy-0.0.5/src/yzy.egg-info/
--rw-rw-rw-   0        0        0      805 2023-06-06 10:21:50.000000 yzy-0.0.5/src/yzy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      259 2023-06-06 10:21:50.000000 yzy-0.0.5/src/yzy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 10:21:50.000000 yzy-0.0.5/src/yzy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-06-06 10:21:50.000000 yzy-0.0.5/src/yzy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-06-06 10:21:50.000000 yzy-0.0.5/src/yzy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 11:49:34.003075 yzy-0.1.0/
+-rw-rw-rw-   0        0        0     1073 2023-04-02 11:39:35.000000 yzy-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      805 2023-06-06 11:49:34.003075 yzy-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2023-04-09 03:08:26.000000 yzy-0.1.0/README.md
+-rw-rw-rw-   0        0        0      607 2023-06-06 11:47:40.000000 yzy-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-06 11:49:34.003075 yzy-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-06 11:49:33.990076 yzy-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-06 11:49:33.994075 yzy-0.1.0/src/yzy/
+-rw-rw-rw-   0        0        0        0 2023-04-02 11:41:50.000000 yzy-0.1.0/src/yzy/__init__.py
+-rw-rw-rw-   0        0        0     5660 2023-06-06 09:19:07.000000 yzy-0.1.0/src/yzy/arxiv.py
+-rw-rw-rw-   0        0        0     2500 2023-06-06 09:17:59.000000 yzy-0.1.0/src/yzy/file2md.py
+-rw-rw-rw-   0        0        0     1973 2023-06-06 09:18:22.000000 yzy-0.1.0/src/yzy/id2md.py
+drwxrwxrwx   0        0        0        0 2023-06-06 11:49:34.002074 yzy-0.1.0/src/yzy.egg-info/
+-rw-rw-rw-   0        0        0      805 2023-06-06 11:49:33.000000 yzy-0.1.0/src/yzy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      259 2023-06-06 11:49:33.000000 yzy-0.1.0/src/yzy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 11:49:33.000000 yzy-0.1.0/src/yzy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-06 11:49:33.000000 yzy-0.1.0/src/yzy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-06 11:49:33.000000 yzy-0.1.0/src/yzy.egg-info/top_level.txt
```

### Comparing `yzy-0.0.5/LICENSE` & `yzy-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yzy-0.0.5/PKG-INFO` & `yzy-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: yzy
-Version: 0.0.5
+Version: 0.1.0
 Summary: Utils
 Author-email: Zhiyuan Yang <im.crazyang@gmail.com>
 Project-URL: Homepage, https://github.com/yzy1996/Python-Code
 Project-URL: Bug Tracker, https://github.com/yzy1996/Python-Code/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # yzy
 
 各种工具
```

### Comparing `yzy-0.0.5/pyproject.toml` & `yzy-0.1.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "yzy"
-version = "0.0.5"
+version = "0.1.0"
 authors = [
   { name="Zhiyuan Yang", email="im.crazyang@gmail.com" },
 ]
 description = "Utils"
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = ">=3.8"
 dependencies =["feedparser",
-               "PyPDF2",
+               "pypdf",
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `yzy-0.0.5/src/yzy/arxiv.py` & `yzy-0.1.0/src/yzy/arxiv.py`

 * *Files identical despite different names*

### Comparing `yzy-0.0.5/src/yzy/file2md.py` & `yzy-0.1.0/src/yzy/file2md.py`

 * *Files identical despite different names*

### Comparing `yzy-0.0.5/src/yzy/id2md.py` & `yzy-0.1.0/src/yzy/id2md.py`

 * *Files identical despite different names*

### Comparing `yzy-0.0.5/src/yzy.egg-info/PKG-INFO` & `yzy-0.1.0/src/yzy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: yzy
-Version: 0.0.5
+Version: 0.1.0
 Summary: Utils
 Author-email: Zhiyuan Yang <im.crazyang@gmail.com>
 Project-URL: Homepage, https://github.com/yzy1996/Python-Code
 Project-URL: Bug Tracker, https://github.com/yzy1996/Python-Code/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # yzy
 
 各种工具
```

