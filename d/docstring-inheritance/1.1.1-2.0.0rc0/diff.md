# Comparing `tmp/docstring-inheritance-1.1.1.tar.gz` & `tmp/docstring-inheritance-2.0.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docstring-inheritance-1.1.1.tar", last modified: Sun Jan 15 20:44:14 2023, max compression
+gzip compressed data, was "docstring-inheritance-2.0.0rc0.tar", last modified: Tue Jun  6 19:37:59 2023, max compression
```

## Comparing `docstring-inheritance-1.1.1.tar` & `docstring-inheritance-2.0.0rc0.tar`

### file list

```diff
@@ -1,44 +1,43 @@
-drwxr-xr-x   0 antoine    (502) staff       (20)        0 2023-01-15 20:44:14.263315 docstring-inheritance-1.1.1/
-drwxr-xr-x   0 antoine    (502) staff       (20)        0 2023-01-15 20:44:14.246073 docstring-inheritance-1.1.1/.github/
-drwxr-xr-x   0 antoine    (502) staff       (20)        0 2023-01-15 20:44:14.251595 docstring-inheritance-1.1.1/.github/workflows/
--rw-r--r--   0 antoine    (502) staff       (20)      912 2022-11-16 08:52:25.000000 docstring-inheritance-1.1.1/.github/workflows/tests.yml
--rw-r--r--   0 antoine    (502) staff       (20)       69 2023-01-15 15:15:57.000000 docstring-inheritance-1.1.1/.gitignore
--rw-r--r--   0 antoine    (502) staff       (20)     2111 2023-01-15 15:15:57.000000 docstring-inheritance-1.1.1/.pre-commit-config.yaml
--rw-r--r--   0 antoine    (502) staff       (20)     1237 2023-01-15 20:41:50.000000 docstring-inheritance-1.1.1/CHANGELOG.md
--rw-r--r--   0 antoine    (502) staff       (20)     1264 2022-11-16 08:46:54.000000 docstring-inheritance-1.1.1/CREDITS.md
--rw-r--r--   0 antoine    (502) staff       (20)     1056 2022-11-16 08:46:54.000000 docstring-inheritance-1.1.1/LICENSE.txt
-drwxr-xr-x   0 antoine    (502) staff       (20)        0 2023-01-15 20:44:14.246345 docstring-inheritance-1.1.1/LICENSES/
-drwxr-xr-x   0 antoine    (502) staff       (20)        0 2023-01-15 20:44:14.252465 docstring-inheritance-1.1.1/LICENSES/headers/
--rw-r--r--   0 antoine    (502) staff       (20)      284 2022-11-16 08:46:54.000000 docstring-inheritance-1.1.1/LICENSES/headers/CC-BY-4.0.txt
--rw-r--r--   0 antoine    (502) staff       (20)     1056 2022-11-16 08:46:54.000000 docstring-inheritance-1.1.1/LICENSES/headers/MIT.txt
--rw-r--r--   0 antoine    (502) staff       (20)     9781 2023-01-15 20:44:14.263677 docstring-inheritance-1.1.1/PKG-INFO
--rw-r--r--   0 antoine    (502) staff       (20)     8689 2023-01-15 20:28:18.000000 docstring-inheritance-1.1.1/README.md
--rw-r--r--   0 antoine    (502) staff       (20)      180 2022-11-16 08:46:54.000000 docstring-inheritance-1.1.1/pyproject.toml
-drwxr-xr-x   0 antoine    (502) staff       (20)        0 2023-01-15 20:44:14.252869 docstring-inheritance-1.1.1/requirements/
--rw-r--r--   0 antoine    (502) staff       (20)      823 2023-01-15 15:15:57.000000 docstring-inheritance-1.1.1/requirements/test.txt
--rw-r--r--   0 antoine    (502) staff       (20)     1403 2023-01-15 20:44:14.265504 docstring-inheritance-1.1.1/setup.cfg
--rw-r--r--   0 antoine    (502) staff       (20)     1165 2022-11-16 08:46:54.000000 docstring-inheritance-1.1.1/setup.py
-drwxr-xr-x   0 antoine    (502) staff       (20)        0 2023-01-15 20:44:14.246917 docstring-inheritance-1.1.1/src/
-drwxr-xr-x   0 antoine    (502) staff       (20)        0 2023-01-15 20:44:14.254506 docstring-inheritance-1.1.1/src/docstring_inheritance/
--rw-r--r--   0 antoine    (502) staff       (20)     3969 2023-01-13 20:30:56.000000 docstring-inheritance-1.1.1/src/docstring_inheritance/__init__.py
--rw-r--r--   0 antoine    (502) staff       (20)     5153 2023-01-15 20:25:15.000000 docstring-inheritance-1.1.1/src/docstring_inheritance/class_docstrings_inheritor.py
-drwxr-xr-x   0 antoine    (502) staff       (20)        0 2023-01-15 20:44:14.259690 docstring-inheritance-1.1.1/src/docstring_inheritance/docstring_inheritors/
--rw-r--r--   0 antoine    (502) staff       (20)     1126 2023-01-13 20:30:56.000000 docstring-inheritance-1.1.1/src/docstring_inheritance/docstring_inheritors/__init__.py
--rw-r--r--   0 antoine    (502) staff       (20)    12216 2023-01-15 20:35:06.000000 docstring-inheritance-1.1.1/src/docstring_inheritance/docstring_inheritors/base.py
--rw-r--r--   0 antoine    (502) staff       (20)     3219 2023-01-13 20:30:56.000000 docstring-inheritance-1.1.1/src/docstring_inheritance/docstring_inheritors/google.py
--rw-r--r--   0 antoine    (502) staff       (20)     2896 2023-01-13 20:30:56.000000 docstring-inheritance-1.1.1/src/docstring_inheritance/docstring_inheritors/numpy.py
--rw-r--r--   0 antoine    (502) staff       (20)        0 2023-01-13 20:30:56.000000 docstring-inheritance-1.1.1/src/docstring_inheritance/py.typed
-drwxr-xr-x   0 antoine    (502) staff       (20)        0 2023-01-15 20:44:14.257301 docstring-inheritance-1.1.1/src/docstring_inheritance.egg-info/
--rw-r--r--   0 antoine    (502) staff       (20)     9781 2023-01-15 20:44:14.000000 docstring-inheritance-1.1.1/src/docstring_inheritance.egg-info/PKG-INFO
--rw-r--r--   0 antoine    (502) staff       (20)     1019 2023-01-15 20:44:14.000000 docstring-inheritance-1.1.1/src/docstring_inheritance.egg-info/SOURCES.txt
--rw-r--r--   0 antoine    (502) staff       (20)        1 2023-01-15 20:44:14.000000 docstring-inheritance-1.1.1/src/docstring_inheritance.egg-info/dependency_links.txt
--rw-r--r--   0 antoine    (502) staff       (20)       38 2023-01-15 20:44:14.000000 docstring-inheritance-1.1.1/src/docstring_inheritance.egg-info/requires.txt
--rw-r--r--   0 antoine    (502) staff       (20)       22 2023-01-15 20:44:14.000000 docstring-inheritance-1.1.1/src/docstring_inheritance.egg-info/top_level.txt
-drwxr-xr-x   0 antoine    (502) staff       (20)        0 2023-01-15 20:44:14.262893 docstring-inheritance-1.1.1/tests/
--rw-r--r--   0 antoine    (502) staff       (20)     5206 2023-01-15 20:33:47.000000 docstring-inheritance-1.1.1/tests/test_base_inheritor.py
--rw-r--r--   0 antoine    (502) staff       (20)     4895 2023-01-15 20:35:06.000000 docstring-inheritance-1.1.1/tests/test_google_inheritor.py
--rw-r--r--   0 antoine    (502) staff       (20)     3690 2023-01-13 20:30:56.000000 docstring-inheritance-1.1.1/tests/test_inheritance_for_functions.py
--rw-r--r--   0 antoine    (502) staff       (20)     3897 2023-01-15 20:36:50.000000 docstring-inheritance-1.1.1/tests/test_metaclass_google.py
--rw-r--r--   0 antoine    (502) staff       (20)     9380 2023-01-15 20:25:15.000000 docstring-inheritance-1.1.1/tests/test_metaclass_numpy.py
--rw-r--r--   0 antoine    (502) staff       (20)     6913 2023-01-15 20:25:15.000000 docstring-inheritance-1.1.1/tests/test_numpy_inheritor.py
--rw-r--r--   0 antoine    (502) staff       (20)      807 2023-01-15 15:15:57.000000 docstring-inheritance-1.1.1/tox.ini
+drwxr-xr-x   0 antoine    (502) staff       (20)        0 2023-06-06 19:37:59.157869 docstring-inheritance-2.0.0rc0/
+drwxr-xr-x   0 antoine    (502) staff       (20)        0 2023-06-06 19:37:59.140432 docstring-inheritance-2.0.0rc0/.github/
+drwxr-xr-x   0 antoine    (502) staff       (20)        0 2023-06-06 19:37:59.146582 docstring-inheritance-2.0.0rc0/.github/workflows/
+-rw-r--r--   0 antoine    (502) staff       (20)      905 2023-06-06 19:35:20.000000 docstring-inheritance-2.0.0rc0/.github/workflows/tests.yml
+-rw-r--r--   0 antoine    (502) staff       (20)       69 2023-01-15 15:15:57.000000 docstring-inheritance-2.0.0rc0/.gitignore
+-rw-r--r--   0 antoine    (502) staff       (20)     2044 2023-06-06 19:35:20.000000 docstring-inheritance-2.0.0rc0/.pre-commit-config.yaml
+-rw-r--r--   0 antoine    (502) staff       (20)     1514 2023-06-06 19:35:20.000000 docstring-inheritance-2.0.0rc0/CHANGELOG.md
+-rw-r--r--   0 antoine    (502) staff       (20)     1264 2022-11-16 08:46:54.000000 docstring-inheritance-2.0.0rc0/CREDITS.md
+-rw-r--r--   0 antoine    (502) staff       (20)     1056 2022-11-16 08:46:54.000000 docstring-inheritance-2.0.0rc0/LICENSE.txt
+drwxr-xr-x   0 antoine    (502) staff       (20)        0 2023-06-06 19:37:59.140920 docstring-inheritance-2.0.0rc0/LICENSES/
+drwxr-xr-x   0 antoine    (502) staff       (20)        0 2023-06-06 19:37:59.147691 docstring-inheritance-2.0.0rc0/LICENSES/headers/
+-rw-r--r--   0 antoine    (502) staff       (20)      284 2022-11-16 08:46:54.000000 docstring-inheritance-2.0.0rc0/LICENSES/headers/CC-BY-4.0.txt
+-rw-r--r--   0 antoine    (502) staff       (20)     1056 2022-11-16 08:46:54.000000 docstring-inheritance-2.0.0rc0/LICENSES/headers/MIT.txt
+-rw-r--r--   0 antoine    (502) staff       (20)     9721 2023-06-06 19:37:59.158204 docstring-inheritance-2.0.0rc0/PKG-INFO
+-rw-r--r--   0 antoine    (502) staff       (20)     8689 2023-06-05 21:34:25.000000 docstring-inheritance-2.0.0rc0/README.md
+-rw-r--r--   0 antoine    (502) staff       (20)     1343 2023-06-06 19:35:20.000000 docstring-inheritance-2.0.0rc0/pyproject.toml
+drwxr-xr-x   0 antoine    (502) staff       (20)        0 2023-06-06 19:37:59.148146 docstring-inheritance-2.0.0rc0/requirements/
+-rw-r--r--   0 antoine    (502) staff       (20)      605 2023-06-06 19:35:20.000000 docstring-inheritance-2.0.0rc0/requirements/test.txt
+-rw-r--r--   0 antoine    (502) staff       (20)      178 2023-06-06 19:37:59.159365 docstring-inheritance-2.0.0rc0/setup.cfg
+drwxr-xr-x   0 antoine    (502) staff       (20)        0 2023-06-06 19:37:59.141880 docstring-inheritance-2.0.0rc0/src/
+drwxr-xr-x   0 antoine    (502) staff       (20)        0 2023-06-06 19:37:59.149396 docstring-inheritance-2.0.0rc0/src/docstring_inheritance/
+-rw-r--r--   0 antoine    (502) staff       (20)     3969 2023-01-13 20:30:56.000000 docstring-inheritance-2.0.0rc0/src/docstring_inheritance/__init__.py
+-rw-r--r--   0 antoine    (502) staff       (20)     5609 2023-06-06 19:35:20.000000 docstring-inheritance-2.0.0rc0/src/docstring_inheritance/class_docstrings_inheritor.py
+drwxr-xr-x   0 antoine    (502) staff       (20)        0 2023-06-06 19:37:59.154256 docstring-inheritance-2.0.0rc0/src/docstring_inheritance/docstring_inheritors/
+-rw-r--r--   0 antoine    (502) staff       (20)     1126 2023-01-13 20:30:56.000000 docstring-inheritance-2.0.0rc0/src/docstring_inheritance/docstring_inheritors/__init__.py
+-rw-r--r--   0 antoine    (502) staff       (20)    12515 2023-06-06 19:35:20.000000 docstring-inheritance-2.0.0rc0/src/docstring_inheritance/docstring_inheritors/base.py
+-rw-r--r--   0 antoine    (502) staff       (20)     3212 2023-06-06 19:35:20.000000 docstring-inheritance-2.0.0rc0/src/docstring_inheritance/docstring_inheritors/google.py
+-rw-r--r--   0 antoine    (502) staff       (20)     2892 2023-06-06 19:35:20.000000 docstring-inheritance-2.0.0rc0/src/docstring_inheritance/docstring_inheritors/numpy.py
+-rw-r--r--   0 antoine    (502) staff       (20)        0 2023-01-13 20:30:56.000000 docstring-inheritance-2.0.0rc0/src/docstring_inheritance/py.typed
+drwxr-xr-x   0 antoine    (502) staff       (20)        0 2023-06-06 19:37:59.152145 docstring-inheritance-2.0.0rc0/src/docstring_inheritance.egg-info/
+-rw-r--r--   0 antoine    (502) staff       (20)     9721 2023-06-06 19:37:59.000000 docstring-inheritance-2.0.0rc0/src/docstring_inheritance.egg-info/PKG-INFO
+-rw-r--r--   0 antoine    (502) staff       (20)     1010 2023-06-06 19:37:59.000000 docstring-inheritance-2.0.0rc0/src/docstring_inheritance.egg-info/SOURCES.txt
+-rw-r--r--   0 antoine    (502) staff       (20)        1 2023-06-06 19:37:59.000000 docstring-inheritance-2.0.0rc0/src/docstring_inheritance.egg-info/dependency_links.txt
+-rw-r--r--   0 antoine    (502) staff       (20)       38 2023-06-06 19:37:59.000000 docstring-inheritance-2.0.0rc0/src/docstring_inheritance.egg-info/requires.txt
+-rw-r--r--   0 antoine    (502) staff       (20)       22 2023-06-06 19:37:59.000000 docstring-inheritance-2.0.0rc0/src/docstring_inheritance.egg-info/top_level.txt
+drwxr-xr-x   0 antoine    (502) staff       (20)        0 2023-06-06 19:37:59.157401 docstring-inheritance-2.0.0rc0/tests/
+-rw-r--r--   0 antoine    (502) staff       (20)     8874 2023-06-06 19:35:20.000000 docstring-inheritance-2.0.0rc0/tests/test_base_inheritor.py
+-rw-r--r--   0 antoine    (502) staff       (20)     4867 2023-06-06 19:35:20.000000 docstring-inheritance-2.0.0rc0/tests/test_google_inheritor.py
+-rw-r--r--   0 antoine    (502) staff       (20)     3690 2023-01-13 20:30:56.000000 docstring-inheritance-2.0.0rc0/tests/test_inheritance_for_functions.py
+-rw-r--r--   0 antoine    (502) staff       (20)     3897 2023-06-05 21:34:25.000000 docstring-inheritance-2.0.0rc0/tests/test_metaclass_google.py
+-rw-r--r--   0 antoine    (502) staff       (20)     9165 2023-06-06 19:35:20.000000 docstring-inheritance-2.0.0rc0/tests/test_metaclass_numpy.py
+-rw-r--r--   0 antoine    (502) staff       (20)     6885 2023-06-06 19:35:20.000000 docstring-inheritance-2.0.0rc0/tests/test_numpy_inheritor.py
+-rw-r--r--   0 antoine    (502) staff       (20)      772 2023-06-06 19:37:11.000000 docstring-inheritance-2.0.0rc0/tox.ini
```

### Comparing `docstring-inheritance-1.1.1/.github/workflows/tests.yml` & `docstring-inheritance-2.0.0rc0/.github/workflows/tests.yml`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 jobs:
   test:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ubuntu-latest, macos-latest, windows-latest]
-        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
+        python-version: ["3.8", "3.9", "3.10", "3.11"]
     steps:
       - uses: actions/checkout@v2
       - name: Setup Python
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install tox
```

