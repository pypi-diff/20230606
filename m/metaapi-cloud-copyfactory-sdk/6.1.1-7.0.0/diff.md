# Comparing `tmp/metaapi_cloud_copyfactory_sdk-6.1.1.tar.gz` & `tmp/metaapi_cloud_copyfactory_sdk-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaapi_cloud_copyfactory_sdk-6.1.1.tar", last modified: Wed Feb 22 08:19:07 2023, max compression
+gzip compressed data, was "metaapi_cloud_copyfactory_sdk-7.0.0.tar", last modified: Tue Jun  6 18:24:39 2023, max compression
```

## Comparing `metaapi_cloud_copyfactory_sdk-6.1.1.tar` & `metaapi_cloud_copyfactory_sdk-7.0.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-02-22 08:19:07.305084 metaapi_cloud_copyfactory_sdk-6.1.1/
--rw-r--r--   0 roman      (501) staff       (20)      781 2023-02-22 08:18:57.000000 metaapi_cloud_copyfactory_sdk-6.1.1/LICENSE
--rw-r--r--   0 roman      (501) staff       (20)      156 2021-03-10 17:33:56.000000 metaapi_cloud_copyfactory_sdk-6.1.1/MANIFEST.in
--rw-r--r--   0 roman      (501) staff       (20)    16729 2023-02-22 08:19:07.304922 metaapi_cloud_copyfactory_sdk-6.1.1/PKG-INFO
--rw-r--r--   0 roman      (501) staff       (20)    15971 2023-02-18 19:13:00.000000 metaapi_cloud_copyfactory_sdk-6.1.1/README.rst
--rw-r--r--   0 roman      (501) staff       (20)     2976 2023-02-22 08:18:37.000000 metaapi_cloud_copyfactory_sdk-6.1.1/changelog.md
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-02-22 08:19:07.292934 metaapi_cloud_copyfactory_sdk-6.1.1/examples/
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-02-22 08:19:07.295912 metaapi_cloud_copyfactory_sdk-6.1.1/examples/copytrade/
--rw-r--r--   0 roman      (501) staff       (20)     2683 2021-09-14 07:31:55.000000 metaapi_cloud_copyfactory_sdk-6.1.1/examples/copytrade/copytrade.py
--rw-r--r--   0 roman      (501) staff       (20)     3592 2023-02-02 11:42:24.000000 metaapi_cloud_copyfactory_sdk-6.1.1/examples/copytrade/externalSignal.py
--rw-r--r--   0 roman      (501) staff       (20)       24 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-6.1.1/examples/copytrade/requirements.txt
--rw-r--r--   0 roman      (501) staff       (20)      924 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-6.1.1/examples/copytrade/stopoutListener.py
--rw-r--r--   0 roman      (501) staff       (20)     1057 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-6.1.1/examples/copytrade/strategyTransactionListener.py
--rw-r--r--   0 roman      (501) staff       (20)     1000 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-6.1.1/examples/copytrade/strategyUserLogListener.py
--rw-r--r--   0 roman      (501) staff       (20)     1071 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-6.1.1/examples/copytrade/subscriberTransactionListener.py
--rw-r--r--   0 roman      (501) staff       (20)     1014 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-6.1.1/examples/copytrade/subscriberUserLogListener.py
--rw-r--r--   0 roman      (501) staff       (20)     3147 2022-04-26 12:25:03.000000 metaapi_cloud_copyfactory_sdk-6.1.1/examples/copytrade/telegram.py
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-02-22 08:19:07.297834 metaapi_cloud_copyfactory_sdk-6.1.1/examples/exampleGenerator/
--rw-r--r--   0 roman      (501) staff       (20)     2683 2021-09-14 07:31:55.000000 metaapi_cloud_copyfactory_sdk-6.1.1/examples/exampleGenerator/copyTradeExample.py
--rw-r--r--   0 roman      (501) staff       (20)     3472 2022-04-26 12:25:03.000000 metaapi_cloud_copyfactory_sdk-6.1.1/examples/exampleGenerator/externalSignalExample.py
--rw-r--r--   0 roman      (501) staff       (20)       24 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-6.1.1/examples/exampleGenerator/requirements.txt
--rw-r--r--   0 roman      (501) staff       (20)     1030 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-6.1.1/examples/exampleGenerator/stopoutListenerExample.py
--rw-r--r--   0 roman      (501) staff       (20)     1032 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-6.1.1/examples/exampleGenerator/strategyTransactionListenerExample.py
--rw-r--r--   0 roman      (501) staff       (20)      975 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-6.1.1/examples/exampleGenerator/strategyUserLogListenerExample.py
--rw-r--r--   0 roman      (501) staff       (20)     1046 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-6.1.1/examples/exampleGenerator/subscriberTransactionListenerExample.py
--rw-r--r--   0 roman      (501) staff       (20)      989 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-6.1.1/examples/exampleGenerator/subscriberUserLogListenerExample.py
--rw-r--r--   0 roman      (501) staff       (20)     3163 2022-04-26 12:25:03.000000 metaapi_cloud_copyfactory_sdk-6.1.1/examples/exampleGenerator/telegramExample.py
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-02-22 08:19:07.298522 metaapi_cloud_copyfactory_sdk-6.1.1/lib/
--rw-r--r--   0 roman      (501) staff       (20)      270 2022-07-12 03:16:48.000000 metaapi_cloud_copyfactory_sdk-6.1.1/lib/__init__.py
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-02-22 08:19:07.300621 metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/
--rw-r--r--   0 roman      (501) staff       (20)       52 2021-03-10 17:33:56.000000 metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/__init__.py
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-02-22 08:19:07.302692 metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/copyFactory/
--rw-r--r--   0 roman      (501) staff       (20)        0 2021-03-10 17:33:56.000000 metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/copyFactory/__init__.py
--rw-r--r--   0 roman      (501) staff       (20)    16776 2022-04-12 17:17:48.000000 metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/copyFactory/configuration_client.py
--rw-r--r--   0 roman      (501) staff       (20)    25225 2022-04-12 17:17:48.000000 metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/copyFactory/configuration_client_test.py
--rw-r--r--   0 roman      (501) staff       (20)    42905 2023-02-02 11:42:24.000000 metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/copyFactory/copyFactory_models.py
--rw-r--r--   0 roman      (501) staff       (20)     6582 2022-07-12 03:16:48.000000 metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/copyFactory/history_client.py
--rw-r--r--   0 roman      (501) staff       (20)     8109 2022-07-12 03:16:48.000000 metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/copyFactory/history_client_test.py
--rw-r--r--   0 roman      (501) staff       (20)     4458 2023-02-02 11:42:24.000000 metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/copyFactory/signal_client.py
--rw-r--r--   0 roman      (501) staff       (20)     3944 2023-02-02 11:42:24.000000 metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/copyFactory/signal_client_test.py
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-02-22 08:19:07.304134 metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/copyFactory/streaming/
--rw-r--r--   0 roman      (501) staff       (20)        0 2022-07-12 03:16:48.000000 metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/copyFactory/streaming/__init__.py
--rw-r--r--   0 roman      (501) staff       (20)      718 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/copyFactory/streaming/stopoutListener.py
--rw-r--r--   0 roman      (501) staff       (20)     3495 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/copyFactory/streaming/stopoutListenerManager.py
--rw-r--r--   0 roman      (501) staff       (20)     6857 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/copyFactory/streaming/stopoutListenerManager_test.py
--rw-r--r--   0 roman      (501) staff       (20)      711 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/copyFactory/streaming/transactionListener.py
--rw-r--r--   0 roman      (501) staff       (20)     7466 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/copyFactory/streaming/transactionListenerManager.py
--rw-r--r--   0 roman      (501) staff       (20)    15751 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/copyFactory/streaming/transactionListenerManager_test.py
--rw-r--r--   0 roman      (501) staff       (20)      688 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/copyFactory/streaming/userLogListener.py
--rw-r--r--   0 roman      (501) staff       (20)     8761 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/copyFactory/streaming/userLogListenerManager.py
--rw-r--r--   0 roman      (501) staff       (20)    16144 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/copyFactory/streaming/userLogListenerManager_test.py
--rw-r--r--   0 roman      (501) staff       (20)    11639 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/copyFactory/trading_client.py
--rw-r--r--   0 roman      (501) staff       (20)    12107 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/copyFactory/trading_client_test.py
--rw-r--r--   0 roman      (501) staff       (20)     6821 2023-02-02 11:42:24.000000 metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/domain_client.py
--rw-r--r--   0 roman      (501) staff       (20)    14227 2023-02-02 11:42:24.000000 metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/domain_client_test.py
--rw-r--r--   0 roman      (501) staff       (20)     4339 2021-03-10 17:33:56.000000 metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/errorHandler.py
--rw-r--r--   0 roman      (501) staff       (20)     7315 2022-07-12 03:16:48.000000 metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/httpClient.py
--rw-r--r--   0 roman      (501) staff       (20)     8696 2022-04-12 17:17:48.000000 metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/httpClient_test.py
--rw-r--r--   0 roman      (501) staff       (20)     1577 2022-04-12 17:17:48.000000 metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/metaApi_client.py
--rw-r--r--   0 roman      (501) staff       (20)     2488 2022-04-12 17:17:48.000000 metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/metaApi_client_test.py
--rw-r--r--   0 roman      (501) staff       (20)     1008 2021-03-10 17:33:56.000000 metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/methodAccessException.py
--rw-r--r--   0 roman      (501) staff       (20)      261 2021-03-10 17:33:56.000000 metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/timeoutException.py
--rw-r--r--   0 roman      (501) staff       (20)     3018 2022-07-12 03:16:48.000000 metaapi_cloud_copyfactory_sdk-6.1.1/lib/copyFactory.py
--rw-r--r--   0 roman      (501) staff       (20)     1984 2022-07-12 03:16:48.000000 metaapi_cloud_copyfactory_sdk-6.1.1/lib/logger.py
--rw-r--r--   0 roman      (501) staff       (20)     3566 2022-04-12 17:17:48.000000 metaapi_cloud_copyfactory_sdk-6.1.1/lib/models.py
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-02-22 08:19:07.304724 metaapi_cloud_copyfactory_sdk-6.1.1/metaapi_cloud_copyfactory_sdk.egg-info/
--rw-r--r--   0 roman      (501) staff       (20)    16729 2023-02-22 08:19:07.000000 metaapi_cloud_copyfactory_sdk-6.1.1/metaapi_cloud_copyfactory_sdk.egg-info/PKG-INFO
--rw-r--r--   0 roman      (501) staff       (20)     2584 2023-02-22 08:19:07.000000 metaapi_cloud_copyfactory_sdk-6.1.1/metaapi_cloud_copyfactory_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 roman      (501) staff       (20)        1 2023-02-22 08:19:07.000000 metaapi_cloud_copyfactory_sdk-6.1.1/metaapi_cloud_copyfactory_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 roman      (501) staff       (20)       87 2023-02-22 08:19:07.000000 metaapi_cloud_copyfactory_sdk-6.1.1/metaapi_cloud_copyfactory_sdk.egg-info/requires.txt
--rw-r--r--   0 roman      (501) staff       (20)       30 2023-02-22 08:19:07.000000 metaapi_cloud_copyfactory_sdk-6.1.1/metaapi_cloud_copyfactory_sdk.egg-info/top_level.txt
--rw-r--r--   0 roman      (501) staff       (20)       38 2023-02-22 08:19:07.305134 metaapi_cloud_copyfactory_sdk-6.1.1/setup.cfg
--rw-r--r--   0 roman      (501) staff       (20)     1520 2023-02-22 08:18:37.000000 metaapi_cloud_copyfactory_sdk-6.1.1/setup.py
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-06-06 18:24:39.480300 metaapi_cloud_copyfactory_sdk-7.0.0/
+-rw-r--r--   0 roman      (501) staff       (20)      781 2023-02-22 08:18:57.000000 metaapi_cloud_copyfactory_sdk-7.0.0/LICENSE
+-rw-r--r--   0 roman      (501) staff       (20)      156 2021-03-10 17:33:56.000000 metaapi_cloud_copyfactory_sdk-7.0.0/MANIFEST.in
+-rw-r--r--   0 roman      (501) staff       (20)    16742 2023-06-06 18:24:39.480140 metaapi_cloud_copyfactory_sdk-7.0.0/PKG-INFO
+-rw-r--r--   0 roman      (501) staff       (20)    15984 2023-06-06 18:24:38.000000 metaapi_cloud_copyfactory_sdk-7.0.0/README.rst
+-rw-r--r--   0 roman      (501) staff       (20)     3144 2023-06-06 18:24:38.000000 metaapi_cloud_copyfactory_sdk-7.0.0/changelog.md
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-06-06 18:24:39.467970 metaapi_cloud_copyfactory_sdk-7.0.0/examples/
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-06-06 18:24:39.471188 metaapi_cloud_copyfactory_sdk-7.0.0/examples/copytrade/
+-rw-r--r--   0 roman      (501) staff       (20)     2683 2021-09-14 07:31:55.000000 metaapi_cloud_copyfactory_sdk-7.0.0/examples/copytrade/copytrade.py
+-rw-r--r--   0 roman      (501) staff       (20)     3592 2023-02-02 11:42:24.000000 metaapi_cloud_copyfactory_sdk-7.0.0/examples/copytrade/externalSignal.py
+-rw-r--r--   0 roman      (501) staff       (20)       24 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-7.0.0/examples/copytrade/requirements.txt
+-rw-r--r--   0 roman      (501) staff       (20)      924 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-7.0.0/examples/copytrade/stopoutListener.py
+-rw-r--r--   0 roman      (501) staff       (20)     1057 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-7.0.0/examples/copytrade/strategyTransactionListener.py
+-rw-r--r--   0 roman      (501) staff       (20)     1000 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-7.0.0/examples/copytrade/strategyUserLogListener.py
+-rw-r--r--   0 roman      (501) staff       (20)     1071 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-7.0.0/examples/copytrade/subscriberTransactionListener.py
+-rw-r--r--   0 roman      (501) staff       (20)     1014 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-7.0.0/examples/copytrade/subscriberUserLogListener.py
+-rw-r--r--   0 roman      (501) staff       (20)     3147 2022-04-26 12:25:03.000000 metaapi_cloud_copyfactory_sdk-7.0.0/examples/copytrade/telegram.py
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-06-06 18:24:39.472822 metaapi_cloud_copyfactory_sdk-7.0.0/examples/exampleGenerator/
+-rw-r--r--   0 roman      (501) staff       (20)     2683 2021-09-14 07:31:55.000000 metaapi_cloud_copyfactory_sdk-7.0.0/examples/exampleGenerator/copyTradeExample.py
+-rw-r--r--   0 roman      (501) staff       (20)     3472 2022-04-26 12:25:03.000000 metaapi_cloud_copyfactory_sdk-7.0.0/examples/exampleGenerator/externalSignalExample.py
+-rw-r--r--   0 roman      (501) staff       (20)       24 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-7.0.0/examples/exampleGenerator/requirements.txt
+-rw-r--r--   0 roman      (501) staff       (20)     1030 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-7.0.0/examples/exampleGenerator/stopoutListenerExample.py
+-rw-r--r--   0 roman      (501) staff       (20)     1032 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-7.0.0/examples/exampleGenerator/strategyTransactionListenerExample.py
+-rw-r--r--   0 roman      (501) staff       (20)      975 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-7.0.0/examples/exampleGenerator/strategyUserLogListenerExample.py
+-rw-r--r--   0 roman      (501) staff       (20)     1046 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-7.0.0/examples/exampleGenerator/subscriberTransactionListenerExample.py
+-rw-r--r--   0 roman      (501) staff       (20)      989 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-7.0.0/examples/exampleGenerator/subscriberUserLogListenerExample.py
+-rw-r--r--   0 roman      (501) staff       (20)     3163 2022-04-26 12:25:03.000000 metaapi_cloud_copyfactory_sdk-7.0.0/examples/exampleGenerator/telegramExample.py
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-06-06 18:24:39.473408 metaapi_cloud_copyfactory_sdk-7.0.0/lib/
+-rw-r--r--   0 roman      (501) staff       (20)      270 2022-07-12 03:16:48.000000 metaapi_cloud_copyfactory_sdk-7.0.0/lib/__init__.py
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-06-06 18:24:39.475204 metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/
+-rw-r--r--   0 roman      (501) staff       (20)       52 2021-03-10 17:33:56.000000 metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/__init__.py
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-06-06 18:24:39.477440 metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/copyFactory/
+-rw-r--r--   0 roman      (501) staff       (20)        0 2021-03-10 17:33:56.000000 metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/copyFactory/__init__.py
+-rw-r--r--   0 roman      (501) staff       (20)    16776 2022-04-12 17:17:48.000000 metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/copyFactory/configuration_client.py
+-rw-r--r--   0 roman      (501) staff       (20)    25225 2022-04-12 17:17:48.000000 metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/copyFactory/configuration_client_test.py
+-rw-r--r--   0 roman      (501) staff       (20)    42905 2023-02-02 11:42:24.000000 metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/copyFactory/copyFactory_models.py
+-rw-r--r--   0 roman      (501) staff       (20)     6582 2022-07-12 03:16:48.000000 metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/copyFactory/history_client.py
+-rw-r--r--   0 roman      (501) staff       (20)     8109 2022-07-12 03:16:48.000000 metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/copyFactory/history_client_test.py
+-rw-r--r--   0 roman      (501) staff       (20)     4458 2023-02-02 11:42:24.000000 metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/copyFactory/signal_client.py
+-rw-r--r--   0 roman      (501) staff       (20)     3944 2023-02-02 11:42:24.000000 metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/copyFactory/signal_client_test.py
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-06-06 18:24:39.479250 metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/copyFactory/streaming/
+-rw-r--r--   0 roman      (501) staff       (20)        0 2022-07-12 03:16:48.000000 metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/copyFactory/streaming/__init__.py
+-rw-r--r--   0 roman      (501) staff       (20)      718 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/copyFactory/streaming/stopoutListener.py
+-rw-r--r--   0 roman      (501) staff       (20)     3495 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/copyFactory/streaming/stopoutListenerManager.py
+-rw-r--r--   0 roman      (501) staff       (20)     6857 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/copyFactory/streaming/stopoutListenerManager_test.py
+-rw-r--r--   0 roman      (501) staff       (20)      711 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/copyFactory/streaming/transactionListener.py
+-rw-r--r--   0 roman      (501) staff       (20)     7466 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/copyFactory/streaming/transactionListenerManager.py
+-rw-r--r--   0 roman      (501) staff       (20)    15751 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/copyFactory/streaming/transactionListenerManager_test.py
+-rw-r--r--   0 roman      (501) staff       (20)      688 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/copyFactory/streaming/userLogListener.py
+-rw-r--r--   0 roman      (501) staff       (20)     8761 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/copyFactory/streaming/userLogListenerManager.py
+-rw-r--r--   0 roman      (501) staff       (20)    16144 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/copyFactory/streaming/userLogListenerManager_test.py
+-rw-r--r--   0 roman      (501) staff       (20)    12589 2023-06-06 18:24:38.000000 metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/copyFactory/trading_client.py
+-rw-r--r--   0 roman      (501) staff       (20)    13490 2023-06-06 18:24:38.000000 metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/copyFactory/trading_client_test.py
+-rw-r--r--   0 roman      (501) staff       (20)     6821 2023-02-02 11:42:24.000000 metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/domain_client.py
+-rw-r--r--   0 roman      (501) staff       (20)    14227 2023-04-07 19:11:46.000000 metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/domain_client_test.py
+-rw-r--r--   0 roman      (501) staff       (20)     4339 2021-03-10 17:33:56.000000 metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/errorHandler.py
+-rw-r--r--   0 roman      (501) staff       (20)     7315 2022-07-12 03:16:48.000000 metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/httpClient.py
+-rw-r--r--   0 roman      (501) staff       (20)     8696 2022-04-12 17:17:48.000000 metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/httpClient_test.py
+-rw-r--r--   0 roman      (501) staff       (20)     1577 2022-04-12 17:17:48.000000 metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/metaApi_client.py
+-rw-r--r--   0 roman      (501) staff       (20)     2488 2022-04-12 17:17:48.000000 metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/metaApi_client_test.py
+-rw-r--r--   0 roman      (501) staff       (20)     1008 2021-03-10 17:33:56.000000 metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/methodAccessException.py
+-rw-r--r--   0 roman      (501) staff       (20)      261 2021-03-10 17:33:56.000000 metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/timeoutException.py
+-rw-r--r--   0 roman      (501) staff       (20)     3018 2022-07-12 03:16:48.000000 metaapi_cloud_copyfactory_sdk-7.0.0/lib/copyFactory.py
+-rw-r--r--   0 roman      (501) staff       (20)     1984 2022-07-12 03:16:48.000000 metaapi_cloud_copyfactory_sdk-7.0.0/lib/logger.py
+-rw-r--r--   0 roman      (501) staff       (20)     3566 2022-04-12 17:17:48.000000 metaapi_cloud_copyfactory_sdk-7.0.0/lib/models.py
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-06-06 18:24:39.479910 metaapi_cloud_copyfactory_sdk-7.0.0/metaapi_cloud_copyfactory_sdk.egg-info/
+-rw-r--r--   0 roman      (501) staff       (20)    16742 2023-06-06 18:24:39.000000 metaapi_cloud_copyfactory_sdk-7.0.0/metaapi_cloud_copyfactory_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 roman      (501) staff       (20)     2584 2023-06-06 18:24:39.000000 metaapi_cloud_copyfactory_sdk-7.0.0/metaapi_cloud_copyfactory_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 roman      (501) staff       (20)        1 2023-06-06 18:24:39.000000 metaapi_cloud_copyfactory_sdk-7.0.0/metaapi_cloud_copyfactory_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 roman      (501) staff       (20)       87 2023-06-06 18:24:39.000000 metaapi_cloud_copyfactory_sdk-7.0.0/metaapi_cloud_copyfactory_sdk.egg-info/requires.txt
+-rw-r--r--   0 roman      (501) staff       (20)       30 2023-06-06 18:24:39.000000 metaapi_cloud_copyfactory_sdk-7.0.0/metaapi_cloud_copyfactory_sdk.egg-info/top_level.txt
+-rw-r--r--   0 roman      (501) staff       (20)       38 2023-06-06 18:24:39.480344 metaapi_cloud_copyfactory_sdk-7.0.0/setup.cfg
+-rw-r--r--   0 roman      (501) staff       (20)     1520 2023-06-06 18:24:38.000000 metaapi_cloud_copyfactory_sdk-7.0.0/setup.py
```

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/LICENSE` & `metaapi_cloud_copyfactory_sdk-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/PKG-INFO` & `metaapi_cloud_copyfactory_sdk-7.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaapi_cloud_copyfactory_sdk
-Version: 6.1.1
+Version: 7.0.0
 Summary: Python SDK for SDK for CopyFactory trade copying API. Can copy trades both between MetaTrader 5 (MT5) and MetaTrader 4 (MT4). (https://metaapi.cloud)
 Home-page: https://github.com/agiliumtrade-ai/copyfactory-python-sdk
 Author: MetaApi DMCC
 Author-email: support@metaapi.cloud
 License: SEE LICENSE IN LICENSE
 Keywords: metaapi.cloud,MetaTrader,MetaTrader 5,MetaTrader 4,MetaTrader5,MetaTrader4,MT,MT4,MT5,forex,copy trading,API,REST,client,sdk,cloud
 Classifier: Programming Language :: Python :: 3
@@ -267,15 +267,15 @@
     account_id = '...' # CopyFactory account id
     strategy_id = '...' # CopyFactory strategy id
 
     # retrieve list of strategy stopouts
     print(await trading_api.get_stopouts(account_id=account_id))
 
     # reset a stopout so that subscription can continue
-    await trading_api.reset_stopouts(account_id=account_id, strategy_id=strategy_id, reason='daily-equity')
+    await trading_api.reset_subscription_stopouts(account_id=account_id, strategy_id=strategy_id, reason='daily-equity')
 
 Managing stopout listeners
 ==========================
 You can subscribe to a stream of stopout events using the stopout listener.
 
 .. code-block:: python
```

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/README.rst` & `metaapi_cloud_copyfactory_sdk-7.0.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -251,15 +251,15 @@
     account_id = '...' # CopyFactory account id
     strategy_id = '...' # CopyFactory strategy id
 
     # retrieve list of strategy stopouts
     print(await trading_api.get_stopouts(account_id=account_id))
 
     # reset a stopout so that subscription can continue
