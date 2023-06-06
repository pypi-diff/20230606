# Comparing `tmp/cijoe-0.9.8.tar.gz` & `tmp/cijoe-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cijoe-0.9.8.tar", last modified: Wed Sep 28 10:12:36 2022, max compression
+gzip compressed data, was "cijoe-0.9.9.tar", last modified: Tue Oct 18 12:12:43 2022, max compression
```

## Comparing `cijoe-0.9.8.tar` & `cijoe-0.9.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 10:12:36.168609 cijoe-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1524 2022-09-28 10:12:25.000000 cijoe-0.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      711 2022-09-28 10:12:36.164609 cijoe-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1128 2022-09-28 10:12:25.000000 cijoe-0.9.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-09-28 10:12:25.000000 cijoe-0.9.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-28 10:12:36.168609 cijoe-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1395 2022-09-28 10:12:25.000000 cijoe-0.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 10:12:36.160609 cijoe-0.9.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 10:12:36.160609 cijoe-0.9.8/src/cijoe/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 10:12:36.160609 cijoe-0.9.8/src/cijoe/cli/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-28 10:12:25.000000 cijoe-0.9.8/src/cijoe/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-28 10:12:25.000000 cijoe-0.9.8/src/cijoe/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13031 2022-09-28 10:12:25.000000 cijoe-0.9.8/src/cijoe/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 10:12:36.164609 cijoe-0.9.8/src/cijoe/core/
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-09-28 10:12:25.000000 cijoe-0.9.8/src/cijoe/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4028 2022-09-28 10:12:25.000000 cijoe-0.9.8/src/cijoe/core/analyser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 10:12:36.164609 cijoe-0.9.8/src/cijoe/core/auxilary/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-28 10:12:25.000000 cijoe-0.9.8/src/cijoe/core/auxilary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5774 2022-09-28 10:12:25.000000 cijoe-0.9.8/src/cijoe/core/command.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 10:12:36.164609 cijoe-0.9.8/src/cijoe/core/configs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-28 10:12:25.000000 cijoe-0.9.8/src/cijoe/core/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      511 2022-09-28 10:12:25.000000 cijoe-0.9.8/src/cijoe/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)      779 2022-09-28 10:12:25.000000 cijoe-0.9.8/src/cijoe/core/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-09-28 10:12:25.000000 cijoe-0.9.8/src/cijoe/core/monitor.py
--rw-r--r--   0 runner    (1001) docker     (121)     5871 2022-09-28 10:12:25.000000 cijoe-0.9.8/src/cijoe/core/processing.py
--rw-r--r--   0 runner    (1001) docker     (121)    13498 2022-09-28 10:12:25.000000 cijoe-0.9.8/src/cijoe/core/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 10:12:36.164609 cijoe-0.9.8/src/cijoe/core/selftest/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-28 10:12:25.000000 cijoe-0.9.8/src/cijoe/core/selftest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-09-28 10:12:25.000000 cijoe-0.9.8/src/cijoe/core/selftest/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2025 2022-09-28 10:12:25.000000 cijoe-0.9.8/src/cijoe/core/selftest/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (121)      209 2022-09-28 10:12:25.000000 cijoe-0.9.8/src/cijoe/core/selftest/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (121)      666 2022-09-28 10:12:25.000000 cijoe-0.9.8/src/cijoe/core/selftest/test_transfer.py
--rw-r--r--   0 runner    (1001) docker     (121)      364 2022-09-28 10:12:25.000000 cijoe-0.9.8/src/cijoe/core/selftest/test_workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 10:12:36.164609 cijoe-0.9.8/src/cijoe/core/templates/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-09-28 10:12:25.000000 cijoe-0.9.8/src/cijoe/core/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5833 2022-09-28 10:12:25.000000 cijoe-0.9.8/src/cijoe/core/transport.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 10:12:36.164609 cijoe-0.9.8/src/cijoe/core/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-09-28 10:12:25.000000 cijoe-0.9.8/src/cijoe/core/workflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 10:12:36.164609 cijoe-0.9.8/src/cijoe/core/worklets/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-28 10:12:25.000000 cijoe-0.9.8/src/cijoe/core/worklets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      565 2022-09-28 10:12:25.000000 cijoe-0.9.8/src/cijoe/core/worklets/cmdrunner.py
--rw-r--r--   0 runner    (1001) docker     (121)      169 2022-09-28 10:12:25.000000 cijoe-0.9.8/src/cijoe/core/worklets/dump_metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-09-28 10:12:25.000000 cijoe-0.9.8/src/cijoe/core/worklets/extract.py
--rw-r--r--   0 runner    (1001) docker     (121)     2085 2022-09-28 10:12:25.000000 cijoe-0.9.8/src/cijoe/core/worklets/reporter.py
--rw-r--r--   0 runner    (1001) docker     (121)     2873 2022-09-28 10:12:25.000000 cijoe-0.9.8/src/cijoe/core/worklets/repository_prep.py
--rw-r--r--   0 runner    (1001) docker     (121)     1366 2022-09-28 10:12:25.000000 cijoe-0.9.8/src/cijoe/core/worklets/testrunner.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 10:12:36.164609 cijoe-0.9.8/src/cijoe/pytest_plugin/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-28 10:12:25.000000 cijoe-0.9.8/src/cijoe/pytest_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3270 2022-09-28 10:12:25.000000 cijoe-0.9.8/src/cijoe/pytest_plugin/hooks_and_fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 10:12:36.160609 cijoe-0.9.8/src/cijoe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      711 2022-09-28 10:12:36.000000 cijoe-0.9.8/src/cijoe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1315 2022-09-28 10:12:36.000000 cijoe-0.9.8/src/cijoe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-28 10:12:36.000000 cijoe-0.9.8/src/cijoe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-09-28 10:12:36.000000 cijoe-0.9.8/src/cijoe.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-28 10:12:36.000000 cijoe-0.9.8/src/cijoe.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-09-28 10:12:36.000000 cijoe-0.9.8/src/cijoe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-09-28 10:12:36.000000 cijoe-0.9.8/src/cijoe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 12:12:43.495383 cijoe-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1524 2022-10-18 12:12:29.000000 cijoe-0.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      711 2022-10-18 12:12:43.495383 cijoe-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1128 2022-10-18 12:12:29.000000 cijoe-0.9.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-10-18 12:12:29.000000 cijoe-0.9.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-18 12:12:43.495383 cijoe-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1395 2022-10-18 12:12:29.000000 cijoe-0.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 12:12:43.491383 cijoe-0.9.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 12:12:43.491383 cijoe-0.9.9/src/cijoe/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 12:12:43.495383 cijoe-0.9.9/src/cijoe/cli/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-18 12:12:29.000000 cijoe-0.9.9/src/cijoe/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-18 12:12:29.000000 cijoe-0.9.9/src/cijoe/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13031 2022-10-18 12:12:29.000000 cijoe-0.9.9/src/cijoe/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 12:12:43.495383 cijoe-0.9.9/src/cijoe/core/
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2022-10-18 12:12:29.000000 cijoe-0.9.9/src/cijoe/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4028 2022-10-18 12:12:29.000000 cijoe-0.9.9/src/cijoe/core/analyser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 12:12:43.495383 cijoe-0.9.9/src/cijoe/core/auxilary/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-18 12:12:29.000000 cijoe-0.9.9/src/cijoe/core/auxilary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5774 2022-10-18 12:12:29.000000 cijoe-0.9.9/src/cijoe/core/command.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 12:12:43.495383 cijoe-0.9.9/src/cijoe/core/configs/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-18 12:12:29.000000 cijoe-0.9.9/src/cijoe/core/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      511 2022-10-18 12:12:29.000000 cijoe-0.9.9/src/cijoe/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)      779 2022-10-18 12:12:29.000000 cijoe-0.9.9/src/cijoe/core/misc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1328 2022-10-18 12:12:29.000000 cijoe-0.9.9/src/cijoe/core/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5871 2022-10-18 12:12:29.000000 cijoe-0.9.9/src/cijoe/core/processing.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13498 2022-10-18 12:12:29.000000 cijoe-0.9.9/src/cijoe/core/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 12:12:43.495383 cijoe-0.9.9/src/cijoe/core/selftest/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-18 12:12:29.000000 cijoe-0.9.9/src/cijoe/core/selftest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      397 2022-10-18 12:12:29.000000 cijoe-0.9.9/src/cijoe/core/selftest/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2025 2022-10-18 12:12:29.000000 cijoe-0.9.9/src/cijoe/core/selftest/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (121)      209 2022-10-18 12:12:29.000000 cijoe-0.9.9/src/cijoe/core/selftest/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (121)      666 2022-10-18 12:12:29.000000 cijoe-0.9.9/src/cijoe/core/selftest/test_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      364 2022-10-18 12:12:29.000000 cijoe-0.9.9/src/cijoe/core/selftest/test_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 12:12:43.495383 cijoe-0.9.9/src/cijoe/core/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-10-18 12:12:29.000000 cijoe-0.9.9/src/cijoe/core/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5869 2022-10-18 12:12:29.000000 cijoe-0.9.9/src/cijoe/core/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 12:12:43.495383 cijoe-0.9.9/src/cijoe/core/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2022-10-18 12:12:29.000000 cijoe-0.9.9/src/cijoe/core/workflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 12:12:43.495383 cijoe-0.9.9/src/cijoe/core/worklets/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-18 12:12:29.000000 cijoe-0.9.9/src/cijoe/core/worklets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      565 2022-10-18 12:12:29.000000 cijoe-0.9.9/src/cijoe/core/worklets/cmdrunner.py
+-rw-r--r--   0 runner    (1001) docker     (121)      169 2022-10-18 12:12:29.000000 cijoe-0.9.9/src/cijoe/core/worklets/dump_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-10-18 12:12:29.000000 cijoe-0.9.9/src/cijoe/core/worklets/extract.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2085 2022-10-18 12:12:29.000000 cijoe-0.9.9/src/cijoe/core/worklets/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2873 2022-10-18 12:12:29.000000 cijoe-0.9.9/src/cijoe/core/worklets/repository_prep.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1366 2022-10-18 12:12:29.000000 cijoe-0.9.9/src/cijoe/core/worklets/testrunner.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 12:12:43.495383 cijoe-0.9.9/src/cijoe/pytest_plugin/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-18 12:12:29.000000 cijoe-0.9.9/src/cijoe/pytest_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3270 2022-10-18 12:12:29.000000 cijoe-0.9.9/src/cijoe/pytest_plugin/hooks_and_fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 12:12:43.491383 cijoe-0.9.9/src/cijoe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      711 2022-10-18 12:12:43.000000 cijoe-0.9.9/src/cijoe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1315 2022-10-18 12:12:43.000000 cijoe-0.9.9/src/cijoe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-18 12:12:43.000000 cijoe-0.9.9/src/cijoe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-10-18 12:12:43.000000 cijoe-0.9.9/src/cijoe.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-18 12:12:43.000000 cijoe-0.9.9/src/cijoe.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       84 2022-10-18 12:12:43.000000 cijoe-0.9.9/src/cijoe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-18 12:12:43.000000 cijoe-0.9.9/src/cijoe.egg-info/top_level.txt
```

### Comparing `cijoe-0.9.8/LICENSE` & `cijoe-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cijoe-0.9.8/PKG-INFO` & `cijoe-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cijoe
-Version: 0.9.8
+Version: 0.9.9
 Summary: UNKNOWN
 Home-page: https://github.com/refenv/cijoe
 Author: Simon A. F. Lund
 Author-email: os@safl.dk
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cijoe-0.9.8/README.rst` & `cijoe-0.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `cijoe-0.9.8/setup.py` & `cijoe-0.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_namespace_packages, setup
 
 setup(
     name="cijoe",
-    version="0.9.8",
+    version="0.9.9",
     author="Simon A. F. Lund",
     author_email="os@safl.dk",
     url="https://github.com/refenv/cijoe",
     license="BSD",
     install_requires=[
         "jinja2",
         "paramiko",
```

