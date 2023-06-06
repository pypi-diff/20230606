# Comparing `tmp/adafruit-circuitpython-mcp3xxx-1.4.8.tar.gz` & `tmp/adafruit-circuitpython-mcp3xxx-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-mcp3xxx-1.4.8.tar", last modified: Tue Jun  7 17:02:23 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-mcp3xxx-1.4.9.tar", last modified: Thu Jun  9 18:15:10 2022, max compression
```

## Comparing `adafruit-circuitpython-mcp3xxx-1.4.8.tar` & `adafruit-circuitpython-mcp3xxx-1.4.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:02:23.443278 adafruit-circuitpython-mcp3xxx-1.4.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:02:23.423278 adafruit-circuitpython-mcp3xxx-1.4.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:02:23.435278 adafruit-circuitpython-mcp3xxx-1.4.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-07 17:02:07.000000 adafruit-circuitpython-mcp3xxx-1.4.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:02:23.435278 adafruit-circuitpython-mcp3xxx-1.4.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-06-07 17:02:07.000000 adafruit-circuitpython-mcp3xxx-1.4.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-07 17:02:07.000000 adafruit-circuitpython-mcp3xxx-1.4.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-07 17:02:07.000000 adafruit-circuitpython-mcp3xxx-1.4.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-07 17:02:07.000000 adafruit-circuitpython-mcp3xxx-1.4.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-06-07 17:02:07.000000 adafruit-circuitpython-mcp3xxx-1.4.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-06-07 17:02:07.000000 adafruit-circuitpython-mcp3xxx-1.4.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-07 17:02:07.000000 adafruit-circuitpython-mcp3xxx-1.4.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-06-07 17:02:07.000000 adafruit-circuitpython-mcp3xxx-1.4.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1087 2022-06-07 17:02:07.000000 adafruit-circuitpython-mcp3xxx-1.4.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:02:23.435278 adafruit-circuitpython-mcp3xxx-1.4.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-07 17:02:07.000000 adafruit-circuitpython-mcp3xxx-1.4.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-07 17:02:07.000000 adafruit-circuitpython-mcp3xxx-1.4.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-07 17:02:07.000000 adafruit-circuitpython-mcp3xxx-1.4.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5869 2022-06-07 17:02:23.443278 adafruit-circuitpython-mcp3xxx-1.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5142 2022-06-07 17:02:07.000000 adafruit-circuitpython-mcp3xxx-1.4.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-07 17:02:07.000000 adafruit-circuitpython-mcp3xxx-1.4.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:02:23.439278 adafruit-circuitpython-mcp3xxx-1.4.8/adafruit_circuitpython_mcp3xxx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5869 2022-06-07 17:02:23.000000 adafruit-circuitpython-mcp3xxx-1.4.8/adafruit_circuitpython_mcp3xxx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1326 2022-06-07 17:02:23.000000 adafruit-circuitpython-mcp3xxx-1.4.8/adafruit_circuitpython_mcp3xxx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-07 17:02:23.000000 adafruit-circuitpython-mcp3xxx-1.4.8/adafruit_circuitpython_mcp3xxx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-06-07 17:02:23.000000 adafruit-circuitpython-mcp3xxx-1.4.8/adafruit_circuitpython_mcp3xxx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-06-07 17:02:23.000000 adafruit-circuitpython-mcp3xxx-1.4.8/adafruit_circuitpython_mcp3xxx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:02:23.439278 adafruit-circuitpython-mcp3xxx-1.4.8/adafruit_mcp3xxx/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:02:07.000000 adafruit-circuitpython-mcp3xxx-1.4.8/adafruit_mcp3xxx/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2281 2022-06-07 17:02:07.000000 adafruit-circuitpython-mcp3xxx-1.4.8/adafruit_mcp3xxx/analog_in.py
--rw-r--r--   0 runner    (1001) docker     (121)     1429 2022-06-07 17:02:07.000000 adafruit-circuitpython-mcp3xxx-1.4.8/adafruit_mcp3xxx/mcp3002.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1232 2022-06-07 17:02:07.000000 adafruit-circuitpython-mcp3xxx-1.4.8/adafruit_mcp3xxx/mcp3004.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1504 2022-06-07 17:02:07.000000 adafruit-circuitpython-mcp3xxx-1.4.8/adafruit_mcp3xxx/mcp3008.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3281 2022-06-07 17:02:07.000000 adafruit-circuitpython-mcp3xxx-1.4.8/adafruit_mcp3xxx/mcp3xxx.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:02:23.443278 adafruit-circuitpython-mcp3xxx-1.4.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:02:23.443278 adafruit-circuitpython-mcp3xxx-1.4.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-07 17:02:07.000000 adafruit-circuitpython-mcp3xxx-1.4.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-07 17:02:07.000000 adafruit-circuitpython-mcp3xxx-1.4.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      416 2022-06-07 17:02:07.000000 adafruit-circuitpython-mcp3xxx-1.4.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:02:07.000000 adafruit-circuitpython-mcp3xxx-1.4.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5517 2022-06-07 17:02:07.000000 adafruit-circuitpython-mcp3xxx-1.4.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1010 2022-06-07 17:02:07.000000 adafruit-circuitpython-mcp3xxx-1.4.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:02:07.000000 adafruit-circuitpython-mcp3xxx-1.4.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      947 2022-06-07 17:02:07.000000 adafruit-circuitpython-mcp3xxx-1.4.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:02:07.000000 adafruit-circuitpython-mcp3xxx-1.4.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-07 17:02:07.000000 adafruit-circuitpython-mcp3xxx-1.4.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:02:23.443278 adafruit-circuitpython-mcp3xxx-1.4.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      642 2022-06-07 17:02:07.000000 adafruit-circuitpython-mcp3xxx-1.4.8/examples/mcp3xxx_mcp3002_differential_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      594 2022-06-07 17:02:07.000000 adafruit-circuitpython-mcp3xxx-1.4.8/examples/mcp3xxx_mcp3002_single_ended_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      642 2022-06-07 17:02:07.000000 adafruit-circuitpython-mcp3xxx-1.4.8/examples/mcp3xxx_mcp3004_differential_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      594 2022-06-07 17:02:07.000000 adafruit-circuitpython-mcp3xxx-1.4.8/examples/mcp3xxx_mcp3004_single_ended_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      642 2022-06-07 17:02:07.000000 adafruit-circuitpython-mcp3xxx-1.4.8/examples/mcp3xxx_mcp3008_differential_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      594 2022-06-07 17:02:07.000000 adafruit-circuitpython-mcp3xxx-1.4.8/examples/mcp3xxx_mcp3008_single_ended_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-06-07 17:02:07.000000 adafruit-circuitpython-mcp3xxx-1.4.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-07 17:02:23.443278 adafruit-circuitpython-mcp3xxx-1.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1843 2022-06-07 17:02:07.000000 adafruit-circuitpython-mcp3xxx-1.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:15:10.407953 adafruit-circuitpython-mcp3xxx-1.4.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:15:10.403953 adafruit-circuitpython-mcp3xxx-1.4.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:15:10.403953 adafruit-circuitpython-mcp3xxx-1.4.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-09 18:14:50.000000 adafruit-circuitpython-mcp3xxx-1.4.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:15:10.403953 adafruit-circuitpython-mcp3xxx-1.4.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-06-09 18:14:50.000000 adafruit-circuitpython-mcp3xxx-1.4.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-09 18:14:50.000000 adafruit-circuitpython-mcp3xxx-1.4.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-09 18:14:50.000000 adafruit-circuitpython-mcp3xxx-1.4.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-09 18:14:50.000000 adafruit-circuitpython-mcp3xxx-1.4.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-06-09 18:14:50.000000 adafruit-circuitpython-mcp3xxx-1.4.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-06-09 18:14:50.000000 adafruit-circuitpython-mcp3xxx-1.4.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-09 18:14:50.000000 adafruit-circuitpython-mcp3xxx-1.4.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-06-09 18:14:50.000000 adafruit-circuitpython-mcp3xxx-1.4.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1087 2022-06-09 18:14:50.000000 adafruit-circuitpython-mcp3xxx-1.4.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:15:10.403953 adafruit-circuitpython-mcp3xxx-1.4.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-09 18:14:50.000000 adafruit-circuitpython-mcp3xxx-1.4.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-09 18:14:50.000000 adafruit-circuitpython-mcp3xxx-1.4.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-09 18:14:50.000000 adafruit-circuitpython-mcp3xxx-1.4.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5869 2022-06-09 18:15:10.407953 adafruit-circuitpython-mcp3xxx-1.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5142 2022-06-09 18:14:50.000000 adafruit-circuitpython-mcp3xxx-1.4.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-09 18:14:50.000000 adafruit-circuitpython-mcp3xxx-1.4.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:15:10.407953 adafruit-circuitpython-mcp3xxx-1.4.9/adafruit_circuitpython_mcp3xxx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5869 2022-06-09 18:15:10.000000 adafruit-circuitpython-mcp3xxx-1.4.9/adafruit_circuitpython_mcp3xxx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1326 2022-06-09 18:15:10.000000 adafruit-circuitpython-mcp3xxx-1.4.9/adafruit_circuitpython_mcp3xxx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-09 18:15:10.000000 adafruit-circuitpython-mcp3xxx-1.4.9/adafruit_circuitpython_mcp3xxx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-06-09 18:15:10.000000 adafruit-circuitpython-mcp3xxx-1.4.9/adafruit_circuitpython_mcp3xxx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-06-09 18:15:10.000000 adafruit-circuitpython-mcp3xxx-1.4.9/adafruit_circuitpython_mcp3xxx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:15:10.407953 adafruit-circuitpython-mcp3xxx-1.4.9/adafruit_mcp3xxx/
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:14:50.000000 adafruit-circuitpython-mcp3xxx-1.4.9/adafruit_mcp3xxx/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2281 2022-06-09 18:14:50.000000 adafruit-circuitpython-mcp3xxx-1.4.9/adafruit_mcp3xxx/analog_in.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1429 2022-06-09 18:14:50.000000 adafruit-circuitpython-mcp3xxx-1.4.9/adafruit_mcp3xxx/mcp3002.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1232 2022-06-09 18:14:50.000000 adafruit-circuitpython-mcp3xxx-1.4.9/adafruit_mcp3xxx/mcp3004.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1504 2022-06-09 18:14:50.000000 adafruit-circuitpython-mcp3xxx-1.4.9/adafruit_mcp3xxx/mcp3008.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3281 2022-06-09 18:14:50.000000 adafruit-circuitpython-mcp3xxx-1.4.9/adafruit_mcp3xxx/mcp3xxx.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:15:10.407953 adafruit-circuitpython-mcp3xxx-1.4.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:15:10.407953 adafruit-circuitpython-mcp3xxx-1.4.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-09 18:14:50.000000 adafruit-circuitpython-mcp3xxx-1.4.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-09 18:14:50.000000 adafruit-circuitpython-mcp3xxx-1.4.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      416 2022-06-09 18:14:50.000000 adafruit-circuitpython-mcp3xxx-1.4.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:14:50.000000 adafruit-circuitpython-mcp3xxx-1.4.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5517 2022-06-09 18:14:50.000000 adafruit-circuitpython-mcp3xxx-1.4.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1010 2022-06-09 18:14:50.000000 adafruit-circuitpython-mcp3xxx-1.4.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:14:50.000000 adafruit-circuitpython-mcp3xxx-1.4.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1025 2022-06-09 18:14:50.000000 adafruit-circuitpython-mcp3xxx-1.4.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:14:50.000000 adafruit-circuitpython-mcp3xxx-1.4.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-09 18:14:50.000000 adafruit-circuitpython-mcp3xxx-1.4.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:15:10.407953 adafruit-circuitpython-mcp3xxx-1.4.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)      642 2022-06-09 18:14:50.000000 adafruit-circuitpython-mcp3xxx-1.4.9/examples/mcp3xxx_mcp3002_differential_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      594 2022-06-09 18:14:50.000000 adafruit-circuitpython-mcp3xxx-1.4.9/examples/mcp3xxx_mcp3002_single_ended_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      642 2022-06-09 18:14:50.000000 adafruit-circuitpython-mcp3xxx-1.4.9/examples/mcp3xxx_mcp3004_differential_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      594 2022-06-09 18:14:50.000000 adafruit-circuitpython-mcp3xxx-1.4.9/examples/mcp3xxx_mcp3004_single_ended_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      642 2022-06-09 18:14:50.000000 adafruit-circuitpython-mcp3xxx-1.4.9/examples/mcp3xxx_mcp3008_differential_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      594 2022-06-09 18:14:50.000000 adafruit-circuitpython-mcp3xxx-1.4.9/examples/mcp3xxx_mcp3008_single_ended_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2022-06-09 18:14:50.000000 adafruit-circuitpython-mcp3xxx-1.4.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-09 18:15:10.407953 adafruit-circuitpython-mcp3xxx-1.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1843 2022-06-09 18:14:50.000000 adafruit-circuitpython-mcp3xxx-1.4.9/setup.py
```

### Comparing `adafruit-circuitpython-mcp3xxx-1.4.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-mcp3xxx-1.4.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp3xxx-1.4.8/.github/workflows/build.yml` & `adafruit-circuitpython-mcp3xxx-1.4.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp3xxx-1.4.8/.github/workflows/release.yml` & `adafruit-circuitpython-mcp3xxx-1.4.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp3xxx-1.4.8/.gitignore` & `adafruit-circuitpython-mcp3xxx-1.4.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp3xxx-1.4.8/.pre-commit-config.yaml` & `adafruit-circuitpython-mcp3xxx-1.4.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp3xxx-1.4.8/.pylintrc` & `adafruit-circuitpython-mcp3xxx-1.4.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp3xxx-1.4.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-mcp3xxx-1.4.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp3xxx-1.4.8/LICENSE` & `adafruit-circuitpython-mcp3xxx-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp3xxx-1.4.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-mcp3xxx-1.4.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp3xxx-1.4.8/LICENSES/MIT.txt` & `adafruit-circuitpython-mcp3xxx-1.4.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp3xxx-1.4.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-mcp3xxx-1.4.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp3xxx-1.4.8/PKG-INFO` & `adafruit-circuitpython-mcp3xxx-1.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-mcp3xxx
-Version: 1.4.8
+Version: 1.4.9
 Summary: CircuitPython library for the MCP3xxx Analog-to-Digital converters.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_MCP3xxx
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit mcp3xxx hardware micropython circuitpython
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-mcp3xxx-1.4.8/README.rst` & `adafruit-circuitpython-mcp3xxx-1.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp3xxx-1.4.8/adafruit_circuitpython_mcp3xxx.egg-info/PKG-INFO` & `adafruit-circuitpython-mcp3xxx-1.4.9/adafruit_circuitpython_mcp3xxx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-mcp3xxx
-Version: 1.4.8
+Version: 1.4.9
 Summary: CircuitPython library for the MCP3xxx Analog-to-Digital converters.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_MCP3xxx
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit mcp3xxx hardware micropython circuitpython
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-mcp3xxx-1.4.8/adafruit_circuitpython_mcp3xxx.egg-info/SOURCES.txt` & `adafruit-circuitpython-mcp3xxx-1.4.9/adafruit_circuitpython_mcp3xxx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp3xxx-1.4.8/adafruit_mcp3xxx/analog_in.py` & `adafruit-circuitpython-mcp3xxx-1.4.9/adafruit_mcp3xxx/analog_in.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp3xxx-1.4.8/adafruit_mcp3xxx/mcp3002.py` & `adafruit-circuitpython-mcp3xxx-1.4.9/adafruit_mcp3xxx/mcp3002.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp3xxx-1.4.8/adafruit_mcp3xxx/mcp3004.py` & `adafruit-circuitpython-mcp3xxx-1.4.9/adafruit_mcp3xxx/mcp3004.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp3xxx-1.4.8/adafruit_mcp3xxx/mcp3008.py` & `adafruit-circuitpython-mcp3xxx-1.4.9/adafruit_mcp3xxx/mcp3008.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp3xxx-1.4.8/adafruit_mcp3xxx/mcp3xxx.py` & `adafruit-circuitpython-mcp3xxx-1.4.9/adafruit_mcp3xxx/mcp3xxx.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp3xxx-1.4.8/docs/_static/favicon.ico` & `adafruit-circuitpython-mcp3xxx-1.4.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp3xxx-1.4.8/docs/conf.py` & `adafruit-circuitpython-mcp3xxx-1.4.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp3xxx-1.4.8/docs/examples.rst` & `adafruit-circuitpython-mcp3xxx-1.4.9/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp3xxx-1.4.8/docs/index.rst` & `adafruit-circuitpython-mcp3xxx-1.4.9/docs/index.rst`

 * *Files 7% similar despite different names*

```diff
@@ -28,15 +28,16 @@
     :caption: Related Products
 
     MCP3008 <https://www.adafruit.com/product/856>
 
 .. toctree::
     :caption: Other Links
 
