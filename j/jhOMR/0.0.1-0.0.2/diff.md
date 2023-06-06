# Comparing `tmp/jhOMR-0.0.1.tar.gz` & `tmp/jhOMR-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jhOMR-0.0.1.tar", last modified: Tue Jun  6 09:05:03 2023, max compression
+gzip compressed data, was "jhOMR-0.0.2.tar", last modified: Tue Jun  6 09:22:46 2023, max compression
```

## Comparing `jhOMR-0.0.1.tar` & `jhOMR-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 09:05:03.457972 jhOMR-0.0.1/
--rw-rw-rw-   0        0        0      227 2023-06-06 09:05:03.457972 jhOMR-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-06 09:05:03.426777 jhOMR-0.0.1/jhOMR/
--rw-rw-rw-   0        0        0    31841 2023-06-05 08:30:12.000000 jhOMR-0.0.1/jhOMR/OMRutils.py
--rw-rw-rw-   0        0        0      132 2023-06-06 08:57:35.000000 jhOMR-0.0.1/jhOMR/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 09:05:03.457972 jhOMR-0.0.1/jhOMR.egg-info/
--rw-rw-rw-   0        0        0      227 2023-06-06 09:05:03.000000 jhOMR-0.0.1/jhOMR.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-06-06 09:05:03.000000 jhOMR-0.0.1/jhOMR.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 09:05:03.000000 jhOMR-0.0.1/jhOMR.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-06 09:05:03.000000 jhOMR-0.0.1/jhOMR.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-06 09:05:03.000000 jhOMR-0.0.1/jhOMR.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 09:05:03.457972 jhOMR-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      302 2023-06-06 09:04:48.000000 jhOMR-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 09:22:46.061003 jhOMR-0.0.2/
+-rw-rw-rw-   0        0        0      227 2023-06-06 09:22:46.060007 jhOMR-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-06 09:22:46.035855 jhOMR-0.0.2/jhOMR/
+-rw-rw-rw-   0        0        0    31841 2023-06-05 08:30:12.000000 jhOMR-0.0.2/jhOMR/OMRutils.py
+-rw-rw-rw-   0        0        0      132 2023-06-06 08:57:35.000000 jhOMR-0.0.2/jhOMR/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 09:22:46.057962 jhOMR-0.0.2/jhOMR.egg-info/
+-rw-rw-rw-   0        0        0      227 2023-06-06 09:22:45.000000 jhOMR-0.0.2/jhOMR.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-06-06 09:22:45.000000 jhOMR-0.0.2/jhOMR.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 09:22:45.000000 jhOMR-0.0.2/jhOMR.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-06 09:22:45.000000 jhOMR-0.0.2/jhOMR.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-06 09:22:45.000000 jhOMR-0.0.2/jhOMR.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 09:22:46.062001 jhOMR-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      312 2023-06-06 09:21:30.000000 jhOMR-0.0.2/setup.py
```

### Comparing `jhOMR-0.0.1/jhOMR/OMRutils.py` & `jhOMR-0.0.2/jhOMR/OMRutils.py`

 * *Files identical despite different names*

