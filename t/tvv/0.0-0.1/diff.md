# Comparing `tmp/tvv-0.0.tar.gz` & `tmp/tvv-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tvv-0.0.tar", last modified: Mon Jun  5 13:25:35 2023, max compression
+gzip compressed data, was "tvv-0.1.tar", last modified: Tue Jun  6 10:44:21 2023, max compression
```

## Comparing `tvv-0.0.tar` & `tvv-0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 13:25:35.308127 tvv-0.0/
--rw-rw-rw-   0        0        0      100 2023-06-05 13:25:35.308127 tvv-0.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-05 13:25:35.308127 tvv-0.0/setup.cfg
--rw-rw-rw-   0        0        0      208 2023-06-05 13:10:48.000000 tvv-0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-05 13:25:35.292497 tvv-0.0/tvv/
--rw-rw-rw-   0        0        0     4241 2023-06-05 12:59:20.000000 tvv-0.0/tvv/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 13:25:35.308127 tvv-0.0/tvv.egg-info/
--rw-rw-rw-   0        0        0      100 2023-06-05 13:25:35.000000 tvv-0.0/tvv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      168 2023-06-05 13:25:35.000000 tvv-0.0/tvv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 13:25:35.000000 tvv-0.0/tvv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-05 13:25:35.000000 tvv-0.0/tvv.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        4 2023-06-05 13:25:35.000000 tvv-0.0/tvv.egg-info/top_level.txt
+drwxr-xr-x   0 gepbl4     (501) staff       (20)        0 2023-06-06 10:44:21.525945 tvv-0.1/
+-rw-r--r--   0 gepbl4     (501) staff       (20)       95 2023-06-06 10:44:21.526003 tvv-0.1/PKG-INFO
+-rw-------   0 gepbl4     (501) staff       (20)       38 2023-06-06 10:44:21.526235 tvv-0.1/setup.cfg
+-rw-------   0 gepbl4     (501) staff       (20)      208 2023-06-06 10:42:42.000000 tvv-0.1/setup.py
+drwxr-xr-x   0 gepbl4     (501) staff       (20)        0 2023-06-06 10:44:21.524991 tvv-0.1/tvv/
+-rw-------   0 gepbl4     (501) staff       (20)     8945 2023-06-06 10:42:43.000000 tvv-0.1/tvv/__init__.py
+drwxr-xr-x   0 gepbl4     (501) staff       (20)        0 2023-06-06 10:44:21.525838 tvv-0.1/tvv.egg-info/
+-rw-r--r--   0 gepbl4     (501) staff       (20)       95 2023-06-06 10:44:21.000000 tvv-0.1/tvv.egg-info/PKG-INFO
+-rw-r--r--   0 gepbl4     (501) staff       (20)      168 2023-06-06 10:44:21.000000 tvv-0.1/tvv.egg-info/SOURCES.txt
+-rw-r--r--   0 gepbl4     (501) staff       (20)        1 2023-06-06 10:44:21.000000 tvv-0.1/tvv.egg-info/dependency_links.txt
+-rw-r--r--   0 gepbl4     (501) staff       (20)        1 2023-06-06 10:44:21.000000 tvv-0.1/tvv.egg-info/not-zip-safe
+-rw-r--r--   0 gepbl4     (501) staff       (20)        4 2023-06-06 10:44:21.000000 tvv-0.1/tvv.egg-info/top_level.txt
```

