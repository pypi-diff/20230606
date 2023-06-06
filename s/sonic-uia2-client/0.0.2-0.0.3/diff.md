# Comparing `tmp/sonic-uia2-client-0.0.2.tar.gz` & `tmp/sonic-uia2-client-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sonic-uia2-client-0.0.2.tar", last modified: Sun Jun  4 12:58:43 2023, max compression
+gzip compressed data, was "sonic-uia2-client-0.0.3.tar", last modified: Tue Jun  6 06:11:24 2023, max compression
```

## Comparing `sonic-uia2-client-0.0.2.tar` & `sonic-uia2-client-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:58:43.983838 sonic-uia2-client-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-04 12:58:30.000000 sonic-uia2-client-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-04 12:58:43.979838 sonic-uia2-client-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-04 12:58:30.000000 sonic-uia2-client-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:58:43.979838 sonic-uia2-client-0.0.2/common/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-04 12:58:30.000000 sonic-uia2-client-0.0.2/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-04 12:58:30.000000 sonic-uia2-client-0.0.2/common/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-04 12:58:30.000000 sonic-uia2-client-0.0.2/common/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-04 12:58:30.000000 sonic-uia2-client-0.0.2/common/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-04 12:58:30.000000 sonic-uia2-client-0.0.2/common/resp_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-04 12:58:30.000000 sonic-uia2-client-0.0.2/common/sonic_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 12:58:43.983838 sonic-uia2-client-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-04 12:58:30.000000 sonic-uia2-client-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:58:43.979838 sonic-uia2-client-0.0.2/sonic_uia2_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-04 12:58:43.000000 sonic-uia2-client-0.0.2/sonic_uia2_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-04 12:58:43.000000 sonic-uia2-client-0.0.2/sonic_uia2_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 12:58:43.000000 sonic-uia2-client-0.0.2/sonic_uia2_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-04 12:58:43.000000 sonic-uia2-client-0.0.2/sonic_uia2_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:58:43.979838 sonic-uia2-client-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-04 12:58:30.000000 sonic-uia2-client-0.0.2/tests/test_driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:58:43.979838 sonic-uia2-client-0.0.2/uia2/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-04 12:58:30.000000 sonic-uia2-client-0.0.2/uia2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-04 12:58:30.000000 sonic-uia2-client-0.0.2/uia2/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:11:24.721294 sonic-uia2-client-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-06 06:11:10.000000 sonic-uia2-client-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-06-06 06:11:24.721294 sonic-uia2-client-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-06 06:11:10.000000 sonic-uia2-client-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:11:24.717294 sonic-uia2-client-0.0.3/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-06 06:11:10.000000 sonic-uia2-client-0.0.3/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-06-06 06:11:10.000000 sonic-uia2-client-0.0.3/client/android_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10580 2023-06-06 06:11:10.000000 sonic-uia2-client-0.0.3/client/uia_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:11:24.717294 sonic-uia2-client-0.0.3/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-06 06:11:10.000000 sonic-uia2-client-0.0.3/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-06 06:11:10.000000 sonic-uia2-client-0.0.3/common/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-06 06:11:10.000000 sonic-uia2-client-0.0.3/common/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-06 06:11:10.000000 sonic-uia2-client-0.0.3/common/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-06 06:11:10.000000 sonic-uia2-client-0.0.3/common/resp_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-06 06:11:10.000000 sonic-uia2-client-0.0.3/common/sonic_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 06:11:24.721294 sonic-uia2-client-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-06 06:11:10.000000 sonic-uia2-client-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:11:24.721294 sonic-uia2-client-0.0.3/sonic_uia2_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-06-06 06:11:24.000000 sonic-uia2-client-0.0.3/sonic_uia2_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-06 06:11:24.000000 sonic-uia2-client-0.0.3/sonic_uia2_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 06:11:24.000000 sonic-uia2-client-0.0.3/sonic_uia2_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-06 06:11:24.000000 sonic-uia2-client-0.0.3/sonic_uia2_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:11:24.721294 sonic-uia2-client-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-06 06:11:10.000000 sonic-uia2-client-0.0.3/tests/test_driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:11:24.721294 sonic-uia2-client-0.0.3/uia2/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-06 06:11:10.000000 sonic-uia2-client-0.0.3/uia2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-06 06:11:10.000000 sonic-uia2-client-0.0.3/uia2/driver.py
```

### Comparing `sonic-uia2-client-0.0.2/LICENSE` & `sonic-uia2-client-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sonic-uia2-client-0.0.2/common/http_client.py` & `sonic-uia2-client-0.0.3/common/http_client.py`

 * *Files identical despite different names*

### Comparing `sonic-uia2-client-0.0.2/common/logger.py` & `sonic-uia2-client-0.0.3/common/logger.py`

 * *Files identical despite different names*

### Comparing `sonic-uia2-client-0.0.2/common/models.py` & `sonic-uia2-client-0.0.3/common/models.py`

 * *Files identical despite different names*

### Comparing `sonic-uia2-client-0.0.2/common/resp_handler.py` & `sonic-uia2-client-0.0.3/common/resp_handler.py`

 * *Files identical despite different names*

### Comparing `sonic-uia2-client-0.0.2/setup.py` & `sonic-uia2-client-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # -*- coding:utf-8 -*-
 import os
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 0
-PATCH = 2
+PATCH = 3
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 
 setup(
     name="sonic-uia2-client",
     version=VERSION,
     author="SonicCloudOrg",
     author_email="soniccloudorg@163.com",
```

### Comparing `sonic-uia2-client-0.0.2/tests/test_driver.py` & `sonic-uia2-client-0.0.3/tests/test_driver.py`

 * *Files identical despite different names*

### Comparing `sonic-uia2-client-0.0.2/uia2/driver.py` & `sonic-uia2-client-0.0.3/uia2/driver.py`

 * *Files identical despite different names*

