# Comparing `tmp/clappform-2.6.0.tar.gz` & `tmp/clappform-3.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clappform-2.6.0.tar", last modified: Fri Mar  3 08:24:08 2023, max compression
+gzip compressed data, was "clappform-3.0.0a2.tar", last modified: Tue Jun  6 12:26:01 2023, max compression
```

## Comparing `clappform-2.6.0.tar` & `clappform-3.0.0a2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 08:24:08.930722 clappform-2.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-03 08:23:59.000000 clappform-2.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-03-03 08:24:08.930722 clappform-2.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-03-03 08:23:59.000000 clappform-2.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-03-03 08:23:59.000000 clappform-2.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-03 08:24:08.930722 clappform-2.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 08:24:08.926722 clappform-2.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 08:24:08.930722 clappform-2.6.0/src/clappform/
--rw-r--r--   0 runner    (1001) docker     (123)    54498 2023-03-03 08:23:59.000000 clappform-2.6.0/src/clappform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13251 2023-03-03 08:23:59.000000 clappform-2.6.0/src/clappform/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-03-03 08:23:59.000000 clappform-2.6.0/src/clappform/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 08:24:08.930722 clappform-2.6.0/src/clappform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-03-03 08:24:08.000000 clappform-2.6.0/src/clappform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-03-03 08:24:08.000000 clappform-2.6.0/src/clappform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 08:24:08.000000 clappform-2.6.0/src/clappform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-03 08:24:08.000000 clappform-2.6.0/src/clappform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-03 08:24:08.000000 clappform-2.6.0/src/clappform.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:26:01.975703 clappform-3.0.0a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-06 12:25:46.000000 clappform-3.0.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-06 12:26:01.975703 clappform-3.0.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-06 12:25:46.000000 clappform-3.0.0a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-06 12:25:46.000000 clappform-3.0.0a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 12:26:01.975703 clappform-3.0.0a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:26:01.975703 clappform-3.0.0a2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:26:01.975703 clappform-3.0.0a2/src/clappform/
+-rw-r--r--   0 runner    (1001) docker     (123)    22106 2023-06-06 12:25:46.000000 clappform-3.0.0a2/src/clappform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21744 2023-06-06 12:25:46.000000 clappform-3.0.0a2/src/clappform/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-06 12:25:46.000000 clappform-3.0.0a2/src/clappform/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:26:01.975703 clappform-3.0.0a2/src/clappform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-06 12:26:01.000000 clappform-3.0.0a2/src/clappform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-06-06 12:26:01.000000 clappform-3.0.0a2/src/clappform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 12:26:01.000000 clappform-3.0.0a2/src/clappform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-06 12:26:01.000000 clappform-3.0.0a2/src/clappform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-06 12:26:01.000000 clappform-3.0.0a2/src/clappform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-06 12:25:46.000000 clappform-3.0.0a2/src/debug.py
```

### Comparing `clappform-2.6.0/LICENSE` & `clappform-3.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `clappform-2.6.0/PKG-INFO` & `clappform-3.0.0a2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clappform
-Version: 2.6.0
+Version: 3.0.0a2
 Summary: Clappform Python API wrapper
 Author-email: "Clappform B.V." <info@clappform.com>
 Project-URL: Documentation, https://clappform.readthedocs.io
 Project-URL: Source, https://github.com/ClappFormOrg/clappform-python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clappform-2.6.0/README.md` & `clappform-3.0.0a2/README.md`

 * *Files identical despite different names*

### Comparing `clappform-2.6.0/pyproject.toml` & `clappform-3.0.0a2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "clappform"
-version = "2.6.0"
+version = "3.0.0-alpha.2"
 authors= [
     { name="Clappform B.V.", email="info@clappform.com" },
 ]
 description = "Clappform Python API wrapper"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "requests==2.28.1",
+    "requests==2.31.0",
     "Cerberus==1.3.4",
     "pandas==1.5.2"
 ]
 
 [project.urls]
 "Documentation" = "https://clappform.readthedocs.io"
 "Source" = "https://github.com/ClappFormOrg/clappform-python"
@@ -50,14 +50,16 @@
                      # the root of the project
 )
 '''
 
 [tool.pylint]
 max-line-length = 88
 disable = [
+    "C0301", # (line-too-long)
+    "C0116", # (missing-function-docstring)
     "C0103", # (invalid-name)
     "R0902", # (too-many-instance-attributes)
     "R0913", # (too-many-arguments)
     "R0904", # (too-many-public-methods)
     "R0903", # (too-few-public-methods)
     "C0302", # (too-many-lines)
 ]
```

### Comparing `clappform-2.6.0/src/clappform.egg-info/PKG-INFO` & `clappform-3.0.0a2/src/clappform.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clappform
-Version: 2.6.0
+Version: 3.0.0a2
 Summary: Clappform Python API wrapper
 Author-email: "Clappform B.V." <info@clappform.com>
 Project-URL: Documentation, https://clappform.readthedocs.io
 Project-URL: Source, https://github.com/ClappFormOrg/clappform-python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

