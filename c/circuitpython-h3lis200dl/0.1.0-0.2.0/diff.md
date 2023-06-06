# Comparing `tmp/circuitpython-h3lis200dl-0.1.0.tar.gz` & `tmp/circuitpython-h3lis200dl-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-h3lis200dl-0.1.0.tar", last modified: Sat Jun  3 21:40:54 2023, max compression
+gzip compressed data, was "circuitpython-h3lis200dl-0.2.0.tar", last modified: Tue Jun  6 00:20:00 2023, max compression
```

## Comparing `circuitpython-h3lis200dl-0.1.0.tar` & `circuitpython-h3lis200dl-0.2.0.tar`

### file list

```diff
@@ -1,41 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:40:54.510936 circuitpython-h3lis200dl-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:40:54.506936 circuitpython-h3lis200dl-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:40:54.506936 circuitpython-h3lis200dl-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-03 21:40:38.000000 circuitpython-h3lis200dl-0.1.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-03 21:40:38.000000 circuitpython-h3lis200dl-0.1.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-03 21:40:38.000000 circuitpython-h3lis200dl-0.1.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-03 21:40:38.000000 circuitpython-h3lis200dl-0.1.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-03 21:40:38.000000 circuitpython-h3lis200dl-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-03 21:40:38.000000 circuitpython-h3lis200dl-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-06-03 21:40:38.000000 circuitpython-h3lis200dl-0.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-03 21:40:38.000000 circuitpython-h3lis200dl-0.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-03 21:40:38.000000 circuitpython-h3lis200dl-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-06-03 21:40:54.510936 circuitpython-h3lis200dl-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-06-03 21:40:38.000000 circuitpython-h3lis200dl-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:40:54.506936 circuitpython-h3lis200dl-0.1.0/circuitpython_h3lis200dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-06-03 21:40:54.000000 circuitpython-h3lis200dl-0.1.0/circuitpython_h3lis200dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-03 21:40:54.000000 circuitpython-h3lis200dl-0.1.0/circuitpython_h3lis200dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 21:40:54.000000 circuitpython-h3lis200dl-0.1.0/circuitpython_h3lis200dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-03 21:40:54.000000 circuitpython-h3lis200dl-0.1.0/circuitpython_h3lis200dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-03 21:40:54.000000 circuitpython-h3lis200dl-0.1.0/circuitpython_h3lis200dl.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:40:54.510936 circuitpython-h3lis200dl-0.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:40:54.510936 circuitpython-h3lis200dl-0.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-03 21:40:38.000000 circuitpython-h3lis200dl-0.1.0/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-03 21:40:38.000000 circuitpython-h3lis200dl-0.1.0/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-03 21:40:38.000000 circuitpython-h3lis200dl-0.1.0/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-03 21:40:38.000000 circuitpython-h3lis200dl-0.1.0/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-03 21:40:38.000000 circuitpython-h3lis200dl-0.1.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-03 21:40:38.000000 circuitpython-h3lis200dl-0.1.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-03 21:40:38.000000 circuitpython-h3lis200dl-0.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-06-03 21:40:38.000000 circuitpython-h3lis200dl-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-03 21:40:38.000000 circuitpython-h3lis200dl-0.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-03 21:40:38.000000 circuitpython-h3lis200dl-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-03 21:40:38.000000 circuitpython-h3lis200dl-0.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 21:40:54.510936 circuitpython-h3lis200dl-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-03 21:40:46.000000 circuitpython-h3lis200dl-0.1.0/examples/h3lis200dl_full_scale_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-03 21:40:46.000000 circuitpython-h3lis200dl-0.1.0/examples/h3lis200dl_operation_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-03 21:40:46.000000 circuitpython-h3lis200dl-0.1.0/examples/h3lis200dl_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-06-03 21:40:46.000000 circuitpython-h3lis200dl-0.1.0/h3lis200dl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-03 21:40:46.000000 circuitpython-h3lis200dl-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-03 21:40:38.000000 circuitpython-h3lis200dl-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 21:40:54.510936 circuitpython-h3lis200dl-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:20:00.567702 circuitpython-h3lis200dl-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:20:00.563702 circuitpython-h3lis200dl-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:20:00.563702 circuitpython-h3lis200dl-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-06 00:19:45.000000 circuitpython-h3lis200dl-0.2.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-06 00:19:45.000000 circuitpython-h3lis200dl-0.2.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-06 00:19:45.000000 circuitpython-h3lis200dl-0.2.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-06 00:19:45.000000 circuitpython-h3lis200dl-0.2.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-06 00:19:45.000000 circuitpython-h3lis200dl-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-06 00:19:45.000000 circuitpython-h3lis200dl-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-06-06 00:19:45.000000 circuitpython-h3lis200dl-0.2.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-06 00:19:45.000000 circuitpython-h3lis200dl-0.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-06 00:19:45.000000 circuitpython-h3lis200dl-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-06-06 00:20:00.567702 circuitpython-h3lis200dl-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-06-06 00:19:45.000000 circuitpython-h3lis200dl-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:20:00.563702 circuitpython-h3lis200dl-0.2.0/circuitpython_h3lis200dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-06-06 00:20:00.000000 circuitpython-h3lis200dl-0.2.0/circuitpython_h3lis200dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-06 00:20:00.000000 circuitpython-h3lis200dl-0.2.0/circuitpython_h3lis200dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 00:20:00.000000 circuitpython-h3lis200dl-0.2.0/circuitpython_h3lis200dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-06 00:20:00.000000 circuitpython-h3lis200dl-0.2.0/circuitpython_h3lis200dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-06 00:20:00.000000 circuitpython-h3lis200dl-0.2.0/circuitpython_h3lis200dl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:20:00.567702 circuitpython-h3lis200dl-0.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:20:00.567702 circuitpython-h3lis200dl-0.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-06-06 00:19:45.000000 circuitpython-h3lis200dl-0.2.0/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-06 00:19:45.000000 circuitpython-h3lis200dl-0.2.0/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-06 00:19:45.000000 circuitpython-h3lis200dl-0.2.0/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-06 00:19:45.000000 circuitpython-h3lis200dl-0.2.0/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-06 00:19:45.000000 circuitpython-h3lis200dl-0.2.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-06 00:19:45.000000 circuitpython-h3lis200dl-0.2.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-06 00:19:45.000000 circuitpython-h3lis200dl-0.2.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-06-06 00:19:45.000000 circuitpython-h3lis200dl-0.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-06 00:19:45.000000 circuitpython-h3lis200dl-0.2.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-06 00:19:45.000000 circuitpython-h3lis200dl-0.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-06 00:19:45.000000 circuitpython-h3lis200dl-0.2.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:20:00.567702 circuitpython-h3lis200dl-0.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-06 00:19:52.000000 circuitpython-h3lis200dl-0.2.0/examples/h3lis200dl_data_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-06 00:19:52.000000 circuitpython-h3lis200dl-0.2.0/examples/h3lis200dl_full_scale_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-06 00:19:52.000000 circuitpython-h3lis200dl-0.2.0/examples/h3lis200dl_high_pass_filter_cutoff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-06 00:19:52.000000 circuitpython-h3lis200dl-0.2.0/examples/h3lis200dl_interrupt_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-06 00:19:52.000000 circuitpython-h3lis200dl-0.2.0/examples/h3lis200dl_operation_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-06 00:19:52.000000 circuitpython-h3lis200dl-0.2.0/examples/h3lis200dl_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18719 2023-06-06 00:19:52.000000 circuitpython-h3lis200dl-0.2.0/h3lis200dl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-06 00:19:52.000000 circuitpython-h3lis200dl-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-06 00:19:45.000000 circuitpython-h3lis200dl-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 00:20:00.567702 circuitpython-h3lis200dl-0.2.0/setup.cfg
```

### Comparing `circuitpython-h3lis200dl-0.1.0/.github/workflows/build.yml` & `circuitpython-h3lis200dl-0.2.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-h3lis200dl-0.1.0/.github/workflows/release_gh.yml` & `circuitpython-h3lis200dl-0.2.0/.github/workflows/release_gh.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-h3lis200dl-0.1.0/.gitignore` & `circuitpython-h3lis200dl-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-h3lis200dl-0.1.0/.pre-commit-config.yaml` & `circuitpython-h3lis200dl-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-h3lis200dl-0.1.0/.pylintrc` & `circuitpython-h3lis200dl-0.2.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-h3lis200dl-0.1.0/LICENSE` & `circuitpython-h3lis200dl-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-h3lis200dl-0.1.0/PKG-INFO` & `circuitpython-h3lis200dl-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-h3lis200dl
-Version: 0.1.0
+Version: 0.2.0
 Summary: CircuitPython Driver for the ST H3LIS200DL Accelerometer
 Author-email: JDM <xxx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_H3LIS200DL
 Keywords: sensor,blinka,circuitpython,micropython,h3lis200dl,acceleration,driver,H3LIS200DL,sensor
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -37,15 +37,15 @@
     :target: https://github.com/jposada202020/CircuitPython_H3LIS200DL/actions
     :alt: Build Status
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
-CircuitPython Driver for the ST H3LIS200DL Accelerometer
+CircuitPython Driver for the ST H3LIS200DL Accelerometer.
 
 
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
```

### Comparing `circuitpython-h3lis200dl-0.1.0/README.rst` & `circuitpython-h3lis200dl-0.2.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     :target: https://github.com/jposada202020/CircuitPython_H3LIS200DL/actions
     :alt: Build Status
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
-CircuitPython Driver for the ST H3LIS200DL Accelerometer
+CircuitPython Driver for the ST H3LIS200DL Accelerometer.
 
 
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
```

### Comparing `circuitpython-h3lis200dl-0.1.0/circuitpython_h3lis200dl.egg-info/PKG-INFO` & `circuitpython-h3lis200dl-0.2.0/circuitpython_h3lis200dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-h3lis200dl
-Version: 0.1.0
+Version: 0.2.0
 Summary: CircuitPython Driver for the ST H3LIS200DL Accelerometer
 Author-email: JDM <xxx@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_H3LIS200DL
 Keywords: sensor,blinka,circuitpython,micropython,h3lis200dl,acceleration,driver,H3LIS200DL,sensor
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -37,15 +37,15 @@
     :target: https://github.com/jposada202020/CircuitPython_H3LIS200DL/actions
     :alt: Build Status
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
     :alt: Code Style: Black
 
