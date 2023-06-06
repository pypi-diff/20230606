# Comparing `tmp/backtestify-0.1.5.tar.gz` & `tmp/backtestify-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backtestify-0.1.5.tar", last modified: Tue Jun  6 17:05:09 2023, max compression
+gzip compressed data, was "backtestify-0.1.6.tar", last modified: Tue Jun  6 17:27:47 2023, max compression
```

## Comparing `backtestify-0.1.5.tar` & `backtestify-0.1.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 17:05:09.870827 backtestify-0.1.5/
--rw-rw-rw-   0        0        0    11558 2023-05-19 19:02:52.000000 backtestify-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     4842 2023-06-06 17:05:09.869827 backtestify-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     4429 2023-06-06 16:56:06.000000 backtestify-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 17:05:09.864313 backtestify-0.1.5/backtestify/
--rw-rw-rw-   0        0        0     1362 2023-05-28 18:33:09.000000 backtestify-0.1.5/backtestify/__init__.py
--rw-rw-rw-   0        0        0      142 2023-05-19 19:02:52.000000 backtestify-0.1.5/backtestify/account.py
--rw-rw-rw-   0        0        0     2792 2023-06-06 16:32:31.000000 backtestify-0.1.5/backtestify/backtester.py
--rw-rw-rw-   0        0        0      696 2023-05-28 19:31:49.000000 backtestify-0.1.5/backtestify/cfd.py
--rw-rw-rw-   0        0        0     1931 2023-05-19 19:02:52.000000 backtestify-0.1.5/backtestify/event.py
--rw-rw-rw-   0        0        0      296 2023-05-19 19:02:52.000000 backtestify-0.1.5/backtestify/event_execution_context.py
--rw-rw-rw-   0        0        0      498 2023-05-19 19:02:52.000000 backtestify-0.1.5/backtestify/event_execution_strategy.py
--rw-rw-rw-   0        0        0       74 2023-05-19 19:02:52.000000 backtestify-0.1.5/backtestify/event_type.py
--rw-rw-rw-   0        0        0      431 2023-05-19 19:02:52.000000 backtestify-0.1.5/backtestify/financial_instrument.py
--rw-rw-rw-   0        0        0       98 2023-05-19 19:02:52.000000 backtestify-0.1.5/backtestify/instrument_type.py
--rw-rw-rw-   0        0        0    10196 2023-05-29 00:05:22.000000 backtestify-0.1.5/backtestify/signal_event.py
--rw-rw-rw-   0        0        0      160 2023-05-19 23:36:19.000000 backtestify-0.1.5/backtestify/signal_type.py
--rw-rw-rw-   0        0        0     4802 2023-06-05 18:57:27.000000 backtestify-0.1.5/backtestify/strategy.py
--rw-rw-rw-   0        0        0      494 2023-05-23 03:39:36.000000 backtestify-0.1.5/backtestify/trade.py
--rw-rw-rw-   0        0        0    11125 2023-06-05 18:52:19.000000 backtestify-0.1.5/backtestify/trade_executor.py
--rw-rw-rw-   0        0        0     2872 2023-05-28 23:20:05.000000 backtestify-0.1.5/backtestify/trade_state.py
-drwxrwxrwx   0        0        0        0 2023-06-06 17:05:09.868828 backtestify-0.1.5/backtestify.egg-info/
--rw-rw-rw-   0        0        0     4842 2023-06-06 17:05:09.000000 backtestify-0.1.5/backtestify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      642 2023-06-06 17:05:09.000000 backtestify-0.1.5/backtestify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 17:05:09.000000 backtestify-0.1.5/backtestify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-06 17:05:09.000000 backtestify-0.1.5/backtestify.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-06 17:05:09.000000 backtestify-0.1.5/backtestify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 17:05:09.870827 backtestify-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      642 2023-06-06 17:04:19.000000 backtestify-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 17:27:47.130602 backtestify-0.1.6/
+-rw-rw-rw-   0        0        0    11558 2023-05-19 19:02:52.000000 backtestify-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     4842 2023-06-06 17:27:47.129579 backtestify-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4429 2023-06-06 16:56:06.000000 backtestify-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 17:27:47.123613 backtestify-0.1.6/backtestify/
+-rw-rw-rw-   0        0        0     1362 2023-05-28 18:33:09.000000 backtestify-0.1.6/backtestify/__init__.py
+-rw-rw-rw-   0        0        0      278 2023-06-06 17:22:21.000000 backtestify-0.1.6/backtestify/account.py
+-rw-rw-rw-   0        0        0     2900 2023-06-06 17:23:12.000000 backtestify-0.1.6/backtestify/backtester.py
+-rw-rw-rw-   0        0        0      696 2023-05-28 19:31:49.000000 backtestify-0.1.6/backtestify/cfd.py
+-rw-rw-rw-   0        0        0     1931 2023-05-19 19:02:52.000000 backtestify-0.1.6/backtestify/event.py
+-rw-rw-rw-   0        0        0      296 2023-06-06 17:22:43.000000 backtestify-0.1.6/backtestify/event_execution_context.py
+-rw-rw-rw-   0        0        0      498 2023-06-06 17:22:39.000000 backtestify-0.1.6/backtestify/event_execution_strategy.py
+-rw-rw-rw-   0        0        0       74 2023-05-19 19:02:52.000000 backtestify-0.1.6/backtestify/event_type.py
+-rw-rw-rw-   0        0        0      431 2023-05-19 19:02:52.000000 backtestify-0.1.6/backtestify/financial_instrument.py
+-rw-rw-rw-   0        0        0       98 2023-05-19 19:02:52.000000 backtestify-0.1.6/backtestify/instrument_type.py
+-rw-rw-rw-   0        0        0    10202 2023-06-06 17:26:29.000000 backtestify-0.1.6/backtestify/signal_event.py
+-rw-rw-rw-   0        0        0      160 2023-05-19 23:36:19.000000 backtestify-0.1.6/backtestify/signal_type.py
+-rw-rw-rw-   0        0        0     4802 2023-06-05 18:57:27.000000 backtestify-0.1.6/backtestify/strategy.py
+-rw-rw-rw-   0        0        0      494 2023-06-06 17:11:07.000000 backtestify-0.1.6/backtestify/trade.py
+-rw-rw-rw-   0        0        0    11125 2023-06-05 18:52:19.000000 backtestify-0.1.6/backtestify/trade_executor.py
+-rw-rw-rw-   0        0        0     2872 2023-05-28 23:20:05.000000 backtestify-0.1.6/backtestify/trade_state.py
+drwxrwxrwx   0        0        0        0 2023-06-06 17:27:47.129053 backtestify-0.1.6/backtestify.egg-info/
+-rw-rw-rw-   0        0        0     4842 2023-06-06 17:27:46.000000 backtestify-0.1.6/backtestify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      642 2023-06-06 17:27:47.000000 backtestify-0.1.6/backtestify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 17:27:46.000000 backtestify-0.1.6/backtestify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-06 17:27:46.000000 backtestify-0.1.6/backtestify.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-06 17:27:46.000000 backtestify-0.1.6/backtestify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 17:27:47.130602 backtestify-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      642 2023-06-06 17:27:03.000000 backtestify-0.1.6/setup.py
```

### Comparing `backtestify-0.1.5/LICENSE` & `backtestify-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `backtestify-0.1.5/PKG-INFO` & `backtestify-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backtestify
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package for backtesting trading strategies
 Home-page: https://github.com/EladioRocha/backtestify
 Author: Eladio Rocha Vizcaino
 Author-email: eladio.rocha99@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/EladioRocha/backtestify/issues
 Description-Content-Type: text/markdown
```