### Comparing `docstring-inheritance-1.1.1/.pre-commit-config.yaml` & `docstring-inheritance-2.0.0rc0/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -15,78 +15,75 @@
   rev: v1.10.0
   hooks:
     - id: rst-backticks
     - id: rst-directive-colons
     - id: rst-inline-touching-normal
 
 - repo: https://github.com/PyCQA/autoflake
-  rev: v2.0.0
+  rev: v2.1.1
   hooks:
     - id: autoflake
       args: [
         --in-place,
         --remove-all-unused-imports,
       ]
 
 - repo: https://github.com/asottile/reorder_python_imports
   rev: v3.9.0
   hooks:
   - id: reorder-python-imports
     args: [
       --application-directories,
       src,
-      --py37-plus,
+      --py38-plus,
       --add-import,
       "from __future__ import annotations",
     ]
 
 - repo: https://github.com/myint/docformatter
-  rev: v1.5.1
+  rev: v1.7.1
   hooks:
     - id: docformatter
       exclude: ^tests/
       args: [
         --in-place,
-        --wrap-summaries,
-        "88",
-        --wrap-descriptions,
-        "88",
+        --black,
       ]
 
 - repo: https://github.com/asottile/pyupgrade
-  rev: v3.3.1
+  rev: v3.4.0
   hooks:
   - id: pyupgrade
