# Comparing `tmp/mypy-boto3-sqs-1.26.129.tar.gz` & `tmp/mypy-boto3-sqs-1.26.148.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-sqs-1.26.129.tar", last modified: Fri May  5 21:04:56 2023, max compression
+gzip compressed data, was "mypy-boto3-sqs-1.26.148.tar", last modified: Tue Jun  6 19:35:54 2023, max compression
```

## Comparing `mypy-boto3-sqs-1.26.129.tar` & `mypy-boto3-sqs-1.26.148.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:04:56.671841 mypy-boto3-sqs-1.26.129/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-05 21:04:46.000000 mypy-boto3-sqs-1.26.129/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17427 2023-05-05 21:04:56.671841 mypy-boto3-sqs-1.26.129/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15954 2023-05-05 21:04:46.000000 mypy-boto3-sqs-1.26.129/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:04:56.667842 mypy-boto3-sqs-1.26.129/mypy_boto3_sqs/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-05 21:04:46.000000 mypy-boto3-sqs-1.26.129/mypy_boto3_sqs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-05 21:04:46.000000 mypy-boto3-sqs-1.26.129/mypy_boto3_sqs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-05 21:04:46.000000 mypy-boto3-sqs-1.26.129/mypy_boto3_sqs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16091 2023-05-05 21:04:46.000000 mypy-boto3-sqs-1.26.129/mypy_boto3_sqs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16062 2023-05-05 21:04:46.000000 mypy-boto3-sqs-1.26.129/mypy_boto3_sqs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10185 2023-05-05 21:04:46.000000 mypy-boto3-sqs-1.26.129/mypy_boto3_sqs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10183 2023-05-05 21:04:46.000000 mypy-boto3-sqs-1.26.129/mypy_boto3_sqs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-05-05 21:04:46.000000 mypy-boto3-sqs-1.26.129/mypy_boto3_sqs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-05-05 21:04:46.000000 mypy-boto3-sqs-1.26.129/mypy_boto3_sqs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 21:04:46.000000 mypy-boto3-sqs-1.26.129/mypy_boto3_sqs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    18793 2023-05-05 21:04:46.000000 mypy-boto3-sqs-1.26.129/mypy_boto3_sqs/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    18754 2023-05-05 21:04:46.000000 mypy-boto3-sqs-1.26.129/mypy_boto3_sqs/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    21885 2023-05-05 21:04:47.000000 mypy-boto3-sqs-1.26.129/mypy_boto3_sqs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21852 2023-05-05 21:04:47.000000 mypy-boto3-sqs-1.26.129/mypy_boto3_sqs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-05 21:04:46.000000 mypy-boto3-sqs-1.26.129/mypy_boto3_sqs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:04:56.671841 mypy-boto3-sqs-1.26.129/mypy_boto3_sqs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17427 2023-05-05 21:04:56.000000 mypy-boto3-sqs-1.26.129/mypy_boto3_sqs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-05 21:04:56.000000 mypy-boto3-sqs-1.26.129/mypy_boto3_sqs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 21:04:56.000000 mypy-boto3-sqs-1.26.129/mypy_boto3_sqs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 21:04:56.000000 mypy-boto3-sqs-1.26.129/mypy_boto3_sqs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-05 21:04:56.000000 mypy-boto3-sqs-1.26.129/mypy_boto3_sqs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 21:04:56.000000 mypy-boto3-sqs-1.26.129/mypy_boto3_sqs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 21:04:56.671841 mypy-boto3-sqs-1.26.129/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-05 21:04:46.000000 mypy-boto3-sqs-1.26.129/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:35:54.118339 mypy-boto3-sqs-1.26.148/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-06 19:35:33.000000 mypy-boto3-sqs-1.26.148/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17731 2023-06-06 19:35:54.118339 mypy-boto3-sqs-1.26.148/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16258 2023-06-06 19:35:33.000000 mypy-boto3-sqs-1.26.148/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:35:54.114339 mypy-boto3-sqs-1.26.148/mypy_boto3_sqs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-06 19:35:33.000000 mypy-boto3-sqs-1.26.148/mypy_boto3_sqs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-06 19:35:33.000000 mypy-boto3-sqs-1.26.148/mypy_boto3_sqs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-06 19:35:33.000000 mypy-boto3-sqs-1.26.148/mypy_boto3_sqs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18039 2023-06-06 19:35:33.000000 mypy-boto3-sqs-1.26.148/mypy_boto3_sqs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18007 2023-06-06 19:35:33.000000 mypy-boto3-sqs-1.26.148/mypy_boto3_sqs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10239 2023-06-06 19:35:34.000000 mypy-boto3-sqs-1.26.148/mypy_boto3_sqs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-06-06 19:35:34.000000 mypy-boto3-sqs-1.26.148/mypy_boto3_sqs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-06 19:35:34.000000 mypy-boto3-sqs-1.26.148/mypy_boto3_sqs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-06-06 19:35:34.000000 mypy-boto3-sqs-1.26.148/mypy_boto3_sqs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 19:35:33.000000 mypy-boto3-sqs-1.26.148/mypy_boto3_sqs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18940 2023-06-06 19:35:34.000000 mypy-boto3-sqs-1.26.148/mypy_boto3_sqs/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18901 2023-06-06 19:35:34.000000 mypy-boto3-sqs-1.26.148/mypy_boto3_sqs/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    24536 2023-06-06 19:35:35.000000 mypy-boto3-sqs-1.26.148/mypy_boto3_sqs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24499 2023-06-06 19:35:34.000000 mypy-boto3-sqs-1.26.148/mypy_boto3_sqs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-06 19:35:33.000000 mypy-boto3-sqs-1.26.148/mypy_boto3_sqs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:35:54.114339 mypy-boto3-sqs-1.26.148/mypy_boto3_sqs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17731 2023-06-06 19:35:54.000000 mypy-boto3-sqs-1.26.148/mypy_boto3_sqs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-06 19:35:54.000000 mypy-boto3-sqs-1.26.148/mypy_boto3_sqs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 19:35:54.000000 mypy-boto3-sqs-1.26.148/mypy_boto3_sqs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 19:35:54.000000 mypy-boto3-sqs-1.26.148/mypy_boto3_sqs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-06 19:35:54.000000 mypy-boto3-sqs-1.26.148/mypy_boto3_sqs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-06 19:35:54.000000 mypy-boto3-sqs-1.26.148/mypy_boto3_sqs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 19:35:54.118339 mypy-boto3-sqs-1.26.148/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-06 19:35:33.000000 mypy-boto3-sqs-1.26.148/setup.py
```

### Comparing `mypy-boto3-sqs-1.26.129/LICENSE` & `mypy-boto3-sqs-1.26.148/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.26.129/PKG-INFO` & `mypy-boto3-sqs-1.26.148/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sqs
-Version: 1.26.129
-Summary: Type annotations for boto3.SQS 1.26.129 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.148
+Summary: Type annotations for boto3.SQS 1.26.148 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sqs.svg?color=blue)](https://pypi.org/project/mypy-boto3-sqs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sqs?color=blue)](https://pypistats.org/packages/mypy-boto3-sqs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SQS 1.26.129](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
+[boto3.SQS 1.26.148](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -415,60 +415,67 @@
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sqs.type_defs import (
     AddPermissionRequestQueueAddPermissionTypeDef,
     AddPermissionRequestRequestTypeDef,
     BatchResultErrorEntryTypeDef,
+    CancelMessageMoveTaskRequestRequestTypeDef,
+    CancelMessageMoveTaskResultTypeDef,
     ChangeMessageVisibilityBatchRequestEntryTypeDef,
     ChangeMessageVisibilityBatchResultEntryTypeDef,
-    ResponseMetadataTypeDef,
     ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef,
     ChangeMessageVisibilityRequestRequestTypeDef,
     CreateQueueRequestRequestTypeDef,
     CreateQueueRequestServiceResourceCreateQueueTypeDef,
+    CreateQueueResultTypeDef,
     DeleteMessageBatchRequestEntryTypeDef,
     DeleteMessageBatchResultEntryTypeDef,
     DeleteMessageRequestRequestTypeDef,
     DeleteQueueRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetQueueAttributesRequestRequestTypeDef,
+    GetQueueAttributesResultTypeDef,
     GetQueueUrlRequestRequestTypeDef,
     GetQueueUrlRequestServiceResourceGetQueueByNameTypeDef,
-    PaginatorConfigTypeDef,
+    GetQueueUrlResultTypeDef,
+    ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
     ListDeadLetterSourceQueuesRequestRequestTypeDef,
+    ListDeadLetterSourceQueuesResultTypeDef,
+    ListMessageMoveTasksRequestRequestTypeDef,
+    ListMessageMoveTasksResultEntryTypeDef,
     ListQueueTagsRequestRequestTypeDef,
+    ListQueueTagsResultTypeDef,
+    ListQueuesRequestListQueuesPaginateTypeDef,
     ListQueuesRequestRequestTypeDef,
+    ListQueuesResultTypeDef,
     MessageAttributeValueTypeDef,
     MessageSystemAttributeValueTypeDef,
+    PaginatorConfigTypeDef,
     PurgeQueueRequestRequestTypeDef,
     ReceiveMessageRequestQueueReceiveMessagesTypeDef,
     ReceiveMessageRequestRequestTypeDef,
     RemovePermissionRequestQueueRemovePermissionTypeDef,
     RemovePermissionRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     SendMessageBatchResultEntryTypeDef,
+    SendMessageResultTypeDef,
     SetQueueAttributesRequestQueueSetAttributesTypeDef,
     SetQueueAttributesRequestRequestTypeDef,
+    StartMessageMoveTaskRequestRequestTypeDef,
+    StartMessageMoveTaskResultTypeDef,
     TagQueueRequestRequestTypeDef,
     UntagQueueRequestRequestTypeDef,
     ChangeMessageVisibilityBatchRequestQueueChangeMessageVisibilityBatchTypeDef,
     ChangeMessageVisibilityBatchRequestRequestTypeDef,
     ChangeMessageVisibilityBatchResultTypeDef,
-    CreateQueueResultTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetQueueAttributesResultTypeDef,
-    GetQueueUrlResultTypeDef,
-    ListDeadLetterSourceQueuesResultTypeDef,
-    ListQueueTagsResultTypeDef,
-    ListQueuesResultTypeDef,
-    SendMessageResultTypeDef,
     DeleteMessageBatchRequestQueueDeleteMessagesTypeDef,
     DeleteMessageBatchRequestRequestTypeDef,
     DeleteMessageBatchResultTypeDef,
-    ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
-    ListQueuesRequestListQueuesPaginateTypeDef,
+    ListMessageMoveTasksResultTypeDef,
     MessageTypeDef,
     SendMessageBatchRequestEntryTypeDef,
     SendMessageRequestQueueSendMessageTypeDef,
     SendMessageRequestRequestTypeDef,
     SendMessageBatchResultTypeDef,
     ReceiveMessageResultTypeDef,
     SendMessageBatchRequestQueueSendMessagesTypeDef,
```

### Comparing `mypy-boto3-sqs-1.26.129/README.md` & `mypy-boto3-sqs-1.26.148/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sqs.svg?color=blue)](https://pypi.org/project/mypy-boto3-sqs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sqs?color=blue)](https://pypistats.org/packages/mypy-boto3-sqs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SQS 1.26.129](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
+[boto3.SQS 1.26.148](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -383,60 +383,67 @@
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sqs.type_defs import (
     AddPermissionRequestQueueAddPermissionTypeDef,
     AddPermissionRequestRequestTypeDef,
     BatchResultErrorEntryTypeDef,
+    CancelMessageMoveTaskRequestRequestTypeDef,
+    CancelMessageMoveTaskResultTypeDef,
     ChangeMessageVisibilityBatchRequestEntryTypeDef,
     ChangeMessageVisibilityBatchResultEntryTypeDef,
-    ResponseMetadataTypeDef,
     ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef,
     ChangeMessageVisibilityRequestRequestTypeDef,
     CreateQueueRequestRequestTypeDef,
     CreateQueueRequestServiceResourceCreateQueueTypeDef,
+    CreateQueueResultTypeDef,
     DeleteMessageBatchRequestEntryTypeDef,
     DeleteMessageBatchResultEntryTypeDef,
     DeleteMessageRequestRequestTypeDef,
     DeleteQueueRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetQueueAttributesRequestRequestTypeDef,
+    GetQueueAttributesResultTypeDef,
     GetQueueUrlRequestRequestTypeDef,
     GetQueueUrlRequestServiceResourceGetQueueByNameTypeDef,
-    PaginatorConfigTypeDef,
+    GetQueueUrlResultTypeDef,
+    ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
     ListDeadLetterSourceQueuesRequestRequestTypeDef,
+    ListDeadLetterSourceQueuesResultTypeDef,
+    ListMessageMoveTasksRequestRequestTypeDef,
+    ListMessageMoveTasksResultEntryTypeDef,
     ListQueueTagsRequestRequestTypeDef,
+    ListQueueTagsResultTypeDef,
+    ListQueuesRequestListQueuesPaginateTypeDef,
     ListQueuesRequestRequestTypeDef,
+    ListQueuesResultTypeDef,
     MessageAttributeValueTypeDef,
     MessageSystemAttributeValueTypeDef,
+    PaginatorConfigTypeDef,
     PurgeQueueRequestRequestTypeDef,
     ReceiveMessageRequestQueueReceiveMessagesTypeDef,
     ReceiveMessageRequestRequestTypeDef,
     RemovePermissionRequestQueueRemovePermissionTypeDef,
     RemovePermissionRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     SendMessageBatchResultEntryTypeDef,
+    SendMessageResultTypeDef,
     SetQueueAttributesRequestQueueSetAttributesTypeDef,
     SetQueueAttributesRequestRequestTypeDef,
+    StartMessageMoveTaskRequestRequestTypeDef,
+    StartMessageMoveTaskResultTypeDef,
     TagQueueRequestRequestTypeDef,
     UntagQueueRequestRequestTypeDef,
     ChangeMessageVisibilityBatchRequestQueueChangeMessageVisibilityBatchTypeDef,
     ChangeMessageVisibilityBatchRequestRequestTypeDef,
     ChangeMessageVisibilityBatchResultTypeDef,
-    CreateQueueResultTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetQueueAttributesResultTypeDef,
-    GetQueueUrlResultTypeDef,
-    ListDeadLetterSourceQueuesResultTypeDef,
-    ListQueueTagsResultTypeDef,
-    ListQueuesResultTypeDef,
-    SendMessageResultTypeDef,
     DeleteMessageBatchRequestQueueDeleteMessagesTypeDef,
     DeleteMessageBatchRequestRequestTypeDef,
     DeleteMessageBatchResultTypeDef,
-    ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
-    ListQueuesRequestListQueuesPaginateTypeDef,
+    ListMessageMoveTasksResultTypeDef,
     MessageTypeDef,
     SendMessageBatchRequestEntryTypeDef,
     SendMessageRequestQueueSendMessageTypeDef,
     SendMessageRequestRequestTypeDef,
     SendMessageBatchResultTypeDef,
     ReceiveMessageResultTypeDef,
     SendMessageBatchRequestQueueSendMessagesTypeDef,
```

### Comparing `mypy-boto3-sqs-1.26.129/mypy_boto3_sqs/__init__.py` & `mypy-boto3-sqs-1.26.148/mypy_boto3_sqs/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.26.129/mypy_boto3_sqs/__init__.pyi` & `mypy-boto3-sqs-1.26.148/mypy_boto3_sqs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.26.129/mypy_boto3_sqs/__main__.py` & `mypy-boto3-sqs-1.26.148/mypy_boto3_sqs/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SQS 1.26.129\nVersion:         1.26.129\nBuilder version:"
+        "Type annotations for boto3.SQS 1.26.148\nVersion:         1.26.148\nBuilder version:"
         " 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.129")
+    print("1.26.148")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-sqs-1.26.129/mypy_boto3_sqs/client.py` & `mypy-boto3-sqs-1.26.148/mypy_boto3_sqs/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,31 +17,34 @@
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import QueueAttributeFilterType, QueueAttributeNameType
 from .paginator import ListDeadLetterSourceQueuesPaginator, ListQueuesPaginator
 from .type_defs import (
+    CancelMessageMoveTaskResultTypeDef,
     ChangeMessageVisibilityBatchRequestEntryTypeDef,
     ChangeMessageVisibilityBatchResultTypeDef,
     CreateQueueResultTypeDef,
     DeleteMessageBatchRequestEntryTypeDef,
     DeleteMessageBatchResultTypeDef,
     EmptyResponseMetadataTypeDef,
     GetQueueAttributesResultTypeDef,
     GetQueueUrlResultTypeDef,
     ListDeadLetterSourceQueuesResultTypeDef,
+    ListMessageMoveTasksResultTypeDef,
     ListQueuesResultTypeDef,
     ListQueueTagsResultTypeDef,
     MessageAttributeValueTypeDef,
     MessageSystemAttributeValueTypeDef,
     ReceiveMessageResultTypeDef,
     SendMessageBatchRequestEntryTypeDef,
     SendMessageBatchResultTypeDef,
     SendMessageResultTypeDef,
+    StartMessageMoveTaskResultTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -69,14 +72,15 @@
     MessageNotInflight: Type[BotocoreClientError]
     OverLimit: Type[BotocoreClientError]
     PurgeQueueInProgress: Type[BotocoreClientError]
     QueueDeletedRecently: Type[BotocoreClientError]
     QueueDoesNotExist: Type[BotocoreClientError]
     QueueNameExists: Type[BotocoreClientError]
     ReceiptHandleIsInvalid: Type[BotocoreClientError]
+    ResourceNotFoundException: Type[BotocoreClientError]
     TooManyEntriesInBatchRequest: Type[BotocoreClientError]
     UnsupportedOperation: Type[BotocoreClientError]
 
 
 class SQSClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client)
@@ -109,14 +113,22 @@
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#can_paginate)
         """
 
+    def cancel_message_move_task(self, *, TaskHandle: str) -> CancelMessageMoveTaskResultTypeDef:
+        """
+        Cancels a specified message movement task.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.cancel_message_move_task)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#cancel_message_move_task)
+        """
+
     def change_message_visibility(
         self, *, QueueUrl: str, ReceiptHandle: str, VisibilityTimeout: int
     ) -> EmptyResponseMetadataTypeDef:
         """
         Changes the visibility timeout of a specified message in a queue to a new value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.change_message_visibility)
@@ -223,14 +235,25 @@
         Returns a list of your queues that have the `RedrivePolicy` queue attribute
         configured with a dead-letter queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.list_dead_letter_source_queues)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#list_dead_letter_source_queues)
         """
 
+    def list_message_move_tasks(
+        self, *, SourceArn: str, MaxResults: int = ...
+    ) -> ListMessageMoveTasksResultTypeDef:
+        """
+        Gets the most recent message movement tasks (up to 10) under a specific source
+        queue.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.list_message_move_tasks)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#list_message_move_tasks)
+        """
+
     def list_queue_tags(self, *, QueueUrl: str) -> ListQueueTagsResultTypeDef:
         """
         List all cost allocation tags added to the specified Amazon SQS queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.list_queue_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#list_queue_tags)
         """
@@ -300,15 +323,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#send_message)
         """
 
     def send_message_batch(
         self, *, QueueUrl: str, Entries: Sequence[SendMessageBatchRequestEntryTypeDef]
     ) -> SendMessageBatchResultTypeDef:
         """
-        Delivers up to ten messages to the specified queue.
+        You can use `SendMessageBatch` to send up to 10 messages to the specified queue
+        by assigning either identical or different values to each message (or by not
+        assigning values at all).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.send_message_batch)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#send_message_batch)
         """
 
     def set_queue_attributes(
         self, *, QueueUrl: str, Attributes: Mapping[QueueAttributeNameType, str]
@@ -316,14 +341,25 @@
         """
         Sets the value of one or more queue attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.set_queue_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#set_queue_attributes)
         """
 
+    def start_message_move_task(
+        self, *, SourceArn: str, DestinationArn: str = ..., MaxNumberOfMessagesPerSecond: int = ...
+    ) -> StartMessageMoveTaskResultTypeDef:
+        """
+        Starts an asynchronous task to move messages from a specified source queue to a
+        specified destination queue.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.start_message_move_task)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#start_message_move_task)
+        """
+
     def tag_queue(self, *, QueueUrl: str, Tags: Mapping[str, str]) -> EmptyResponseMetadataTypeDef:
         """
         Add cost allocation tags to the specified Amazon SQS queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.tag_queue)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#tag_queue)
         """
```

### Comparing `mypy-boto3-sqs-1.26.129/mypy_boto3_sqs/client.pyi` & `mypy-boto3-sqs-1.26.148/mypy_boto3_sqs/client.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -17,31 +17,34 @@
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import QueueAttributeFilterType, QueueAttributeNameType
 from .paginator import ListDeadLetterSourceQueuesPaginator, ListQueuesPaginator
 from .type_defs import (
+    CancelMessageMoveTaskResultTypeDef,
     ChangeMessageVisibilityBatchRequestEntryTypeDef,
     ChangeMessageVisibilityBatchResultTypeDef,
     CreateQueueResultTypeDef,
     DeleteMessageBatchRequestEntryTypeDef,
     DeleteMessageBatchResultTypeDef,
     EmptyResponseMetadataTypeDef,
     GetQueueAttributesResultTypeDef,
     GetQueueUrlResultTypeDef,
     ListDeadLetterSourceQueuesResultTypeDef,
+    ListMessageMoveTasksResultTypeDef,
     ListQueuesResultTypeDef,
     ListQueueTagsResultTypeDef,
     MessageAttributeValueTypeDef,
     MessageSystemAttributeValueTypeDef,
     ReceiveMessageResultTypeDef,
     SendMessageBatchRequestEntryTypeDef,
     SendMessageBatchResultTypeDef,
     SendMessageResultTypeDef,
+    StartMessageMoveTaskResultTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -66,14 +69,15 @@
     MessageNotInflight: Type[BotocoreClientError]
     OverLimit: Type[BotocoreClientError]
     PurgeQueueInProgress: Type[BotocoreClientError]
     QueueDeletedRecently: Type[BotocoreClientError]
     QueueDoesNotExist: Type[BotocoreClientError]
     QueueNameExists: Type[BotocoreClientError]
     ReceiptHandleIsInvalid: Type[BotocoreClientError]
+    ResourceNotFoundException: Type[BotocoreClientError]
     TooManyEntriesInBatchRequest: Type[BotocoreClientError]
     UnsupportedOperation: Type[BotocoreClientError]
 
 class SQSClient(BaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/)
@@ -102,14 +106,21 @@
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.can_paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#can_paginate)
         """
+    def cancel_message_move_task(self, *, TaskHandle: str) -> CancelMessageMoveTaskResultTypeDef:
+        """
+        Cancels a specified message movement task.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.cancel_message_move_task)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#cancel_message_move_task)
+        """
     def change_message_visibility(
         self, *, QueueUrl: str, ReceiptHandle: str, VisibilityTimeout: int
     ) -> EmptyResponseMetadataTypeDef:
         """
         Changes the visibility timeout of a specified message in a queue to a new value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.change_message_visibility)
