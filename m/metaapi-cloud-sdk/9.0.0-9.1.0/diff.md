# Comparing `tmp/metaapi_cloud_sdk-9.0.0.tar.gz` & `tmp/metaapi_cloud_sdk-9.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/metaapi_cloud_sdk-9.0.0.tar", last modified: Sun Nov  1 09:55:12 2020, max compression
+gzip compressed data, was "dist/metaapi_cloud_sdk-9.1.0.tar", last modified: Sun Nov  8 14:33:03 2020, max compression
```

## Comparing `metaapi_cloud_sdk-9.0.0.tar` & `metaapi_cloud_sdk-9.1.0.tar`

### file list

```diff
@@ -1,112 +1,117 @@
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2020-11-01 09:55:12.000000 metaapi_cloud_sdk-9.0.0/
--rw-r--r--   0 roman      (501) staff       (20)      780 2020-06-27 16:25:18.000000 metaapi_cloud_sdk-9.0.0/LICENSE
--rw-r--r--   0 roman      (501) staff       (20)      142 2020-06-27 21:51:26.000000 metaapi_cloud_sdk-9.0.0/MANIFEST.in
--rw-r--r--   0 roman      (501) staff       (20)    27849 2020-11-01 09:55:12.000000 metaapi_cloud_sdk-9.0.0/PKG-INFO
--rw-r--r--   0 roman      (501) staff       (20)    22579 2020-11-01 09:54:50.000000 metaapi_cloud_sdk-9.0.0/README.rst
--rw-r--r--   0 roman      (501) staff       (20)     4812 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/changelog.md
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2020-11-01 09:55:12.000000 metaapi_cloud_sdk-9.0.0/examples/
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2020-11-01 09:55:12.000000 metaapi_cloud_sdk-9.0.0/examples/exampleGenerator/
--rw-r--r--   0 roman      (501) staff       (20)       25 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/examples/exampleGenerator/requirements.txt
--rw-r--r--   0 roman      (501) staff       (20)     3305 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/examples/exampleGenerator/rpcExample.py
--rw-r--r--   0 roman      (501) staff       (20)     2657 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/examples/exampleGenerator/synchronizationExample.py
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2020-11-01 09:55:12.000000 metaapi_cloud_sdk-9.0.0/examples/mt4/
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2020-11-01 09:55:12.000000 metaapi_cloud_sdk-9.0.0/examples/mt4/.metaapi/
--rw-r--r--   0 roman      (501) staff       (20)  1931916 2020-10-28 14:51:04.000000 metaapi_cloud_sdk-9.0.0/examples/mt4/.metaapi/11779f61-9dc5-4292-807b-f52906804439-deals.bin
--rw-r--r--   0 roman      (501) staff       (20)  5755801 2020-10-28 14:51:04.000000 metaapi_cloud_sdk-9.0.0/examples/mt4/.metaapi/11779f61-9dc5-4292-807b-f52906804439-historyOrders.bin
--rw-r--r--   0 roman      (501) staff       (20)     2527 2020-09-12 22:25:43.000000 metaapi_cloud_sdk-9.0.0/examples/mt4/.metaapi/9c283a6c-5c41-4351-a6e5-d974970ace0e-deals.bin
--rw-r--r--   0 roman      (501) staff       (20)  3552802 2020-09-12 22:25:43.000000 metaapi_cloud_sdk-9.0.0/examples/mt4/.metaapi/9c283a6c-5c41-4351-a6e5-d974970ace0e-historyOrders.bin
--rw-r--r--   0 roman      (501) staff       (20)     5013 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/examples/mt4/metaApiRpcExample.py
--rw-r--r--   0 roman      (501) staff       (20)     4368 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/examples/mt4/metaApiSynchronizationExample.py
--rw-r--r--   0 roman      (501) staff       (20)       25 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/examples/mt4/requirements.txt
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2020-11-01 09:55:12.000000 metaapi_cloud_sdk-9.0.0/examples/mt5/
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2020-11-01 09:55:12.000000 metaapi_cloud_sdk-9.0.0/examples/mt5/.metaapi/
--rw-r--r--   0 roman      (501) staff       (20)  1012522 2020-09-12 20:36:52.000000 metaapi_cloud_sdk-9.0.0/examples/mt5/.metaapi/76037e9a-ab26-4138-9013-496034dda8eb-deals.bin
--rw-r--r--   0 roman      (501) staff       (20)   558532 2020-09-12 20:36:52.000000 metaapi_cloud_sdk-9.0.0/examples/mt5/.metaapi/76037e9a-ab26-4138-9013-496034dda8eb-historyOrders.bin
--rw-r--r--   0 roman      (501) staff       (20)    82452 2020-09-12 21:06:51.000000 metaapi_cloud_sdk-9.0.0/examples/mt5/.metaapi/92b4a96e-0dbb-4bb5-924e-3d78dc097f81-deals.bin
--rw-r--r--   0 roman      (501) staff       (20)  1700153 2020-09-12 21:06:51.000000 metaapi_cloud_sdk-9.0.0/examples/mt5/.metaapi/92b4a96e-0dbb-4bb5-924e-3d78dc097f81-historyOrders.bin
--rw-r--r--   0 roman      (501) staff       (20)  1931056 2020-09-05 07:19:11.000000 metaapi_cloud_sdk-9.0.0/examples/mt5/.metaapi/a9fb463b-44d9-4336-a88f-3e458b02689f-deals.bin
--rw-r--r--   0 roman      (501) staff       (20)  2409166 2020-09-05 07:19:11.000000 metaapi_cloud_sdk-9.0.0/examples/mt5/.metaapi/a9fb463b-44d9-4336-a88f-3e458b02689f-historyOrders.bin
--rw-r--r--   0 roman      (501) staff       (20)     4997 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/examples/mt5/metaApiRpcExample.py
--rw-r--r--   0 roman      (501) staff       (20)     4397 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/examples/mt5/metaApiSynchronizationExample.py
--rw-r--r--   0 roman      (501) staff       (20)       25 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/examples/mt5/requirements.txt
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2020-11-01 09:55:12.000000 metaapi_cloud_sdk-9.0.0/examples/streamQuotes/
--rw-r--r--   0 roman      (501) staff       (20)     1877 2020-08-11 16:10:20.000000 metaapi_cloud_sdk-9.0.0/examples/streamQuotes/.env
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2020-11-01 09:55:12.000000 metaapi_cloud_sdk-9.0.0/examples/streamQuotes/.metaapi/
--rw-r--r--   0 roman      (501) staff       (20)      230 2020-10-28 14:53:35.000000 metaapi_cloud_sdk-9.0.0/examples/streamQuotes/.metaapi/96d1b1d9-b651-47ec-9f10-97a7c5c9fb67-deals.bin
--rw-r--r--   0 roman      (501) staff       (20)     8287 2020-10-28 14:53:35.000000 metaapi_cloud_sdk-9.0.0/examples/streamQuotes/.metaapi/96d1b1d9-b651-47ec-9f10-97a7c5c9fb67-historyOrders.bin
--rw-r--r--   0 roman      (501) staff       (20)       25 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/examples/streamQuotes/requirements.txt
--rw-r--r--   0 roman      (501) staff       (20)     1771 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/examples/streamQuotes/streamQuotes.py
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2020-11-01 09:55:12.000000 metaapi_cloud_sdk-9.0.0/lib/
--rw-r--r--   0 roman      (501) staff       (20)      277 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/__init__.py
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2020-11-01 09:55:12.000000 metaapi_cloud_sdk-9.0.0/lib/clients/
--rw-r--r--   0 roman      (501) staff       (20)       52 2020-07-11 06:42:47.000000 metaapi_cloud_sdk-9.0.0/lib/clients/__init__.py
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2020-11-01 09:55:12.000000 metaapi_cloud_sdk-9.0.0/lib/clients/copyFactory/
--rw-r--r--   0 roman      (501) staff       (20)        0 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/clients/copyFactory/__init__.py
--rw-r--r--   0 roman      (501) staff       (20)     9196 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/clients/copyFactory/configuration_client.py
--rw-r--r--   0 roman      (501) staff       (20)    16963 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/clients/copyFactory/configuration_client_test.py
--rw-r--r--   0 roman      (501) staff       (20)    17341 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/clients/copyFactory/copyFactory_models.py
--rw-r--r--   0 roman      (501) staff       (20)     7932 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/clients/copyFactory/history_client.py
--rw-r--r--   0 roman      (501) staff       (20)    12740 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/clients/copyFactory/history_client_test.py
--rw-r--r--   0 roman      (501) staff       (20)     3573 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/clients/copyFactory/trading_client.py
--rw-r--r--   0 roman      (501) staff       (20)     5232 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/clients/copyFactory/trading_client_test.py
--rw-r--r--   0 roman      (501) staff       (20)     3296 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/clients/errorHandler.py
--rw-r--r--   0 roman      (501) staff       (20)     3077 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/clients/httpClient.py
--rw-r--r--   0 roman      (501) staff       (20)     3132 2020-08-21 23:43:50.000000 metaapi_cloud_sdk-9.0.0/lib/clients/httpClient_test.py
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2020-11-01 09:55:12.000000 metaapi_cloud_sdk-9.0.0/lib/clients/metaApi/
--rw-r--r--   0 roman      (501) staff       (20)        0 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/clients/metaApi/__init__.py
--rw-r--r--   0 roman      (501) staff       (20)    49502 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/clients/metaApi/metaApiWebsocket_client.py
--rw-r--r--   0 roman      (501) staff       (20)    44058 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/clients/metaApi/metaApiWebsocket_client_test.py
--rw-r--r--   0 roman      (501) staff       (20)    13214 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/clients/metaApi/metatraderAccount_client.py
--rw-r--r--   0 roman      (501) staff       (20)    13678 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/clients/metaApi/metatraderAccount_client_test.py
--rw-r--r--   0 roman      (501) staff       (20)      356 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/clients/metaApi/notConnectedException.py
--rw-r--r--   0 roman      (501) staff       (20)      516 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/clients/metaApi/notSynchronizedException.py
--rw-r--r--   0 roman      (501) staff       (20)     5837 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/clients/metaApi/packetOrderer.py
--rw-r--r--   0 roman      (501) staff       (20)    11587 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/clients/metaApi/packetOrderer_test.py
--rw-r--r--   0 roman      (501) staff       (20)     7630 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/clients/metaApi/provisioningProfile_client.py
--rw-r--r--   0 roman      (501) staff       (20)     8989 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/clients/metaApi/provisioningProfile_client_test.py
--rw-r--r--   0 roman      (501) staff       (20)      393 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/clients/metaApi/reconnectListener.py
--rw-r--r--   0 roman      (501) staff       (20)     5821 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/clients/metaApi/synchronizationListener.py
--rw-r--r--   0 roman      (501) staff       (20)      478 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/clients/metaApi/tradeException.py
--rw-r--r--   0 roman      (501) staff       (20)     1744 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/clients/metaApi_client.py
--rw-r--r--   0 roman      (501) staff       (20)     2344 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/clients/metaApi_client_test.py
--rw-r--r--   0 roman      (501) staff       (20)     1013 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/clients/methodAccessException.py
--rw-r--r--   0 roman      (501) staff       (20)      358 2020-06-27 16:25:18.000000 metaapi_cloud_sdk-9.0.0/lib/clients/timeoutException.py
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2020-11-01 09:55:12.000000 metaapi_cloud_sdk-9.0.0/lib/copyFactory/
--rw-r--r--   0 roman      (501) staff       (20)     1537 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/copyFactory/copyFactory.py
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2020-11-01 09:55:12.000000 metaapi_cloud_sdk-9.0.0/lib/integration_tests/
--rw-r--r--   0 roman      (501) staff       (20)        0 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/integration_tests/__init__.py
--rw-r--r--   0 roman      (501) staff       (20)     3078 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/integration_tests/doubleSynchronizationTest_test.py
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2020-11-01 09:55:12.000000 metaapi_cloud_sdk-9.0.0/lib/integration_tests/files/
--rw-r--r--   0 roman      (501) staff       (20)    35784 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/integration_tests/files/servers.dat
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2020-11-01 09:55:12.000000 metaapi_cloud_sdk-9.0.0/lib/metaApi/
--rw-r--r--   0 roman      (501) staff       (20)        0 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/metaApi/__init__.py
--rw-r--r--   0 roman      (501) staff       (20)     2272 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/metaApi/connectionRegistry.py
--rw-r--r--   0 roman      (501) staff       (20)     1002 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/metaApi/connectionRegistryModel.py
--rw-r--r--   0 roman      (501) staff       (20)     4412 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/metaApi/connectionRegistry_test.py
--rw-r--r--   0 roman      (501) staff       (20)     8412 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/metaApi/historyFileManager.py
--rw-r--r--   0 roman      (501) staff       (20)    10853 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/metaApi/historyFileManager_test.py
--rw-r--r--   0 roman      (501) staff       (20)     3464 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/metaApi/historyStorage.py
--rw-r--r--   0 roman      (501) staff       (20)     6169 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/metaApi/memoryHistoryStorage.py
--rw-r--r--   0 roman      (501) staff       (20)      769 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/metaApi/memoryHistoryStorageModel.py
--rw-r--r--   0 roman      (501) staff       (20)     9291 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/metaApi/memoryHistoryStorage_test.py
--rw-r--r--   0 roman      (501) staff       (20)     2597 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/metaApi/metaApi.py
--rw-r--r--   0 roman      (501) staff       (20)    31165 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/metaApi/metaApiConnection.py
--rw-r--r--   0 roman      (501) staff       (20)    33181 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/metaApi/metaApiConnection_test.py
--rw-r--r--   0 roman      (501) staff       (20)    11732 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/metaApi/metatraderAccount.py
--rw-r--r--   0 roman      (501) staff       (20)     3215 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/metaApi/metatraderAccountApi.py
--rw-r--r--   0 roman      (501) staff       (20)    27075 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/metaApi/metatraderAccountApi_test.py
--rw-r--r--   0 roman      (501) staff       (20)     6878 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/metaApi/metatraderAccountModel.py
--rw-r--r--   0 roman      (501) staff       (20)    24706 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/metaApi/models.py
--rw-r--r--   0 roman      (501) staff       (20)     3429 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/metaApi/provisioningProfile.py
--rw-r--r--   0 roman      (501) staff       (20)     2389 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/metaApi/provisioningProfileApi.py
--rw-r--r--   0 roman      (501) staff       (20)     7151 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/metaApi/provisioningProfileApi_test.py
--rw-r--r--   0 roman      (501) staff       (20)    10480 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/metaApi/terminalState.py
--rw-r--r--   0 roman      (501) staff       (20)     6327 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/lib/metaApi/terminalState_test.py
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2020-11-01 09:55:12.000000 metaapi_cloud_sdk-9.0.0/metaapi_cloud_sdk.egg-info/
--rw-r--r--   0 roman      (501) staff       (20)    27849 2020-11-01 09:55:12.000000 metaapi_cloud_sdk-9.0.0/metaapi_cloud_sdk.egg-info/PKG-INFO
--rw-r--r--   0 roman      (501) staff       (20)     3825 2020-11-01 09:55:12.000000 metaapi_cloud_sdk-9.0.0/metaapi_cloud_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 roman      (501) staff       (20)        1 2020-11-01 09:55:12.000000 metaapi_cloud_sdk-9.0.0/metaapi_cloud_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 roman      (501) staff       (20)      151 2020-11-01 09:55:12.000000 metaapi_cloud_sdk-9.0.0/metaapi_cloud_sdk.egg-info/requires.txt
--rw-r--r--   0 roman      (501) staff       (20)       18 2020-11-01 09:55:12.000000 metaapi_cloud_sdk-9.0.0/metaapi_cloud_sdk.egg-info/top_level.txt
--rw-r--r--   0 roman      (501) staff       (20)       38 2020-11-01 09:55:12.000000 metaapi_cloud_sdk-9.0.0/setup.cfg
--rw-r--r--   0 roman      (501) staff       (20)     1714 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.0.0/setup.py
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2020-11-08 14:33:03.271066 metaapi_cloud_sdk-9.1.0/
+-rw-r--r--   0 roman      (501) staff       (20)      780 2020-06-27 16:25:18.000000 metaapi_cloud_sdk-9.1.0/LICENSE
+-rw-r--r--   0 roman      (501) staff       (20)      142 2020-06-27 21:51:26.000000 metaapi_cloud_sdk-9.1.0/MANIFEST.in
+-rw-r--r--   0 roman      (501) staff       (20)    28925 2020-11-08 14:33:03.270708 metaapi_cloud_sdk-9.1.0/PKG-INFO
+-rw-r--r--   0 roman      (501) staff       (20)    23447 2020-11-08 14:32:36.000000 metaapi_cloud_sdk-9.1.0/README.rst
+-rw-r--r--   0 roman      (501) staff       (20)     4941 2020-11-08 14:32:36.000000 metaapi_cloud_sdk-9.1.0/changelog.md
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2020-11-08 14:33:02.900947 metaapi_cloud_sdk-9.1.0/examples/
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2020-11-08 14:33:02.907426 metaapi_cloud_sdk-9.1.0/examples/exampleGenerator/
+-rw-r--r--   0 roman      (501) staff       (20)       25 2020-11-08 14:32:36.000000 metaapi_cloud_sdk-9.1.0/examples/exampleGenerator/requirements.txt
+-rw-r--r--   0 roman      (501) staff       (20)     3305 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/examples/exampleGenerator/rpcExample.py
+-rw-r--r--   0 roman      (501) staff       (20)     2657 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/examples/exampleGenerator/synchronizationExample.py
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2020-11-08 14:33:02.910831 metaapi_cloud_sdk-9.1.0/examples/mt4/
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2020-11-08 14:33:02.971031 metaapi_cloud_sdk-9.1.0/examples/mt4/.metaapi/
+-rw-r--r--   0 roman      (501) staff       (20)  1931916 2020-10-28 14:51:04.000000 metaapi_cloud_sdk-9.1.0/examples/mt4/.metaapi/11779f61-9dc5-4292-807b-f52906804439-deals.bin
+-rw-r--r--   0 roman      (501) staff       (20)  5755801 2020-10-28 14:51:04.000000 metaapi_cloud_sdk-9.1.0/examples/mt4/.metaapi/11779f61-9dc5-4292-807b-f52906804439-historyOrders.bin
+-rw-r--r--   0 roman      (501) staff       (20)     2527 2020-09-12 22:25:43.000000 metaapi_cloud_sdk-9.1.0/examples/mt4/.metaapi/9c283a6c-5c41-4351-a6e5-d974970ace0e-deals.bin
+-rw-r--r--   0 roman      (501) staff       (20)  3552802 2020-09-12 22:25:43.000000 metaapi_cloud_sdk-9.1.0/examples/mt4/.metaapi/9c283a6c-5c41-4351-a6e5-d974970ace0e-historyOrders.bin
+-rw-r--r--   0 roman      (501) staff       (20)     5013 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/examples/mt4/metaApiRpcExample.py
+-rw-r--r--   0 roman      (501) staff       (20)     4368 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/examples/mt4/metaApiSynchronizationExample.py
+-rw-r--r--   0 roman      (501) staff       (20)       25 2020-11-08 14:32:36.000000 metaapi_cloud_sdk-9.1.0/examples/mt4/requirements.txt
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2020-11-08 14:33:03.003063 metaapi_cloud_sdk-9.1.0/examples/mt5/
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2020-11-08 14:33:03.071995 metaapi_cloud_sdk-9.1.0/examples/mt5/.metaapi/
+-rw-r--r--   0 roman      (501) staff       (20)  1012522 2020-09-12 20:36:52.000000 metaapi_cloud_sdk-9.1.0/examples/mt5/.metaapi/76037e9a-ab26-4138-9013-496034dda8eb-deals.bin
+-rw-r--r--   0 roman      (501) staff       (20)   558532 2020-09-12 20:36:52.000000 metaapi_cloud_sdk-9.1.0/examples/mt5/.metaapi/76037e9a-ab26-4138-9013-496034dda8eb-historyOrders.bin
+-rw-r--r--   0 roman      (501) staff       (20)    82452 2020-09-12 21:06:51.000000 metaapi_cloud_sdk-9.1.0/examples/mt5/.metaapi/92b4a96e-0dbb-4bb5-924e-3d78dc097f81-deals.bin
+-rw-r--r--   0 roman      (501) staff       (20)  1700153 2020-09-12 21:06:51.000000 metaapi_cloud_sdk-9.1.0/examples/mt5/.metaapi/92b4a96e-0dbb-4bb5-924e-3d78dc097f81-historyOrders.bin
+-rw-r--r--   0 roman      (501) staff       (20)  1931056 2020-09-05 07:19:11.000000 metaapi_cloud_sdk-9.1.0/examples/mt5/.metaapi/a9fb463b-44d9-4336-a88f-3e458b02689f-deals.bin
+-rw-r--r--   0 roman      (501) staff       (20)  2409166 2020-09-05 07:19:11.000000 metaapi_cloud_sdk-9.1.0/examples/mt5/.metaapi/a9fb463b-44d9-4336-a88f-3e458b02689f-historyOrders.bin
+-rw-r--r--   0 roman      (501) staff       (20)     4997 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/examples/mt5/metaApiRpcExample.py
+-rw-r--r--   0 roman      (501) staff       (20)     4398 2020-11-08 14:32:36.000000 metaapi_cloud_sdk-9.1.0/examples/mt5/metaApiSynchronizationExample.py
+-rw-r--r--   0 roman      (501) staff       (20)       25 2020-11-08 14:32:36.000000 metaapi_cloud_sdk-9.1.0/examples/mt5/requirements.txt
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2020-11-08 14:33:03.100602 metaapi_cloud_sdk-9.1.0/examples/streamQuotes/
+-rw-r--r--   0 roman      (501) staff       (20)     1877 2020-08-11 16:10:20.000000 metaapi_cloud_sdk-9.1.0/examples/streamQuotes/.env
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2020-11-08 14:33:03.103287 metaapi_cloud_sdk-9.1.0/examples/streamQuotes/.metaapi/
+-rw-r--r--   0 roman      (501) staff       (20)      230 2020-10-28 14:53:35.000000 metaapi_cloud_sdk-9.1.0/examples/streamQuotes/.metaapi/96d1b1d9-b651-47ec-9f10-97a7c5c9fb67-deals.bin
+-rw-r--r--   0 roman      (501) staff       (20)     8287 2020-10-28 14:53:35.000000 metaapi_cloud_sdk-9.1.0/examples/streamQuotes/.metaapi/96d1b1d9-b651-47ec-9f10-97a7c5c9fb67-historyOrders.bin
+-rw-r--r--   0 roman      (501) staff       (20)       25 2020-11-08 14:32:36.000000 metaapi_cloud_sdk-9.1.0/examples/streamQuotes/requirements.txt
+-rw-r--r--   0 roman      (501) staff       (20)     1771 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/examples/streamQuotes/streamQuotes.py
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2020-11-08 14:33:03.105993 metaapi_cloud_sdk-9.1.0/lib/
+-rw-r--r--   0 roman      (501) staff       (20)      277 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/__init__.py
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2020-11-08 14:33:03.124349 metaapi_cloud_sdk-9.1.0/lib/clients/
+-rw-r--r--   0 roman      (501) staff       (20)       52 2020-07-11 06:42:47.000000 metaapi_cloud_sdk-9.1.0/lib/clients/__init__.py
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2020-11-08 14:33:03.139177 metaapi_cloud_sdk-9.1.0/lib/clients/copyFactory/
+-rw-r--r--   0 roman      (501) staff       (20)        0 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/clients/copyFactory/__init__.py
+-rw-r--r--   0 roman      (501) staff       (20)     9196 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/clients/copyFactory/configuration_client.py
+-rw-r--r--   0 roman      (501) staff       (20)    16963 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/clients/copyFactory/configuration_client_test.py
+-rw-r--r--   0 roman      (501) staff       (20)    17341 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/clients/copyFactory/copyFactory_models.py
+-rw-r--r--   0 roman      (501) staff       (20)     7932 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/clients/copyFactory/history_client.py
+-rw-r--r--   0 roman      (501) staff       (20)    12740 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/clients/copyFactory/history_client_test.py
+-rw-r--r--   0 roman      (501) staff       (20)     3573 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/clients/copyFactory/trading_client.py
+-rw-r--r--   0 roman      (501) staff       (20)     5232 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/clients/copyFactory/trading_client_test.py
+-rw-r--r--   0 roman      (501) staff       (20)     3296 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/clients/errorHandler.py
+-rw-r--r--   0 roman      (501) staff       (20)     3077 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/clients/httpClient.py
+-rw-r--r--   0 roman      (501) staff       (20)     3132 2020-08-21 23:43:50.000000 metaapi_cloud_sdk-9.1.0/lib/clients/httpClient_test.py
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2020-11-08 14:33:03.186363 metaapi_cloud_sdk-9.1.0/lib/clients/metaApi/
+-rw-r--r--   0 roman      (501) staff       (20)        0 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/clients/metaApi/__init__.py
+-rw-r--r--   0 roman      (501) staff       (20)    49340 2020-11-08 14:32:36.000000 metaapi_cloud_sdk-9.1.0/lib/clients/metaApi/metaApiWebsocket_client.py
+-rw-r--r--   0 roman      (501) staff       (20)    44058 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/clients/metaApi/metaApiWebsocket_client_test.py
+-rw-r--r--   0 roman      (501) staff       (20)    13214 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/clients/metaApi/metatraderAccount_client.py
+-rw-r--r--   0 roman      (501) staff       (20)    13678 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/clients/metaApi/metatraderAccount_client_test.py
+-rw-r--r--   0 roman      (501) staff       (20)     3872 2020-11-08 14:32:36.000000 metaapi_cloud_sdk-9.1.0/lib/clients/metaApi/metatraderDemoAccount_client.py
+-rw-r--r--   0 roman      (501) staff       (20)     4138 2020-11-08 14:32:36.000000 metaapi_cloud_sdk-9.1.0/lib/clients/metaApi/metatraderDemoAccount_client_test.py
+-rw-r--r--   0 roman      (501) staff       (20)      356 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/clients/metaApi/notConnectedException.py
+-rw-r--r--   0 roman      (501) staff       (20)      516 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/clients/metaApi/notSynchronizedException.py
+-rw-r--r--   0 roman      (501) staff       (20)     5867 2020-11-08 14:32:36.000000 metaapi_cloud_sdk-9.1.0/lib/clients/metaApi/packetOrderer.py
+-rw-r--r--   0 roman      (501) staff       (20)    12393 2020-11-08 14:32:36.000000 metaapi_cloud_sdk-9.1.0/lib/clients/metaApi/packetOrderer_test.py
+-rw-r--r--   0 roman      (501) staff       (20)     7630 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/clients/metaApi/provisioningProfile_client.py
+-rw-r--r--   0 roman      (501) staff       (20)     8989 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/clients/metaApi/provisioningProfile_client_test.py
+-rw-r--r--   0 roman      (501) staff       (20)      393 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/clients/metaApi/reconnectListener.py
+-rw-r--r--   0 roman      (501) staff       (20)     5821 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/clients/metaApi/synchronizationListener.py
+-rw-r--r--   0 roman      (501) staff       (20)      478 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/clients/metaApi/tradeException.py
+-rw-r--r--   0 roman      (501) staff       (20)     1744 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/clients/metaApi_client.py
+-rw-r--r--   0 roman      (501) staff       (20)     2344 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/clients/metaApi_client_test.py
+-rw-r--r--   0 roman      (501) staff       (20)     1013 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/clients/methodAccessException.py
+-rw-r--r--   0 roman      (501) staff       (20)      358 2020-06-27 16:25:18.000000 metaapi_cloud_sdk-9.1.0/lib/clients/timeoutException.py
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2020-11-08 14:33:03.190252 metaapi_cloud_sdk-9.1.0/lib/copyFactory/
+-rw-r--r--   0 roman      (501) staff       (20)     1537 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/copyFactory/copyFactory.py
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2020-11-08 14:33:03.195792 metaapi_cloud_sdk-9.1.0/lib/integration_tests/
+-rw-r--r--   0 roman      (501) staff       (20)        0 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/integration_tests/__init__.py
+-rw-r--r--   0 roman      (501) staff       (20)     3078 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/integration_tests/doubleSynchronizationTest_test.py
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2020-11-08 14:33:03.197903 metaapi_cloud_sdk-9.1.0/lib/integration_tests/files/
+-rw-r--r--   0 roman      (501) staff       (20)    35784 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/integration_tests/files/servers.dat
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2020-11-08 14:33:03.257708 metaapi_cloud_sdk-9.1.0/lib/metaApi/
+-rw-r--r--   0 roman      (501) staff       (20)        0 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/metaApi/__init__.py
+-rw-r--r--   0 roman      (501) staff       (20)     2272 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/metaApi/connectionRegistry.py
+-rw-r--r--   0 roman      (501) staff       (20)     1002 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/metaApi/connectionRegistryModel.py
+-rw-r--r--   0 roman      (501) staff       (20)     4412 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/metaApi/connectionRegistry_test.py
+-rw-r--r--   0 roman      (501) staff       (20)     8412 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/metaApi/historyFileManager.py
+-rw-r--r--   0 roman      (501) staff       (20)    10853 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/metaApi/historyFileManager_test.py
+-rw-r--r--   0 roman      (501) staff       (20)     3464 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/metaApi/historyStorage.py
+-rw-r--r--   0 roman      (501) staff       (20)     6169 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/metaApi/memoryHistoryStorage.py
+-rw-r--r--   0 roman      (501) staff       (20)      769 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/metaApi/memoryHistoryStorageModel.py
+-rw-r--r--   0 roman      (501) staff       (20)     9291 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/metaApi/memoryHistoryStorage_test.py
+-rw-r--r--   0 roman      (501) staff       (20)     3215 2020-11-08 14:32:36.000000 metaapi_cloud_sdk-9.1.0/lib/metaApi/metaApi.py
+-rw-r--r--   0 roman      (501) staff       (20)    31165 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/metaApi/metaApiConnection.py
+-rw-r--r--   0 roman      (501) staff       (20)    33181 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/metaApi/metaApiConnection_test.py
+-rw-r--r--   0 roman      (501) staff       (20)    11732 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/metaApi/metatraderAccount.py
+-rw-r--r--   0 roman      (501) staff       (20)     3215 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/metaApi/metatraderAccountApi.py
+-rw-r--r--   0 roman      (501) staff       (20)    27075 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/metaApi/metatraderAccountApi_test.py
+-rw-r--r--   0 roman      (501) staff       (20)     6878 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/metaApi/metatraderAccountModel.py
+-rw-r--r--   0 roman      (501) staff       (20)     1137 2020-11-08 14:32:36.000000 metaapi_cloud_sdk-9.1.0/lib/metaApi/metatraderDemoAccount.py
+-rw-r--r--   0 roman      (501) staff       (20)     1592 2020-11-08 14:32:36.000000 metaapi_cloud_sdk-9.1.0/lib/metaApi/metatraderDemoAccountApi.py
+-rw-r--r--   0 roman      (501) staff       (20)     2977 2020-11-08 14:32:36.000000 metaapi_cloud_sdk-9.1.0/lib/metaApi/metatraderDemoAccountApi_test.py
+-rw-r--r--   0 roman      (501) staff       (20)    24706 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/metaApi/models.py
+-rw-r--r--   0 roman      (501) staff       (20)     3429 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/metaApi/provisioningProfile.py
+-rw-r--r--   0 roman      (501) staff       (20)     2389 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/metaApi/provisioningProfileApi.py
+-rw-r--r--   0 roman      (501) staff       (20)     7151 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/metaApi/provisioningProfileApi_test.py
+-rw-r--r--   0 roman      (501) staff       (20)    10480 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/metaApi/terminalState.py
+-rw-r--r--   0 roman      (501) staff       (20)     6327 2020-11-01 09:50:11.000000 metaapi_cloud_sdk-9.1.0/lib/metaApi/terminalState_test.py
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2020-11-08 14:33:03.270043 metaapi_cloud_sdk-9.1.0/metaapi_cloud_sdk.egg-info/
+-rw-r--r--   0 roman      (501) staff       (20)    28925 2020-11-08 14:33:02.000000 metaapi_cloud_sdk-9.1.0/metaapi_cloud_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 roman      (501) staff       (20)     4056 2020-11-08 14:33:02.000000 metaapi_cloud_sdk-9.1.0/metaapi_cloud_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 roman      (501) staff       (20)        1 2020-11-08 14:33:02.000000 metaapi_cloud_sdk-9.1.0/metaapi_cloud_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 roman      (501) staff       (20)      151 2020-11-08 14:33:02.000000 metaapi_cloud_sdk-9.1.0/metaapi_cloud_sdk.egg-info/requires.txt
+-rw-r--r--   0 roman      (501) staff       (20)       18 2020-11-08 14:33:02.000000 metaapi_cloud_sdk-9.1.0/metaapi_cloud_sdk.egg-info/top_level.txt
+-rw-r--r--   0 roman      (501) staff       (20)       38 2020-11-08 14:33:03.271157 metaapi_cloud_sdk-9.1.0/setup.cfg
+-rw-r--r--   0 roman      (501) staff       (20)     1714 2020-11-08 14:32:36.000000 metaapi_cloud_sdk-9.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `metaapi_cloud_sdk-9.0.0/LICENSE` & `metaapi_cloud_sdk-9.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/PKG-INFO` & `metaapi_cloud_sdk-9.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaapi_cloud_sdk
-Version: 9.0.0
+Version: 9.1.0
 Summary: SDK for MetaApi, a professional cloud forex API which includes MetaTrader REST API and MetaTrader websocket API. Supports both MetaTrader 5 (MT5) and MetaTrader 4 (MT4). CopyFactorycopy trading API included. (https://metaapi.cloud)
 Home-page: https://github.com/agiliumtrade-ai/metaapi-python-sdk
 Author: Agilium Labs LLC
 Author-email: agiliumtrade@agiliumtrade.ai
 License: SEE LICENSE IN LICENSE
 Description: metaapi.cloud SDK for Python
         ############################
@@ -364,14 +364,40 @@
             print(await connection.cancel_order('46870472'))
         
             # if you need to, check the extra result information in stringCode and numericCode properties of the response
             result = await connection.create_market_buy_order('GBPUSD', 0.07, 0.9, 2.0, {'comment': 'comment',
                                                                                          'clientId': 'TE_GBPUSD_7hyINWqAl'})
             print('Trade successful, result code is ' + result['stringCode'])
         
+        Managing MetaTrader demo accounts via API
+        ===========================================
+        Please note that not all MT4/MT5 servers allows you to create demo accounts using the method below.
+        
+        Create a MetaTrader 4 demo account
+        ----------------------------------
+        .. code-block:: python
+        
+            demo_account = await api.metatrader_demo_account_api.create_mt4_demo_account(provisioningProfile.id, {
+                'balance': 100000,
+                'email': 'example@example.com',
+                'leverage': 100,
+                'serverName': 'Exness-Trial4'
+            })
+        
+        Create a MetaTrader 5 demo account
+        ----------------------------------
+        .. code-block:: python
+        
+            demo_account = await api.metatrader_demo_account_api.create_mt5_demo_account(provisioningProfile.id, {
+                'balance': 100000,
+                'email': 'example@example.com',
+                'leverage': 100,
+                'serverName': 'ICMarketsSC-Demo'
+            })
+        
         CopyFactory copy trading API (experimental)
         ===========================================
         
         CopyFactory is a powerful trade copying API which makes developing forex
         trade copying applications as easy as writing few lines of code.
         
         At this point this feature is experimental and we have not yet defined a final price for it.
```

