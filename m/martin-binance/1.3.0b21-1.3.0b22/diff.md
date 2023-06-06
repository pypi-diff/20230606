# Comparing `tmp/martin-binance-1.3.0b21.tar.gz` & `tmp/martin-binance-1.3.0b22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "martin-binance-1.3.0b21.tar", last modified: Tue Jun  6 18:37:43 2023, max compression
+gzip compressed data, was "martin-binance-1.3.0b22.tar", last modified: Tue Jun  6 19:02:43 2023, max compression
```

## Comparing `martin-binance-1.3.0b21.tar` & `martin-binance-1.3.0b22.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0      154 2022-06-16 20:42:55.292826 martin-binance-1.3.0b21/.deepsource.toml
--rw-r--r--   0        0        0       79 2022-09-29 14:39:58.264847 martin-binance-1.3.0b21/.dockerignore
--rw-r--r--   0        0        0       68 2022-06-16 20:42:55.292826 martin-binance-1.3.0b21/.github/FUNDING.yml
--rw-r--r--   0        0        0      665 2022-09-29 14:39:58.268851 martin-binance-1.3.0b21/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      604 2022-09-29 14:39:58.268851 martin-binance-1.3.0b21/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      837 2023-01-08 14:15:30.514225 martin-binance-1.3.0b21/.github/workflows/codeql.yml
--rw-r--r--   0        0        0       45 2022-09-29 14:39:58.268851 martin-binance-1.3.0b21/.gitignore
--rwxr-xr-x   0        0        0    17691 2023-06-06 16:49:15.643997 martin-binance-1.3.0b21/CHANGELOG.md
--rw-r--r--   0        0        0      601 2022-11-24 16:46:07.400338 martin-binance-1.3.0b21/Dockerfile
--rw-r--r--   0        0        0     1079 2022-06-16 20:37:23.392898 martin-binance-1.3.0b21/LICENSE
--rwxr-xr-x   0        0        0    35437 2023-05-30 12:20:07.843798 martin-binance-1.3.0b21/README.md
--rwxr-xr-x   0        0        0    89295 2021-12-09 10:16:46.764494 martin-binance-1.3.0b21/doc/Create_strategy.png
--rwxr-xr-x   0        0        0    26452 2021-12-09 10:16:46.764494 martin-binance-1.3.0b21/doc/Model of logarithmic grid.ods
--rw-r--r--   0        0        0  5309091 2021-12-09 10:16:46.820491 martin-binance-1.3.0b21/doc/Modified martingale.svg
--rwxr-xr-x   0        0        0    79517 2021-12-09 10:16:46.824491 martin-binance-1.3.0b21/doc/graf1.png
--rwxr-xr-x   0        0        0    10318 2021-12-09 10:16:46.824491 martin-binance-1.3.0b21/doc/tlg_notify.png
--rwxr-xr-x   0        0        0     9332 2021-12-09 10:16:46.824491 martin-binance-1.3.0b21/doc/tmux.png
--rw-r--r--   0        0        0     2004 2023-06-05 20:18:03.227997 martin-binance-1.3.0b21/martin_binance/__init__.py
--rw-r--r--   0        0        0     2218 2023-06-05 19:37:24.375292 martin-binance-1.3.0b21/martin_binance/backtest/OoTSP.py
--rw-r--r--   0        0        0     2949 2023-06-03 09:17:19.879857 martin-binance-1.3.0b21/martin_binance/backtest/VCoSEL.py
--rw-r--r--   0        0        0        0 2023-06-01 20:26:31.871396 martin-binance-1.3.0b21/martin_binance/backtest/__init__.py
--rw-r--r--   0        0        0    12323 2023-06-04 14:26:32.096258 martin-binance-1.3.0b21/martin_binance/backtest/exchange_simulator.py
--rw-r--r--   0        0        0     6474 2023-06-01 20:26:31.871396 martin-binance-1.3.0b21/martin_binance/cli_0_BTCUSDT.py.template
--rw-r--r--   0        0        0     6469 2023-06-01 20:26:31.871396 martin-binance-1.3.0b21/martin_binance/cli_1_BTCUSDT.py.template
--rw-r--r--   0        0        0     6475 2023-06-01 20:26:31.871396 martin-binance-1.3.0b21/martin_binance/cli_2_TESTBTCTESTUSDT.py.template
--rw-r--r--   0        0        0     4710 2023-06-01 20:26:31.871396 martin-binance-1.3.0b21/martin_binance/client.py
--rw-r--r--   0        0        0   181583 2023-06-06 18:14:42.861974 martin-binance-1.3.0b21/martin_binance/executor.py
--rw-r--r--   0        0        0   237568 2022-09-29 14:39:58.276860 martin-binance-1.3.0b21/martin_binance/funds_rate.db.template
--rwxr-xr-x   0        0        0   337272 2022-09-29 14:39:58.276860 martin-binance-1.3.0b21/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so
--rw-r--r--   0        0        0      376 2022-12-19 14:10:45.443888 martin-binance-1.3.0b21/martin_binance/margin/margin_req.txt
--rw-r--r--   0        0        0      348 2023-01-08 14:15:30.514225 martin-binance-1.3.0b21/martin_binance/margin/margin_req_win.txt
--rw-r--r--   0        0        0    79598 2023-06-06 16:41:38.089871 martin-binance-1.3.0b21/martin_binance/margin_wrapper.py
--rw-r--r--   0        0        0     1472 2023-01-19 11:11:07.967695 martin-binance-1.3.0b21/martin_binance/ms_cfg.toml.template
--rw-r--r--   0        0        0      485 2021-12-09 09:06:56.984779 martin-binance-1.3.0b21/martin_binance/service/.tmux.conf
--rwxr-xr-x   0        0        0      319 2022-09-29 14:39:58.280864 martin-binance-1.3.0b21/martin_binance/service/funds_export.service
--rwxr-xr-x   0        0        0    16185 2023-05-30 12:20:07.847793 martin-binance-1.3.0b21/martin_binance/service/funds_rate_exporter.py
--rwxr-xr-x   0        0        0    75764 2023-05-30 12:20:07.847793 martin-binance-1.3.0b21/martin_binance/service/grafana.json
--rwxr-xr-x   0        0        0     1276 2022-09-29 14:39:58.280864 martin-binance-1.3.0b21/martin_binance/service/relaunch.py
--rwxr-xr-x   0        0        0      271 2022-09-29 14:39:58.284868 martin-binance-1.3.0b21/martin_binance/service/relaunch.service
--rwxr-xr-x   0        0        0      372 2021-12-09 09:06:56.984779 martin-binance-1.3.0b21/martin_binance/service/tmux.service
--rw-r--r--   0        0        0     1203 2023-06-03 20:53:44.166165 martin-binance-1.3.0b21/pyproject.toml
--rw-r--r--   0        0        0      320 2023-06-03 20:53:44.162164 martin-binance-1.3.0b21/requirements.txt
--rw-r--r--   0        0        0     2390 2023-01-19 11:11:07.971695 martin-binance-1.3.0b21/uml/architecture.puml
--rw-r--r--   0        0        0    36614 1970-01-01 00:00:00.000000 martin-binance-1.3.0b21/PKG-INFO
+-rw-r--r--   0        0        0      154 2022-06-16 20:42:55.292826 martin-binance-1.3.0b22/.deepsource.toml
+-rw-r--r--   0        0        0       79 2022-09-29 14:39:58.264847 martin-binance-1.3.0b22/.dockerignore
+-rw-r--r--   0        0        0       68 2022-06-16 20:42:55.292826 martin-binance-1.3.0b22/.github/FUNDING.yml
+-rw-r--r--   0        0        0      665 2022-09-29 14:39:58.268851 martin-binance-1.3.0b22/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      604 2022-09-29 14:39:58.268851 martin-binance-1.3.0b22/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      837 2023-01-08 14:15:30.514225 martin-binance-1.3.0b22/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0       45 2022-09-29 14:39:58.268851 martin-binance-1.3.0b22/.gitignore
+-rwxr-xr-x   0        0        0    17691 2023-06-06 16:49:15.643997 martin-binance-1.3.0b22/CHANGELOG.md
+-rw-r--r--   0        0        0      601 2022-11-24 16:46:07.400338 martin-binance-1.3.0b22/Dockerfile
+-rw-r--r--   0        0        0     1079 2022-06-16 20:37:23.392898 martin-binance-1.3.0b22/LICENSE
+-rwxr-xr-x   0        0        0    35437 2023-05-30 12:20:07.843798 martin-binance-1.3.0b22/README.md
+-rwxr-xr-x   0        0        0    89295 2021-12-09 10:16:46.764494 martin-binance-1.3.0b22/doc/Create_strategy.png
+-rwxr-xr-x   0        0        0    26452 2021-12-09 10:16:46.764494 martin-binance-1.3.0b22/doc/Model of logarithmic grid.ods
+-rw-r--r--   0        0        0  5309091 2021-12-09 10:16:46.820491 martin-binance-1.3.0b22/doc/Modified martingale.svg
+-rwxr-xr-x   0        0        0    79517 2021-12-09 10:16:46.824491 martin-binance-1.3.0b22/doc/graf1.png
+-rwxr-xr-x   0        0        0    10318 2021-12-09 10:16:46.824491 martin-binance-1.3.0b22/doc/tlg_notify.png
+-rwxr-xr-x   0        0        0     9332 2021-12-09 10:16:46.824491 martin-binance-1.3.0b22/doc/tmux.png
+-rw-r--r--   0        0        0     2004 2023-06-06 19:02:16.703877 martin-binance-1.3.0b22/martin_binance/__init__.py
+-rw-r--r--   0        0        0     2218 2023-06-05 19:37:24.375292 martin-binance-1.3.0b22/martin_binance/backtest/OoTSP.py
+-rw-r--r--   0        0        0     2949 2023-06-03 09:17:19.879857 martin-binance-1.3.0b22/martin_binance/backtest/VCoSEL.py
+-rw-r--r--   0        0        0        0 2023-06-01 20:26:31.871396 martin-binance-1.3.0b22/martin_binance/backtest/__init__.py
+-rw-r--r--   0        0        0    12323 2023-06-04 14:26:32.096258 martin-binance-1.3.0b22/martin_binance/backtest/exchange_simulator.py
+-rw-r--r--   0        0        0     6474 2023-06-01 20:26:31.871396 martin-binance-1.3.0b22/martin_binance/cli_0_BTCUSDT.py.template
+-rw-r--r--   0        0        0     6469 2023-06-01 20:26:31.871396 martin-binance-1.3.0b22/martin_binance/cli_1_BTCUSDT.py.template
+-rw-r--r--   0        0        0     6475 2023-06-01 20:26:31.871396 martin-binance-1.3.0b22/martin_binance/cli_2_TESTBTCTESTUSDT.py.template
+-rw-r--r--   0        0        0     4710 2023-06-01 20:26:31.871396 martin-binance-1.3.0b22/martin_binance/client.py
+-rw-r--r--   0        0        0   181595 2023-06-06 19:02:16.719858 martin-binance-1.3.0b22/martin_binance/executor.py
+-rw-r--r--   0        0        0   237568 2022-09-29 14:39:58.276860 martin-binance-1.3.0b22/martin_binance/funds_rate.db.template
+-rwxr-xr-x   0        0        0   337272 2022-09-29 14:39:58.276860 martin-binance-1.3.0b22/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so
+-rw-r--r--   0        0        0      376 2022-12-19 14:10:45.443888 martin-binance-1.3.0b22/martin_binance/margin/margin_req.txt
+-rw-r--r--   0        0        0      348 2023-01-08 14:15:30.514225 martin-binance-1.3.0b22/martin_binance/margin/margin_req_win.txt
+-rw-r--r--   0        0        0    79598 2023-06-06 16:41:38.089871 martin-binance-1.3.0b22/martin_binance/margin_wrapper.py
+-rw-r--r--   0        0        0     1472 2023-01-19 11:11:07.967695 martin-binance-1.3.0b22/martin_binance/ms_cfg.toml.template
+-rw-r--r--   0        0        0      485 2021-12-09 09:06:56.984779 martin-binance-1.3.0b22/martin_binance/service/.tmux.conf
+-rwxr-xr-x   0        0        0      319 2022-09-29 14:39:58.280864 martin-binance-1.3.0b22/martin_binance/service/funds_export.service
+-rwxr-xr-x   0        0        0    16185 2023-05-30 12:20:07.847793 martin-binance-1.3.0b22/martin_binance/service/funds_rate_exporter.py
+-rwxr-xr-x   0        0        0    75764 2023-05-30 12:20:07.847793 martin-binance-1.3.0b22/martin_binance/service/grafana.json
+-rwxr-xr-x   0        0        0     1276 2022-09-29 14:39:58.280864 martin-binance-1.3.0b22/martin_binance/service/relaunch.py
+-rwxr-xr-x   0        0        0      271 2022-09-29 14:39:58.284868 martin-binance-1.3.0b22/martin_binance/service/relaunch.service
+-rwxr-xr-x   0        0        0      372 2021-12-09 09:06:56.984779 martin-binance-1.3.0b22/martin_binance/service/tmux.service
+-rw-r--r--   0        0        0     1203 2023-06-03 20:53:44.166165 martin-binance-1.3.0b22/pyproject.toml
+-rw-r--r--   0        0        0      320 2023-06-03 20:53:44.162164 martin-binance-1.3.0b22/requirements.txt
+-rw-r--r--   0        0        0     2390 2023-01-19 11:11:07.971695 martin-binance-1.3.0b22/uml/architecture.puml
+-rw-r--r--   0        0        0    36614 1970-01-01 00:00:00.000000 martin-binance-1.3.0b22/PKG-INFO
```

### Comparing `martin-binance-1.3.0b21/.github/ISSUE_TEMPLATE/bug_report.md` & `martin-binance-1.3.0b22/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b21/.github/ISSUE_TEMPLATE/feature_request.md` & `martin-binance-1.3.0b22/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b21/.github/workflows/codeql.yml` & `martin-binance-1.3.0b22/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b21/CHANGELOG.md` & `martin-binance-1.3.0b22/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b21/Dockerfile` & `martin-binance-1.3.0b22/Dockerfile`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b21/LICENSE` & `martin-binance-1.3.0b22/LICENSE`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b21/README.md` & `martin-binance-1.3.0b22/README.md`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b21/doc/Create_strategy.png` & `martin-binance-1.3.0b22/doc/Create_strategy.png`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b21/doc/Model of logarithmic grid.ods` & `martin-binance-1.3.0b22/doc/Model of logarithmic grid.ods`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b21/doc/Modified martingale.svg` & `martin-binance-1.3.0b22/doc/Modified martingale.svg`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b21/doc/graf1.png` & `martin-binance-1.3.0b22/doc/graf1.png`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b21/doc/tlg_notify.png` & `martin-binance-1.3.0b22/doc/tlg_notify.png`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b21/doc/tmux.png` & `martin-binance-1.3.0b22/doc/tmux.png`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b21/martin_binance/__init__.py` & `martin-binance-1.3.0b22/martin_binance/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 """
 Free trading system for Binance SPOT API
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.0b21"
+__version__ = "1.3.0b22"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 from pathlib import Path
 from shutil import copy
 #
 import platform
```

