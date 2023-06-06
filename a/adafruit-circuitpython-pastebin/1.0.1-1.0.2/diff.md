# Comparing `tmp/adafruit-circuitpython-pastebin-1.0.1.tar.gz` & `tmp/adafruit-circuitpython-pastebin-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-pastebin-1.0.1.tar", last modified: Sun Mar 26 00:40:54 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-pastebin-1.0.2.tar", last modified: Tue Jun  6 19:42:18 2023, max compression
```

## Comparing `adafruit-circuitpython-pastebin-1.0.1.tar` & `adafruit-circuitpython-pastebin-1.0.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 00:40:54.577518 adafruit-circuitpython-pastebin-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 00:40:54.573518 adafruit-circuitpython-pastebin-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 00:40:54.573518 adafruit-circuitpython-pastebin-1.0.1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-03-26 00:40:36.000000 adafruit-circuitpython-pastebin-1.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 00:40:54.573518 adafruit-circuitpython-pastebin-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-26 00:40:36.000000 adafruit-circuitpython-pastebin-1.0.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-03-26 00:40:36.000000 adafruit-circuitpython-pastebin-1.0.1/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-26 00:40:36.000000 adafruit-circuitpython-pastebin-1.0.1/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-26 00:40:36.000000 adafruit-circuitpython-pastebin-1.0.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-03-26 00:40:36.000000 adafruit-circuitpython-pastebin-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-03-26 00:40:36.000000 adafruit-circuitpython-pastebin-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-03-26 00:40:36.000000 adafruit-circuitpython-pastebin-1.0.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-03-26 00:40:36.000000 adafruit-circuitpython-pastebin-1.0.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-03-26 00:40:36.000000 adafruit-circuitpython-pastebin-1.0.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-03-26 00:40:36.000000 adafruit-circuitpython-pastebin-1.0.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 00:40:54.573518 adafruit-circuitpython-pastebin-1.0.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-03-26 00:40:36.000000 adafruit-circuitpython-pastebin-1.0.1/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-26 00:40:36.000000 adafruit-circuitpython-pastebin-1.0.1/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-26 00:40:36.000000 adafruit-circuitpython-pastebin-1.0.1/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-03-26 00:40:54.577518 adafruit-circuitpython-pastebin-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-03-26 00:40:36.000000 adafruit-circuitpython-pastebin-1.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-03-26 00:40:36.000000 adafruit-circuitpython-pastebin-1.0.1/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 00:40:54.577518 adafruit-circuitpython-pastebin-1.0.1/adafruit_circuitpython_pastebin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-03-26 00:40:54.000000 adafruit-circuitpython-pastebin-1.0.1/adafruit_circuitpython_pastebin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-03-26 00:40:54.000000 adafruit-circuitpython-pastebin-1.0.1/adafruit_circuitpython_pastebin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 00:40:54.000000 adafruit-circuitpython-pastebin-1.0.1/adafruit_circuitpython_pastebin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-26 00:40:54.000000 adafruit-circuitpython-pastebin-1.0.1/adafruit_circuitpython_pastebin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-26 00:40:54.000000 adafruit-circuitpython-pastebin-1.0.1/adafruit_circuitpython_pastebin.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 00:40:54.577518 adafruit-circuitpython-pastebin-1.0.1/adafruit_pastebin/
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-03-26 00:40:46.000000 adafruit-circuitpython-pastebin-1.0.1/adafruit_pastebin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-03-26 00:40:46.000000 adafruit-circuitpython-pastebin-1.0.1/adafruit_pastebin/adafruit_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-03-26 00:40:46.000000 adafruit-circuitpython-pastebin-1.0.1/adafruit_pastebin/gist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-03-26 00:40:46.000000 adafruit-circuitpython-pastebin-1.0.1/adafruit_pastebin/pastebin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 00:40:54.577518 adafruit-circuitpython-pastebin-1.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 00:40:54.577518 adafruit-circuitpython-pastebin-1.0.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-03-26 00:40:36.000000 adafruit-circuitpython-pastebin-1.0.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-26 00:40:36.000000 adafruit-circuitpython-pastebin-1.0.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-03-26 00:40:36.000000 adafruit-circuitpython-pastebin-1.0.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-26 00:40:36.000000 adafruit-circuitpython-pastebin-1.0.1/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-03-26 00:40:36.000000 adafruit-circuitpython-pastebin-1.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-03-26 00:40:36.000000 adafruit-circuitpython-pastebin-1.0.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-26 00:40:36.000000 adafruit-circuitpython-pastebin-1.0.1/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-03-26 00:40:36.000000 adafruit-circuitpython-pastebin-1.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-26 00:40:36.000000 adafruit-circuitpython-pastebin-1.0.1/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-26 00:40:36.000000 adafruit-circuitpython-pastebin-1.0.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 00:40:54.577518 adafruit-circuitpython-pastebin-1.0.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-03-26 00:40:46.000000 adafruit-circuitpython-pastebin-1.0.1/examples/pastebin_aio_cpython.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-03-26 00:40:46.000000 adafruit-circuitpython-pastebin-1.0.1/examples/pastebin_gist_cpython.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-03-26 00:40:46.000000 adafruit-circuitpython-pastebin-1.0.1/examples/pastebin_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-03-26 00:40:46.000000 adafruit-circuitpython-pastebin-1.0.1/examples/pastebin_simpletest_cpython.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-26 00:40:36.000000 adafruit-circuitpython-pastebin-1.0.1/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-03-26 00:40:46.000000 adafruit-circuitpython-pastebin-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-26 00:40:36.000000 adafruit-circuitpython-pastebin-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-26 00:40:54.577518 adafruit-circuitpython-pastebin-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:42:18.652814 adafruit-circuitpython-pastebin-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:42:18.644814 adafruit-circuitpython-pastebin-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:42:18.648814 adafruit-circuitpython-pastebin-1.0.2/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-06 19:42:00.000000 adafruit-circuitpython-pastebin-1.0.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:42:18.648814 adafruit-circuitpython-pastebin-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-06 19:42:00.000000 adafruit-circuitpython-pastebin-1.0.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-06 19:42:00.000000 adafruit-circuitpython-pastebin-1.0.2/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-06 19:42:00.000000 adafruit-circuitpython-pastebin-1.0.2/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-06 19:42:00.000000 adafruit-circuitpython-pastebin-1.0.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-06 19:42:00.000000 adafruit-circuitpython-pastebin-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-06 19:42:00.000000 adafruit-circuitpython-pastebin-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-06-06 19:42:00.000000 adafruit-circuitpython-pastebin-1.0.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-06 19:42:00.000000 adafruit-circuitpython-pastebin-1.0.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-06-06 19:42:00.000000 adafruit-circuitpython-pastebin-1.0.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-06 19:42:00.000000 adafruit-circuitpython-pastebin-1.0.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:42:18.648814 adafruit-circuitpython-pastebin-1.0.2/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-06-06 19:42:00.000000 adafruit-circuitpython-pastebin-1.0.2/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-06 19:42:00.000000 adafruit-circuitpython-pastebin-1.0.2/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-06 19:42:00.000000 adafruit-circuitpython-pastebin-1.0.2/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-06-06 19:42:18.652814 adafruit-circuitpython-pastebin-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-06-06 19:42:00.000000 adafruit-circuitpython-pastebin-1.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-06 19:42:00.000000 adafruit-circuitpython-pastebin-1.0.2/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:42:18.648814 adafruit-circuitpython-pastebin-1.0.2/adafruit_circuitpython_pastebin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-06-06 19:42:18.000000 adafruit-circuitpython-pastebin-1.0.2/adafruit_circuitpython_pastebin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-06 19:42:18.000000 adafruit-circuitpython-pastebin-1.0.2/adafruit_circuitpython_pastebin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 19:42:18.000000 adafruit-circuitpython-pastebin-1.0.2/adafruit_circuitpython_pastebin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-06 19:42:18.000000 adafruit-circuitpython-pastebin-1.0.2/adafruit_circuitpython_pastebin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-06 19:42:18.000000 adafruit-circuitpython-pastebin-1.0.2/adafruit_circuitpython_pastebin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:42:18.648814 adafruit-circuitpython-pastebin-1.0.2/adafruit_pastebin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-06 19:42:10.000000 adafruit-circuitpython-pastebin-1.0.2/adafruit_pastebin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-06 19:42:10.000000 adafruit-circuitpython-pastebin-1.0.2/adafruit_pastebin/adafruit_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-06-06 19:42:10.000000 adafruit-circuitpython-pastebin-1.0.2/adafruit_pastebin/gist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-06-06 19:42:10.000000 adafruit-circuitpython-pastebin-1.0.2/adafruit_pastebin/pastebin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:42:18.652814 adafruit-circuitpython-pastebin-1.0.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:42:18.652814 adafruit-circuitpython-pastebin-1.0.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-06 19:42:00.000000 adafruit-circuitpython-pastebin-1.0.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-06 19:42:00.000000 adafruit-circuitpython-pastebin-1.0.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-06 19:42:00.000000 adafruit-circuitpython-pastebin-1.0.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-06 19:42:00.000000 adafruit-circuitpython-pastebin-1.0.2/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-06-06 19:42:00.000000 adafruit-circuitpython-pastebin-1.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-06 19:42:00.000000 adafruit-circuitpython-pastebin-1.0.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-06 19:42:00.000000 adafruit-circuitpython-pastebin-1.0.2/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-06 19:42:00.000000 adafruit-circuitpython-pastebin-1.0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-06 19:42:00.000000 adafruit-circuitpython-pastebin-1.0.2/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-06 19:42:00.000000 adafruit-circuitpython-pastebin-1.0.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:42:18.652814 adafruit-circuitpython-pastebin-1.0.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-06 19:42:10.000000 adafruit-circuitpython-pastebin-1.0.2/examples/pastebin_aio_cpython.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-06 19:42:10.000000 adafruit-circuitpython-pastebin-1.0.2/examples/pastebin_gist_cpython.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-06 19:42:10.000000 adafruit-circuitpython-pastebin-1.0.2/examples/pastebin_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-06 19:42:10.000000 adafruit-circuitpython-pastebin-1.0.2/examples/pastebin_simpletest_cpython.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-06 19:42:00.000000 adafruit-circuitpython-pastebin-1.0.2/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-06 19:42:10.000000 adafruit-circuitpython-pastebin-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-06 19:42:00.000000 adafruit-circuitpython-pastebin-1.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 19:42:18.652814 adafruit-circuitpython-pastebin-1.0.2/setup.cfg
```

### Comparing `adafruit-circuitpython-pastebin-1.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-pastebin-1.0.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pastebin-1.0.1/.gitignore` & `adafruit-circuitpython-pastebin-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pastebin-1.0.1/.pre-commit-config.yaml` & `adafruit-circuitpython-pastebin-1.0.2/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
   - repo: https://github.com/python/black