-    Download <https://github.com/adafruit/adafruit_CircuitPython_MCP3xxx/releases/latest>
+    Download from GitHub <https://github.com/adafruit/adafruit_CircuitPython_MCP3xxx/releases/latest>
+    Download Library Bundle <https://circuitpython.org/libraries>
     CircuitPython Reference Documentation <https://docs.circuitpython.org>
     CircuitPython Support Forum <https://forums.adafruit.com/viewforum.php?f=60>
     Discord Chat <https://adafru.it/discord>
     Adafruit Learning System <https://learn.adafruit.com>
     Adafruit Blog <https://blog.adafruit.com>
     Adafruit Store <https://www.adafruit.com>
```

### Comparing `adafruit-circuitpython-mcp3xxx-1.4.8/examples/mcp3xxx_mcp3002_differential_simpletest.py` & `adafruit-circuitpython-mcp3xxx-1.4.9/examples/mcp3xxx_mcp3002_differential_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp3xxx-1.4.8/examples/mcp3xxx_mcp3002_single_ended_simpletest.py` & `adafruit-circuitpython-mcp3xxx-1.4.9/examples/mcp3xxx_mcp3002_single_ended_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp3xxx-1.4.8/examples/mcp3xxx_mcp3004_differential_simpletest.py` & `adafruit-circuitpython-mcp3xxx-1.4.9/examples/mcp3xxx_mcp3004_differential_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp3xxx-1.4.8/examples/mcp3xxx_mcp3004_single_ended_simpletest.py` & `adafruit-circuitpython-mcp3xxx-1.4.9/examples/mcp3xxx_mcp3004_single_ended_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp3xxx-1.4.8/examples/mcp3xxx_mcp3008_differential_simpletest.py` & `adafruit-circuitpython-mcp3xxx-1.4.9/examples/mcp3xxx_mcp3008_differential_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp3xxx-1.4.8/examples/mcp3xxx_mcp3008_single_ended_simpletest.py` & `adafruit-circuitpython-mcp3xxx-1.4.9/examples/mcp3xxx_mcp3008_single_ended_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp3xxx-1.4.8/setup.py` & `adafruit-circuitpython-mcp3xxx-1.4.9/setup.py`

 * *Files identical despite different names*

