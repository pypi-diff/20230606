# Comparing `tmp/backtestify-0.1.2.tar.gz` & `tmp/backtestify-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backtestify-0.1.2.tar", last modified: Tue Jun  6 16:01:41 2023, max compression
+gzip compressed data, was "backtestify-0.1.3.tar", last modified: Tue Jun  6 16:35:09 2023, max compression
```

## Comparing `backtestify-0.1.2.tar` & `backtestify-0.1.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 16:01:41.567894 backtestify-0.1.2/
--rw-rw-rw-   0        0        0    11558 2023-05-19 19:02:52.000000 backtestify-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      409 2023-06-06 16:01:41.566893 backtestify-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-05-19 19:02:52.000000 backtestify-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 16:01:41.559749 backtestify-0.1.2/backtestify/
--rw-rw-rw-   0        0        0     1362 2023-05-28 18:33:09.000000 backtestify-0.1.2/backtestify/__init__.py
--rw-rw-rw-   0        0        0      142 2023-05-19 19:02:52.000000 backtestify-0.1.2/backtestify/account.py
--rw-rw-rw-   0        0        0     2764 2023-06-05 18:49:46.000000 backtestify-0.1.2/backtestify/backtester.py
--rw-rw-rw-   0        0        0      696 2023-05-28 19:31:49.000000 backtestify-0.1.2/backtestify/cfd.py
--rw-rw-rw-   0        0        0     1931 2023-05-19 19:02:52.000000 backtestify-0.1.2/backtestify/event.py
--rw-rw-rw-   0        0        0      296 2023-05-19 19:02:52.000000 backtestify-0.1.2/backtestify/event_execution_context.py
--rw-rw-rw-   0        0        0      498 2023-05-19 19:02:52.000000 backtestify-0.1.2/backtestify/event_execution_strategy.py
--rw-rw-rw-   0        0        0       74 2023-05-19 19:02:52.000000 backtestify-0.1.2/backtestify/event_type.py
--rw-rw-rw-   0        0        0      431 2023-05-19 19:02:52.000000 backtestify-0.1.2/backtestify/financial_instrument.py
--rw-rw-rw-   0        0        0       98 2023-05-19 19:02:52.000000 backtestify-0.1.2/backtestify/instrument_type.py
--rw-rw-rw-   0        0        0    10196 2023-05-29 00:05:22.000000 backtestify-0.1.2/backtestify/signal_event.py
--rw-rw-rw-   0        0        0      160 2023-05-19 23:36:19.000000 backtestify-0.1.2/backtestify/signal_type.py
--rw-rw-rw-   0        0        0     4802 2023-06-05 18:57:27.000000 backtestify-0.1.2/backtestify/strategy.py
--rw-rw-rw-   0        0        0      494 2023-05-23 03:39:36.000000 backtestify-0.1.2/backtestify/trade.py
--rw-rw-rw-   0        0        0    11125 2023-06-05 18:52:19.000000 backtestify-0.1.2/backtestify/trade_executor.py
--rw-rw-rw-   0        0        0     2872 2023-05-28 23:20:05.000000 backtestify-0.1.2/backtestify/trade_state.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:01:41.565891 backtestify-0.1.2/backtestify.egg-info/
--rw-rw-rw-   0        0        0      409 2023-06-06 16:01:41.000000 backtestify-0.1.2/backtestify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      642 2023-06-06 16:01:41.000000 backtestify-0.1.2/backtestify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 16:01:41.000000 backtestify-0.1.2/backtestify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-06 16:01:41.000000 backtestify-0.1.2/backtestify.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-06 16:01:41.000000 backtestify-0.1.2/backtestify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 16:01:41.567894 backtestify-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      662 2023-06-06 15:57:33.000000 backtestify-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:35:09.404052 backtestify-0.1.3/
+-rw-rw-rw-   0        0        0    11558 2023-05-19 19:02:52.000000 backtestify-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      409 2023-06-06 16:35:09.403056 backtestify-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1499 2023-06-06 16:20:35.000000 backtestify-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 16:35:09.397536 backtestify-0.1.3/backtestify/
+-rw-rw-rw-   0        0        0     1362 2023-05-28 18:33:09.000000 backtestify-0.1.3/backtestify/__init__.py
+-rw-rw-rw-   0        0        0      142 2023-05-19 19:02:52.000000 backtestify-0.1.3/backtestify/account.py
+-rw-rw-rw-   0        0        0     2792 2023-06-06 16:32:31.000000 backtestify-0.1.3/backtestify/backtester.py
+-rw-rw-rw-   0        0        0      696 2023-05-28 19:31:49.000000 backtestify-0.1.3/backtestify/cfd.py
+-rw-rw-rw-   0        0        0     1931 2023-05-19 19:02:52.000000 backtestify-0.1.3/backtestify/event.py
+-rw-rw-rw-   0        0        0      296 2023-05-19 19:02:52.000000 backtestify-0.1.3/backtestify/event_execution_context.py
+-rw-rw-rw-   0        0        0      498 2023-05-19 19:02:52.000000 backtestify-0.1.3/backtestify/event_execution_strategy.py
+-rw-rw-rw-   0        0        0       74 2023-05-19 19:02:52.000000 backtestify-0.1.3/backtestify/event_type.py
+-rw-rw-rw-   0        0        0      431 2023-05-19 19:02:52.000000 backtestify-0.1.3/backtestify/financial_instrument.py
+-rw-rw-rw-   0        0        0       98 2023-05-19 19:02:52.000000 backtestify-0.1.3/backtestify/instrument_type.py
+-rw-rw-rw-   0        0        0    10196 2023-05-29 00:05:22.000000 backtestify-0.1.3/backtestify/signal_event.py
+-rw-rw-rw-   0        0        0      160 2023-05-19 23:36:19.000000 backtestify-0.1.3/backtestify/signal_type.py
+-rw-rw-rw-   0        0        0     4802 2023-06-05 18:57:27.000000 backtestify-0.1.3/backtestify/strategy.py
+-rw-rw-rw-   0        0        0      494 2023-05-23 03:39:36.000000 backtestify-0.1.3/backtestify/trade.py
+-rw-rw-rw-   0        0        0    11125 2023-06-05 18:52:19.000000 backtestify-0.1.3/backtestify/trade_executor.py
+-rw-rw-rw-   0        0        0     2872 2023-05-28 23:20:05.000000 backtestify-0.1.3/backtestify/trade_state.py
+drwxrwxrwx   0        0        0        0 2023-06-06 16:35:09.402174 backtestify-0.1.3/backtestify.egg-info/
+-rw-rw-rw-   0        0        0      409 2023-06-06 16:35:09.000000 backtestify-0.1.3/backtestify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      642 2023-06-06 16:35:09.000000 backtestify-0.1.3/backtestify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 16:35:09.000000 backtestify-0.1.3/backtestify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-06 16:35:09.000000 backtestify-0.1.3/backtestify.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-06 16:35:09.000000 backtestify-0.1.3/backtestify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 16:35:09.404052 backtestify-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      662 2023-06-06 16:33:08.000000 backtestify-0.1.3/setup.py
```

### Comparing `backtestify-0.1.2/LICENSE` & `backtestify-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `backtestify-0.1.2/backtestify/__init__.py` & `backtestify-0.1.3/backtestify/__init__.py`

 * *Files identical despite different names*

