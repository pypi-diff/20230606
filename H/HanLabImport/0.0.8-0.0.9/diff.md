# Comparing `tmp/HanLabImport-0.0.8.tar.gz` & `tmp/HanLabImport-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HanLabImport-0.0.8.tar", last modified: Wed May 31 21:11:46 2023, max compression
+gzip compressed data, was "HanLabImport-0.0.9.tar", last modified: Thu Jun  1 16:00:28 2023, max compression
```

## Comparing `HanLabImport-0.0.8.tar` & `HanLabImport-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:11:46.443028 HanLabImport-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:11:46.443028 HanLabImport-0.0.8/HanLabImport/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-31 21:11:35.000000 HanLabImport-0.0.8/HanLabImport/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:11:46.443028 HanLabImport-0.0.8/HanLabImport/config/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-31 21:11:35.000000 HanLabImport-0.0.8/HanLabImport/config/HanLab.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-31 21:11:35.000000 HanLabImport-0.0.8/HanLabImport/io.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 21:11:35.000000 HanLabImport-0.0.8/HanLabImport/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 21:11:46.443028 HanLabImport-0.0.8/HanLabImport.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-31 21:11:46.000000 HanLabImport-0.0.8/HanLabImport.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-31 21:11:46.000000 HanLabImport-0.0.8/HanLabImport.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 21:11:46.000000 HanLabImport-0.0.8/HanLabImport.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-31 21:11:46.000000 HanLabImport-0.0.8/HanLabImport.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-31 21:11:46.000000 HanLabImport-0.0.8/HanLabImport.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-31 21:11:35.000000 HanLabImport-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-31 21:11:46.443028 HanLabImport-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-31 21:11:35.000000 HanLabImport-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-31 21:11:35.000000 HanLabImport-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 21:11:46.443028 HanLabImport-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-31 21:11:35.000000 HanLabImport-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:00:28.312106 HanLabImport-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:00:28.312106 HanLabImport-0.0.9/HanLabImport/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-01 16:00:17.000000 HanLabImport-0.0.9/HanLabImport/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:00:28.312106 HanLabImport-0.0.9/HanLabImport/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-01 16:00:17.000000 HanLabImport-0.0.9/HanLabImport/config/HanLab.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-01 16:00:17.000000 HanLabImport-0.0.9/HanLabImport/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 16:00:17.000000 HanLabImport-0.0.9/HanLabImport/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:00:28.312106 HanLabImport-0.0.9/HanLabImport.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-01 16:00:28.000000 HanLabImport-0.0.9/HanLabImport.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-01 16:00:28.000000 HanLabImport-0.0.9/HanLabImport.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 16:00:28.000000 HanLabImport-0.0.9/HanLabImport.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-01 16:00:28.000000 HanLabImport-0.0.9/HanLabImport.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-01 16:00:28.000000 HanLabImport-0.0.9/HanLabImport.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-01 16:00:17.000000 HanLabImport-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-01 16:00:28.312106 HanLabImport-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-01 16:00:17.000000 HanLabImport-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-01 16:00:17.000000 HanLabImport-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 16:00:28.312106 HanLabImport-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-01 16:00:17.000000 HanLabImport-0.0.9/setup.py
```

### Comparing `HanLabImport-0.0.8/HanLabImport/config/HanLab.cfg` & `HanLabImport-0.0.9/HanLabImport/config/HanLab.cfg`

 * *Files identical despite different names*

### Comparing `HanLabImport-0.0.8/HanLabImport/io.py` & `HanLabImport-0.0.9/HanLabImport/io.py`

 * *Files identical despite different names*

### Comparing `HanLabImport-0.0.8/HanLabImport.egg-info/PKG-INFO` & `HanLabImport-0.0.9/HanLabImport.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HanLabImport
-Version: 0.0.8
+Version: 0.0.9
 Summary: Import tools for DNPLab specific to the Han Lab
 Home-page: https://github.com/Bridge12Technologies/HanLabImport
 Author: Thorsten Maly
 Author-email: tmaly@bridge12.com
 Project-URL: Tracker, https://github.com/Bridge12Technologies/HanLabImport/issues
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `HanLabImport-0.0.8/LICENSE` & `HanLabImport-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `HanLabImport-0.0.8/PKG-INFO` & `HanLabImport-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HanLabImport
-Version: 0.0.8
+Version: 0.0.9
 Summary: Import tools for DNPLab specific to the Han Lab
 Home-page: https://github.com/Bridge12Technologies/HanLabImport
 Author: Thorsten Maly
 Author-email: tmaly@bridge12.com
 Project-URL: Tracker, https://github.com/Bridge12Technologies/HanLabImport/issues
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `HanLabImport-0.0.8/README.md` & `HanLabImport-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `HanLabImport-0.0.8/setup.py` & `HanLabImport-0.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     long_description_content_type="text/markdown",
     author="Thorsten Maly",
     author_email="tmaly@bridge12.com",
     python_requires=">=3.10",
     install_requires=[
         "numpy>=1.24",
     ],
-    data_files=[('HanLabImport', ['HanLabImport/config/HanLab.cfg'])],
+    # data_files=[('HanLabImport', ['HanLabImport/config/HanLab.cfg'])],
+    package_data={"HanLabImport": ["config/HanLab.cfg"]},
     packages=setuptools.find_packages(),
     url="https://github.com/Bridge12Technologies/HanLabImport",
     project_urls={
         "Tracker": "https://github.com/Bridge12Technologies/HanLabImport/issues"
     },
 )
```

