# Comparing `tmp/denpy-1.0.1.tar.gz` & `tmp/denpy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denpy-1.0.1.tar", last modified: Thu Jun  1 14:12:06 2023, max compression
+gzip compressed data, was "denpy-1.0.2.tar", last modified: Tue Jun  6 19:59:32 2023, max compression
```

## Comparing `denpy-1.0.1.tar` & `denpy-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 14:12:06.345129 denpy-1.0.1/
--rw-rw-rw-   0        0        0      127 2023-06-01 14:12:06.345129 denpy-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-01 14:12:06.341139 denpy-1.0.1/denpy/
--rw-rw-rw-   0        0        0      137 2023-05-31 18:58:29.000000 denpy-1.0.1/denpy/__init__.py
--rw-rw-rw-   0        0        0      437 2023-05-30 12:22:14.000000 denpy-1.0.1/denpy/color.py
--rw-rw-rw-   0        0        0     1613 2023-05-29 08:55:28.000000 denpy-1.0.1/denpy/database.py
--rw-rw-rw-   0        0        0      422 2023-06-01 14:11:30.000000 denpy-1.0.1/denpy/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-01 14:12:06.344784 denpy-1.0.1/denpy.egg-info/
--rw-rw-rw-   0        0        0      127 2023-06-01 14:12:06.000000 denpy-1.0.1/denpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2023-06-01 14:12:06.000000 denpy-1.0.1/denpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 14:12:06.000000 denpy-1.0.1/denpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-01 14:12:06.000000 denpy-1.0.1/denpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 14:12:06.346126 denpy-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      220 2023-06-01 14:11:59.000000 denpy-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 19:59:32.029268 denpy-1.0.2/
+-rw-rw-rw-   0        0        0      127 2023-06-06 19:59:32.028271 denpy-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-06 19:59:32.024282 denpy-1.0.2/denpy/
+-rw-rw-rw-   0        0        0      137 2023-05-31 18:58:29.000000 denpy-1.0.2/denpy/__init__.py
+-rw-rw-rw-   0        0        0      401 2023-06-01 15:01:37.000000 denpy-1.0.2/denpy/color.py
+-rw-rw-rw-   0        0        0     1613 2023-05-29 08:55:28.000000 denpy-1.0.2/denpy/database.py
+-rw-rw-rw-   0        0        0      882 2023-06-06 19:57:37.000000 denpy-1.0.2/denpy/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-06 19:59:32.027274 denpy-1.0.2/denpy.egg-info/
+-rw-rw-rw-   0        0        0      127 2023-06-06 19:59:31.000000 denpy-1.0.2/denpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2023-06-06 19:59:31.000000 denpy-1.0.2/denpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 19:59:31.000000 denpy-1.0.2/denpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-06 19:59:31.000000 denpy-1.0.2/denpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 19:59:32.029268 denpy-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      220 2023-06-06 19:59:27.000000 denpy-1.0.2/setup.py
```

### Comparing `denpy-1.0.1/denpy/database.py` & `denpy-1.0.2/denpy/database.py`

 * *Files identical despite different names*