@@ -205,14 +216,24 @@
         """
         Returns a list of your queues that have the `RedrivePolicy` queue attribute
         configured with a dead-letter queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.list_dead_letter_source_queues)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#list_dead_letter_source_queues)
         """
+    def list_message_move_tasks(
+        self, *, SourceArn: str, MaxResults: int = ...
+    ) -> ListMessageMoveTasksResultTypeDef:
+        """
+        Gets the most recent message movement tasks (up to 10) under a specific source
+        queue.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.list_message_move_tasks)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#list_message_move_tasks)
+        """
     def list_queue_tags(self, *, QueueUrl: str) -> ListQueueTagsResultTypeDef:
         """
         List all cost allocation tags added to the specified Amazon SQS queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.list_queue_tags)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#list_queue_tags)
         """
@@ -276,28 +297,40 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.send_message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#send_message)
         """
     def send_message_batch(
         self, *, QueueUrl: str, Entries: Sequence[SendMessageBatchRequestEntryTypeDef]
     ) -> SendMessageBatchResultTypeDef:
         """
-        Delivers up to ten messages to the specified queue.
+        You can use `SendMessageBatch` to send up to 10 messages to the specified queue
+        by assigning either identical or different values to each message (or by not
+        assigning values at all).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.send_message_batch)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#send_message_batch)
         """
     def set_queue_attributes(
         self, *, QueueUrl: str, Attributes: Mapping[QueueAttributeNameType, str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Sets the value of one or more queue attributes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.set_queue_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#set_queue_attributes)
         """
