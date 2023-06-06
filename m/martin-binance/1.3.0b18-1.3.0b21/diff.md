# Comparing `tmp/martin-binance-1.3.0b18.tar.gz` & `tmp/martin-binance-1.3.0b21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "martin-binance-1.3.0b18.tar", last modified: Sun Jun  4 09:35:44 2023, max compression
+gzip compressed data, was "martin-binance-1.3.0b21.tar", last modified: Tue Jun  6 18:37:43 2023, max compression
```

## Comparing `martin-binance-1.3.0b18.tar` & `martin-binance-1.3.0b21.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      154 2022-06-16 20:42:55.292826 martin-binance-1.3.0b18/.deepsource.toml
--rw-r--r--   0        0        0       79 2022-09-29 14:39:58.264847 martin-binance-1.3.0b18/.dockerignore
--rw-r--r--   0        0        0       68 2022-06-16 20:42:55.292826 martin-binance-1.3.0b18/.github/FUNDING.yml
--rw-r--r--   0        0        0      665 2022-09-29 14:39:58.268851 martin-binance-1.3.0b18/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      604 2022-09-29 14:39:58.268851 martin-binance-1.3.0b18/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      837 2023-01-08 14:15:30.514225 martin-binance-1.3.0b18/.github/workflows/codeql.yml
--rw-r--r--   0        0        0       45 2022-09-29 14:39:58.268851 martin-binance-1.3.0b18/.gitignore
--rwxr-xr-x   0        0        0    17466 2023-06-04 09:16:25.405483 martin-binance-1.3.0b18/CHANGELOG.md
--rw-r--r--   0        0        0      601 2022-11-24 16:46:07.400338 martin-binance-1.3.0b18/Dockerfile
--rw-r--r--   0        0        0     1079 2022-06-16 20:37:23.392898 martin-binance-1.3.0b18/LICENSE
--rwxr-xr-x   0        0        0    35437 2023-05-30 12:20:07.843798 martin-binance-1.3.0b18/README.md
--rwxr-xr-x   0        0        0    89295 2021-12-09 10:16:46.764494 martin-binance-1.3.0b18/doc/Create_strategy.png
--rwxr-xr-x   0        0        0    26452 2021-12-09 10:16:46.764494 martin-binance-1.3.0b18/doc/Model of logarithmic grid.ods
--rw-r--r--   0        0        0  5309091 2021-12-09 10:16:46.820491 martin-binance-1.3.0b18/doc/Modified martingale.svg
--rwxr-xr-x   0        0        0    79517 2021-12-09 10:16:46.824491 martin-binance-1.3.0b18/doc/graf1.png
--rwxr-xr-x   0        0        0    10318 2021-12-09 10:16:46.824491 martin-binance-1.3.0b18/doc/tlg_notify.png
--rwxr-xr-x   0        0        0     9332 2021-12-09 10:16:46.824491 martin-binance-1.3.0b18/doc/tmux.png
--rw-r--r--   0        0        0     1941 2023-06-04 09:02:30.443389 martin-binance-1.3.0b18/martin_binance/__init__.py
--rw-r--r--   0        0        0     2012 2023-06-03 20:42:37.621820 martin-binance-1.3.0b18/martin_binance/backtest/OoTSP.py
--rw-r--r--   0        0        0     2949 2023-06-03 09:17:19.879857 martin-binance-1.3.0b18/martin_binance/backtest/VCoSEL.py
--rw-r--r--   0        0        0        0 2023-06-01 20:26:31.871396 martin-binance-1.3.0b18/martin_binance/backtest/__init__.py
--rw-r--r--   0        0        0    12120 2023-06-02 12:08:24.729428 martin-binance-1.3.0b18/martin_binance/backtest/exchange_simulator.py
--rw-r--r--   0        0        0     6474 2023-06-01 20:26:31.871396 martin-binance-1.3.0b18/martin_binance/cli_0_BTCUSDT.py.template
--rw-r--r--   0        0        0     6469 2023-06-01 20:26:31.871396 martin-binance-1.3.0b18/martin_binance/cli_1_BTCUSDT.py.template
--rw-r--r--   0        0        0     6475 2023-06-01 20:26:31.871396 martin-binance-1.3.0b18/martin_binance/cli_2_TESTBTCTESTUSDT.py.template
--rw-r--r--   0        0        0     4710 2023-06-01 20:26:31.871396 martin-binance-1.3.0b18/martin_binance/client.py
--rw-r--r--   0        0        0   181446 2023-06-04 09:02:30.439389 martin-binance-1.3.0b18/martin_binance/executor.py
--rw-r--r--   0        0        0   237568 2022-09-29 14:39:58.276860 martin-binance-1.3.0b18/martin_binance/funds_rate.db.template
--rwxr-xr-x   0        0        0   337272 2022-09-29 14:39:58.276860 martin-binance-1.3.0b18/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so
--rw-r--r--   0        0        0      376 2022-12-19 14:10:45.443888 martin-binance-1.3.0b18/martin_binance/margin/margin_req.txt
--rw-r--r--   0        0        0      348 2023-01-08 14:15:30.514225 martin-binance-1.3.0b18/martin_binance/margin/margin_req_win.txt
--rw-r--r--   0        0        0    77874 2023-06-03 18:24:38.067992 martin-binance-1.3.0b18/martin_binance/margin_wrapper.py
--rw-r--r--   0        0        0     1472 2023-01-19 11:11:07.967695 martin-binance-1.3.0b18/martin_binance/ms_cfg.toml.template
--rw-r--r--   0        0        0      485 2021-12-09 09:06:56.984779 martin-binance-1.3.0b18/martin_binance/service/.tmux.conf
--rwxr-xr-x   0        0        0      319 2022-09-29 14:39:58.280864 martin-binance-1.3.0b18/martin_binance/service/funds_export.service
--rwxr-xr-x   0        0        0    16185 2023-05-30 12:20:07.847793 martin-binance-1.3.0b18/martin_binance/service/funds_rate_exporter.py
--rwxr-xr-x   0        0        0    75764 2023-05-30 12:20:07.847793 martin-binance-1.3.0b18/martin_binance/service/grafana.json
--rwxr-xr-x   0        0        0     1276 2022-09-29 14:39:58.280864 martin-binance-1.3.0b18/martin_binance/service/relaunch.py
--rwxr-xr-x   0        0        0      271 2022-09-29 14:39:58.284868 martin-binance-1.3.0b18/martin_binance/service/relaunch.service
--rwxr-xr-x   0        0        0      372 2021-12-09 09:06:56.984779 martin-binance-1.3.0b18/martin_binance/service/tmux.service
--rw-r--r--   0        0        0     1203 2023-06-03 20:53:44.166165 martin-binance-1.3.0b18/pyproject.toml
--rw-r--r--   0        0        0      320 2023-06-03 20:53:44.162164 martin-binance-1.3.0b18/requirements.txt
--rw-r--r--   0        0        0     2390 2023-01-19 11:11:07.971695 martin-binance-1.3.0b18/uml/architecture.puml
--rw-r--r--   0        0        0    36614 1970-01-01 00:00:00.000000 martin-binance-1.3.0b18/PKG-INFO
+-rw-r--r--   0        0        0      154 2022-06-16 20:42:55.292826 martin-binance-1.3.0b21/.deepsource.toml
+-rw-r--r--   0        0        0       79 2022-09-29 14:39:58.264847 martin-binance-1.3.0b21/.dockerignore
+-rw-r--r--   0        0        0       68 2022-06-16 20:42:55.292826 martin-binance-1.3.0b21/.github/FUNDING.yml
+-rw-r--r--   0        0        0      665 2022-09-29 14:39:58.268851 martin-binance-1.3.0b21/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      604 2022-09-29 14:39:58.268851 martin-binance-1.3.0b21/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      837 2023-01-08 14:15:30.514225 martin-binance-1.3.0b21/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0       45 2022-09-29 14:39:58.268851 martin-binance-1.3.0b21/.gitignore
+-rwxr-xr-x   0        0        0    17691 2023-06-06 16:49:15.643997 martin-binance-1.3.0b21/CHANGELOG.md
+-rw-r--r--   0        0        0      601 2022-11-24 16:46:07.400338 martin-binance-1.3.0b21/Dockerfile
+-rw-r--r--   0        0        0     1079 2022-06-16 20:37:23.392898 martin-binance-1.3.0b21/LICENSE
+-rwxr-xr-x   0        0        0    35437 2023-05-30 12:20:07.843798 martin-binance-1.3.0b21/README.md
+-rwxr-xr-x   0        0        0    89295 2021-12-09 10:16:46.764494 martin-binance-1.3.0b21/doc/Create_strategy.png
+-rwxr-xr-x   0        0        0    26452 2021-12-09 10:16:46.764494 martin-binance-1.3.0b21/doc/Model of logarithmic grid.ods
+-rw-r--r--   0        0        0  5309091 2021-12-09 10:16:46.820491 martin-binance-1.3.0b21/doc/Modified martingale.svg
+-rwxr-xr-x   0        0        0    79517 2021-12-09 10:16:46.824491 martin-binance-1.3.0b21/doc/graf1.png
+-rwxr-xr-x   0        0        0    10318 2021-12-09 10:16:46.824491 martin-binance-1.3.0b21/doc/tlg_notify.png
+-rwxr-xr-x   0        0        0     9332 2021-12-09 10:16:46.824491 martin-binance-1.3.0b21/doc/tmux.png
+-rw-r--r--   0        0        0     2004 2023-06-05 20:18:03.227997 martin-binance-1.3.0b21/martin_binance/__init__.py
+-rw-r--r--   0        0        0     2218 2023-06-05 19:37:24.375292 martin-binance-1.3.0b21/martin_binance/backtest/OoTSP.py
+-rw-r--r--   0        0        0     2949 2023-06-03 09:17:19.879857 martin-binance-1.3.0b21/martin_binance/backtest/VCoSEL.py
+-rw-r--r--   0        0        0        0 2023-06-01 20:26:31.871396 martin-binance-1.3.0b21/martin_binance/backtest/__init__.py
+-rw-r--r--   0        0        0    12323 2023-06-04 14:26:32.096258 martin-binance-1.3.0b21/martin_binance/backtest/exchange_simulator.py
+-rw-r--r--   0        0        0     6474 2023-06-01 20:26:31.871396 martin-binance-1.3.0b21/martin_binance/cli_0_BTCUSDT.py.template
+-rw-r--r--   0        0        0     6469 2023-06-01 20:26:31.871396 martin-binance-1.3.0b21/martin_binance/cli_1_BTCUSDT.py.template
+-rw-r--r--   0        0        0     6475 2023-06-01 20:26:31.871396 martin-binance-1.3.0b21/martin_binance/cli_2_TESTBTCTESTUSDT.py.template
+-rw-r--r--   0        0        0     4710 2023-06-01 20:26:31.871396 martin-binance-1.3.0b21/martin_binance/client.py
+-rw-r--r--   0        0        0   181583 2023-06-06 18:14:42.861974 martin-binance-1.3.0b21/martin_binance/executor.py
+-rw-r--r--   0        0        0   237568 2022-09-29 14:39:58.276860 martin-binance-1.3.0b21/martin_binance/funds_rate.db.template
+-rwxr-xr-x   0        0        0   337272 2022-09-29 14:39:58.276860 martin-binance-1.3.0b21/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so
+-rw-r--r--   0        0        0      376 2022-12-19 14:10:45.443888 martin-binance-1.3.0b21/martin_binance/margin/margin_req.txt
+-rw-r--r--   0        0        0      348 2023-01-08 14:15:30.514225 martin-binance-1.3.0b21/martin_binance/margin/margin_req_win.txt
+-rw-r--r--   0        0        0    79598 2023-06-06 16:41:38.089871 martin-binance-1.3.0b21/martin_binance/margin_wrapper.py
+-rw-r--r--   0        0        0     1472 2023-01-19 11:11:07.967695 martin-binance-1.3.0b21/martin_binance/ms_cfg.toml.template
+-rw-r--r--   0        0        0      485 2021-12-09 09:06:56.984779 martin-binance-1.3.0b21/martin_binance/service/.tmux.conf
+-rwxr-xr-x   0        0        0      319 2022-09-29 14:39:58.280864 martin-binance-1.3.0b21/martin_binance/service/funds_export.service
+-rwxr-xr-x   0        0        0    16185 2023-05-30 12:20:07.847793 martin-binance-1.3.0b21/martin_binance/service/funds_rate_exporter.py
+-rwxr-xr-x   0        0        0    75764 2023-05-30 12:20:07.847793 martin-binance-1.3.0b21/martin_binance/service/grafana.json
+-rwxr-xr-x   0        0        0     1276 2022-09-29 14:39:58.280864 martin-binance-1.3.0b21/martin_binance/service/relaunch.py
+-rwxr-xr-x   0        0        0      271 2022-09-29 14:39:58.284868 martin-binance-1.3.0b21/martin_binance/service/relaunch.service
+-rwxr-xr-x   0        0        0      372 2021-12-09 09:06:56.984779 martin-binance-1.3.0b21/martin_binance/service/tmux.service
+-rw-r--r--   0        0        0     1203 2023-06-03 20:53:44.166165 martin-binance-1.3.0b21/pyproject.toml
+-rw-r--r--   0        0        0      320 2023-06-03 20:53:44.162164 martin-binance-1.3.0b21/requirements.txt
+-rw-r--r--   0        0        0     2390 2023-01-19 11:11:07.971695 martin-binance-1.3.0b21/uml/architecture.puml
+-rw-r--r--   0        0        0    36614 1970-01-01 00:00:00.000000 martin-binance-1.3.0b21/PKG-INFO
```

### Comparing `martin-binance-1.3.0b18/.github/ISSUE_TEMPLATE/bug_report.md` & `martin-binance-1.3.0b21/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b18/.github/ISSUE_TEMPLATE/feature_request.md` & `martin-binance-1.3.0b21/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b18/.github/workflows/codeql.yml` & `martin-binance-1.3.0b21/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b18/CHANGELOG.md` & `martin-binance-1.3.0b21/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,18 @@
-## v1.3.0b18 2023-06-04
+## v1.3.0b18-21 2023-06-06
 ### Fix
 * #59
 