### Comparing `cijoe-0.9.8/src/cijoe/cli/cli.py` & `cijoe-0.9.9/src/cijoe/cli/cli.py`

 * *Files identical despite different names*

### Comparing `cijoe-0.9.8/src/cijoe/core/analyser.py` & `cijoe-0.9.9/src/cijoe/core/analyser.py`

 * *Files identical despite different names*

### Comparing `cijoe-0.9.8/src/cijoe/core/command.py` & `cijoe-0.9.9/src/cijoe/core/command.py`

 * *Files identical despite different names*

### Comparing `cijoe-0.9.8/src/cijoe/core/misc.py` & `cijoe-0.9.9/src/cijoe/core/misc.py`

 * *Files identical despite different names*

### Comparing `cijoe-0.9.8/src/cijoe/core/monitor.py` & `cijoe-0.9.9/src/cijoe/core/monitor.py`

 * *Files identical despite different names*

### Comparing `cijoe-0.9.8/src/cijoe/core/processing.py` & `cijoe-0.9.9/src/cijoe/core/processing.py`

 * *Files identical despite different names*

### Comparing `cijoe-0.9.8/src/cijoe/core/resources.py` & `cijoe-0.9.9/src/cijoe/core/resources.py`

 * *Files identical despite different names*

### Comparing `cijoe-0.9.8/src/cijoe/core/selftest/test_collector.py` & `cijoe-0.9.9/src/cijoe/core/selftest/test_collector.py`

 * *Files identical despite different names*