### Comparing `metaapi_cloud_sdk-9.0.0/README.rst` & `metaapi_cloud_sdk-9.1.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -356,14 +356,40 @@
     print(await connection.cancel_order('46870472'))
 
     # if you need to, check the extra result information in stringCode and numericCode properties of the response
     result = await connection.create_market_buy_order('GBPUSD', 0.07, 0.9, 2.0, {'comment': 'comment',
                                                                                  'clientId': 'TE_GBPUSD_7hyINWqAl'})
     print('Trade successful, result code is ' + result['stringCode'])
 
+Managing MetaTrader demo accounts via API
+===========================================
+Please note that not all MT4/MT5 servers allows you to create demo accounts using the method below.
+
+Create a MetaTrader 4 demo account
+----------------------------------
+.. code-block:: python
+
+    demo_account = await api.metatrader_demo_account_api.create_mt4_demo_account(provisioningProfile.id, {
+        'balance': 100000,
+        'email': 'example@example.com',
+        'leverage': 100,
+        'serverName': 'Exness-Trial4'
+    })
+
+Create a MetaTrader 5 demo account
+----------------------------------
+.. code-block:: python
+
+    demo_account = await api.metatrader_demo_account_api.create_mt5_demo_account(provisioningProfile.id, {
+        'balance': 100000,
+        'email': 'example@example.com',
+        'leverage': 100,
+        'serverName': 'ICMarketsSC-Demo'
+    })
+
 CopyFactory copy trading API (experimental)
 ===========================================
 
 CopyFactory is a powerful trade copying API which makes developing forex
 trade copying applications as easy as writing few lines of code.
 
 At this point this feature is experimental and we have not yet defined a final price for it.
