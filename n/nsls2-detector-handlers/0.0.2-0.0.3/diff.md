# Comparing `tmp/nsls2-detector-handlers-0.0.2.tar.gz` & `tmp/nsls2-detector-handlers-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nsls2-detector-handlers-0.0.2.tar", last modified: Wed Jul  1 17:32:49 2020, max compression
+gzip compressed data, was "nsls2-detector-handlers-0.0.3.tar", last modified: Tue Jun  6 14:55:18 2023, max compression
```

## Comparing `nsls2-detector-handlers-0.0.2.tar` & `nsls2-detector-handlers-0.0.3.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 mhart     (1002) mhart     (1003)        0 2020-07-01 17:32:49.000000 nsls2-detector-handlers-0.0.2/
--rw-r--r--   0 mhart     (1002) mhart     (1003)      166 2020-07-01 17:22:04.000000 nsls2-detector-handlers-0.0.2/AUTHORS.rst
--rw-r--r--   0 mhart     (1002) mhart     (1003)     3199 2020-07-01 17:22:04.000000 nsls2-detector-handlers-0.0.2/CONTRIBUTING.rst
--rw-r--r--   0 mhart     (1002) mhart     (1003)     1538 2020-07-01 17:22:04.000000 nsls2-detector-handlers-0.0.2/LICENSE
--rw-r--r--   0 mhart     (1002) mhart     (1003)      376 2020-07-01 17:22:04.000000 nsls2-detector-handlers-0.0.2/MANIFEST.in
--rw-r--r--   0 mhart     (1002) mhart     (1003)     1183 2020-07-01 17:32:49.000000 nsls2-detector-handlers-0.0.2/PKG-INFO
--rw-r--r--   0 mhart     (1002) mhart     (1003)      558 2020-07-01 17:22:04.000000 nsls2-detector-handlers-0.0.2/README.rst
-drwxr-xr-x   0 mhart     (1002) mhart     (1003)        0 2020-07-01 17:32:49.000000 nsls2-detector-handlers-0.0.2/docs/
--rw-r--r--   0 mhart     (1002) mhart     (1003)      673 2020-07-01 17:22:04.000000 nsls2-detector-handlers-0.0.2/docs/Makefile
--rw-r--r--   0 mhart     (1002) mhart     (1003)      797 2020-07-01 17:22:04.000000 nsls2-detector-handlers-0.0.2/docs/make.bat
-drwxr-xr-x   0 mhart     (1002) mhart     (1003)        0 2020-07-01 17:32:49.000000 nsls2-detector-handlers-0.0.2/docs/source/
--rw-r--r--   0 mhart     (1002) mhart     (1003)     6552 2020-07-01 17:22:04.000000 nsls2-detector-handlers-0.0.2/docs/source/conf.py
--rw-r--r--   0 mhart     (1002) mhart     (1003)      405 2020-07-01 17:22:04.000000 nsls2-detector-handlers-0.0.2/docs/source/index.rst
--rw-r--r--   0 mhart     (1002) mhart     (1003)      105 2020-07-01 17:22:04.000000 nsls2-detector-handlers-0.0.2/docs/source/installation.rst
--rw-r--r--   0 mhart     (1002) mhart     (1003)     1083 2020-07-01 17:22:04.000000 nsls2-detector-handlers-0.0.2/docs/source/min_versions.rst
--rw-r--r--   0 mhart     (1002) mhart     (1003)      107 2020-07-01 17:22:04.000000 nsls2-detector-handlers-0.0.2/docs/source/release-history.rst
--rw-r--r--   0 mhart     (1002) mhart     (1003)      123 2020-07-01 17:22:04.000000 nsls2-detector-handlers-0.0.2/docs/source/usage.rst
-drwxr-xr-x   0 mhart     (1002) mhart     (1003)        0 2020-07-01 17:32:49.000000 nsls2-detector-handlers-0.0.2/nsls2_detector_handlers/
--rw-r--r--   0 mhart     (1002) mhart     (1003)      581 2020-07-01 17:22:04.000000 nsls2-detector-handlers-0.0.2/nsls2_detector_handlers/__init__.py
--rw-r--r--   0 mhart     (1002) mhart     (1003)      497 2020-07-01 17:32:49.000000 nsls2-detector-handlers-0.0.2/nsls2_detector_handlers/_version.py
--rw-r--r--   0 mhart     (1002) mhart     (1003)     2440 2020-07-01 17:22:04.000000 nsls2-detector-handlers-0.0.2/nsls2_detector_handlers/electrometer.py
--rw-r--r--   0 mhart     (1002) mhart     (1003)     3347 2020-07-01 17:22:04.000000 nsls2-detector-handlers-0.0.2/nsls2_detector_handlers/pizzabox.py
--rw-r--r--   0 mhart     (1002) mhart     (1003)      405 2020-07-01 17:22:04.000000 nsls2-detector-handlers-0.0.2/nsls2_detector_handlers/srx_flyscans.py
-drwxr-xr-x   0 mhart     (1002) mhart     (1003)        0 2020-07-01 17:32:49.000000 nsls2-detector-handlers-0.0.2/nsls2_detector_handlers/tests/
--rw-r--r--   0 mhart     (1002) mhart     (1003)        0 2020-07-01 17:22:04.000000 nsls2-detector-handlers-0.0.2/nsls2_detector_handlers/tests/__init__.py
--rw-r--r--   0 mhart     (1002) mhart     (1003)        0 2020-07-01 17:22:04.000000 nsls2-detector-handlers-0.0.2/nsls2_detector_handlers/tests/conftest.py
--rw-r--r--   0 mhart     (1002) mhart     (1003)       99 2020-07-01 17:22:04.000000 nsls2-detector-handlers-0.0.2/nsls2_detector_handlers/tests/test_examples.py
-drwxr-xr-x   0 mhart     (1002) mhart     (1003)        0 2020-07-01 17:32:49.000000 nsls2-detector-handlers-0.0.2/nsls2_detector_handlers.egg-info/
--rw-r--r--   0 mhart     (1002) mhart     (1003)     1183 2020-07-01 17:32:49.000000 nsls2-detector-handlers-0.0.2/nsls2_detector_handlers.egg-info/PKG-INFO
--rw-r--r--   0 mhart     (1002) mhart     (1003)      894 2020-07-01 17:32:49.000000 nsls2-detector-handlers-0.0.2/nsls2_detector_handlers.egg-info/SOURCES.txt
--rw-r--r--   0 mhart     (1002) mhart     (1003)        1 2020-07-01 17:32:49.000000 nsls2-detector-handlers-0.0.2/nsls2_detector_handlers.egg-info/dependency_links.txt
--rw-r--r--   0 mhart     (1002) mhart     (1003)      717 2020-07-01 17:32:49.000000 nsls2-detector-handlers-0.0.2/nsls2_detector_handlers.egg-info/entry_points.txt
--rw-r--r--   0 mhart     (1002) mhart     (1003)       18 2020-07-01 17:32:49.000000 nsls2-detector-handlers-0.0.2/nsls2_detector_handlers.egg-info/requires.txt
--rw-r--r--   0 mhart     (1002) mhart     (1003)       24 2020-07-01 17:32:49.000000 nsls2-detector-handlers-0.0.2/nsls2_detector_handlers.egg-info/top_level.txt
--rw-r--r--   0 mhart     (1002) mhart     (1003)       71 2020-07-01 17:22:04.000000 nsls2-detector-handlers-0.0.2/requirements.txt
--rw-r--r--   0 mhart     (1002) mhart     (1003)      210 2020-07-01 17:32:49.000000 nsls2-detector-handlers-0.0.2/setup.cfg
--rw-r--r--   0 mhart     (1002) mhart     (1003)     2989 2020-07-01 17:22:04.000000 nsls2-detector-handlers-0.0.2/setup.py
--rw-r--r--   0 mhart     (1002) mhart     (1003)    68611 2020-07-01 17:22:04.000000 nsls2-detector-handlers-0.0.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:55:18.350795 nsls2-detector-handlers-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-06 14:55:10.000000 nsls2-detector-handlers-0.0.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-06-06 14:55:10.000000 nsls2-detector-handlers-0.0.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-06 14:55:10.000000 nsls2-detector-handlers-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-06 14:55:10.000000 nsls2-detector-handlers-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-06 14:55:18.350795 nsls2-detector-handlers-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-06 14:55:10.000000 nsls2-detector-handlers-0.0.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:55:18.346795 nsls2-detector-handlers-0.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-06 14:55:10.000000 nsls2-detector-handlers-0.0.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-06 14:55:10.000000 nsls2-detector-handlers-0.0.3/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:55:18.346795 nsls2-detector-handlers-0.0.3/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-06-06 14:55:10.000000 nsls2-detector-handlers-0.0.3/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-06 14:55:10.000000 nsls2-detector-handlers-0.0.3/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-06 14:55:10.000000 nsls2-detector-handlers-0.0.3/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-06 14:55:10.000000 nsls2-detector-handlers-0.0.3/docs/source/min_versions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-06 14:55:10.000000 nsls2-detector-handlers-0.0.3/docs/source/release-history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-06 14:55:10.000000 nsls2-detector-handlers-0.0.3/docs/source/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:55:18.350795 nsls2-detector-handlers-0.0.3/nsls2_detector_handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-06 14:55:10.000000 nsls2-detector-handlers-0.0.3/nsls2_detector_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-06 14:55:18.350795 nsls2-detector-handlers-0.0.3/nsls2_detector_handlers/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-06-06 14:55:10.000000 nsls2-detector-handlers-0.0.3/nsls2_detector_handlers/electrometer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-06-06 14:55:10.000000 nsls2-detector-handlers-0.0.3/nsls2_detector_handlers/pizzabox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-06 14:55:10.000000 nsls2-detector-handlers-0.0.3/nsls2_detector_handlers/srx_flyscans.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:55:18.350795 nsls2-detector-handlers-0.0.3/nsls2_detector_handlers/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:55:10.000000 nsls2-detector-handlers-0.0.3/nsls2_detector_handlers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:55:10.000000 nsls2-detector-handlers-0.0.3/nsls2_detector_handlers/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-06 14:55:10.000000 nsls2-detector-handlers-0.0.3/nsls2_detector_handlers/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-06 14:55:10.000000 nsls2-detector-handlers-0.0.3/nsls2_detector_handlers/webcam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:55:18.350795 nsls2-detector-handlers-0.0.3/nsls2_detector_handlers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-06 14:55:18.000000 nsls2-detector-handlers-0.0.3/nsls2_detector_handlers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-06 14:55:18.000000 nsls2-detector-handlers-0.0.3/nsls2_detector_handlers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 14:55:18.000000 nsls2-detector-handlers-0.0.3/nsls2_detector_handlers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-06 14:55:18.000000 nsls2-detector-handlers-0.0.3/nsls2_detector_handlers.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-06 14:55:18.000000 nsls2-detector-handlers-0.0.3/nsls2_detector_handlers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-06 14:55:18.000000 nsls2-detector-handlers-0.0.3/nsls2_detector_handlers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-06 14:55:10.000000 nsls2-detector-handlers-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-06 14:55:18.350795 nsls2-detector-handlers-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-06-06 14:55:10.000000 nsls2-detector-handlers-0.0.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68573 2023-06-06 14:55:10.000000 nsls2-detector-handlers-0.0.3/versioneer.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `nsls2-detector-handlers-0.0.2/CONTRIBUTING.rst` & `nsls2-detector-handlers-0.0.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nsls2-detector-handlers-0.0.2/LICENSE` & `nsls2-detector-handlers-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nsls2-detector-handlers-0.0.2/PKG-INFO` & `nsls2-detector-handlers-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: nsls2-detector-handlers
-Version: 0.0.2
+Version: 0.0.3
 Summary: Staging repo for handlers specific to NSLS-II
 Home-page: https://github.com/bluesky/nsls2-detector-handlers
 Author: Brookhaven National Laboratory
 Author-email: dama@bnl.gov
 License: BSD (3-clause)
-Description: =======================
-        nsls2-detector-handlers
-        =======================
-        
-        .. image:: https://img.shields.io/travis/bluesky/nsls2-detector-handlers.svg
-                :target: https://travis-ci.org/bluesky/nsls2-detector-handlers
-        
-        .. image:: https://img.shields.io/pypi/v/nsls2-detector-handlers.svg
-                :target: https://pypi.python.org/pypi/nsls2-detector-handlers
-        
-        
-        Staging repo for handlers specific to NSLS-II
-        
-        * Free software: 3-clause BSD license
-        * Documentation: (COMING SOON!) https://bluesky.github.io/nsls2-detector-handlers.
-        
-        Features
-        --------
-        
-        * TODO
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+=======================
+nsls2-detector-handlers
+=======================
+
+.. image:: https://img.shields.io/travis/bluesky/nsls2-detector-handlers.svg
+        :target: https://travis-ci.org/bluesky/nsls2-detector-handlers
+
+.. image:: https://img.shields.io/pypi/v/nsls2-detector-handlers.svg
+        :target: https://pypi.python.org/pypi/nsls2-detector-handlers
+
+
+Staging repo for handlers specific to NSLS-II
+
+* Free software: 3-clause BSD license
+* Documentation: (COMING SOON!) https://bluesky.github.io/nsls2-detector-handlers.
+
+Features
+--------
+
+* TODO
```

