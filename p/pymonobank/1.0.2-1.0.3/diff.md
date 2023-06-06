# Comparing `tmp/pymonobank-1.0.2.tar.gz` & `tmp/pymonobank-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymonobank-1.0.2.tar", max compression
+gzip compressed data, was "pymonobank-1.0.3.tar", max compression
```

## Comparing `pymonobank-1.0.2.tar` & `pymonobank-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       85 2023-06-06 17:54:51.686637 pymonobank-1.0.2/README.md
--rw-r--r--   0        0        0        0 2023-06-06 18:14:14.104875 pymonobank-1.0.2/pymonobank/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 19:52:55.238124 pymonobank-1.0.2/pymonobank/core/__init__.py
--rw-r--r--   0        0        0     3766 2023-06-06 13:44:04.662926 pymonobank-1.0.2/pymonobank/core/api.py
--rw-r--r--   0        0        0       56 2023-06-05 20:33:24.324334 pymonobank-1.0.2/pymonobank/core/invoice/__init__.py
--rw-r--r--   0        0        0     1195 2023-06-06 13:38:48.747785 pymonobank-1.0.2/pymonobank/core/invoice/invoice.py
--rw-r--r--   0        0        0      670 2023-06-05 20:55:54.452138 pymonobank-1.0.2/pymonobank/core/invoice/schemas.py
--rw-r--r--   0        0        0       24 2023-06-05 20:53:41.469690 pymonobank-1.0.2/pymonobank/core/merchant/__init__.py
--rw-r--r--   0        0        0      497 2023-06-06 13:38:48.741119 pymonobank-1.0.2/pymonobank/core/merchant/merchant.py
--rw-r--r--   0        0        0       61 2023-06-05 19:57:10.270516 pymonobank-1.0.2/pymonobank/request/__init__.py
--rw-r--r--   0        0        0      115 2023-06-05 20:19:08.704472 pymonobank-1.0.2/pymonobank/request/exceptions.py
--rw-r--r--   0        0        0      284 2023-06-05 19:57:10.263849 pymonobank-1.0.2/pymonobank/request/methods.py
--rw-r--r--   0        0        0       32 2023-06-05 20:06:43.357645 pymonobank-1.0.2/pymonobank/schemas/__init__.py
--rw-r--r--   0        0        0      143 2023-06-05 20:06:43.364311 pymonobank-1.0.2/pymonobank/schemas/base.py
--rw-r--r--   0        0        0        0 2023-06-05 20:20:54.611108 pymonobank-1.0.2/pymonobank/utils/__init__.py
--rw-r--r--   0        0        0      121 2023-06-05 20:28:53.212483 pymonobank-1.0.2/pymonobank/utils/currencies/__init__.py
--rw-r--r--   0        0        0      397 2023-06-06 18:53:23.724566 pymonobank-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      677 1970-01-01 00:00:00.000000 pymonobank-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0       85 2023-06-06 17:54:51.686637 pymonobank-1.0.3/README.md
+-rw-r--r--   0        0        0      242 2023-06-06 18:57:40.436318 pymonobank-1.0.3/pymonobank/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 19:52:55.238124 pymonobank-1.0.3/pymonobank/core/__init__.py
+-rw-r--r--   0        0        0     3772 2023-06-06 18:57:40.426319 pymonobank-1.0.3/pymonobank/core/api.py
+-rw-r--r--   0        0        0       56 2023-06-05 20:33:24.324334 pymonobank-1.0.3/pymonobank/core/invoice/__init__.py
+-rw-r--r--   0        0        0     1207 2023-06-06 18:57:40.432985 pymonobank-1.0.3/pymonobank/core/invoice/invoice.py
+-rw-r--r--   0        0        0      682 2023-06-06 18:57:40.449651 pymonobank-1.0.3/pymonobank/core/invoice/schemas.py
+-rw-r--r--   0        0        0       24 2023-06-05 20:53:41.469690 pymonobank-1.0.3/pymonobank/core/merchant/__init__.py
+-rw-r--r--   0        0        0      509 2023-06-06 18:57:40.446318 pymonobank-1.0.3/pymonobank/core/merchant/merchant.py
+-rw-r--r--   0        0        0       61 2023-06-05 19:57:10.270516 pymonobank-1.0.3/pymonobank/request/__init__.py
+-rw-r--r--   0        0        0      115 2023-06-05 20:19:08.704472 pymonobank-1.0.3/pymonobank/request/exceptions.py
+-rw-r--r--   0        0        0      284 2023-06-05 19:57:10.263849 pymonobank-1.0.3/pymonobank/request/methods.py
+-rw-r--r--   0        0        0       32 2023-06-05 20:06:43.357645 pymonobank-1.0.3/pymonobank/schemas/__init__.py
+-rw-r--r--   0        0        0      143 2023-06-05 20:06:43.364311 pymonobank-1.0.3/pymonobank/schemas/base.py
+-rw-r--r--   0        0        0        0 2023-06-05 20:20:54.611108 pymonobank-1.0.3/pymonobank/utils/__init__.py
+-rw-r--r--   0        0        0      121 2023-06-05 20:28:53.212483 pymonobank-1.0.3/pymonobank/utils/currencies/__init__.py
+-rw-r--r--   0        0        0      397 2023-06-06 18:57:46.242663 pymonobank-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      677 1970-01-01 00:00:00.000000 pymonobank-1.0.3/PKG-INFO
```

### Comparing `pymonobank-1.0.2/pymonobank/core/api.py` & `pymonobank-1.0.3/pymonobank/core/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import requests
 
-from mono.request import RequestPOST, RequestGET, exceptions
+from pymonobank.request import RequestPOST, RequestGET, exceptions
 
 
 class MonoApi(object):
     BASE_URL = 'https://api.monobank.ua'
     AUTH_HEADER = 'X-Token'
     TOKEN = None
```

### Comparing `pymonobank-1.0.2/pymonobank/core/invoice/invoice.py` & `pymonobank-1.0.3/pymonobank/core/invoice/invoice.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import requests
 
-from mono.core.api import MonoApi
-from mono.request import RequestMethods
+from pymonobank.core.api import MonoApi
+from pymonobank.request import RequestMethods
 
 from .schemas import InvoiceData, StatusInvoiceData
 
 
 class MonoInvoice(MonoApi):
     CREATE = MonoApi.BASE_URL + '/api/merchant/invoice/create'
     STATUS = MonoApi.BASE_URL + '/api/merchant/invoice/status'
```

### Comparing `pymonobank-1.0.2/pymonobank/core/invoice/schemas.py` & `pymonobank-1.0.3/pymonobank/core/invoice/schemas.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from dataclasses import dataclass
 
-from mono.schemas import BaseDataclass
-from mono.utils.currencies import Currencies
+from pymonobank.schemas import BaseDataclass
+from pymonobank.utils.currencies import Currencies
 
 
 __all__ = (
     'InvoiceData',
     'StatusInvoiceData'
 )
```

### Comparing `pymonobank-1.0.2/PKG-INFO` & `pymonobank-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymonobank
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python client for Monobank API
 Author: Alex Stulen
 Author-email: ookno16@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

