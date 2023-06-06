# Comparing `tmp/mypy-boto3-signer-1.26.0.post1.tar.gz` & `tmp/mypy-boto3-signer-1.26.148.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-signer-1.26.0.post1.tar", last modified: Tue Nov  1 21:44:01 2022, max compression
+gzip compressed data, was "mypy-boto3-signer-1.26.148.tar", last modified: Tue Jun  6 19:35:54 2023, max compression
```

## Comparing `mypy-boto3-signer-1.26.0.post1.tar` & `mypy-boto3-signer-1.26.148.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:44:01.068850 mypy-boto3-signer-1.26.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-11-01 21:41:28.000000 mypy-boto3-signer-1.26.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    15811 2022-11-01 21:44:01.060850 mypy-boto3-signer-1.26.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    14374 2022-11-01 21:41:28.000000 mypy-boto3-signer-1.26.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:44:01.048850 mypy-boto3-signer-1.26.0.post1/mypy_boto3_signer/
--rw-r--r--   0 runner    (1001) docker     (121)     1278 2022-11-01 21:41:28.000000 mypy-boto3-signer-1.26.0.post1/mypy_boto3_signer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1277 2022-11-01 21:41:28.000000 mypy-boto3-signer-1.26.0.post1/mypy_boto3_signer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      913 2022-11-01 21:41:29.000000 mypy-boto3-signer-1.26.0.post1/mypy_boto3_signer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15845 2022-11-01 21:41:29.000000 mypy-boto3-signer-1.26.0.post1/mypy_boto3_signer/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    15817 2022-11-01 21:41:29.000000 mypy-boto3-signer-1.26.0.post1/mypy_boto3_signer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7955 2022-11-01 21:41:29.000000 mypy-boto3-signer-1.26.0.post1/mypy_boto3_signer/literals.py
--rw-r--r--   0 runner    (1001) docker     (121)     7953 2022-11-01 21:41:29.000000 mypy-boto3-signer-1.26.0.post1/mypy_boto3_signer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4642 2022-11-01 21:41:29.000000 mypy-boto3-signer-1.26.0.post1/mypy_boto3_signer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (121)     4637 2022-11-01 21:41:29.000000 mypy-boto3-signer-1.26.0.post1/mypy_boto3_signer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-01 21:41:29.000000 mypy-boto3-signer-1.26.0.post1/mypy_boto3_signer/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    20008 2022-11-01 21:41:29.000000 mypy-boto3-signer-1.26.0.post1/mypy_boto3_signer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (121)    19993 2022-11-01 21:41:29.000000 mypy-boto3-signer-1.26.0.post1/mypy_boto3_signer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-01 21:41:28.000000 mypy-boto3-signer-1.26.0.post1/mypy_boto3_signer/version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1431 2022-11-01 21:41:29.000000 mypy-boto3-signer-1.26.0.post1/mypy_boto3_signer/waiter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1430 2022-11-01 21:41:29.000000 mypy-boto3-signer-1.26.0.post1/mypy_boto3_signer/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-01 21:44:01.060850 mypy-boto3-signer-1.26.0.post1/mypy_boto3_signer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    15811 2022-11-01 21:44:00.000000 mypy-boto3-signer-1.26.0.post1/mypy_boto3_signer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      718 2022-11-01 21:44:00.000000 mypy-boto3-signer-1.26.0.post1/mypy_boto3_signer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:44:00.000000 mypy-boto3-signer-1.26.0.post1/mypy_boto3_signer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-01 21:44:00.000000 mypy-boto3-signer-1.26.0.post1/mypy_boto3_signer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-01 21:44:00.000000 mypy-boto3-signer-1.26.0.post1/mypy_boto3_signer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-01 21:44:00.000000 mypy-boto3-signer-1.26.0.post1/mypy_boto3_signer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-01 21:44:01.068850 mypy-boto3-signer-1.26.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1950 2022-11-01 21:41:28.000000 mypy-boto3-signer-1.26.0.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:35:54.134339 mypy-boto3-signer-1.26.148/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-06 19:35:31.000000 mypy-boto3-signer-1.26.148/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16010 2023-06-06 19:35:54.134339 mypy-boto3-signer-1.26.148/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14525 2023-06-06 19:35:31.000000 mypy-boto3-signer-1.26.148/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:35:54.134339 mypy-boto3-signer-1.26.148/mypy_boto3_signer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-06 19:35:31.000000 mypy-boto3-signer-1.26.148/mypy_boto3_signer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-06 19:35:31.000000 mypy-boto3-signer-1.26.148/mypy_boto3_signer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-06 19:35:31.000000 mypy-boto3-signer-1.26.148/mypy_boto3_signer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17273 2023-06-06 19:35:32.000000 mypy-boto3-signer-1.26.148/mypy_boto3_signer/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17243 2023-06-06 19:35:31.000000 mypy-boto3-signer-1.26.148/mypy_boto3_signer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8945 2023-06-06 19:35:32.000000 mypy-boto3-signer-1.26.148/mypy_boto3_signer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-06-06 19:35:32.000000 mypy-boto3-signer-1.26.148/mypy_boto3_signer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-06 19:35:32.000000 mypy-boto3-signer-1.26.148/mypy_boto3_signer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-06-06 19:35:32.000000 mypy-boto3-signer-1.26.148/mypy_boto3_signer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 19:35:31.000000 mypy-boto3-signer-1.26.148/mypy_boto3_signer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21560 2023-06-06 19:35:32.000000 mypy-boto3-signer-1.26.148/mypy_boto3_signer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21543 2023-06-06 19:35:32.000000 mypy-boto3-signer-1.26.148/mypy_boto3_signer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-06 19:35:31.000000 mypy-boto3-signer-1.26.148/mypy_boto3_signer/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-06 19:35:32.000000 mypy-boto3-signer-1.26.148/mypy_boto3_signer/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-06-06 19:35:32.000000 mypy-boto3-signer-1.26.148/mypy_boto3_signer/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:35:54.134339 mypy-boto3-signer-1.26.148/mypy_boto3_signer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16010 2023-06-06 19:35:54.000000 mypy-boto3-signer-1.26.148/mypy_boto3_signer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-06 19:35:54.000000 mypy-boto3-signer-1.26.148/mypy_boto3_signer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 19:35:54.000000 mypy-boto3-signer-1.26.148/mypy_boto3_signer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 19:35:54.000000 mypy-boto3-signer-1.26.148/mypy_boto3_signer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-06 19:35:54.000000 mypy-boto3-signer-1.26.148/mypy_boto3_signer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-06 19:35:54.000000 mypy-boto3-signer-1.26.148/mypy_boto3_signer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 19:35:54.134339 mypy-boto3-signer-1.26.148/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-06 19:35:31.000000 mypy-boto3-signer-1.26.148/setup.py
```

### Comparing `mypy-boto3-signer-1.26.0.post1/LICENSE` & `mypy-boto3-signer-1.26.148/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Vlad Emelianov
+Copyright (c) 2023 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-signer-1.26.0.post1/PKG-INFO` & `mypy-boto3-signer-1.26.148/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-signer
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.signer 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.148
+Summary: Type annotations for boto3.signer 1.26.148 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,43 +18,44 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-signer"></a>
 
 # mypy-boto3-signer
 
 [![PyPI - mypy-boto3-signer](https://img.shields.io/pypi/v/mypy-boto3-signer.svg?color=blue)](https://pypi.org/project/mypy-boto3-signer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-signer.svg?color=blue)](https://pypi.org/project/mypy-boto3-signer)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-signer?color=blue)](https://pypistats.org/packages/mypy-boto3-signer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.signer 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
+[boto3.signer 1.26.148](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-signer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -343,14 +344,15 @@
     SuccessfulSigningJobWaiterName,
     ValidityTypeType,
     signerServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     WaiterName,
+    RegionName,
 )
 
 
 def check_value(value: CategoryType) -> bool:
     ...
 ```
 
@@ -360,57 +362,61 @@
 
 `mypy_boto3_signer.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_signer.type_defs import (
     AddProfilePermissionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AddProfilePermissionResponseTypeDef,
     CancelSigningProfileRequestRequestTypeDef,
     DescribeSigningJobRequestRequestTypeDef,
     WaiterConfigTypeDef,
     SigningJobRevocationRecordTypeDef,
     SigningMaterialTypeDef,
     S3DestinationTypeDef,
+    EmptyResponseMetadataTypeDef,
     EncryptionAlgorithmOptionsTypeDef,
+    GetRevocationStatusRequestRequestTypeDef,
+    GetRevocationStatusResponseTypeDef,
     GetSigningPlatformRequestRequestTypeDef,
     SigningImageFormatTypeDef,
     GetSigningProfileRequestRequestTypeDef,
     SignatureValidityPeriodTypeDef,
     SigningProfileRevocationRecordTypeDef,
     HashAlgorithmOptionsTypeDef,
     ListProfilePermissionsRequestRequestTypeDef,
     PermissionTypeDef,
-    PaginatorConfigTypeDef,
+    ListSigningJobsRequestListSigningJobsPaginateTypeDef,
     ListSigningJobsRequestRequestTypeDef,
+    ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef,
     ListSigningPlatformsRequestRequestTypeDef,
+    ListSigningProfilesRequestListSigningProfilesPaginateTypeDef,
     ListSigningProfilesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
+    PutSigningProfileResponseTypeDef,
     RemoveProfilePermissionRequestRequestTypeDef,
+    RemoveProfilePermissionResponseTypeDef,
+    ResponseMetadataTypeDef,
     RevokeSignatureRequestRequestTypeDef,
     RevokeSigningProfileRequestRequestTypeDef,
     S3SignedObjectTypeDef,
     S3SourceTypeDef,
+    SignPayloadRequestRequestTypeDef,
+    SignPayloadResponseTypeDef,
     SigningConfigurationOverridesTypeDef,
+    StartSigningJobResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    AddProfilePermissionResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PutSigningProfileResponseTypeDef,
-    RemoveProfilePermissionResponseTypeDef,
-    StartSigningJobResponseTypeDef,
     DescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef,
     DestinationTypeDef,
     SigningProfileTypeDef,
     SigningConfigurationTypeDef,
     ListProfilePermissionsResponseTypeDef,
-    ListSigningJobsRequestListSigningJobsPaginateTypeDef,
-    ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef,
-    ListSigningProfilesRequestListSigningProfilesPaginateTypeDef,
     SignedObjectTypeDef,
     SourceTypeDef,
     SigningPlatformOverridesTypeDef,
     ListSigningProfilesResponseTypeDef,
     GetSigningPlatformResponseTypeDef,
     SigningPlatformTypeDef,
     SigningJobTypeDef,
@@ -430,42 +436,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-signer-1.26.0.post1/README.md` & `mypy-boto3-signer-1.26.148/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-signer"></a>
 
 # mypy-boto3-signer
 
 [![PyPI - mypy-boto3-signer](https://img.shields.io/pypi/v/mypy-boto3-signer.svg?color=blue)](https://pypi.org/project/mypy-boto3-signer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-signer.svg?color=blue)](https://pypi.org/project/mypy-boto3-signer)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-signer?color=blue)](https://pypistats.org/packages/mypy-boto3-signer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.signer 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
+[boto3.signer 1.26.148](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-signer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -312,14 +312,15 @@
     SuccessfulSigningJobWaiterName,
     ValidityTypeType,
     signerServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     WaiterName,
+    RegionName,
 )
 
 
 def check_value(value: CategoryType) -> bool:
     ...
 ```
 
@@ -329,57 +330,61 @@
 
 `mypy_boto3_signer.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_signer.type_defs import (
     AddProfilePermissionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AddProfilePermissionResponseTypeDef,
     CancelSigningProfileRequestRequestTypeDef,
     DescribeSigningJobRequestRequestTypeDef,
     WaiterConfigTypeDef,
     SigningJobRevocationRecordTypeDef,
     SigningMaterialTypeDef,
     S3DestinationTypeDef,
+    EmptyResponseMetadataTypeDef,
     EncryptionAlgorithmOptionsTypeDef,
+    GetRevocationStatusRequestRequestTypeDef,
+    GetRevocationStatusResponseTypeDef,
     GetSigningPlatformRequestRequestTypeDef,
     SigningImageFormatTypeDef,
     GetSigningProfileRequestRequestTypeDef,
     SignatureValidityPeriodTypeDef,
     SigningProfileRevocationRecordTypeDef,
     HashAlgorithmOptionsTypeDef,
     ListProfilePermissionsRequestRequestTypeDef,
     PermissionTypeDef,
-    PaginatorConfigTypeDef,
+    ListSigningJobsRequestListSigningJobsPaginateTypeDef,
     ListSigningJobsRequestRequestTypeDef,
+    ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef,
     ListSigningPlatformsRequestRequestTypeDef,
+    ListSigningProfilesRequestListSigningProfilesPaginateTypeDef,
     ListSigningProfilesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
+    PutSigningProfileResponseTypeDef,
     RemoveProfilePermissionRequestRequestTypeDef,
+    RemoveProfilePermissionResponseTypeDef,
+    ResponseMetadataTypeDef,
     RevokeSignatureRequestRequestTypeDef,
     RevokeSigningProfileRequestRequestTypeDef,
     S3SignedObjectTypeDef,
     S3SourceTypeDef,
+    SignPayloadRequestRequestTypeDef,
+    SignPayloadResponseTypeDef,
     SigningConfigurationOverridesTypeDef,
+    StartSigningJobResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    AddProfilePermissionResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PutSigningProfileResponseTypeDef,
-    RemoveProfilePermissionResponseTypeDef,
-    StartSigningJobResponseTypeDef,
     DescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef,
     DestinationTypeDef,
     SigningProfileTypeDef,
     SigningConfigurationTypeDef,
     ListProfilePermissionsResponseTypeDef,
-    ListSigningJobsRequestListSigningJobsPaginateTypeDef,
-    ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef,
-    ListSigningProfilesRequestListSigningProfilesPaginateTypeDef,
     SignedObjectTypeDef,
     SourceTypeDef,
     SigningPlatformOverridesTypeDef,
     ListSigningProfilesResponseTypeDef,
     GetSigningPlatformResponseTypeDef,
     SigningPlatformTypeDef,
     SigningJobTypeDef,
@@ -399,42 +404,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-signer-1.26.0.post1/mypy_boto3_signer/__init__.py` & `mypy-boto3-signer-1.26.148/mypy_boto3_signer/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-signer-1.26.0.post1/mypy_boto3_signer/__init__.pyi` & `mypy-boto3-signer-1.26.148/mypy_boto3_signer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-signer-1.26.0.post1/mypy_boto3_signer/__main__.py` & `mypy-boto3-signer-1.26.148/mypy_boto3_signer/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.signer 1.26.0\nVersion:         1.26.0.post1\nBuilder version:"
-        " 7.11.10\nDocs:           "
+        "Type annotations for boto3.signer 1.26.148\nVersion:         1.26.148\nBuilder version:"
+        " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.0.post1")
+    print("1.26.148")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-signer-1.26.0.post1/mypy_boto3_signer/client.py` & `mypy-boto3-signer-1.26.148/mypy_boto3_signer/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,41 +11,44 @@
 
     session = Session()
     client: signerClient = session.client("signer")
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
+from botocore.response import StreamingBody
 
 from .literals import SigningProfileStatusType, SigningStatusType
 from .paginator import (
     ListSigningJobsPaginator,
     ListSigningPlatformsPaginator,
     ListSigningProfilesPaginator,
 )
 from .type_defs import (
     AddProfilePermissionResponseTypeDef,
     DescribeSigningJobResponseTypeDef,
     DestinationTypeDef,
     EmptyResponseMetadataTypeDef,
+    GetRevocationStatusResponseTypeDef,
     GetSigningPlatformResponseTypeDef,
     GetSigningProfileResponseTypeDef,
     ListProfilePermissionsResponseTypeDef,
     ListSigningJobsResponseTypeDef,
     ListSigningPlatformsResponseTypeDef,
     ListSigningProfilesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutSigningProfileResponseTypeDef,
     RemoveProfilePermissionResponseTypeDef,
     SignatureValidityPeriodTypeDef,
     SigningMaterialTypeDef,
     SigningPlatformOverridesTypeDef,
+    SignPayloadResponseTypeDef,
     SourceTypeDef,
     StartSigningJobResponseTypeDef,
 )
 from .waiter import SuccessfulSigningJobWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -154,14 +157,31 @@
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#generate_presigned_url)
         """
 
+    def get_revocation_status(
+        self,
+        *,
+        signatureTimestamp: Union[datetime, str],
+        platformId: str,
+        profileVersionArn: str,
+        jobArn: str,
+        certificateHashes: Sequence[str]
+    ) -> GetRevocationStatusResponseTypeDef:
+        """
+        Retrieves the revocation status of one or more of the signing profile, signing
+        job, and signing certificate.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_revocation_status)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#get_revocation_status)
+        """
+
     def get_signing_platform(self, *, platformId: str) -> GetSigningPlatformResponseTypeDef:
         """
         Returns information on a specific signing platform.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_signing_platform)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#get_signing_platform)
         """
@@ -296,14 +316,29 @@
         """
         Changes the state of a signing profile to REVOKED.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.revoke_signing_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#revoke_signing_profile)
         """
 
+    def sign_payload(
+        self,
+        *,
+        profileName: str,
+        payload: Union[str, bytes, IO[Any], StreamingBody],
+        payloadFormat: str,
+        profileOwner: str = ...
+    ) -> SignPayloadResponseTypeDef:
+        """
+        Signs a binary payload and returns a signature envelope.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.sign_payload)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#sign_payload)
+        """
+
     def start_signing_job(
         self,
         *,
         source: SourceTypeDef,
         destination: DestinationTypeDef,
         profileName: str,
         clientRequestToken: str,
```

### Comparing `mypy-boto3-signer-1.26.0.post1/mypy_boto3_signer/client.pyi` & `mypy-boto3-signer-1.26.148/mypy_boto3_signer/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -11,41 +11,44 @@
 
     session = Session()
     client: signerClient = session.client("signer")
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
+from botocore.response import StreamingBody
 
 from .literals import SigningProfileStatusType, SigningStatusType
 from .paginator import (
     ListSigningJobsPaginator,
     ListSigningPlatformsPaginator,
     ListSigningProfilesPaginator,
 )
 from .type_defs import (
     AddProfilePermissionResponseTypeDef,
     DescribeSigningJobResponseTypeDef,
     DestinationTypeDef,
     EmptyResponseMetadataTypeDef,
+    GetRevocationStatusResponseTypeDef,
     GetSigningPlatformResponseTypeDef,
     GetSigningProfileResponseTypeDef,
     ListProfilePermissionsResponseTypeDef,
     ListSigningJobsResponseTypeDef,
     ListSigningPlatformsResponseTypeDef,
     ListSigningProfilesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutSigningProfileResponseTypeDef,
     RemoveProfilePermissionResponseTypeDef,
     SignatureValidityPeriodTypeDef,
     SigningMaterialTypeDef,
     SigningPlatformOverridesTypeDef,
+    SignPayloadResponseTypeDef,
     SourceTypeDef,
     StartSigningJobResponseTypeDef,
 )
 from .waiter import SuccessfulSigningJobWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -143,14 +146,30 @@
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#generate_presigned_url)
         """
+    def get_revocation_status(
+        self,
+        *,
+        signatureTimestamp: Union[datetime, str],
+        platformId: str,
+        profileVersionArn: str,
+        jobArn: str,
+        certificateHashes: Sequence[str]
+    ) -> GetRevocationStatusResponseTypeDef:
+        """
+        Retrieves the revocation status of one or more of the signing profile, signing
+        job, and signing certificate.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_revocation_status)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#get_revocation_status)
+        """
     def get_signing_platform(self, *, platformId: str) -> GetSigningPlatformResponseTypeDef:
         """
         Returns information on a specific signing platform.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.get_signing_platform)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#get_signing_platform)
         """
@@ -274,14 +293,28 @@
     ) -> EmptyResponseMetadataTypeDef:
         """
         Changes the state of a signing profile to REVOKED.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.revoke_signing_profile)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#revoke_signing_profile)
         """
+    def sign_payload(
+        self,
+        *,
+        profileName: str,
+        payload: Union[str, bytes, IO[Any], StreamingBody],
+        payloadFormat: str,
+        profileOwner: str = ...
+    ) -> SignPayloadResponseTypeDef:
+        """
+        Signs a binary payload and returns a signature envelope.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Client.sign_payload)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/client/#sign_payload)
+        """
     def start_signing_job(
         self,
         *,
         source: SourceTypeDef,
         destination: DestinationTypeDef,
         profileName: str,
         clientRequestToken: str,
```

### Comparing `mypy-boto3-signer-1.26.0.post1/mypy_boto3_signer/literals.py` & `mypy-boto3-signer-1.26.148/mypy_boto3_signer/literals.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     "SuccessfulSigningJobWaiterName",
     "ValidityTypeType",
     "signerServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
+    "RegionName",
 )
 
 
 CategoryType = Literal["AWSIoT"]
 EncryptionAlgorithmType = Literal["ECDSA", "RSA"]
 HashAlgorithmType = Literal["SHA1", "SHA256"]
 ImageFormatType = Literal["JSON", "JSONDetached", "JSONEmbedded"]
@@ -71,14 +72,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -88,27 +90,31 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -137,14 +143,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -189,51 +196,57 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -246,14 +259,15 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
+    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -265,28 +279,33 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
+    "osis",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -295,14 +314,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -313,55 +333,63 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
+    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
+    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
@@ -381,7 +409,29 @@
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal["list_signing_jobs", "list_signing_platforms", "list_signing_profiles"]
 WaiterName = Literal["successful_signing_job"]
+RegionName = Literal[
+    "af-south-1",
+    "ap-east-1",
+    "ap-northeast-1",
+    "ap-northeast-2",
+    "ap-south-1",
+    "ap-southeast-1",
+    "ap-southeast-2",
+    "ca-central-1",
+    "eu-central-1",
+    "eu-north-1",
+    "eu-south-1",
+    "eu-west-1",
+    "eu-west-2",
+    "eu-west-3",
+    "me-south-1",
+    "sa-east-1",
+    "us-east-1",
+    "us-east-2",
+    "us-west-1",
+    "us-west-2",
+]
```

### Comparing `mypy-boto3-signer-1.26.0.post1/mypy_boto3_signer/literals.pyi` & `mypy-boto3-signer-1.26.148/mypy_boto3_signer/literals.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     "SuccessfulSigningJobWaiterName",
     "ValidityTypeType",
     "signerServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
+    "RegionName",
 )
 
 CategoryType = Literal["AWSIoT"]
 EncryptionAlgorithmType = Literal["ECDSA", "RSA"]
 HashAlgorithmType = Literal["SHA1", "SHA256"]
 ImageFormatType = Literal["JSON", "JSONDetached", "JSONEmbedded"]
 ListSigningJobsPaginatorName = Literal["list_signing_jobs"]
