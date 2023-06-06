# Comparing `tmp/mozlog-7.1.1.tar.gz` & `tmp/mozlog-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozlog-7.1.1.tar", last modified: Fri Nov 18 20:01:45 2022, max compression
+gzip compressed data, was "mozlog-8.0.0.tar", last modified: Tue Jun  6 17:43:22 2023, max compression
```

## Comparing `mozlog-7.1.1.tar` & `mozlog-8.0.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2022-11-18 20:01:45.213701 mozlog-7.1.1/
--rw-r--r--   0 ahal      (1000) ahal      (1000)      816 2022-11-18 20:01:45.213701 mozlog-7.1.1/PKG-INFO
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2022-11-18 20:01:45.203701 mozlog-7.1.1/mozlog/
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1120 2021-11-02 21:49:43.000000 mozlog-7.1.1/mozlog/__init__.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3189 2021-11-02 21:49:43.000000 mozlog-7.1.1/mozlog/capture.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    12388 2022-11-17 14:26:50.000000 mozlog-7.1.1/mozlog/commandline.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2022-11-18 20:01:45.213701 mozlog-7.1.1/mozlog/formatters/
--rw-r--r--   0 ahal      (1000) ahal      (1000)      850 2021-11-02 21:49:43.000000 mozlog-7.1.1/mozlog/formatters/__init__.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)      942 2021-11-02 21:49:43.000000 mozlog-7.1.1/mozlog/formatters/base.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     4842 2022-11-17 14:26:50.000000 mozlog-7.1.1/mozlog/formatters/errorsummary.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    14529 2022-11-17 14:26:50.000000 mozlog-7.1.1/mozlog/formatters/grouping.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2022-11-18 20:01:45.213701 mozlog-7.1.1/mozlog/formatters/html/
--rw-r--r--   0 ahal      (1000) ahal      (1000)      301 2021-11-02 21:49:43.000000 mozlog-7.1.1/mozlog/formatters/html/__init__.py
--rwxr-xr-x   0 ahal      (1000) ahal      (1000)    13863 2021-11-02 21:49:43.000000 mozlog-7.1.1/mozlog/formatters/html/html.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     4489 2021-11-02 21:49:43.000000 mozlog-7.1.1/mozlog/formatters/html/main.js
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2776 2021-11-02 21:49:43.000000 mozlog-7.1.1/mozlog/formatters/html/style.css
--rw-r--r--   0 ahal      (1000) ahal      (1000)     9529 2022-05-11 13:34:49.000000 mozlog-7.1.1/mozlog/formatters/html/xmlgen.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    22937 2022-11-17 14:26:50.000000 mozlog-7.1.1/mozlog/formatters/machformatter.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1764 2021-11-02 21:49:43.000000 mozlog-7.1.1/mozlog/formatters/process.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    15510 2022-05-11 13:34:49.000000 mozlog-7.1.1/mozlog/formatters/tbplformatter.py
--rwxr-xr-x   0 ahal      (1000) ahal      (1000)     2530 2021-11-02 21:49:43.000000 mozlog-7.1.1/mozlog/formatters/unittest.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     4062 2021-11-02 21:49:43.000000 mozlog-7.1.1/mozlog/formatters/xunit.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2022-11-18 20:01:45.213701 mozlog-7.1.1/mozlog/handlers/
--rw-r--r--   0 ahal      (1000) ahal      (1000)      635 2021-11-02 21:49:43.000000 mozlog-7.1.1/mozlog/handlers/__init__.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     4578 2022-11-03 21:30:36.000000 mozlog-7.1.1/mozlog/handlers/base.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3029 2021-11-02 21:49:43.000000 mozlog-7.1.1/mozlog/handlers/bufferhandler.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1699 2021-11-02 21:49:44.000000 mozlog-7.1.1/mozlog/handlers/messagehandler.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3455 2021-11-02 21:49:44.000000 mozlog-7.1.1/mozlog/handlers/statushandler.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     7168 2021-11-02 21:49:44.000000 mozlog-7.1.1/mozlog/handlers/summaryhandler.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     5991 2021-11-02 21:49:43.000000 mozlog-7.1.1/mozlog/handlers/valgrindhandler.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     8721 2021-11-02 21:49:44.000000 mozlog-7.1.1/mozlog/logtypes.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2466 2021-11-02 21:49:44.000000 mozlog-7.1.1/mozlog/proxy.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2022-11-18 20:01:45.213701 mozlog-7.1.1/mozlog/pytest_mozlog/
--rw-r--r--   0 ahal      (1000) ahal      (1000)        0 2021-11-02 21:49:44.000000 mozlog-7.1.1/mozlog/pytest_mozlog/__init__.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     5388 2021-11-02 21:49:44.000000 mozlog-7.1.1/mozlog/pytest_mozlog/plugin.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2878 2021-11-02 21:49:44.000000 mozlog-7.1.1/mozlog/reader.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2022-11-18 20:01:45.213701 mozlog-7.1.1/mozlog/scripts/
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1151 2021-11-02 21:49:44.000000 mozlog-7.1.1/mozlog/scripts/__init__.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1519 2021-11-02 21:49:43.000000 mozlog-7.1.1/mozlog/scripts/format.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2586 2021-11-02 21:49:43.000000 mozlog-7.1.1/mozlog/scripts/logmerge.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     4093 2021-11-02 21:49:43.000000 mozlog-7.1.1/mozlog/scripts/unstable.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1519 2021-11-02 21:49:43.000000 mozlog-7.1.1/mozlog/stdadapter.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    24436 2022-05-11 13:34:49.000000 mozlog-7.1.1/mozlog/structuredlog.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2022-11-18 20:01:45.213701 mozlog-7.1.1/mozlog/unstructured/
--rw-r--r--   0 ahal      (1000) ahal      (1000)      358 2021-11-02 21:49:43.000000 mozlog-7.1.1/mozlog/unstructured/__init__.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     6710 2021-11-02 21:49:43.000000 mozlog-7.1.1/mozlog/unstructured/logger.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1542 2021-11-02 21:49:43.000000 mozlog-7.1.1/mozlog/unstructured/loggingmixin.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1883 2021-11-02 21:49:43.000000 mozlog-7.1.1/mozlog/unstructured/loglistener.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2022-11-18 20:01:45.213701 mozlog-7.1.1/mozlog.egg-info/
--rw-r--r--   0 ahal      (1000) ahal      (1000)      816 2022-11-18 20:01:45.000000 mozlog-7.1.1/mozlog.egg-info/PKG-INFO
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1348 2022-11-18 20:01:45.000000 mozlog-7.1.1/mozlog.egg-info/SOURCES.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)        1 2022-11-18 20:01:45.000000 mozlog-7.1.1/mozlog.egg-info/dependency_links.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)       51 2022-11-18 20:01:45.000000 mozlog-7.1.1/mozlog.egg-info/entry_points.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)        1 2022-11-18 20:01:45.000000 mozlog-7.1.1/mozlog.egg-info/not-zip-safe
--rw-r--r--   0 ahal      (1000) ahal      (1000)       44 2022-11-18 20:01:45.000000 mozlog-7.1.1/mozlog.egg-info/requires.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)        7 2022-11-18 20:01:45.000000 mozlog-7.1.1/mozlog.egg-info/top_level.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)       67 2022-11-18 20:01:45.213701 mozlog-7.1.1/setup.cfg
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1595 2022-11-17 14:26:50.000000 mozlog-7.1.1/setup.py
+drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2023-06-06 17:43:22.059277 mozlog-8.0.0/
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      815 2023-06-06 17:43:22.059277 mozlog-8.0.0/PKG-INFO
+drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2023-06-06 17:43:22.055277 mozlog-8.0.0/mozlog/
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     1054 2023-02-28 20:00:23.000000 mozlog-8.0.0/mozlog/__init__.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     3149 2023-02-28 20:00:23.000000 mozlog-8.0.0/mozlog/capture.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)    12348 2023-02-28 20:00:23.000000 mozlog-8.0.0/mozlog/commandline.py
+drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2023-06-06 17:43:22.059277 mozlog-8.0.0/mozlog/formatters/
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      809 2023-02-28 20:00:23.000000 mozlog-8.0.0/mozlog/formatters/__init__.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      903 2023-02-28 20:00:23.000000 mozlog-8.0.0/mozlog/formatters/base.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     4802 2023-06-06 17:43:01.000000 mozlog-8.0.0/mozlog/formatters/errorsummary.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)    14490 2023-05-02 16:41:23.000000 mozlog-8.0.0/mozlog/formatters/grouping.py
+drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2023-06-06 17:43:22.059277 mozlog-8.0.0/mozlog/formatters/html/
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      261 2023-02-28 20:00:23.000000 mozlog-8.0.0/mozlog/formatters/html/__init__.py
+-rwxrwxr-x   0 jgraham   (1000) jgraham   (1000)    13823 2023-02-28 20:00:23.000000 mozlog-8.0.0/mozlog/formatters/html/html.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     4489 2023-06-06 17:43:01.000000 mozlog-8.0.0/mozlog/formatters/html/main.js
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     2776 2022-10-26 19:22:41.000000 mozlog-8.0.0/mozlog/formatters/html/style.css
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     9489 2023-02-28 20:00:23.000000 mozlog-8.0.0/mozlog/formatters/html/xmlgen.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)    22897 2023-04-14 13:05:53.000000 mozlog-8.0.0/mozlog/formatters/machformatter.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     1725 2023-02-28 20:00:23.000000 mozlog-8.0.0/mozlog/formatters/process.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)    15461 2023-06-06 17:43:01.000000 mozlog-8.0.0/mozlog/formatters/tbplformatter.py
+-rwxrwxr-x   0 jgraham   (1000) jgraham   (1000)     2480 2023-02-28 20:00:23.000000 mozlog-8.0.0/mozlog/formatters/unittest.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     4022 2023-02-28 20:00:23.000000 mozlog-8.0.0/mozlog/formatters/xunit.py
+drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2023-06-06 17:43:22.059277 mozlog-8.0.0/mozlog/handlers/
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      595 2023-02-28 20:00:23.000000 mozlog-8.0.0/mozlog/handlers/__init__.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     4640 2023-05-02 16:41:23.000000 mozlog-8.0.0/mozlog/handlers/base.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     2989 2023-02-28 20:00:23.000000 mozlog-8.0.0/mozlog/handlers/bufferhandler.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     1659 2023-02-28 20:00:23.000000 mozlog-8.0.0/mozlog/handlers/messagehandler.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     3401 2023-02-28 20:00:23.000000 mozlog-8.0.0/mozlog/handlers/statushandler.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     7116 2023-02-28 20:00:23.000000 mozlog-8.0.0/mozlog/handlers/summaryhandler.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     5952 2023-02-28 20:00:23.000000 mozlog-8.0.0/mozlog/handlers/valgrindhandler.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     8661 2023-02-28 20:00:23.000000 mozlog-8.0.0/mozlog/logtypes.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     2426 2023-02-28 20:00:23.000000 mozlog-8.0.0/mozlog/proxy.py
+drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2023-06-06 17:43:22.059277 mozlog-8.0.0/mozlog/pytest_mozlog/
+-rw-r--r--   0 jgraham   (1000) jgraham   (1000)        0 2018-10-20 23:26:05.000000 mozlog-8.0.0/mozlog/pytest_mozlog/__init__.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     5349 2023-05-02 16:41:23.000000 mozlog-8.0.0/mozlog/pytest_mozlog/plugin.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     2838 2023-02-28 20:00:23.000000 mozlog-8.0.0/mozlog/reader.py
+drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2023-06-06 17:43:22.059277 mozlog-8.0.0/mozlog/scripts/
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     1112 2023-02-28 20:00:23.000000 mozlog-8.0.0/mozlog/scripts/__init__.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     1479 2023-02-28 20:00:23.000000 mozlog-8.0.0/mozlog/scripts/format.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     2531 2023-02-28 20:00:23.000000 mozlog-8.0.0/mozlog/scripts/logmerge.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     4038 2023-05-02 16:41:23.000000 mozlog-8.0.0/mozlog/scripts/unstable.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     1479 2023-02-28 20:00:23.000000 mozlog-8.0.0/mozlog/stdadapter.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)    27777 2023-05-16 08:58:30.000000 mozlog-8.0.0/mozlog/structuredlog.py
+drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2023-06-06 17:43:22.059277 mozlog-8.0.0/mozlog/unstructured/
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      318 2023-02-28 20:00:23.000000 mozlog-8.0.0/mozlog/unstructured/__init__.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     6656 2023-02-28 20:00:23.000000 mozlog-8.0.0/mozlog/unstructured/logger.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     1489 2023-02-28 20:00:23.000000 mozlog-8.0.0/mozlog/unstructured/loggingmixin.py
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     1844 2023-02-28 20:00:23.000000 mozlog-8.0.0/mozlog/unstructured/loglistener.py
+drwxrwxr-x   0 jgraham   (1000) jgraham   (1000)        0 2023-06-06 17:43:22.059277 mozlog-8.0.0/mozlog.egg-info/
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)      815 2023-06-06 17:43:22.000000 mozlog-8.0.0/mozlog.egg-info/PKG-INFO
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     1348 2023-06-06 17:43:22.000000 mozlog-8.0.0/mozlog.egg-info/SOURCES.txt
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)        1 2023-06-06 17:43:22.000000 mozlog-8.0.0/mozlog.egg-info/dependency_links.txt
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)       50 2023-06-06 17:43:22.000000 mozlog-8.0.0/mozlog.egg-info/entry_points.txt
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)        1 2023-06-06 17:43:22.000000 mozlog-8.0.0/mozlog.egg-info/not-zip-safe
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)       44 2023-06-06 17:43:22.000000 mozlog-8.0.0/mozlog.egg-info/requires.txt
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)        7 2023-06-06 17:43:22.000000 mozlog-8.0.0/mozlog.egg-info/top_level.txt
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)       67 2023-06-06 17:43:22.059277 mozlog-8.0.0/setup.cfg
+-rw-rw-r--   0 jgraham   (1000) jgraham   (1000)     1555 2023-05-22 15:01:04.000000 mozlog-8.0.0/setup.py
```

### Comparing `mozlog-7.1.1/PKG-INFO` & `mozlog-8.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozlog
-Version: 7.1.1
+Version: 8.0.0
 Summary: Robust log handling specialized for logging in the Mozilla universe
 Home-page: https://wiki.mozilla.org/Auto-tools/Projects/Mozbase
 Author: Mozilla Automation and Testing Team
 Author-email: tools@lists.mozilla.org
 License: Mozilla Public License 2.0 (MPL 2.0)
 Platform: Any
 Classifier: Development Status :: 4 - Beta