### Comparing `nsls2-detector-handlers-0.0.2/README.rst` & `nsls2-detector-handlers-0.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `nsls2-detector-handlers-0.0.2/docs/Makefile` & `nsls2-detector-handlers-0.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nsls2-detector-handlers-0.0.2/docs/make.bat` & `nsls2-detector-handlers-0.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nsls2-detector-handlers-0.0.2/docs/source/conf.py` & `nsls2-detector-handlers-0.0.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nsls2-detector-handlers-0.0.2/docs/source/min_versions.rst` & `nsls2-detector-handlers-0.0.3/docs/source/min_versions.rst`

 * *Files identical despite different names*

### Comparing `nsls2-detector-handlers-0.0.2/nsls2_detector_handlers/__init__.py` & `nsls2-detector-handlers-0.0.3/nsls2_detector_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `nsls2-detector-handlers-0.0.2/nsls2_detector_handlers/electrometer.py` & `nsls2-detector-handlers-0.0.3/nsls2_detector_handlers/electrometer.py`

 * *Files identical despite different names*

### Comparing `nsls2-detector-handlers-0.0.2/nsls2_detector_handlers/pizzabox.py` & `nsls2-detector-handlers-0.0.3/nsls2_detector_handlers/pizzabox.py`

 * *Files identical despite different names*