### Comparing `backtestify-0.1.5/README.md` & `backtestify-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `backtestify-0.1.5/backtestify/__init__.py` & `backtestify-0.1.6/backtestify/__init__.py`

 * *Files identical despite different names*

### Comparing `backtestify-0.1.5/backtestify/backtester.py` & `backtestify-0.1.6/backtestify/backtester.py`

 * *Files 10% similar despite different names*

```diff
@@ -59,14 +59,16 @@
         if not isinstance(response, (list, tuple)):
             response = [response]
 
         for res in response:
             if isinstance(res, TradeState):
                 self.trading_state[current_bar] = res
                 self.current_trade_state = res
+                self.account.set_equity(res.equity)
+                self.account.set_balance(res.balance)
             elif isinstance(res, Trade):
                 self.trades.append(res)
 
     @property
     def results(self):
         trades = []
```

### Comparing `backtestify-0.1.5/backtestify/cfd.py` & `backtestify-0.1.6/backtestify/cfd.py`

 * *Files identical despite different names*

### Comparing `backtestify-0.1.5/backtestify/event.py` & `backtestify-0.1.6/backtestify/event.py`

 * *Files identical despite different names*

### Comparing `backtestify-0.1.5/backtestify/signal_event.py` & `backtestify-0.1.6/backtestify/signal_event.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,22 +186,22 @@
         return stop_loss * pips if use_stop_loss else 0
 
     def update_unrealized_profit(self, trade_state, instrument, close_price):
         if trade_state.signal is None:
             return trade_state
         
         current_close_price = close_price + (instrument.spread_points if trade_state.signal == SignalType.SELL else 0)
