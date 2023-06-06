# Comparing `tmp/vnpy_xex-2023.6.5.1.tar.gz` & `tmp/vnpy_xex-2023.6.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnpy_xex-2023.6.5.1.tar", last modified: Mon Jun  5 10:03:45 2023, max compression
+gzip compressed data, was "vnpy_xex-2023.6.6.1.tar", last modified: Tue Jun  6 01:58:47 2023, max compression
```

## Comparing `vnpy_xex-2023.6.5.1.tar` & `vnpy_xex-2023.6.6.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-06-05 10:03:45.676872 vnpy_xex-2023.6.5.1/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1065 2023-05-26 07:16:27.000000 vnpy_xex-2023.6.5.1/LICENSE
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1007 2023-06-05 10:03:45.676976 vnpy_xex-2023.6.5.1/PKG-INFO
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       80 2023-05-30 10:14:13.000000 vnpy_xex-2023.6.5.1/README.md
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)      994 2023-06-05 10:03:45.677477 vnpy_xex-2023.6.5.1/setup.cfg
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       39 2023-05-26 07:26:45.000000 vnpy_xex-2023.6.5.1/setup.py
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-06-05 10:03:45.673759 vnpy_xex-2023.6.5.1/vnpy_xex/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)      583 2023-05-26 07:16:27.000000 vnpy_xex-2023.6.5.1/vnpy_xex/__init__.py
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)    23960 2023-06-05 10:02:35.000000 vnpy_xex-2023.6.5.1/vnpy_xex/xex_gateway.py
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-06-05 10:03:45.676659 vnpy_xex-2023.6.5.1/vnpy_xex.egg-info/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1007 2023-06-05 10:03:45.000000 vnpy_xex-2023.6.5.1/vnpy_xex.egg-info/PKG-INFO
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)      271 2023-06-05 10:03:45.000000 vnpy_xex-2023.6.5.1/vnpy_xex.egg-info/SOURCES.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-06-05 10:03:45.000000 vnpy_xex-2023.6.5.1/vnpy_xex.egg-info/dependency_links.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-05-30 10:16:02.000000 vnpy_xex-2023.6.5.1/vnpy_xex.egg-info/not-zip-safe
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       46 2023-06-05 10:03:45.000000 vnpy_xex-2023.6.5.1/vnpy_xex.egg-info/requires.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)        9 2023-06-05 10:03:45.000000 vnpy_xex-2023.6.5.1/vnpy_xex.egg-info/top_level.txt
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-06-06 01:58:47.812948 vnpy_xex-2023.6.6.1/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1065 2023-05-26 07:16:27.000000 vnpy_xex-2023.6.6.1/LICENSE
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1007 2023-06-06 01:58:47.813038 vnpy_xex-2023.6.6.1/PKG-INFO
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       80 2023-05-30 10:14:13.000000 vnpy_xex-2023.6.6.1/README.md
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)      993 2023-06-06 01:58:47.813491 vnpy_xex-2023.6.6.1/setup.cfg
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       39 2023-05-26 07:26:45.000000 vnpy_xex-2023.6.6.1/setup.py
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-06-06 01:58:47.810556 vnpy_xex-2023.6.6.1/vnpy_xex/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)      583 2023-05-26 07:16:27.000000 vnpy_xex-2023.6.6.1/vnpy_xex/__init__.py
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)    24550 2023-06-06 01:44:41.000000 vnpy_xex-2023.6.6.1/vnpy_xex/xex_gateway.py
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-06-06 01:58:47.812749 vnpy_xex-2023.6.6.1/vnpy_xex.egg-info/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1007 2023-06-06 01:58:47.000000 vnpy_xex-2023.6.6.1/vnpy_xex.egg-info/PKG-INFO
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)      271 2023-06-06 01:58:47.000000 vnpy_xex-2023.6.6.1/vnpy_xex.egg-info/SOURCES.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-06-06 01:58:47.000000 vnpy_xex-2023.6.6.1/vnpy_xex.egg-info/dependency_links.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-05-30 10:16:02.000000 vnpy_xex-2023.6.6.1/vnpy_xex.egg-info/not-zip-safe
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       46 2023-06-06 01:58:47.000000 vnpy_xex-2023.6.6.1/vnpy_xex.egg-info/requires.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)        9 2023-06-06 01:58:47.000000 vnpy_xex-2023.6.6.1/vnpy_xex.egg-info/top_level.txt
```

### Comparing `vnpy_xex-2023.6.5.1/LICENSE` & `vnpy_xex-2023.6.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vnpy_xex-2023.6.5.1/PKG-INFO` & `vnpy_xex-2023.6.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy_xex
-Version: 2023.6.5.1
+Version: 2023.6.6.1
 Summary: gateway of xex exchange for vnpy
 Home-page: https://github.com/monk-after-90s/vnpy_xex
 Author: antas
 Author-email: 907333918@qq.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `vnpy_xex-2023.6.5.1/setup.cfg` & `vnpy_xex-2023.6.6.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vnpy_xex
-version = 2023.6.05.1
+version = 2023.6.6.1
 url = https://github.com/monk-after-90s/vnpy_xex
 license = MIT
 author = antas
 author_email = 907333918@qq.com
 description = gateway of xex exchange for vnpy
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `vnpy_xex-2023.6.5.1/vnpy_xex/__init__.py` & `vnpy_xex-2023.6.6.1/vnpy_xex/__init__.py`

 * *Files identical despite different names*

### Comparing `vnpy_xex-2023.6.5.1/vnpy_xex/xex_gateway.py` & `vnpy_xex-2023.6.6.1/vnpy_xex/xex_gateway.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import json
 import time
 from asyncio import run_coroutine_threadsafe
 from copy import copy
 from datetime import datetime, timedelta
 from enum import Enum
 from threading import Lock