+    def start_message_move_task(
+        self, *, SourceArn: str, DestinationArn: str = ..., MaxNumberOfMessagesPerSecond: int = ...
+    ) -> StartMessageMoveTaskResultTypeDef:
+        """
+        Starts an asynchronous task to move messages from a specified source queue to a
+        specified destination queue.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.start_message_move_task)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#start_message_move_task)
+        """
     def tag_queue(self, *, QueueUrl: str, Tags: Mapping[str, str]) -> EmptyResponseMetadataTypeDef:
         """
         Add cost allocation tags to the specified Amazon SQS queue.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Client.tag_queue)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/client/#tag_queue)
         """
```

### Comparing `mypy-boto3-sqs-1.26.129/mypy_boto3_sqs/literals.py` & `mypy-boto3-sqs-1.26.148/mypy_boto3_sqs/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -14,37 +14,36 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ListDeadLetterSourceQueuesPaginatorName",
     "ListQueuesPaginatorName",
     "MessageSystemAttributeNameForSendsType",
     "MessageSystemAttributeNameType",
     "QueueAttributeFilterType",
     "QueueAttributeNameType",
     "SQSServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ListDeadLetterSourceQueuesPaginatorName = Literal["list_dead_letter_source_queues"]
 ListQueuesPaginatorName = Literal["list_queues"]
 MessageSystemAttributeNameForSendsType = Literal["AWSTraceHeader"]
 MessageSystemAttributeNameType = Literal[
     "AWSTraceHeader",
     "ApproximateFirstReceiveTimestamp",
     "ApproximateReceiveCount",
+    "DeadLetterQueueSourceArn",
     "MessageDeduplicationId",
     "MessageGroupId",
     "SenderId",
     "SentTimestamp",
     "SequenceNumber",
 ]
 QueueAttributeFilterType = Literal[
@@ -311,14 +310,15 @@
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
```

### Comparing `mypy-boto3-sqs-1.26.129/mypy_boto3_sqs/literals.pyi` & `mypy-boto3-sqs-1.26.148/mypy_boto3_sqs/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,35 +14,38 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "ListDeadLetterSourceQueuesPaginatorName",
     "ListQueuesPaginatorName",
     "MessageSystemAttributeNameForSendsType",
     "MessageSystemAttributeNameType",
     "QueueAttributeFilterType",
     "QueueAttributeNameType",
     "SQSServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 ListDeadLetterSourceQueuesPaginatorName = Literal["list_dead_letter_source_queues"]
 ListQueuesPaginatorName = Literal["list_queues"]
 MessageSystemAttributeNameForSendsType = Literal["AWSTraceHeader"]
 MessageSystemAttributeNameType = Literal[
     "AWSTraceHeader",
     "ApproximateFirstReceiveTimestamp",
     "ApproximateReceiveCount",
+    "DeadLetterQueueSourceArn",
     "MessageDeduplicationId",
     "MessageGroupId",
     "SenderId",
     "SentTimestamp",
     "SequenceNumber",
 ]
 QueueAttributeFilterType = Literal[
@@ -309,14 +312,15 @@
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
```

### Comparing `mypy-boto3-sqs-1.26.129/mypy_boto3_sqs/paginator.py` & `mypy-boto3-sqs-1.26.148/mypy_boto3_sqs/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,28 +47,28 @@
 class ListDeadLetterSourceQueuesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Paginator.ListDeadLetterSourceQueues)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/paginators/#listdeadlettersourcequeuespaginator)
     """
 
     def paginate(
-        self, *, QueueUrl: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, QueueUrl: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDeadLetterSourceQueuesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Paginator.ListDeadLetterSourceQueues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/paginators/#listdeadlettersourcequeuespaginator)
         """
 
 
 class ListQueuesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Paginator.ListQueues)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/paginators/#listqueuespaginator)
     """
 
     def paginate(
-        self, *, QueueNamePrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, QueueNamePrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListQueuesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Paginator.ListQueues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/paginators/#listqueuespaginator)
         """