-    args: [--py37-plus]
+    args: [--py38-plus]
 
 - repo: https://github.com/psf/black
-  rev: 22.12.0
+  rev: 23.3.0
   hooks:
   - id: black
 
 - repo: https://github.com/PyCQA/flake8
   rev: 6.0.0
   hooks:
   - id: flake8
     additional_dependencies:
       - flake8-bugbear==22.12.6
       - flake8-docstrings==1.6.0
       - flake8-print==5.0.0
       - pep8-naming==0.13.3
 
 - repo: https://github.com/pre-commit/mirrors-mypy
-  rev: v0.991
+  rev: v1.3.0
   hooks:
     - id: mypy
       exclude: ^(tests/|setup\.py)
       args:
         - --strict
 
 - repo: https://github.com/Lucas-C/pre-commit-hooks
-  rev: v1.3.1
+  rev: v1.5.1
   hooks:
     - id: insert-license
       name: insert MIT license
       files: \.py$
       args:
         - --license-filepath
         - LICENSES/headers/MIT.txt
```

### Comparing `docstring-inheritance-1.1.1/CHANGELOG.md` & `docstring-inheritance-2.0.0rc0/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,21 @@
 
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [2.0.0rc0] - 2023-06
+### Changed
+- Docstring inheritance for methods only inherit from the first found parent.
+### Fixed
+- Docstring inheritance for methods with no argument descriptions.
+- Format of the arguments provided with the default description for the Numpy style.
+
 ## [1.1.1] - 2023-01
 ### Fixed
 - Docstring inheritance for methods with multiple parents.
 
 ## [1.1.0] - 2023-01
 ### Added
 - Support class docstrings with `__init__` signature description.
