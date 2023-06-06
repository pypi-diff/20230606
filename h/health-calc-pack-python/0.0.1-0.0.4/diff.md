# Comparing `tmp/health-calc-pack-python-0.0.1.tar.gz` & `tmp/health-calc-pack-python-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "health-calc-pack-python-0.0.1.tar", last modified: Mon Jun  5 20:50:55 2023, max compression
+gzip compressed data, was "health-calc-pack-python-0.0.4.tar", last modified: Tue Jun  6 00:29:55 2023, max compression
```

## Comparing `health-calc-pack-python-0.0.1.tar` & `health-calc-pack-python-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:50:55.866701 health-calc-pack-python-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-05 20:50:55.866701 health-calc-pack-python-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-05 20:50:31.000000 health-calc-pack-python-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-05 20:50:31.000000 health-calc-pack-python-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 20:50:55.866701 health-calc-pack-python-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:50:55.862701 health-calc-pack-python-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:50:55.866701 health-calc-pack-python-0.0.1/src/health_calc_pack_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-05 20:50:55.000000 health-calc-pack-python-0.0.1/src/health_calc_pack_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-05 20:50:55.000000 health-calc-pack-python-0.0.1/src/health_calc_pack_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 20:50:55.000000 health-calc-pack-python-0.0.1/src/health_calc_pack_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-05 20:50:55.000000 health-calc-pack-python-0.0.1/src/health_calc_pack_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:50:55.866701 health-calc-pack-python-0.0.1/src/person/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-05 20:50:31.000000 health-calc-pack-python-0.0.1/src/person/Person.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 20:50:31.000000 health-calc-pack-python-0.0.1/src/person/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:50:55.866701 health-calc-pack-python-0.0.1/src/test/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-06-05 20:50:31.000000 health-calc-pack-python-0.0.1/src/test/test_Person.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:29:55.682255 health-calc-pack-python-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-06 00:29:55.682255 health-calc-pack-python-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-06 00:29:31.000000 health-calc-pack-python-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-06 00:29:31.000000 health-calc-pack-python-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 00:29:55.682255 health-calc-pack-python-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:29:55.678255 health-calc-pack-python-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:29:55.682255 health-calc-pack-python-0.0.4/src/health_calc_pack_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-06 00:29:55.000000 health-calc-pack-python-0.0.4/src/health_calc_pack_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-06 00:29:55.000000 health-calc-pack-python-0.0.4/src/health_calc_pack_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 00:29:55.000000 health-calc-pack-python-0.0.4/src/health_calc_pack_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-06 00:29:55.000000 health-calc-pack-python-0.0.4/src/health_calc_pack_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:29:55.682255 health-calc-pack-python-0.0.4/src/person/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-06 00:29:31.000000 health-calc-pack-python-0.0.4/src/person/Person.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 00:29:31.000000 health-calc-pack-python-0.0.4/src/person/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:29:55.682255 health-calc-pack-python-0.0.4/src/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-06 00:29:31.000000 health-calc-pack-python-0.0.4/src/test/test_Person.py
```

### Comparing `health-calc-pack-python-0.0.1/PKG-INFO` & `health-calc-pack-python-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: health-calc-pack-python
-Version: 0.0.1
+Version: 0.0.4
 Summary: Health calculations package
 Author-email: Nilton Fernandes <niltonfernandesj@gmail.com>
 Project-URL: Homepage, https://github.com/niltonfernandesj/health-calc-pack-python
 Project-URL: Bug Tracker, https://github.com/niltonfernandesj/health-calc-pack-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `health-calc-pack-python-0.0.1/pyproject.toml` & `health-calc-pack-python-0.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "health-calc-pack-python"
-version = "0.0.1"
+version = "0.0.4"
 authors = [
   { name="Nilton Fernandes", email="niltonfernandesj@gmail.com" },
 ]
 description = "Health calculations package"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `health-calc-pack-python-0.0.1/src/health_calc_pack_python.egg-info/PKG-INFO` & `health-calc-pack-python-0.0.4/src/health_calc_pack_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: health-calc-pack-python
-Version: 0.0.1
+Version: 0.0.4
 Summary: Health calculations package
 Author-email: Nilton Fernandes <niltonfernandesj@gmail.com>
 Project-URL: Homepage, https://github.com/niltonfernandesj/health-calc-pack-python
 Project-URL: Bug Tracker, https://github.com/niltonfernandesj/health-calc-pack-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

