# Comparing `tmp/vnpy_xex-2023.6.6.1.tar.gz` & `tmp/vnpy_xex-2023.6.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnpy_xex-2023.6.6.1.tar", last modified: Tue Jun  6 01:58:47 2023, max compression
+gzip compressed data, was "vnpy_xex-2023.6.6.2.tar", last modified: Tue Jun  6 08:00:50 2023, max compression
```

## Comparing `vnpy_xex-2023.6.6.1.tar` & `vnpy_xex-2023.6.6.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-06-06 01:58:47.812948 vnpy_xex-2023.6.6.1/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1065 2023-05-26 07:16:27.000000 vnpy_xex-2023.6.6.1/LICENSE
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1007 2023-06-06 01:58:47.813038 vnpy_xex-2023.6.6.1/PKG-INFO
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       80 2023-05-30 10:14:13.000000 vnpy_xex-2023.6.6.1/README.md
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)      993 2023-06-06 01:58:47.813491 vnpy_xex-2023.6.6.1/setup.cfg
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       39 2023-05-26 07:26:45.000000 vnpy_xex-2023.6.6.1/setup.py
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-06-06 01:58:47.810556 vnpy_xex-2023.6.6.1/vnpy_xex/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)      583 2023-05-26 07:16:27.000000 vnpy_xex-2023.6.6.1/vnpy_xex/__init__.py
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)    24550 2023-06-06 01:44:41.000000 vnpy_xex-2023.6.6.1/vnpy_xex/xex_gateway.py
-drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-06-06 01:58:47.812749 vnpy_xex-2023.6.6.1/vnpy_xex.egg-info/
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1007 2023-06-06 01:58:47.000000 vnpy_xex-2023.6.6.1/vnpy_xex.egg-info/PKG-INFO
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)      271 2023-06-06 01:58:47.000000 vnpy_xex-2023.6.6.1/vnpy_xex.egg-info/SOURCES.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-06-06 01:58:47.000000 vnpy_xex-2023.6.6.1/vnpy_xex.egg-info/dependency_links.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-05-30 10:16:02.000000 vnpy_xex-2023.6.6.1/vnpy_xex.egg-info/not-zip-safe
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)       46 2023-06-06 01:58:47.000000 vnpy_xex-2023.6.6.1/vnpy_xex.egg-info/requires.txt
--rw-r--r--   0 90houlaoheshang   (501) staff       (20)        9 2023-06-06 01:58:47.000000 vnpy_xex-2023.6.6.1/vnpy_xex.egg-info/top_level.txt
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-06-06 08:00:50.249199 vnpy_xex-2023.6.6.2/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1065 2023-05-26 07:16:27.000000 vnpy_xex-2023.6.6.2/LICENSE
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1007 2023-06-06 08:00:50.249340 vnpy_xex-2023.6.6.2/PKG-INFO
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       80 2023-05-30 10:14:13.000000 vnpy_xex-2023.6.6.2/README.md
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)      993 2023-06-06 08:00:50.250317 vnpy_xex-2023.6.6.2/setup.cfg
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       39 2023-05-26 07:26:45.000000 vnpy_xex-2023.6.6.2/setup.py
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-06-06 08:00:50.243752 vnpy_xex-2023.6.6.2/vnpy_xex/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)      583 2023-05-26 07:16:27.000000 vnpy_xex-2023.6.6.2/vnpy_xex/__init__.py
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)    24586 2023-06-06 07:59:02.000000 vnpy_xex-2023.6.6.2/vnpy_xex/xex_gateway.py
+drwxr-xr-x   0 90houlaoheshang   (501) staff       (20)        0 2023-06-06 08:00:50.248906 vnpy_xex-2023.6.6.2/vnpy_xex.egg-info/
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)     1007 2023-06-06 08:00:50.000000 vnpy_xex-2023.6.6.2/vnpy_xex.egg-info/PKG-INFO
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)      271 2023-06-06 08:00:50.000000 vnpy_xex-2023.6.6.2/vnpy_xex.egg-info/SOURCES.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-06-06 08:00:50.000000 vnpy_xex-2023.6.6.2/vnpy_xex.egg-info/dependency_links.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)        1 2023-05-30 10:16:02.000000 vnpy_xex-2023.6.6.2/vnpy_xex.egg-info/not-zip-safe
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)       46 2023-06-06 08:00:50.000000 vnpy_xex-2023.6.6.2/vnpy_xex.egg-info/requires.txt
+-rw-r--r--   0 90houlaoheshang   (501) staff       (20)        9 2023-06-06 08:00:50.000000 vnpy_xex-2023.6.6.2/vnpy_xex.egg-info/top_level.txt
```

### Comparing `vnpy_xex-2023.6.6.1/LICENSE` & `vnpy_xex-2023.6.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vnpy_xex-2023.6.6.1/PKG-INFO` & `vnpy_xex-2023.6.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy_xex
-Version: 2023.6.6.1
+Version: 2023.6.6.2
 Summary: gateway of xex exchange for vnpy
 Home-page: https://github.com/monk-after-90s/vnpy_xex
 Author: antas
 Author-email: 907333918@qq.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `vnpy_xex-2023.6.6.1/setup.cfg` & `vnpy_xex-2023.6.6.2/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = vnpy_xex
-version = 2023.6.6.1
+version = 2023.6.6.2
 url = https://github.com/monk-after-90s/vnpy_xex
 license = MIT
 author = antas
 author_email = 907333918@qq.com
 description = gateway of xex exchange for vnpy
 long_description = file: README.md
 long_description_content_type = text/markdown
```

### Comparing `vnpy_xex-2023.6.6.1/vnpy_xex/__init__.py` & `vnpy_xex-2023.6.6.2/vnpy_xex/__init__.py`

 * *Files identical despite different names*

### Comparing `vnpy_xex-2023.6.6.1/vnpy_xex/xex_gateway.py` & `vnpy_xex-2023.6.6.2/vnpy_xex/xex_gateway.py`

 * *Files 1% similar despite different names*

```diff
@@ -679,15 +679,15 @@
         )
         setattr(order, "origin_orderId", data['orderId'])
 
         order_last_snapshot = self.gateway.get_order(orderid)
 
         self.gateway.on_order(order)
         # 计算trade
-        if order.traded > order_last_snapshot.traded:
+        if order_last_snapshot is not None and order.traded > order_last_snapshot.traded:
             trade_volume = order.traded - order_last_snapshot.traded
             contract: ContractData = symbol_contract_map.get(order.symbol, None)
             if contract:
                 trade_volume = round_to(trade_volume, contract.min_volume)
 
             if not trade_volume:
                 return
```

### Comparing `vnpy_xex-2023.6.6.1/vnpy_xex.egg-info/PKG-INFO` & `vnpy_xex-2023.6.6.2/vnpy_xex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy-xex
-Version: 2023.6.6.1
+Version: 2023.6.6.2
 Summary: gateway of xex exchange for vnpy
 Home-page: https://github.com/monk-after-90s/vnpy_xex
 Author: antas
 Author-email: 907333918@qq.com
 License: MIT
 Keywords: quant,quantitative,investment,trading,algotrading
 Classifier: Development Status :: 5 - Production/Stable
```