@@ -13,8 +13,7 @@
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 
 see https://firefox-source-docs.mozilla.org/mozbase/index.html
-
```

### Comparing `mozlog-7.1.1/mozlog/__init__.py` & `mozlog-8.0.0/mozlog/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,23 +9,19 @@
 facilities for recording test results.
 
 The old unstructured module is deprecated. It simply wraps Python's
 logging_ module and adds a few convenience methods for logging test
 results and events.
 """
 
-from __future__ import absolute_import
-
 import sys
 
-from . import commandline
-from . import structuredlog
-from . import unstructured
-from .structuredlog import get_default_logger, set_default_logger
+from . import commandline, structuredlog, unstructured
 from .proxy import get_proxy_logger
+from .structuredlog import get_default_logger, set_default_logger
 
 # Backwards compatibility shim for consumers that use mozlog.structured
 structured = sys.modules[__name__]
 sys.modules["{}.structured".format(__name__)] = structured
 
 __all__ = [
     "commandline",
```

### Comparing `mozlog-7.1.1/mozlog/capture.py` & `mozlog-8.0.0/mozlog/capture.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
-
 import sys
 import threading
 from io import BytesIO
 
 
 class LogThread(threading.Thread):
     def __init__(self, queue, logger, level):
```

### Comparing `mozlog-7.1.1/mozlog/commandline.py` & `mozlog-8.0.0/mozlog/commandline.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
-
 import argparse
 import optparse
 import os
 import sys
 from collections import defaultdict
 
 import six
```

### Comparing `mozlog-7.1.1/mozlog/formatters/__init__.py` & `mozlog-8.0.0/mozlog/formatters/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
-
-from .unittest import UnittestFormatter
-from .xunit import XUnitFormatter
+from .errorsummary import ErrorSummaryFormatter
+from .grouping import GroupingFormatter
 from .html import HTMLFormatter
 from .machformatter import MachFormatter
 from .tbplformatter import TbplFormatter
-from .errorsummary import ErrorSummaryFormatter
-from .grouping import GroupingFormatter
-
+from .unittest import UnittestFormatter
+from .xunit import XUnitFormatter
 
 try:
     import ujson as json
 except ImportError:
     import json
```

### Comparing `mozlog-7.1.1/mozlog/formatters/base.py` & `mozlog-8.0.0/mozlog/formatters/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
+from mozlog.handlers.messagehandler import MessageHandler
 
 from ..reader import LogHandler
-from mozlog.handlers.messagehandler import MessageHandler
 
 
 class BaseFormatter(LogHandler):
     """Base class for implementing non-trivial formatters.
 
     Subclasses are expected to provide a method for each action type they
     wish to handle, each taking a single argument for the test data.