```

### Comparing `docstring-inheritance-1.1.1/CREDITS.md` & `docstring-inheritance-2.0.0rc0/CREDITS.md`

 * *Files identical despite different names*

### Comparing `docstring-inheritance-1.1.1/LICENSE.txt` & `docstring-inheritance-2.0.0rc0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `docstring-inheritance-1.1.1/LICENSES/headers/MIT.txt` & `docstring-inheritance-2.0.0rc0/LICENSES/headers/MIT.txt`

 * *Files identical despite different names*

### Comparing `docstring-inheritance-1.1.1/PKG-INFO` & `docstring-inheritance-2.0.0rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 Metadata-Version: 2.1
 Name: docstring-inheritance
-Version: 1.1.1
+Version: 2.0.0rc0
 Summary: Avoid writing and maintaining duplicated docstrings.
-Home-page: https://github.com/AntoineD/docstring-inheritance
 Author: Antoine Dechaume
 License: MIT
 Project-URL: Documentation, https://antoined.github.io/docstring-inheritance
+Project-URL: Homepage, https://github.com/AntoineD/docstring-inheritance
 Project-URL: Source, https://github.com/AntoineD/docstring-inheritance
 Project-URL: Tracker, https://github.com/AntoineD/docstring-inheritance/issues
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: <3.12,>=3.7
+Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.txt
-License-File: CREDITS.md
 
 <!--
  Copyright 2021 Antoine DECHAUME
 
  This work is licensed under the Creative Commons Attribution 4.0
  International License. To view a copy of this license, visit
  http://creativecommons.org/licenses/by/4.0/ or send a letter to Creative