### Comparing `backtestify-0.1.2/backtestify/backtester.py` & `backtestify-0.1.3/backtestify/backtester.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,7 +71,9 @@
         trades = []
 
         for trade in self.trades:
             trades.append(trade.__dict__)
 
         df_trades = pd.DataFrame(trades)
         df_trades = df_trades.set_index('timestamp')
+
+        return df_trades
```

### Comparing `backtestify-0.1.2/backtestify/cfd.py` & `backtestify-0.1.3/backtestify/cfd.py`

 * *Files identical despite different names*

### Comparing `backtestify-0.1.2/backtestify/event.py` & `backtestify-0.1.3/backtestify/event.py`

 * *Files identical despite different names*

### Comparing `backtestify-0.1.2/backtestify/signal_event.py` & `backtestify-0.1.3/backtestify/signal_event.py`

 * *Files identical despite different names*

### Comparing `backtestify-0.1.2/backtestify/strategy.py` & `backtestify-0.1.3/backtestify/strategy.py`

 * *Files identical despite different names*

### Comparing `backtestify-0.1.2/backtestify/trade_executor.py` & `backtestify-0.1.3/backtestify/trade_executor.py`

 * *Files identical despite different names*

### Comparing `backtestify-0.1.2/backtestify/trade_state.py` & `backtestify-0.1.3/backtestify/trade_state.py`

 * *Files identical despite different names*

### Comparing `backtestify-0.1.2/backtestify.egg-info/SOURCES.txt` & `backtestify-0.1.3/backtestify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backtestify-0.1.2/setup.py` & `backtestify-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as file:
     more_description = file.read()
 
 setuptools.setup(
     name="backtestify",
-    version="0.1.2",
+    version="0.1.3",
     author="Eladio Rocha Vizcaino",
     author_email="eladio.rocha99@gmail.com",
     description="A package for backtesting trading strategies",
     more_description=more_description,
     long_description_content_type="text/markdown",
     url="https://github.com/EladioRocha/backtestify",
     project_urls={
```