```

### Comparing `metaapi_cloud_sdk-9.0.0/changelog.md` & `metaapi_cloud_sdk-9.1.0/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+9.1.0
+  - added API to register MetaTrader demo accounts
+  - fixed packet orderer to do not cause unnecessary resynchronization
+
 9.0.0
   - added contractSize field to MetatraderSymbolSpecification model
   - added quoteSessions and tradeSessions to MetatraderSymbolSpecification model
   - added more fields to MetatraderSymbolSpecification model
   - breaking change: add on_positions_replaced and on_order_replaced events into SynchronizationListener and no longer invoke on_position_updated and on_order_updated during initial synchronization
   - removed excessive log message from subscribe API
   - breaking change: introduced synchronizationStarted event to increase synchronization stability
```

### Comparing `metaapi_cloud_sdk-9.0.0/examples/exampleGenerator/rpcExample.py` & `metaapi_cloud_sdk-9.1.0/examples/exampleGenerator/rpcExample.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/examples/exampleGenerator/synchronizationExample.py` & `metaapi_cloud_sdk-9.1.0/examples/exampleGenerator/synchronizationExample.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/examples/mt4/.metaapi/11779f61-9dc5-4292-807b-f52906804439-deals.bin` & `metaapi_cloud_sdk-9.1.0/examples/mt4/.metaapi/11779f61-9dc5-4292-807b-f52906804439-deals.bin`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/examples/mt4/.metaapi/11779f61-9dc5-4292-807b-f52906804439-historyOrders.bin` & `metaapi_cloud_sdk-9.1.0/examples/mt4/.metaapi/11779f61-9dc5-4292-807b-f52906804439-historyOrders.bin`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/examples/mt4/.metaapi/9c283a6c-5c41-4351-a6e5-d974970ace0e-deals.bin` & `metaapi_cloud_sdk-9.1.0/examples/mt4/.metaapi/9c283a6c-5c41-4351-a6e5-d974970ace0e-deals.bin`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/examples/mt4/.metaapi/9c283a6c-5c41-4351-a6e5-d974970ace0e-historyOrders.bin` & `metaapi_cloud_sdk-9.1.0/examples/mt4/.metaapi/9c283a6c-5c41-4351-a6e5-d974970ace0e-historyOrders.bin`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/examples/mt4/metaApiRpcExample.py` & `metaapi_cloud_sdk-9.1.0/examples/mt4/metaApiRpcExample.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/examples/mt4/metaApiSynchronizationExample.py` & `metaapi_cloud_sdk-9.1.0/examples/mt4/metaApiSynchronizationExample.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/examples/mt5/.metaapi/76037e9a-ab26-4138-9013-496034dda8eb-deals.bin` & `metaapi_cloud_sdk-9.1.0/examples/mt5/.metaapi/76037e9a-ab26-4138-9013-496034dda8eb-deals.bin`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/examples/mt5/.metaapi/76037e9a-ab26-4138-9013-496034dda8eb-historyOrders.bin` & `metaapi_cloud_sdk-9.1.0/examples/mt5/.metaapi/76037e9a-ab26-4138-9013-496034dda8eb-historyOrders.bin`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/examples/mt5/.metaapi/92b4a96e-0dbb-4bb5-924e-3d78dc097f81-deals.bin` & `metaapi_cloud_sdk-9.1.0/examples/mt5/.metaapi/92b4a96e-0dbb-4bb5-924e-3d78dc097f81-deals.bin`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/examples/mt5/.metaapi/92b4a96e-0dbb-4bb5-924e-3d78dc097f81-historyOrders.bin` & `metaapi_cloud_sdk-9.1.0/examples/mt5/.metaapi/92b4a96e-0dbb-4bb5-924e-3d78dc097f81-historyOrders.bin`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/examples/mt5/.metaapi/a9fb463b-44d9-4336-a88f-3e458b02689f-deals.bin` & `metaapi_cloud_sdk-9.1.0/examples/mt5/.metaapi/a9fb463b-44d9-4336-a88f-3e458b02689f-deals.bin`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/examples/mt5/.metaapi/a9fb463b-44d9-4336-a88f-3e458b02689f-historyOrders.bin` & `metaapi_cloud_sdk-9.1.0/examples/mt5/.metaapi/a9fb463b-44d9-4336-a88f-3e458b02689f-historyOrders.bin`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/examples/mt5/metaApiRpcExample.py` & `metaapi_cloud_sdk-9.1.0/examples/mt5/metaApiRpcExample.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/examples/mt5/metaApiSynchronizationExample.py` & `metaapi_cloud_sdk-9.1.0/examples/mt5/metaApiSynchronizationExample.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 token = os.getenv('TOKEN') or '<put in your token here>'
 login = os.getenv('LOGIN') or '<put in your MT login here>'
 password = os.getenv('PASSWORD') or '<put in your MT password here>'
 server_name = os.getenv('SERVER') or '<put in your MT server name here>'
 server_dat_file = os.getenv('PATH_TO_SERVERS_DAT') or '/path/to/your/servers.dat'
 api = MetaApi(token)
 