### Comparing `nsls2-detector-handlers-0.0.2/nsls2_detector_handlers.egg-info/PKG-INFO` & `nsls2-detector-handlers-0.0.3/nsls2_detector_handlers.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,35 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: nsls2-detector-handlers
-Version: 0.0.2
+Version: 0.0.3
 Summary: Staging repo for handlers specific to NSLS-II
 Home-page: https://github.com/bluesky/nsls2-detector-handlers
 Author: Brookhaven National Laboratory
 Author-email: dama@bnl.gov
 License: BSD (3-clause)
-Description: =======================
-        nsls2-detector-handlers
-        =======================
-        
-        .. image:: https://img.shields.io/travis/bluesky/nsls2-detector-handlers.svg
-                :target: https://travis-ci.org/bluesky/nsls2-detector-handlers
-        
-        .. image:: https://img.shields.io/pypi/v/nsls2-detector-handlers.svg
-                :target: https://pypi.python.org/pypi/nsls2-detector-handlers
-        
-        
-        Staging repo for handlers specific to NSLS-II
-        
-        * Free software: 3-clause BSD license
-        * Documentation: (COMING SOON!) https://bluesky.github.io/nsls2-detector-handlers.
-        
-        Features
-        --------
-        
-        * TODO
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+=======================
+nsls2-detector-handlers
+=======================
+
+.. image:: https://img.shields.io/travis/bluesky/nsls2-detector-handlers.svg
+        :target: https://travis-ci.org/bluesky/nsls2-detector-handlers
+
+.. image:: https://img.shields.io/pypi/v/nsls2-detector-handlers.svg
+        :target: https://pypi.python.org/pypi/nsls2-detector-handlers
+
+
+Staging repo for handlers specific to NSLS-II
+
+* Free software: 3-clause BSD license
+* Documentation: (COMING SOON!) https://bluesky.github.io/nsls2-detector-handlers.
+
+Features
+--------
+
+* TODO
```

### Comparing `nsls2-detector-handlers-0.0.2/nsls2_detector_handlers.egg-info/SOURCES.txt` & `nsls2-detector-handlers-0.0.3/nsls2_detector_handlers.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 docs/source/release-history.rst
 docs/source/usage.rst
 nsls2_detector_handlers/__init__.py
 nsls2_detector_handlers/_version.py
 nsls2_detector_handlers/electrometer.py
 nsls2_detector_handlers/pizzabox.py
 nsls2_detector_handlers/srx_flyscans.py
