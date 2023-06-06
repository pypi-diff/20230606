# Comparing `tmp/ghastoolkit-0.3.2.tar.gz` & `tmp/ghastoolkit-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghastoolkit-0.3.2.tar", last modified: Mon Jun  5 18:46:12 2023, max compression
+gzip compressed data, was "ghastoolkit-0.4.0.tar", last modified: Tue Jun  6 19:45:04 2023, max compression
```

## Comparing `ghastoolkit-0.3.2.tar` & `ghastoolkit-0.4.0.tar`

### file list

```diff
@@ -1,50 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:12.853889 ghastoolkit-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-05 18:46:12.853889 ghastoolkit-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 18:46:12.853889 ghastoolkit-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:12.849889 ghastoolkit-0.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:12.849889 ghastoolkit-0.3.2/src/ghastoolkit/
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:12.853889 ghastoolkit-0.3.2/src/ghastoolkit/codeql/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/codeql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/codeql/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/codeql/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/codeql/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/codeql/results.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/codeql/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:12.853889 ghastoolkit-0.3.2/src/ghastoolkit/octokit/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/octokit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/octokit/codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/octokit/dependabot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/octokit/dependencygraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/octokit/github.py
--rw-r--r--   0 runner    (1001) docker     (123)    10968 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/octokit/octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/octokit/secretscanning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:12.853889 ghastoolkit-0.3.2/src/ghastoolkit/secretscanning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/secretscanning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/secretscanning/secretalerts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:12.853889 ghastoolkit-0.3.2/src/ghastoolkit/supplychain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/supplychain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/supplychain/advisories.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/supplychain/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/supplychain/dependencyalert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/src/ghastoolkit/supplychain/licensing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:12.849889 ghastoolkit-0.3.2/src/ghastoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-05 18:46:12.000000 ghastoolkit-0.3.2/src/ghastoolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-05 18:46:12.000000 ghastoolkit-0.3.2/src/ghastoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 18:46:12.000000 ghastoolkit-0.3.2/src/ghastoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-05 18:46:12.000000 ghastoolkit-0.3.2/src/ghastoolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-05 18:46:12.000000 ghastoolkit-0.3.2/src/ghastoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:46:12.853889 ghastoolkit-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/tests/test_codeqldb.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/tests/test_codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/tests/test_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/tests/test_depgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/tests/test_github.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/tests/test_licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/tests/test_octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-05 18:45:40.000000 ghastoolkit-0.3.2/tests/test_secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:45:04.397640 ghastoolkit-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-06 19:45:04.397640 ghastoolkit-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 19:45:04.397640 ghastoolkit-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:45:04.393639 ghastoolkit-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:45:04.393639 ghastoolkit-0.4.0/src/ghastoolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:45:04.393639 ghastoolkit-0.4.0/src/ghastoolkit/codeql/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/codeql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/codeql/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/codeql/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/codeql/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/codeql/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/codeql/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:45:04.397640 ghastoolkit-0.4.0/src/ghastoolkit/octokit/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/octokit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/octokit/clearlydefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/octokit/codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/octokit/dependabot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/octokit/dependencygraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/octokit/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10968 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/octokit/octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/octokit/secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:45:04.397640 ghastoolkit-0.4.0/src/ghastoolkit/secretscanning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/secretscanning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/secretscanning/secretalerts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:45:04.397640 ghastoolkit-0.4.0/src/ghastoolkit/supplychain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/supplychain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/supplychain/advisories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/supplychain/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/supplychain/dependencyalert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/src/ghastoolkit/supplychain/licensing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:45:04.393639 ghastoolkit-0.4.0/src/ghastoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-06-06 19:45:04.000000 ghastoolkit-0.4.0/src/ghastoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-06 19:45:04.000000 ghastoolkit-0.4.0/src/ghastoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 19:45:04.000000 ghastoolkit-0.4.0/src/ghastoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-06 19:45:04.000000 ghastoolkit-0.4.0/src/ghastoolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-06 19:45:04.000000 ghastoolkit-0.4.0/src/ghastoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:45:04.397640 ghastoolkit-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/tests/test_clearlydefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/tests/test_codeqldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/tests/test_codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/tests/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/tests/test_depgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/tests/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/tests/test_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/tests/test_octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-06 19:44:32.000000 ghastoolkit-0.4.0/tests/test_secretscanning.py
```

### Comparing `ghastoolkit-0.3.2/LICENSE` & `ghastoolkit-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.2/PKG-INFO` & `ghastoolkit-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.3.2
+Version: 0.4.0
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.3.2/README.md` & `ghastoolkit-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.2/pyproject.toml` & `ghastoolkit-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ghastoolkit"
-version = "0.3.2"
+version = "0.4.0"
 authors = [
   { name="GeekMasher" },
 ]
 description = "GitHub Advanced Security Python Toolkit"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `ghastoolkit-0.3.2/src/ghastoolkit/__init__.py` & `ghastoolkit-0.4.0/src/ghastoolkit/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __name__ = "ghastoolkit"
 __title__ = "GHAS Toolkit"
 
-__version__ = "0.3.2"
+__version__ = "0.4.0"
 
 __description__ = "GitHub Advanced Security Python Toolkit"
 __summary__ = """\
 GitHub Advanced Security Python Toolkit
 """
 
 __url__ = "https://github.com/GeekMasher/ghastoolkit"
```