+### Update
+* Sync record/play
+* Add SAVE_DS = True  # Save session result data (ticker, orders) for compare
+* up requirements for exchanges-wrapper to 1.3.0-1
+* refactoring class StrategyBase
+* + backtest_data_control()
+ 
 ## v1.3.0b12 2023-06-02
 ### Fix
 * deepsource issues
 
 ## v1.3.0b11 2023-06-01
 ### Fix
 * Bitfinex: rename test pair from AAABBB to TESTBTCTESTUSDT, update template
```

### Comparing `martin-binance-1.3.0b18/Dockerfile` & `martin-binance-1.3.0b21/Dockerfile`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b18/LICENSE` & `martin-binance-1.3.0b21/LICENSE`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b18/README.md` & `martin-binance-1.3.0b21/README.md`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b18/doc/Create_strategy.png` & `martin-binance-1.3.0b21/doc/Create_strategy.png`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b18/doc/Model of logarithmic grid.ods` & `martin-binance-1.3.0b21/doc/Model of logarithmic grid.ods`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b18/doc/Modified martingale.svg` & `martin-binance-1.3.0b21/doc/Modified martingale.svg`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b18/doc/graf1.png` & `martin-binance-1.3.0b21/doc/graf1.png`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b18/doc/tlg_notify.png` & `martin-binance-1.3.0b21/doc/tlg_notify.png`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b18/doc/tmux.png` & `martin-binance-1.3.0b21/doc/tmux.png`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b18/martin_binance/__init__.py` & `martin-binance-1.3.0b21/martin_binance/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 """
 Free trading system for Binance SPOT API
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.0b18"
+__version__ = "1.3.0b21"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 from pathlib import Path
 from shutil import copy
 #
 import platform
@@ -47,7 +47,9 @@
     copy(Path(Path(__file__).parent.absolute(), "cli_1_BTCUSDT.py.template"), Path(WORK_PATH, "cli_1_BTCUSDT.py"))
     copy(Path(Path(__file__).parent.absolute(), "cli_2_TESTBTCTESTUSDT.py.template"),
          Path(WORK_PATH, "cli_2_TESTBTCTESTUSDT.py"))
     print(f"Before the first run, set the parameters in {CONFIG_FILE}")
     if STANDALONE:
         raise SystemExit(1)
     raise UserWarning()
+
+# TODO Add parameter for not record analytics data in 'S' MODE
```