+nsls2_detector_handlers/webcam.py
 nsls2_detector_handlers.egg-info/PKG-INFO
 nsls2_detector_handlers.egg-info/SOURCES.txt
 nsls2_detector_handlers.egg-info/dependency_links.txt
 nsls2_detector_handlers.egg-info/entry_points.txt
 nsls2_detector_handlers.egg-info/requires.txt
 nsls2_detector_handlers.egg-info/top_level.txt
 nsls2_detector_handlers/tests/__init__.py
```

### Comparing `nsls2-detector-handlers-0.0.2/nsls2_detector_handlers.egg-info/entry_points.txt` & `nsls2-detector-handlers-0.0.3/nsls2_detector_handlers.egg-info/entry_points.txt`

 * *Files 0% similar despite different names*

```diff
@@ -4,8 +4,7 @@
 PIZZABOX_AN_FILE_TXT_PD = nsls2_detector_handlers.pizzabox:PizzaBoxAnHandlerTxtPD
 PIZZABOX_DI_FILE_TXT = nsls2_detector_handlers.pizzabox:PizzaBoxDIHandlerTxt
 PIZZABOX_DI_FILE_TXT_PD = nsls2_detector_handlers.pizzabox:PizzaBoxDIHandlerTxtPD
 PIZZABOX_ENC_FILE_TXT = nsls2_detector_handlers.pizzabox:PizzaBoxEncHandlerTxt
 PIZZABOX_ENC_FILE_TXT_PD = nsls2_detector_handlers.pizzabox:PizzaBoxEncHandlerTxtPD
 SIS_HDF51 = nsls2_detector_handlers.srx_flyscans:ZebraHDF5Handler
 ZEBRA_HDF51 = nsls2_detector_handlers.srx_flyscans:ZebraHDF5Handler
-
```

### Comparing `nsls2-detector-handlers-0.0.2/setup.py` & `nsls2-detector-handlers-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `nsls2-detector-handlers-0.0.2/versioneer.py` & `nsls2-detector-handlers-0.0.3/versioneer.py`

 * *Files 0% similar despite different names*

```diff
@@ -335,17 +335,16 @@
 def get_config_from_root(root):
     """Read the project setup.cfg file to determine Versioneer config."""
     # This might raise EnvironmentError (if setup.cfg is missing), or
     # configparser.NoSectionError (if it lacks a [versioneer] section), or
     # configparser.NoOptionError (if it lacks "VCS="). See the docstring at
     # the top of versioneer.py for instructions on writing your setup.cfg .
     setup_cfg = os.path.join(root, "setup.cfg")
-    parser = configparser.SafeConfigParser()
-    with open(setup_cfg, "r") as f:
-        parser.readfp(f)
+    parser = configparser.ConfigParser()
+    parser.read(setup_cfg)
     VCS = parser.get("versioneer", "VCS")  # mandatory
 
     def get(parser, name):
         if parser.has_option("versioneer", name):
             return parser.get("versioneer", name)
         return None
     cfg = VersioneerConfig()
```

