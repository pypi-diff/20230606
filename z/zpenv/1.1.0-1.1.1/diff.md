# Comparing `tmp/zpenv-1.1.0.tar.gz` & `tmp/zpenv-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zpenv-1.1.0.tar", last modified: Tue Jun  6 20:49:15 2023, max compression
+gzip compressed data, was "zpenv-1.1.1.tar", last modified: Tue Jun  6 20:51:54 2023, max compression
```

## Comparing `zpenv-1.1.0.tar` & `zpenv-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 20:49:15.536000 zpenv-1.1.0/
--rw-rw-rw-   0        0        0      300 2023-06-06 20:49:15.531000 zpenv-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      111 2023-06-06 20:44:32.000000 zpenv-1.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-06 20:49:15.535000 zpenv-1.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-06 20:49:15.482000 zpenv-1.1.0/zpenv/
--rw-rw-rw-   0        0        0       20 2023-06-06 20:41:18.000000 zpenv-1.1.0/zpenv/__init__.py
--rw-rw-rw-   0        0        0       61 2023-06-06 18:50:58.000000 zpenv-1.1.0/zpenv/__main__.py
--rw-rw-rw-   0        0        0    31382 2023-06-06 20:40:58.000000 zpenv-1.1.0/zpenv/zpenv.py
-drwxrwxrwx   0        0        0        0 2023-06-06 20:49:15.525000 zpenv-1.1.0/zpenv.egg-info/
--rw-rw-rw-   0        0        0      300 2023-06-06 20:49:14.000000 zpenv-1.1.0/zpenv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-06-06 20:49:15.000000 zpenv-1.1.0/zpenv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 20:49:15.000000 zpenv-1.1.0/zpenv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-06-06 20:49:15.000000 zpenv-1.1.0/zpenv.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       27 2023-06-06 20:49:15.000000 zpenv-1.1.0/zpenv.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-06 20:49:15.000000 zpenv-1.1.0/zpenv.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-06 20:51:54.384000 zpenv-1.1.1/
+-rw-rw-rw-   0        0        0     5138 2023-06-06 20:51:54.380000 zpenv-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4917 2022-12-26 19:01:11.000000 zpenv-1.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-06 20:51:54.383000 zpenv-1.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-06 20:51:54.331000 zpenv-1.1.1/zpenv/
+-rw-rw-rw-   0        0        0       20 2023-06-06 20:41:18.000000 zpenv-1.1.1/zpenv/__init__.py
+-rw-rw-rw-   0        0        0       61 2023-06-06 18:50:58.000000 zpenv-1.1.1/zpenv/__main__.py
+-rw-rw-rw-   0        0        0    31382 2023-06-06 20:40:58.000000 zpenv-1.1.1/zpenv/zpenv.py
+drwxrwxrwx   0        0        0        0 2023-06-06 20:51:54.374000 zpenv-1.1.1/zpenv.egg-info/
+-rw-rw-rw-   0        0        0     5138 2023-06-06 20:51:53.000000 zpenv-1.1.1/zpenv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2023-06-06 20:51:54.000000 zpenv-1.1.1/zpenv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 20:51:53.000000 zpenv-1.1.1/zpenv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-06 20:51:53.000000 zpenv-1.1.1/zpenv.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       27 2023-06-06 20:51:54.000000 zpenv-1.1.1/zpenv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-06 20:51:54.000000 zpenv-1.1.1/zpenv.egg-info/top_level.txt
```

### Comparing `zpenv-1.1.0/zpenv/zpenv.py` & `zpenv-1.1.1/zpenv/zpenv.py`

 * *Files identical despite different names*