-CircuitPython Driver for the ST H3LIS200DL Accelerometer
+CircuitPython Driver for the ST H3LIS200DL Accelerometer.
 
 
 Dependencies
 =============
 This driver depends on:
 
 * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
```

### Comparing `circuitpython-h3lis200dl-0.1.0/circuitpython_h3lis200dl.egg-info/SOURCES.txt` & `circuitpython-h3lis200dl-0.2.0/circuitpython_h3lis200dl.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -23,10 +23,13 @@
 docs/requirements.txt
 docs/_static/Logo.png
 docs/_static/Logo.png.license
 docs/_static/extra_css.css
 docs/_static/extra_css.css.license
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
+examples/h3lis200dl_data_rate.py
 examples/h3lis200dl_full_scale_selection.py
+examples/h3lis200dl_high_pass_filter_cutoff.py
+examples/h3lis200dl_interrupt_example.py
 examples/h3lis200dl_operation_mode.py
 examples/h3lis200dl_simpletest.py
```

### Comparing `circuitpython-h3lis200dl-0.1.0/docs/_static/Logo.png` & `circuitpython-h3lis200dl-0.2.0/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `circuitpython-h3lis200dl-0.1.0/docs/_static/favicon.ico` & `circuitpython-h3lis200dl-0.2.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-h3lis200dl-0.1.0/docs/conf.py` & `circuitpython-h3lis200dl-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-h3lis200dl-0.1.0/examples/h3lis200dl_full_scale_selection.py` & `circuitpython-h3lis200dl-0.2.0/examples/h3lis200dl_full_scale_selection.py`

 * *Files identical despite different names*

### Comparing `circuitpython-h3lis200dl-0.1.0/examples/h3lis200dl_operation_mode.py` & `circuitpython-h3lis200dl-0.2.0/examples/h3lis200dl_operation_mode.py`

 * *Files identical despite different names*

### Comparing `circuitpython-h3lis200dl-0.1.0/pyproject.toml` & `circuitpython-h3lis200dl-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-h3lis200dl"
 description = "CircuitPython Driver for the ST H3LIS200DL Accelerometer"
-version = "0.1.0"
+version = "0.2.0"
 readme = "README.rst"
 authors = [
     {name = "JDM", email = "xxx@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/CircuitPython_H3LIS200DL"}
 keywords = [
     "sensor",
```

