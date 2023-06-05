# Comparing `tmp/adafruit-circuitpython-matrixkeypad-1.2.8.tar.gz` & `tmp/adafruit-circuitpython-matrixkeypad-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-matrixkeypad-1.2.8.tar", last modified: Tue Jun  7 17:09:43 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-matrixkeypad-1.2.9.tar", last modified: Thu Jun  9 18:28:51 2022, max compression
```

## Comparing `adafruit-circuitpython-matrixkeypad-1.2.8.tar` & `adafruit-circuitpython-matrixkeypad-1.2.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:09:43.596800 adafruit-circuitpython-matrixkeypad-1.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:09:43.592800 adafruit-circuitpython-matrixkeypad-1.2.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:09:43.592800 adafruit-circuitpython-matrixkeypad-1.2.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-07 17:09:30.000000 adafruit-circuitpython-matrixkeypad-1.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:09:43.592800 adafruit-circuitpython-matrixkeypad-1.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-06-07 17:09:30.000000 adafruit-circuitpython-matrixkeypad-1.2.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-07 17:09:30.000000 adafruit-circuitpython-matrixkeypad-1.2.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-07 17:09:30.000000 adafruit-circuitpython-matrixkeypad-1.2.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-07 17:09:30.000000 adafruit-circuitpython-matrixkeypad-1.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-06-07 17:09:30.000000 adafruit-circuitpython-matrixkeypad-1.2.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-06-07 17:09:30.000000 adafruit-circuitpython-matrixkeypad-1.2.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-07 17:09:30.000000 adafruit-circuitpython-matrixkeypad-1.2.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-06-07 17:09:30.000000 adafruit-circuitpython-matrixkeypad-1.2.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1087 2022-06-07 17:09:30.000000 adafruit-circuitpython-matrixkeypad-1.2.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:09:43.596800 adafruit-circuitpython-matrixkeypad-1.2.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-07 17:09:30.000000 adafruit-circuitpython-matrixkeypad-1.2.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-07 17:09:30.000000 adafruit-circuitpython-matrixkeypad-1.2.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-07 17:09:30.000000 adafruit-circuitpython-matrixkeypad-1.2.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3661 2022-06-07 17:09:43.596800 adafruit-circuitpython-matrixkeypad-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2936 2022-06-07 17:09:30.000000 adafruit-circuitpython-matrixkeypad-1.2.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-07 17:09:30.000000 adafruit-circuitpython-matrixkeypad-1.2.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:09:43.596800 adafruit-circuitpython-matrixkeypad-1.2.8/adafruit_circuitpython_matrixkeypad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3661 2022-06-07 17:09:43.000000 adafruit-circuitpython-matrixkeypad-1.2.8/adafruit_circuitpython_matrixkeypad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      998 2022-06-07 17:09:43.000000 adafruit-circuitpython-matrixkeypad-1.2.8/adafruit_circuitpython_matrixkeypad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-07 17:09:43.000000 adafruit-circuitpython-matrixkeypad-1.2.8/adafruit_circuitpython_matrixkeypad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-06-07 17:09:43.000000 adafruit-circuitpython-matrixkeypad-1.2.8/adafruit_circuitpython_matrixkeypad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-06-07 17:09:43.000000 adafruit-circuitpython-matrixkeypad-1.2.8/adafruit_circuitpython_matrixkeypad.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2548 2022-06-07 17:09:30.000000 adafruit-circuitpython-matrixkeypad-1.2.8/adafruit_matrixkeypad.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:09:43.596800 adafruit-circuitpython-matrixkeypad-1.2.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:09:43.596800 adafruit-circuitpython-matrixkeypad-1.2.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-07 17:09:30.000000 adafruit-circuitpython-matrixkeypad-1.2.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-07 17:09:30.000000 adafruit-circuitpython-matrixkeypad-1.2.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      271 2022-06-07 17:09:30.000000 adafruit-circuitpython-matrixkeypad-1.2.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:09:30.000000 adafruit-circuitpython-matrixkeypad-1.2.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5726 2022-06-07 17:09:30.000000 adafruit-circuitpython-matrixkeypad-1.2.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-06-07 17:09:30.000000 adafruit-circuitpython-matrixkeypad-1.2.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:09:30.000000 adafruit-circuitpython-matrixkeypad-1.2.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      899 2022-06-07 17:09:30.000000 adafruit-circuitpython-matrixkeypad-1.2.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:09:30.000000 adafruit-circuitpython-matrixkeypad-1.2.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-07 17:09:30.000000 adafruit-circuitpython-matrixkeypad-1.2.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:09:43.596800 adafruit-circuitpython-matrixkeypad-1.2.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      614 2022-06-07 17:09:30.000000 adafruit-circuitpython-matrixkeypad-1.2.8/examples/matrixkeypad_4x4.py
--rw-r--r--   0 runner    (1001) docker     (121)      931 2022-06-07 17:09:30.000000 adafruit-circuitpython-matrixkeypad-1.2.8/examples/matrixkeypad_rpi_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      963 2022-06-07 17:09:30.000000 adafruit-circuitpython-matrixkeypad-1.2.8/examples/matrixkeypad_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-06-07 17:09:30.000000 adafruit-circuitpython-matrixkeypad-1.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-07 17:09:43.596800 adafruit-circuitpython-matrixkeypad-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1812 2022-06-07 17:09:30.000000 adafruit-circuitpython-matrixkeypad-1.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:28:51.837632 adafruit-circuitpython-matrixkeypad-1.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:28:51.825631 adafruit-circuitpython-matrixkeypad-1.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:28:51.829631 adafruit-circuitpython-matrixkeypad-1.2.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-09 18:28:42.000000 adafruit-circuitpython-matrixkeypad-1.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:28:51.829631 adafruit-circuitpython-matrixkeypad-1.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-06-09 18:28:42.000000 adafruit-circuitpython-matrixkeypad-1.2.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-09 18:28:42.000000 adafruit-circuitpython-matrixkeypad-1.2.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-09 18:28:42.000000 adafruit-circuitpython-matrixkeypad-1.2.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-09 18:28:42.000000 adafruit-circuitpython-matrixkeypad-1.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-06-09 18:28:42.000000 adafruit-circuitpython-matrixkeypad-1.2.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-06-09 18:28:42.000000 adafruit-circuitpython-matrixkeypad-1.2.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-09 18:28:42.000000 adafruit-circuitpython-matrixkeypad-1.2.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-06-09 18:28:42.000000 adafruit-circuitpython-matrixkeypad-1.2.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1087 2022-06-09 18:28:42.000000 adafruit-circuitpython-matrixkeypad-1.2.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:28:51.829631 adafruit-circuitpython-matrixkeypad-1.2.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-09 18:28:42.000000 adafruit-circuitpython-matrixkeypad-1.2.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-09 18:28:42.000000 adafruit-circuitpython-matrixkeypad-1.2.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-09 18:28:42.000000 adafruit-circuitpython-matrixkeypad-1.2.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3661 2022-06-09 18:28:51.837632 adafruit-circuitpython-matrixkeypad-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2936 2022-06-09 18:28:42.000000 adafruit-circuitpython-matrixkeypad-1.2.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-09 18:28:42.000000 adafruit-circuitpython-matrixkeypad-1.2.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:28:51.833632 adafruit-circuitpython-matrixkeypad-1.2.9/adafruit_circuitpython_matrixkeypad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3661 2022-06-09 18:28:51.000000 adafruit-circuitpython-matrixkeypad-1.2.9/adafruit_circuitpython_matrixkeypad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      998 2022-06-09 18:28:51.000000 adafruit-circuitpython-matrixkeypad-1.2.9/adafruit_circuitpython_matrixkeypad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-09 18:28:51.000000 adafruit-circuitpython-matrixkeypad-1.2.9/adafruit_circuitpython_matrixkeypad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-06-09 18:28:51.000000 adafruit-circuitpython-matrixkeypad-1.2.9/adafruit_circuitpython_matrixkeypad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-06-09 18:28:51.000000 adafruit-circuitpython-matrixkeypad-1.2.9/adafruit_circuitpython_matrixkeypad.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2548 2022-06-09 18:28:42.000000 adafruit-circuitpython-matrixkeypad-1.2.9/adafruit_matrixkeypad.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:28:51.833632 adafruit-circuitpython-matrixkeypad-1.2.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:28:51.833632 adafruit-circuitpython-matrixkeypad-1.2.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-09 18:28:42.000000 adafruit-circuitpython-matrixkeypad-1.2.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-09 18:28:42.000000 adafruit-circuitpython-matrixkeypad-1.2.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      271 2022-06-09 18:28:42.000000 adafruit-circuitpython-matrixkeypad-1.2.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:28:42.000000 adafruit-circuitpython-matrixkeypad-1.2.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5726 2022-06-09 18:28:42.000000 adafruit-circuitpython-matrixkeypad-1.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      198 2022-06-09 18:28:42.000000 adafruit-circuitpython-matrixkeypad-1.2.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:28:42.000000 adafruit-circuitpython-matrixkeypad-1.2.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      977 2022-06-09 18:28:42.000000 adafruit-circuitpython-matrixkeypad-1.2.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:28:42.000000 adafruit-circuitpython-matrixkeypad-1.2.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-09 18:28:42.000000 adafruit-circuitpython-matrixkeypad-1.2.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:28:51.837632 adafruit-circuitpython-matrixkeypad-1.2.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)      614 2022-06-09 18:28:42.000000 adafruit-circuitpython-matrixkeypad-1.2.9/examples/matrixkeypad_4x4.py
+-rw-r--r--   0 runner    (1001) docker     (121)      931 2022-06-09 18:28:42.000000 adafruit-circuitpython-matrixkeypad-1.2.9/examples/matrixkeypad_rpi_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      963 2022-06-09 18:28:42.000000 adafruit-circuitpython-matrixkeypad-1.2.9/examples/matrixkeypad_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      119 2022-06-09 18:28:42.000000 adafruit-circuitpython-matrixkeypad-1.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-09 18:28:51.837632 adafruit-circuitpython-matrixkeypad-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1812 2022-06-09 18:28:42.000000 adafruit-circuitpython-matrixkeypad-1.2.9/setup.py
```

### Comparing `adafruit-circuitpython-matrixkeypad-1.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-matrixkeypad-1.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixkeypad-1.2.8/.github/workflows/build.yml` & `adafruit-circuitpython-matrixkeypad-1.2.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixkeypad-1.2.8/.github/workflows/release.yml` & `adafruit-circuitpython-matrixkeypad-1.2.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixkeypad-1.2.8/.gitignore` & `adafruit-circuitpython-matrixkeypad-1.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixkeypad-1.2.8/.pre-commit-config.yaml` & `adafruit-circuitpython-matrixkeypad-1.2.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixkeypad-1.2.8/.pylintrc` & `adafruit-circuitpython-matrixkeypad-1.2.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixkeypad-1.2.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-matrixkeypad-1.2.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixkeypad-1.2.8/LICENSE` & `adafruit-circuitpython-matrixkeypad-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixkeypad-1.2.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-matrixkeypad-1.2.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixkeypad-1.2.8/LICENSES/MIT.txt` & `adafruit-circuitpython-matrixkeypad-1.2.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixkeypad-1.2.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-matrixkeypad-1.2.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixkeypad-1.2.8/PKG-INFO` & `adafruit-circuitpython-matrixkeypad-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-matrixkeypad
-Version: 1.2.8
+Version: 1.2.9
 Summary: CircuitPython library for passive matrix keypads.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_MatrixKeypad
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit matrix keypad hardware micropython circuitpython
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-matrixkeypad-1.2.8/README.rst` & `adafruit-circuitpython-matrixkeypad-1.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixkeypad-1.2.8/adafruit_circuitpython_matrixkeypad.egg-info/PKG-INFO` & `adafruit-circuitpython-matrixkeypad-1.2.9/adafruit_circuitpython_matrixkeypad.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-matrixkeypad
-Version: 1.2.8
+Version: 1.2.9
 Summary: CircuitPython library for passive matrix keypads.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_MatrixKeypad
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit matrix keypad hardware micropython circuitpython
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-matrixkeypad-1.2.8/adafruit_circuitpython_matrixkeypad.egg-info/SOURCES.txt` & `adafruit-circuitpython-matrixkeypad-1.2.9/adafruit_circuitpython_matrixkeypad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixkeypad-1.2.8/adafruit_matrixkeypad.py` & `adafruit-circuitpython-matrixkeypad-1.2.9/adafruit_matrixkeypad.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixkeypad-1.2.8/docs/_static/favicon.ico` & `adafruit-circuitpython-matrixkeypad-1.2.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixkeypad-1.2.8/docs/conf.py` & `adafruit-circuitpython-matrixkeypad-1.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixkeypad-1.2.8/docs/index.rst` & `adafruit-circuitpython-matrixkeypad-1.2.9/docs/index.rst`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 
 .. toctree::
     :caption: Related Products
 
 .. toctree::
     :caption: Other Links
 
-    Download <https://github.com/adafruit/adafruit_CircuitPython_MatrixKeypad/releases/latest>
+    Download from GitHub <https://github.com/adafruit/adafruit_CircuitPython_MatrixKeypad/releases/latest>
+    Download Library Bundle <https://circuitpython.org/libraries>
     CircuitPython Reference Documentation <https://docs.circuitpython.org>
     CircuitPython Support Forum <https://forums.adafruit.com/viewforum.php?f=60>
     Discord Chat <https://adafru.it/discord>
     Adafruit Learning System <https://learn.adafruit.com>
     Adafruit Blog <https://blog.adafruit.com>
     Adafruit Store <https://www.adafruit.com>
```

### Comparing `adafruit-circuitpython-matrixkeypad-1.2.8/examples/matrixkeypad_4x4.py` & `adafruit-circuitpython-matrixkeypad-1.2.9/examples/matrixkeypad_4x4.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixkeypad-1.2.8/examples/matrixkeypad_rpi_simpletest.py` & `adafruit-circuitpython-matrixkeypad-1.2.9/examples/matrixkeypad_rpi_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixkeypad-1.2.8/examples/matrixkeypad_simpletest.py` & `adafruit-circuitpython-matrixkeypad-1.2.9/examples/matrixkeypad_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-matrixkeypad-1.2.8/setup.py` & `adafruit-circuitpython-matrixkeypad-1.2.9/setup.py`

 * *Files identical despite different names*