### Comparing `martin-binance-1.3.0b18/martin_binance/backtest/OoTSP.py` & `martin-binance-1.3.0b21/martin_binance/backtest/OoTSP.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,41 +2,45 @@
 # -*- coding: utf-8 -*-
 """
 Optimization of Trading Strategy Parameters
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.0b16"
+__version__ = "1.3.0b20"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 from pathlib import Path
 import importlib.util
 from decimal import Decimal
 import optuna
 
+from tkinter.filedialog import askopenfile
 from martin_binance import BACKTEST_PATH
 
 
-spec = importlib.util.spec_from_file_location(
-    "strategy", Path(BACKTEST_PATH, Path("BTCUSDT_SOURCE", "cli_7_BTCUSDT.py"))
-)
+strategy = askopenfile(defaultextension='py',
+                       title='Select a file with strategy parameters',
+                       initialdir=str(BACKTEST_PATH))
+
+spec = importlib.util.spec_from_file_location("strategy", Path(BACKTEST_PATH, strategy.name))
 
 mbs = importlib.util.module_from_spec(spec)
 spec.loader.exec_module(mbs)
 
 PARAMS_FLOAT = ['PRICE_SHIFT', 'KBB']
 
 
 def try_trade(**kwargs):
     for key, value in kwargs.items():
         print(key, value)
         setattr(mbs.ex, key, value if isinstance(value, int) or key in PARAMS_FLOAT else Decimal(f"{value}"))
     mbs.ex.MODE = 'S'
+    mbs.ex.SAVE_DS = False
     mbs.trade()
     result = float(mbs.session_result.get('profit', 0)) + float(mbs.session_result.get('free', 0))
     return result
 
 
 def objective(trial):
     params = {
@@ -51,10 +55,10 @@
         'KBB': trial.suggest_float('KBB', 1, 5, step=0.5),
         'LINEAR_GRID_K': trial.suggest_int('LINEAR_GRID_K', 0, 100, step=10),
     }
     return try_trade(**params)
 
 
 study = optuna.create_study(direction="maximize")
-study.optimize(objective, n_trials=1000)
+study.optimize(objective, n_trials=100)
 
 print(f"Optimal parameters: {study.best_params} for get {study.best_value}")
```

### Comparing `martin-binance-1.3.0b18/martin_binance/backtest/VCoSEL.py` & `martin-binance-1.3.0b21/martin_binance/backtest/VCoSEL.py`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b18/martin_binance/backtest/exchange_simulator.py` & `martin-binance-1.3.0b21/martin_binance/backtest/exchange_simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,16 @@
         self.order_creation_time = lt
         self.quote_asset_transacted: str
         self.last_quote_asset_transacted: str
         self.quote_order_quantity: str
 
 
 class Account:
-    def __init__(self):
+    def __init__(self, save_ds: bool):
+        self.save_ds = save_ds
         self.funds = Funds()
         self.fee_maker = Decimal('0')
         self.fee_taker = Decimal('0')
         self.orders = []
         self.orders_buy = pd.Series()
         self.orders_sell = pd.Series()
         self.trade_id = 0
@@ -130,18 +131,20 @@
             order.quote_order_quantity = order.cummulative_quote_qty
             #
             self.funds.on_order_created(buy=buy, amount=amount, price=price)
             self.funds.on_order_filled(order.side, order.orig_qty, order.last_executed_price, self.fee_taker)
         else:
             if buy:
                 self.orders_buy.at[order_id] = Decimal(price)
-                self.grid_buy[lt] = self.orders_buy
+                if self.save_ds:
+                    self.grid_buy[lt] = self.orders_buy
             else:
                 self.orders_sell.at[order_id] = Decimal(price)
-                self.grid_sell[lt] = self.orders_sell
+                if self.save_ds:
+                    self.grid_sell[lt] = self.orders_sell
             #
             self.funds.on_order_created(buy=buy, amount=amount, price=price)
 
         self.orders.append(order)
 
         # print(f"create_order.order: {vars(order)}")
         return {'symbol': order.symbol,
@@ -162,19 +165,19 @@
 
     def cancel_order(self, order_id: int, ts: int):
         order = self.orders[order_id]
         order.status = 'CANCELED'
         try:
             if order.side == 'BUY':
                 self.orders_buy = self.orders_buy.drop(order_id)
-                if self.orders_buy.values.size:
+                if self.save_ds and self.orders_buy.values.size:
                     self.grid_buy[ts] = self.orders_buy
             else:
                 self.orders_sell = self.orders_sell.drop(order_id)
-                if self.orders_sell.values.size:
+                if self.save_ds and self.orders_sell.values.size:
                     self.grid_sell[ts] = self.orders_sell
         except Exception as ex:
             raise UserWarning(f"Order {order_id} not active: {ex}")
         else:
             self.orders[order_id] = order
             self.funds.on_order_canceled(order.side, order.orig_qty, order.price)
             return {'symbol': order.symbol,
@@ -211,20 +214,21 @@
         _i = self.orders_sell[self.orders_sell <= self.ticker_last].index
         try:
             self.orders_sell = self.orders_sell.drop(_i.values)
         except Exception as ex:
             print(ex)
         orders_id.extend(_i.values)
 
-        # Save data for analytics
-        self.ticker[ts] = ticker['lastPrice']
-        if self.orders_sell.values.size:
-            self.grid_sell[ts] = self.orders_sell
-        if self.orders_buy.values.size:
-            self.grid_buy[ts] = self.orders_buy
+        if self.save_ds:
+            # Save data for analytics
+            self.ticker[ts] = ticker['lastPrice']
+            if self.orders_sell.values.size:
+                self.grid_sell[ts] = self.orders_sell
+            if self.orders_buy.values.size:
+                self.grid_buy[ts] = self.orders_buy
         #
         orders_filled = []
         for order_id in orders_id:
             order = self.orders[order_id]
             if order.status == 'NEW':
                 order.transact_time = int(ticker['closeTime'])
                 order.executed_qty = order.orig_qty
```

### Comparing `martin-binance-1.3.0b18/martin_binance/cli_0_BTCUSDT.py.template` & `martin-binance-1.3.0b21/martin_binance/cli_0_BTCUSDT.py.template`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b18/martin_binance/cli_1_BTCUSDT.py.template` & `martin-binance-1.3.0b21/martin_binance/cli_1_BTCUSDT.py.template`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b18/martin_binance/cli_2_TESTBTCTESTUSDT.py.template` & `martin-binance-1.3.0b21/martin_binance/cli_2_TESTBTCTESTUSDT.py.template`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b18/martin_binance/client.py` & `martin-binance-1.3.0b21/martin_binance/client.py`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b18/martin_binance/executor.py` & `martin-binance-1.3.0b21/martin_binance/executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ####################################################################
 # Cyclic grid strategy based on martingale
 ##################################################################
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.0b18"
+__version__ = "1.3.0b20"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = 'https://github.com/DogsTailFarmer'
 ##################################################################
 import sys
 import gc
 import statistics
 from decimal import Decimal, ROUND_FLOOR, ROUND_CEILING
@@ -102,14 +102,16 @@
 TOKEN = str()
 CHANNEL_ID = str()
 STOP_TLG = 'stop_signal_QWE#@!'
 INLINE_BOT = True
 # Backtesting
 MODE = 'T'  # 'T' - Trade, 'TC' - Trade and Collect, 'S' - Simulate
 XTIME = 500  # Time accelerator
+SAVE_DS = True  # Save session result data (ticker, orders) for compare
+SAVE_PERIOD = 1 * 60 * 60  # sec, timetable for save data portion, but memory limitation consider also matter
 # endregion
 
 
 class Style:
     BLACK: str = '\033[30m'
     RED: str = '\033[31m'
     B_RED: str = '\033[1;31m'
@@ -711,15 +713,15 @@
         self.cycle_status = ()  # - Operational status for current cycle, orders count
         self.grid_update_started = None  # - Flag when grid update process started
         self.start_reverse_time = None  # -
         self.last_ticker_update = 0  # -
         self.grid_only_restart = None  # -
         self.local_time = self.get_time if STANDALONE else time.time
         self.wait_wss_refresh = {}  # -
-        self.start_collect = False
+        self.start_collect = None
 
     def init(self, check_funds: bool = True) -> None:  # skipcq: PYL-W0221
         self.message_log('Start Init section')
         if not FEE_IN_PAIR and FEE_SECOND:
             init_params_error = 'FEE_IN_PAIR and FEE_SECOND'
         elif not FEE_IN_PAIR and FEE_BNB_IN_PAIR:
             init_params_error = 'FEE_IN_PAIR and FEE_BNB_IN_PAIR'
@@ -736,15 +738,14 @@
         db_management()
         tcm = self.get_trading_capability_manager()
         self.f_currency = self.get_first_currency()
         self.s_currency = self.get_second_currency()
         self.tlg_header = f"{EXCHANGE[ID_EXCHANGE]}, {self.f_currency}/{self.s_currency}. "
         self.message_log(f"{self.tlg_header}", color=Style.B_WHITE)
         self.status_time = int(self.local_time())
-        # self.cycle_time = datetime.utcnow()
         self.start_after_shift = True
         self.over_price = OVER_PRICE
         self.order_q = ORDER_Q
         self.martin = (MARTIN + 100) / 100
         if not check_funds:
             self.first_run = False
         if GRID_ONLY:
@@ -972,15 +973,15 @@
                 self.grid_update(frequency='low')
             elif self.heartbeat_counter % 30 == 0:
                 self.grid_update(frequency='mid')
             else:
                 self.grid_update(frequency='hi')
         if self.heartbeat_counter > 150:
             self.heartbeat_counter = 0
-            if MODE in ('T', 'TC'):
+            if MODE in ('T', 'TC') and not GRID_ONLY:
                 # Update t_funds.active set True
                 data_to_db = {'f_currency': self.f_currency,
                               's_currency': self.s_currency,
                               'destination': 't_funds.active update'}
                 if self.queue_to_db:
                     self.queue_to_db.put(data_to_db)
         if self.wait_refunding_for_start or self.tp_order_hold or self.grid_hold:
@@ -1061,17 +1062,16 @@
             self.message_log("restore_strategy_state from saved state:", log_level=LogLevel.DEBUG)
             self.message_log("\n".join(f"{k}\t{v}" for k, v in strategy_state.items()), log_level=LogLevel.DEBUG)
             #
             self.command = json.loads(strategy_state.get('command'))
             self.cycle_buy = json.loads(strategy_state.get('cycle_buy'))
             self.cycle_buy_count = json.loads(strategy_state.get('cycle_buy_count'))
             self.cycle_sell_count = json.loads(strategy_state.get('cycle_sell_count'))
-            self.cycle_time = json.loads(strategy_state.get('cycle_time'))
-            if self.cycle_time:
-                self.cycle_time = datetime.strptime(self.cycle_time, '%Y-%m-%d %H:%M:%S.%f')
+            self.cycle_time = json.loads(strategy_state.get('cycle_time', str(datetime.utcnow())))
+            self.cycle_time = datetime.strptime(self.cycle_time, '%Y-%m-%d %H:%M:%S.%f')
             self.cycle_time_reverse = json.loads(strategy_state.get('cycle_time_reverse'))
             if self.cycle_time_reverse:
                 self.cycle_time_reverse = datetime.strptime(self.cycle_time_reverse, '%Y-%m-%d %H:%M:%S.%f')
             self.deposit_first = f2d(json.loads(strategy_state.get('deposit_first')))
             self.deposit_second = f2d(json.loads(strategy_state.get('deposit_second')))
             self.last_shift_time = json.loads(strategy_state.get('last_shift_time')) or self.local_time()
             self.martin = f2d(json.loads(strategy_state.get('martin')))
@@ -1427,18 +1427,18 @@
                              f"For all cycles profit:\n"
                              f"First: {self.sum_profit_first}\n"
                              f"Second: {self.sum_profit_second}\n"
                              f"Summary: {self.sum_profit_first * self.avg_rate + self.sum_profit_second:f}\n")
         if self.first_run or MODE in ('T', 'TC'):
             self.cycle_time = datetime.utcnow()
         mem = psutil.virtual_memory().percent if psutil else 0
-        if mem > 80:
+        if mem > 85:
             self.message_log(f"For {VPS_NAME} critical memory availability, end", tlg=True)
             self.command = 'end'
-        elif mem > 70:
+        elif mem > 75:
             self.message_log(f"For {VPS_NAME} low memory availability, stop after end of cycle", tlg=True)
             self.command = 'stop'
         if self.command == 'end' or (self.command == 'stop' and
                                      (not self.reverse or (self.reverse and REVERSE_STOP))):
             self.command = 'stopped'
             self.start_collect = 1
             self.message_log('Stop, waiting manual action', tlg=True)
@@ -2158,17 +2158,17 @@
         self.message_log(f"set_trade_conditions: buy_side: {buy_side}, depo: {float(depo):f}, base_price: {base_price},"
                          f" reverse_target_amount: {reverse_target_amount}, amount_min: {amount_min},"
                          f" step_size: {step_size}, delta_min: {delta_min}", LogLevel.DEBUG)
         if not additional_grid and not grid_update and not GRID_ONLY and 0 < PROFIT_MAX < 100:
             try:
                 profit_max = min(PROFIT_MAX, max(PROFIT, f2d(100 * self.atr() / self.get_buffered_ticker().last_price)))
             except statistics.StatisticsError as ex:
-                self.message_log(f"Can't get ATR value: {ex}, use default PROFIT_MAX value", LogLevel.WARNING)
-                profit_max = PROFIT_MAX
-            self.message_log(f"Profit max for first order volume is: {profit_max}", LogLevel.DEBUG)
+                self.message_log(f"Can't get ATR value: {ex}, use default PROFIT value", LogLevel.WARNING)
+                profit_max = PROFIT
+            self.message_log(f"Profit max for first order volume is set {profit_max}%", LogLevel.DEBUG)
             k_m = 1 - profit_max / 100
             amount_first_grid = max(amount_min, (step_size * base_price / ((1 / k_m) - 1)) / base_price)
             amount_first_grid = self.round_truncate(amount_first_grid, base=True, _rounding=ROUND_CEILING)
         else:
             amount_first_grid = amount_min
         if self.reverse:
             over_price = self.calc_over_price(buy_side,
```

### Comparing `martin-binance-1.3.0b18/martin_binance/funds_rate.db.template` & `martin-binance-1.3.0b21/martin_binance/funds_rate.db.template`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b18/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so` & `martin-binance-1.3.0b21/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b18/martin_binance/margin_wrapper.py` & `martin-binance-1.3.0b21/martin_binance/margin_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 """
 margin.de <-> Python strategy <-> <margin_wrapper> <-> exchanges-wrapper <-> Exchanges API/WSS
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.0b14"
+__version__ = "1.3.0b21"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 import ast
 import asyncio
 import simplejson as json
 import logging
 import math
 import os
 import time
 import sqlite3
 import random
 import traceback
 import pandas as pd