### Comparing `cijoe-0.9.8/src/cijoe/core/selftest/test_transfer.py` & `cijoe-0.9.9/src/cijoe/core/selftest/test_transfer.py`

 * *Files identical despite different names*

### Comparing `cijoe-0.9.8/src/cijoe/core/transport.py` & `cijoe-0.9.9/src/cijoe/core/transport.py`

 * *Files 5% similar despite different names*

```diff
@@ -139,16 +139,16 @@
             cmd = f"cd {cwd}; {cmd}"
 
         try:
             self.__connect()
 
             _, stdout, stderr = self.ssh.exec_command(cmd, environment=env)
 
-            logfile.write(stdout.read().decode(ENCODING))
-            logfile.write(stderr.read().decode(ENCODING))
+            logfile.write(stdout.read().decode(ENCODING, errors='replace'))
+            logfile.write(stderr.read().decode(ENCODING, errors='replace'))
 
             err = stdout.channel.recv_exit_status()
 
             self.__disconnect()
         except paramiko.ssh_exception.SSHException as exc:
             err = (
                 exc.errno
```

### Comparing `cijoe-0.9.8/src/cijoe/core/worklets/cmdrunner.py` & `cijoe-0.9.9/src/cijoe/core/worklets/cmdrunner.py`

 * *Files identical despite different names*