-    await trading_api.reset_stopouts(account_id=account_id, strategy_id=strategy_id, reason='daily-equity')
+    await trading_api.reset_subscription_stopouts(account_id=account_id, strategy_id=strategy_id, reason='daily-equity')
 
 Managing stopout listeners
 ==========================
 You can subscribe to a stream of stopout events using the stopout listener.
 
 .. code-block:: python
```

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/changelog.md` & `metaapi_cloud_copyfactory_sdk-7.0.0/changelog.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+7.0.0
+  - breaking change: updated `TradingClient` method `reset_stopouts` to `reset_subscription_stopouts`
+  - added method `TradingClient.reset_subscriber_stopouts`
+
 6.1.1
   - update package information
 
 6.1.0
   - added retrieve strategy external signals method
   - added rolling over to the first region if requests on all regions failed
```

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/examples/copytrade/copytrade.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/examples/copytrade/copytrade.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/examples/copytrade/externalSignal.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/examples/copytrade/externalSignal.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/examples/copytrade/stopoutListener.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/examples/copytrade/stopoutListener.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/examples/copytrade/strategyTransactionListener.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/examples/copytrade/strategyTransactionListener.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/examples/copytrade/strategyUserLogListener.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/examples/copytrade/strategyUserLogListener.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/examples/copytrade/subscriberTransactionListener.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/examples/copytrade/subscriberTransactionListener.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/examples/copytrade/subscriberUserLogListener.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/examples/copytrade/subscriberUserLogListener.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/examples/copytrade/telegram.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/examples/copytrade/telegram.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/examples/exampleGenerator/copyTradeExample.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/examples/exampleGenerator/copyTradeExample.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/examples/exampleGenerator/externalSignalExample.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/examples/exampleGenerator/externalSignalExample.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/examples/exampleGenerator/stopoutListenerExample.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/examples/exampleGenerator/stopoutListenerExample.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/examples/exampleGenerator/strategyTransactionListenerExample.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/examples/exampleGenerator/strategyTransactionListenerExample.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/examples/exampleGenerator/strategyUserLogListenerExample.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/examples/exampleGenerator/strategyUserLogListenerExample.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/examples/exampleGenerator/subscriberTransactionListenerExample.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/examples/exampleGenerator/subscriberTransactionListenerExample.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/examples/exampleGenerator/subscriberUserLogListenerExample.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/examples/exampleGenerator/subscriberUserLogListenerExample.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/examples/exampleGenerator/telegramExample.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/examples/exampleGenerator/telegramExample.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/copyFactory/configuration_client.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/copyFactory/configuration_client.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/copyFactory/configuration_client_test.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/copyFactory/configuration_client_test.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/copyFactory/copyFactory_models.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/copyFactory/copyFactory_models.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/copyFactory/history_client.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/copyFactory/history_client.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/copyFactory/history_client_test.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/copyFactory/history_client_test.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/copyFactory/signal_client.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/copyFactory/signal_client.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/copyFactory/signal_client_test.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/copyFactory/signal_client_test.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/copyFactory/streaming/stopoutListener.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/copyFactory/streaming/stopoutListener.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/copyFactory/streaming/stopoutListenerManager.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/copyFactory/streaming/stopoutListenerManager.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/copyFactory/streaming/stopoutListenerManager_test.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/copyFactory/streaming/stopoutListenerManager_test.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/copyFactory/streaming/transactionListener.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/copyFactory/streaming/transactionListener.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/copyFactory/streaming/transactionListenerManager.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/copyFactory/streaming/transactionListenerManager.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/copyFactory/streaming/transactionListenerManager_test.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/copyFactory/streaming/transactionListenerManager_test.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/copyFactory/streaming/userLogListener.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/copyFactory/streaming/userLogListener.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/copyFactory/streaming/userLogListenerManager.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/copyFactory/streaming/userLogListenerManager.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/copyFactory/streaming/userLogListenerManager_test.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/copyFactory/streaming/userLogListenerManager_test.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/copyFactory/trading_client.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/copyFactory/trading_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,39 +90,62 @@
                 'auth-token': self._token
             }
         }
         result = await self._domainClient.request_copyfactory(opts)
         convert_iso_time_to_date(result)
         return result
 