+
 async def test_meta_api_synchronization():
     try:
         profiles = await api.provisioning_profile_api.get_provisioning_profiles()
 
         # create test MetaTrader account profile
         profile = None
         for item in profiles:
```

### Comparing `metaapi_cloud_sdk-9.0.0/examples/streamQuotes/.env` & `metaapi_cloud_sdk-9.1.0/examples/streamQuotes/.env`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/examples/streamQuotes/.metaapi/96d1b1d9-b651-47ec-9f10-97a7c5c9fb67-historyOrders.bin` & `metaapi_cloud_sdk-9.1.0/examples/streamQuotes/.metaapi/96d1b1d9-b651-47ec-9f10-97a7c5c9fb67-historyOrders.bin`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/examples/streamQuotes/streamQuotes.py` & `metaapi_cloud_sdk-9.1.0/examples/streamQuotes/streamQuotes.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/clients/copyFactory/configuration_client.py` & `metaapi_cloud_sdk-9.1.0/lib/clients/copyFactory/configuration_client.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/clients/copyFactory/configuration_client_test.py` & `metaapi_cloud_sdk-9.1.0/lib/clients/copyFactory/configuration_client_test.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/clients/copyFactory/copyFactory_models.py` & `metaapi_cloud_sdk-9.1.0/lib/clients/copyFactory/copyFactory_models.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/clients/copyFactory/history_client.py` & `metaapi_cloud_sdk-9.1.0/lib/clients/copyFactory/history_client.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/clients/copyFactory/history_client_test.py` & `metaapi_cloud_sdk-9.1.0/lib/clients/copyFactory/history_client_test.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/clients/copyFactory/trading_client.py` & `metaapi_cloud_sdk-9.1.0/lib/clients/copyFactory/trading_client.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/clients/copyFactory/trading_client_test.py` & `metaapi_cloud_sdk-9.1.0/lib/clients/copyFactory/trading_client_test.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/clients/errorHandler.py` & `metaapi_cloud_sdk-9.1.0/lib/clients/errorHandler.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/clients/httpClient.py` & `metaapi_cloud_sdk-9.1.0/lib/clients/httpClient.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/clients/httpClient_test.py` & `metaapi_cloud_sdk-9.1.0/lib/clients/httpClient_test.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/clients/metaApi/metaApiWebsocket_client.py` & `metaapi_cloud_sdk-9.1.0/lib/clients/metaApi/metaApiWebsocket_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,18 +50,16 @@
             account_id: Account id.
             expected_sequence_number: Expected s/n.
             actual_sequence_number: Actual s/n.
             packet: Packet data.
             received_at: Time the packet was received at.
         """
         print(f'[{datetime.now().isoformat()}] MetaApi websocket client received an out of order packet type ' +
-              f'{packet["type"]} for account id {account_id}. ' +
-              (f'Expected s/n {expected_sequence_number} does not match the actual of {actual_sequence_number}' if
-               expected_sequence_number != -1 else
-               f'Packet with s/n {actual_sequence_number} has come before initial synchronization packet'))
+              f'{packet["type"]} for account id {account_id}. Expected s/n {expected_sequence_number} does not ' +
+              f'match the actual of {actual_sequence_number}')
         self.subscribe(account_id)
 
     def set_url(self, url: str):
         """Patch server URL for use in unit tests
 
         Args:
             url: Patched server URL.