### Comparing `ghastoolkit-0.3.2/src/ghastoolkit/__main__.py` & `ghastoolkit-0.4.0/src/ghastoolkit/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.2/src/ghastoolkit/codeql/cli.py` & `ghastoolkit-0.4.0/src/ghastoolkit/codeql/cli.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.2/src/ghastoolkit/codeql/databases.py` & `ghastoolkit-0.4.0/src/ghastoolkit/codeql/databases.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.2/src/ghastoolkit/codeql/results.py` & `ghastoolkit-0.4.0/src/ghastoolkit/codeql/results.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.2/src/ghastoolkit/octokit/codescanning.py` & `ghastoolkit-0.4.0/src/ghastoolkit/octokit/codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.2/src/ghastoolkit/octokit/dependabot.py` & `ghastoolkit-0.4.0/src/ghastoolkit/octokit/dependabot.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.2/src/ghastoolkit/octokit/github.py` & `ghastoolkit-0.4.0/src/ghastoolkit/octokit/github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.2/src/ghastoolkit/octokit/octokit.py` & `ghastoolkit-0.4.0/src/ghastoolkit/octokit/octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.2/src/ghastoolkit/octokit/secretscanning.py` & `ghastoolkit-0.4.0/src/ghastoolkit/octokit/secretscanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.2/src/ghastoolkit/secretscanning/secretalerts.py` & `ghastoolkit-0.4.0/src/ghastoolkit/secretscanning/secretalerts.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.2/src/ghastoolkit/supplychain/dependencies.py` & `ghastoolkit-0.4.0/src/ghastoolkit/supplychain/dependencies.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     namespace: Optional[str] = None
     version: Optional[str] = None
     manager: Optional[str] = None
     path: Optional[str] = None
     qualifiers: dict[str, str] = field(default_factory=dict)
 
     # Licensing information
-    licence: Optional[str] = None
+    license: Optional[str] = None
     # Security Alerts
     alerts: list[DependencyAlert] = field(default_factory=list)
 
     def getPurl(self, version: bool = True) -> str:
         """Get PURL
         https://github.com/package-url/purl-spec
         """
@@ -124,37 +124,54 @@
     def findLicenses(self, licenses: list[str]) -> "Dependencies":
         """Find Denied License"""
         regex_list = [re.compile(name_filter) for name_filter in licenses]
         return Dependencies(
             [
                 dep
                 for dep in self
-                if any(regex.search(dep.licence or "NA") for regex in regex_list)
+                if any(regex.search(dep.license or "NA") for regex in regex_list)
             ]
         )
 
     def findUnknownLicenses(
         self, licenses: Optional[list[str]] = None
     ) -> "Dependencies":
         """Find all the dependencies with no license"""
         licenses = licenses or NO_LICENSES
         return self.findLicenses(licenses)
 
     def applyLicenses(self, licenses: Licenses):
         """Given a list of licenses (Licenses) apply a license"""
         for i, dep in enumerate(self):