-    async def reset_stopouts(self, subscriber_id: str, strategy_id: str, reason: CopyFactoryStrategyStopoutReason) \
-            -> Response:
-        """Resets strategy stopouts. See
-        https://metaapi.cloud/docs/copyfactory/restApi/api/trading/resetStopOuts/
+    async def reset_subscription_stopouts(self, subscriber_id: str, strategy_id: str,
+                                          reason: CopyFactoryStrategyStopoutReason) -> Response:
+        """Resets subscription stopouts. See
+        https://metaapi.cloud/docs/copyfactory/restApi/api/trading/resetSubscriptionStopOuts/
 
         Args:
             subscriber_id: Account id.
             strategy_id: Strategy id.
             reason: Stopout reason to reset.
 
         Returns:
             A coroutine which resolves when the stopouts are reset.
         """
         if self._is_not_jwt_token():
-            return self._handle_no_access_exception('reset_stopouts')
+            return self._handle_no_access_exception('reset_subscription_stopouts')
         opts = {
             'url': f'/users/current/subscribers/{subscriber_id}/subscription-strategies/{strategy_id}' +
                    f'/stopouts/{reason}/reset',
             'method': 'POST',
             'headers': {
                 'auth-token': self._token
             }
         }
         return await self._domainClient.request_copyfactory(opts)
 
+    async def reset_subscriber_stopouts(self, subscriber_id: str, reason: CopyFactoryStrategyStopoutReason) \
+            -> Response:
+        """Resets subscriber stopouts. See
+        https://metaapi.cloud/docs/copyfactory/restApi/api/trading/resetSubscriberStopOuts/
+
+        Args:
+            subscriber_id: Account id.
+            reason: Stopout reason to reset.
+
+        Returns:
+            A coroutine which resolves when the stopouts are reset.
+        """
+        if self._is_not_jwt_token():
+            return self._handle_no_access_exception('reset_subscriber_stopouts')
+        opts = {
+            'url': f'/users/current/subscribers/{subscriber_id}/stopouts/{reason}/reset',
+            'method': 'POST',
+            'headers': {
+                'auth-token': self._token
+            }
+        }
+        return await self._domainClient.request_copyfactory(opts)
+
     async def get_user_log(self, subscriber_id: str, start_time: datetime = None, end_time: datetime = None,
                            strategy_id: str = None, position_id: str = None, level: LogLevel = None,
                            offset: int = 0, limit: int = 1000) -> 'List[CopyFactoryUserLogMessage]':
         """Returns copy trading user log for an account and time range, sorted in reverse chronological order. See
         https://metaapi.cloud/docs/copyfactory/restApi/api/trading/getUserLog/
 
         Args:
```

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/copyFactory/trading_client_test.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/copyFactory/trading_client_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -86,15 +86,15 @@
             assert err.__str__() == 'You can not invoke get_stopouts method, ' + \
                    'because you have connected with account access token. Please use API access token from ' + \
                    'https://app.metaapi.cloud/token page to invoke this method.'
 
     @pytest.mark.asyncio
     async def test_reset_stopouts(self):
         """Should reset stopouts."""
-        await trading_client.reset_stopouts('e8867baa-5ec2-45ae-9930-4d5cea18d0d6', 'ABCD', 'daily-equity')
+        await trading_client.reset_subscription_stopouts('e8867baa-5ec2-45ae-9930-4d5cea18d0d6', 'ABCD', 'daily-equity')
         domain_client.request_copyfactory.assert_called_with({
             'url': '/users/current/subscribers/' +
             'e8867baa-5ec2-45ae-9930-4d5cea18d0d6/subscription-strategies/ABCD/stopouts/daily-equity/reset',
             'method': 'POST',
             'headers': {
                 'auth-token': token
             },
@@ -102,19 +102,45 @@
 
     @pytest.mark.asyncio
     async def test_not_reset_stopouts_with_account_token(self):
         """Should not reset stopouts with account token."""
         domain_client.token = 'token'
         trading_client = TradingClient(domain_client)
         try:
-            await trading_client.reset_stopouts('e8867baa-5ec2-45ae-9930-4d5cea18d0d6',
-                                                'ABCD', 'daily-equity')
+            await trading_client.reset_subscription_stopouts('e8867baa-5ec2-45ae-9930-4d5cea18d0d6',
+                                                             'ABCD', 'daily-equity')
             pytest.fail()
         except Exception as err:
-            assert err.__str__() == 'You can not invoke reset_stopouts method, ' + \
+            assert err.__str__() == 'You can not invoke reset_subscription_stopouts method, ' + \
+                   'because you have connected with account access token. Please use API access token from ' + \
+                   'https://app.metaapi.cloud/token page to invoke this method.'
+
+    @pytest.mark.asyncio
+    async def test_reset_subscriber_stopouts(self):
+        """Should reset subscriber stopouts."""
+        await trading_client.reset_subscriber_stopouts('e8867baa-5ec2-45ae-9930-4d5cea18d0d6', 'daily-equity')
+        domain_client.request_copyfactory.assert_called_with({
+            'url': '/users/current/subscribers/e8867baa-5ec2-45ae-9930-4d5cea18d0d6/stopouts/daily-equity/reset',
+            'method': 'POST',
+            'headers': {
+                'auth-token': token
+            },
+        })
+
+    @pytest.mark.asyncio
+    async def test_not_reset_subscriber_stopouts_with_account_token(self):
+        """Should not reset subscriber stopouts with account token."""
+        domain_client.token = 'token'
+        trading_client = TradingClient(domain_client)
+        try:
+            await trading_client.reset_subscriber_stopouts('e8867baa-5ec2-45ae-9930-4d5cea18d0d6',
+                                                           'daily-equity')
+            pytest.fail()
+        except Exception as err:
+            assert err.__str__() == 'You can not invoke reset_subscriber_stopouts method, ' + \
                    'because you have connected with account access token. Please use API access token from ' + \
                    'https://app.metaapi.cloud/token page to invoke this method.'
 
     @pytest.mark.asyncio
     async def test_retrieve_copy_trading_log(self):
         """Should retrieve copy trading user log."""
         expected = [{
```

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/domain_client.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/domain_client.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/domain_client_test.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/domain_client_test.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/errorHandler.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/errorHandler.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/httpClient.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/httpClient.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/httpClient_test.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/httpClient_test.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/metaApi_client.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/metaApi_client.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/metaApi_client_test.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/metaApi_client_test.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/lib/clients/methodAccessException.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/lib/clients/methodAccessException.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/lib/copyFactory.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/lib/copyFactory.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/lib/logger.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/lib/logger.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/lib/models.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/lib/models.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/metaapi_cloud_copyfactory_sdk.egg-info/PKG-INFO` & `metaapi_cloud_copyfactory_sdk-7.0.0/metaapi_cloud_copyfactory_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaapi-cloud-copyfactory-sdk
-Version: 6.1.1
+Version: 7.0.0
 Summary: Python SDK for SDK for CopyFactory trade copying API. Can copy trades both between MetaTrader 5 (MT5) and MetaTrader 4 (MT4). (https://metaapi.cloud)
 Home-page: https://github.com/agiliumtrade-ai/copyfactory-python-sdk
 Author: MetaApi DMCC
 Author-email: support@metaapi.cloud
 License: SEE LICENSE IN LICENSE
 Keywords: metaapi.cloud,MetaTrader,MetaTrader 5,MetaTrader 4,MetaTrader5,MetaTrader4,MT,MT4,MT5,forex,copy trading,API,REST,client,sdk,cloud
 Classifier: Programming Language :: Python :: 3
@@ -267,15 +267,15 @@
     account_id = '...' # CopyFactory account id
     strategy_id = '...' # CopyFactory strategy id
 
     # retrieve list of strategy stopouts
     print(await trading_api.get_stopouts(account_id=account_id))
 
     # reset a stopout so that subscription can continue
-    await trading_api.reset_stopouts(account_id=account_id, strategy_id=strategy_id, reason='daily-equity')
+    await trading_api.reset_subscription_stopouts(account_id=account_id, strategy_id=strategy_id, reason='daily-equity')
 
 Managing stopout listeners
 ==========================
 You can subscribe to a stream of stopout events using the stopout listener.
 
 .. code-block:: python
```

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/metaapi_cloud_copyfactory_sdk.egg-info/SOURCES.txt` & `metaapi_cloud_copyfactory_sdk-7.0.0/metaapi_cloud_copyfactory_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-6.1.1/setup.py` & `metaapi_cloud_copyfactory_sdk-7.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 tests_require = [
     'pytest==6.2.5', 'pytest-mock', 'pytest-asyncio==0.16.0', 'asynctest', 'aiohttp', 'mock', 'freezegun==1.0.0',
     'respx==0.19.2'
 ]
 
 setuptools.setup(
     name="metaapi_cloud_copyfactory_sdk",
-    version="6.1.1",
+    version="7.0.0",
     author="MetaApi DMCC",
     author_email="support@metaapi.cloud",
     description="Python SDK for SDK for CopyFactory trade copying API. Can copy trades both between MetaTrader 5 "
                 "(MT5) and MetaTrader 4 (MT4). (https://metaapi.cloud)",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     keywords=['metaapi.cloud', 'MetaTrader', 'MetaTrader 5', 'MetaTrader 4', 'MetaTrader5', 'MetaTrader4', 'MT', 'MT4',
```