```

### Comparing `metaapi_cloud_sdk-9.0.0/lib/clients/metaApi/metaApiWebsocket_client_test.py` & `metaapi_cloud_sdk-9.1.0/lib/clients/metaApi/metaApiWebsocket_client_test.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/clients/metaApi/metatraderAccount_client.py` & `metaapi_cloud_sdk-9.1.0/lib/clients/metaApi/metatraderAccount_client.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/clients/metaApi/metatraderAccount_client_test.py` & `metaapi_cloud_sdk-9.1.0/lib/clients/metaApi/metatraderAccount_client_test.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/clients/metaApi/notSynchronizedException.py` & `metaapi_cloud_sdk-9.1.0/lib/clients/metaApi/notSynchronizedException.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/clients/metaApi/packetOrderer.py` & `metaapi_cloud_sdk-9.1.0/lib/clients/metaApi/packetOrderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,12 +104,12 @@
         for key, wait_list in self._packetsByAccountId.items():
             if len(wait_list) and \
                     (wait_list[0][
                          'receivedAt'].timestamp() + self._orderingTimeoutInSeconds) < datetime.now().timestamp():
                 account_id = wait_list[0]['accountId']
                 if account_id not in self._isOutOfOrderEmitted or not self._isOutOfOrderEmitted[account_id]:
                     self._isOutOfOrderEmitted[account_id] = True