-        floating_profit = (
+        unrealized_profit = (
             instrument.position_size
             * (current_close_price - trade_state.adjusted_price if trade_state.signal == SignalType.BUY else trade_state.adjusted_price - current_close_price)
             * instrument.point_value
             * instrument.currency_ratio
         )
-        trade_state.unrealized_profit = floating_profit
-        trade_state.equity = trade_state.balance + floating_profit
+        trade_state.unrealized_profit = unrealized_profit
+        trade_state.equity = trade_state.balance + unrealized_profit
 
         return trade_state
 
     def __str__(self):
         return "Event: %s, Timestamp: %s, Symbol: %s, Signal: %s, Take Profit: %s, Stop Loss: %s" % (self.event_type, self.timestamp, self.symbol, self.signal, self.take_profit, self.stop_loss)
 
     def __repr__(self):
```

### Comparing `backtestify-0.1.5/backtestify/strategy.py` & `backtestify-0.1.6/backtestify/strategy.py`

 * *Files identical despite different names*

### Comparing `backtestify-0.1.5/backtestify/trade_executor.py` & `backtestify-0.1.6/backtestify/trade_executor.py`

 * *Files identical despite different names*

### Comparing `backtestify-0.1.5/backtestify/trade_state.py` & `backtestify-0.1.6/backtestify/trade_state.py`

 * *Files identical despite different names*

### Comparing `backtestify-0.1.5/backtestify.egg-info/PKG-INFO` & `backtestify-0.1.6/backtestify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backtestify
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package for backtesting trading strategies
 Home-page: https://github.com/EladioRocha/backtestify
 Author: Eladio Rocha Vizcaino
 Author-email: eladio.rocha99@gmail.com
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/EladioRocha/backtestify/issues
 Description-Content-Type: text/markdown
```

### Comparing `backtestify-0.1.5/backtestify.egg-info/SOURCES.txt` & `backtestify-0.1.6/backtestify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backtestify-0.1.5/setup.py` & `backtestify-0.1.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as file:
     readme = file.read()
 
 setuptools.setup(
     name="backtestify",
-    version="0.1.5",
+    version="0.1.6",
     author="Eladio Rocha Vizcaino",
     author_email="eladio.rocha99@gmail.com",
     description="A package for backtesting trading strategies",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/EladioRocha/backtestify",
     project_urls={
```