```

### Comparing `docstring-inheritance-1.1.1/README.md` & `docstring-inheritance-2.0.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `docstring-inheritance-1.1.1/requirements/test.txt` & `docstring-inheritance-2.0.0rc0/requirements/test.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,28 @@
 #
-# This file is autogenerated by pip-compile with Python 3.7
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
 #    pip-compile --extra=test --output-file=requirements/test.txt
 #
-attrs==22.2.0
-    # via pytest
-covdefaults==2.2.2
+covdefaults==2.3.0
     # via docstring-inheritance (setup.py)
-coverage[toml]==7.0.5
+coverage[toml]==7.2.7
     # via
     #   covdefaults
     #   pytest-cov
-exceptiongroup==1.1.0
+exceptiongroup==1.1.1
     # via pytest
-importlib-metadata==6.0.0
-    # via
-    #   pluggy
-    #   pytest
 iniconfig==2.0.0
     # via pytest
-packaging==23.0
+packaging==23.1
     # via pytest
 pluggy==1.0.0
     # via pytest
-pytest==7.2.0
+pytest==7.3.1
     # via
     #   docstring-inheritance (setup.py)
     #   pytest-cov
-pytest-cov==4.0.0
+pytest-cov==4.1.0
     # via docstring-inheritance (setup.py)
 tomli==2.0.1
-    # via
-    #   coverage
-    #   pytest
-typing-extensions==4.4.0
-    # via importlib-metadata
-zipp==3.11.0
-    # via importlib-metadata
+    # via pytest
```

### Comparing `docstring-inheritance-1.1.1/setup.py` & `docstring-inheritance-2.0.0rc0/src/docstring_inheritance/docstring_inheritors/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,11 +14,7 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 from __future__ import annotations
-
-import setuptools
-
-setuptools.setup()
```

### Comparing `docstring-inheritance-1.1.1/src/docstring_inheritance/__init__.py` & `docstring-inheritance-2.0.0rc0/src/docstring_inheritance/__init__.py`

 * *Files identical despite different names*

### Comparing `docstring-inheritance-1.1.1/src/docstring_inheritance/class_docstrings_inheritor.py` & `docstring-inheritance-2.0.0rc0/src/docstring_inheritance/class_docstrings_inheritor.py`

 * *Files 12% similar despite different names*

```diff
@@ -99,37 +99,42 @@
                 init_method.__doc__ = self._cls.__doc__
                 func = init_method
                 init_doc_changed = True
 
         if func is None:
             func = self._create_dummy_func_with_doc(self._cls.__doc__)
 