+import beeprint
+from loguru import logger
 from vnpy_websocket import WebsocketClient
 import pytz
 from typing import Any, Dict, List
 from requests.exceptions import SSLError
 from vnpy.trader.constant import (
     Direction,
     Exchange,
@@ -470,29 +472,36 @@
                     symbol_contract_map[contract.symbol] = contract
 
             self.gateway.write_log("合约信息查询成功")
             self.query_order()
 
     def on_send_order(self, data: dict, request: Request) -> None:
         """委托下单回报"""
-        pass
+        logger.debug(
+            f"on_send_order data={beeprint.pp(data, output=False, sort_keys=False)} {request.path=} request.params={beeprint.pp(request.params, output=False, sort_keys=False)}")
 
     def on_send_order_failed(self, status_code: str, request: Request) -> None:
         """委托下单失败服务器报错回报"""
+        logger.debug(
+            f"on_send_order_failed {status_code=} {request.path=} request.params={beeprint.pp(request.params, output=False, sort_keys=False)}")
+
         order: OrderData = request.extra
         order.status = Status.REJECTED
         self.gateway.on_order(order)
 
         msg: str = f"委托失败，状态码：{status_code}，信息：{request.response.text}"
         self.gateway.write_log(msg)
 
     def on_send_order_error(
             self, exception_type: type, exception_value: Exception, tb, request: Request
     ) -> None:
         """委托下单回报函数报错回报"""
+        logger.debug(
+            f"on_send_order_error {exception_type=} {exception_value=} {tb=} {request.path=} request.params={beeprint.pp(request.params, output=False, sort_keys=False)}")
+
         order: OrderData = request.extra
         order.status = Status.REJECTED
         self.gateway.on_order(order)
 
         if not issubclass(exception_type, (ConnectionError, SSLError)):
             self.on_error(exception_type, exception_value, tb, request)
```

### Comparing `vnpy_xex-2023.6.5.1/vnpy_xex.egg-info/PKG-INFO` & `vnpy_xex-2023.6.6.1/vnpy_xex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy-xex
-Version: 2023.6.5.1
+Version: 2023.6.6.1
 Summary: gateway of xex exchange for vnpy
 Home-page: https://github.com/monk-after-90s/vnpy_xex
 Author: antas
 Author-email: 907333918@qq.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Classifier: Development Status :: 5 - Production/Stable
```