-    rev: 22.3.0
+    rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/fsfe/reuse-tool
-    rev: v0.14.0
+    rev: v1.1.2
     hooks:
       - id: reuse
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.2.0
+    rev: v4.4.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/pylint
-    rev: v2.15.5
+    rev: v2.17.4
     hooks:
       - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string,duplicate-code
         exclude: "^(docs/|examples/|tests/|setup.py$)"
```

### Comparing `adafruit-circuitpython-pastebin-1.0.1/.pylintrc` & `adafruit-circuitpython-pastebin-1.0.2/.pylintrc`

 * *Files 1% similar despite different names*

```diff
@@ -392,8 +392,8 @@
 min-public-methods=1
 
 
 [EXCEPTIONS]
 
 # Exceptions that will emit a warning when being caught. Defaults to
 # "Exception"
-overgeneral-exceptions=Exception
+overgeneral-exceptions=builtins.Exception
```

### Comparing `adafruit-circuitpython-pastebin-1.0.1/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-pastebin-1.0.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pastebin-1.0.1/LICENSE` & `adafruit-circuitpython-pastebin-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pastebin-1.0.1/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-pastebin-1.0.2/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pastebin-1.0.1/LICENSES/MIT.txt` & `adafruit-circuitpython-pastebin-1.0.2/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pastebin-1.0.1/LICENSES/Unlicense.txt` & `adafruit-circuitpython-pastebin-1.0.2/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pastebin-1.0.1/PKG-INFO` & `adafruit-circuitpython-pastebin-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-pastebin
-Version: 1.0.1
+Version: 1.0.2
 Summary: CircuitPython library for interacting with online pastebin services
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Pastebin
 Keywords: adafruit,blinka,circuitpython,micropython,pastebin,pastebin,text,online,api
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-pastebin-1.0.1/README.rst` & `adafruit-circuitpython-pastebin-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pastebin-1.0.1/adafruit_circuitpython_pastebin.egg-info/PKG-INFO` & `adafruit-circuitpython-pastebin-1.0.2/adafruit_circuitpython_pastebin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-pastebin
-Version: 1.0.1
+Version: 1.0.2
 Summary: CircuitPython library for interacting with online pastebin services
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Pastebin
 Keywords: adafruit,blinka,circuitpython,micropython,pastebin,pastebin,text,online,api
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-pastebin-1.0.1/adafruit_circuitpython_pastebin.egg-info/SOURCES.txt` & `adafruit-circuitpython-pastebin-1.0.2/adafruit_circuitpython_pastebin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pastebin-1.0.1/adafruit_pastebin/__init__.py` & `adafruit-circuitpython-pastebin-1.0.2/adafruit_pastebin/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
         def __str__(self) -> str:  # pylint: disable=invalid-str-returned
             ...
 
 except ImportError:
     pass
 
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Pastebin.git"
 
 
 # pylint: disable=too-few-public-methods
 class _Pastebin:
     """
     Generic paste bin class
```

### Comparing `adafruit-circuitpython-pastebin-1.0.1/adafruit_pastebin/adafruit_io.py` & `adafruit-circuitpython-pastebin-1.0.2/adafruit_pastebin/adafruit_io.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pastebin-1.0.1/adafruit_pastebin/gist.py` & `adafruit-circuitpython-pastebin-1.0.2/adafruit_pastebin/gist.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pastebin-1.0.1/adafruit_pastebin/pastebin.py` & `adafruit-circuitpython-pastebin-1.0.2/adafruit_pastebin/pastebin.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pastebin-1.0.1/docs/_static/favicon.ico` & `adafruit-circuitpython-pastebin-1.0.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pastebin-1.0.1/docs/conf.py` & `adafruit-circuitpython-pastebin-1.0.2/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # -- General configuration ------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx.ext.autodoc",
+    "sphinxcontrib.jquery",
     "sphinx.ext.intersphinx",
     "sphinx.ext.napoleon",
     "sphinx.ext.todo",
 ]
 
 # TODO: Please Read!
 # Uncomment the below if you use native CircuitPython modules such as
```

### Comparing `adafruit-circuitpython-pastebin-1.0.1/docs/index.rst` & `adafruit-circuitpython-pastebin-1.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pastebin-1.0.1/examples/pastebin_aio_cpython.py` & `adafruit-circuitpython-pastebin-1.0.2/examples/pastebin_aio_cpython.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pastebin-1.0.1/examples/pastebin_gist_cpython.py` & `adafruit-circuitpython-pastebin-1.0.2/examples/pastebin_gist_cpython.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pastebin-1.0.1/examples/pastebin_simpletest.py` & `adafruit-circuitpython-pastebin-1.0.2/examples/pastebin_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pastebin-1.0.1/examples/pastebin_simpletest_cpython.py` & `adafruit-circuitpython-pastebin-1.0.2/examples/pastebin_simpletest_cpython.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pastebin-1.0.1/pyproject.toml` & `adafruit-circuitpython-pastebin-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-pastebin"
 description = "CircuitPython library for interacting with online pastebin services"
-version = "1.0.1"
+version = "1.0.2"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Pastebin"}
 keywords = [
     "adafruit",
```

