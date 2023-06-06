# Comparing `tmp/tvv-0.1.tar.gz` & `tmp/tvv-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tvv-0.1.tar", last modified: Tue Jun  6 10:44:21 2023, max compression
+gzip compressed data, was "tvv-0.2.tar", last modified: Tue Jun  6 12:00:13 2023, max compression
```

## Comparing `tvv-0.1.tar` & `tvv-0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 gepbl4     (501) staff       (20)        0 2023-06-06 10:44:21.525945 tvv-0.1/
--rw-r--r--   0 gepbl4     (501) staff       (20)       95 2023-06-06 10:44:21.526003 tvv-0.1/PKG-INFO
--rw-------   0 gepbl4     (501) staff       (20)       38 2023-06-06 10:44:21.526235 tvv-0.1/setup.cfg
--rw-------   0 gepbl4     (501) staff       (20)      208 2023-06-06 10:42:42.000000 tvv-0.1/setup.py
-drwxr-xr-x   0 gepbl4     (501) staff       (20)        0 2023-06-06 10:44:21.524991 tvv-0.1/tvv/
--rw-------   0 gepbl4     (501) staff       (20)     8945 2023-06-06 10:42:43.000000 tvv-0.1/tvv/__init__.py
-drwxr-xr-x   0 gepbl4     (501) staff       (20)        0 2023-06-06 10:44:21.525838 tvv-0.1/tvv.egg-info/
--rw-r--r--   0 gepbl4     (501) staff       (20)       95 2023-06-06 10:44:21.000000 tvv-0.1/tvv.egg-info/PKG-INFO
--rw-r--r--   0 gepbl4     (501) staff       (20)      168 2023-06-06 10:44:21.000000 tvv-0.1/tvv.egg-info/SOURCES.txt
--rw-r--r--   0 gepbl4     (501) staff       (20)        1 2023-06-06 10:44:21.000000 tvv-0.1/tvv.egg-info/dependency_links.txt
--rw-r--r--   0 gepbl4     (501) staff       (20)        1 2023-06-06 10:44:21.000000 tvv-0.1/tvv.egg-info/not-zip-safe
--rw-r--r--   0 gepbl4     (501) staff       (20)        4 2023-06-06 10:44:21.000000 tvv-0.1/tvv.egg-info/top_level.txt
+drwxr-xr-x   0 gepbl4     (501) staff       (20)        0 2023-06-06 12:00:13.013636 tvv-0.2/
+-rw-r--r--   0 gepbl4     (501) staff       (20)       95 2023-06-06 12:00:13.013696 tvv-0.2/PKG-INFO
+-rw-------   0 gepbl4     (501) staff       (20)       38 2023-06-06 12:00:13.013912 tvv-0.2/setup.cfg
+-rw-------   0 gepbl4     (501) staff       (20)      208 2023-06-06 11:59:25.000000 tvv-0.2/setup.py
+drwxr-xr-x   0 gepbl4     (501) staff       (20)        0 2023-06-06 12:00:13.012848 tvv-0.2/tvv/
+-rw-------   0 gepbl4     (501) staff       (20)    12308 2023-06-06 11:58:51.000000 tvv-0.2/tvv/__init__.py
+drwxr-xr-x   0 gepbl4     (501) staff       (20)        0 2023-06-06 12:00:13.013530 tvv-0.2/tvv.egg-info/
+-rw-r--r--   0 gepbl4     (501) staff       (20)       95 2023-06-06 12:00:12.000000 tvv-0.2/tvv.egg-info/PKG-INFO
+-rw-r--r--   0 gepbl4     (501) staff       (20)      168 2023-06-06 12:00:12.000000 tvv-0.2/tvv.egg-info/SOURCES.txt
+-rw-r--r--   0 gepbl4     (501) staff       (20)        1 2023-06-06 12:00:12.000000 tvv-0.2/tvv.egg-info/dependency_links.txt
+-rw-r--r--   0 gepbl4     (501) staff       (20)        1 2023-06-06 12:00:12.000000 tvv-0.2/tvv.egg-info/not-zip-safe
+-rw-r--r--   0 gepbl4     (501) staff       (20)        4 2023-06-06 12:00:12.000000 tvv-0.2/tvv.egg-info/top_level.txt
```