@@ -69,14 +70,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -86,27 +88,31 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -135,14 +141,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -187,51 +194,57 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -244,14 +257,15 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
+    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -263,28 +277,33 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
+    "osis",
     "outposts",
     "panorama",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -293,14 +312,15 @@
     "rds",
     "rds-data",
     "redshift",
     "redshift-data",
     "redshift-serverless",
     "rekognition",
     "resiliencehub",
+    "resource-explorer-2",
     "resource-groups",
     "resourcegroupstaggingapi",
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
@@ -311,55 +331,63 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
+    "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
+    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
@@ -379,7 +407,29 @@
     "opsworks",
     "s3",
     "sns",
     "sqs",
 ]
 PaginatorName = Literal["list_signing_jobs", "list_signing_platforms", "list_signing_profiles"]
 WaiterName = Literal["successful_signing_job"]
+RegionName = Literal[
+    "af-south-1",
+    "ap-east-1",
+    "ap-northeast-1",
+    "ap-northeast-2",
+    "ap-south-1",
+    "ap-southeast-1",
+    "ap-southeast-2",
+    "ca-central-1",
+    "eu-central-1",
+    "eu-north-1",
+    "eu-south-1",
+    "eu-west-1",
+    "eu-west-2",
+    "eu-west-3",
+    "me-south-1",
+    "sa-east-1",
+    "us-east-1",
+    "us-east-2",
+    "us-west-1",
+    "us-west-2",
+]
```

### Comparing `mypy-boto3-signer-1.26.0.post1/mypy_boto3_signer/paginator.py` & `mypy-boto3-signer-1.26.148/mypy_boto3_signer/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         status: SigningStatusType = ...,
         platformId: str = ...,
         requestedBy: str = ...,
         isRevoked: bool = ...,
         signatureExpiresBefore: Union[datetime, str] = ...,
         signatureExpiresAfter: Union[datetime, str] = ...,
         jobInvoker: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSigningJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/paginators/#listsigningjobspaginator)
         """
 
 
@@ -85,15 +85,15 @@
 
     def paginate(
         self,
         *,
         category: str = ...,
         partner: str = ...,
         target: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSigningPlatformsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningPlatforms.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/paginators/#listsigningplatformspaginator)
         """
 
 