+import shutil
+import psutil
 
 from colorama import init as color_init
 from decimal import Decimal
 from pathlib import Path
 from datetime import datetime, timedelta
 
 # noinspection PyPackageRequirements
@@ -389,26 +391,14 @@
     send_request = None
     for_request = None
     wss_fire_up = False
     backtest = {}
     delay_ordering_s = 0.5
     bulk_orders_cancel = {}
 
-    def __init__(self):
-        self.time_operational = {'start': 0.0, 'ts': 0.0, 'new': 0.0}  # - See get_time()
-        self.ticker = {}
-        self.order_book = {}
-        self.klines = {}  # KLines snapshot
-        self.candles = {}  # Candles stream
-        self.account = None
-        self.grid_buy = {}
-        self.grid_sell = {}
-
-    def __call__(self):
-        return self
 
     class Klines:
         klines_series = {}
         klines_lim = int()
 
         def __init__(self, _interval):
             self.interval = _interval
@@ -429,104 +419,115 @@
                         del self.kline[0]
                 self.klines_series[self.interval] = self.kline
 
         @classmethod
         def get_kline(cls, _interval) -> []:
             return cls.klines_series.get(_interval, [])
 
-    @classmethod
-    def order_exist(cls, _id) -> bool:
-        return any(i.id == _id for i in cls.orders)
-
-    @classmethod
-    def all_order_exist(cls, _id) -> bool:
-        return any(i.id == _id for i in cls.all_orders)
-
-    @classmethod
-    def get_trading_capability_manager(cls) -> TradingCapabilityManager:
-        # print(f"get_trading_capability_manager.info_symbol: {cls.info_symbol}")
-        return StrategyBase.tcm
-
-    @classmethod
-    def get_first_currency(cls) -> str:
-        return cls.info_symbol.get('baseAsset')
-
-    @classmethod
-    def get_second_currency(cls) -> str:
-        return cls.info_symbol.get('quoteAsset')
-
-    @classmethod
-    def get_buffered_ticker(cls) -> Ticker:
-        # print(f"get_buffered_ticker.ticker: {cls.ticker}")
-        return Ticker(cls.ticker)
-
-    @classmethod
-    def get_buffered_funds(cls) -> Dict[str, FundsEntry]:
-        # print(f"get_buffered_funds.funds: {cls.funds}")
-        if cls.strategy.local_time() - cls.get_buffered_funds_last_time > cls.rate_limiter:
+
+    def __init__(self):
+        print("Init StrategyBase")
+        self.time_operational = {'start': 0.0, 'ts': 0.0, 'new': 0.0}  # - See get_time()
+        self.s_ticker = {}
+        self.s_order_book = {}
+        self.klines = {}  # KLines snapshot
+        self.candles = {}  # Candles stream
+        self.account = backTestAccount(ms.SAVE_DS) if ms.MODE == 'S' else None
+        self.grid_buy = {}
+        self.grid_sell = {}
+
+    def __call__(self):
+        return self
+
+    def reset_var(self):
+        self.s_ticker = {}
+        self.s_order_book = {}
+        self.klines = {}  # KLines snapshot
+        self.candles = {}  # Candles stream
+        self.grid_buy = {}
+        self.grid_sell = {}
+
+    @staticmethod
+    def reset_class_var():
+        cls = StrategyBase
+        cls.ticker = {}
+        cls.funds = {}
+        cls.order_book = {}
+        cls.order_id = int(datetime.now().strftime("%S%M")) * 1000
+        cls.wait_order_id = []  # List of placed orders for time-out detect
+        cls.canceled_order_id = []  # List canceled orders  for time-out detect
+        cls.all_trades = []  # List of all (limit = ALL_TRADES_LIST_LIMIT) trades for a specific account and symbol
+        cls.trades = []  # List of trades associated with strategy (limit = TRADES_LIST_LIMIT)
+        cls.all_orders = []  # List of all open orders for symbol
+        cls.orders = []  # List orders associated with strategy
+        cls.get_buffered_funds_last_time = time.time()
+        cls.rate_limiter = RATE_LIMITER
+        cls.start_time_ms = int(time.time() * 1000)
+        cls.backtest = {}
+        cls.bulk_orders_cancel = {}
+
+    def message_log(self,*args, **kwargs):
+        pass
+
+    def order_exist(self, _id) -> bool:
+        return any(i.id == _id for i in self.orders)
+
+    def all_order_exist(self, _id) -> bool:
+        return any(i.id == _id for i in self.all_orders)
+
+    def get_trading_capability_manager(self) -> TradingCapabilityManager:
+        # print(f"get_trading_capability_manager.tcm: {vars(StrategyBase.tcm)}")
+        return self.tcm
+
+    def get_first_currency(self) -> str:
+        return self.info_symbol.get('baseAsset')
+
+    def get_second_currency(self) -> str:
+        return self.info_symbol.get('quoteAsset')
+
+    def get_buffered_ticker(self) -> Ticker:
+        # print(f"get_buffered_ticker.ticker: {self.ticker}")
+        return Ticker(self.ticker)
+
+    def get_buffered_funds(self) -> Dict[str, FundsEntry]:
+        # print(f"get_buffered_funds.funds: {self.funds}")
+        if self.strategy.local_time() - self.get_buffered_funds_last_time > self.rate_limiter:
             # noinspection PyTypeChecker
             loop.create_task(buffered_funds(print_info=False))