```

### Comparing `mozlog-7.1.1/mozlog/formatters/errorsummary.py` & `mozlog-8.0.0/mozlog/formatters/errorsummary.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 
-from __future__ import absolute_import
-
 import json
 from collections import defaultdict
 
 from .base import BaseFormatter
 
 
 class ErrorSummaryFormatter(BaseFormatter):
```

### Comparing `mozlog-7.1.1/mozlog/formatters/grouping.py` & `mozlog-8.0.0/mozlog/formatters/grouping.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
-from __future__ import absolute_import
-
 import collections
 import os
 import platform
 import subprocess
 import sys
 
 import six
+
 from mozlog.formatters import base
 
 DEFAULT_MOVE_UP_CODE = u"\x1b[A"
 DEFAULT_CLEAR_EOL_CODE = u"\x1b[K"
 
 
 class GroupingFormatter(base.BaseFormatter):
```

### Comparing `mozlog-7.1.1/mozlog/formatters/html/html.py` & `mozlog-8.0.0/mozlog/formatters/html/html.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 #!/usr/bin/env python
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
-
 import base64
-from datetime import datetime
-import os
 import json
-
-from .. import base
-
+import os
 from collections import defaultdict
+from datetime import datetime
+
 import six
 
+from .. import base
+
 html = None
 raw = None
 
 if six.PY2:
     from cgi import escape
 else:
     from html import escape