-        for cls_ in self.__mro_classes:
-            self._docstring_inheritor(cls_.__doc__, func)
+        for parent_cls in self.__mro_classes:
+            # As opposed to the attribute inheritance, and following the way a class is
+            # assembled by type(), the docstring of a class is the combination of the
+            # docstrings of its parents.
+            self._docstring_inheritor(parent_cls.__doc__, func)
 
         self._cls.__doc__ = func.__doc__
 
         if self._init_in_class and init_doc_changed:
             init_method.__doc__ = old_init_doc
 
     def _inherit_attrs_docstrings(
         self,
     ) -> None:
         """Create the inherited docstrings for the class attributes."""
         for attr_name, attr in self._cls.__dict__.items():
             if not isinstance(attr, FunctionType):
                 continue
 
-            for cls_ in self.__mro_classes:
-                method = getattr(cls_, attr_name, None)
-                if method is None:
-                    continue
-                parent_doc = method.__doc__
-                if parent_doc is not None:
-                    self._docstring_inheritor(parent_doc, attr)
+            for parent_cls in self.__mro_classes:
+                parent_method = getattr(parent_cls, attr_name, None)
+                if parent_method is not None:
+                    parent_doc = parent_method.__doc__
+                    if parent_doc is not None:
+                        self._docstring_inheritor(parent_doc, attr)
+                        # As opposed to the class docstring inheritance, and following
+                        # the MRO for methods, we inherit only from the first found parent.
+                        break
 
     @staticmethod
     def _create_dummy_func_with_doc(docstring: str | None) -> Callable[..., Any]:
         """Create a dummy function with a given docstring.
 
         Args:
             docstring: The docstring to be assigned.
```

### Comparing `docstring-inheritance-1.1.1/src/docstring_inheritance/docstring_inheritors/base.py` & `docstring-inheritance-2.0.0rc0/src/docstring_inheritance/docstring_inheritors/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,18 +65,24 @@
         "Warns",
         "Warnings",
         "See Also",
         "Notes",
         "References",
         "Examples",
     ]
-    _ARGS_SECTION_ITEMS_NAMES: ClassVar[set[str]]
-    _SECTION_ITEMS_NAMES: ClassVar[set[str]]
+    """Names of the sections."""
+
+    _ARGS_SECTION_NAMES: ClassVar[set[str]]
+    """Names of the sections for method and function arguments."""
+
+    _SECTION_NAMES_WITH_ITEMS: ClassVar[set[str]]
+    """Names of the sections with items."""
 
     MISSING_ARG_DESCRIPTION: ClassVar[str] = "The description is missing."
+    """Fall back description for an argument without a given description."""
 
     def __call__(self, parent_doc: str | None, child_func: Callable[..., Any]) -> None:
         """
         Args:
             parent_doc: The docstring of the parent.
             child_func: The child function which docstring inherit from the parent.
         """
@@ -161,15 +167,15 @@
         for line2, line1 in lines_pairs:
             line2_rstripped = line2.rstrip()
 
             section_name, section_body = cls._parse_one_section(
                 line1, line2_rstripped, reversed_section_body_lines
             )
             if section_name is not None and section_body is not None:
-                if section_name in cls._SECTION_ITEMS_NAMES:
+                if section_name in cls._SECTION_NAMES_WITH_ITEMS:
                     reversed_sections[section_name] = cls._parse_section_items(
                         section_body
                     )
                 else:
                     reversed_sections[section_name] = section_body
 
                 # We took into account line1 in addition to line2,
@@ -245,52 +251,53 @@
             child_section_names - parent_section_names_to_copy
         )
         for section_name in child_sections_names_to_copy:
             temp_sections[section_name] = child_sections[section_name]
 
         # For sections with items, the sections common to parent and child are merged.
         common_section_names_with_items = (
-            parent_section_names & child_section_names & cls._SECTION_ITEMS_NAMES
+            parent_section_names & child_section_names & cls._SECTION_NAMES_WITH_ITEMS
         )
 
         for section_name in common_section_names_with_items:
             temp_section_items = cast(
                 Dict[str, str], parent_sections[section_name]
             ).copy()
             temp_section_items.update(
                 cast(Dict[str, str], child_sections[section_name])
             )
 
-            if section_name in cls._ARGS_SECTION_ITEMS_NAMES:
-                temp_section_items = cls._inherit_section_items_with_args(
-                    child_func,
-                    temp_section_items,
-                )
-
             temp_sections[section_name] = temp_section_items
 
-        # Order the standard sections.
+        # Args section shall be filtered.
+        for section_name in temp_sections.keys() & cls._ARGS_SECTION_NAMES:
+            temp_sections[section_name] = cls._filter_args_section(
+                child_func,
+                cast(Dict[str, str], temp_sections[section_name]),
+            )
+
+        # Reorder the standard sections.
         new_child_sections = {
             section_name: temp_sections.pop(section_name)
             for section_name in cls._SECTION_NAMES
             if section_name in temp_sections
         }
 
         # Add the remaining non-standard sections.
         new_child_sections.update(temp_sections)
 
         return new_child_sections
 
     @classmethod
-    def _inherit_section_items_with_args(
+    def _filter_args_section(
         cls,
         func: Callable[..., Any],
         section_items: dict[str, str],
     ) -> dict[str, str]:
-        """Inherit section items for the args of a signature.
+        """Filter the args section items with the args of a signature.
 
         The argument ``self`` is removed. The arguments are ordered according to the
         signature of ``func``. An argument of ``func`` missing in ``section_items`` gets
         a default description defined in :attr:`.MISSING_ARG_DESCRIPTION`.
 
         Args:
             func: The function that provides the signature.
```

### Comparing `docstring-inheritance-1.1.1/src/docstring_inheritance/docstring_inheritors/google.py` & `docstring-inheritance-2.0.0rc0/src/docstring_inheritance/docstring_inheritors/google.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,17 +30,17 @@
     """A class for inheriting docstrings in Google format."""
 
     _SECTION_NAMES: ClassVar[list[str | None]] = list(
         AbstractDocstringInheritor._SECTION_NAMES
     )
     _SECTION_NAMES[1] = "Args"
 
-    _ARGS_SECTION_ITEMS_NAMES: ClassVar[set[str]] = {"Args"}
+    _ARGS_SECTION_NAMES: ClassVar[set[str]] = {"Args"}
 
-    _SECTION_ITEMS_NAMES: ClassVar[set[str]] = _ARGS_SECTION_ITEMS_NAMES | {
+    _SECTION_NAMES_WITH_ITEMS: ClassVar[set[str]] = _ARGS_SECTION_NAMES | {
         "Attributes",
         "Methods",
     }
 
     MISSING_ARG_DESCRIPTION = f": {AbstractDocstringInheritor.MISSING_ARG_DESCRIPTION}"
 
     @classmethod
```

### Comparing `docstring-inheritance-1.1.1/src/docstring_inheritance/docstring_inheritors/numpy.py` & `docstring-inheritance-2.0.0rc0/src/docstring_inheritance/docstring_inheritors/numpy.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,27 +23,27 @@
 
 from .base import AbstractDocstringInheritor
 
 
 class NumpyDocstringInheritor(AbstractDocstringInheritor):
     """A class for inheriting docstrings in Numpy format."""
 
-    _ARGS_SECTION_ITEMS_NAMES: ClassVar[set[str]] = {
+    _ARGS_SECTION_NAMES: ClassVar[set[str]] = {
         "Parameters",
         "Other Parameters",
     }
 
-    _SECTION_ITEMS_NAMES: ClassVar[set[str]] = _ARGS_SECTION_ITEMS_NAMES | {
+    _SECTION_NAMES_WITH_ITEMS: ClassVar[set[str]] = _ARGS_SECTION_NAMES | {
         "Attributes",
         "Methods",
     }
 
     MISSING_ARG_DESCRIPTION: ClassVar[
         str
-    ] = f":\n{AbstractDocstringInheritor.MISSING_ARG_DESCRIPTION}"
+    ] = f"\n    {AbstractDocstringInheritor.MISSING_ARG_DESCRIPTION}"
 
     @classmethod
     def _parse_one_section(
         cls, line1: str, line2_rstripped: str, reversed_section_body_lines: list[str]
     ) -> tuple[str, str] | tuple[None, None]:
         # See https://github.com/numpy/numpydoc/blob/d85f54ea342c1d223374343be88da94ce9f58dec/numpydoc/docscrape.py#L179  # noqa: B950
         if len(line2_rstripped) >= 3 and (set(line2_rstripped) in ({"-"}, {"="})):
```

### Comparing `docstring-inheritance-1.1.1/src/docstring_inheritance.egg-info/PKG-INFO` & `docstring-inheritance-2.0.0rc0/src/docstring_inheritance.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 Metadata-Version: 2.1
 Name: docstring-inheritance
-Version: 1.1.1
+Version: 2.0.0rc0
 Summary: Avoid writing and maintaining duplicated docstrings.
-Home-page: https://github.com/AntoineD/docstring-inheritance
 Author: Antoine Dechaume
 License: MIT
 Project-URL: Documentation, https://antoined.github.io/docstring-inheritance
+Project-URL: Homepage, https://github.com/AntoineD/docstring-inheritance
 Project-URL: Source, https://github.com/AntoineD/docstring-inheritance
 Project-URL: Tracker, https://github.com/AntoineD/docstring-inheritance/issues
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: <3.12,>=3.7
+Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.txt
-License-File: CREDITS.md
 
 <!--
  Copyright 2021 Antoine DECHAUME
 
  This work is licensed under the Creative Commons Attribution 4.0
  International License. To view a copy of this license, visit
  http://creativecommons.org/licenses/by/4.0/ or send a letter to Creative
```

### Comparing `docstring-inheritance-1.1.1/src/docstring_inheritance.egg-info/SOURCES.txt` & `docstring-inheritance-2.0.0rc0/src/docstring_inheritance.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 .pre-commit-config.yaml
 CHANGELOG.md
 CREDITS.md
 LICENSE.txt
 README.md
 pyproject.toml
 setup.cfg
-setup.py
 tox.ini
 .github/workflows/tests.yml
 LICENSES/headers/CC-BY-4.0.txt
 LICENSES/headers/MIT.txt
 requirements/test.txt
 src/docstring_inheritance/__init__.py
 src/docstring_inheritance/class_docstrings_inheritor.py
```

### Comparing `docstring-inheritance-1.1.1/tests/test_google_inheritor.py` & `docstring-inheritance-2.0.0rc0/tests/test_google_inheritor.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,13 +198,11 @@
 
 def test_inherit_section_items_with_args():
     def func(arg):
         """"""
 
     expected = {"arg": GoogleDocstringInheritor.MISSING_ARG_DESCRIPTION}
 
-    assert (
-        GoogleDocstringInheritor._inherit_section_items_with_args(func, {}) == expected
-    )
+    assert GoogleDocstringInheritor._filter_args_section(func, {}) == expected
 
 
 # TODO: test section order and all sections items
```

### Comparing `docstring-inheritance-1.1.1/tests/test_inheritance_for_functions.py` & `docstring-inheritance-2.0.0rc0/tests/test_inheritance_for_functions.py`

 * *Files identical despite different names*

### Comparing `docstring-inheritance-1.1.1/tests/test_metaclass_google.py` & `docstring-inheritance-2.0.0rc0/tests/test_metaclass_google.py`

 * *Files identical despite different names*

### Comparing `docstring-inheritance-1.1.1/tests/test_metaclass_numpy.py` & `docstring-inheritance-2.0.0rc0/tests/test_metaclass_numpy.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,16 +35,16 @@
 def assert_args_inheritance(cls):
     excepted = """
 Parameters
 ----------
 xx: int
 x: int
 *args: int
