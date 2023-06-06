# Comparing `tmp/telebirrweb-1.0.0.tar.gz` & `tmp/telebirrweb-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telebirrweb-1.0.0.tar", last modified: Tue Jun  6 12:21:16 2023, max compression
+gzip compressed data, was "telebirrweb-1.0.1.tar", last modified: Tue Jun  6 14:56:18 2023, max compression
```

## Comparing `telebirrweb-1.0.0.tar` & `telebirrweb-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-06 12:21:16.210255 telebirrweb-1.0.0/
--rw-r--r--   0 apple      (501) staff       (20)     1068 2023-06-06 12:02:41.000000 telebirrweb-1.0.0/LICENSE
--rw-r--r--   0 apple      (501) staff       (20)     1038 2023-06-06 12:21:16.210348 telebirrweb-1.0.0/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)       80 2023-06-06 12:02:41.000000 telebirrweb-1.0.0/README.md
--rwxr-xr-x   0 apple      (501) staff       (20)       79 2023-06-06 12:21:16.210608 telebirrweb-1.0.0/setup.cfg
--rwxr-xr-x   0 apple      (501) staff       (20)     1160 2023-06-06 12:21:11.000000 telebirrweb-1.0.0/setup.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-06 12:21:16.209196 telebirrweb-1.0.0/telebirrweb/
--rw-r--r--   0 apple      (501) staff       (20)       34 2023-06-06 12:16:20.000000 telebirrweb-1.0.0/telebirrweb/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     5504 2023-06-06 12:02:41.000000 telebirrweb-1.0.0/telebirrweb/telebirr.py
--rw-r--r--   0 apple      (501) staff       (20)      744 2023-06-06 12:02:41.000000 telebirrweb-1.0.0/telebirrweb/test.py
--rw-r--r--   0 apple      (501) staff       (20)      301 2023-06-06 12:02:41.000000 telebirrweb-1.0.0/telebirrweb/utils.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-06 12:21:16.210119 telebirrweb-1.0.0/telebirrweb.egg-info/
--rw-r--r--   0 apple      (501) staff       (20)     1038 2023-06-06 12:21:16.000000 telebirrweb-1.0.0/telebirrweb.egg-info/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)      299 2023-06-06 12:21:16.000000 telebirrweb-1.0.0/telebirrweb.egg-info/SOURCES.txt
--rw-r--r--   0 apple      (501) staff       (20)        1 2023-06-06 12:21:16.000000 telebirrweb-1.0.0/telebirrweb.egg-info/dependency_links.txt
--rw-r--r--   0 apple      (501) staff       (20)       30 2023-06-06 12:21:16.000000 telebirrweb-1.0.0/telebirrweb.egg-info/requires.txt
--rw-r--r--   0 apple      (501) staff       (20)       12 2023-06-06 12:21:16.000000 telebirrweb-1.0.0/telebirrweb.egg-info/top_level.txt
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-06 14:56:18.050857 telebirrweb-1.0.1/
+-rw-r--r--   0 apple      (501) staff       (20)     1068 2023-06-06 12:02:41.000000 telebirrweb-1.0.1/LICENSE
+-rw-r--r--   0 apple      (501) staff       (20)     1930 2023-06-06 14:56:18.050926 telebirrweb-1.0.1/PKG-INFO
+-rw-r--r--   0 apple      (501) staff       (20)      851 2023-06-06 14:50:46.000000 telebirrweb-1.0.1/README.md
+-rwxr-xr-x   0 apple      (501) staff       (20)       79 2023-06-06 14:56:18.051111 telebirrweb-1.0.1/setup.cfg
+-rwxr-xr-x   0 apple      (501) staff       (20)     1416 2023-06-06 14:56:11.000000 telebirrweb-1.0.1/setup.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-06 14:56:18.050094 telebirrweb-1.0.1/telebirrweb/
+-rw-r--r--   0 apple      (501) staff       (20)       34 2023-06-06 12:16:20.000000 telebirrweb-1.0.1/telebirrweb/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     5504 2023-06-06 12:02:41.000000 telebirrweb-1.0.1/telebirrweb/telebirr.py
+-rw-r--r--   0 apple      (501) staff       (20)      744 2023-06-06 12:02:41.000000 telebirrweb-1.0.1/telebirrweb/test.py
+-rw-r--r--   0 apple      (501) staff       (20)      301 2023-06-06 12:02:41.000000 telebirrweb-1.0.1/telebirrweb/utils.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-06 14:56:18.050714 telebirrweb-1.0.1/telebirrweb.egg-info/
+-rw-r--r--   0 apple      (501) staff       (20)     1930 2023-06-06 14:56:18.000000 telebirrweb-1.0.1/telebirrweb.egg-info/PKG-INFO
+-rw-r--r--   0 apple      (501) staff       (20)      299 2023-06-06 14:56:18.000000 telebirrweb-1.0.1/telebirrweb.egg-info/SOURCES.txt
+-rw-r--r--   0 apple      (501) staff       (20)        1 2023-06-06 14:56:18.000000 telebirrweb-1.0.1/telebirrweb.egg-info/dependency_links.txt
+-rw-r--r--   0 apple      (501) staff       (20)       30 2023-06-06 14:56:18.000000 telebirrweb-1.0.1/telebirrweb.egg-info/requires.txt
+-rw-r--r--   0 apple      (501) staff       (20)       12 2023-06-06 14:56:18.000000 telebirrweb-1.0.1/telebirrweb.egg-info/top_level.txt
```

### Comparing `telebirrweb-1.0.0/LICENSE` & `telebirrweb-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `telebirrweb-1.0.0/telebirrweb/telebirr.py` & `telebirrweb-1.0.1/telebirrweb/telebirr.py`

 * *Files identical despite different names*

### Comparing `telebirrweb-1.0.0/telebirrweb/test.py` & `telebirrweb-1.0.1/telebirrweb/test.py`

 * *Files identical despite different names*

