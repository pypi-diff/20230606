# Comparing `tmp/backtestify-0.1.4.tar.gz` & `tmp/backtestify-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backtestify-0.1.4.tar", last modified: Tue Jun  6 16:59:28 2023, max compression
+gzip compressed data, was "backtestify-0.1.5.tar", last modified: Tue Jun  6 17:05:09 2023, max compression
```

## Comparing `backtestify-0.1.4.tar` & `backtestify-0.1.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 16:59:28.510114 backtestify-0.1.4/
--rw-rw-rw-   0        0        0    11558 2023-05-19 19:02:52.000000 backtestify-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      409 2023-06-06 16:59:28.509105 backtestify-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     4429 2023-06-06 16:56:06.000000 backtestify-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 16:59:28.502596 backtestify-0.1.4/backtestify/
--rw-rw-rw-   0        0        0     1362 2023-05-28 18:33:09.000000 backtestify-0.1.4/backtestify/__init__.py
--rw-rw-rw-   0        0        0      142 2023-05-19 19:02:52.000000 backtestify-0.1.4/backtestify/account.py
--rw-rw-rw-   0        0        0     2792 2023-06-06 16:32:31.000000 backtestify-0.1.4/backtestify/backtester.py
--rw-rw-rw-   0        0        0      696 2023-05-28 19:31:49.000000 backtestify-0.1.4/backtestify/cfd.py
--rw-rw-rw-   0        0        0     1931 2023-05-19 19:02:52.000000 backtestify-0.1.4/backtestify/event.py
--rw-rw-rw-   0        0        0      296 2023-05-19 19:02:52.000000 backtestify-0.1.4/backtestify/event_execution_context.py
--rw-rw-rw-   0        0        0      498 2023-05-19 19:02:52.000000 backtestify-0.1.4/backtestify/event_execution_strategy.py
--rw-rw-rw-   0        0        0       74 2023-05-19 19:02:52.000000 backtestify-0.1.4/backtestify/event_type.py
--rw-rw-rw-   0        0        0      431 2023-05-19 19:02:52.000000 backtestify-0.1.4/backtestify/financial_instrument.py
--rw-rw-rw-   0        0        0       98 2023-05-19 19:02:52.000000 backtestify-0.1.4/backtestify/instrument_type.py
--rw-rw-rw-   0        0        0    10196 2023-05-29 00:05:22.000000 backtestify-0.1.4/backtestify/signal_event.py
--rw-rw-rw-   0        0        0      160 2023-05-19 23:36:19.000000 backtestify-0.1.4/backtestify/signal_type.py
--rw-rw-rw-   0        0        0     4802 2023-06-05 18:57:27.000000 backtestify-0.1.4/backtestify/strategy.py
--rw-rw-rw-   0        0        0      494 2023-05-23 03:39:36.000000 backtestify-0.1.4/backtestify/trade.py
--rw-rw-rw-   0        0        0    11125 2023-06-05 18:52:19.000000 backtestify-0.1.4/backtestify/trade_executor.py
--rw-rw-rw-   0        0        0     2872 2023-05-28 23:20:05.000000 backtestify-0.1.4/backtestify/trade_state.py
-drwxrwxrwx   0        0        0        0 2023-06-06 16:59:28.508100 backtestify-0.1.4/backtestify.egg-info/
--rw-rw-rw-   0        0        0      409 2023-06-06 16:59:28.000000 backtestify-0.1.4/backtestify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      642 2023-06-06 16:59:28.000000 backtestify-0.1.4/backtestify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 16:59:28.000000 backtestify-0.1.4/backtestify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-06 16:59:28.000000 backtestify-0.1.4/backtestify.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-06 16:59:28.000000 backtestify-0.1.4/backtestify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 16:59:28.510114 backtestify-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      662 2023-06-06 16:58:40.000000 backtestify-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 17:05:09.870827 backtestify-0.1.5/
+-rw-rw-rw-   0        0        0    11558 2023-05-19 19:02:52.000000 backtestify-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     4842 2023-06-06 17:05:09.869827 backtestify-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4429 2023-06-06 16:56:06.000000 backtestify-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 17:05:09.864313 backtestify-0.1.5/backtestify/
+-rw-rw-rw-   0        0        0     1362 2023-05-28 18:33:09.000000 backtestify-0.1.5/backtestify/__init__.py
+-rw-rw-rw-   0        0        0      142 2023-05-19 19:02:52.000000 backtestify-0.1.5/backtestify/account.py
+-rw-rw-rw-   0        0        0     2792 2023-06-06 16:32:31.000000 backtestify-0.1.5/backtestify/backtester.py
+-rw-rw-rw-   0        0        0      696 2023-05-28 19:31:49.000000 backtestify-0.1.5/backtestify/cfd.py
+-rw-rw-rw-   0        0        0     1931 2023-05-19 19:02:52.000000 backtestify-0.1.5/backtestify/event.py
+-rw-rw-rw-   0        0        0      296 2023-05-19 19:02:52.000000 backtestify-0.1.5/backtestify/event_execution_context.py
+-rw-rw-rw-   0        0        0      498 2023-05-19 19:02:52.000000 backtestify-0.1.5/backtestify/event_execution_strategy.py
+-rw-rw-rw-   0        0        0       74 2023-05-19 19:02:52.000000 backtestify-0.1.5/backtestify/event_type.py
+-rw-rw-rw-   0        0        0      431 2023-05-19 19:02:52.000000 backtestify-0.1.5/backtestify/financial_instrument.py
+-rw-rw-rw-   0        0        0       98 2023-05-19 19:02:52.000000 backtestify-0.1.5/backtestify/instrument_type.py
+-rw-rw-rw-   0        0        0    10196 2023-05-29 00:05:22.000000 backtestify-0.1.5/backtestify/signal_event.py
+-rw-rw-rw-   0        0        0      160 2023-05-19 23:36:19.000000 backtestify-0.1.5/backtestify/signal_type.py
+-rw-rw-rw-   0        0        0     4802 2023-06-05 18:57:27.000000 backtestify-0.1.5/backtestify/strategy.py
+-rw-rw-rw-   0        0        0      494 2023-05-23 03:39:36.000000 backtestify-0.1.5/backtestify/trade.py
+-rw-rw-rw-   0        0        0    11125 2023-06-05 18:52:19.000000 backtestify-0.1.5/backtestify/trade_executor.py
+-rw-rw-rw-   0        0        0     2872 2023-05-28 23:20:05.000000 backtestify-0.1.5/backtestify/trade_state.py
+drwxrwxrwx   0        0        0        0 2023-06-06 17:05:09.868828 backtestify-0.1.5/backtestify.egg-info/
+-rw-rw-rw-   0        0        0     4842 2023-06-06 17:05:09.000000 backtestify-0.1.5/backtestify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      642 2023-06-06 17:05:09.000000 backtestify-0.1.5/backtestify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 17:05:09.000000 backtestify-0.1.5/backtestify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-06 17:05:09.000000 backtestify-0.1.5/backtestify.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-06 17:05:09.000000 backtestify-0.1.5/backtestify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 17:05:09.870827 backtestify-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      642 2023-06-06 17:04:19.000000 backtestify-0.1.5/setup.py
```

### Comparing `backtestify-0.1.4/LICENSE` & `backtestify-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `backtestify-0.1.4/README.md` & `backtestify-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `backtestify-0.1.4/backtestify/__init__.py` & `backtestify-0.1.5/backtestify/__init__.py`

 * *Files identical despite different names*

### Comparing `backtestify-0.1.4/backtestify/backtester.py` & `backtestify-0.1.5/backtestify/backtester.py`

 * *Files identical despite different names*

### Comparing `backtestify-0.1.4/backtestify/cfd.py` & `backtestify-0.1.5/backtestify/cfd.py`

 * *Files identical despite different names*

### Comparing `backtestify-0.1.4/backtestify/event.py` & `backtestify-0.1.5/backtestify/event.py`

 * *Files identical despite different names*

### Comparing `backtestify-0.1.4/backtestify/signal_event.py` & `backtestify-0.1.5/backtestify/signal_event.py`

 * *Files identical despite different names*

### Comparing `backtestify-0.1.4/backtestify/strategy.py` & `backtestify-0.1.5/backtestify/strategy.py`

 * *Files identical despite different names*

### Comparing `backtestify-0.1.4/backtestify/trade_executor.py` & `backtestify-0.1.5/backtestify/trade_executor.py`

 * *Files identical despite different names*

### Comparing `backtestify-0.1.4/backtestify/trade_state.py` & `backtestify-0.1.5/backtestify/trade_state.py`

 * *Files identical despite different names*

### Comparing `backtestify-0.1.4/backtestify.egg-info/SOURCES.txt` & `backtestify-0.1.5/backtestify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

