# Comparing `tmp/backtestify-0.1.1.tar.gz` & `tmp/backtestify-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\backtestify-0.1.1.tar", last modified: Mon May 29 00:16:43 2023, max compression
+gzip compressed data, was "backtestify-0.1.2.tar", last modified: Tue Jun  6 16:01:41 2023, max compression
```

## Comparing `backtestify-0.1.1.tar` & `backtestify-0.1.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 00:16:43.000000 backtestify-0.1.1/
--rw-rw-rw-   0        0        0    11558 2023-05-19 19:02:52.000000 backtestify-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      409 2023-05-29 00:16:43.000000 backtestify-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-05-19 19:02:52.000000 backtestify-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 00:16:43.000000 backtestify-0.1.1/backtestify/
--rw-rw-rw-   0        0        0     1362 2023-05-28 18:33:09.000000 backtestify-0.1.1/backtestify/__init__.py
--rw-rw-rw-   0        0        0      142 2023-05-19 19:02:52.000000 backtestify-0.1.1/backtestify/account.py
--rw-rw-rw-   0        0        0     2503 2023-05-28 23:36:45.000000 backtestify-0.1.1/backtestify/backtester.py
--rw-rw-rw-   0        0        0      696 2023-05-28 19:31:49.000000 backtestify-0.1.1/backtestify/cfd.py
--rw-rw-rw-   0        0        0     1931 2023-05-19 19:02:52.000000 backtestify-0.1.1/backtestify/event.py
--rw-rw-rw-   0        0        0      296 2023-05-19 19:02:52.000000 backtestify-0.1.1/backtestify/event_execution_context.py
--rw-rw-rw-   0        0        0      498 2023-05-19 19:02:52.000000 backtestify-0.1.1/backtestify/event_execution_strategy.py
--rw-rw-rw-   0        0        0       74 2023-05-19 19:02:52.000000 backtestify-0.1.1/backtestify/event_type.py
--rw-rw-rw-   0        0        0      431 2023-05-19 19:02:52.000000 backtestify-0.1.1/backtestify/financial_instrument.py
--rw-rw-rw-   0        0        0       98 2023-05-19 19:02:52.000000 backtestify-0.1.1/backtestify/instrument_type.py
--rw-rw-rw-   0        0        0    10196 2023-05-29 00:05:22.000000 backtestify-0.1.1/backtestify/signal_event.py
--rw-rw-rw-   0        0        0      160 2023-05-19 23:36:19.000000 backtestify-0.1.1/backtestify/signal_type.py
--rw-rw-rw-   0        0        0     4822 2023-05-28 22:45:19.000000 backtestify-0.1.1/backtestify/strategy.py
--rw-rw-rw-   0        0        0      494 2023-05-23 03:39:36.000000 backtestify-0.1.1/backtestify/trade.py
--rw-rw-rw-   0        0        0    11120 2023-05-28 18:37:46.000000 backtestify-0.1.1/backtestify/trade_executor.py
--rw-rw-rw-   0        0        0     2872 2023-05-28 23:20:05.000000 backtestify-0.1.1/backtestify/trade_state.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:16:43.000000 backtestify-0.1.1/backtestify.egg-info/
--rw-rw-rw-   0        0        0      409 2023-05-29 00:16:43.000000 backtestify-0.1.1/backtestify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      642 2023-05-29 00:16:43.000000 backtestify-0.1.1/backtestify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 00:16:43.000000 backtestify-0.1.1/backtestify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-29 00:16:43.000000 backtestify-0.1.1/backtestify.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-29 00:16:43.000000 backtestify-0.1.1/backtestify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 00:16:43.000000 backtestify-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      662 2023-05-29 00:15:02.000000 backtestify-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:01:41.567894 backtestify-0.1.2/
+-rw-rw-rw-   0        0        0    11558 2023-05-19 19:02:52.000000 backtestify-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      409 2023-06-06 16:01:41.566893 backtestify-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-05-19 19:02:52.000000 backtestify-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 16:01:41.559749 backtestify-0.1.2/backtestify/
+-rw-rw-rw-   0        0        0     1362 2023-05-28 18:33:09.000000 backtestify-0.1.2/backtestify/__init__.py
+-rw-rw-rw-   0        0        0      142 2023-05-19 19:02:52.000000 backtestify-0.1.2/backtestify/account.py
+-rw-rw-rw-   0        0        0     2764 2023-06-05 18:49:46.000000 backtestify-0.1.2/backtestify/backtester.py
+-rw-rw-rw-   0        0        0      696 2023-05-28 19:31:49.000000 backtestify-0.1.2/backtestify/cfd.py
+-rw-rw-rw-   0        0        0     1931 2023-05-19 19:02:52.000000 backtestify-0.1.2/backtestify/event.py
+-rw-rw-rw-   0        0        0      296 2023-05-19 19:02:52.000000 backtestify-0.1.2/backtestify/event_execution_context.py
+-rw-rw-rw-   0        0        0      498 2023-05-19 19:02:52.000000 backtestify-0.1.2/backtestify/event_execution_strategy.py
+-rw-rw-rw-   0        0        0       74 2023-05-19 19:02:52.000000 backtestify-0.1.2/backtestify/event_type.py
+-rw-rw-rw-   0        0        0      431 2023-05-19 19:02:52.000000 backtestify-0.1.2/backtestify/financial_instrument.py
+-rw-rw-rw-   0        0        0       98 2023-05-19 19:02:52.000000 backtestify-0.1.2/backtestify/instrument_type.py
+-rw-rw-rw-   0        0        0    10196 2023-05-29 00:05:22.000000 backtestify-0.1.2/backtestify/signal_event.py
+-rw-rw-rw-   0        0        0      160 2023-05-19 23:36:19.000000 backtestify-0.1.2/backtestify/signal_type.py
+-rw-rw-rw-   0        0        0     4802 2023-06-05 18:57:27.000000 backtestify-0.1.2/backtestify/strategy.py
+-rw-rw-rw-   0        0        0      494 2023-05-23 03:39:36.000000 backtestify-0.1.2/backtestify/trade.py
+-rw-rw-rw-   0        0        0    11125 2023-06-05 18:52:19.000000 backtestify-0.1.2/backtestify/trade_executor.py
+-rw-rw-rw-   0        0        0     2872 2023-05-28 23:20:05.000000 backtestify-0.1.2/backtestify/trade_state.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:01:41.565891 backtestify-0.1.2/backtestify.egg-info/
+-rw-rw-rw-   0        0        0      409 2023-06-06 16:01:41.000000 backtestify-0.1.2/backtestify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      642 2023-06-06 16:01:41.000000 backtestify-0.1.2/backtestify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 16:01:41.000000 backtestify-0.1.2/backtestify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-06 16:01:41.000000 backtestify-0.1.2/backtestify.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-06 16:01:41.000000 backtestify-0.1.2/backtestify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 16:01:41.567894 backtestify-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      662 2023-06-06 15:57:33.000000 backtestify-0.1.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `backtestify-0.1.1/LICENSE` & `backtestify-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `backtestify-0.1.1/backtestify/__init__.py` & `backtestify-0.1.2/backtestify/__init__.py`

 * *Files identical despite different names*

### Comparing `backtestify-0.1.1/backtestify/backtester.py` & `backtestify-0.1.2/backtestify/backtester.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+import pandas as pd
+
 from backtestify.trade_state import TradeState
 from backtestify.event_execution_context import EventExecutionContext
 from backtestify.event_execution_strategy import SignalEventExecutionStrategy
 from backtestify.signal_event import SignalEvent
 from backtestify.trade import Trade
 
