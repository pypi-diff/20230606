# Comparing `tmp/plutous_trade_crypto-0.0.8.tar.gz` & `tmp/plutous_trade_crypto-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plutous_trade_crypto-0.0.8.tar", max compression
+gzip compressed data, was "plutous_trade_crypto-0.0.9.tar", max compression
```

## Comparing `plutous_trade_crypto-0.0.8.tar` & `plutous_trade_crypto-0.0.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1064 2023-01-08 12:06:02.705678 plutous_trade_crypto-0.0.8/LICENSE
--rw-r--r--   0        0        0       54 2023-01-08 12:06:02.705678 plutous_trade_crypto-0.0.8/README.md
--rw-r--r--   0        0        0       65 2023-01-08 12:06:02.705678 plutous_trade_crypto-0.0.8/plutous/__init__.py
--rw-r--r--   0        0        0       65 2023-01-08 12:06:02.705678 plutous_trade_crypto-0.0.8/plutous/trade/__init__.py
--rw-r--r--   0        0        0       21 2023-05-22 19:28:53.283994 plutous_trade_crypto-0.0.8/plutous/trade/crypto/__init__.py
--rw-r--r--   0        0        0     3379 2023-05-10 12:56:23.847802 plutous_trade_crypto-0.0.8/plutous/trade/crypto/alembic.ini
--rw-r--r--   0        0        0        0 2023-05-13 03:22:38.353244 plutous_trade_crypto-0.0.8/plutous/trade/crypto/app/__init__.py
--rw-r--r--   0        0        0      622 2023-05-22 19:25:55.670914 plutous_trade_crypto-0.0.8/plutous/trade/crypto/app/main.py
--rw-r--r--   0        0        0      140 2023-05-22 19:22:06.212847 plutous_trade_crypto-0.0.8/plutous/trade/crypto/app/models.py
--rw-r--r--   0        0        0        0 2023-05-12 08:22:34.782657 plutous_trade_crypto-0.0.8/plutous/trade/crypto/cli/__init__.py
--rw-r--r--   0        0        0      574 2023-05-22 16:04:38.509464 plutous_trade_crypto-0.0.8/plutous/trade/crypto/cli/database.py
--rw-r--r--   0        0        0      135 2023-05-16 09:06:32.409428 plutous_trade_crypto-0.0.8/plutous/trade/crypto/cli/main.py
--rw-r--r--   0        0        0      216 2023-05-10 18:19:43.739470 plutous_trade_crypto-0.0.8/plutous/trade/crypto/collectors/__init__.py
--rw-r--r--   0        0        0      513 2023-05-10 18:40:29.490637 plutous_trade_crypto-0.0.8/plutous/trade/crypto/collectors/base.py
--rw-r--r--   0        0        0      172 2023-05-10 18:41:14.018182 plutous_trade_crypto-0.0.8/plutous/trade/crypto/collectors/funding_rate.py
--rw-r--r--   0        0        0       88 2023-05-10 17:34:01.381163 plutous_trade_crypto-0.0.8/plutous/trade/crypto/collectors/long_short_ratio.py
--rw-r--r--   0        0        0       79 2023-05-10 18:19:43.739470 plutous_trade_crypto-0.0.8/plutous/trade/crypto/collectors/ohlcv.py
--rw-r--r--   0        0        0       86 2023-05-10 17:34:30.463478 plutous_trade_crypto-0.0.8/plutous/trade/crypto/collectors/open_interest.py
--rw-r--r--   0        0        0        0 2023-05-21 17:19:36.941622 plutous_trade_crypto-0.0.8/plutous/trade/crypto/commands/__init__.py
--rw-r--r--   0        0        0        0 2023-05-21 17:20:01.916024 plutous_trade_crypto-0.0.8/plutous/trade/crypto/commands/base.py
--rw-r--r--   0        0        0     4326 2023-05-22 19:25:40.949498 plutous_trade_crypto-0.0.8/plutous/trade/crypto/commands/bot.py
--rw-r--r--   0        0        0       98 2023-05-10 17:43:41.343327 plutous_trade_crypto-0.0.8/plutous/trade/crypto/config.py
--rw-r--r--   0        0        0       65 2023-05-12 10:17:35.407061 plutous_trade_crypto-0.0.8/plutous/trade/crypto/enums/__init__.py
--rw-r--r--   0        0        0      514 2023-05-22 16:14:44.239714 plutous_trade_crypto-0.0.8/plutous/trade/crypto/enums/exchange.py
--rw-r--r--   0        0        0       89 2023-05-21 17:27:13.801556 plutous_trade_crypto-0.0.8/plutous/trade/crypto/enums/order_type.py
--rw-r--r--   0        0        0      545 2023-01-13 12:53:06.868724 plutous_trade_crypto-0.0.8/plutous/trade/crypto/exchanges/__init__.py
--rw-r--r--   0        0        0    26099 2023-05-13 03:11:36.363085 plutous_trade_crypto-0.0.8/plutous/trade/crypto/exchanges/binance.py
--rw-r--r--   0        0        0     6758 2023-02-09 01:38:34.931606 plutous_trade_crypto-0.0.8/plutous/trade/crypto/exchanges/bitget.py
--rw-r--r--   0        0        0     9056 2023-01-24 17:08:43.291912 plutous_trade_crypto-0.0.8/plutous/trade/crypto/exchanges/bybit.py
--rw-r--r--   0        0        0      243 2023-01-18 17:49:03.301016 plutous_trade_crypto-0.0.8/plutous/trade/crypto/exchanges/coinex.py
--rw-r--r--   0        0        0     3432 2023-01-08 12:06:02.705678 plutous_trade_crypto-0.0.8/plutous/trade/crypto/exchanges/gateio.py
--rw-r--r--   0        0        0     5479 2023-01-08 12:06:02.705678 plutous_trade_crypto-0.0.8/plutous/trade/crypto/exchanges/huobi.py
--rw-r--r--   0        0        0     2402 2023-01-13 23:16:12.206570 plutous_trade_crypto-0.0.8/plutous/trade/crypto/exchanges/kucoin.py
--rw-r--r--   0        0        0     7009 2023-01-08 12:06:02.705678 plutous_trade_crypto-0.0.8/plutous/trade/crypto/exchanges/mexc.py
--rw-r--r--   0        0        0     5762 2023-03-05 16:41:45.182876 plutous_trade_crypto-0.0.8/plutous/trade/crypto/exchanges/okx.py
--rw-r--r--   0        0        0     2482 2023-01-08 12:06:02.705678 plutous_trade_crypto-0.0.8/plutous/trade/crypto/exchanges/phemex.py
--rw-r--r--   0        0        0       51 2023-01-13 23:17:03.314313 plutous_trade_crypto-0.0.8/plutous/trade/crypto/exchanges/woo.py
--rw-r--r--   0        0        0       38 2023-05-10 12:56:23.851803 plutous_trade_crypto-0.0.8/plutous/trade/crypto/migrations/README
--rw-r--r--   0        0        0     2135 2023-05-10 18:07:49.326597 plutous_trade_crypto-0.0.8/plutous/trade/crypto/migrations/env.py
--rw-r--r--   0        0        0      510 2023-05-10 12:56:23.847802 plutous_trade_crypto-0.0.8/plutous/trade/crypto/migrations/script.py.mako
--rw-r--r--   0        0        0      170 2023-05-16 12:54:41.106899 plutous_trade_crypto-0.0.8/plutous/trade/crypto/models/__init__.py
--rw-r--r--   0        0        0      899 2023-05-22 16:26:55.117999 plutous_trade_crypto-0.0.8/plutous/trade/crypto/models/base.py
--rw-r--r--   0        0        0      118 2023-05-16 12:52:34.126691 plutous_trade_crypto-0.0.8/plutous/trade/crypto/models/funding_rate.py
--rw-r--r--   0        0        0      189 2023-05-16 12:52:45.027739 plutous_trade_crypto-0.0.8/plutous/trade/crypto/models/long_short_ratio.py
--rw-r--r--   0        0        0      304 2023-05-16 12:52:54.744674 plutous_trade_crypto-0.0.8/plutous/trade/crypto/models/ohlcv.py
--rw-r--r--   0        0        0      119 2023-05-16 12:53:05.037663 plutous_trade_crypto-0.0.8/plutous/trade/crypto/models/open_interest.py
--rw-r--r--   0        0        0        0 2023-05-13 03:12:04.505389 plutous_trade_crypto-0.0.8/plutous/trade/crypto/utils/__init__.py
--rw-r--r--   0        0        0        0 2023-05-13 03:16:16.838039 plutous_trade_crypto-0.0.8/plutous/trade/crypto/utils/limit_chaser.py
--rw-r--r--   0        0        0     4492 2023-05-13 03:11:05.296543 plutous_trade_crypto-0.0.8/plutous/trade/crypto/utils/paginate.py
--rw-r--r--   0        0        0      618 2023-05-22 19:28:59.228566 plutous_trade_crypto-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      640 1970-01-01 00:00:00.000000 plutous_trade_crypto-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-01-08 12:06:02.705678 plutous_trade_crypto-0.0.9/LICENSE
+-rw-r--r--   0        0        0       54 2023-01-08 12:06:02.705678 plutous_trade_crypto-0.0.9/README.md
+-rw-r--r--   0        0        0       65 2023-01-08 12:06:02.705678 plutous_trade_crypto-0.0.9/plutous/__init__.py
+-rw-r--r--   0        0        0       65 2023-01-08 12:06:02.705678 plutous_trade_crypto-0.0.9/plutous/trade/__init__.py
+-rw-r--r--   0        0        0       21 2023-05-22 19:44:47.331743 plutous_trade_crypto-0.0.9/plutous/trade/crypto/__init__.py
+-rw-r--r--   0        0        0     3379 2023-05-10 12:56:23.847802 plutous_trade_crypto-0.0.9/plutous/trade/crypto/alembic.ini
+-rw-r--r--   0        0        0        0 2023-05-13 03:22:38.353244 plutous_trade_crypto-0.0.9/plutous/trade/crypto/app/__init__.py
+-rw-r--r--   0        0        0      622 2023-05-22 19:25:55.670914 plutous_trade_crypto-0.0.9/plutous/trade/crypto/app/main.py
+-rw-r--r--   0        0        0      140 2023-05-22 19:22:06.212847 plutous_trade_crypto-0.0.9/plutous/trade/crypto/app/models.py
+-rw-r--r--   0        0        0        0 2023-05-12 08:22:34.782657 plutous_trade_crypto-0.0.9/plutous/trade/crypto/cli/__init__.py
+-rw-r--r--   0        0        0      574 2023-05-22 16:04:38.509464 plutous_trade_crypto-0.0.9/plutous/trade/crypto/cli/database.py
+-rw-r--r--   0        0        0      135 2023-05-16 09:06:32.409428 plutous_trade_crypto-0.0.9/plutous/trade/crypto/cli/main.py
+-rw-r--r--   0        0        0      216 2023-05-10 18:19:43.739470 plutous_trade_crypto-0.0.9/plutous/trade/crypto/collectors/__init__.py
+-rw-r--r--   0        0        0      513 2023-05-10 18:40:29.490637 plutous_trade_crypto-0.0.9/plutous/trade/crypto/collectors/base.py
+-rw-r--r--   0        0        0      172 2023-05-10 18:41:14.018182 plutous_trade_crypto-0.0.9/plutous/trade/crypto/collectors/funding_rate.py
+-rw-r--r--   0        0        0       88 2023-05-10 17:34:01.381163 plutous_trade_crypto-0.0.9/plutous/trade/crypto/collectors/long_short_ratio.py
+-rw-r--r--   0        0        0       79 2023-05-10 18:19:43.739470 plutous_trade_crypto-0.0.9/plutous/trade/crypto/collectors/ohlcv.py
+-rw-r--r--   0        0        0       86 2023-05-10 17:34:30.463478 plutous_trade_crypto-0.0.9/plutous/trade/crypto/collectors/open_interest.py
+-rw-r--r--   0        0        0        0 2023-05-21 17:19:36.941622 plutous_trade_crypto-0.0.9/plutous/trade/crypto/commands/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-21 17:20:01.916024 plutous_trade_crypto-0.0.9/plutous/trade/crypto/commands/base.py
+-rw-r--r--   0        0        0     4296 2023-05-22 19:40:12.745337 plutous_trade_crypto-0.0.9/plutous/trade/crypto/commands/bot.py
+-rw-r--r--   0        0        0       98 2023-05-10 17:43:41.343327 plutous_trade_crypto-0.0.9/plutous/trade/crypto/config.py
+-rw-r--r--   0        0        0       65 2023-05-12 10:17:35.407061 plutous_trade_crypto-0.0.9/plutous/trade/crypto/enums/__init__.py
+-rw-r--r--   0        0        0      514 2023-05-22 16:14:44.239714 plutous_trade_crypto-0.0.9/plutous/trade/crypto/enums/exchange.py
+-rw-r--r--   0        0        0       89 2023-05-21 17:27:13.801556 plutous_trade_crypto-0.0.9/plutous/trade/crypto/enums/order_type.py
+-rw-r--r--   0        0        0      545 2023-01-13 12:53:06.868724 plutous_trade_crypto-0.0.9/plutous/trade/crypto/exchanges/__init__.py
+-rw-r--r--   0        0        0    26099 2023-05-13 03:11:36.363085 plutous_trade_crypto-0.0.9/plutous/trade/crypto/exchanges/binance.py
+-rw-r--r--   0        0        0     6758 2023-02-09 01:38:34.931606 plutous_trade_crypto-0.0.9/plutous/trade/crypto/exchanges/bitget.py
+-rw-r--r--   0        0        0     9056 2023-01-24 17:08:43.291912 plutous_trade_crypto-0.0.9/plutous/trade/crypto/exchanges/bybit.py
+-rw-r--r--   0        0        0      243 2023-01-18 17:49:03.301016 plutous_trade_crypto-0.0.9/plutous/trade/crypto/exchanges/coinex.py
+-rw-r--r--   0        0        0     3432 2023-01-08 12:06:02.705678 plutous_trade_crypto-0.0.9/plutous/trade/crypto/exchanges/gateio.py
+-rw-r--r--   0        0        0     5479 2023-01-08 12:06:02.705678 plutous_trade_crypto-0.0.9/plutous/trade/crypto/exchanges/huobi.py
+-rw-r--r--   0        0        0     2402 2023-01-13 23:16:12.206570 plutous_trade_crypto-0.0.9/plutous/trade/crypto/exchanges/kucoin.py
+-rw-r--r--   0        0        0     7009 2023-01-08 12:06:02.705678 plutous_trade_crypto-0.0.9/plutous/trade/crypto/exchanges/mexc.py
+-rw-r--r--   0        0        0     5762 2023-03-05 16:41:45.182876 plutous_trade_crypto-0.0.9/plutous/trade/crypto/exchanges/okx.py
+-rw-r--r--   0        0        0     2482 2023-01-08 12:06:02.705678 plutous_trade_crypto-0.0.9/plutous/trade/crypto/exchanges/phemex.py
+-rw-r--r--   0        0        0       51 2023-01-13 23:17:03.314313 plutous_trade_crypto-0.0.9/plutous/trade/crypto/exchanges/woo.py
+-rw-r--r--   0        0        0       38 2023-05-10 12:56:23.851803 plutous_trade_crypto-0.0.9/plutous/trade/crypto/migrations/README
+-rw-r--r--   0        0        0     2135 2023-05-10 18:07:49.326597 plutous_trade_crypto-0.0.9/plutous/trade/crypto/migrations/env.py
+-rw-r--r--   0        0        0      510 2023-05-10 12:56:23.847802 plutous_trade_crypto-0.0.9/plutous/trade/crypto/migrations/script.py.mako
+-rw-r--r--   0        0        0      170 2023-05-16 12:54:41.106899 plutous_trade_crypto-0.0.9/plutous/trade/crypto/models/__init__.py
+-rw-r--r--   0        0        0      899 2023-05-22 16:26:55.117999 plutous_trade_crypto-0.0.9/plutous/trade/crypto/models/base.py
+-rw-r--r--   0        0        0      118 2023-05-16 12:52:34.126691 plutous_trade_crypto-0.0.9/plutous/trade/crypto/models/funding_rate.py
+-rw-r--r--   0        0        0      189 2023-05-16 12:52:45.027739 plutous_trade_crypto-0.0.9/plutous/trade/crypto/models/long_short_ratio.py
+-rw-r--r--   0        0        0      304 2023-05-16 12:52:54.744674 plutous_trade_crypto-0.0.9/plutous/trade/crypto/models/ohlcv.py
+-rw-r--r--   0        0        0      119 2023-05-16 12:53:05.037663 plutous_trade_crypto-0.0.9/plutous/trade/crypto/models/open_interest.py
+-rw-r--r--   0        0        0        0 2023-05-13 03:12:04.505389 plutous_trade_crypto-0.0.9/plutous/trade/crypto/utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-13 03:16:16.838039 plutous_trade_crypto-0.0.9/plutous/trade/crypto/utils/limit_chaser.py
+-rw-r--r--   0        0        0     4492 2023-05-13 03:11:05.296543 plutous_trade_crypto-0.0.9/plutous/trade/crypto/utils/paginate.py
+-rw-r--r--   0        0        0      618 2023-05-22 19:44:36.954745 plutous_trade_crypto-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      640 1970-01-01 00:00:00.000000 plutous_trade_crypto-0.0.9/PKG-INFO
```

### Comparing `plutous_trade_crypto-0.0.8/LICENSE` & `plutous_trade_crypto-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `plutous_trade_crypto-0.0.8/plutous/trade/crypto/alembic.ini` & `plutous_trade_crypto-0.0.9/plutous/trade/crypto/alembic.ini`

 * *Files identical despite different names*

