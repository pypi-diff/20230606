# Comparing `tmp/error-parity-0.1.0.tar.gz` & `tmp/error-parity-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "error-parity-0.1.0.tar", last modified: Tue Jun  6 11:03:45 2023, max compression
+gzip compressed data, was "error-parity-0.1.1.tar", last modified: Tue Jun  6 11:07:27 2023, max compression
```

## Comparing `error-parity-0.1.0.tar` & `error-parity-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:03:45.165179 error-parity-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-06 11:03:33.000000 error-parity-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-06 11:03:33.000000 error-parity-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-06-06 11:03:45.165179 error-parity-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-06 11:03:33.000000 error-parity-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:03:45.161179 error-parity-0.1.0/error_parity/
--rwxr-xr-x   0 runner    (1001) docker     (123)       93 2023-06-06 11:03:33.000000 error-parity-0.1.0/error_parity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-06 11:03:33.000000 error-parity-0.1.0/error_parity/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    16548 2023-06-06 11:03:33.000000 error-parity-0.1.0/error_parity/classifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16492 2023-06-06 11:03:33.000000 error-parity-0.1.0/error_parity/cvxpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15143 2023-06-06 11:03:33.000000 error-parity-0.1.0/error_parity/equal_odds.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-06-06 11:03:33.000000 error-parity-0.1.0/error_parity/roc_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:03:45.161179 error-parity-0.1.0/error_parity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-06-06 11:03:45.000000 error-parity-0.1.0/error_parity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-06 11:03:45.000000 error-parity-0.1.0/error_parity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 11:03:45.000000 error-parity-0.1.0/error_parity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-06 11:03:45.000000 error-parity-0.1.0/error_parity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-06 11:03:45.000000 error-parity-0.1.0/error_parity.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:03:45.161179 error-parity-0.1.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-06 11:03:33.000000 error-parity-0.1.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-06 11:03:33.000000 error-parity-0.1.0/requirements/main.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-06 11:03:33.000000 error-parity-0.1.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 11:03:45.165179 error-parity-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-06 11:03:33.000000 error-parity-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:03:45.165179 error-parity-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 11:03:33.000000 error-parity-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-06 11:03:33.000000 error-parity-0.1.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-06 11:03:33.000000 error-parity-0.1.0/tests/test_equal_odds.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:07:27.726400 error-parity-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-06 11:07:14.000000 error-parity-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-06 11:07:14.000000 error-parity-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-06-06 11:07:27.726400 error-parity-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-06 11:07:14.000000 error-parity-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:07:27.722401 error-parity-0.1.1/error_parity/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       93 2023-06-06 11:07:14.000000 error-parity-0.1.1/error_parity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-06 11:07:14.000000 error-parity-0.1.1/error_parity/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16548 2023-06-06 11:07:14.000000 error-parity-0.1.1/error_parity/classifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16492 2023-06-06 11:07:14.000000 error-parity-0.1.1/error_parity/cvxpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15143 2023-06-06 11:07:14.000000 error-parity-0.1.1/error_parity/equal_odds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-06-06 11:07:14.000000 error-parity-0.1.1/error_parity/roc_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:07:27.726400 error-parity-0.1.1/error_parity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-06-06 11:07:27.000000 error-parity-0.1.1/error_parity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-06 11:07:27.000000 error-parity-0.1.1/error_parity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 11:07:27.000000 error-parity-0.1.1/error_parity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-06 11:07:27.000000 error-parity-0.1.1/error_parity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-06 11:07:27.000000 error-parity-0.1.1/error_parity.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:07:27.726400 error-parity-0.1.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-06 11:07:14.000000 error-parity-0.1.1/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-06 11:07:14.000000 error-parity-0.1.1/requirements/main.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-06 11:07:14.000000 error-parity-0.1.1/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 11:07:27.726400 error-parity-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-06 11:07:14.000000 error-parity-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:07:27.726400 error-parity-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 11:07:14.000000 error-parity-0.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-06-06 11:07:14.000000 error-parity-0.1.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-06 11:07:14.000000 error-parity-0.1.1/tests/test_equal_odds.py
```

### Comparing `error-parity-0.1.0/LICENSE` & `error-parity-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `error-parity-0.1.0/PKG-INFO` & `error-parity-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error-parity
-Version: 0.1.0
+Version: 0.1.1
 Summary: Achieve error-rate parity between protected groups for any predictor
 Home-page: https://github.com/AndreFCruz/error-parity
 Author: AndreFCruz
 License: MIT
 Keywords: ml,optimization,fairness,error-parity,equal-odds
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `error-parity-0.1.0/README.md` & `error-parity-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `error-parity-0.1.0/error_parity/classifiers.py` & `error-parity-0.1.1/error_parity/classifiers.py`

 * *Files identical despite different names*

### Comparing `error-parity-0.1.0/error_parity/cvxpy_utils.py` & `error-parity-0.1.1/error_parity/cvxpy_utils.py`

 * *Files identical despite different names*

### Comparing `error-parity-0.1.0/error_parity/equal_odds.py` & `error-parity-0.1.1/error_parity/equal_odds.py`

 * *Files identical despite different names*

### Comparing `error-parity-0.1.0/error_parity/roc_utils.py` & `error-parity-0.1.1/error_parity/roc_utils.py`

 * *Files identical despite different names*

### Comparing `error-parity-0.1.0/error_parity.egg-info/PKG-INFO` & `error-parity-0.1.1/error_parity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error-parity
-Version: 0.1.0
+Version: 0.1.1
 Summary: Achieve error-rate parity between protected groups for any predictor
 Home-page: https://github.com/AndreFCruz/error-parity
 Author: AndreFCruz
 License: MIT
 Keywords: ml,optimization,fairness,error-parity,equal-odds
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `error-parity-0.1.0/setup.py` & `error-parity-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `error-parity-0.1.0/tests/conftest.py` & `error-parity-0.1.1/tests/conftest.py`

 * *Files identical despite different names*

