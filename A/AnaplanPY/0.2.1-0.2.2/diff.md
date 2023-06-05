# Comparing `tmp/AnaplanPY-0.2.1.tar.gz` & `tmp/AnaplanPY-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AnaplanPY-0.2.1.tar", last modified: Mon Jun  5 22:57:11 2023, max compression
+gzip compressed data, was "AnaplanPY-0.2.2.tar", last modified: Mon Jun  5 23:19:03 2023, max compression
```

## Comparing `AnaplanPY-0.2.1.tar` & `AnaplanPY-0.2.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 22:57:11.901401 AnaplanPY-0.2.1/
--rw-rw-rw-   0        0        0      258 2023-06-05 22:57:11.901401 AnaplanPY-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-05 22:29:45.000000 AnaplanPY-0.2.1/README.rst
--rw-rw-rw-   0        0        0      115 2023-06-05 22:57:11.903170 AnaplanPY-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      418 2023-06-05 22:56:19.000000 AnaplanPY-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-05 22:57:11.873124 AnaplanPY-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-05 22:57:11.899398 AnaplanPY-0.2.1/src/AnaplanPY.egg-info/
--rw-rw-rw-   0        0        0      258 2023-06-05 22:57:11.000000 AnaplanPY-0.2.1/src/AnaplanPY.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2023-06-05 22:57:11.000000 AnaplanPY-0.2.1/src/AnaplanPY.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 22:57:11.000000 AnaplanPY-0.2.1/src/AnaplanPY.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-05 22:57:11.000000 AnaplanPY-0.2.1/src/AnaplanPY.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 22:57:11.000000 AnaplanPY-0.2.1/src/AnaplanPY.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-05 23:19:03.239792 AnaplanPY-0.2.2/
+-rw-rw-rw-   0        0        0      258 2023-06-05 23:19:03.240754 AnaplanPY-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-05 22:29:45.000000 AnaplanPY-0.2.2/README.rst
+-rw-rw-rw-   0        0        0      115 2023-06-05 23:19:03.243733 AnaplanPY-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      418 2023-06-05 23:18:33.000000 AnaplanPY-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-05 23:19:03.199709 AnaplanPY-0.2.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-05 23:19:03.236754 AnaplanPY-0.2.2/src/AnaplanPY.egg-info/
+-rw-rw-rw-   0        0        0      258 2023-06-05 23:19:03.000000 AnaplanPY-0.2.2/src/AnaplanPY.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2023-06-05 23:19:03.000000 AnaplanPY-0.2.2/src/AnaplanPY.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 23:19:03.000000 AnaplanPY-0.2.2/src/AnaplanPY.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-05 23:19:03.000000 AnaplanPY-0.2.2/src/AnaplanPY.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-05 23:19:03.000000 AnaplanPY-0.2.2/src/AnaplanPY.egg-info/top_level.txt
```