-            cls.get_buffered_funds_last_time = cls.strategy.local_time()
-        return {cls.base_asset: FundsEntry(cls.funds[cls.base_asset]),
-                cls.quote_asset: FundsEntry(cls.funds[cls.quote_asset])}
-
-    @classmethod
-    def get_buffered_order_book(cls) -> OrderBook:
-        # print(f"get_buffered_order_book.order_book: {cls.order_book}")
-        return OrderBook(cls.order_book)
-
-    @classmethod
-    def get_buffered_recent_candles(cls, candle_size_in_minutes: int, number_of_candles: int = 50,
-                                    include_current_building_candle: bool = False) -> List[Candle]:
-        size = convert_from_minute(candle_size_in_minutes)
-        kline = StrategyBase.Klines.get_kline(size)
-        if len(kline) > number_of_candles+1:
-            return kline[-number_of_candles-(0 if include_current_building_candle else 1):
-                         None if include_current_building_candle else -1]
-        return kline[:None if include_current_building_candle else -1]
+            self.get_buffered_funds_last_time = self.strategy.local_time()
+        return {self.base_asset: FundsEntry(self.funds[self.base_asset]),
+                self.quote_asset: FundsEntry(self.funds[self.quote_asset])}
+
+    def get_buffered_order_book(self) -> OrderBook:
+        # print(f"get_buffered_order_book.order_book: {self.order_book}")
+        return OrderBook(self.order_book)
 
-    @classmethod
-    def place_limit_order(cls, buy: bool, amount: Decimal, price: Decimal) -> int:
+    def place_limit_order(self, buy: bool, amount: Decimal, price: Decimal) -> int:
+        cls = StrategyBase
         cls.order_id += 1
