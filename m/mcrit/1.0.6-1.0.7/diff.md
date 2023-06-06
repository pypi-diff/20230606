# Comparing `tmp/mcrit-1.0.6.tar.gz` & `tmp/mcrit-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcrit-1.0.6.tar", last modified: Fri Jun  2 13:44:05 2023, max compression
+gzip compressed data, was "mcrit-1.0.7.tar", last modified: Tue Jun  6 15:22:58 2023, max compression
```

## Comparing `mcrit-1.0.6.tar` & `mcrit-1.0.7.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-02 13:44:05.467274 mcrit-1.0.6/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    35149 2022-05-13 09:44:28.000000 mcrit-1.0.6/LICENSE
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    13152 2023-06-02 13:44:05.467274 mcrit-1.0.6/PKG-INFO
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    10783 2023-06-02 13:43:04.000000 mcrit-1.0.6/README.md
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-02 13:44:05.459274 mcrit-1.0.6/mcrit/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    21415 2022-12-14 11:14:13.000000 mcrit-1.0.6/mcrit/Worker.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.6/mcrit/__init__.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1838 2023-03-21 09:06:40.000000 mcrit-1.0.6/mcrit/__main__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-02 13:44:05.459274 mcrit-1.0.6/mcrit/client/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    28489 2023-05-12 13:29:52.000000 mcrit-1.0.6/mcrit/client/McritClient.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    18792 2023-05-23 08:56:46.000000 mcrit-1.0.6/mcrit/client/McritConsole.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.6/mcrit/client/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-02 13:44:05.459274 mcrit-1.0.6/mcrit/config/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      855 2022-05-13 09:44:28.000000 mcrit-1.0.6/mcrit/config/ConfigInterface.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      960 2023-06-02 13:43:10.000000 mcrit-1.0.6/mcrit/config/McritConfig.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     2148 2023-04-10 15:53:10.000000 mcrit-1.0.6/mcrit/config/MinHashConfig.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      821 2022-05-13 09:44:28.000000 mcrit-1.0.6/mcrit/config/QueueConfig.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1974 2022-05-13 09:44:28.000000 mcrit-1.0.6/mcrit/config/ShinglerConfig.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1775 2022-07-29 10:29:16.000000 mcrit-1.0.6/mcrit/config/StorageConfig.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.6/mcrit/config/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-02 13:44:05.459274 mcrit-1.0.6/mcrit/index/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    29120 2023-04-26 15:34:26.000000 mcrit-1.0.6/mcrit/index/MinHashIndex.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3890 2022-08-08 11:41:38.000000 mcrit-1.0.6/mcrit/index/SearchCursor.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     6210 2022-08-08 11:41:38.000000 mcrit-1.0.6/mcrit/index/SearchQueryParser.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     6366 2022-08-08 11:41:38.000000 mcrit-1.0.6/mcrit/index/SearchQueryTree.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.6/mcrit/index/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-02 13:44:05.459274 mcrit-1.0.6/mcrit/libs/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.6/mcrit/libs/__init__.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    16784 2022-08-23 11:53:24.000000 mcrit-1.0.6/mcrit/libs/mongoqueue.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    14152 2022-05-13 09:44:28.000000 mcrit-1.0.6/mcrit/libs/pymmh3.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     2028 2022-05-13 09:44:28.000000 mcrit-1.0.6/mcrit/libs/utility.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-02 13:44:05.463274 mcrit-1.0.6/mcrit/matchers/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     6378 2022-08-31 07:13:17.000000 mcrit-1.0.6/mcrit/matchers/MatcherCross.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    28260 2023-04-10 15:53:10.000000 mcrit-1.0.6/mcrit/matchers/MatcherInterface.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3014 2022-11-25 14:50:57.000000 mcrit-1.0.6/mcrit/matchers/MatcherQuery.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3097 2023-04-10 15:53:10.000000 mcrit-1.0.6/mcrit/matchers/MatcherQueryFunction.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      751 2022-09-28 13:53:00.000000 mcrit-1.0.6/mcrit/matchers/MatcherSample.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     2429 2022-12-14 11:14:13.000000 mcrit-1.0.6/mcrit/matchers/MatcherVs.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-08-29 06:59:30.000000 mcrit-1.0.6/mcrit/matchers/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-02 13:44:05.463274 mcrit-1.0.6/mcrit/minhash/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3662 2022-05-13 09:44:28.000000 mcrit-1.0.6/mcrit/minhash/MinHash.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    10547 2022-11-11 10:02:06.000000 mcrit-1.0.6/mcrit/minhash/MinHasher.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3212 2022-05-13 09:44:28.000000 mcrit-1.0.6/mcrit/minhash/ShingleLoader.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.6/mcrit/minhash/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-02 13:44:05.463274 mcrit-1.0.6/mcrit/queue/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    10980 2022-08-31 07:13:17.000000 mcrit-1.0.6/mcrit/queue/LocalQueue.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1308 2022-05-13 09:44:28.000000 mcrit-1.0.6/mcrit/queue/QueueFactory.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    14987 2022-10-12 12:19:42.000000 mcrit-1.0.6/mcrit/queue/QueueRemoteCalls.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-08-29 06:36:44.000000 mcrit-1.0.6/mcrit/queue/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-02 13:44:05.463274 mcrit-1.0.6/mcrit/server/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1297 2023-03-21 14:19:34.000000 mcrit-1.0.6/mcrit/server/BlocksResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     6004 2023-03-21 14:19:34.000000 mcrit-1.0.6/mcrit/server/FamilyResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3764 2023-05-12 13:35:06.000000 mcrit-1.0.6/mcrit/server/FunctionResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     4609 2023-03-21 14:19:34.000000 mcrit-1.0.6/mcrit/server/JobResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     3551 2023-03-21 14:19:34.000000 mcrit-1.0.6/mcrit/server/MatchResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     7608 2023-03-22 15:50:20.000000 mcrit-1.0.6/mcrit/server/QueryResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    11793 2023-03-21 14:19:34.000000 mcrit-1.0.6/mcrit/server/SampleResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     5159 2023-03-21 14:19:34.000000 mcrit-1.0.6/mcrit/server/StatusResource.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.6/mcrit/server/__init__.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     5887 2023-03-17 17:07:42.000000 mcrit-1.0.6/mcrit/server/application_routes.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1868 2023-03-21 14:19:34.000000 mcrit-1.0.6/mcrit/server/utils.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)       69 2022-05-13 09:44:28.000000 mcrit-1.0.6/mcrit/server/wsgi.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-02 13:44:05.463274 mcrit-1.0.6/mcrit/storage/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     2077 2022-08-03 10:24:19.000000 mcrit-1.0.6/mcrit/storage/FamilyEntry.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     6415 2023-03-21 14:19:34.000000 mcrit-1.0.6/mcrit/storage/FunctionEntry.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1661 2023-03-21 14:19:34.000000 mcrit-1.0.6/mcrit/storage/FunctionLabelEntry.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     2764 2023-02-27 12:31:29.000000 mcrit-1.0.6/mcrit/storage/MatchedFunctionEntry.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     6617 2023-02-14 15:17:18.000000 mcrit-1.0.6/mcrit/storage/MatchedSampleEntry.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1389 2023-04-10 15:53:10.000000 mcrit-1.0.6/mcrit/storage/MatchingCache.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    25691 2023-06-02 12:31:24.000000 mcrit-1.0.6/mcrit/storage/MatchingResult.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    44811 2023-03-24 15:01:21.000000 mcrit-1.0.6/mcrit/storage/MemoryStorage.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    59597 2023-04-26 15:32:48.000000 mcrit-1.0.6/mcrit/storage/MongoDbStorage.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     4932 2023-03-17 17:07:42.000000 mcrit-1.0.6/mcrit/storage/SampleEntry.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      735 2022-11-13 10:29:45.000000 mcrit-1.0.6/mcrit/storage/StorageFactory.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    25158 2023-03-21 14:19:34.000000 mcrit-1.0.6/mcrit/storage/StorageInterface.py
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.6/mcrit/storage/__init__.py
-drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-02 13:44:05.459274 mcrit-1.0.6/mcrit.egg-info/
--rw-rw-r--   0 pnx       (1000) pnx       (1000)    13152 2023-06-02 13:44:05.000000 mcrit-1.0.6/mcrit.egg-info/PKG-INFO
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1950 2023-06-02 13:44:05.000000 mcrit-1.0.6/mcrit.egg-info/SOURCES.txt
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        1 2023-06-02 13:44:05.000000 mcrit-1.0.6/mcrit.egg-info/dependency_links.txt
--rw-rw-r--   0 pnx       (1000) pnx       (1000)      135 2023-06-02 13:44:05.000000 mcrit-1.0.6/mcrit.egg-info/requires.txt
--rw-rw-r--   0 pnx       (1000) pnx       (1000)        6 2023-06-02 13:44:05.000000 mcrit-1.0.6/mcrit.egg-info/top_level.txt
--rw-rw-r--   0 pnx       (1000) pnx       (1000)       38 2023-06-02 13:44:05.467274 mcrit-1.0.6/setup.cfg
--rw-rw-r--   0 pnx       (1000) pnx       (1000)     1355 2023-06-02 13:43:00.000000 mcrit-1.0.6/setup.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-06 15:22:58.519425 mcrit-1.0.7/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    35149 2022-05-13 09:44:28.000000 mcrit-1.0.7/LICENSE
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    13233 2023-06-06 15:22:58.519425 mcrit-1.0.7/PKG-INFO
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    10856 2023-06-06 15:21:51.000000 mcrit-1.0.7/README.md
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-06 15:22:58.255431 mcrit-1.0.7/mcrit/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    21415 2022-12-14 11:14:13.000000 mcrit-1.0.7/mcrit/Worker.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.7/mcrit/__init__.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1838 2023-03-21 09:06:40.000000 mcrit-1.0.7/mcrit/__main__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-06 15:22:58.287430 mcrit-1.0.7/mcrit/client/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    28489 2023-05-12 13:29:52.000000 mcrit-1.0.7/mcrit/client/McritClient.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    18792 2023-05-23 08:56:46.000000 mcrit-1.0.7/mcrit/client/McritConsole.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.7/mcrit/client/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-06 15:22:58.287430 mcrit-1.0.7/mcrit/config/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)      855 2022-05-13 09:44:28.000000 mcrit-1.0.7/mcrit/config/ConfigInterface.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)      960 2023-06-06 15:21:29.000000 mcrit-1.0.7/mcrit/config/McritConfig.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     2148 2023-04-10 15:53:10.000000 mcrit-1.0.7/mcrit/config/MinHashConfig.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)      821 2022-05-13 09:44:28.000000 mcrit-1.0.7/mcrit/config/QueueConfig.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1974 2022-05-13 09:44:28.000000 mcrit-1.0.7/mcrit/config/ShinglerConfig.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1775 2022-07-29 10:29:16.000000 mcrit-1.0.7/mcrit/config/StorageConfig.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.7/mcrit/config/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-06 15:22:58.307430 mcrit-1.0.7/mcrit/index/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    29120 2023-04-26 15:34:26.000000 mcrit-1.0.7/mcrit/index/MinHashIndex.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3890 2022-08-08 11:41:38.000000 mcrit-1.0.7/mcrit/index/SearchCursor.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     6210 2022-08-08 11:41:38.000000 mcrit-1.0.7/mcrit/index/SearchQueryParser.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     6366 2022-08-08 11:41:38.000000 mcrit-1.0.7/mcrit/index/SearchQueryTree.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.7/mcrit/index/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-06 15:22:58.327429 mcrit-1.0.7/mcrit/libs/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.7/mcrit/libs/__init__.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    16784 2022-08-23 11:53:24.000000 mcrit-1.0.7/mcrit/libs/mongoqueue.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    14152 2022-05-13 09:44:28.000000 mcrit-1.0.7/mcrit/libs/pymmh3.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     2028 2022-05-13 09:44:28.000000 mcrit-1.0.7/mcrit/libs/utility.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-06 15:22:58.383428 mcrit-1.0.7/mcrit/matchers/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     6378 2022-08-31 07:13:17.000000 mcrit-1.0.7/mcrit/matchers/MatcherCross.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    28260 2023-04-10 15:53:10.000000 mcrit-1.0.7/mcrit/matchers/MatcherInterface.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3014 2022-11-25 14:50:57.000000 mcrit-1.0.7/mcrit/matchers/MatcherQuery.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3097 2023-04-10 15:53:10.000000 mcrit-1.0.7/mcrit/matchers/MatcherQueryFunction.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)      751 2022-09-28 13:53:00.000000 mcrit-1.0.7/mcrit/matchers/MatcherSample.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     2429 2022-12-14 11:14:13.000000 mcrit-1.0.7/mcrit/matchers/MatcherVs.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-08-29 06:59:30.000000 mcrit-1.0.7/mcrit/matchers/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-06 15:22:58.403428 mcrit-1.0.7/mcrit/minhash/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3662 2022-05-13 09:44:28.000000 mcrit-1.0.7/mcrit/minhash/MinHash.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    10547 2022-11-11 10:02:06.000000 mcrit-1.0.7/mcrit/minhash/MinHasher.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3212 2022-05-13 09:44:28.000000 mcrit-1.0.7/mcrit/minhash/ShingleLoader.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.7/mcrit/minhash/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-06 15:22:58.403428 mcrit-1.0.7/mcrit/queue/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    10980 2022-08-31 07:13:17.000000 mcrit-1.0.7/mcrit/queue/LocalQueue.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1308 2022-05-13 09:44:28.000000 mcrit-1.0.7/mcrit/queue/QueueFactory.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    14987 2022-10-12 12:19:42.000000 mcrit-1.0.7/mcrit/queue/QueueRemoteCalls.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-08-29 06:36:44.000000 mcrit-1.0.7/mcrit/queue/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-06 15:22:58.511426 mcrit-1.0.7/mcrit/server/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1297 2023-03-21 14:19:34.000000 mcrit-1.0.7/mcrit/server/BlocksResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     6004 2023-03-21 14:19:34.000000 mcrit-1.0.7/mcrit/server/FamilyResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3764 2023-05-12 13:35:06.000000 mcrit-1.0.7/mcrit/server/FunctionResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     4609 2023-03-21 14:19:34.000000 mcrit-1.0.7/mcrit/server/JobResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     3551 2023-03-21 14:19:34.000000 mcrit-1.0.7/mcrit/server/MatchResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     7608 2023-03-22 15:50:20.000000 mcrit-1.0.7/mcrit/server/QueryResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    11793 2023-03-21 14:19:34.000000 mcrit-1.0.7/mcrit/server/SampleResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     5159 2023-03-21 14:19:34.000000 mcrit-1.0.7/mcrit/server/StatusResource.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.7/mcrit/server/__init__.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     5887 2023-03-17 17:07:42.000000 mcrit-1.0.7/mcrit/server/application_routes.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1868 2023-03-21 14:19:34.000000 mcrit-1.0.7/mcrit/server/utils.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)       69 2022-05-13 09:44:28.000000 mcrit-1.0.7/mcrit/server/wsgi.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-06 15:22:58.519425 mcrit-1.0.7/mcrit/storage/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     2077 2022-08-03 10:24:19.000000 mcrit-1.0.7/mcrit/storage/FamilyEntry.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     6415 2023-03-21 14:19:34.000000 mcrit-1.0.7/mcrit/storage/FunctionEntry.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1661 2023-03-21 14:19:34.000000 mcrit-1.0.7/mcrit/storage/FunctionLabelEntry.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     2764 2023-02-27 12:31:29.000000 mcrit-1.0.7/mcrit/storage/MatchedFunctionEntry.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     6617 2023-02-14 15:17:18.000000 mcrit-1.0.7/mcrit/storage/MatchedSampleEntry.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1389 2023-04-10 15:53:10.000000 mcrit-1.0.7/mcrit/storage/MatchingCache.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    27557 2023-06-06 15:15:08.000000 mcrit-1.0.7/mcrit/storage/MatchingResult.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    44811 2023-03-24 15:01:21.000000 mcrit-1.0.7/mcrit/storage/MemoryStorage.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    59597 2023-04-26 15:32:48.000000 mcrit-1.0.7/mcrit/storage/MongoDbStorage.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     4932 2023-03-17 17:07:42.000000 mcrit-1.0.7/mcrit/storage/SampleEntry.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)      735 2022-11-13 10:29:45.000000 mcrit-1.0.7/mcrit/storage/StorageFactory.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    25158 2023-03-21 14:19:34.000000 mcrit-1.0.7/mcrit/storage/StorageInterface.py
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        0 2022-05-13 09:44:28.000000 mcrit-1.0.7/mcrit/storage/__init__.py
+drwxrwxr-x   0 pnx       (1000) pnx       (1000)        0 2023-06-06 15:22:58.271431 mcrit-1.0.7/mcrit.egg-info/
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)    13233 2023-06-06 15:22:58.000000 mcrit-1.0.7/mcrit.egg-info/PKG-INFO
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1950 2023-06-06 15:22:58.000000 mcrit-1.0.7/mcrit.egg-info/SOURCES.txt
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        1 2023-06-06 15:22:58.000000 mcrit-1.0.7/mcrit.egg-info/dependency_links.txt
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)      135 2023-06-06 15:22:58.000000 mcrit-1.0.7/mcrit.egg-info/requires.txt
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)        6 2023-06-06 15:22:58.000000 mcrit-1.0.7/mcrit.egg-info/top_level.txt
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)       38 2023-06-06 15:22:58.519425 mcrit-1.0.7/setup.cfg
+-rw-rw-r--   0 pnx       (1000) pnx       (1000)     1355 2023-06-06 15:21:36.000000 mcrit-1.0.7/setup.py
```

### Comparing `mcrit-1.0.6/LICENSE` & `mcrit-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/PKG-INFO` & `mcrit-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcrit
-Version: 1.0.6
+Version: 1.0.7
 Summary: MCRIT is a framework created for simplified application of the MinHash algorithm to code similarity.
 Home-page: https://github.com/danielplohmann/mcrit
 Author: Daniel Plohmann, Manuel Blatt, Steffen Enders, Paul Hordiienko
 Author-email: daniel.plohmann@fkie.fraunhofer.de
 License: NU General Public License v3 (GPLv3)
 Description: # MinHash-based Code Relationship & Investigation Toolkit (MCRIT)
         [![Test](https://github.com/danielplohmann/mcrit/actions/workflows/test.yml/badge.svg)](https://github.com/danielplohmann/mcrit/actions/workflows/test.yml)
@@ -121,14 +121,15 @@
         ./plugins/ida/ida_mcrit.py
         ```
         
         in IDA.
         
         
         ## Version History
+         * 2023-06-06 v1.0.7: Extended filtering capabilities on MatchingResult.
          * 2023-06-02 v1.0.6: IDA plugin can now task matching jobs, show their results and batch import labels. Harmonization of MatchingResult.
          * 2023-05-22 v1.0.3: More robustness for path verification when using MCRIT CLI on Malpedia repo folder.
          * 2023-05-12 v1.0.1: Some progress on label import for the IDA plugin. Reflected API extension of MCRITweb in McritClient.
          * 2023-04-10 v1.0.0: Milestone release for Botconf 2023.
          * 2023-04-10 v0.25.0: IDA plugin can now do function queries for the currently viewed function.
          * 2023-03-24 v0.24.2: McritClient can forward username/apitoken, addJsonReport is now forwardable.
          * 2023-03-21 v0.24.0: FunctionEntries now can store additional FunctionLabelEntries, along submitting user/date.
```

### Comparing `mcrit-1.0.6/README.md` & `mcrit-1.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,15 @@
 ./plugins/ida/ida_mcrit.py
 ```
 
 in IDA.
 
 
 ## Version History
+ * 2023-06-06 v1.0.7: Extended filtering capabilities on MatchingResult.
  * 2023-06-02 v1.0.6: IDA plugin can now task matching jobs, show their results and batch import labels. Harmonization of MatchingResult.
  * 2023-05-22 v1.0.3: More robustness for path verification when using MCRIT CLI on Malpedia repo folder.
  * 2023-05-12 v1.0.1: Some progress on label import for the IDA plugin. Reflected API extension of MCRITweb in McritClient.
  * 2023-04-10 v1.0.0: Milestone release for Botconf 2023.
  * 2023-04-10 v0.25.0: IDA plugin can now do function queries for the currently viewed function.
  * 2023-03-24 v0.24.2: McritClient can forward username/apitoken, addJsonReport is now forwardable.
  * 2023-03-21 v0.24.0: FunctionEntries now can store additional FunctionLabelEntries, along submitting user/date.
```

### Comparing `mcrit-1.0.6/mcrit/Worker.py` & `mcrit-1.0.7/mcrit/Worker.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/__main__.py` & `mcrit-1.0.7/mcrit/__main__.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/client/McritClient.py` & `mcrit-1.0.7/mcrit/client/McritClient.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/client/McritConsole.py` & `mcrit-1.0.7/mcrit/client/McritConsole.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/config/ConfigInterface.py` & `mcrit-1.0.7/mcrit/config/ConfigInterface.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/config/McritConfig.py` & `mcrit-1.0.7/mcrit/config/McritConfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from .ShinglerConfig import ShinglerConfig
 from .StorageConfig import StorageConfig
 
 
 class McritConfig(object):
 
     # NOTE to self: always change this in setup.py as well!
-    VERSION = "1.0.6"
+    VERSION = "1.0.7"
     CONFIG_FILE_PATH = str(os.path.abspath(__file__))
     PROJECT_ROOT = str(os.path.abspath(os.sep.join([CONFIG_FILE_PATH, "..", ".."])))
 
     ### global logging-config setup
     # Only do basicConfig if no handlers have been configured
     LOG_PATH = "./"
     LOG_LEVEL = logging.INFO
```

### Comparing `mcrit-1.0.6/mcrit/config/MinHashConfig.py` & `mcrit-1.0.7/mcrit/config/MinHashConfig.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/config/QueueConfig.py` & `mcrit-1.0.7/mcrit/config/QueueConfig.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/config/ShinglerConfig.py` & `mcrit-1.0.7/mcrit/config/ShinglerConfig.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/config/StorageConfig.py` & `mcrit-1.0.7/mcrit/config/StorageConfig.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/index/MinHashIndex.py` & `mcrit-1.0.7/mcrit/index/MinHashIndex.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/index/SearchCursor.py` & `mcrit-1.0.7/mcrit/index/SearchCursor.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/index/SearchQueryParser.py` & `mcrit-1.0.7/mcrit/index/SearchQueryParser.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/index/SearchQueryTree.py` & `mcrit-1.0.7/mcrit/index/SearchQueryTree.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/libs/mongoqueue.py` & `mcrit-1.0.7/mcrit/libs/mongoqueue.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/libs/pymmh3.py` & `mcrit-1.0.7/mcrit/libs/pymmh3.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/libs/utility.py` & `mcrit-1.0.7/mcrit/libs/utility.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/matchers/MatcherCross.py` & `mcrit-1.0.7/mcrit/matchers/MatcherCross.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/matchers/MatcherInterface.py` & `mcrit-1.0.7/mcrit/matchers/MatcherInterface.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/matchers/MatcherQuery.py` & `mcrit-1.0.7/mcrit/matchers/MatcherQuery.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/matchers/MatcherQueryFunction.py` & `mcrit-1.0.7/mcrit/matchers/MatcherQueryFunction.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/matchers/MatcherSample.py` & `mcrit-1.0.7/mcrit/matchers/MatcherSample.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/matchers/MatcherVs.py` & `mcrit-1.0.7/mcrit/matchers/MatcherVs.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/minhash/MinHash.py` & `mcrit-1.0.7/mcrit/minhash/MinHash.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/minhash/MinHasher.py` & `mcrit-1.0.7/mcrit/minhash/MinHasher.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/minhash/ShingleLoader.py` & `mcrit-1.0.7/mcrit/minhash/ShingleLoader.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/queue/LocalQueue.py` & `mcrit-1.0.7/mcrit/queue/LocalQueue.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/queue/QueueFactory.py` & `mcrit-1.0.7/mcrit/queue/QueueFactory.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/queue/QueueRemoteCalls.py` & `mcrit-1.0.7/mcrit/queue/QueueRemoteCalls.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/server/BlocksResource.py` & `mcrit-1.0.7/mcrit/server/BlocksResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/server/FamilyResource.py` & `mcrit-1.0.7/mcrit/server/FamilyResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/server/FunctionResource.py` & `mcrit-1.0.7/mcrit/server/FunctionResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/server/JobResource.py` & `mcrit-1.0.7/mcrit/server/JobResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/server/MatchResource.py` & `mcrit-1.0.7/mcrit/server/MatchResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/server/QueryResource.py` & `mcrit-1.0.7/mcrit/server/QueryResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/server/SampleResource.py` & `mcrit-1.0.7/mcrit/server/SampleResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/server/StatusResource.py` & `mcrit-1.0.7/mcrit/server/StatusResource.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/server/application_routes.py` & `mcrit-1.0.7/mcrit/server/application_routes.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/server/utils.py` & `mcrit-1.0.7/mcrit/server/utils.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/storage/FamilyEntry.py` & `mcrit-1.0.7/mcrit/storage/FamilyEntry.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/storage/FunctionEntry.py` & `mcrit-1.0.7/mcrit/storage/FunctionEntry.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/storage/FunctionLabelEntry.py` & `mcrit-1.0.7/mcrit/storage/FunctionLabelEntry.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/storage/MatchedFunctionEntry.py` & `mcrit-1.0.7/mcrit/storage/MatchedFunctionEntry.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/storage/MatchedSampleEntry.py` & `mcrit-1.0.7/mcrit/storage/MatchedSampleEntry.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/storage/MatchingCache.py` & `mcrit-1.0.7/mcrit/storage/MatchingCache.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/storage/MatchingResult.py` & `mcrit-1.0.7/mcrit/storage/MatchingResult.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,40 +89,54 @@
             self.filterToFrequencyMinScore(self.filter_values["filter_frequency_min_score"])
         if self.filter_values.get("filter_frequency_nonlib_min_score", None):
             self.filterToFrequencyMinScore(self.filter_values["filter_frequency_nonlib_min_score"], nonlib=True)
         if self.filter_values.get("filter_unique_only", None):
             self.filterToUniqueMatchesOnly()
         if self.filter_values.get("filter_exclude_own_family", None):
             self.excludeOwnFamily()
+        if self.filter_values.get("filter_family_name", None):
+            self.filterByFamilyName(self.filter_values["filter_family_name"])
         # filter functions
         if self.filter_values.get("filter_exclude_library", None):
             self.excludeLibraryMatches()
         if self.filter_values.get("filter_max_num_families", None):
             self.filterToFamilyCount(self.filter_values["filter_max_num_families"])
         if self.filter_values.get("filter_max_num_samples", None):
             self.filterToSampleCount(self.filter_values["filter_max_num_samples"])
         if self.filter_values.get("filter_function_min_score", None):
             self.filterToFunctionScore(min_score=self.filter_values["filter_function_min_score"])
         if self.filter_values.get("filter_function_max_score", None):
             self.filterToFunctionScore(max_score=self.filter_values["filter_function_max_score"])
+        if self.filter_values.get("filter_function_offset", None):
+            self.filterToFunctionOffset(self.filter_values["filter_function_offset"])
         if self.filter_values.get("filter_exclude_pic", None):
             self.excludePicMatches()
+        if self.filter_values.get("filter_func_unique", None):
+            self.filterToUniqueFunctionMatchesOnly()
 
     def getFamilyNameByFamilyId(self, family_id):
         if self.family_id_to_name_map is None:
             self.family_id_to_name_map = {}
             for sample_match in self.sample_matches:
                 self.family_id_to_name_map[sample_match.family_id] = sample_match.family
         return self.family_id_to_name_map[family_id] if family_id in self.family_id_to_name_map else ""
     
     def getFamilyIdsMatchedByFunctionId(self, function_id):
         if function_id not in self.function_id_to_family_ids_matched:
             return 0
         return self.function_id_to_family_ids_matched[function_id]
 
+    def filterByFamilyName(self, filter_term):
+        """ reduce families and samples to those where family_name is part of the family_name """
+        filtered_sample_matches = []
+        for sample_match in self.filtered_sample_matches:
+            if filter_term in sample_match.family:
+                filtered_sample_matches.append(sample_match)
+        self.filtered_sample_matches = filtered_sample_matches
+
     def filterToDirectMinScore(self, min_score, nonlib=False):
         """ reduce aggregated sample matches to those with direct score of min_score or higher, but nonlib flag is not applied to library samples """
         filtered_sample_matches = []
         for sample_match in self.filtered_sample_matches:
             if nonlib:
                 if sample_match.is_library:
                     filtered_sample_matches.append(sample_match)
@@ -152,14 +166,32 @@
         filtered_sample_matches = []
         for sample_match in self.filtered_sample_matches:
             unique_info = self.getUniqueFamilyMatchInfoForSample(sample_match.sample_id)
             if unique_info["unique_score"] > 0 or sample_match.is_library:
                 filtered_sample_matches.append(sample_match)
         self.filtered_sample_matches = filtered_sample_matches
 
+    def filterToUniqueFunctionMatchesOnly(self):
+        """ reduce function matches to those with unique matches (with respect to the family) only """
+        aggregated = self.getAggregatedFunctionMatches()
+        filtered_function_matches = []
+        unique_info_by_function_id = {entry["function_id"]: entry["num_families_matched"] == 1 for entry in aggregated}
+        for function_match in self.filtered_function_matches:
+            if unique_info_by_function_id[function_match.function_id]:
+                filtered_function_matches.append(function_match)
+        self.filtered_function_matches = filtered_function_matches
+
+    def filterToFunctionOffset(self, offset):
+        """ reduce function matches to those that match a specific offset """
+        filtered_function_matches = []
+        for function_match in self.filtered_function_matches:
+            if function_match.offset == offset:
+                filtered_function_matches.append(function_match)
+        self.filtered_function_matches = filtered_function_matches
+
     def excludeOwnFamily(self):
         """ remove all sample matches with the same family_id as the reference samples"""
         filtered_sample_matches = []
         for sample_match in self.filtered_sample_matches:
             if sample_match.family_id != self.reference_sample_entry.family_id:
                 filtered_sample_matches.append(sample_match)
         self.filtered_sample_matches = filtered_sample_matches
```

### Comparing `mcrit-1.0.6/mcrit/storage/MemoryStorage.py` & `mcrit-1.0.7/mcrit/storage/MemoryStorage.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/storage/MongoDbStorage.py` & `mcrit-1.0.7/mcrit/storage/MongoDbStorage.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/storage/SampleEntry.py` & `mcrit-1.0.7/mcrit/storage/SampleEntry.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/storage/StorageFactory.py` & `mcrit-1.0.7/mcrit/storage/StorageFactory.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit/storage/StorageInterface.py` & `mcrit-1.0.7/mcrit/storage/StorageInterface.py`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/mcrit.egg-info/PKG-INFO` & `mcrit-1.0.7/mcrit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcrit
-Version: 1.0.6
+Version: 1.0.7
 Summary: MCRIT is a framework created for simplified application of the MinHash algorithm to code similarity.
 Home-page: https://github.com/danielplohmann/mcrit
 Author: Daniel Plohmann, Manuel Blatt, Steffen Enders, Paul Hordiienko
 Author-email: daniel.plohmann@fkie.fraunhofer.de
 License: NU General Public License v3 (GPLv3)
 Description: # MinHash-based Code Relationship & Investigation Toolkit (MCRIT)
         [![Test](https://github.com/danielplohmann/mcrit/actions/workflows/test.yml/badge.svg)](https://github.com/danielplohmann/mcrit/actions/workflows/test.yml)
@@ -121,14 +121,15 @@
         ./plugins/ida/ida_mcrit.py
         ```
         
         in IDA.
         
         
         ## Version History
+         * 2023-06-06 v1.0.7: Extended filtering capabilities on MatchingResult.
          * 2023-06-02 v1.0.6: IDA plugin can now task matching jobs, show their results and batch import labels. Harmonization of MatchingResult.
          * 2023-05-22 v1.0.3: More robustness for path verification when using MCRIT CLI on Malpedia repo folder.
          * 2023-05-12 v1.0.1: Some progress on label import for the IDA plugin. Reflected API extension of MCRITweb in McritClient.
          * 2023-04-10 v1.0.0: Milestone release for Botconf 2023.
          * 2023-04-10 v0.25.0: IDA plugin can now do function queries for the currently viewed function.
          * 2023-03-24 v0.24.2: McritClient can forward username/apitoken, addJsonReport is now forwardable.
          * 2023-03-21 v0.24.0: FunctionEntries now can store additional FunctionLabelEntries, along submitting user/date.
```

### Comparing `mcrit-1.0.6/mcrit.egg-info/SOURCES.txt` & `mcrit-1.0.7/mcrit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mcrit-1.0.6/setup.py` & `mcrit-1.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     "smda>=1.3.0",
     "tqdm",
     "waitress",
 ]
 
 setup(
     name='mcrit',
-    version="1.0.6",
+    version="1.0.7",
     description='MCRIT is a framework created for simplified application of the MinHash algorithm to code similarity.',
     long_description_content_type="text/markdown",
     long_description=README,
     author='Daniel Plohmann, Manuel Blatt, Steffen Enders, Paul Hordiienko',
     author_email='daniel.plohmann@fkie.fraunhofer.de',
     url='https://github.com/danielplohmann/mcrit',
     license="NU General Public License v3 (GPLv3)",
```