+
 class Backtester:
     def __init__(self, strategy, instrument, account):
         self.strategy = strategy
         self.instrument = instrument
         self.account = account
         self.events = []
         self.trading_state = []
@@ -59,8 +62,16 @@
         for res in response:
             if isinstance(res, TradeState):
                 self.trading_state[current_bar] = res
                 self.current_trade_state = res
             elif isinstance(res, Trade):
                 self.trades.append(res)
 
+    @property
+    def results(self):
+        trades = []
+
+        for trade in self.trades:
+            trades.append(trade.__dict__)
 
+        df_trades = pd.DataFrame(trades)
+        df_trades = df_trades.set_index('timestamp')
```

### Comparing `backtestify-0.1.1/backtestify/cfd.py` & `backtestify-0.1.2/backtestify/cfd.py`

 * *Files identical despite different names*

### Comparing `backtestify-0.1.1/backtestify/event.py` & `backtestify-0.1.2/backtestify/event.py`

 * *Files identical despite different names*

### Comparing `backtestify-0.1.1/backtestify/signal_event.py` & `backtestify-0.1.2/backtestify/signal_event.py`

 * *Files identical despite different names*

### Comparing `backtestify-0.1.1/backtestify/strategy.py` & `backtestify-0.1.2/backtestify/strategy.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,22 +90,22 @@
             self.set_ohlcv(signal)
             self.set_timestamp_if_none(signal)
             self.set_swap_info_if_none(signal)
             self.set_symbol_if_none(signal)
             self.set_previous_event(signal)
             self.set_bar_index(signal)
 