-            if dep.licence and dep.licence not in NO_LICENSES:
+            if dep.license and dep.license not in NO_LICENSES:
                 continue
             purl = dep.getPurl(version=False)
             dblicense = licenses.find(purl)
             if dblicense:
-                dep.licence = " OR ".join(dblicense)
+                dep.license = " OR ".join(dblicense)
+                self[i] = dep
+
+    def applyClearlyDefined(self):
+        """Reachout to Clearly Definded API, get the licenses for a component,
+        and update all the Dependencies
+        """
+        from ghastoolkit.octokit.clearlydefined import ClearlyDefined
+
+        clearly = ClearlyDefined()
+
+        for i, dep in enumerate(self):
+            if dep.license and dep.license not in NO_LICENSES:
+                continue
+            licenses = clearly.getLicenses(dep)
+            if licenses:
+                dep.license = " OR ".join(licenses)
                 self[i] = dep
 
     def contains(self, dependency: Dependency) -> bool:
+        """Contains the dependency"""
         purl = dependency.getPurl(version=False)
         for dep in self:
             if dep.name == dependency.name or dep.getPurl(version=False) == purl:
                 return True
         return False
 
     def find(self, name: str) -> Optional[Dependency]:
@@ -174,7 +191,20 @@
 
     def findNames(self, names: list[str]) -> "Dependencies":
         """Find by Name using wildcards"""
         regex_list = [re.compile(name_filter) for name_filter in names]
         return Dependencies(
             [dep for dep in self if any(regex.search(dep.name) for regex in regex_list)]
         )
+
+    def updateDependency(self, dependency: Dependency):
+        """Update a dependency in our list with the incoming information"""
+        for dep in self:
+            if dependency.name == dep.name or dependency.fullname == dep.fullname:
+                dep.__dict__.update(dependency.__dict__)
+                # self[i] = new_dep
+                break
+
+    def updateDependencies(self, dependencies: "Dependencies"):
+        """Update a list of dependencies"""
+        for dep in dependencies:
+            self.updateDependency(dep)
```

### Comparing `ghastoolkit-0.3.2/src/ghastoolkit/supplychain/dependencyalert.py` & `ghastoolkit-0.4.0/src/ghastoolkit/supplychain/dependencyalert.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.2/src/ghastoolkit/supplychain/licensing.py` & `ghastoolkit-0.4.0/src/ghastoolkit/supplychain/licensing.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.2/src/ghastoolkit.egg-info/PKG-INFO` & `ghastoolkit-0.4.0/src/ghastoolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.3.2
+Version: 0.4.0
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.3.2/src/ghastoolkit.egg-info/SOURCES.txt` & `ghastoolkit-0.4.0/src/ghastoolkit.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -11,27 +11,29 @@
 src/ghastoolkit/codeql/__init__.py
 src/ghastoolkit/codeql/cli.py
 src/ghastoolkit/codeql/consts.py
 src/ghastoolkit/codeql/databases.py
 src/ghastoolkit/codeql/results.py
 src/ghastoolkit/codeql/utils.py
 src/ghastoolkit/octokit/__init__.py
+src/ghastoolkit/octokit/clearlydefined.py
 src/ghastoolkit/octokit/codescanning.py
 src/ghastoolkit/octokit/dependabot.py
 src/ghastoolkit/octokit/dependencygraph.py
 src/ghastoolkit/octokit/github.py
 src/ghastoolkit/octokit/octokit.py
 src/ghastoolkit/octokit/secretscanning.py
 src/ghastoolkit/secretscanning/__init__.py
 src/ghastoolkit/secretscanning/secretalerts.py
 src/ghastoolkit/supplychain/__init__.py
 src/ghastoolkit/supplychain/advisories.py
 src/ghastoolkit/supplychain/dependencies.py
 src/ghastoolkit/supplychain/dependencyalert.py
 src/ghastoolkit/supplychain/licensing.py