```

### Comparing `mozlog-7.1.1/mozlog/formatters/html/main.js` & `mozlog-8.0.0/mozlog/formatters/html/main.js`

 * *Files identical despite different names*

### Comparing `mozlog-7.1.1/mozlog/formatters/html/style.css` & `mozlog-8.0.0/mozlog/formatters/html/style.css`

 * *Files identical despite different names*

### Comparing `mozlog-7.1.1/mozlog/formatters/html/xmlgen.py` & `mozlog-8.0.0/mozlog/formatters/html/xmlgen.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,18 +18,16 @@
 SOFTWARE.
 
 This file is originally from: https://bitbucket.org/hpk42/py, specifically:
 https://bitbucket.org/hpk42/py/src/980c8d526463958ee7cae678a7e4e9b054f36b94/py/_xmlgen.py?at=default
 by holger krekel, holger at merlinux eu. 2009
 """
 
-from __future__ import absolute_import
-
-import sys
 import re
+import sys
 
 if sys.version_info >= (3, 0):
 
     def u(s):
         return s
 
     def unicode(x):
```

### Comparing `mozlog-7.1.1/mozlog/formatters/machformatter.py` & `mozlog-8.0.0/mozlog/formatters/machformatter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 
-from __future__ import absolute_import
-
 import time
 from functools import reduce
 
 import six
 from mozterm import Terminal
 
 from ..handlers import SummaryHandler
```

### Comparing `mozlog-7.1.1/mozlog/formatters/process.py` & `mozlog-8.0.0/mozlog/formatters/process.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
-
 import os
 import signal
+
 from six.moves import range
 
 # a dict cache of signal number -> signal name
 _SIG_NAME = None
 
 
 def strsig(n):
```

### Comparing `mozlog-7.1.1/mozlog/formatters/tbplformatter.py` & `mozlog-8.0.0/mozlog/formatters/tbplformatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import, division
-
 import functools
 from collections import deque
+from functools import reduce
+
+import six
 
+from ..handlers import SummaryHandler
 from .base import BaseFormatter
 from .process import strstatus
-from ..handlers import SummaryHandler
-import six
-from functools import reduce
 
 
 def output_subtests(func):
     @functools.wraps(func)
     def inner(self, data):
         if self.subtests_count:
             return self._format_subtests(data.get("component")) + func(self, data)
```

### Comparing `mozlog-7.1.1/mozlog/formatters/unittest.py` & `mozlog-8.0.0/mozlog/formatters/unittest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 #!/usr/bin/env python
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 
-from __future__ import absolute_import, division
-
 from . import base
 
 
 class UnittestFormatter(base.BaseFormatter):
     """Formatter designed to produce output in a format like that used by
     the ``unittest`` module in the standard library."""
```

### Comparing `mozlog-7.1.1/mozlog/formatters/xunit.py` & `mozlog-8.0.0/mozlog/formatters/xunit.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
-
 from xml.etree import ElementTree
 
 import six
 
 from . import base
```

### Comparing `mozlog-7.1.1/mozlog/handlers/__init__.py` & `mozlog-8.0.0/mozlog/handlers/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
-
-from .base import LogLevelFilter, StreamHandler, BaseHandler
+from .base import BaseHandler, LogLevelFilter, StreamHandler
+from .bufferhandler import BufferHandler
 from .statushandler import StatusHandler
 from .summaryhandler import SummaryHandler
-from .bufferhandler import BufferHandler
 from .valgrindhandler import ValgrindHandler
 
 __all__ = [
     "LogLevelFilter",
     "StreamHandler",
     "BaseHandler",
     "StatusHandler",
```

### Comparing `mozlog-7.1.1/mozlog/handlers/base.py` & `mozlog-8.0.0/mozlog/handlers/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
 
-from threading import Lock
 import codecs
 import locale
+from threading import Lock
 
-from mozlog.structuredlog import log_levels
 import six
+
 from mozlog.handlers.messagehandler import MessageHandler
+from mozlog.structuredlog import log_levels
 
 
 class BaseHandler(object):
     """A base handler providing message handling facilities to
     derived classes.
     """
 
@@ -73,20 +73,23 @@
         :param data: Structured log message dictionary."""
         formatted = self.formatter(data)
         if not formatted:
             return
         with self._lock:
             if six.PY3:
                 import io
+
                 import mozfile
 
                 source_enc = "utf-8"
                 target_enc = "utf-8"
                 if isinstance(self.stream, io.BytesIO):
-                    target_enc = self.stream.encoding
+                    target_enc = None
+                    if hasattr(self.stream, "encoding"):
+                        target_enc = self.stream.encoding
                 if target_enc is None:
                     target_enc = locale.getpreferredencoding()
 
                 if isinstance(self.stream, io.StringIO) and isinstance(
                     formatted, bytes
                 ):
                     formatted = formatted.decode(source_enc, "replace")