### Comparing `martin-binance-1.3.0b21/martin_binance/backtest/OoTSP.py` & `martin-binance-1.3.0b22/martin_binance/backtest/OoTSP.py`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b21/martin_binance/backtest/VCoSEL.py` & `martin-binance-1.3.0b22/martin_binance/backtest/VCoSEL.py`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b21/martin_binance/backtest/exchange_simulator.py` & `martin-binance-1.3.0b22/martin_binance/backtest/exchange_simulator.py`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b21/martin_binance/cli_0_BTCUSDT.py.template` & `martin-binance-1.3.0b22/martin_binance/cli_0_BTCUSDT.py.template`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b21/martin_binance/cli_1_BTCUSDT.py.template` & `martin-binance-1.3.0b22/martin_binance/cli_1_BTCUSDT.py.template`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b21/martin_binance/cli_2_TESTBTCTESTUSDT.py.template` & `martin-binance-1.3.0b22/martin_binance/cli_2_TESTBTCTESTUSDT.py.template`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b21/martin_binance/client.py` & `martin-binance-1.3.0b22/martin_binance/client.py`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b21/martin_binance/executor.py` & `martin-binance-1.3.0b22/martin_binance/executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ####################################################################
 # Cyclic grid strategy based on martingale
 ##################################################################
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.3.0b20"
+__version__ = "1.3.0b22"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = 'https://github.com/DogsTailFarmer'
 ##################################################################
 import sys
 import gc
 import statistics
 from decimal import Decimal, ROUND_FLOOR, ROUND_CEILING