-                    expected_sequence_number = (self._sequenceNumberByAccount[account_id] + 1) \
-                        if account_id in self._sequenceNumberByAccount else -1
-                    self._outOfOrderListener.on_out_of_order_packet(
-                        wait_list[0]['accountId'], expected_sequence_number, wait_list[0]['sequenceNumber'],
-                        wait_list[0]['packet'], wait_list[0]['receivedAt'])
+                    # Do not emit onOutOfOrderPacket for packets that come before synchronizationStarted
+                    if account_id in self._sequenceNumberByAccount:
+                        self._outOfOrderListener.on_out_of_order_packet(
+                            wait_list[0]['accountId'], self._sequenceNumberByAccount[account_id] + 1,
+                            wait_list[0]['sequenceNumber'], wait_list[0]['packet'], wait_list[0]['receivedAt'])
```

### Comparing `metaapi_cloud_sdk-9.0.0/lib/clients/metaApi/packetOrderer_test.py` & `metaapi_cloud_sdk-9.1.0/lib/clients/metaApi/packetOrderer_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             'connectionId': 'accountId',
             'accountId': 'accountId'
         }
         assert packet_orderer.restore_order(packet_without_sn) == [packet_without_sn]
 
     @pytest.mark.asyncio
     async def test_restore(self):
-        """Should restore packet order starting from packet of specifications type."""
+        """Should restore packet order."""
         first_packet = {
             'type': 'synchronizationStarted',
             'sequenceTimestamp': 1603124267178,
             'sequenceNumber': 13,
             'synchronizationId': 'synchronizationId',
             'accountId': 'accountId'
         }
@@ -60,16 +60,16 @@
         assert packet_orderer.restore_order(second_packet) == []
         assert packet_orderer.restore_order(first_packet) == [first_packet, second_packet]
         assert packet_orderer.restore_order(fourth_packet) == []
         assert packet_orderer.restore_order(third_packet) == [third_packet, fourth_packet]
 
     @pytest.mark.asyncio
     async def test_filter_prev_sync_packets_with_specifications(self):