+tests/test_clearlydefined.py
 tests/test_codeqldb.py
 tests/test_codescanning.py
 tests/test_default.py
 tests/test_dependencies.py
 tests/test_depgraph.py
 tests/test_github.py
 tests/test_licenses.py
```

### Comparing `ghastoolkit-0.3.2/tests/test_codeqldb.py` & `ghastoolkit-0.4.0/tests/test_codeqldb.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.2/tests/test_codescanning.py` & `ghastoolkit-0.4.0/tests/test_codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.2/tests/test_default.py` & `ghastoolkit-0.4.0/tests/test_default.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.2/tests/test_dependencies.py` & `ghastoolkit-0.4.0/tests/test_dependencies.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 
 from ghastoolkit import Dependencies, Dependency, Licenses
 
 
 class TestDependencies(unittest.TestCase):
     def setUp(self) -> None:
         self.deps = Dependencies()
-        self.deps.append(Dependency("urllib3", manager="pypi", licence="MIT"))
-        self.deps.append(Dependency("rich", manager="pypi", licence="NOASSERTION"))
-        self.deps.append(Dependency("pyyaml", manager="pypi", licence="GPL-3.0"))
-        self.deps.append(Dependency("pyproject-hooks", manager="pypi", licence="Apache-2.0"))
-        self.deps.append(Dependency("requests", manager="pypi", licence="GPL-2.0"))
+        self.deps.append(Dependency("urllib3", manager="pypi", license="MIT"))
+        self.deps.append(Dependency("rich", manager="pypi", license="NOASSERTION"))
+        self.deps.append(Dependency("pyyaml", manager="pypi", license="GPL-3.0"))
+        self.deps.append(Dependency("pyproject-hooks", manager="pypi", license="Apache-2.0"))
+        self.deps.append(Dependency("requests", manager="pypi", license="GPL-2.0"))
         return super().setUp()
 
     def test_license(self):
         mit = self.deps.findLicenses(["MIT"])
         self.assertEqual(len(mit), 1)
         self.assertEqual(mit[0].name, "urllib3")
 
@@ -52,10 +52,18 @@
         self.deps.applyLicenses(licenses)
         
         deps = self.deps.findUnknownLicenses()
         self.assertEqual(len(deps), 0)
 
         dep = self.deps.find("rich")
         self.assertEqual(dep.name, "rich")
-        self.assertEqual(dep.licence, "MIT")
+        self.assertEqual(dep.license, "MIT")
 
+    def test_update_dep(self):
+        dep = Dependency("urllib3", manager="pypi", license="Apache-2")
+
+        self.deps.updateDependency(dep)
+
+        urllib_dep = self.deps.find("urllib3")
+        self.assertEqual(urllib_dep.name, "urllib3")
+        self.assertEqual(urllib_dep.license, "Apache-2")
```

### Comparing `ghastoolkit-0.3.2/tests/test_depgraph.py` & `ghastoolkit-0.4.0/tests/test_depgraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.2/tests/test_github.py` & `ghastoolkit-0.4.0/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.2/tests/test_licenses.py` & `ghastoolkit-0.4.0/tests/test_licenses.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,10 +21,10 @@
         dependencies.append(Dependency("ghastoolkit", "com.geekmasher", manager="maven"))
         self.assertEqual(len(dependencies), 1)
         
         dependencies.applyLicenses(self.licenses)
 
         dep = dependencies.pop(0)
         self.assertTrue(isinstance(dep, Dependency))
-        self.assertEqual(dep.licence, "MIT")
+        self.assertEqual(dep.license, "MIT")
```

### Comparing `ghastoolkit-0.3.2/tests/test_octokit.py` & `ghastoolkit-0.4.0/tests/test_octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.3.2/tests/test_secretscanning.py` & `ghastoolkit-0.4.0/tests/test_secretscanning.py`

 * *Files identical despite different names*