```

### Comparing `mypy-boto3-sqs-1.26.129/mypy_boto3_sqs/paginator.pyi` & `mypy-boto3-sqs-1.26.148/mypy_boto3_sqs/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -44,27 +44,27 @@
 class ListDeadLetterSourceQueuesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Paginator.ListDeadLetterSourceQueues)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/paginators/#listdeadlettersourcequeuespaginator)
     """
 
     def paginate(
-        self, *, QueueUrl: str, PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, QueueUrl: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListDeadLetterSourceQueuesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Paginator.ListDeadLetterSourceQueues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/paginators/#listdeadlettersourcequeuespaginator)
         """
 
 class ListQueuesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Paginator.ListQueues)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/paginators/#listqueuespaginator)
     """
 
     def paginate(
-        self, *, QueueNamePrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
+        self, *, QueueNamePrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
     ) -> _PageIterator[ListQueuesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Paginator.ListQueues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/paginators/#listqueuespaginator)
         """
```

### Comparing `mypy-boto3-sqs-1.26.129/mypy_boto3_sqs/service_resource.py` & `mypy-boto3-sqs-1.26.148/mypy_boto3_sqs/service_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -336,15 +336,17 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#queuesend_message-method)
         """
 
     def send_messages(
         self, *, Entries: Sequence[SendMessageBatchRequestEntryTypeDef]
     ) -> SendMessageBatchResultTypeDef:
         """
-        Delivers up to ten messages to the specified queue.
+        You can use `SendMessageBatch` to send up to 10 messages to the specified queue
+        by assigning either identical or different values to each message (or by not
+        assigning values at all).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.send_messages)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#queuesend_messages-method)
         """
 
     def set_attributes(self, *, Attributes: Mapping[QueueAttributeNameType, str]) -> None:
         """
```

### Comparing `mypy-boto3-sqs-1.26.129/mypy_boto3_sqs/service_resource.pyi` & `mypy-boto3-sqs-1.26.148/mypy_boto3_sqs/service_resource.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -305,15 +305,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.send_message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#queuesend_message-method)
         """
     def send_messages(
         self, *, Entries: Sequence[SendMessageBatchRequestEntryTypeDef]
     ) -> SendMessageBatchResultTypeDef:
         """
-        Delivers up to ten messages to the specified queue.
+        You can use `SendMessageBatch` to send up to 10 messages to the specified queue
+        by assigning either identical or different values to each message (or by not
+        assigning values at all).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS.Queue.send_messages)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/service_resource/#queuesend_messages-method)
         """
     def set_attributes(self, *, Attributes: Mapping[QueueAttributeNameType, str]) -> None:
         """
         Sets the value of one or more queue attributes.
```

### Comparing `mypy-boto3-sqs-1.26.129/mypy_boto3_sqs/type_defs.py` & `mypy-boto3-sqs-1.26.148/mypy_boto3_sqs/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,60 +32,67 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AddPermissionRequestQueueAddPermissionTypeDef",
     "AddPermissionRequestRequestTypeDef",
     "BatchResultErrorEntryTypeDef",
+    "CancelMessageMoveTaskRequestRequestTypeDef",
+    "CancelMessageMoveTaskResultTypeDef",
     "ChangeMessageVisibilityBatchRequestEntryTypeDef",
     "ChangeMessageVisibilityBatchResultEntryTypeDef",
-    "ResponseMetadataTypeDef",
     "ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef",
     "ChangeMessageVisibilityRequestRequestTypeDef",
     "CreateQueueRequestRequestTypeDef",
     "CreateQueueRequestServiceResourceCreateQueueTypeDef",
+    "CreateQueueResultTypeDef",
     "DeleteMessageBatchRequestEntryTypeDef",
     "DeleteMessageBatchResultEntryTypeDef",
     "DeleteMessageRequestRequestTypeDef",
     "DeleteQueueRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetQueueAttributesRequestRequestTypeDef",
+    "GetQueueAttributesResultTypeDef",
     "GetQueueUrlRequestRequestTypeDef",
     "GetQueueUrlRequestServiceResourceGetQueueByNameTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetQueueUrlResultTypeDef",
+    "ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
     "ListDeadLetterSourceQueuesRequestRequestTypeDef",
+    "ListDeadLetterSourceQueuesResultTypeDef",
+    "ListMessageMoveTasksRequestRequestTypeDef",
+    "ListMessageMoveTasksResultEntryTypeDef",
     "ListQueueTagsRequestRequestTypeDef",
+    "ListQueueTagsResultTypeDef",
+    "ListQueuesRequestListQueuesPaginateTypeDef",
     "ListQueuesRequestRequestTypeDef",
+    "ListQueuesResultTypeDef",
     "MessageAttributeValueTypeDef",
     "MessageSystemAttributeValueTypeDef",
+    "PaginatorConfigTypeDef",
     "PurgeQueueRequestRequestTypeDef",
     "ReceiveMessageRequestQueueReceiveMessagesTypeDef",
     "ReceiveMessageRequestRequestTypeDef",
     "RemovePermissionRequestQueueRemovePermissionTypeDef",
     "RemovePermissionRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "SendMessageBatchResultEntryTypeDef",
+    "SendMessageResultTypeDef",
     "SetQueueAttributesRequestQueueSetAttributesTypeDef",
     "SetQueueAttributesRequestRequestTypeDef",
+    "StartMessageMoveTaskRequestRequestTypeDef",
+    "StartMessageMoveTaskResultTypeDef",
     "TagQueueRequestRequestTypeDef",
     "UntagQueueRequestRequestTypeDef",
     "ChangeMessageVisibilityBatchRequestQueueChangeMessageVisibilityBatchTypeDef",
     "ChangeMessageVisibilityBatchRequestRequestTypeDef",
     "ChangeMessageVisibilityBatchResultTypeDef",
-    "CreateQueueResultTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetQueueAttributesResultTypeDef",
-    "GetQueueUrlResultTypeDef",
-    "ListDeadLetterSourceQueuesResultTypeDef",
-    "ListQueueTagsResultTypeDef",
-    "ListQueuesResultTypeDef",
-    "SendMessageResultTypeDef",
     "DeleteMessageBatchRequestQueueDeleteMessagesTypeDef",
     "DeleteMessageBatchRequestRequestTypeDef",
     "DeleteMessageBatchResultTypeDef",
-    "ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
-    "ListQueuesRequestListQueuesPaginateTypeDef",
+    "ListMessageMoveTasksResultTypeDef",
     "MessageTypeDef",
     "SendMessageBatchRequestEntryTypeDef",
     "SendMessageRequestQueueSendMessageTypeDef",
     "SendMessageRequestRequestTypeDef",
     "SendMessageBatchResultTypeDef",
     "ReceiveMessageResultTypeDef",
     "SendMessageBatchRequestQueueSendMessagesTypeDef",
@@ -130,14 +137,29 @@
 
 class BatchResultErrorEntryTypeDef(
     _RequiredBatchResultErrorEntryTypeDef, _OptionalBatchResultErrorEntryTypeDef
 ):
     pass
 
 