-        StrategyBase.strategy.message_log(f"Send order id:{cls.order_id} for {'BUY' if buy else 'SELL'}"
+        self.message_log(f"Send order id:{cls.order_id} for {'BUY' if buy else 'SELL'}"
                                           f" {any2str(amount)} by {any2str(price)} = {any2str(amount * price)}",
                                           color=ms.Style.B_YELLOW)
         loop.create_task(place_limit_order_timeout(cls.order_id))
         loop.create_task(create_limit_order(cls.order_id, buy, any2str(amount), any2str(price)))
-        if StrategyBase.exchange == 'huobi':
+        if cls.exchange == 'huobi':
             time.sleep(0.02)
-        elif StrategyBase.exchange == 'okx':
+        elif cls.exchange == 'okx':
             time.sleep(0.035)
         return cls.order_id
 
-    @classmethod
-    def cancel_order(cls, order_id: int) -> None:
-        loop.create_task(cancel_order_timeout(order_id))
-        loop.create_task(cancel_order_call(order_id))
-
-    @classmethod
-    def cancel_all_order(cls, order_id: int) -> None:
-        loop.create_task(cancel_order_timeout(order_id))
-        loop.create_task(cancel_all_order_call(order_id))
-
-    @classmethod
-    def get_buffered_completed_trades(cls, get_all_trades: bool = False) -> List[PrivateTrade]:
+    def get_buffered_completed_trades(self, get_all_trades: bool = False) -> List[PrivateTrade]:
         if get_all_trades:
-            return StrategyBase.all_trades
-        return StrategyBase.trades
+            return self.all_trades
+        return self.trades
 
-    @classmethod
-    def get_buffered_open_orders(cls, get_all_orders: bool = False) -> List[Order]:
+    def get_buffered_open_orders(self, get_all_orders: bool = False) -> List[Order]:
         if get_all_orders:
-            return cls.all_orders
-        return cls.orders
-
-    @classmethod
-    def transfer_to_master(cls, symbol: str, amount: str):
-        loop.create_task(transfer2master(symbol, amount))
+            return self.all_orders
+        return self.orders
 
     def get_time(self) -> float:
         """
         For backtesting purpose. Calculating monotonic local time based on self.time_operational['new'] value.
         It can be set from external source as int(time.time()) getting from historical data. If can't setting
         return system int(time.time()) Unix time.
         :return: int
@@ -545,25 +546,48 @@
             else:
                 self.time_operational['start'] = last = self.time_operational['new']
             self.time_operational['ts'] = time.time()
         else:
             last = time.time()
         return last
 
-    @classmethod
-    def open_orders_snapshot(cls):
+    def open_orders_snapshot(self):
         orders_buy = {}
         orders_sell = {}
-        for order in cls.orders:
+        for order in self.orders:
             if order.buy:
                 orders_buy[order.id] = order.price
             else:
                 orders_sell[order.id] = order.price
-        cls.strategy.grid_buy.update({int(time.time() * 1000): pd.Series(orders_buy)})
-        cls.strategy.grid_sell.update({int(time.time() * 1000): pd.Series(orders_sell)})
+        self.grid_buy.update({int(time.time() * 1000): pd.Series(orders_buy)})
+        self.grid_sell.update({int(time.time() * 1000): pd.Series(orders_sell)})
+
+    @staticmethod
+    def get_buffered_recent_candles(candle_size_in_minutes: int, number_of_candles: int = 50,
+                                    include_current_building_candle: bool = False) -> List[Candle]:
+        size = convert_from_minute(candle_size_in_minutes)
+        kline = StrategyBase.Klines.get_kline(size)
+        if len(kline) > number_of_candles+1:
+            return kline[-number_of_candles-(0 if include_current_building_candle else 1):
+                         None if include_current_building_candle else -1]
+        return kline[:None if include_current_building_candle else -1]
+
+    @staticmethod
+    def cancel_order(order_id: int) -> None:
+        loop.create_task(cancel_order_timeout(order_id))
+        loop.create_task(cancel_order_call(order_id))
+
+    @staticmethod
+    def cancel_all_order(order_id: int) -> None:
+        loop.create_task(cancel_order_timeout(order_id))
+        loop.create_task(cancel_all_order_call(order_id))
+
+    @staticmethod
+    def transfer_to_master(symbol: str, amount: str):
+        loop.create_task(transfer2master(symbol, amount))
 
 
 async def heartbeat(_session):
     cls = StrategyBase
     # print(f"tik-tak ', {int(time.time() * 1000)}, _client_id: {_client_id}")
     last_exec_time = time.time()
     while cls.strategy:
@@ -731,46 +755,15 @@
 async def ask_exit():
     cls = StrategyBase
     if cls.strategy:
         cls.strategy.message_log("Got signal for exit", color=ms.Style.MAGENTA)
 
         if ms.MODE == 'TC':
             # Save stream data for backtesting
-            # Save ticker
-            ds = pd.Series(cls.strategy.ticker)
-            ds.to_pickle(Path(BACKTEST_PATH, f"{ms.SYMBOL}_ticker.pkl"))
-            # Save order_book
-            ds = pd.Series(cls.strategy.order_book)
-            ds.to_pickle(Path(BACKTEST_PATH, f"{ms.SYMBOL}_order_book.pkl"))
-            # Save klines snapshot
-            json.dump(cls.strategy.klines, open(Path(BACKTEST_PATH, f"{ms.SYMBOL}_klines.json"), 'w'))
-            # Save candles
-            for k, v in cls.strategy.candles.items():
-                ds = pd.Series(v)
-                ds.to_pickle(Path(BACKTEST_PATH, f"{ms.SYMBOL}_candles_{k}.pkl"))
-            # Save session detail for analytics
-            session_path = Path(BACKTEST_PATH, f"{ms.SYMBOL}_SOURCE")
-            session_path.mkdir(parents=True, exist_ok=True)
-            #
-            d_ticker = {}
-            for k, v in cls.strategy.ticker.items():
-                d_ticker[k] = v['lastPrice']
-            ds_ticker = pd.Series(d_ticker).astype(float)
-            ds_ticker.index = pd.to_datetime(ds_ticker.index, unit='ms')
-            #
-            df_grid_sell = pd.DataFrame().from_dict(cls.strategy.grid_sell, orient='index')
-            df_grid_sell.index = pd.to_datetime(df_grid_sell.index, unit='ms')
-            df_grid_buy = pd.DataFrame().from_dict(cls.strategy.grid_buy, orient='index')
-            df_grid_buy.index = pd.to_datetime(df_grid_buy.index, unit='ms')
-            #
-            ds_ticker.to_pickle(Path(session_path, "ticker.pkl"))
-            df_grid_sell.to_pickle(Path(session_path, "sell.pkl"))
-            df_grid_buy.to_pickle(Path(session_path, "buy.pkl"))
-            #
-            copy(ms.PARAMS, Path(session_path, Path(ms.PARAMS).name))
+            session_data_handler(cls.strategy)
 
         if ms.MODE in ('T', 'TC'):
             await cls.send_request(cls.stub.StopStream, api_pb2.MarketRequest, symbol=cls.symbol)
 
         tasks = [t for t in asyncio.all_tasks() if t is not asyncio.current_task()]
         [task.cancel() for task in tasks]
         print(f"Cancelling {len(tasks)} outstanding tasks")
@@ -786,36 +779,105 @@
             if answer.lower() != 'y':
                 ms.LAST_STATE_FILE.replace(ms.LAST_STATE_FILE.with_suffix('.bak'))
                 print('Current state cleared')
             else:
                 print('OK')
 
 
+def session_data_handler(cls):
+    """
+    Save raw data for back testing and session snapshot for compare.
+    :param cls: StrategyBase.strategy
+    :return:
+    """
+    session_root = Path(BACKTEST_PATH, f"{cls.exchange}_{cls.symbol}")
+    raw_path = Path(session_root, "raw")
+    raw_path.mkdir(parents=True, exist_ok=True)
+    # Save ticker
+    ds = pd.Series(cls.s_ticker)
+    ds.to_pickle(Path(raw_path, "ticker.pkl"))
+    # Save order_book
+    ds = pd.Series(cls.s_order_book)
+    ds.to_pickle(Path(raw_path, "order_book.pkl"))
+    # Save klines snapshot
+    json.dump(cls.klines, open(Path(raw_path, "klines.json"), 'w'))
+    # Save candles
+    for k, v in cls.candles.items():
+        ds = pd.Series(v)
+        ds.to_pickle(Path(raw_path, f"candles_{k}.pkl"))
+    # Save session detail for analytics
+    session_data = Path(session_root, "snapshot")
+    session_data.mkdir(parents=True, exist_ok=True)
+    #
+    d_ticker = {}
+    for k, v in cls.s_ticker.items():
+        d_ticker[k] = v['lastPrice']
+    ds_ticker = pd.Series(d_ticker).astype(float)
+    ds_ticker.index = pd.to_datetime(ds_ticker.index, unit='ms')
+    #
+    df_grid_sell = pd.DataFrame().from_dict(cls.grid_sell, orient='index')
+    df_grid_sell.index = pd.to_datetime(df_grid_sell.index, unit='ms')
+    df_grid_buy = pd.DataFrame().from_dict(cls.grid_buy, orient='index')
+    df_grid_buy.index = pd.to_datetime(df_grid_buy.index, unit='ms')
+    #
+    ds_ticker.to_pickle(Path(session_data, "ticker.pkl"))
+    df_grid_sell.to_pickle(Path(session_data, "sell.pkl"))
+    df_grid_buy.to_pickle(Path(session_data, "buy.pkl"))
+    #
+    copy(ms.PARAMS, Path(session_root, Path(ms.PARAMS).name))
+
+    shutil.make_archive(str(Path(BACKTEST_PATH,f"{session_root}_{datetime.now().strftime('%m%d-%H:%M')}")),
+                        'zip',
+                        session_root)
+
+    print(f"Stream data for backtesting saved to {session_root}")
+
+
+async def backtest_data_control():
+    """
+    Control memory usage and safe saving by predefined timetable
+    """
+    cls = StrategyBase.strategy
+    delay = HEARTBEAT * 300  # 10 min
+    ts = time.time()
+    while True:
+        mem = psutil.virtual_memory().percent
+        if time.time() - ts > ms.SAVE_PERIOD or mem > 70:
+            sc = cls.start_collect
+            if sc:
+                cls.start_collect = False
+                session_data_handler(cls)
+                cls.reset_var()
+                cls.start_collect = sc
+                ts = time.time()
+        await asyncio.sleep(delay)
+
+
 async def buffered_candle():
     cls = StrategyBase
-    StrategyBase.Klines.klines_lim = KLINES_LIM
+    cls.Klines.klines_lim = KLINES_LIM
     klines = {}
     klines_from_file = {}
     if ms.MODE == 'S':
-        klines_from_file = json.load(open(Path(BACKTEST_PATH, f"{ms.SYMBOL}_klines.json")))
+        klines_from_file = json.load(open(Path(BACKTEST_PATH, f"{cls.exchange}_{cls.symbol}/raw/klines.json")))
     for i in KLINES_INIT:
         if ms.MODE in ('T', 'TC'):
             res = await cls.send_request(cls.stub.FetchKlines, api_pb2.FetchKlinesRequest,
                                          symbol=cls.symbol,
                                          interval=i.value,
                                          limit=KLINES_LIM)
             kline = json_format.MessageToDict(res)
-            if ms.MODE == 'TC':
+            if ms.MODE == 'TC' and (cls.strategy.start_collect or cls.strategy.start_collect is None):
                 cls.strategy.klines[i.value] = kline
         else:
             kline = klines_from_file.get(i.value, {})
         # print(f"buffered_candle.kline: {kline}")
         candles = kline.get('klines', [])
         if candles:
-            kline_i = StrategyBase.Klines(i.value)
+            kline_i = cls.Klines(i.value)
             for candle in candles:
                 kline_i.refresh(json.loads(candle))
                 # print(f"buffered_candle.candle: {candle}")
             klines[i.value] = kline_i
     if len(klines) == len(KLINES_INIT):
         loop.create_task(on_klines_update(klines))
     else:
@@ -830,23 +892,23 @@
     if ms.MODE in ('T', 'TC'):
         try:
             async for candle in cls.for_request(cls.stub.OnKlinesUpdate, api_pb2.FetchKlinesRequest,
                                                 symbol=cls.symbol,
                                                 interval=json.dumps(_interval)):
                 # print(f"on_klines_update: {candle.symbol}, {candle.interval}, candle: {json.loads(candle.candle)}")
                 _klines.get(candle.interval).refresh(json.loads(candle.candle))
-                if ms.MODE == 'TC':
+                if ms.MODE == 'TC' and (cls.strategy.start_collect or cls.strategy.start_collect is None):
                     new_raw = {int(time.time() * 1000): candle.candle}
                     cls.strategy.candles.setdefault(candle.interval, new_raw).update(new_raw)
         except Exception as ex:
             logger.warning(f"Exception on WSS, on_klines_update loop closed: {ex}")
             cls.wss_fire_up = True
     else:
         for i in _interval:
-            ds = pd.read_pickle(Path(BACKTEST_PATH, f"{ms.SYMBOL}_candles_{i}.pkl"))
+            ds = pd.read_pickle(Path(BACKTEST_PATH, f"{cls.exchange}_{cls.symbol}/raw/candles_{i}.pkl"))
             loop.create_task(aiter_candles(ds, _klines, i))
 
 
 async def aiter_candles(ds: pd.Series, _klines: {str: StrategyBase.Klines}, _i: str):
     async for row in loop_ds(ds):
         _klines.get(_i).refresh(json.loads(row))
     print(f"Backtest candles *** {_i} *** timeSeries ended")
@@ -905,15 +967,15 @@
         else:
             if res.success:
                 run = True
         await asyncio.sleep(HEARTBEAT)
     while run:
         try:
             res = await cls.send_request(cls.stub.CheckStream, api_pb2.MarketRequest, symbol=cls.symbol)
-            if not res.success:
+            if res is None or not res.success:
                 cls.wss_fire_up = True
                 raise UserWarning(f"Not active WSS for {cls.symbol} on {cls.exchange}, restart request sent")
             _orders = await cls.send_request(cls.stub.FetchOpenOrders, api_pb2.MarketRequest, symbol=cls.symbol)
             if _orders is None:
                 raise UserWarning("Can't fetch open orders")
             StrategyBase.rate_limiter = max(StrategyBase.rate_limiter, _orders.rate_limiter)
             orders = json_format.MessageToDict(_orders).get('items', [])
@@ -964,16 +1026,16 @@
                     cls.strategy.message_log("Trying restore saved state after restart", color=ms.Style.GREEN)
                 try:
                     last_state = {}
                     if cls.last_state:
                         last_state.update(cls.last_state)
                         cls.last_state = None
                         # Restore StrategyBase class var
-                        cls.order_id = (json.loads(last_state.pop(ms_order_id, 0)) or
-                                        int(ms.datetime.now().strftime("%S%M")) * 1000)
+                        cls.order_id = json.loads(last_state.pop(ms_order_id,
+                                                                 str(int(datetime.now().strftime("%S%M")) * 1000)))
                         cls.start_time_ms = json.loads(last_state.pop('ms_start_time_ms', str(int(time.time() * 1000))))
                         cls.trades = jsonpickle.decode(last_state.pop('ms_trades', '[]'))
                         cls.orders = jsonpickle.decode(last_state.pop(ms_orders, '[]'))
                     else:
                         last_state.pop(ms_order_id, None)
                         # last_state.pop('ms.trades', None)
                         last_state.pop(ms_orders, None)
@@ -1087,15 +1149,15 @@
     except Exception as ex:
         logger.warning(f"Exception on WSS, on_order_update loop closed: {ex}")
         cls.wss_fire_up = True
 
 
 def on_order_update_handler(cls, ed):
     if (cls.symbol == ed['symbol']
-            and cls.order_exist(ed['order_id'])
+            and cls.strategy.order_exist(ed['order_id'])
             and ed['order_status'] in ('FILLED', 'PARTIALLY_FILLED')):
         if ed['order_status'] == 'FILLED':
             # Remove from all_orders and orders lists
             remove_from_orders_lists([ed['order_id']])
         if trade_not_exist(ed['order_id'], ed['trade_id']):
             trade = {"qty": ed['last_executed_quantity'],
                      "isBuyer": bool(ed['side'] == 'BUY'),
@@ -1188,16 +1250,16 @@
                 cls.trades.append(PrivateTrade(trade))
                 if len(cls.all_trades) > ALL_TRADES_LIST_LIMIT:
                     del cls.all_trades[0]
                 cls.all_trades.append(PrivateTrade(trade))
             if executed_qty < orig_qty:
                 cls.orders.append(order)
                 cls.all_orders.append(order)
-            if ms.MODE == 'TC':
-                cls.open_orders_snapshot()
+            if ms.MODE == 'TC' and cls.strategy.start_collect:
+                cls.strategy.open_orders_snapshot()
             elif ms.MODE == 'S':
                 await on_funds_update()
             cls.strategy.on_place_order_success(_id, order)
 
 
 async def place_limit_order_timeout(_id):
     cls = StrategyBase
@@ -1235,16 +1297,16 @@
         # print(f"cancel_order_call.result: {result}")
         # Remove from all_orders and orders lists
         if result:
             remove_from_orders_lists([_id])
             cls.strategy.message_log(f"Cancel order {_id} success", color=ms.Style.GREEN)
             cls.strategy.on_cancel_order_success(_id, Order(result))
             cls.canceled_order_id.append(_id)
-            if ms.MODE == 'TC':
-                cls.open_orders_snapshot()
+            if ms.MODE == 'TC' and cls.strategy.start_collect:
+                cls.strategy.open_orders_snapshot()
             elif ms.MODE == 'S':
                 await on_funds_update()
 
 
 async def cancel_all_order_call(_id: int):
     cls = StrategyBase
     try:
@@ -1342,14 +1404,17 @@
     """
     Pandas time Series asynchronous generator with delay (real time/XTIME) multiplier
     :param tik: True - update local time
     :param ds: pandas time Series object
     :return: next row
     """
     cls = StrategyBase
+    while not cls.strategy.start_collect:
+        await asyncio.sleep(0.1)
+
     index_prev = 0
     for index, row in ds.items():
         delay = (index - index_prev) if index_prev else 0
         index_prev = index
         if tik:
             cls.strategy.time_operational['new'] = index / 1000
         await asyncio.sleep(delay / (1000 * ms.XTIME))
@@ -1370,16 +1435,16 @@
                               'closeTime': ticker.event_time}
                 cls.ticker = ticker_24h
                 cls.strategy.on_new_ticker(Ticker(cls.ticker))
                 #
                 if ms.MODE == 'TC' and cls.strategy.start_collect:
                     # print(f"on_ticker_update.ticker_24h: {ticker_24h}")
                     ticker_24h['delay'] = cls.delay_ordering_s
-                    cls.strategy.ticker.update({int(time.time() * 1000): ticker_24h})
-                    cls.open_orders_snapshot()
+                    cls.strategy.s_ticker.update({int(time.time() * 1000): ticker_24h})
+                    cls.strategy.open_orders_snapshot()
         except Exception as ex:
             logger.warning(f"Exception on WSS, on_ticker_update loop closed: {ex}")
             cls.wss_fire_up = True
     else:
         async for row in loop_ds(cls.backtest['ticker'], tik=True):
             cls.delay_ordering_s = row.pop('delay', 0)
             cls.ticker = row
@@ -1394,33 +1459,35 @@
 
 def back_test_handler(cls):
     # Test result handler
     test_time = datetime.utcnow() - cls.strategy.cycle_time
     original_time = (cls.backtest['ticker'].index.max() - cls.backtest['ticker'].index.min()) / 1000
     original_time = timedelta(seconds=original_time)
     print(f"Original time: {original_time}, test time: {test_time}, x = {original_time / test_time:.2f}")
-    # Save test data
-    session_path = Path(BACKTEST_PATH, f"{ms.SYMBOL}_{datetime.now().strftime('%m%d-%H:%M:%S')}")
-    session_path.mkdir(parents=True)
-    ds_ticker = pd.Series(cls.strategy.account.ticker).astype(float)
-    ds_ticker.index = pd.to_datetime(ds_ticker.index, unit='ms')
-    df_grid_sell = pd.DataFrame().from_dict(cls.strategy.account.grid_sell, orient='index').astype(float)
-    df_grid_sell.index = pd.to_datetime(df_grid_sell.index, unit='ms')
-    df_grid_buy = pd.DataFrame().from_dict(cls.strategy.account.grid_buy, orient='index').astype(float)
-    df_grid_buy.index = pd.to_datetime(df_grid_buy.index, unit='ms')
-    #
-    ds_ticker.to_pickle(Path(session_path, "ticker.pkl"))
-    df_grid_sell.to_pickle(Path(session_path, "sell.pkl"))
-    df_grid_buy.to_pickle(Path(session_path, "buy.pkl"))
-    copy(ms.PARAMS, Path(session_path, Path(ms.PARAMS).name))
-    #
+    if ms.SAVE_DS:
+        # Save test data
+        session_path = Path(BACKTEST_PATH,
+                            f"{cls.exchange}_{cls.symbol}_{datetime.now().strftime('%m%d-%H:%M:%S')}")
+        session_path.mkdir(parents=True)
+        ds_ticker = pd.Series(cls.strategy.account.ticker).astype(float)
+        ds_ticker.index = pd.to_datetime(ds_ticker.index, unit='ms')
+        df_grid_sell = pd.DataFrame().from_dict(cls.strategy.account.grid_sell, orient='index').astype(float)
+        df_grid_sell.index = pd.to_datetime(df_grid_sell.index, unit='ms')
+        df_grid_buy = pd.DataFrame().from_dict(cls.strategy.account.grid_buy, orient='index').astype(float)
+        df_grid_buy.index = pd.to_datetime(df_grid_buy.index, unit='ms')
+        #
+        ds_ticker.to_pickle(Path(session_path, "ticker.pkl"))
+        df_grid_sell.to_pickle(Path(session_path, "sell.pkl"))
+        df_grid_buy.to_pickle(Path(session_path, "buy.pkl"))
+        copy(ms.PARAMS, Path(session_path, Path(ms.PARAMS).name))
+        print(f"Session data saved to: {session_path}")
+        #
     s_profit = session_result['profit'] = f"{cls.strategy.get_sum_profit()}"
     s_free = session_result['free'] = f"{cls.strategy.get_free_assets(mode='free')[2]}"
     print(f"Session profit: {s_profit}, free: {s_free}, total: {float(s_profit) + float(s_free)}")
-    print(f"Session data saved to: {session_path}")
     loop.stop()
 
 
 def order_book_prepare(_order_book: {}) -> {}:
     order_book = json_format.MessageToDict(_order_book)
     order_book_bids = order_book.pop('bids', [])
     order_book_asks = order_book.pop('asks', [])
@@ -1442,15 +1509,15 @@
             async for _order_book in cls.for_request(cls.stub.OnOrderBookUpdate, api_pb2.MarketRequest,
                                                      symbol=cls.symbol):
                 order_book = order_book_prepare(_order_book)
                 # print(f"on_order_book_update.order_book: {order_book}")
                 cls.order_book = order_book
                 cls.strategy.on_new_order_book(OrderBook(cls.order_book))
                 if ms.MODE == 'TC' and cls.strategy.start_collect:
-                    cls.strategy.order_book.update({int(time.time() * 1000): order_book})
+                    cls.strategy.s_order_book.update({int(time.time() * 1000): order_book})
         except Exception as ex:
             logger.warning(f"Exception on WSS, on_order_book_update loop closed: {ex}")
             cls.wss_fire_up = True
     else:
         async for row in loop_ds(cls.backtest['order_book']):
             cls.order_book = row
             cls.strategy.on_new_order_book(OrderBook(cls.order_book))
@@ -1489,14 +1556,16 @@
     await buffered_candle()
     loop.create_task(on_order_book_update())
     if ms.MODE in ('T', 'TC'):
         # User Stream
         loop.create_task(on_funds_update())
         loop.create_task(on_order_update())
         loop.create_task(on_balance_update())
+        if ms.MODE =='TC':
+            loop.create_task(backtest_data_control())
 
 
 async def wss_init(update_max_queue_size=False):
     cls = StrategyBase
     cls.strategy.message_log(f"Init WSS, client_id: {cls.client_id}")
     if cls.client_id:
         await wss_declare()
@@ -1627,44 +1696,30 @@
                                                  symbol=_symbol)
                 cls.ticker = json_format.MessageToDict(_ticker)
                 # print(f"main.ticker: {cls.ticker}")
                 loop.create_task(save_asset())
         #
         else:
             # Init class atr for reuse in next backtest cycle
-            cls.ticker = {}
-            cls.funds = {}
-            cls.order_book = {}
-            cls.order_id = int(datetime.now().strftime("%S%M")) * 1000
-            cls.wait_order_id = []  # List of placed orders for time-out detect
-            cls.canceled_order_id = []  # List canceled orders  for time-out detect
-            cls.all_trades = []  # List of all (limit = ALL_TRADES_LIST_LIMIT) trades for a specific account and symbol
-            cls.trades = []  # List of trades associated with strategy (limit = TRADES_LIST_LIMIT)
-            cls.all_orders = []  # List of all open orders for symbol
-            cls.orders = []  # List orders associated with strategy
-            cls.get_buffered_funds_last_time = time.time()
-            cls.rate_limiter = RATE_LIMITER
-            cls.start_time_ms = int(time.time() * 1000)
-            cls.backtest = {}
-            cls.bulk_orders_cancel = {}
+            cls.reset_class_var()
 
         if ms.MODE == 'S':
-            cls.strategy.account = backTestAccount()
-            #
             cls.strategy.account.funds.base = {'asset': cls.base_asset,
                                                'free': f"{ms.AMOUNT_FIRST}",
                                                'locked': '0.0'}
             cls.strategy.account.funds.quote = {'asset': cls.quote_asset,
                                                 'free': f"{ms.AMOUNT_SECOND}",
                                                 'locked': '0.0'}
             cls.strategy.account.fee_maker = ms.FEE_MAKER
             cls.strategy.account.fee_taker = ms.FEE_TAKER
             #
-            cls.backtest['ticker'] = pd.read_pickle(Path(BACKTEST_PATH, f"{ms.SYMBOL}_ticker.pkl"))
-            cls.backtest['order_book'] = pd.read_pickle(Path(BACKTEST_PATH, f"{ms.SYMBOL}_order_book.pkl"))
+            cls.backtest['ticker'] = pd.read_pickle(Path(BACKTEST_PATH,
+                                                         f"{cls.exchange}_{cls.symbol}/raw/ticker.pkl"))
+            cls.backtest['order_book'] = pd.read_pickle(Path(BACKTEST_PATH,
+                                                             f"{cls.exchange}_{cls.symbol}/raw/order_book.pkl"))
             cls.ticker = cls.backtest['ticker'].iat[0]
             cls.order_book = cls.backtest['order_book'].iat[0]
         #
         await buffered_funds()
         answer = str()
         restored = True
         if restore_state:
```

### Comparing `martin-binance-1.3.0b18/martin_binance/ms_cfg.toml.template` & `martin-binance-1.3.0b21/martin_binance/ms_cfg.toml.template`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b18/martin_binance/service/funds_rate_exporter.py` & `martin-binance-1.3.0b21/martin_binance/service/funds_rate_exporter.py`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b18/martin_binance/service/grafana.json` & `martin-binance-1.3.0b21/martin_binance/service/grafana.json`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b18/martin_binance/service/relaunch.py` & `martin-binance-1.3.0b21/martin_binance/service/relaunch.py`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b18/pyproject.toml` & `martin-binance-1.3.0b21/pyproject.toml`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b18/uml/architecture.puml` & `martin-binance-1.3.0b21/uml/architecture.puml`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b18/PKG-INFO` & `martin-binance-1.3.0b21/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: martin-binance
-Version: 1.3.0b18
+Version: 1.3.0b21
 Summary: Free trading system for Binance SPOT API
 Author-email: Jerry Fedorenko <jerry.fedorenko@yahoo.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: martin-binance Version: 1.3.0b18 Summary: Free
+Metadata-Version: 2.1 Name: martin-binance Version: 1.3.0b21 Summary: Free
 trading system for Binance SPOT API Author-email: Jerry Fedorenko
 fedorenko@yahoo.com> Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Classifier: Programming Language :: Python :: 3 Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: Unix Classifier: Operating
 System :: Microsoft :: Windows Classifier: Operating System :: MacOS Requires-
 Dist: exchanges-wrapper==1.3.0.post1 Requires-Dist: margin-strategy-sdk==0.0.11
```

