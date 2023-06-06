# Comparing `tmp/BroadSword-0.0.2.tar.gz` & `tmp/BroadSword-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BroadSword-0.0.2.tar", last modified: Tue Jun  6 18:29:18 2023, max compression
+gzip compressed data, was "BroadSword-0.1.tar", last modified: Tue Jun  6 17:57:37 2023, max compression
```

## Comparing `BroadSword-0.0.2.tar` & `BroadSword-0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:29:18.898453 BroadSword-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-06 18:29:08.000000 BroadSword-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-06 18:29:18.898453 BroadSword-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-06 18:29:08.000000 BroadSword-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-06 18:29:08.000000 BroadSword-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-06 18:29:18.898453 BroadSword-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:29:18.894453 BroadSword-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:29:18.898453 BroadSword-0.0.2/src/BroadSword/
--rw-r--r--   0 runner    (1001) docker     (123)    16575 2023-06-06 18:29:08.000000 BroadSword-0.0.2/src/BroadSword/BroadSword.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 18:29:08.000000 BroadSword-0.0.2/src/BroadSword/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 18:29:18.898453 BroadSword-0.0.2/src/BroadSword.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-06 18:29:18.000000 BroadSword-0.0.2/src/BroadSword.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-06 18:29:18.000000 BroadSword-0.0.2/src/BroadSword.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 18:29:18.000000 BroadSword-0.0.2/src/BroadSword.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-06 18:29:18.000000 BroadSword-0.0.2/src/BroadSword.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-06 18:29:18.000000 BroadSword-0.0.2/src/BroadSword.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:57:37.360304 BroadSword-0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-06 17:57:16.000000 BroadSword-0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-06 17:57:37.360304 BroadSword-0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-06 17:57:16.000000 BroadSword-0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-06 17:57:16.000000 BroadSword-0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-06 17:57:37.360304 BroadSword-0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:57:37.360304 BroadSword-0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:57:37.360304 BroadSword-0.1/src/BroadSword/
+-rw-r--r--   0 runner    (1001) docker     (123)    16575 2023-06-06 17:57:16.000000 BroadSword-0.1/src/BroadSword/BroadSword.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 17:57:16.000000 BroadSword-0.1/src/BroadSword/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:57:37.360304 BroadSword-0.1/src/BroadSword.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-06 17:57:37.000000 BroadSword-0.1/src/BroadSword.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-06 17:57:37.000000 BroadSword-0.1/src/BroadSword.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 17:57:37.000000 BroadSword-0.1/src/BroadSword.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-06 17:57:37.000000 BroadSword-0.1/src/BroadSword.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-06 17:57:37.000000 BroadSword-0.1/src/BroadSword.egg-info/top_level.txt
```

### Comparing `BroadSword-0.0.2/LICENSE` & `BroadSword-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `BroadSword-0.0.2/PKG-INFO` & `BroadSword-0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BroadSword
-Version: 0.0.2
+Version: 0.1
 Summary: Python script to broaden calculated spectra from Wien2k and compare to experimental data at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 Home-page: https://github.com/Cody-Somers/BroadSword
 Author: Cody Somers
 Author-email: cas003@usask.ca
 Project-URL: Beamline Information, https://reixs.lightsource.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `BroadSword-0.0.2/setup.cfg` & `BroadSword-0.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = BroadSword
-version = 0.0.2
+version = 0.1
 author = Cody Somers
 author_email = cas003@usask.ca
 description = Python script to broaden calculated spectra from Wien2k and compare to experimental data at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Cody-Somers/BroadSword
 project_urls = 
@@ -16,14 +16,15 @@
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.6
 install_requires = 
+	ctypes
 	numpy
 	pandas
 	bokeh>=2.3.3,<3
 
 [options.packages.find]
 where = src
```

### Comparing `BroadSword-0.0.2/src/BroadSword/BroadSword.py` & `BroadSword-0.1/src/BroadSword/BroadSword.py`

 * *Files identical despite different names*

### Comparing `BroadSword-0.0.2/src/BroadSword.egg-info/PKG-INFO` & `BroadSword-0.1/src/BroadSword.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BroadSword
-Version: 0.0.2
+Version: 0.1
 Summary: Python script to broaden calculated spectra from Wien2k and compare to experimental data at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 Home-page: https://github.com/Cody-Somers/BroadSword
 Author: Cody Somers
 Author-email: cas003@usask.ca
 Project-URL: Beamline Information, https://reixs.lightsource.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

