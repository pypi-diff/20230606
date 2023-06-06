# Comparing `tmp/jhOMR-0.0.3.tar.gz` & `tmp/jhOMR-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jhOMR-0.0.3.tar", last modified: Tue Jun  6 09:58:37 2023, max compression
+gzip compressed data, was "jhOMR-0.0.4.tar", last modified: Tue Jun  6 10:20:04 2023, max compression
```

## Comparing `jhOMR-0.0.3.tar` & `jhOMR-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 09:58:37.283260 jhOMR-0.0.3/
--rw-rw-rw-   0        0        0      227 2023-06-06 09:58:37.283260 jhOMR-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-06 09:58:37.267635 jhOMR-0.0.3/jhOMR/
--rw-rw-rw-   0        0        0    31827 2023-06-06 09:57:56.000000 jhOMR-0.0.3/jhOMR/OMRutils.py
--rw-rw-rw-   0        0        0      132 2023-06-06 08:57:35.000000 jhOMR-0.0.3/jhOMR/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 09:58:37.283260 jhOMR-0.0.3/jhOMR.egg-info/
--rw-rw-rw-   0        0        0      227 2023-06-06 09:58:37.000000 jhOMR-0.0.3/jhOMR.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-06-06 09:58:37.000000 jhOMR-0.0.3/jhOMR.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 09:58:37.000000 jhOMR-0.0.3/jhOMR.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-06-06 09:58:37.000000 jhOMR-0.0.3/jhOMR.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-06 09:58:37.000000 jhOMR-0.0.3/jhOMR.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 09:58:37.283260 jhOMR-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      312 2023-06-06 09:58:29.000000 jhOMR-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 10:20:04.987878 jhOMR-0.0.4/
+-rw-rw-rw-   0        0        0      227 2023-06-06 10:20:04.987878 jhOMR-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-06 10:20:04.972255 jhOMR-0.0.4/jhOMR/
+-rw-rw-rw-   0        0        0    31827 2023-06-06 09:57:56.000000 jhOMR-0.0.4/jhOMR/OMRutils.py
+-rw-rw-rw-   0        0        0      188 2023-06-06 10:19:41.000000 jhOMR-0.0.4/jhOMR/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 10:20:04.987878 jhOMR-0.0.4/jhOMR.egg-info/
+-rw-rw-rw-   0        0        0      227 2023-06-06 10:20:04.000000 jhOMR-0.0.4/jhOMR.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-06-06 10:20:04.000000 jhOMR-0.0.4/jhOMR.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 10:20:04.000000 jhOMR-0.0.4/jhOMR.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-06 10:20:04.000000 jhOMR-0.0.4/jhOMR.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-06 10:20:04.000000 jhOMR-0.0.4/jhOMR.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 10:20:04.987878 jhOMR-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      323 2023-06-06 10:17:34.000000 jhOMR-0.0.4/setup.py
```

### Comparing `jhOMR-0.0.3/jhOMR/OMRutils.py` & `jhOMR-0.0.4/jhOMR/OMRutils.py`

 * *Files identical despite different names*