+CancelMessageMoveTaskRequestRequestTypeDef = TypedDict(
+    "CancelMessageMoveTaskRequestRequestTypeDef",
+    {
+        "TaskHandle": str,
+    },
+)
+
+CancelMessageMoveTaskResultTypeDef = TypedDict(
+    "CancelMessageMoveTaskResultTypeDef",
+    {
+        "ApproximateNumberOfMessagesMoved": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredChangeMessageVisibilityBatchRequestEntryTypeDef = TypedDict(
     "_RequiredChangeMessageVisibilityBatchRequestEntryTypeDef",
     {
         "Id": str,
         "ReceiptHandle": str,
     },
 )
@@ -160,25 +182,14 @@
 ChangeMessageVisibilityBatchResultEntryTypeDef = TypedDict(
     "ChangeMessageVisibilityBatchResultEntryTypeDef",
     {
         "Id": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef = TypedDict(
     "ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef",
     {
         "VisibilityTimeout": int,
     },
 )
 
@@ -232,14 +243,22 @@
 class CreateQueueRequestServiceResourceCreateQueueTypeDef(
     _RequiredCreateQueueRequestServiceResourceCreateQueueTypeDef,
     _OptionalCreateQueueRequestServiceResourceCreateQueueTypeDef,
 ):
     pass
 
 
+CreateQueueResultTypeDef = TypedDict(
+    "CreateQueueResultTypeDef",
+    {
+        "QueueUrl": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteMessageBatchRequestEntryTypeDef = TypedDict(
     "DeleteMessageBatchRequestEntryTypeDef",
     {
         "Id": str,
         "ReceiptHandle": str,
     },
 )
@@ -262,14 +281,21 @@
 DeleteQueueRequestRequestTypeDef = TypedDict(
     "DeleteQueueRequestRequestTypeDef",
     {
         "QueueUrl": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetQueueAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredGetQueueAttributesRequestRequestTypeDef",
     {
         "QueueUrl": str,
     },
 )
 _OptionalGetQueueAttributesRequestRequestTypeDef = TypedDict(
@@ -284,14 +310,22 @@
 class GetQueueAttributesRequestRequestTypeDef(
     _RequiredGetQueueAttributesRequestRequestTypeDef,
     _OptionalGetQueueAttributesRequestRequestTypeDef,
 ):
     pass
 
 
+GetQueueAttributesResultTypeDef = TypedDict(
+    "GetQueueAttributesResultTypeDef",
+    {
+        "Attributes": Dict[QueueAttributeNameType, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetQueueUrlRequestRequestTypeDef = TypedDict(
     "_RequiredGetQueueUrlRequestRequestTypeDef",
     {
         "QueueName": str,
     },
 )
 _OptionalGetQueueUrlRequestRequestTypeDef = TypedDict(
@@ -327,24 +361,44 @@
 class GetQueueUrlRequestServiceResourceGetQueueByNameTypeDef(
     _RequiredGetQueueUrlRequestServiceResourceGetQueueByNameTypeDef,
     _OptionalGetQueueUrlRequestServiceResourceGetQueueByNameTypeDef,
 ):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetQueueUrlResultTypeDef = TypedDict(
+    "GetQueueUrlResultTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "QueueUrl": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef = TypedDict(
+    "_RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
+    {
+        "QueueUrl": str,
+    },
+)
+_OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef = TypedDict(
+    "_OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+
+class ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef(
+    _RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
+    _OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
+):
+    pass
+
+
 _RequiredListDeadLetterSourceQueuesRequestRequestTypeDef = TypedDict(
     "_RequiredListDeadLetterSourceQueuesRequestRequestTypeDef",
     {
         "QueueUrl": str,
     },
 )
 _OptionalListDeadLetterSourceQueuesRequestRequestTypeDef = TypedDict(
@@ -360,31 +414,104 @@
 class ListDeadLetterSourceQueuesRequestRequestTypeDef(
     _RequiredListDeadLetterSourceQueuesRequestRequestTypeDef,
     _OptionalListDeadLetterSourceQueuesRequestRequestTypeDef,
 ):
     pass
 
 
+ListDeadLetterSourceQueuesResultTypeDef = TypedDict(
+    "ListDeadLetterSourceQueuesResultTypeDef",
+    {
+        "queueUrls": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListMessageMoveTasksRequestRequestTypeDef = TypedDict(
+    "_RequiredListMessageMoveTasksRequestRequestTypeDef",
+    {
+        "SourceArn": str,
+    },
+)
+_OptionalListMessageMoveTasksRequestRequestTypeDef = TypedDict(
+    "_OptionalListMessageMoveTasksRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+
+class ListMessageMoveTasksRequestRequestTypeDef(
+    _RequiredListMessageMoveTasksRequestRequestTypeDef,
+    _OptionalListMessageMoveTasksRequestRequestTypeDef,
+):
+    pass
+
+
+ListMessageMoveTasksResultEntryTypeDef = TypedDict(
+    "ListMessageMoveTasksResultEntryTypeDef",
+    {
+        "TaskHandle": str,
+        "Status": str,
+        "SourceArn": str,
+        "DestinationArn": str,
+        "MaxNumberOfMessagesPerSecond": int,
+        "ApproximateNumberOfMessagesMoved": int,
+        "ApproximateNumberOfMessagesToMove": int,
+        "FailureReason": str,
+        "StartedTimestamp": int,
+    },
+    total=False,
+)
+
 ListQueueTagsRequestRequestTypeDef = TypedDict(
     "ListQueueTagsRequestRequestTypeDef",
     {
         "QueueUrl": str,
     },
 )
 
+ListQueueTagsResultTypeDef = TypedDict(
+    "ListQueueTagsResultTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListQueuesRequestListQueuesPaginateTypeDef = TypedDict(
+    "ListQueuesRequestListQueuesPaginateTypeDef",
+    {
+        "QueueNamePrefix": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListQueuesRequestRequestTypeDef = TypedDict(
     "ListQueuesRequestRequestTypeDef",
     {
         "QueueNamePrefix": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListQueuesResultTypeDef = TypedDict(
+    "ListQueuesResultTypeDef",
+    {
+        "QueueUrls": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredMessageAttributeValueTypeDef = TypedDict(
     "_RequiredMessageAttributeValueTypeDef",
     {
         "DataType": str,
     },
 )
 _OptionalMessageAttributeValueTypeDef = TypedDict(
@@ -425,14 +552,24 @@
 
 class MessageSystemAttributeValueTypeDef(
     _RequiredMessageSystemAttributeValueTypeDef, _OptionalMessageSystemAttributeValueTypeDef
 ):
     pass
 
 
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
 PurgeQueueRequestRequestTypeDef = TypedDict(
     "PurgeQueueRequestRequestTypeDef",
     {
         "QueueUrl": str,
     },
 )
 
@@ -486,14 +623,25 @@
     "RemovePermissionRequestRequestTypeDef",
     {
         "QueueUrl": str,
         "Label": str,
     },
 )
 
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
 _RequiredSendMessageBatchResultEntryTypeDef = TypedDict(
     "_RequiredSendMessageBatchResultEntryTypeDef",
     {
         "Id": str,
         "MessageId": str,
         "MD5OfMessageBody": str,
     },
@@ -511,14 +659,26 @@
 
 class SendMessageBatchResultEntryTypeDef(
     _RequiredSendMessageBatchResultEntryTypeDef, _OptionalSendMessageBatchResultEntryTypeDef
 ):
     pass
 
 
+SendMessageResultTypeDef = TypedDict(
+    "SendMessageResultTypeDef",
+    {
+        "MD5OfMessageBody": str,
+        "MD5OfMessageAttributes": str,
+        "MD5OfMessageSystemAttributes": str,
+        "MessageId": str,
+        "SequenceNumber": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SetQueueAttributesRequestQueueSetAttributesTypeDef = TypedDict(
     "SetQueueAttributesRequestQueueSetAttributesTypeDef",
     {
         "Attributes": Mapping[QueueAttributeNameType, str],
     },
 )
 
@@ -526,14 +686,45 @@
     "SetQueueAttributesRequestRequestTypeDef",
     {
         "QueueUrl": str,
         "Attributes": Mapping[QueueAttributeNameType, str],
     },
 )
 
+_RequiredStartMessageMoveTaskRequestRequestTypeDef = TypedDict(
+    "_RequiredStartMessageMoveTaskRequestRequestTypeDef",
+    {
+        "SourceArn": str,
+    },
+)
+_OptionalStartMessageMoveTaskRequestRequestTypeDef = TypedDict(
+    "_OptionalStartMessageMoveTaskRequestRequestTypeDef",
+    {
+        "DestinationArn": str,
+        "MaxNumberOfMessagesPerSecond": int,
+    },
+    total=False,
+)
+
+
+class StartMessageMoveTaskRequestRequestTypeDef(
+    _RequiredStartMessageMoveTaskRequestRequestTypeDef,
+    _OptionalStartMessageMoveTaskRequestRequestTypeDef,
+):
+    pass
+
+
+StartMessageMoveTaskResultTypeDef = TypedDict(
+    "StartMessageMoveTaskResultTypeDef",
+    {
+        "TaskHandle": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TagQueueRequestRequestTypeDef = TypedDict(
     "TagQueueRequestRequestTypeDef",
     {
         "QueueUrl": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -562,84 +753,15 @@
 )
 
 ChangeMessageVisibilityBatchResultTypeDef = TypedDict(
     "ChangeMessageVisibilityBatchResultTypeDef",
     {
         "Successful": List[ChangeMessageVisibilityBatchResultEntryTypeDef],
         "Failed": List[BatchResultErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateQueueResultTypeDef = TypedDict(
-    "CreateQueueResultTypeDef",
-    {
-        "QueueUrl": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetQueueAttributesResultTypeDef = TypedDict(
-    "GetQueueAttributesResultTypeDef",
-    {
-        "Attributes": Dict[QueueAttributeNameType, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetQueueUrlResultTypeDef = TypedDict(
-    "GetQueueUrlResultTypeDef",
-    {
-        "QueueUrl": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDeadLetterSourceQueuesResultTypeDef = TypedDict(
-    "ListDeadLetterSourceQueuesResultTypeDef",
-    {
-        "queueUrls": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListQueueTagsResultTypeDef = TypedDict(
-    "ListQueueTagsResultTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListQueuesResultTypeDef = TypedDict(
-    "ListQueuesResultTypeDef",
-    {
-        "QueueUrls": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SendMessageResultTypeDef = TypedDict(
-    "SendMessageResultTypeDef",
-    {
-        "MD5OfMessageBody": str,
-        "MD5OfMessageAttributes": str,
-        "MD5OfMessageSystemAttributes": str,
-        "MessageId": str,
-        "SequenceNumber": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteMessageBatchRequestQueueDeleteMessagesTypeDef = TypedDict(
     "DeleteMessageBatchRequestQueueDeleteMessagesTypeDef",
     {
         "Entries": Sequence[DeleteMessageBatchRequestEntryTypeDef],
@@ -655,47 +777,24 @@
 )
 
 DeleteMessageBatchResultTypeDef = TypedDict(
     "DeleteMessageBatchResultTypeDef",
     {
         "Successful": List[DeleteMessageBatchResultEntryTypeDef],
         "Failed": List[BatchResultErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef = TypedDict(
-    "_RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
-    {
-        "QueueUrl": str,
-    },
-)
-_OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef = TypedDict(
-    "_OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
-
-class ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef(
-    _RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
-    _OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
-):
-    pass
-
-
-ListQueuesRequestListQueuesPaginateTypeDef = TypedDict(
-    "ListQueuesRequestListQueuesPaginateTypeDef",
+ListMessageMoveTasksResultTypeDef = TypedDict(
+    "ListMessageMoveTasksResultTypeDef",
     {
-        "QueueNamePrefix": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
+        "Results": List[ListMessageMoveTasksResultEntryTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
-    total=False,
 )
 
 MessageTypeDef = TypedDict(
     "MessageTypeDef",
     {
         "MessageId": str,
         "ReceiptHandle": str,
@@ -793,23 +892,23 @@
 
 
 SendMessageBatchResultTypeDef = TypedDict(
     "SendMessageBatchResultTypeDef",
     {
         "Successful": List[SendMessageBatchResultEntryTypeDef],
         "Failed": List[BatchResultErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReceiveMessageResultTypeDef = TypedDict(
     "ReceiveMessageResultTypeDef",
     {
         "Messages": List[MessageTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SendMessageBatchRequestQueueSendMessagesTypeDef = TypedDict(
     "SendMessageBatchRequestQueueSendMessagesTypeDef",
     {
         "Entries": Sequence[SendMessageBatchRequestEntryTypeDef],
```

### Comparing `mypy-boto3-sqs-1.26.129/mypy_boto3_sqs/type_defs.pyi` & `mypy-boto3-sqs-1.26.148/mypy_boto3_sqs/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -31,60 +31,67 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AddPermissionRequestQueueAddPermissionTypeDef",
     "AddPermissionRequestRequestTypeDef",
     "BatchResultErrorEntryTypeDef",
+    "CancelMessageMoveTaskRequestRequestTypeDef",
+    "CancelMessageMoveTaskResultTypeDef",
     "ChangeMessageVisibilityBatchRequestEntryTypeDef",
     "ChangeMessageVisibilityBatchResultEntryTypeDef",
-    "ResponseMetadataTypeDef",
     "ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef",
     "ChangeMessageVisibilityRequestRequestTypeDef",
     "CreateQueueRequestRequestTypeDef",
     "CreateQueueRequestServiceResourceCreateQueueTypeDef",
+    "CreateQueueResultTypeDef",
     "DeleteMessageBatchRequestEntryTypeDef",
     "DeleteMessageBatchResultEntryTypeDef",
     "DeleteMessageRequestRequestTypeDef",
     "DeleteQueueRequestRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetQueueAttributesRequestRequestTypeDef",
+    "GetQueueAttributesResultTypeDef",
     "GetQueueUrlRequestRequestTypeDef",
     "GetQueueUrlRequestServiceResourceGetQueueByNameTypeDef",
-    "PaginatorConfigTypeDef",
+    "GetQueueUrlResultTypeDef",
+    "ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
     "ListDeadLetterSourceQueuesRequestRequestTypeDef",
+    "ListDeadLetterSourceQueuesResultTypeDef",
+    "ListMessageMoveTasksRequestRequestTypeDef",
+    "ListMessageMoveTasksResultEntryTypeDef",
     "ListQueueTagsRequestRequestTypeDef",
+    "ListQueueTagsResultTypeDef",
+    "ListQueuesRequestListQueuesPaginateTypeDef",
     "ListQueuesRequestRequestTypeDef",
+    "ListQueuesResultTypeDef",
     "MessageAttributeValueTypeDef",
     "MessageSystemAttributeValueTypeDef",
+    "PaginatorConfigTypeDef",
     "PurgeQueueRequestRequestTypeDef",
     "ReceiveMessageRequestQueueReceiveMessagesTypeDef",
     "ReceiveMessageRequestRequestTypeDef",
     "RemovePermissionRequestQueueRemovePermissionTypeDef",
     "RemovePermissionRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "SendMessageBatchResultEntryTypeDef",
+    "SendMessageResultTypeDef",
     "SetQueueAttributesRequestQueueSetAttributesTypeDef",
     "SetQueueAttributesRequestRequestTypeDef",
+    "StartMessageMoveTaskRequestRequestTypeDef",
+    "StartMessageMoveTaskResultTypeDef",
     "TagQueueRequestRequestTypeDef",
     "UntagQueueRequestRequestTypeDef",
     "ChangeMessageVisibilityBatchRequestQueueChangeMessageVisibilityBatchTypeDef",
     "ChangeMessageVisibilityBatchRequestRequestTypeDef",
     "ChangeMessageVisibilityBatchResultTypeDef",
-    "CreateQueueResultTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetQueueAttributesResultTypeDef",
-    "GetQueueUrlResultTypeDef",
-    "ListDeadLetterSourceQueuesResultTypeDef",
-    "ListQueueTagsResultTypeDef",
-    "ListQueuesResultTypeDef",
-    "SendMessageResultTypeDef",
     "DeleteMessageBatchRequestQueueDeleteMessagesTypeDef",
     "DeleteMessageBatchRequestRequestTypeDef",
     "DeleteMessageBatchResultTypeDef",
-    "ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
-    "ListQueuesRequestListQueuesPaginateTypeDef",
+    "ListMessageMoveTasksResultTypeDef",
     "MessageTypeDef",
     "SendMessageBatchRequestEntryTypeDef",
     "SendMessageRequestQueueSendMessageTypeDef",
     "SendMessageRequestRequestTypeDef",
     "SendMessageBatchResultTypeDef",
     "ReceiveMessageResultTypeDef",
     "SendMessageBatchRequestQueueSendMessagesTypeDef",
@@ -127,14 +134,29 @@
 )
 
 class BatchResultErrorEntryTypeDef(
     _RequiredBatchResultErrorEntryTypeDef, _OptionalBatchResultErrorEntryTypeDef
 ):
     pass
 
+CancelMessageMoveTaskRequestRequestTypeDef = TypedDict(
+    "CancelMessageMoveTaskRequestRequestTypeDef",
+    {
+        "TaskHandle": str,
+    },
+)
+
+CancelMessageMoveTaskResultTypeDef = TypedDict(
+    "CancelMessageMoveTaskResultTypeDef",
+    {
+        "ApproximateNumberOfMessagesMoved": int,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredChangeMessageVisibilityBatchRequestEntryTypeDef = TypedDict(
     "_RequiredChangeMessageVisibilityBatchRequestEntryTypeDef",
     {
         "Id": str,
         "ReceiptHandle": str,
     },
 )
@@ -155,25 +177,14 @@
 ChangeMessageVisibilityBatchResultEntryTypeDef = TypedDict(
     "ChangeMessageVisibilityBatchResultEntryTypeDef",
     {
         "Id": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef = TypedDict(
     "ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef",
     {
         "VisibilityTimeout": int,
     },
 )
 
@@ -223,14 +234,22 @@
 
 class CreateQueueRequestServiceResourceCreateQueueTypeDef(
     _RequiredCreateQueueRequestServiceResourceCreateQueueTypeDef,
     _OptionalCreateQueueRequestServiceResourceCreateQueueTypeDef,
 ):
     pass
 
+CreateQueueResultTypeDef = TypedDict(
+    "CreateQueueResultTypeDef",
+    {
+        "QueueUrl": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 DeleteMessageBatchRequestEntryTypeDef = TypedDict(
     "DeleteMessageBatchRequestEntryTypeDef",
     {
         "Id": str,
         "ReceiptHandle": str,
     },
 )
@@ -253,14 +272,21 @@
 DeleteQueueRequestRequestTypeDef = TypedDict(
     "DeleteQueueRequestRequestTypeDef",
     {
         "QueueUrl": str,
     },
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetQueueAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredGetQueueAttributesRequestRequestTypeDef",
     {
         "QueueUrl": str,
     },
 )
 _OptionalGetQueueAttributesRequestRequestTypeDef = TypedDict(
@@ -273,14 +299,22 @@
 
 class GetQueueAttributesRequestRequestTypeDef(
     _RequiredGetQueueAttributesRequestRequestTypeDef,
     _OptionalGetQueueAttributesRequestRequestTypeDef,
 ):
     pass
 
+GetQueueAttributesResultTypeDef = TypedDict(
+    "GetQueueAttributesResultTypeDef",
+    {
+        "Attributes": Dict[QueueAttributeNameType, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredGetQueueUrlRequestRequestTypeDef = TypedDict(
     "_RequiredGetQueueUrlRequestRequestTypeDef",
     {
         "QueueName": str,
     },
 )
 _OptionalGetQueueUrlRequestRequestTypeDef = TypedDict(
@@ -312,24 +346,42 @@
 
 class GetQueueUrlRequestServiceResourceGetQueueByNameTypeDef(
     _RequiredGetQueueUrlRequestServiceResourceGetQueueByNameTypeDef,
     _OptionalGetQueueUrlRequestServiceResourceGetQueueByNameTypeDef,
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetQueueUrlResultTypeDef = TypedDict(
+    "GetQueueUrlResultTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "QueueUrl": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef = TypedDict(
+    "_RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
+    {
+        "QueueUrl": str,
+    },
+)
+_OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef = TypedDict(
+    "_OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
+    {
+        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+class ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef(
+    _RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
+    _OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
+):
+    pass
+
 _RequiredListDeadLetterSourceQueuesRequestRequestTypeDef = TypedDict(
     "_RequiredListDeadLetterSourceQueuesRequestRequestTypeDef",
     {
         "QueueUrl": str,
     },
 )
 _OptionalListDeadLetterSourceQueuesRequestRequestTypeDef = TypedDict(
@@ -343,31 +395,102 @@
 
 class ListDeadLetterSourceQueuesRequestRequestTypeDef(
     _RequiredListDeadLetterSourceQueuesRequestRequestTypeDef,
     _OptionalListDeadLetterSourceQueuesRequestRequestTypeDef,
 ):
     pass
 
+ListDeadLetterSourceQueuesResultTypeDef = TypedDict(
+    "ListDeadLetterSourceQueuesResultTypeDef",
+    {
+        "queueUrls": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+_RequiredListMessageMoveTasksRequestRequestTypeDef = TypedDict(
+    "_RequiredListMessageMoveTasksRequestRequestTypeDef",
+    {
+        "SourceArn": str,
+    },
+)
+_OptionalListMessageMoveTasksRequestRequestTypeDef = TypedDict(
+    "_OptionalListMessageMoveTasksRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+class ListMessageMoveTasksRequestRequestTypeDef(
+    _RequiredListMessageMoveTasksRequestRequestTypeDef,
+    _OptionalListMessageMoveTasksRequestRequestTypeDef,
+):
+    pass
+
+ListMessageMoveTasksResultEntryTypeDef = TypedDict(
+    "ListMessageMoveTasksResultEntryTypeDef",
+    {
+        "TaskHandle": str,
+        "Status": str,
+        "SourceArn": str,
+        "DestinationArn": str,
+        "MaxNumberOfMessagesPerSecond": int,
+        "ApproximateNumberOfMessagesMoved": int,
+        "ApproximateNumberOfMessagesToMove": int,
+        "FailureReason": str,
+        "StartedTimestamp": int,
+    },
+    total=False,
+)
+
 ListQueueTagsRequestRequestTypeDef = TypedDict(
     "ListQueueTagsRequestRequestTypeDef",
     {
         "QueueUrl": str,
     },
 )
 
+ListQueueTagsResultTypeDef = TypedDict(
+    "ListQueueTagsResultTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
+ListQueuesRequestListQueuesPaginateTypeDef = TypedDict(
+    "ListQueuesRequestListQueuesPaginateTypeDef",
+    {
+        "QueueNamePrefix": str,
+        "PaginationConfig": "PaginatorConfigTypeDef",
+    },
+    total=False,
+)
+
 ListQueuesRequestRequestTypeDef = TypedDict(
     "ListQueuesRequestRequestTypeDef",
     {
         "QueueNamePrefix": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+ListQueuesResultTypeDef = TypedDict(
+    "ListQueuesResultTypeDef",
+    {
+        "QueueUrls": List[str],
+        "NextToken": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 _RequiredMessageAttributeValueTypeDef = TypedDict(
     "_RequiredMessageAttributeValueTypeDef",
     {
         "DataType": str,
     },
 )
 _OptionalMessageAttributeValueTypeDef = TypedDict(
@@ -404,14 +527,24 @@
 )
 
 class MessageSystemAttributeValueTypeDef(
     _RequiredMessageSystemAttributeValueTypeDef, _OptionalMessageSystemAttributeValueTypeDef
 ):
     pass
 
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
 PurgeQueueRequestRequestTypeDef = TypedDict(
     "PurgeQueueRequestRequestTypeDef",
     {
         "QueueUrl": str,
     },
 )
 
@@ -463,14 +596,25 @@
     "RemovePermissionRequestRequestTypeDef",
     {
         "QueueUrl": str,
         "Label": str,
     },
 )
 
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
 _RequiredSendMessageBatchResultEntryTypeDef = TypedDict(
     "_RequiredSendMessageBatchResultEntryTypeDef",
     {
         "Id": str,
         "MessageId": str,
         "MD5OfMessageBody": str,
     },
@@ -486,14 +630,26 @@
 )
 
 class SendMessageBatchResultEntryTypeDef(
     _RequiredSendMessageBatchResultEntryTypeDef, _OptionalSendMessageBatchResultEntryTypeDef
 ):
     pass
 
+SendMessageResultTypeDef = TypedDict(
+    "SendMessageResultTypeDef",
+    {
+        "MD5OfMessageBody": str,
+        "MD5OfMessageAttributes": str,
+        "MD5OfMessageSystemAttributes": str,
+        "MessageId": str,
+        "SequenceNumber": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 SetQueueAttributesRequestQueueSetAttributesTypeDef = TypedDict(
     "SetQueueAttributesRequestQueueSetAttributesTypeDef",
     {
         "Attributes": Mapping[QueueAttributeNameType, str],
     },
 )
 
@@ -501,14 +657,43 @@
     "SetQueueAttributesRequestRequestTypeDef",
     {
         "QueueUrl": str,
         "Attributes": Mapping[QueueAttributeNameType, str],
     },
 )
 
+_RequiredStartMessageMoveTaskRequestRequestTypeDef = TypedDict(
+    "_RequiredStartMessageMoveTaskRequestRequestTypeDef",
+    {
+        "SourceArn": str,
+    },
+)
+_OptionalStartMessageMoveTaskRequestRequestTypeDef = TypedDict(
+    "_OptionalStartMessageMoveTaskRequestRequestTypeDef",
+    {
+        "DestinationArn": str,
+        "MaxNumberOfMessagesPerSecond": int,
+    },
+    total=False,
+)
+
+class StartMessageMoveTaskRequestRequestTypeDef(
+    _RequiredStartMessageMoveTaskRequestRequestTypeDef,
+    _OptionalStartMessageMoveTaskRequestRequestTypeDef,
+):
+    pass
+
+StartMessageMoveTaskResultTypeDef = TypedDict(
+    "StartMessageMoveTaskResultTypeDef",
+    {
+        "TaskHandle": str,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
+    },
+)
+
 TagQueueRequestRequestTypeDef = TypedDict(
     "TagQueueRequestRequestTypeDef",
     {
         "QueueUrl": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -537,84 +722,15 @@
 )
 
 ChangeMessageVisibilityBatchResultTypeDef = TypedDict(
     "ChangeMessageVisibilityBatchResultTypeDef",
     {
         "Successful": List[ChangeMessageVisibilityBatchResultEntryTypeDef],
         "Failed": List[BatchResultErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CreateQueueResultTypeDef = TypedDict(
-    "CreateQueueResultTypeDef",
-    {
-        "QueueUrl": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetQueueAttributesResultTypeDef = TypedDict(
-    "GetQueueAttributesResultTypeDef",
-    {
-        "Attributes": Dict[QueueAttributeNameType, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetQueueUrlResultTypeDef = TypedDict(
-    "GetQueueUrlResultTypeDef",
-    {
-        "QueueUrl": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListDeadLetterSourceQueuesResultTypeDef = TypedDict(
-    "ListDeadLetterSourceQueuesResultTypeDef",
-    {
-        "queueUrls": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListQueueTagsResultTypeDef = TypedDict(
-    "ListQueueTagsResultTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListQueuesResultTypeDef = TypedDict(
-    "ListQueuesResultTypeDef",
-    {
-        "QueueUrls": List[str],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SendMessageResultTypeDef = TypedDict(
-    "SendMessageResultTypeDef",
-    {
-        "MD5OfMessageBody": str,
-        "MD5OfMessageAttributes": str,
-        "MD5OfMessageSystemAttributes": str,
-        "MessageId": str,
-        "SequenceNumber": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 DeleteMessageBatchRequestQueueDeleteMessagesTypeDef = TypedDict(
     "DeleteMessageBatchRequestQueueDeleteMessagesTypeDef",
     {
         "Entries": Sequence[DeleteMessageBatchRequestEntryTypeDef],
@@ -630,46 +746,25 @@
 )
 
 DeleteMessageBatchResultTypeDef = TypedDict(
     "DeleteMessageBatchResultTypeDef",
     {
         "Successful": List[DeleteMessageBatchResultEntryTypeDef],
         "Failed": List[BatchResultErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
-_RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef = TypedDict(
-    "_RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
+ListMessageMoveTasksResultTypeDef = TypedDict(
+    "ListMessageMoveTasksResultTypeDef",
     {
-        "QueueUrl": str,
+        "Results": List[ListMessageMoveTasksResultEntryTypeDef],
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
-_OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef = TypedDict(
-    "_OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef",
-    {
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
-
-class ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef(
-    _RequiredListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
-    _OptionalListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
-):
-    pass
-
-ListQueuesRequestListQueuesPaginateTypeDef = TypedDict(
-    "ListQueuesRequestListQueuesPaginateTypeDef",
-    {
-        "QueueNamePrefix": str,
-        "PaginationConfig": PaginatorConfigTypeDef,
-    },
-    total=False,
-)
 
 MessageTypeDef = TypedDict(
     "MessageTypeDef",
     {
         "MessageId": str,
         "ReceiptHandle": str,
         "MD5OfBody": str,
@@ -760,23 +855,23 @@
     pass
 
 SendMessageBatchResultTypeDef = TypedDict(
     "SendMessageBatchResultTypeDef",
     {
         "Successful": List[SendMessageBatchResultEntryTypeDef],
         "Failed": List[BatchResultErrorEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 ReceiveMessageResultTypeDef = TypedDict(
     "ReceiveMessageResultTypeDef",
     {
         "Messages": List[MessageTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
 )
 
 SendMessageBatchRequestQueueSendMessagesTypeDef = TypedDict(
     "SendMessageBatchRequestQueueSendMessagesTypeDef",
     {
         "Entries": Sequence[SendMessageBatchRequestEntryTypeDef],
```

### Comparing `mypy-boto3-sqs-1.26.129/mypy_boto3_sqs.egg-info/PKG-INFO` & `mypy-boto3-sqs-1.26.148/mypy_boto3_sqs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-sqs
-Version: 1.26.129
-Summary: Type annotations for boto3.SQS 1.26.129 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.148
+Summary: Type annotations for boto3.SQS 1.26.148 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-sqs.svg?color=blue)](https://pypi.org/project/mypy-boto3-sqs)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_sqs/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-sqs?color=blue)](https://pypistats.org/packages/mypy-boto3-sqs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SQS 1.26.129](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
+[boto3.SQS 1.26.148](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sqs.html#SQS)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -415,60 +415,67 @@
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_sqs.type_defs import (
     AddPermissionRequestQueueAddPermissionTypeDef,
     AddPermissionRequestRequestTypeDef,
     BatchResultErrorEntryTypeDef,
+    CancelMessageMoveTaskRequestRequestTypeDef,
+    CancelMessageMoveTaskResultTypeDef,
     ChangeMessageVisibilityBatchRequestEntryTypeDef,
     ChangeMessageVisibilityBatchResultEntryTypeDef,
-    ResponseMetadataTypeDef,
     ChangeMessageVisibilityRequestMessageChangeVisibilityTypeDef,
     ChangeMessageVisibilityRequestRequestTypeDef,
     CreateQueueRequestRequestTypeDef,
     CreateQueueRequestServiceResourceCreateQueueTypeDef,
+    CreateQueueResultTypeDef,
     DeleteMessageBatchRequestEntryTypeDef,
     DeleteMessageBatchResultEntryTypeDef,
     DeleteMessageRequestRequestTypeDef,
     DeleteQueueRequestRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetQueueAttributesRequestRequestTypeDef,
+    GetQueueAttributesResultTypeDef,
     GetQueueUrlRequestRequestTypeDef,
     GetQueueUrlRequestServiceResourceGetQueueByNameTypeDef,
-    PaginatorConfigTypeDef,
+    GetQueueUrlResultTypeDef,
+    ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
     ListDeadLetterSourceQueuesRequestRequestTypeDef,
+    ListDeadLetterSourceQueuesResultTypeDef,
+    ListMessageMoveTasksRequestRequestTypeDef,
+    ListMessageMoveTasksResultEntryTypeDef,
     ListQueueTagsRequestRequestTypeDef,
+    ListQueueTagsResultTypeDef,
+    ListQueuesRequestListQueuesPaginateTypeDef,
     ListQueuesRequestRequestTypeDef,
+    ListQueuesResultTypeDef,
     MessageAttributeValueTypeDef,
     MessageSystemAttributeValueTypeDef,
+    PaginatorConfigTypeDef,
     PurgeQueueRequestRequestTypeDef,
     ReceiveMessageRequestQueueReceiveMessagesTypeDef,
     ReceiveMessageRequestRequestTypeDef,
     RemovePermissionRequestQueueRemovePermissionTypeDef,
     RemovePermissionRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     SendMessageBatchResultEntryTypeDef,
+    SendMessageResultTypeDef,
     SetQueueAttributesRequestQueueSetAttributesTypeDef,
     SetQueueAttributesRequestRequestTypeDef,
+    StartMessageMoveTaskRequestRequestTypeDef,
+    StartMessageMoveTaskResultTypeDef,
     TagQueueRequestRequestTypeDef,
     UntagQueueRequestRequestTypeDef,
     ChangeMessageVisibilityBatchRequestQueueChangeMessageVisibilityBatchTypeDef,
     ChangeMessageVisibilityBatchRequestRequestTypeDef,
     ChangeMessageVisibilityBatchResultTypeDef,
-    CreateQueueResultTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetQueueAttributesResultTypeDef,
-    GetQueueUrlResultTypeDef,
-    ListDeadLetterSourceQueuesResultTypeDef,
-    ListQueueTagsResultTypeDef,
-    ListQueuesResultTypeDef,
-    SendMessageResultTypeDef,
     DeleteMessageBatchRequestQueueDeleteMessagesTypeDef,
     DeleteMessageBatchRequestRequestTypeDef,
     DeleteMessageBatchResultTypeDef,
-    ListDeadLetterSourceQueuesRequestListDeadLetterSourceQueuesPaginateTypeDef,
-    ListQueuesRequestListQueuesPaginateTypeDef,
+    ListMessageMoveTasksResultTypeDef,
     MessageTypeDef,
     SendMessageBatchRequestEntryTypeDef,
     SendMessageRequestQueueSendMessageTypeDef,
     SendMessageRequestRequestTypeDef,
     SendMessageBatchResultTypeDef,
     ReceiveMessageResultTypeDef,
     SendMessageBatchRequestQueueSendMessagesTypeDef,
```

### Comparing `mypy-boto3-sqs-1.26.129/mypy_boto3_sqs.egg-info/SOURCES.txt` & `mypy-boto3-sqs-1.26.148/mypy_boto3_sqs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-sqs-1.26.129/setup.py` & `mypy-boto3-sqs-1.26.148/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-sqs",
-    version="1.26.129",
+    version="1.26.148",
     packages=["mypy_boto3_sqs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SQS 1.26.129 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.SQS 1.26.148 service generated with mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