@@ -1062,16 +1062,17 @@
             self.message_log("restore_strategy_state from saved state:", log_level=LogLevel.DEBUG)
             self.message_log("\n".join(f"{k}\t{v}" for k, v in strategy_state.items()), log_level=LogLevel.DEBUG)
             #
             self.command = json.loads(strategy_state.get('command'))
             self.cycle_buy = json.loads(strategy_state.get('cycle_buy'))
             self.cycle_buy_count = json.loads(strategy_state.get('cycle_buy_count'))
             self.cycle_sell_count = json.loads(strategy_state.get('cycle_sell_count'))
-            self.cycle_time = json.loads(strategy_state.get('cycle_time', str(datetime.utcnow())))
-            self.cycle_time = datetime.strptime(self.cycle_time, '%Y-%m-%d %H:%M:%S.%f')
+            self.cycle_time = json.loads(strategy_state.get('cycle_time'))
+            if self.cycle_time:
+                self.cycle_time = datetime.strptime(self.cycle_time, '%Y-%m-%d %H:%M:%S.%f')
             self.cycle_time_reverse = json.loads(strategy_state.get('cycle_time_reverse'))
             if self.cycle_time_reverse:
                 self.cycle_time_reverse = datetime.strptime(self.cycle_time_reverse, '%Y-%m-%d %H:%M:%S.%f')
             self.deposit_first = f2d(json.loads(strategy_state.get('deposit_first')))
             self.deposit_second = f2d(json.loads(strategy_state.get('deposit_second')))
             self.last_shift_time = json.loads(strategy_state.get('last_shift_time')) or self.local_time()
             self.martin = f2d(json.loads(strategy_state.get('martin')))
