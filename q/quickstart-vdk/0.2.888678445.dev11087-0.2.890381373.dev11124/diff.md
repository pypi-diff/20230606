# Comparing `tmp/quickstart-vdk-0.2.888678445.dev11087.tar.gz` & `tmp/quickstart-vdk-0.2.890381373.dev11124.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstart-vdk-0.2.888678445.dev11087.tar", last modified: Sun Jun  4 04:23:00 2023, max compression
+gzip compressed data, was "quickstart-vdk-0.2.890381373.dev11124.tar", last modified: Tue Jun  6 04:22:29 2023, max compression
```

## Comparing `quickstart-vdk-0.2.888678445.dev11087.tar` & `quickstart-vdk-0.2.890381373.dev11124.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 04:23:00.842533 quickstart-vdk-0.2.888678445.dev11087/
--rw-r--r--   0 root         (0) root         (0)     1017 2023-06-04 04:23:00.838533 quickstart-vdk-0.2.888678445.dev11087/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      386 2023-06-04 04:20:19.000000 quickstart-vdk-0.2.888678445.dev11087/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 04:23:00.838533 quickstart-vdk-0.2.888678445.dev11087/quickstart_vdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1017 2023-06-04 04:23:00.000000 quickstart-vdk-0.2.888678445.dev11087/quickstart_vdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      227 2023-06-04 04:23:00.000000 quickstart-vdk-0.2.888678445.dev11087/quickstart_vdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-04 04:23:00.000000 quickstart-vdk-0.2.888678445.dev11087/quickstart_vdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      105 2023-06-04 04:23:00.000000 quickstart-vdk-0.2.888678445.dev11087/quickstart_vdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-06-04 04:23:00.000000 quickstart-vdk-0.2.888678445.dev11087/quickstart_vdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-04 04:23:00.842533 quickstart-vdk-0.2.888678445.dev11087/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1300 2023-06-04 04:22:50.000000 quickstart-vdk-0.2.888678445.dev11087/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 04:23:00.838533 quickstart-vdk-0.2.888678445.dev11087/tests/
--rw-rw-rw-   0 root         (0) root         (0)      114 2023-06-04 04:20:19.000000 quickstart-vdk-0.2.888678445.dev11087/tests/test_dummy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 04:22:29.270742 quickstart-vdk-0.2.890381373.dev11124/
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-06-06 04:22:29.270742 quickstart-vdk-0.2.890381373.dev11124/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      386 2023-06-06 04:19:38.000000 quickstart-vdk-0.2.890381373.dev11124/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 04:22:29.266742 quickstart-vdk-0.2.890381373.dev11124/quickstart_vdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-06-06 04:22:29.000000 quickstart-vdk-0.2.890381373.dev11124/quickstart_vdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      227 2023-06-06 04:22:29.000000 quickstart-vdk-0.2.890381373.dev11124/quickstart_vdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 04:22:29.000000 quickstart-vdk-0.2.890381373.dev11124/quickstart_vdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      105 2023-06-06 04:22:29.000000 quickstart-vdk-0.2.890381373.dev11124/quickstart_vdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-06 04:22:29.000000 quickstart-vdk-0.2.890381373.dev11124/quickstart_vdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 04:22:29.270742 quickstart-vdk-0.2.890381373.dev11124/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1300 2023-06-06 04:22:19.000000 quickstart-vdk-0.2.890381373.dev11124/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 04:22:29.270742 quickstart-vdk-0.2.890381373.dev11124/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      114 2023-06-06 04:19:38.000000 quickstart-vdk-0.2.890381373.dev11124/tests/test_dummy.py
```

### Comparing `quickstart-vdk-0.2.888678445.dev11087/PKG-INFO` & `quickstart-vdk-0.2.890381373.dev11124/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.888678445.dev11087
+Version: 0.2.890381373.dev11124
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.888678445.dev11087/quickstart_vdk.egg-info/PKG-INFO` & `quickstart-vdk-0.2.890381373.dev11124/quickstart_vdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstart-vdk
-Version: 0.2.888678445.dev11087
+Version: 0.2.890381373.dev11124
 Summary: Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `quickstart-vdk-0.2.888678445.dev11087/setup.py` & `quickstart-vdk-0.2.890381373.dev11124/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.2.888678445.dev11087"
+__version__ = "0.2.890381373.dev11124"
 
 setuptools.setup(
     name="quickstart-vdk",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK packaging containing common plugins to get started quickly using it.",
     long_description=pathlib.Path("README.md").read_text(),
```