```

### Comparing `mozlog-7.1.1/mozlog/handlers/bufferhandler.py` & `mozlog-8.0.0/mozlog/handlers/bufferhandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
-
 from .base import BaseHandler
 
 
 class BufferHandler(BaseHandler):
     """Handler that maintains a circular buffer of messages based on the
     size and actions specified by a user.
```

### Comparing `mozlog-7.1.1/mozlog/handlers/messagehandler.py` & `mozlog-8.0.0/mozlog/handlers/messagehandler.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
-
 
 class MessageHandler(object):
     """A message handler providing message handling facilities to
     classes derived from BaseHandler and BaseFormatter. This is a
     composition class, to ensure handlers and formatters remain separate.
 
     :param inner: A handler-like callable that may receive messages
```

### Comparing `mozlog-7.1.1/mozlog/handlers/statushandler.py` & `mozlog-8.0.0/mozlog/handlers/statushandler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,12 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
-
-from collections import (
-    defaultdict,
-    namedtuple,
-)
-
+from collections import defaultdict, namedtuple
 
 RunSummary = namedtuple(
     "RunSummary",
     (
         "unexpected_statuses",
         "expected_statuses",
         "known_intermittent_statuses",
```

### Comparing `mozlog-7.1.1/mozlog/handlers/summaryhandler.py` & `mozlog-8.0.0/mozlog/handlers/summaryhandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
+from collections import OrderedDict, defaultdict
 
-from collections import (
-    defaultdict,
-    OrderedDict,
-)
+import six
 
 from ..reader import LogHandler
-import six
 
 
 class SummaryHandler(LogHandler):
     """Handler class for storing suite summary information.
 
     Can handle multiple suites in a single run. Summary
     information is stored on the self.summary instance variable.
```

### Comparing `mozlog-7.1.1/mozlog/handlers/valgrindhandler.py` & `mozlog-8.0.0/mozlog/handlers/valgrindhandler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
+import re
 
 from .base import BaseHandler
-import re
 
 
 class ValgrindHandler(BaseHandler):
     def __init__(self, inner):
         BaseHandler.__init__(self, inner)
         self.inner = inner
         self.vFilter = ValgrindFilter()
```

### Comparing `mozlog-7.1.1/mozlog/logtypes.py` & `mozlog-8.0.0/mozlog/logtypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
-
 import inspect
+
 import six
-from six.moves import range
-from six.moves import zip
+from six.moves import range, zip
 
 convertor_registry = {}
 missing = object()
 no_default = object()
 
 
 class log_action(object):
```

### Comparing `mozlog-7.1.1/mozlog/proxy.py` & `mozlog-8.0.0/mozlog/proxy.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
-
 from threading import Thread
 
-from .structuredlog import get_default_logger, StructuredLogger
+from .structuredlog import StructuredLogger, get_default_logger
 
 
 class ProxyLogger(object):
     """
     A ProxyLogger behaves like a
     :class:`mozlog.structuredlog.StructuredLogger`.
```

### Comparing `mozlog-7.1.1/mozlog/pytest_mozlog/plugin.py` & `mozlog-8.0.0/mozlog/pytest_mozlog/plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
-
-import mozlog
 import time
 
 import pytest
 import six
 
+import mozlog
+
 
 def pytest_addoption(parser):
     # We can't simply use mozlog.commandline.add_logging_group(parser) here because
     # Pytest's parser doesn't have the add_argument_group method Mozlog expects.
     group = parser.getgroup("mozlog")
 
     for name, (_class, _help) in six.iteritems(mozlog.commandline.log_formatters):
```

### Comparing `mozlog-7.1.1/mozlog/reader.py` & `mozlog-8.0.0/mozlog/reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
-
 import json
 
 
 def read(log_f, raise_on_error=False):
     """Return a generator that will return the entries in a structured log file.
     Note that the caller must not close the file whilst the generator is still
     in use.
```

### Comparing `mozlog-7.1.1/mozlog/scripts/__init__.py` & `mozlog-8.0.0/mozlog/scripts/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 #!/usr/bin/env python
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 
-from __future__ import absolute_import
-
 import argparse
-import unstable
+
 import format as formatlog
 import logmerge
 import six
+import unstable
 
 
 def get_parser():
     parser = argparse.ArgumentParser(
         "structlog", description="Tools for dealing with structured logs"
     )
```

### Comparing `mozlog-7.1.1/mozlog/scripts/format.py` & `mozlog-8.0.0/mozlog/scripts/format.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
-
 import argparse
 import sys
 
-from .. import handlers, commandline, reader
+from .. import commandline, handlers, reader
 
 
 def get_parser(add_help=True):
     parser = argparse.ArgumentParser(
         "format", description="Format a structured log stream", add_help=add_help
     )
     parser.add_argument(
```

### Comparing `mozlog-7.1.1/mozlog/scripts/logmerge.py` & `mozlog-8.0.0/mozlog/scripts/logmerge.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import, print_function
-
 import argparse
 import json
 import os
 import sys
-from threading import current_thread
 import time
+from threading import current_thread
+
 from mozlog.reader import read
 
 
 def dump_entry(entry, output):
     json.dump(entry, output)
     output.write("\n")
```

### Comparing `mozlog-7.1.1/mozlog/scripts/unstable.py` & `mozlog-8.0.0/mozlog/scripts/unstable.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import, print_function
-
 import argparse
-from collections import defaultdict
 import json
+from collections import defaultdict
 
-from mozlog import reader
 import six
 
+from mozlog import reader
+
 
 class StatusHandler(reader.LogHandler):
     def __init__(self):
         self.run_info = None
         self.statuses = defaultdict(
             lambda: defaultdict(lambda: defaultdict(lambda: defaultdict(int)))
         )
```

### Comparing `mozlog-7.1.1/mozlog/stdadapter.py` & `mozlog-8.0.0/mozlog/stdadapter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
-
 import logging
 
 from .structuredlog import StructuredLogger, log_levels
 
 
 class UnstructuredHandler(logging.Handler):
     def __init__(self, name=None, level=logging.NOTSET):
```

### Comparing `mozlog-7.1.1/mozlog/structuredlog.py` & `mozlog-8.0.0/mozlog/structuredlog.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,99 +1,113 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import, print_function, unicode_literals
-
-from multiprocessing import current_process
-from threading import current_thread, Lock
 import json
 import sys
 import time
 import traceback
+from multiprocessing import current_process
+from threading import Lock, current_thread
+
+import six
 
 from .logtypes import (
-    Unicode,
-    TestId,
-    TestList,
-    Status,
-    SubStatus,
-    Dict,
-    List,
-    Int,
     Any,
-    Tuple,
     Boolean,
+    Dict,
+    Int,
+    List,
     Nullable,
+    Status,
+    SubStatus,
+    TestId,
+    TestList,
+    Tuple,
+    Unicode,
+    convertor_registry,
+    log_action,
 )
-from .logtypes import log_action, convertor_registry
-import six
 
 """Structured Logging for recording test results.
 
 Allowed actions, and subfields:
   suite_start
       tests  - List of test names
       name - Name for the suite
+      run_info - Dictionary of run properties
+
+  add_subsuite
+      name - Name for the subsuite (must be unique)
+      run_info - Updates to the suite run_info (optional)
 
   suite_end
 
   test_start
       test - ID for the test
       path - Relative path to test (optional)
+      subsuite - Name of the subsuite to which test belongs (optional)
 
   test_end
       test - ID for the test
       status [PASS | FAIL | OK | ERROR | TIMEOUT | CRASH |
               ASSERT PRECONDITION_FAILED | SKIP] - test status
       expected [As for status] - Status that the test was expected to get,
                                  or absent if the test got the expected status
       extra - Dictionary of harness-specific extra information e.g. debug info
       known_intermittent - List of known intermittent statuses that should
                            not fail a test. eg. ['FAIL', 'TIMEOUT']
+      subsuite - Name of the subsuite to which test belongs (optional)
 
   test_status
       test - ID for the test
       subtest - Name of the subtest
       status [PASS | FAIL | TIMEOUT |
               PRECONDITION_FAILED | NOTRUN | SKIP] - test status
       expected [As for status] - Status that the subtest was expected to get,
                                  or absent if the subtest got the expected status
       known_intermittent - List of known intermittent statuses that should
                            not fail a test. eg. ['FAIL', 'TIMEOUT']
+      subsuite - Name of the subsuite to which test belongs (optional)
 
   process_output
       process - PID of the process
       command - Command line of the process
       data - Output data from the process
+      test - ID of the test that the process was running (optional)
+      subsuite - Name of the subsuite that the process was running (optional)
 
   assertion_count
       count - Number of assertions produced
       min_expected - Minimum expected number of assertions
       max_expected - Maximum expected number of assertions
+      subsuite - Name of the subsuite for the tests that ran (optional)
 
   lsan_leak
       frames - List of stack frames from the leak report
       scope - An identifier for the set of tests run during the browser session
               (e.g. a directory name)
       allowed_match - A stack frame in the list that matched a rule meaning the
                       leak is expected
+      subsuite - Name of the subsuite for the tests that ran (optional)
 
   lsan_summary
       bytes - Number of bytes leaked
       allocations - Number of allocations
       allowed - Boolean indicating whether all detected leaks matched allow rules
+      subsuite - Name of the subsuite for the tests that ran (optional)
 
   mozleak_object
      process - Process that leaked
      bytes - Number of bytes that leaked
      name - Name of the object that leaked
      scope - An identifier for the set of tests run during the browser session
              (e.g. a directory name)
      allowed - Boolean indicating whether the leak was permitted
+     subsuite - Name of the subsuite for the tests that ran (optional)
 
   log
       level [CRITICAL | ERROR | WARNING |
              INFO | DEBUG] - level of the logging message
       message - Message to log
 
 Subfields for all messages:
@@ -157,14 +171,15 @@
 
 class LoggerState(object):
     def __init__(self):
         self.reset()
 
     def reset(self):
         self.handlers = []
+        self.subsuites = set()
         self.running_tests = set()
         self.suite_started = False
         self.component_states = {}
         self.has_shutdown = False
 
 
 class ComponentState(object):
@@ -270,14 +285,18 @@
 
         self._handle_log(data)
 
     def _log_data(self, action, data=None):
         if data is None:
             data = {}
 
+        if data.get("subsuite") and data["subsuite"] not in self._state.subsuites:
+            self.error(f"Unrecognised subsuite {data['subsuite']}")
+            return
+
         log_data = self._make_log_data(action, data)
         self._handle_log(log_data)
 
     def _handle_log(self, data):
         if self._state.has_shutdown:
             raise LoggerShutdownError(
                 "{} action received after shutdown.".format(data["action"])
@@ -353,29 +372,56 @@
         :param dict device_info: Optional target device information provided by mozdevice.
         """
         if not self._ensure_suite_state("suite_start", data):
             return
 
         self._log_data("suite_start", data)
 
+    @log_action(
+        Unicode("name"),
+        Dict(Any, "run_info", default=None, optional=True),
+    )
+    def add_subsuite(self, data):
+        """Log a add_subsuite message
+
+        :param str name: Name to identify the subsuite.
+        :param dict run_info: Optional information about the subsuite. This updates the suite run_info.
+        """
+        if data["name"] in self._state.subsuites:
+            return
+        run_info = data.get("run_info", {"subsuite": data["name"]})
+        if "subsuite" not in run_info:
+            run_info = run_info.copy()
+            run_info["subsuite"] = data["name"]
+        data["run_info"] = run_info
+        self._state.subsuites.add(data["name"])
+        self._log_data("add_subsuite", data)
+
     @log_action(Dict(Any, "extra", default=None, optional=True))
     def suite_end(self, data):
         """Log a suite_end message"""
         if not self._ensure_suite_state("suite_end", data):
             return
 
+        self._state.subsuites.clear()
+
         self._log_data("suite_end", data)
 
-    @log_action(TestId("test"), Unicode("path", default=None, optional=True))
+    @log_action(
+        TestId("test"),
+        Unicode("path", default=None, optional=True),
+        Unicode("subsuite", default=None, optional=True),
+    )
     def test_start(self, data):
         """Log a test_start message
 
         :param test: Identifier of the test that will run.
         :param path: Path to test relative to some base (typically the root of
                      the source tree).
+        :param subsuite: Optional name of the subsuite to which the test belongs.
         """
         if not self._state.suite_started:
             self.error(
                 "Got test_start message before suite_start for test %s" % data["test"]
             )
             return
         if data["test"] in self._state.running_tests:
@@ -389,27 +435,30 @@
         Unicode("subtest"),
         SubStatus("status"),
         SubStatus("expected", default="PASS"),
         Unicode("message", default=None, optional=True),
         Unicode("stack", default=None, optional=True),
         Dict(Any, "extra", default=None, optional=True),
         List(SubStatus, "known_intermittent", default=None, optional=True),
+        Unicode("subsuite", default=None, optional=True),
     )
     def test_status(self, data):
         """
         Log a test_status message indicating a subtest result. Tests that
         do not have subtests are not expected to produce test_status messages.
 
         :param test: Identifier of the test that produced the result.
         :param subtest: Name of the subtest.
         :param status: Status string indicating the subtest result
         :param expected: Status string indicating the expected subtest result.
-        :param message: String containing a message associated with the result.
-        :param stack: a stack trace encountered during test execution.
-        :param extra: suite-specific data associated with the test result.
+        :param message: Optional string containing a message associated with the result.
+        :param stack: Optional stack trace encountered during test execution.
+        :param extra: Optional suite-specific data associated with the test result.
+        :param known_intermittent: Optional list of string expected intermittent statuses
+        :param subsuite: Optional name of the subsuite to which the test belongs.
         """
 
         if data["expected"] == data["status"] or data["status"] == "SKIP":
             del data["expected"]
 
         if data["test"] not in self._state.running_tests:
             self.error(
@@ -424,28 +473,30 @@
         TestId("test"),
         Status("status"),
         Status("expected", default="OK"),
         Unicode("message", default=None, optional=True),
         Unicode("stack", default=None, optional=True),
         Dict(Any, "extra", default=None, optional=True),
         List(Status, "known_intermittent", default=None, optional=True),
+        Unicode("subsuite", default=None, optional=True),
     )
     def test_end(self, data):
         """
         Log a test_end message indicating that a test completed. For tests
         with subtests this indicates whether the overall test completed without
         errors. For tests without subtests this indicates the test result
         directly.
 
         :param test: Identifier of the test that produced the result.
         :param status: Status string indicating the test result
         :param expected: Status string indicating the expected test result.
-        :param message: String containing a message associated with the result.
-        :param stack: a stack trace encountered during test execution.
-        :param extra: suite-specific data associated with the test result.
+        :param message: Optonal string containing a message associated with the result.
+        :param stack: Optional stack trace encountered during test execution.
+        :param extra: Optional suite-specific data associated with the test result.
+        :param subsuite: Optional name of the subsuite to which the test belongs.
         """
 
         if data["expected"] == data["status"] or data["status"] == "SKIP":
             del data["expected"]
 
         if data["test"] not in self._state.running_tests:
             self.error(
@@ -456,23 +507,27 @@
             self._state.running_tests.remove(data["test"])
             self._log_data("test_end", data)
 
     @log_action(
         Unicode("process"),
         Unicode("data"),
         Unicode("command", default=None, optional=True),
+        TestId("test", default=None, optional=True),
+        Unicode("subsuite", default=None, optional=True),
     )
     def process_output(self, data):
         """Log output from a managed process.
 
         :param process: A unique identifier for the process producing the output
                         (typically the pid)
         :param data: The output to log
-        :param command: A string representing the full command line used to start
+        :param command: Optional string representing the full command line used to start
                         the process.
+        :param test: Optional ID of the test which the process was running.
+        :param subsuite: Optional name of the subsuite which the process was running.
         """
         self._log_data("process_output", data)
 
     @log_action(
         Unicode("process", default=None),
         Unicode("signature", default="[Unknown]"),
         TestId("test", default=None, optional=True),
@@ -480,98 +535,117 @@
         Unicode("minidump_extra", default=None, optional=True),
         Int("stackwalk_retcode", default=None, optional=True),
         Unicode("stackwalk_stdout", default=None, optional=True),
         Unicode("stackwalk_stderr", default=None, optional=True),
         Unicode("reason", default=None, optional=True),
         Unicode("java_stack", default=None, optional=True),
         List(Unicode, "stackwalk_errors", default=None),
+        Unicode("subsuite", default=None, optional=True),
     )
     def crash(self, data):
         if data["stackwalk_errors"] is None:
             data["stackwalk_errors"] = []
 
         self._log_data("crash", data)
 
     @log_action(
         Unicode("primary", default=None), List(Unicode, "secondary", default=None)
     )
     def valgrind_error(self, data):
         self._log_data("valgrind_error", data)
 
-    @log_action(Unicode("process"), Unicode("command", default=None, optional=True))
+    @log_action(
+        Unicode("process"),
+        Unicode("command", default=None, optional=True),
+        Unicode("subsuite", default=None, optional=True),
+    )
     def process_start(self, data):
         """Log start event of a process.
 
         :param process: A unique identifier for the process producing the
                         output (typically the pid)
-        :param command: A string representing the full command line used to
+        :param command: Optional string representing the full command line used to
                         start the process.
+        :param subsuite: Optional name of the subsuite using the process.
         """
         self._log_data("process_start", data)
 
     @log_action(
         Unicode("process"),
         Int("exitcode"),
         Unicode("command", default=None, optional=True),
+        Unicode("subsuite", default=None, optional=True),
     )
     def process_exit(self, data):
         """Log exit event of a process.
 
         :param process: A unique identifier for the process producing the
                         output (typically the pid)
         :param exitcode: the exit code
-        :param command: A string representing the full command line used to
+        :param command: Optional string representing the full command line used to
                         start the process.
+        :param subsuite: Optional name of the subsuite using the process.
         """
         self._log_data("process_exit", data)
 
-    @log_action(TestId("test"), Int("count"), Int("min_expected"), Int("max_expected"))
+    @log_action(
+        TestId("test"),
+        Int("count"),
+        Int("min_expected"),
+        Int("max_expected"),
+        Unicode("subsuite", default=None, optional=True),
+    )
     def assertion_count(self, data):
         """Log count of assertions produced when running a test.
 
-        :param count: - Number of assertions produced
-        :param min_expected: - Minimum expected number of assertions
-        :param max_expected: - Maximum expected number of assertions
+        :param count: Number of assertions produced
+        :param min_expected: Minimum expected number of assertions
+        :param max_expected: Maximum expected number of assertions
+        :param subsuite: Optional name of the subsuite for the tests that ran
         """
         self._log_data("assertion_count", data)
 
     @log_action(
         List(Unicode, "frames"),
         Unicode("scope", optional=True, default=None),
         Unicode("allowed_match", optional=True, default=None),
+        Unicode("subsuite", default=None, optional=True),
     )
     def lsan_leak(self, data):
         self._log_data("lsan_leak", data)
 
     @log_action(
         Int("bytes"),
         Int("allocations"),
         Boolean("allowed", optional=True, default=False),
+        Unicode("subsuite", default=None, optional=True),
     )
     def lsan_summary(self, data):
         self._log_data("lsan_summary", data)
 
     @log_action(
         Unicode("process"),
         Int("bytes"),
         Unicode("name"),
         Unicode("scope", optional=True, default=None),
         Boolean("allowed", optional=True, default=False),
+        Unicode("subsuite", default=None, optional=True),
     )
     def mozleak_object(self, data):
         self._log_data("mozleak_object", data)
 
     @log_action(
         Unicode("process"),
         Nullable(Int, "bytes"),
         Int("threshold"),
         List(Unicode, "objects"),
         Unicode("scope", optional=True, default=None),
         Boolean("induced_crash", optional=True, default=False),
         Boolean("ignore_missing", optional=True, default=False),
+        Unicode("subsuite", default=None, optional=True),
     )
     def mozleak_total(self, data):
         self._log_data("mozleak_total", data)
 
     @log_action()
     def shutdown(self, data):
         """Shutdown the logger.
```

### Comparing `mozlog-7.1.1/mozlog/unstructured/logger.py` & `mozlog-8.0.0/mozlog/unstructured/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,21 @@
 # flake8: noqa
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
-
-from logging import getLogger as getSysLogger
-from logging import *
+import json
 
 # Some of the build slave environments don't see the following when doing
 # 'from logging import *'
 # see https://bugzilla.mozilla.org/show_bug.cgi?id=700415#c35
-from logging import (
-    getLoggerClass,
-    addLevelName,
-    setLoggerClass,
-    shutdown,
-    debug,
-    info,
-    basicConfig,
-)
-import json
+from logging import *
+from logging import addLevelName, basicConfig, debug
+from logging import getLogger as getSysLogger
+from logging import getLoggerClass, info, setLoggerClass, shutdown
 
 _default_level = INFO
 _LoggerClass = getLoggerClass()
 
 # Define mozlog specific log levels
 START = _default_level + 1
 END = _default_level + 2
```

### Comparing `mozlog-7.1.1/mozlog/unstructured/loggingmixin.py` & `mozlog-8.0.0/mozlog/unstructured/loggingmixin.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
-
-from .logger import (
-    Logger,
-    getLogger,
-)
+from .logger import Logger, getLogger
 
 
 class LoggingMixin(object):
     """Expose a subset of logging functions to an inheriting class."""
 
     def set_logger(self, logger_instance=None, name=None):
         """Method for setting the underlying logger instance to be used."""
```

### Comparing `mozlog-7.1.1/mozlog/unstructured/loglistener.py` & `mozlog-8.0.0/mozlog/unstructured/loglistener.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
-
-from six.moves import socketserver
 import json
 import socket
 
+from six.moves import socketserver
+
 
 class LogMessageServer(socketserver.TCPServer):
     def __init__(self, server_address, logger, message_callback=None, timeout=3):
         socketserver.TCPServer.__init__(self, server_address, LogMessageHandler)
         self._logger = logger
         self._message_callback = message_callback
         self.timeout = timeout
```

### Comparing `mozlog-7.1.1/mozlog.egg-info/PKG-INFO` & `mozlog-8.0.0/mozlog.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozlog
-Version: 7.1.1
+Version: 8.0.0
 Summary: Robust log handling specialized for logging in the Mozilla universe
 Home-page: https://wiki.mozilla.org/Auto-tools/Projects/Mozbase
 Author: Mozilla Automation and Testing Team
 Author-email: tools@lists.mozilla.org
 License: Mozilla Public License 2.0 (MPL 2.0)
 Platform: Any
 Classifier: Development Status :: 4 - Beta
@@ -13,8 +13,7 @@
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 
 see https://firefox-source-docs.mozilla.org/mozbase/index.html
-
```

### Comparing `mozlog-7.1.1/mozlog.egg-info/SOURCES.txt` & `mozlog-8.0.0/mozlog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mozlog-7.1.1/setup.py` & `mozlog-8.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this file,
 # You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from __future__ import absolute_import
-
 from setuptools import find_packages, setup
 
 PACKAGE_NAME = "mozlog"
-PACKAGE_VERSION = "7.1.1"
+PACKAGE_VERSION = "8.0.0"
 DEPS = [
     "blessed>=1.19.1",
     "mozterm",
     "mozfile",
     "six >= 1.13.0",
 ]
```

