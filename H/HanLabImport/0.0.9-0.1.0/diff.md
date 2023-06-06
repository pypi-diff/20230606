# Comparing `tmp/HanLabImport-0.0.9.tar.gz` & `tmp/HanLabImport-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HanLabImport-0.0.9.tar", last modified: Thu Jun  1 16:00:28 2023, max compression
+gzip compressed data, was "HanLabImport-0.1.0.tar", last modified: Tue Jun  6 12:28:21 2023, max compression
```

## Comparing `HanLabImport-0.0.9.tar` & `HanLabImport-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:00:28.312106 HanLabImport-0.0.9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:00:28.312106 HanLabImport-0.0.9/HanLabImport/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-01 16:00:17.000000 HanLabImport-0.0.9/HanLabImport/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:00:28.312106 HanLabImport-0.0.9/HanLabImport/config/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-01 16:00:17.000000 HanLabImport-0.0.9/HanLabImport/config/HanLab.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-01 16:00:17.000000 HanLabImport-0.0.9/HanLabImport/io.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 16:00:17.000000 HanLabImport-0.0.9/HanLabImport/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:00:28.312106 HanLabImport-0.0.9/HanLabImport.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-01 16:00:28.000000 HanLabImport-0.0.9/HanLabImport.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-01 16:00:28.000000 HanLabImport-0.0.9/HanLabImport.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 16:00:28.000000 HanLabImport-0.0.9/HanLabImport.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-01 16:00:28.000000 HanLabImport-0.0.9/HanLabImport.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-01 16:00:28.000000 HanLabImport-0.0.9/HanLabImport.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-01 16:00:17.000000 HanLabImport-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-01 16:00:28.312106 HanLabImport-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-01 16:00:17.000000 HanLabImport-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-01 16:00:17.000000 HanLabImport-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 16:00:28.312106 HanLabImport-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-01 16:00:17.000000 HanLabImport-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:28:21.867796 HanLabImport-0.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:28:21.867796 HanLabImport-0.1.0/HanLabImport/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-06 12:28:11.000000 HanLabImport-0.1.0/HanLabImport/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:28:21.867796 HanLabImport-0.1.0/HanLabImport/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-06 12:28:11.000000 HanLabImport-0.1.0/HanLabImport/config/HanLab.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-06 12:28:11.000000 HanLabImport-0.1.0/HanLabImport/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-06 12:28:11.000000 HanLabImport-0.1.0/HanLabImport/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-06 12:28:11.000000 HanLabImport-0.1.0/HanLabImport/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-06 12:28:11.000000 HanLabImport-0.1.0/HanLabImport/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:28:21.867796 HanLabImport-0.1.0/HanLabImport.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-06 12:28:21.000000 HanLabImport-0.1.0/HanLabImport.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-06 12:28:21.000000 HanLabImport-0.1.0/HanLabImport.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 12:28:21.000000 HanLabImport-0.1.0/HanLabImport.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-06 12:28:21.000000 HanLabImport-0.1.0/HanLabImport.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-06 12:28:21.000000 HanLabImport-0.1.0/HanLabImport.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-06 12:28:11.000000 HanLabImport-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-06-06 12:28:21.867796 HanLabImport-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-06 12:28:11.000000 HanLabImport-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-06 12:28:11.000000 HanLabImport-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 12:28:21.867796 HanLabImport-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-06 12:28:11.000000 HanLabImport-0.1.0/setup.py
```

### Comparing `HanLabImport-0.0.9/HanLabImport/config/HanLab.cfg` & `HanLabImport-0.1.0/HanLabImport/config/HanLab.cfg`

 * *Files identical despite different names*

### Comparing `HanLabImport-0.0.9/HanLabImport/io.py` & `HanLabImport-0.1.0/HanLabImport/io.py`

 * *Files identical despite different names*

### Comparing `HanLabImport-0.0.9/HanLabImport.egg-info/PKG-INFO` & `HanLabImport-0.1.0/HanLabImport.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: HanLabImport
-Version: 0.0.9
+Version: 0.1.0
 Summary: Import tools for DNPLab specific to the Han Lab
 Home-page: https://github.com/Bridge12Technologies/HanLabImport
 Author: Thorsten Maly
 Author-email: tmaly@bridge12.com
 Project-URL: Tracker, https://github.com/Bridge12Technologies/HanLabImport/issues
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![http://dnplab.net](https://img.shields.io/pypi/v/dnplab)](https://pypi.org/project/dnplab/)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dnplab)](https://www.python.org/downloads/)
-[![Downloads](https://pepy.tech/badge/dnplab/month)](https://pepy.tech/project/dnplab)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/HanLabImport)](https://www.python.org/downloads/)
+[![Downloads](https://static.pepy.tech/badge/hanlabimport)](https://pepy.tech/project/hanlabimport)
 
 HanLabImport is a support package for DNPLab to import data recorded in the lab of Prof. Song-I Han.
 
 For more information about DNPLab vist: www.dnplab.org
 
 # Features
```

### Comparing `HanLabImport-0.0.9/LICENSE` & `HanLabImport-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `HanLabImport-0.0.9/PKG-INFO` & `HanLabImport-0.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: HanLabImport
-Version: 0.0.9
+Version: 0.1.0
 Summary: Import tools for DNPLab specific to the Han Lab
 Home-page: https://github.com/Bridge12Technologies/HanLabImport
 Author: Thorsten Maly
 Author-email: tmaly@bridge12.com
 Project-URL: Tracker, https://github.com/Bridge12Technologies/HanLabImport/issues
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![http://dnplab.net](https://img.shields.io/pypi/v/dnplab)](https://pypi.org/project/dnplab/)
-[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dnplab)](https://www.python.org/downloads/)
-[![Downloads](https://pepy.tech/badge/dnplab/month)](https://pepy.tech/project/dnplab)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/HanLabImport)](https://www.python.org/downloads/)
+[![Downloads](https://static.pepy.tech/badge/hanlabimport)](https://pepy.tech/project/hanlabimport)
 
 HanLabImport is a support package for DNPLab to import data recorded in the lab of Prof. Song-I Han.
 
 For more information about DNPLab vist: www.dnplab.org
 
 # Features
```

### Comparing `HanLabImport-0.0.9/setup.py` & `HanLabImport-0.1.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     long_description_content_type="text/markdown",
     author="Thorsten Maly",
     author_email="tmaly@bridge12.com",
     python_requires=">=3.10",
     install_requires=[
         "numpy>=1.24",
     ],
-    # data_files=[('HanLabImport', ['HanLabImport/config/HanLab.cfg'])],
     package_data={"HanLabImport": ["config/HanLab.cfg"]},
     packages=setuptools.find_packages(),
     url="https://github.com/Bridge12Technologies/HanLabImport",
     project_urls={
         "Tracker": "https://github.com/Bridge12Technologies/HanLabImport/issues"
     },
 )
```

