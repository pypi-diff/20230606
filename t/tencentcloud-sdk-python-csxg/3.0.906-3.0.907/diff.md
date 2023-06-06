# Comparing `tmp/tencentcloud-sdk-python-csxg-3.0.906.tar.gz` & `tmp/tencentcloud-sdk-python-csxg-3.0.907.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-csxg-3.0.906.tar", last modified: Mon Jun  5 00:31:57 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-csxg-3.0.907.tar", last modified: Tue Jun  6 02:23:42 2023, max compression
```

## Comparing `tencentcloud-sdk-python-csxg-3.0.906.tar` & `tencentcloud-sdk-python-csxg-3.0.907.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:31:57.000000 tencentcloud-sdk-python-csxg-3.0.906/
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-05 00:31:57.000000 tencentcloud-sdk-python-csxg-3.0.906/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:31:57.000000 tencentcloud-sdk-python-csxg-3.0.906/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-05 00:31:57.000000 tencentcloud-sdk-python-csxg-3.0.906/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:31:57.000000 tencentcloud-sdk-python-csxg-3.0.906/tencentcloud/csxg/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:31:57.000000 tencentcloud-sdk-python-csxg-3.0.906/tencentcloud/csxg/v20230303/
--rw-r--r--   0 root         (0) root         (0)      769 2023-06-05 00:31:57.000000 tencentcloud-sdk-python-csxg-3.0.906/tencentcloud/csxg/v20230303/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:31:57.000000 tencentcloud-sdk-python-csxg-3.0.906/tencentcloud/csxg/v20230303/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3409 2023-06-05 00:31:57.000000 tencentcloud-sdk-python-csxg-3.0.906/tencentcloud/csxg/v20230303/models.py
--rw-r--r--   0 root         (0) root         (0)     5377 2023-06-05 00:31:57.000000 tencentcloud-sdk-python-csxg-3.0.906/tencentcloud/csxg/v20230303/csxg_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 00:31:57.000000 tencentcloud-sdk-python-csxg-3.0.906/tencentcloud/csxg/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 00:31:57.000000 tencentcloud-sdk-python-csxg-3.0.906/tencentcloud_sdk_python_csxg.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 00:31:57.000000 tencentcloud-sdk-python-csxg-3.0.906/tencentcloud_sdk_python_csxg.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-06-05 00:31:57.000000 tencentcloud-sdk-python-csxg-3.0.906/tencentcloud_sdk_python_csxg.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-05 00:31:57.000000 tencentcloud-sdk-python-csxg-3.0.906/tencentcloud_sdk_python_csxg.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-05 00:31:57.000000 tencentcloud-sdk-python-csxg-3.0.906/tencentcloud_sdk_python_csxg.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-05 00:31:57.000000 tencentcloud-sdk-python-csxg-3.0.906/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-06-05 00:31:57.000000 tencentcloud-sdk-python-csxg-3.0.906/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-05 00:31:57.000000 tencentcloud-sdk-python-csxg-3.0.906/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:23:42.000000 tencentcloud-sdk-python-csxg-3.0.907/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-06 02:23:42.000000 tencentcloud-sdk-python-csxg-3.0.907/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:23:42.000000 tencentcloud-sdk-python-csxg-3.0.907/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-06 02:23:42.000000 tencentcloud-sdk-python-csxg-3.0.907/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:23:42.000000 tencentcloud-sdk-python-csxg-3.0.907/tencentcloud/csxg/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:23:42.000000 tencentcloud-sdk-python-csxg-3.0.907/tencentcloud/csxg/v20230303/
+-rw-r--r--   0 root         (0) root         (0)      769 2023-06-06 02:23:42.000000 tencentcloud-sdk-python-csxg-3.0.907/tencentcloud/csxg/v20230303/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:23:42.000000 tencentcloud-sdk-python-csxg-3.0.907/tencentcloud/csxg/v20230303/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3409 2023-06-06 02:23:42.000000 tencentcloud-sdk-python-csxg-3.0.907/tencentcloud/csxg/v20230303/models.py
+-rw-r--r--   0 root         (0) root         (0)     5377 2023-06-06 02:23:42.000000 tencentcloud-sdk-python-csxg-3.0.907/tencentcloud/csxg/v20230303/csxg_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 02:23:42.000000 tencentcloud-sdk-python-csxg-3.0.907/tencentcloud/csxg/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 02:23:42.000000 tencentcloud-sdk-python-csxg-3.0.907/tencentcloud_sdk_python_csxg.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 02:23:42.000000 tencentcloud-sdk-python-csxg-3.0.907/tencentcloud_sdk_python_csxg.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-06-06 02:23:42.000000 tencentcloud-sdk-python-csxg-3.0.907/tencentcloud_sdk_python_csxg.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-06 02:23:42.000000 tencentcloud-sdk-python-csxg-3.0.907/tencentcloud_sdk_python_csxg.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-06 02:23:42.000000 tencentcloud-sdk-python-csxg-3.0.907/tencentcloud_sdk_python_csxg.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-06 02:23:42.000000 tencentcloud-sdk-python-csxg-3.0.907/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-06-06 02:23:42.000000 tencentcloud-sdk-python-csxg-3.0.907/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-06 02:23:42.000000 tencentcloud-sdk-python-csxg-3.0.907/setup.cfg
```

### Comparing `tencentcloud-sdk-python-csxg-3.0.906/README.rst` & `tencentcloud-sdk-python-csxg-3.0.907/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-csxg-3.0.906/tencentcloud/__init__.py` & `tencentcloud-sdk-python-csxg-3.0.907/tencentcloud/csxg/v20230303/errorcodes.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,21 @@
-# -*- coding: utf-8 -*-
-# Copyright 1999-2018 Tencent Ltd.
+# -*- coding: utf8 -*-
+# Copyright (c) 2017-2021 THL A29 Limited, a Tencent company. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.906'
+# 超过配额限制。
+LIMITEXCEEDED = 'LimitExceeded'
+
+# 资源不存在。
+RESOURCENOTFOUND = 'ResourceNotFound'
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tencentcloud-sdk-python-csxg-3.0.906/tencentcloud/csxg/v20230303/models.py` & `tencentcloud-sdk-python-csxg-3.0.907/tencentcloud/csxg/v20230303/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-csxg-3.0.906/tencentcloud/csxg/v20230303/csxg_client.py` & `tencentcloud-sdk-python-csxg-3.0.907/tencentcloud/csxg/v20230303/csxg_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-csxg-3.0.906/tencentcloud_sdk_python_csxg.egg-info/PKG-INFO` & `tencentcloud-sdk-python-csxg-3.0.907/tencentcloud_sdk_python_csxg.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-csxg
-Version: 3.0.906
+Version: 3.0.907
 Summary: Tencent Cloud Csxg SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-csxg-3.0.906/PKG-INFO` & `tencentcloud-sdk-python-csxg-3.0.907/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-csxg
-Version: 3.0.906
+Version: 3.0.907
 Summary: Tencent Cloud Csxg SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-csxg-3.0.906/setup.py` & `tencentcloud-sdk-python-csxg-3.0.907/setup.py`

 * *Files identical despite different names*