### Comparing `cijoe-0.9.8/src/cijoe/core/worklets/reporter.py` & `cijoe-0.9.9/src/cijoe/core/worklets/reporter.py`

 * *Files identical despite different names*

### Comparing `cijoe-0.9.8/src/cijoe/core/worklets/repository_prep.py` & `cijoe-0.9.9/src/cijoe/core/worklets/repository_prep.py`

 * *Files identical despite different names*

### Comparing `cijoe-0.9.8/src/cijoe/core/worklets/testrunner.py` & `cijoe-0.9.9/src/cijoe/core/worklets/testrunner.py`

 * *Files identical despite different names*

### Comparing `cijoe-0.9.8/src/cijoe/pytest_plugin/hooks_and_fixtures.py` & `cijoe-0.9.9/src/cijoe/pytest_plugin/hooks_and_fixtures.py`

 * *Files identical despite different names*

### Comparing `cijoe-0.9.8/src/cijoe.egg-info/PKG-INFO` & `cijoe-0.9.9/src/cijoe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cijoe
-Version: 0.9.8
+Version: 0.9.9
 Summary: UNKNOWN
 Home-page: https://github.com/refenv/cijoe
 Author: Simon A. F. Lund
 Author-email: os@safl.dk
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `cijoe-0.9.8/src/cijoe.egg-info/SOURCES.txt` & `cijoe-0.9.9/src/cijoe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