-yy:
-The description is missing.
+yy
+    The description is missing.
 y: float
 **kwargs: int"""
 
     assert cls.method.__doc__ == excepted
 
 
 @parametrize_inheritance
@@ -319,42 +319,30 @@
             x: x doc
 
             Returns
             -------
             int
             """
 
-    class Parent2:
-        def method(self, *args, y=None, **kwargs):
-            """Summary 2
-
-            Parameters
-            ----------
-            *args: int
-            y: float
-            **kwargs: int
-
-            Returns
-            -------
-            float
-            """
-
-    class Child(Parent1, Parent2, metaclass=inheritance_class):
+    class Child(Parent1, metaclass=inheritance_class):
         def method(self, w, x, *args, y=None, **kwargs):
             pass
 
     excepted = """Summary 1
 
 Parameters
 ----------
 w: w doc
 x: x doc
-*args: int
-y: float
-**kwargs: int
+*args
+    The description is missing.
+y
+    The description is missing.
+**kwargs
+    The description is missing.
 
 Returns
 -------
 int"""
 
     assert Child.method.__doc__ == excepted
```

### Comparing `docstring-inheritance-1.1.1/tests/test_numpy_inheritor.py` & `docstring-inheritance-2.0.0rc0/tests/test_numpy_inheritor.py`

 * *Files 5% similar despite different names*

```diff
@@ -259,13 +259,11 @@
 
 def test_inherit_section_items_with_args():
     def func(arg):
         """"""
 
     expected = {"arg": NumpyDocstringInheritor.MISSING_ARG_DESCRIPTION}
 