-    def apply_strategy(self, next_candle):
+    def apply_strategy(self, on_tick):
         # Save the amount of size of the prices_info
         prices_info_size = len(self.prices_info)
 
         for index, _ in enumerate(self.prices_info.itertuples()):
             self.current_index = index
             history = self.get_past_info(shift=1)
-            result_events = next_candle(history)
+            result_events = on_tick(history)
 
             # Create initial event to open the first trade
             initial_event = SignalEvent(signal=None) if index == 0 else None
 
             # Create last event to close the last trade
             last_event = SignalEvent(signal=SignalType.EXIT) if index == prices_info_size - 1 else None
 
@@ -122,12 +122,12 @@
 
             self.set_information(result_events)
             self.events.extend(result_events)
 
         return self.events
 
     def generate_signals(self):
-        if not hasattr(self, "next_candle"):
-            raise NotImplementedError("Subclasses should implement a next_candle method.")
+        if not hasattr(self, "on_tick"):
+            raise NotImplementedError("Subclasses should implement a on_tick method.")
         
-        events = self.apply_strategy(self.next_candle)
+        events = self.apply_strategy(self.on_tick)
         return events
```

### Comparing `backtestify-0.1.1/backtestify/trade_executor.py` & `backtestify-0.1.2/backtestify/trade_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
         
         trade = Trade(
             timestamp=self.timestamp,
             bar=self.current_bar,
             signal=event_signal,
             size=position_size * (1 if event_signal == SignalType.BUY else -1),
             price=trade_state.adjusted_price,
-            profit=0,
+            profit=profit,
             balance=trade_state.balance,
             stop_loss=trade_state.stop_loss,
             take_profit=trade_state.take_profit
         )
 
         return trade
```

### Comparing `backtestify-0.1.1/backtestify/trade_state.py` & `backtestify-0.1.2/backtestify/trade_state.py`

 * *Files identical despite different names*

### Comparing `backtestify-0.1.1/backtestify.egg-info/SOURCES.txt` & `backtestify-0.1.2/backtestify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backtestify-0.1.1/setup.py` & `backtestify-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as file:
     more_description = file.read()
 
 setuptools.setup(
     name="backtestify",
-    version="0.1.1",
+    version="0.1.2",
     author="Eladio Rocha Vizcaino",
     author_email="eladio.rocha99@gmail.com",
     description="A package for backtesting trading strategies",
     more_description=more_description,
     long_description_content_type="text/markdown",
     url="https://github.com/EladioRocha/backtestify",
     project_urls={
```

