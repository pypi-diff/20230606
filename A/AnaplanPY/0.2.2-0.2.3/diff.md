# Comparing `tmp/AnaplanPY-0.2.2.tar.gz` & `tmp/AnaplanPY-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AnaplanPY-0.2.2.tar", last modified: Mon Jun  5 23:19:03 2023, max compression
+gzip compressed data, was "AnaplanPY-0.2.3.tar", last modified: Tue Jun  6 05:15:10 2023, max compression
```

## Comparing `AnaplanPY-0.2.2.tar` & `AnaplanPY-0.2.3.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 23:19:03.239792 AnaplanPY-0.2.2/
--rw-rw-rw-   0        0        0      258 2023-06-05 23:19:03.240754 AnaplanPY-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-05 22:29:45.000000 AnaplanPY-0.2.2/README.rst
--rw-rw-rw-   0        0        0      115 2023-06-05 23:19:03.243733 AnaplanPY-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      418 2023-06-05 23:18:33.000000 AnaplanPY-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-05 23:19:03.199709 AnaplanPY-0.2.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-05 23:19:03.236754 AnaplanPY-0.2.2/src/AnaplanPY.egg-info/
--rw-rw-rw-   0        0        0      258 2023-06-05 23:19:03.000000 AnaplanPY-0.2.2/src/AnaplanPY.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2023-06-05 23:19:03.000000 AnaplanPY-0.2.2/src/AnaplanPY.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 23:19:03.000000 AnaplanPY-0.2.2/src/AnaplanPY.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-05 23:19:03.000000 AnaplanPY-0.2.2/src/AnaplanPY.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 23:19:03.000000 AnaplanPY-0.2.2/src/AnaplanPY.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 05:15:10.609898 AnaplanPY-0.2.3/
+drwxrwxrwx   0        0        0        0 2023-06-06 05:15:10.604142 AnaplanPY-0.2.3/AnaplanPY/
+-rw-rw-rw-   0        0        0    13468 2023-06-05 22:36:53.000000 AnaplanPY-0.2.3/AnaplanPY/AnaplanPY.py
+-rw-rw-rw-   0        0        0       16 2023-06-05 23:17:31.000000 AnaplanPY-0.2.3/AnaplanPY/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 05:15:10.609898 AnaplanPY-0.2.3/AnaplanPY.egg-info/
+-rw-rw-rw-   0        0        0      290 2023-06-06 05:15:10.000000 AnaplanPY-0.2.3/AnaplanPY.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-06-06 05:15:10.000000 AnaplanPY-0.2.3/AnaplanPY.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 05:15:10.000000 AnaplanPY-0.2.3/AnaplanPY.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-06 05:15:10.000000 AnaplanPY-0.2.3/AnaplanPY.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-06 05:15:10.000000 AnaplanPY-0.2.3/AnaplanPY.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      290 2023-06-06 05:15:10.610893 AnaplanPY-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-05 22:29:45.000000 AnaplanPY-0.2.3/README.rst
+-rw-rw-rw-   0        0        0      115 2023-06-06 05:15:10.612009 AnaplanPY-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      464 2023-06-06 05:12:47.000000 AnaplanPY-0.2.3/setup.py
```