-    assert (
-        NumpyDocstringInheritor._inherit_section_items_with_args(func, {}) == expected
-    )
+    assert NumpyDocstringInheritor._filter_args_section(func, {}) == expected
 
 
 # TODO: test section order and all sections items
```

### Comparing `docstring-inheritance-1.1.1/tox.ini` & `docstring-inheritance-2.0.0rc0/tox.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tox]
 min_version = 4
-env_list = py{37,38,39,310,311}
+env_list = py{38,39,310,311}
 
 [testenv]
 package = wheel
 deps =
     -r requirements/test.txt
 set_env =
-    coverage: __COVERAGE_POSARGS=--cov --cov-config=setup.cfg --cov-report=xml --cov-report=html
+    coverage: __COVERAGE_POSARGS=--cov --cov-config=pyproject.toml --cov-report=xml --cov-report=html
 commands =
     pytest {env:__COVERAGE_POSARGS:} {posargs}
 
 [testenv:create-dist]
 description = create the pypi distribution
 # See packaging info at https://pypi.org/help/#publishing.
 deps =
@@ -19,17 +19,16 @@
     build
 skip_install = true
 allowlist_externals = rm
 commands =
     rm -rf dist build
     python -m build
     twine check dist/*
-    python setup.py check --metadata
 
 [testenv:update-deps-test]
 description = update the test envs dependencies
-base_python = python3.7
+base_python = python3.8
 set_env =
 deps = pip-tools
 skip_install = true
 commands =
     pip-compile -U --extra test -o requirements/test.txt
```