-        """Should filter out packets from previous synchronization attempt that includes specifications."""
-        previous_specifications = {
+        """Should filter out packets from previous synchronization attempt that includes synchronization start."""
+        previous_start = {
             'type': 'synchronizationStarted',
             'sequenceTimestamp': 1603124267178,
             'sequenceNumber': 13,
             'synchronizationId': 'synchronizationId',
             'accountId': 'accountId'
         }
         one_of_previous_packets = {
@@ -87,44 +87,44 @@
         }
         this_second_packet = {
             'type': 'prices',
             'sequenceTimestamp': 1603124268198,
             'sequenceNumber': 2,
             'accountId': 'accountId'
         }
-        assert packet_orderer.restore_order(previous_specifications) == [previous_specifications]
+        assert packet_orderer.restore_order(previous_start) == [previous_start]
         assert packet_orderer.restore_order(one_of_previous_packets) == []
         assert packet_orderer.restore_order(this_second_packet) == []
         assert packet_orderer.restore_order(this_specifications) == [this_specifications, this_second_packet]
 
     @pytest.mark.asyncio
     async def test_filter_prev_sync_packets_without_specifications(self):
-        """Should filter out packets from previous synchronization attempt that does not includes specifications."""
+        """Should filter out packets from previous synchronization attempt that does not includes the start."""
         one_of_previous_packets = {
             'type': 'positions',
             'sequenceTimestamp': 1603124267188,
             'sequenceNumber': 15,
             'accountId': 'accountId'
         }
-        this_specifications = {
+        this_start = {
             'type': 'synchronizationStarted',
             'sequenceTimestamp': 1603124267198,
             'sequenceNumber': 1,
             'synchronizationId': 'synchronizationId',
             'accountId': 'accountId'
         }
         this_second_packet = {
             'type': 'prices',
             'sequenceTimestamp': 1603124268198,
             'sequenceNumber': 2,
             'accountId': 'accountId'
         }
         assert packet_orderer.restore_order(one_of_previous_packets) == []
         assert packet_orderer.restore_order(this_second_packet) == []
-        assert packet_orderer.restore_order(this_specifications) == [this_specifications, this_second_packet]
+        assert packet_orderer.restore_order(this_start) == [this_start, this_second_packet]
 
     @pytest.mark.asyncio
     async def test_duplicate(self):
         """Should pass through duplicate packets."""
         specifications_packet = {
             'type': 'synchronizationStarted',
             'sequenceTimestamp': 1603124267198,
@@ -209,23 +209,24 @@
         }
         not_timed_out_packet = {
             'accountId': 'accountId',
             'sequenceNumber': 15,
             'packet': {},
             'receivedAt': datetime.fromtimestamp(10000000000)
         }
+        packet_orderer._sequenceNumberByAccount['accountId'] = 1
         packet_orderer._packetsByAccountId['accountId'] = [
             timed_out_packet,
             not_timed_out_packet
         ]
         await asyncio.sleep(1)
         out_of_order_listener.on_out_of_order_packet.assert_called_once()
         args_list = out_of_order_listener.on_out_of_order_packet.call_args_list[0].args
         assert args_list[0] == 'accountId'
-        assert args_list[1] == -1
+        assert args_list[1] == 2
         assert args_list[2] == 11
         assert args_list[3] == timed_out_packet['packet']
         await asyncio.sleep(1)
         out_of_order_listener.on_out_of_order_packet.assert_called_once()
 
     @pytest.mark.asyncio
     async def test_not_call_out_of_order_if_not_timeout(self):
@@ -239,22 +240,42 @@
         }
         not_timed_out_packet = {
             'accountId': 'accountId',
             'sequenceNumber': 15,
             'packet': {},
             'receivedAt': datetime.fromtimestamp(10000000000)
         }
+        packet_orderer._sequenceNumberByAccount['accountId'] = 1
         packet_orderer._packetsByAccountId['accountId'] = [
             not_timed_out_packet,
             timed_out_packet
         ]
         await asyncio.sleep(1)
         out_of_order_listener.on_out_of_order_packet.assert_not_called()
 
     @pytest.mark.asyncio
+    async def test_not_call_out_of_order_if_before_sync_start(self):
+        """Should not call on-out-of-order listener for packets that come before synchronization start."""
+        out_of_order_listener.on_out_of_order_packet = MagicMock()
+        out_of_order_packet = {
+            'accountId': 'accountId',
+            'sequenceNumber': 11,
+            'packet': {},
+            'receivedAt': date
+        }
+
+        # There were no synchronization start packets
+        if 'accountId' in packet_orderer._sequenceNumberByAccount:
+            del packet_orderer._sequenceNumberByAccount['accountId']
+
+        packet_orderer._packetsByAccountId['accountId'] = [out_of_order_packet]
+        await asyncio.sleep(1)
+        out_of_order_listener.on_out_of_order_packet.assert_not_called()
+
+    @pytest.mark.asyncio
     async def test_maintain_fixed_queue(self):
         """Should maintain a fixed queue of wait list."""
         packet_orderer._waitListSizeLimit = 1
         second_packet = {
             'type': 'prices',
             'sequenceTimestamp': 1603124267180,
             'sequenceNumber': 14,
@@ -270,18 +291,18 @@
         assert len(packet_orderer._packetsByAccountId['accountId']) == 1
         assert packet_orderer._packetsByAccountId['accountId'][0]['packet'] == second_packet
         packet_orderer.restore_order(third_packet)
         assert len(packet_orderer._packetsByAccountId['accountId']) == 1
         assert packet_orderer._packetsByAccountId['accountId'][0]['packet'] == third_packet
 
     @pytest.mark.asyncio
-    async def test_count_specification_packets_with_no_sync_id_as_out_of_order(self):
-        """Should count specification packets with undefined synchronziationId as out-of-order."""
-        specifications_packet = {
+    async def test_count_start_packets_with_no_sync_id_as_out_of_order(self):
+        """Should count start packets with undefined synchronziationId as out-of-order."""
+        start_packet = {
             'type': 'synchronizationStarted',
             'sequenceTimestamp': 1603124267198,
             'sequenceNumber': 16,
             'accountId': 'accountId'
         }
-        assert packet_orderer.restore_order(specifications_packet) == []
+        assert packet_orderer.restore_order(start_packet) == []
         assert len(packet_orderer._packetsByAccountId['accountId']) == 1
-        assert packet_orderer._packetsByAccountId['accountId'][0]['packet'] == specifications_packet
+        assert packet_orderer._packetsByAccountId['accountId'][0]['packet'] == start_packet
```

### Comparing `metaapi_cloud_sdk-9.0.0/lib/clients/metaApi/provisioningProfile_client.py` & `metaapi_cloud_sdk-9.1.0/lib/clients/metaApi/provisioningProfile_client.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/clients/metaApi/provisioningProfile_client_test.py` & `metaapi_cloud_sdk-9.1.0/lib/clients/metaApi/provisioningProfile_client_test.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/clients/metaApi/synchronizationListener.py` & `metaapi_cloud_sdk-9.1.0/lib/clients/metaApi/synchronizationListener.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/clients/metaApi_client.py` & `metaapi_cloud_sdk-9.1.0/lib/clients/metaApi_client.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/clients/metaApi_client_test.py` & `metaapi_cloud_sdk-9.1.0/lib/clients/metaApi_client_test.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/clients/methodAccessException.py` & `metaapi_cloud_sdk-9.1.0/lib/clients/methodAccessException.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/copyFactory/copyFactory.py` & `metaapi_cloud_sdk-9.1.0/lib/copyFactory/copyFactory.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/integration_tests/doubleSynchronizationTest_test.py` & `metaapi_cloud_sdk-9.1.0/lib/integration_tests/doubleSynchronizationTest_test.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/integration_tests/files/servers.dat` & `metaapi_cloud_sdk-9.1.0/lib/integration_tests/files/servers.dat`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/metaApi/connectionRegistry.py` & `metaapi_cloud_sdk-9.1.0/lib/metaApi/connectionRegistry.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/metaApi/connectionRegistryModel.py` & `metaapi_cloud_sdk-9.1.0/lib/metaApi/connectionRegistryModel.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/metaApi/connectionRegistry_test.py` & `metaapi_cloud_sdk-9.1.0/lib/metaApi/connectionRegistry_test.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/metaApi/historyFileManager.py` & `metaapi_cloud_sdk-9.1.0/lib/metaApi/historyFileManager.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/metaApi/historyFileManager_test.py` & `metaapi_cloud_sdk-9.1.0/lib/metaApi/historyFileManager_test.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/metaApi/historyStorage.py` & `metaapi_cloud_sdk-9.1.0/lib/metaApi/historyStorage.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/metaApi/memoryHistoryStorage.py` & `metaapi_cloud_sdk-9.1.0/lib/metaApi/memoryHistoryStorage.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/metaApi/memoryHistoryStorageModel.py` & `metaapi_cloud_sdk-9.1.0/lib/metaApi/memoryHistoryStorageModel.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/metaApi/memoryHistoryStorage_test.py` & `metaapi_cloud_sdk-9.1.0/lib/metaApi/memoryHistoryStorage_test.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/metaApi/metaApi.py` & `metaapi_cloud_sdk-9.1.0/lib/metaApi/metaApi.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from ..clients.metaApi.metaApiWebsocket_client import MetaApiWebsocketClient
 from ..metaApi.provisioningProfileApi import ProvisioningProfileApi
 from ..clients.metaApi.provisioningProfile_client import ProvisioningProfileClient
 from ..metaApi.metatraderAccountApi import MetatraderAccountApi
 from ..clients.metaApi.metatraderAccount_client import MetatraderAccountClient
 from ..clients.errorHandler import ValidationException
 from ..metaApi.connectionRegistry import ConnectionRegistry
+from .metatraderDemoAccountApi import MetatraderDemoAccountApi
+from ..clients.metaApi.metatraderDemoAccount_client import MetatraderDemoAccountClient
 import re
 
 
 class MetaApi:
     """MetaApi MetaTrader API SDK"""
 
     def __init__(self, token: str, application: str = 'MetaApi', domain: str = 'agiliumtrade.agiliumtrade.ai',
@@ -29,14 +31,16 @@
         http_client = HttpClient(request_timeout)
         self._metaApiWebsocketClient = MetaApiWebsocketClient(token, application, domain, request_timeout,
                                                               connect_timeout)
         self._provisioningProfileApi = ProvisioningProfileApi(ProvisioningProfileClient(http_client, token, domain))
         self._connectionRegistry = ConnectionRegistry(self._metaApiWebsocketClient, application)
         self._metatraderAccountApi = MetatraderAccountApi(MetatraderAccountClient(http_client, token, domain),
                                                           self._metaApiWebsocketClient, self._connectionRegistry)
+        self._metatraderDemoAccountApi = MetatraderDemoAccountApi(MetatraderDemoAccountClient(http_client, token,
+                                                                                              domain))
 
     @property
     def provisioning_profile_api(self) -> ProvisioningProfileApi:
         """Returns provisioning profile API.
 
         Returns:
             Provisioning profile API.
@@ -48,10 +52,19 @@
         """Returns MetaTrader account API.
 
         Returns:
             MetaTrader account API.
         """
         return self._metatraderAccountApi
 
+    @property
+    def metatrader_demo_account_api(self) -> MetatraderDemoAccountApi:
+        """Returns MetaTrader demo account API.
+
+        Returns:
+            MetaTrader demo account API.
+        """
+        return self._metatraderDemoAccountApi
+
     def close(self):
         """Closes all clients and connections"""
         self._metaApiWebsocketClient.close()
```

### Comparing `metaapi_cloud_sdk-9.0.0/lib/metaApi/metaApiConnection.py` & `metaapi_cloud_sdk-9.1.0/lib/metaApi/metaApiConnection.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/metaApi/metaApiConnection_test.py` & `metaapi_cloud_sdk-9.1.0/lib/metaApi/metaApiConnection_test.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/metaApi/metatraderAccount.py` & `metaapi_cloud_sdk-9.1.0/lib/metaApi/metatraderAccount.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/metaApi/metatraderAccountApi.py` & `metaapi_cloud_sdk-9.1.0/lib/metaApi/metatraderAccountApi.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/metaApi/metatraderAccountApi_test.py` & `metaapi_cloud_sdk-9.1.0/lib/metaApi/metatraderAccountApi_test.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/metaApi/metatraderAccountModel.py` & `metaapi_cloud_sdk-9.1.0/lib/metaApi/metatraderAccountModel.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/metaApi/models.py` & `metaapi_cloud_sdk-9.1.0/lib/metaApi/models.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/metaApi/provisioningProfile.py` & `metaapi_cloud_sdk-9.1.0/lib/metaApi/provisioningProfile.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/metaApi/provisioningProfileApi.py` & `metaapi_cloud_sdk-9.1.0/lib/metaApi/provisioningProfileApi.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/metaApi/provisioningProfileApi_test.py` & `metaapi_cloud_sdk-9.1.0/lib/metaApi/provisioningProfileApi_test.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/metaApi/terminalState.py` & `metaapi_cloud_sdk-9.1.0/lib/metaApi/terminalState.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/lib/metaApi/terminalState_test.py` & `metaapi_cloud_sdk-9.1.0/lib/metaApi/terminalState_test.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_sdk-9.0.0/metaapi_cloud_sdk.egg-info/PKG-INFO` & `metaapi_cloud_sdk-9.1.0/metaapi_cloud_sdk.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaapi-cloud-sdk
-Version: 9.0.0
+Version: 9.1.0
 Summary: SDK for MetaApi, a professional cloud forex API which includes MetaTrader REST API and MetaTrader websocket API. Supports both MetaTrader 5 (MT5) and MetaTrader 4 (MT4). CopyFactorycopy trading API included. (https://metaapi.cloud)
 Home-page: https://github.com/agiliumtrade-ai/metaapi-python-sdk
 Author: Agilium Labs LLC
 Author-email: agiliumtrade@agiliumtrade.ai
 License: SEE LICENSE IN LICENSE
 Description: metaapi.cloud SDK for Python
         ############################
@@ -364,14 +364,40 @@
             print(await connection.cancel_order('46870472'))
         
             # if you need to, check the extra result information in stringCode and numericCode properties of the response
             result = await connection.create_market_buy_order('GBPUSD', 0.07, 0.9, 2.0, {'comment': 'comment',
                                                                                          'clientId': 'TE_GBPUSD_7hyINWqAl'})
             print('Trade successful, result code is ' + result['stringCode'])
         
+        Managing MetaTrader demo accounts via API
+        ===========================================
+        Please note that not all MT4/MT5 servers allows you to create demo accounts using the method below.
+        
+        Create a MetaTrader 4 demo account
+        ----------------------------------
+        .. code-block:: python
+        
+            demo_account = await api.metatrader_demo_account_api.create_mt4_demo_account(provisioningProfile.id, {
+                'balance': 100000,
+                'email': 'example@example.com',
+                'leverage': 100,
+                'serverName': 'Exness-Trial4'
+            })
+        
+        Create a MetaTrader 5 demo account
+        ----------------------------------
+        .. code-block:: python
+        
+            demo_account = await api.metatrader_demo_account_api.create_mt5_demo_account(provisioningProfile.id, {
+                'balance': 100000,
+                'email': 'example@example.com',
+                'leverage': 100,
+                'serverName': 'ICMarketsSC-Demo'
+            })
+        
         CopyFactory copy trading API (experimental)
         ===========================================
         
         CopyFactory is a powerful trade copying API which makes developing forex
         trade copying applications as easy as writing few lines of code.
         
         At this point this feature is experimental and we have not yet defined a final price for it.
```

### Comparing `metaapi_cloud_sdk-9.0.0/metaapi_cloud_sdk.egg-info/SOURCES.txt` & `metaapi_cloud_sdk-9.1.0/metaapi_cloud_sdk.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -45,14 +45,16 @@
 lib/clients/copyFactory/trading_client.py
 lib/clients/copyFactory/trading_client_test.py
 lib/clients/metaApi/__init__.py
 lib/clients/metaApi/metaApiWebsocket_client.py
 lib/clients/metaApi/metaApiWebsocket_client_test.py
 lib/clients/metaApi/metatraderAccount_client.py
 lib/clients/metaApi/metatraderAccount_client_test.py
+lib/clients/metaApi/metatraderDemoAccount_client.py
+lib/clients/metaApi/metatraderDemoAccount_client_test.py
 lib/clients/metaApi/notConnectedException.py
 lib/clients/metaApi/notSynchronizedException.py
 lib/clients/metaApi/packetOrderer.py
 lib/clients/metaApi/packetOrderer_test.py
 lib/clients/metaApi/provisioningProfile_client.py
 lib/clients/metaApi/provisioningProfile_client_test.py
 lib/clients/metaApi/reconnectListener.py
@@ -75,14 +77,17 @@
 lib/metaApi/metaApi.py
 lib/metaApi/metaApiConnection.py
 lib/metaApi/metaApiConnection_test.py
 lib/metaApi/metatraderAccount.py
 lib/metaApi/metatraderAccountApi.py
 lib/metaApi/metatraderAccountApi_test.py
 lib/metaApi/metatraderAccountModel.py
+lib/metaApi/metatraderDemoAccount.py
+lib/metaApi/metatraderDemoAccountApi.py
+lib/metaApi/metatraderDemoAccountApi_test.py
 lib/metaApi/models.py
 lib/metaApi/provisioningProfile.py
 lib/metaApi/provisioningProfileApi.py
 lib/metaApi/provisioningProfileApi_test.py
 lib/metaApi/terminalState.py
 lib/metaApi/terminalState_test.py
 metaapi_cloud_sdk.egg-info/PKG-INFO
```

### Comparing `metaapi_cloud_sdk-9.0.0/setup.py` & `metaapi_cloud_sdk-9.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 tests_require = [
       'pytest', 'pytest-mock', 'pytest-asyncio', 'asynctest', 'aiohttp', 'responses', 'mock'
 ]
 
 setuptools.setup(
     name="metaapi_cloud_sdk",
-    version="9.0.0",
+    version="9.1.0",
     author="Agilium Labs LLC",
     author_email="agiliumtrade@agiliumtrade.ai",
     description="SDK for MetaApi, a professional cloud forex API which includes MetaTrader REST API "
                 "and MetaTrader websocket API. Supports both MetaTrader 5 (MT5) and MetaTrader 4 (MT4). CopyFactory"
                 "copy trading API included. (https://metaapi.cloud)",
     long_description=long_description,
     long_description_content_type="text/x-rst",
```