@@ -105,13 +105,13 @@
 
     def paginate(
         self,
         *,
         includeCanceled: bool = ...,
         platformId: str = ...,
         statuses: Sequence[SigningProfileStatusType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSigningProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/paginators/#listsigningprofilespaginator)
         """
```

### Comparing `mypy-boto3-signer-1.26.0.post1/mypy_boto3_signer/paginator.pyi` & `mypy-boto3-signer-1.26.148/mypy_boto3_signer/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         status: SigningStatusType = ...,
         platformId: str = ...,
         requestedBy: str = ...,
         isRevoked: bool = ...,
         signatureExpiresBefore: Union[datetime, str] = ...,
         signatureExpiresAfter: Union[datetime, str] = ...,
         jobInvoker: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSigningJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/paginators/#listsigningjobspaginator)
         """
 
 class ListSigningPlatformsPaginator(Paginator):
@@ -81,15 +81,15 @@
 
     def paginate(
         self,
         *,
         category: str = ...,
         partner: str = ...,
         target: str = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSigningPlatformsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningPlatforms.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/paginators/#listsigningplatformspaginator)
         """
 
 class ListSigningProfilesPaginator(Paginator):
@@ -100,13 +100,13 @@
 
     def paginate(
         self,
         *,
         includeCanceled: bool = ...,
         platformId: str = ...,
         statuses: Sequence[SigningProfileStatusType] = ...,
-        PaginationConfig: PaginatorConfigTypeDef = ...
+        PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListSigningProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer.Paginator.ListSigningProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/paginators/#listsigningprofilespaginator)
         """
```

### Comparing `mypy-boto3-signer-1.26.0.post1/mypy_boto3_signer/type_defs.py` & `mypy-boto3-signer-1.26.148/mypy_boto3_signer/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,17 @@
     from mypy_boto3_signer.type_defs import AddProfilePermissionRequestRequestTypeDef
 
     data: AddProfilePermissionRequestRequestTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import IO, Any, Dict, List, Mapping, Sequence, Union
+
+from botocore.response import StreamingBody
 
 from .literals import (
     EncryptionAlgorithmType,
     HashAlgorithmType,
     ImageFormatType,
     SigningProfileStatusType,
     SigningStatusType,
@@ -32,57 +34,61 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AddProfilePermissionRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AddProfilePermissionResponseTypeDef",
     "CancelSigningProfileRequestRequestTypeDef",
     "DescribeSigningJobRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "SigningJobRevocationRecordTypeDef",
     "SigningMaterialTypeDef",
     "S3DestinationTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EncryptionAlgorithmOptionsTypeDef",
+    "GetRevocationStatusRequestRequestTypeDef",
+    "GetRevocationStatusResponseTypeDef",
     "GetSigningPlatformRequestRequestTypeDef",
     "SigningImageFormatTypeDef",
     "GetSigningProfileRequestRequestTypeDef",
     "SignatureValidityPeriodTypeDef",
     "SigningProfileRevocationRecordTypeDef",
     "HashAlgorithmOptionsTypeDef",
     "ListProfilePermissionsRequestRequestTypeDef",
     "PermissionTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListSigningJobsRequestListSigningJobsPaginateTypeDef",
     "ListSigningJobsRequestRequestTypeDef",
+    "ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef",
     "ListSigningPlatformsRequestRequestTypeDef",
+    "ListSigningProfilesRequestListSigningProfilesPaginateTypeDef",
     "ListSigningProfilesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
+    "PutSigningProfileResponseTypeDef",
     "RemoveProfilePermissionRequestRequestTypeDef",
+    "RemoveProfilePermissionResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "RevokeSignatureRequestRequestTypeDef",
     "RevokeSigningProfileRequestRequestTypeDef",
     "S3SignedObjectTypeDef",
     "S3SourceTypeDef",
+    "SignPayloadRequestRequestTypeDef",
+    "SignPayloadResponseTypeDef",
     "SigningConfigurationOverridesTypeDef",
+    "StartSigningJobResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "AddProfilePermissionResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PutSigningProfileResponseTypeDef",
-    "RemoveProfilePermissionResponseTypeDef",
-    "StartSigningJobResponseTypeDef",
     "DescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef",
     "DestinationTypeDef",
     "SigningProfileTypeDef",
     "SigningConfigurationTypeDef",
     "ListProfilePermissionsResponseTypeDef",
-    "ListSigningJobsRequestListSigningJobsPaginateTypeDef",
-    "ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef",
-    "ListSigningProfilesRequestListSigningProfilesPaginateTypeDef",
     "SignedObjectTypeDef",
     "SourceTypeDef",
     "SigningPlatformOverridesTypeDef",
     "ListSigningProfilesResponseTypeDef",
     "GetSigningPlatformResponseTypeDef",
     "SigningPlatformTypeDef",
     "SigningJobTypeDef",
@@ -116,22 +122,19 @@
 class AddProfilePermissionRequestRequestTypeDef(
     _RequiredAddProfilePermissionRequestRequestTypeDef,
     _OptionalAddProfilePermissionRequestRequestTypeDef,
 ):
     pass
 
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AddProfilePermissionResponseTypeDef = TypedDict(
+    "AddProfilePermissionResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "revisionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CancelSigningProfileRequestRequestTypeDef = TypedDict(
     "CancelSigningProfileRequestRequestTypeDef",
     {
         "profileName": str,
@@ -176,22 +179,48 @@
     {
         "bucketName": str,
         "prefix": str,
     },
     total=False,
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EncryptionAlgorithmOptionsTypeDef = TypedDict(
     "EncryptionAlgorithmOptionsTypeDef",
     {
         "allowedValues": List[EncryptionAlgorithmType],
         "defaultValue": EncryptionAlgorithmType,
     },
 )
 
+GetRevocationStatusRequestRequestTypeDef = TypedDict(
+    "GetRevocationStatusRequestRequestTypeDef",
+    {
+        "signatureTimestamp": Union[datetime, str],
+        "platformId": str,
+        "profileVersionArn": str,
+        "jobArn": str,
+        "certificateHashes": Sequence[str],
+    },
+)
+
+GetRevocationStatusResponseTypeDef = TypedDict(
+    "GetRevocationStatusResponseTypeDef",
+    {
+        "revokedEntities": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetSigningPlatformRequestRequestTypeDef = TypedDict(
     "GetSigningPlatformRequestRequestTypeDef",
     {
         "platformId": str,
     },
 )
 
@@ -280,20 +309,25 @@
         "principal": str,
         "statementId": str,
         "profileVersion": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListSigningJobsRequestListSigningJobsPaginateTypeDef = TypedDict(
+    "ListSigningJobsRequestListSigningJobsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "status": SigningStatusType,
+        "platformId": str,
+        "requestedBy": str,
+        "isRevoked": bool,
+        "signatureExpiresBefore": Union[datetime, str],
+        "signatureExpiresAfter": Union[datetime, str],
+        "jobInvoker": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListSigningJobsRequestRequestTypeDef = TypedDict(
     "ListSigningJobsRequestRequestTypeDef",
     {
@@ -306,26 +340,48 @@
         "signatureExpiresBefore": Union[datetime, str],
         "signatureExpiresAfter": Union[datetime, str],
         "jobInvoker": str,
     },
     total=False,
 )
 
+ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef = TypedDict(
+    "ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef",
+    {
+        "category": str,
+        "partner": str,
+        "target": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSigningPlatformsRequestRequestTypeDef = TypedDict(
     "ListSigningPlatformsRequestRequestTypeDef",
     {
         "category": str,
         "partner": str,
         "target": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+ListSigningProfilesRequestListSigningProfilesPaginateTypeDef = TypedDict(
+    "ListSigningProfilesRequestListSigningProfilesPaginateTypeDef",
+    {
+        "includeCanceled": bool,
+        "platformId": str,
+        "statuses": Sequence[SigningProfileStatusType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSigningProfilesRequestRequestTypeDef = TypedDict(
     "ListSigningProfilesRequestRequestTypeDef",
     {
         "includeCanceled": bool,
         "maxResults": int,
         "nextToken": str,
         "platformId": str,
@@ -337,23 +393,70 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
+PutSigningProfileResponseTypeDef = TypedDict(
+    "PutSigningProfileResponseTypeDef",
+    {
+        "arn": str,
+        "profileVersion": str,
+        "profileVersionArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RemoveProfilePermissionRequestRequestTypeDef = TypedDict(
     "RemoveProfilePermissionRequestRequestTypeDef",
     {
         "profileName": str,
         "revisionId": str,
         "statementId": str,
     },
 )
 
+RemoveProfilePermissionResponseTypeDef = TypedDict(
+    "RemoveProfilePermissionResponseTypeDef",
+    {
+        "revisionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 _RequiredRevokeSignatureRequestRequestTypeDef = TypedDict(
     "_RequiredRevokeSignatureRequestRequestTypeDef",
     {
         "jobId": str,
         "reason": str,
     },
 )
@@ -396,86 +499,79 @@
     {
         "bucketName": str,
         "key": str,
         "version": str,
     },
 )
 
-SigningConfigurationOverridesTypeDef = TypedDict(
-    "SigningConfigurationOverridesTypeDef",
+_RequiredSignPayloadRequestRequestTypeDef = TypedDict(
+    "_RequiredSignPayloadRequestRequestTypeDef",
     {
-        "encryptionAlgorithm": EncryptionAlgorithmType,
-        "hashAlgorithm": HashAlgorithmType,
+        "profileName": str,
+        "payload": Union[str, bytes, IO[Any], StreamingBody],
+        "payloadFormat": str,
     },
-    total=False,
 )
-
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+_OptionalSignPayloadRequestRequestTypeDef = TypedDict(
+    "_OptionalSignPayloadRequestRequestTypeDef",
     {
-        "resourceArn": str,
-        "tags": Mapping[str, str],
+        "profileOwner": str,
     },
+    total=False,
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
-    {
-        "resourceArn": str,
-        "tagKeys": Sequence[str],
-    },
-)
 
-AddProfilePermissionResponseTypeDef = TypedDict(
-    "AddProfilePermissionResponseTypeDef",
-    {
-        "revisionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class SignPayloadRequestRequestTypeDef(
+    _RequiredSignPayloadRequestRequestTypeDef, _OptionalSignPayloadRequestRequestTypeDef
+):
+    pass
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+
+SignPayloadResponseTypeDef = TypedDict(
+    "SignPayloadResponseTypeDef",
     {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "jobId": str,
+        "jobOwner": str,
+        "metadata": Dict[str, str],
+        "signature": bytes,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+SigningConfigurationOverridesTypeDef = TypedDict(
+    "SigningConfigurationOverridesTypeDef",
     {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "encryptionAlgorithm": EncryptionAlgorithmType,
+        "hashAlgorithm": HashAlgorithmType,
     },
+    total=False,
 )
 
-PutSigningProfileResponseTypeDef = TypedDict(
-    "PutSigningProfileResponseTypeDef",
+StartSigningJobResponseTypeDef = TypedDict(
+    "StartSigningJobResponseTypeDef",
     {
-        "arn": str,
-        "profileVersion": str,
-        "profileVersionArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "jobId": str,
+        "jobOwner": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RemoveProfilePermissionResponseTypeDef = TypedDict(
-    "RemoveProfilePermissionResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "revisionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "resourceArn": str,
+        "tags": Mapping[str, str],
     },
 )
 
-StartSigningJobResponseTypeDef = TypedDict(
-    "StartSigningJobResponseTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "jobId": str,
-        "jobOwner": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "resourceArn": str,
+        "tagKeys": Sequence[str],
     },
 )
 
 _RequiredDescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef = TypedDict(
     "_RequiredDescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef",
     {
         "jobId": str,
@@ -534,53 +630,16 @@
 ListProfilePermissionsResponseTypeDef = TypedDict(
     "ListProfilePermissionsResponseTypeDef",
     {
         "revisionId": str,
         "policySizeBytes": int,
         "permissions": List[PermissionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListSigningJobsRequestListSigningJobsPaginateTypeDef = TypedDict(
-    "ListSigningJobsRequestListSigningJobsPaginateTypeDef",
-    {
-        "status": SigningStatusType,
-        "platformId": str,
-        "requestedBy": str,
-        "isRevoked": bool,
-        "signatureExpiresBefore": Union[datetime, str],
-        "signatureExpiresAfter": Union[datetime, str],
-        "jobInvoker": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef = TypedDict(
-    "ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef",
-    {
-        "category": str,
-        "partner": str,
-        "target": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSigningProfilesRequestListSigningProfilesPaginateTypeDef = TypedDict(
-    "ListSigningProfilesRequestListSigningProfilesPaginateTypeDef",
-    {
-        "includeCanceled": bool,
-        "platformId": str,
-        "statuses": Sequence[SigningProfileStatusType],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 SignedObjectTypeDef = TypedDict(
     "SignedObjectTypeDef",
     {
         "s3": S3SignedObjectTypeDef,
     },
@@ -605,15 +664,15 @@
 )
 
 ListSigningProfilesResponseTypeDef = TypedDict(
     "ListSigningProfilesResponseTypeDef",
     {
         "profiles": List[SigningProfileTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSigningPlatformResponseTypeDef = TypedDict(
     "GetSigningPlatformResponseTypeDef",
     {
         "platformId": str,
@@ -621,15 +680,15 @@
         "partner": str,
         "target": str,
         "category": Literal["AWSIoT"],
         "signingConfiguration": SigningConfigurationTypeDef,
         "signingImageFormat": SigningImageFormatTypeDef,
         "maxSizeInMB": int,
         "revocationSupported": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SigningPlatformTypeDef = TypedDict(
     "SigningPlatformTypeDef",
     {
         "platformId": str,
@@ -708,15 +767,15 @@
         "requestedBy": str,
         "status": SigningStatusType,
         "statusReason": str,
         "revocationRecord": SigningJobRevocationRecordTypeDef,
         "signedObject": SignedObjectTypeDef,
         "jobOwner": str,
         "jobInvoker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSigningProfileResponseTypeDef = TypedDict(
     "GetSigningProfileResponseTypeDef",
     {
         "profileName": str,
@@ -729,15 +788,15 @@
         "signatureValidityPeriod": SignatureValidityPeriodTypeDef,
         "overrides": SigningPlatformOverridesTypeDef,
         "signingParameters": Dict[str, str],
         "status": SigningProfileStatusType,
         "statusReason": str,
         "arn": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutSigningProfileRequestRequestTypeDef = TypedDict(
     "_RequiredPutSigningProfileRequestRequestTypeDef",
     {
         "profileName": str,
@@ -764,19 +823,19 @@
 
 
 ListSigningPlatformsResponseTypeDef = TypedDict(
     "ListSigningPlatformsResponseTypeDef",
     {
         "platforms": List[SigningPlatformTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSigningJobsResponseTypeDef = TypedDict(
     "ListSigningJobsResponseTypeDef",
     {
         "jobs": List[SigningJobTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-signer-1.26.0.post1/mypy_boto3_signer/type_defs.pyi` & `mypy-boto3-signer-1.26.148/mypy_boto3_signer/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,17 @@
     from mypy_boto3_signer.type_defs import AddProfilePermissionRequestRequestTypeDef
 
     data: AddProfilePermissionRequestRequestTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import IO, Any, Dict, List, Mapping, Sequence, Union
+
+from botocore.response import StreamingBody
 
 from .literals import (
     EncryptionAlgorithmType,
     HashAlgorithmType,
     ImageFormatType,
     SigningProfileStatusType,
     SigningStatusType,
@@ -31,57 +33,61 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AddProfilePermissionRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "AddProfilePermissionResponseTypeDef",
     "CancelSigningProfileRequestRequestTypeDef",
     "DescribeSigningJobRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "SigningJobRevocationRecordTypeDef",
     "SigningMaterialTypeDef",
     "S3DestinationTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EncryptionAlgorithmOptionsTypeDef",
+    "GetRevocationStatusRequestRequestTypeDef",
+    "GetRevocationStatusResponseTypeDef",
     "GetSigningPlatformRequestRequestTypeDef",
     "SigningImageFormatTypeDef",
     "GetSigningProfileRequestRequestTypeDef",
     "SignatureValidityPeriodTypeDef",
     "SigningProfileRevocationRecordTypeDef",
     "HashAlgorithmOptionsTypeDef",
     "ListProfilePermissionsRequestRequestTypeDef",
     "PermissionTypeDef",
-    "PaginatorConfigTypeDef",
+    "ListSigningJobsRequestListSigningJobsPaginateTypeDef",
     "ListSigningJobsRequestRequestTypeDef",
+    "ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef",
     "ListSigningPlatformsRequestRequestTypeDef",
+    "ListSigningProfilesRequestListSigningProfilesPaginateTypeDef",
     "ListSigningProfilesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PaginatorConfigTypeDef",
+    "PutSigningProfileResponseTypeDef",
     "RemoveProfilePermissionRequestRequestTypeDef",
+    "RemoveProfilePermissionResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "RevokeSignatureRequestRequestTypeDef",
     "RevokeSigningProfileRequestRequestTypeDef",
     "S3SignedObjectTypeDef",
     "S3SourceTypeDef",
+    "SignPayloadRequestRequestTypeDef",
+    "SignPayloadResponseTypeDef",
     "SigningConfigurationOverridesTypeDef",
+    "StartSigningJobResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "AddProfilePermissionResponseTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PutSigningProfileResponseTypeDef",
-    "RemoveProfilePermissionResponseTypeDef",
-    "StartSigningJobResponseTypeDef",
     "DescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef",
     "DestinationTypeDef",
     "SigningProfileTypeDef",
     "SigningConfigurationTypeDef",
     "ListProfilePermissionsResponseTypeDef",
-    "ListSigningJobsRequestListSigningJobsPaginateTypeDef",
-    "ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef",
-    "ListSigningProfilesRequestListSigningProfilesPaginateTypeDef",
     "SignedObjectTypeDef",
     "SourceTypeDef",
     "SigningPlatformOverridesTypeDef",
     "ListSigningProfilesResponseTypeDef",
     "GetSigningPlatformResponseTypeDef",
     "SigningPlatformTypeDef",
     "SigningJobTypeDef",
@@ -113,22 +119,19 @@
 
 class AddProfilePermissionRequestRequestTypeDef(
     _RequiredAddProfilePermissionRequestRequestTypeDef,
     _OptionalAddProfilePermissionRequestRequestTypeDef,
 ):
     pass
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+AddProfilePermissionResponseTypeDef = TypedDict(
+    "AddProfilePermissionResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "revisionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 CancelSigningProfileRequestRequestTypeDef = TypedDict(
     "CancelSigningProfileRequestRequestTypeDef",
     {
         "profileName": str,
@@ -173,22 +176,48 @@
     {
         "bucketName": str,
         "prefix": str,
     },
     total=False,
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 EncryptionAlgorithmOptionsTypeDef = TypedDict(
     "EncryptionAlgorithmOptionsTypeDef",
     {
         "allowedValues": List[EncryptionAlgorithmType],
         "defaultValue": EncryptionAlgorithmType,
     },
 )
 
+GetRevocationStatusRequestRequestTypeDef = TypedDict(
+    "GetRevocationStatusRequestRequestTypeDef",
+    {
+        "signatureTimestamp": Union[datetime, str],
+        "platformId": str,
+        "profileVersionArn": str,
+        "jobArn": str,
+        "certificateHashes": Sequence[str],
+    },
+)
+
+GetRevocationStatusResponseTypeDef = TypedDict(
+    "GetRevocationStatusResponseTypeDef",
+    {
+        "revokedEntities": List[str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 GetSigningPlatformRequestRequestTypeDef = TypedDict(
     "GetSigningPlatformRequestRequestTypeDef",
     {
         "platformId": str,
     },
 )
 
@@ -273,20 +302,25 @@
         "principal": str,
         "statementId": str,
         "profileVersion": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+ListSigningJobsRequestListSigningJobsPaginateTypeDef = TypedDict(
+    "ListSigningJobsRequestListSigningJobsPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "status": SigningStatusType,
+        "platformId": str,
+        "requestedBy": str,
+        "isRevoked": bool,
+        "signatureExpiresBefore": Union[datetime, str],
+        "signatureExpiresAfter": Union[datetime, str],
+        "jobInvoker": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
 ListSigningJobsRequestRequestTypeDef = TypedDict(
     "ListSigningJobsRequestRequestTypeDef",
     {
@@ -299,26 +333,48 @@
         "signatureExpiresBefore": Union[datetime, str],
         "signatureExpiresAfter": Union[datetime, str],
         "jobInvoker": str,
     },
     total=False,
 )
 
+ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef = TypedDict(
+    "ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef",
+    {
+        "category": str,
+        "partner": str,
+        "target": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSigningPlatformsRequestRequestTypeDef = TypedDict(
     "ListSigningPlatformsRequestRequestTypeDef",
     {
         "category": str,
         "partner": str,
         "target": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+ListSigningProfilesRequestListSigningProfilesPaginateTypeDef = TypedDict(
+    "ListSigningProfilesRequestListSigningProfilesPaginateTypeDef",
+    {
+        "includeCanceled": bool,
+        "platformId": str,
+        "statuses": Sequence[SigningProfileStatusType],
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListSigningProfilesRequestRequestTypeDef = TypedDict(
     "ListSigningProfilesRequestRequestTypeDef",
     {
         "includeCanceled": bool,
         "maxResults": int,
         "nextToken": str,
         "platformId": str,
@@ -330,23 +386,70 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
+PutSigningProfileResponseTypeDef = TypedDict(
+    "PutSigningProfileResponseTypeDef",
+    {
+        "arn": str,
+        "profileVersion": str,
+        "profileVersionArn": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 RemoveProfilePermissionRequestRequestTypeDef = TypedDict(
     "RemoveProfilePermissionRequestRequestTypeDef",
     {
         "profileName": str,
         "revisionId": str,
         "statementId": str,
     },
 )
 
+RemoveProfilePermissionResponseTypeDef = TypedDict(
+    "RemoveProfilePermissionResponseTypeDef",
+    {
+        "revisionId": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 _RequiredRevokeSignatureRequestRequestTypeDef = TypedDict(
     "_RequiredRevokeSignatureRequestRequestTypeDef",
     {
         "jobId": str,
         "reason": str,
     },
 )
@@ -387,86 +490,77 @@
     {
         "bucketName": str,
         "key": str,
         "version": str,
     },
 )
 
-SigningConfigurationOverridesTypeDef = TypedDict(
-    "SigningConfigurationOverridesTypeDef",
+_RequiredSignPayloadRequestRequestTypeDef = TypedDict(
+    "_RequiredSignPayloadRequestRequestTypeDef",
     {
-        "encryptionAlgorithm": EncryptionAlgorithmType,
-        "hashAlgorithm": HashAlgorithmType,
+        "profileName": str,
+        "payload": Union[str, bytes, IO[Any], StreamingBody],
+        "payloadFormat": str,
     },
-    total=False,
 )
-
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+_OptionalSignPayloadRequestRequestTypeDef = TypedDict(
+    "_OptionalSignPayloadRequestRequestTypeDef",
     {
-        "resourceArn": str,
-        "tags": Mapping[str, str],
-    },
-)
-
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
-    {
-        "resourceArn": str,
-        "tagKeys": Sequence[str],
+        "profileOwner": str,
     },
+    total=False,
 )
 
-AddProfilePermissionResponseTypeDef = TypedDict(
-    "AddProfilePermissionResponseTypeDef",
-    {
-        "revisionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+class SignPayloadRequestRequestTypeDef(
+    _RequiredSignPayloadRequestRequestTypeDef, _OptionalSignPayloadRequestRequestTypeDef
+):
+    pass
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+SignPayloadResponseTypeDef = TypedDict(
+    "SignPayloadResponseTypeDef",
     {
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "jobId": str,
+        "jobOwner": str,
+        "metadata": Dict[str, str],
+        "signature": bytes,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+SigningConfigurationOverridesTypeDef = TypedDict(
+    "SigningConfigurationOverridesTypeDef",
     {
-        "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "encryptionAlgorithm": EncryptionAlgorithmType,
+        "hashAlgorithm": HashAlgorithmType,
     },
+    total=False,
 )
 
-PutSigningProfileResponseTypeDef = TypedDict(
-    "PutSigningProfileResponseTypeDef",
+StartSigningJobResponseTypeDef = TypedDict(
+    "StartSigningJobResponseTypeDef",
     {
-        "arn": str,
-        "profileVersion": str,
-        "profileVersionArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "jobId": str,
+        "jobOwner": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-RemoveProfilePermissionResponseTypeDef = TypedDict(
-    "RemoveProfilePermissionResponseTypeDef",
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
     {
-        "revisionId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "resourceArn": str,
+        "tags": Mapping[str, str],
     },
 )
 
-StartSigningJobResponseTypeDef = TypedDict(
-    "StartSigningJobResponseTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "jobId": str,
-        "jobOwner": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "resourceArn": str,
+        "tagKeys": Sequence[str],
     },
 )
 
 _RequiredDescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef = TypedDict(
     "_RequiredDescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef",
     {
         "jobId": str,
@@ -523,53 +617,16 @@
 ListProfilePermissionsResponseTypeDef = TypedDict(
     "ListProfilePermissionsResponseTypeDef",
     {
         "revisionId": str,
         "policySizeBytes": int,
         "permissions": List[PermissionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListSigningJobsRequestListSigningJobsPaginateTypeDef = TypedDict(
-    "ListSigningJobsRequestListSigningJobsPaginateTypeDef",
-    {
-        "status": SigningStatusType,
-        "platformId": str,
-        "requestedBy": str,
-        "isRevoked": bool,
-        "signatureExpiresBefore": Union[datetime, str],
-        "signatureExpiresAfter": Union[datetime, str],
-        "jobInvoker": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef = TypedDict(
-    "ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef",
-    {
-        "category": str,
-        "partner": str,
-        "target": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-ListSigningProfilesRequestListSigningProfilesPaginateTypeDef = TypedDict(
-    "ListSigningProfilesRequestListSigningProfilesPaginateTypeDef",
-    {
-        "includeCanceled": bool,
-        "platformId": str,
-        "statuses": Sequence[SigningProfileStatusType],
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 SignedObjectTypeDef = TypedDict(
     "SignedObjectTypeDef",
     {
         "s3": S3SignedObjectTypeDef,
     },
@@ -594,15 +651,15 @@
 )
 
 ListSigningProfilesResponseTypeDef = TypedDict(
     "ListSigningProfilesResponseTypeDef",
     {
         "profiles": List[SigningProfileTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSigningPlatformResponseTypeDef = TypedDict(
     "GetSigningPlatformResponseTypeDef",
     {
         "platformId": str,
@@ -610,15 +667,15 @@
         "partner": str,
         "target": str,
         "category": Literal["AWSIoT"],
         "signingConfiguration": SigningConfigurationTypeDef,
         "signingImageFormat": SigningImageFormatTypeDef,
         "maxSizeInMB": int,
         "revocationSupported": bool,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SigningPlatformTypeDef = TypedDict(
     "SigningPlatformTypeDef",
     {
         "platformId": str,
@@ -695,15 +752,15 @@
         "requestedBy": str,
         "status": SigningStatusType,
         "statusReason": str,
         "revocationRecord": SigningJobRevocationRecordTypeDef,
         "signedObject": SignedObjectTypeDef,
         "jobOwner": str,
         "jobInvoker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 GetSigningProfileResponseTypeDef = TypedDict(
     "GetSigningProfileResponseTypeDef",
     {
         "profileName": str,
@@ -716,15 +773,15 @@
         "signatureValidityPeriod": SignatureValidityPeriodTypeDef,
         "overrides": SigningPlatformOverridesTypeDef,
         "signingParameters": Dict[str, str],
         "status": SigningProfileStatusType,
         "statusReason": str,
         "arn": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 _RequiredPutSigningProfileRequestRequestTypeDef = TypedDict(
     "_RequiredPutSigningProfileRequestRequestTypeDef",
     {
         "profileName": str,
@@ -749,19 +806,19 @@
     pass
 
 ListSigningPlatformsResponseTypeDef = TypedDict(
     "ListSigningPlatformsResponseTypeDef",
     {
         "platforms": List[SigningPlatformTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ListSigningJobsResponseTypeDef = TypedDict(
     "ListSigningJobsResponseTypeDef",
     {
         "jobs": List[SigningJobTypeDef],
         "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
```

### Comparing `mypy-boto3-signer-1.26.0.post1/mypy_boto3_signer/waiter.py` & `mypy-boto3-signer-1.26.148/mypy_boto3_signer/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-signer-1.26.0.post1/mypy_boto3_signer/waiter.pyi` & `mypy-boto3-signer-1.26.148/mypy_boto3_signer/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-signer-1.26.0.post1/mypy_boto3_signer.egg-info/PKG-INFO` & `mypy-boto3-signer-1.26.148/mypy_boto3_signer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-signer
-Version: 1.26.0.post1
-Summary: Type annotations for boto3.signer 1.26.0 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.148
+Summary: Type annotations for boto3.signer 1.26.148 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,43 +18,44 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-signer"></a>
 
 # mypy-boto3-signer
 
 [![PyPI - mypy-boto3-signer](https://img.shields.io/pypi/v/mypy-boto3-signer.svg?color=blue)](https://pypi.org/project/mypy-boto3-signer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-signer.svg?color=blue)](https://pypi.org/project/mypy-boto3-signer)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-signer?color=blue)](https://pypistats.org/packages/mypy-boto3-signer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.signer 1.26.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
+[boto3.signer 1.26.148](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer.html#signer)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-signer docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -343,14 +344,15 @@
     SuccessfulSigningJobWaiterName,
     ValidityTypeType,
     signerServiceName,
     ServiceName,
     ResourceServiceName,
     PaginatorName,
     WaiterName,
+    RegionName,
 )
 
 
 def check_value(value: CategoryType) -> bool:
     ...
 ```
 
@@ -360,57 +362,61 @@
 
 `mypy_boto3_signer.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_signer.type_defs import (
     AddProfilePermissionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    AddProfilePermissionResponseTypeDef,
     CancelSigningProfileRequestRequestTypeDef,
     DescribeSigningJobRequestRequestTypeDef,
     WaiterConfigTypeDef,
     SigningJobRevocationRecordTypeDef,
     SigningMaterialTypeDef,
     S3DestinationTypeDef,
+    EmptyResponseMetadataTypeDef,
     EncryptionAlgorithmOptionsTypeDef,
+    GetRevocationStatusRequestRequestTypeDef,
+    GetRevocationStatusResponseTypeDef,
     GetSigningPlatformRequestRequestTypeDef,
     SigningImageFormatTypeDef,
     GetSigningProfileRequestRequestTypeDef,
     SignatureValidityPeriodTypeDef,
     SigningProfileRevocationRecordTypeDef,
     HashAlgorithmOptionsTypeDef,
     ListProfilePermissionsRequestRequestTypeDef,
     PermissionTypeDef,
-    PaginatorConfigTypeDef,
+    ListSigningJobsRequestListSigningJobsPaginateTypeDef,
     ListSigningJobsRequestRequestTypeDef,
+    ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef,
     ListSigningPlatformsRequestRequestTypeDef,
+    ListSigningProfilesRequestListSigningProfilesPaginateTypeDef,
     ListSigningProfilesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PaginatorConfigTypeDef,
+    PutSigningProfileResponseTypeDef,
     RemoveProfilePermissionRequestRequestTypeDef,
+    RemoveProfilePermissionResponseTypeDef,
+    ResponseMetadataTypeDef,
     RevokeSignatureRequestRequestTypeDef,
     RevokeSigningProfileRequestRequestTypeDef,
     S3SignedObjectTypeDef,
     S3SourceTypeDef,
+    SignPayloadRequestRequestTypeDef,
+    SignPayloadResponseTypeDef,
     SigningConfigurationOverridesTypeDef,
+    StartSigningJobResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    AddProfilePermissionResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PutSigningProfileResponseTypeDef,
-    RemoveProfilePermissionResponseTypeDef,
-    StartSigningJobResponseTypeDef,
     DescribeSigningJobRequestSuccessfulSigningJobWaitTypeDef,
     DestinationTypeDef,
     SigningProfileTypeDef,
     SigningConfigurationTypeDef,
     ListProfilePermissionsResponseTypeDef,
-    ListSigningJobsRequestListSigningJobsPaginateTypeDef,
-    ListSigningPlatformsRequestListSigningPlatformsPaginateTypeDef,
-    ListSigningProfilesRequestListSigningProfilesPaginateTypeDef,
     SignedObjectTypeDef,
     SourceTypeDef,
     SigningPlatformOverridesTypeDef,
     ListSigningProfilesResponseTypeDef,
     GetSigningPlatformResponseTypeDef,
     SigningPlatformTypeDef,
     SigningJobTypeDef,
@@ -430,42 +436,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-signer-1.26.0.post1/mypy_boto3_signer.egg-info/SOURCES.txt` & `mypy-boto3-signer-1.26.148/mypy_boto3_signer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-signer-1.26.0.post1/setup.py` & `mypy-boto3-signer-1.26.148/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,53 +1,55 @@
 """
 Setup script for mypy-boto3-signer.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-signer",
-    version="1.26.0.post1",
+    version="1.26.148",
     packages=["mypy_boto3_signer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.signer 1.26.0 service generated with mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.signer 1.26.148 service generated with mypy-boto3-builder"
+        " 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 signer type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_signer": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_signer": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_signer/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        "typing-extensions>=4.1.0",
+        'typing-extensions>=4.1.0; python_version<"3.9"',
     ],
     zip_safe=False,
 )
```

