# Comparing `tmp/MYPACKAGE123dpp-1.0.tar.gz` & `tmp/MYPACKAGE123dpp-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MYPACKAGE123dpp-1.0.tar", last modified: Tue Jun  6 19:57:09 2023, max compression
+gzip compressed data, was "MYPACKAGE123dpp-1.1.tar", last modified: Tue Jun  6 20:04:01 2023, max compression
```

## Comparing `MYPACKAGE123dpp-1.0.tar` & `MYPACKAGE123dpp-1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 19:57:09.094339 MYPACKAGE123dpp-1.0/
-drwxrwxrwx   0        0        0        0 2023-06-06 19:57:09.090338 MYPACKAGE123dpp-1.0/MYPACKAGE123dpp.egg-info/
--rw-rw-rw-   0        0        0      131 2023-06-06 19:57:08.000000 MYPACKAGE123dpp-1.0/MYPACKAGE123dpp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      189 2023-06-06 19:57:09.000000 MYPACKAGE123dpp-1.0/MYPACKAGE123dpp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 19:57:08.000000 MYPACKAGE123dpp-1.0/MYPACKAGE123dpp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-06 19:57:08.000000 MYPACKAGE123dpp-1.0/MYPACKAGE123dpp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      131 2023-06-06 19:57:09.093339 MYPACKAGE123dpp-1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-06 19:57:09.092338 MYPACKAGE123dpp-1.0/TranslateApi/
--rw-rw-rw-   0        0        0      875 2023-06-06 19:45:17.000000 MYPACKAGE123dpp-1.0/TranslateApi/__init__.py
--rw-rw-rw-   0        0        0       42 2023-06-06 19:57:09.094339 MYPACKAGE123dpp-1.0/setup.cfg
--rw-rw-rw-   0        0        0      227 2023-06-06 19:57:03.000000 MYPACKAGE123dpp-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 20:04:01.652594 MYPACKAGE123dpp-1.1/
+drwxrwxrwx   0        0        0        0 2023-06-06 20:04:01.648594 MYPACKAGE123dpp-1.1/MYPACKAGE123dpp.egg-info/
+-rw-rw-rw-   0        0        0      131 2023-06-06 20:04:01.000000 MYPACKAGE123dpp-1.1/MYPACKAGE123dpp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      189 2023-06-06 20:04:01.000000 MYPACKAGE123dpp-1.1/MYPACKAGE123dpp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 20:04:01.000000 MYPACKAGE123dpp-1.1/MYPACKAGE123dpp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-06 20:04:01.000000 MYPACKAGE123dpp-1.1/MYPACKAGE123dpp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      131 2023-06-06 20:04:01.651594 MYPACKAGE123dpp-1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-06 20:04:01.650596 MYPACKAGE123dpp-1.1/TranslateApi/
+-rw-rw-rw-   0        0        0      902 2023-06-06 20:03:44.000000 MYPACKAGE123dpp-1.1/TranslateApi/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-06-06 20:04:01.652594 MYPACKAGE123dpp-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      227 2023-06-06 20:03:04.000000 MYPACKAGE123dpp-1.1/setup.py
```