### Comparing `plutous_trade_crypto-0.0.8/plutous/trade/crypto/app/main.py` & `plutous_trade_crypto-0.0.9/plutous/trade/crypto/app/main.py`

 * *Files identical despite different names*

### Comparing `plutous_trade_crypto-0.0.8/plutous/trade/crypto/cli/database.py` & `plutous_trade_crypto-0.0.9/plutous/trade/crypto/cli/database.py`

 * *Files identical despite different names*

### Comparing `plutous_trade_crypto-0.0.8/plutous/trade/crypto/collectors/base.py` & `plutous_trade_crypto-0.0.9/plutous/trade/crypto/collectors/base.py`

 * *Files identical despite different names*

### Comparing `plutous_trade_crypto-0.0.8/plutous/trade/crypto/commands/bot.py` & `plutous_trade_crypto-0.0.9/plutous/trade/crypto/commands/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from datetime import datetime
 from typing import Any
 
 from pydantic import BaseModel
 from sqlalchemy.orm import Session
 
 from plutous.trade.crypto import exchanges as ex
 from plutous.trade.enums import Action, PositionSide, StrategyDirection
```

### Comparing `plutous_trade_crypto-0.0.8/plutous/trade/crypto/enums/exchange.py` & `plutous_trade_crypto-0.0.9/plutous/trade/crypto/enums/exchange.py`

 * *Files identical despite different names*

### Comparing `plutous_trade_crypto-0.0.8/plutous/trade/crypto/exchanges/__init__.py` & `plutous_trade_crypto-0.0.9/plutous/trade/crypto/exchanges/__init__.py`

 * *Files identical despite different names*

### Comparing `plutous_trade_crypto-0.0.8/plutous/trade/crypto/exchanges/binance.py` & `plutous_trade_crypto-0.0.9/plutous/trade/crypto/exchanges/binance.py`

 * *Files identical despite different names*

### Comparing `plutous_trade_crypto-0.0.8/plutous/trade/crypto/exchanges/bitget.py` & `plutous_trade_crypto-0.0.9/plutous/trade/crypto/exchanges/bitget.py`

 * *Files identical despite different names*

### Comparing `plutous_trade_crypto-0.0.8/plutous/trade/crypto/exchanges/bybit.py` & `plutous_trade_crypto-0.0.9/plutous/trade/crypto/exchanges/bybit.py`

 * *Files identical despite different names*

### Comparing `plutous_trade_crypto-0.0.8/plutous/trade/crypto/exchanges/gateio.py` & `plutous_trade_crypto-0.0.9/plutous/trade/crypto/exchanges/gateio.py`

 * *Files identical despite different names*

### Comparing `plutous_trade_crypto-0.0.8/plutous/trade/crypto/exchanges/huobi.py` & `plutous_trade_crypto-0.0.9/plutous/trade/crypto/exchanges/huobi.py`

 * *Files identical despite different names*

### Comparing `plutous_trade_crypto-0.0.8/plutous/trade/crypto/exchanges/kucoin.py` & `plutous_trade_crypto-0.0.9/plutous/trade/crypto/exchanges/kucoin.py`

 * *Files identical despite different names*

### Comparing `plutous_trade_crypto-0.0.8/plutous/trade/crypto/exchanges/mexc.py` & `plutous_trade_crypto-0.0.9/plutous/trade/crypto/exchanges/mexc.py`

 * *Files identical despite different names*

### Comparing `plutous_trade_crypto-0.0.8/plutous/trade/crypto/exchanges/okx.py` & `plutous_trade_crypto-0.0.9/plutous/trade/crypto/exchanges/okx.py`

 * *Files identical despite different names*

### Comparing `plutous_trade_crypto-0.0.8/plutous/trade/crypto/exchanges/phemex.py` & `plutous_trade_crypto-0.0.9/plutous/trade/crypto/exchanges/phemex.py`

 * *Files identical despite different names*

### Comparing `plutous_trade_crypto-0.0.8/plutous/trade/crypto/migrations/env.py` & `plutous_trade_crypto-0.0.9/plutous/trade/crypto/migrations/env.py`

 * *Files identical despite different names*

### Comparing `plutous_trade_crypto-0.0.8/plutous/trade/crypto/models/base.py` & `plutous_trade_crypto-0.0.9/plutous/trade/crypto/models/base.py`

 * *Files identical despite different names*

### Comparing `plutous_trade_crypto-0.0.8/plutous/trade/crypto/utils/paginate.py` & `plutous_trade_crypto-0.0.9/plutous/trade/crypto/utils/paginate.py`

 * *Files identical despite different names*

### Comparing `plutous_trade_crypto-0.0.8/pyproject.toml` & `plutous_trade_crypto-0.0.9/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "plutous-trade-crypto"
-version = "0.0.8"
+version = "0.0.9"
 description = "Plutous Crypto Trading Library"
 packages = [{include = "plutous"}]
 authors = ["Cheun Hong <cheunhong@plutous.io>"]
 readme = "README.md"
 license="MIT"
 classifiers = [
     "Programming Language :: Python :: 3.10",
```

### Comparing `plutous_trade_crypto-0.0.8/PKG-INFO` & `plutous_trade_crypto-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plutous-trade-crypto
-Version: 0.0.8
+Version: 0.0.9
 Summary: Plutous Crypto Trading Library
 License: MIT
 Author: Cheun Hong
 Author-email: cheunhong@plutous.io
 Requires-Python: >=3.10,<3.11
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