```

### Comparing `martin-binance-1.3.0b21/martin_binance/funds_rate.db.template` & `martin-binance-1.3.0b22/martin_binance/funds_rate.db.template`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b21/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so` & `martin-binance-1.3.0b22/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b21/martin_binance/margin_wrapper.py` & `martin-binance-1.3.0b22/martin_binance/margin_wrapper.py`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b21/martin_binance/ms_cfg.toml.template` & `martin-binance-1.3.0b22/martin_binance/ms_cfg.toml.template`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b21/martin_binance/service/funds_rate_exporter.py` & `martin-binance-1.3.0b22/martin_binance/service/funds_rate_exporter.py`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b21/martin_binance/service/grafana.json` & `martin-binance-1.3.0b22/martin_binance/service/grafana.json`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b21/martin_binance/service/relaunch.py` & `martin-binance-1.3.0b22/martin_binance/service/relaunch.py`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b21/pyproject.toml` & `martin-binance-1.3.0b22/pyproject.toml`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b21/uml/architecture.puml` & `martin-binance-1.3.0b22/uml/architecture.puml`

 * *Files identical despite different names*

### Comparing `martin-binance-1.3.0b21/PKG-INFO` & `martin-binance-1.3.0b22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: martin-binance
-Version: 1.3.0b21
+Version: 1.3.0b22
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
-Metadata-Version: 2.1 Name: martin-binance Version: 1.3.0b21 Summary: Free
+Metadata-Version: 2.1 Name: martin-binance Version: 1.3.0b22 Summary: Free
 trading system for Binance SPOT API Author-email: Jerry Fedorenko
 fedorenko@yahoo.com> Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Classifier: Programming Language :: Python :: 3 Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: Unix Classifier: Operating
 System :: Microsoft :: Windows Classifier: Operating System :: MacOS Requires-
 Dist: exchanges-wrapper==1.3.0.post1 Requires-Dist: margin-strategy-sdk==0.0.11
```

