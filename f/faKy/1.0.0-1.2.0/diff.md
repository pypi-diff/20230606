# Comparing `tmp/faKy-1.0.0.tar.gz` & `tmp/faKy-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faKy-1.0.0.tar", last modified: Tue Jun  6 08:35:58 2023, max compression
+gzip compressed data, was "faKy-1.2.0.tar", last modified: Tue Jun  6 10:53:53 2023, max compression
```

## Comparing `faKy-1.0.0.tar` & `faKy-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 08:35:58.841002 faKy-1.0.0/
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      197 2023-06-06 08:35:58.840650 faKy-1.0.0/PKG-INFO
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        6 2023-06-06 08:12:19.000000 faKy-1.0.0/README.md
-drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 08:35:58.837071 faKy-1.0.0/faKy/
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        1 2023-06-06 08:19:35.000000 faKy-1.0.0/faKy/__init__.py
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     8053 2023-06-06 08:14:25.000000 faKy-1.0.0/faKy/faKy.py
-drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 08:35:58.840150 faKy-1.0.0/faKy.egg-info/
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      197 2023-06-06 08:35:58.000000 faKy-1.0.0/faKy.egg-info/PKG-INFO
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      187 2023-06-06 08:35:58.000000 faKy-1.0.0/faKy.egg-info/SOURCES.txt
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        1 2023-06-06 08:35:58.000000 faKy-1.0.0/faKy.egg-info/dependency_links.txt
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      404 2023-06-06 08:35:58.000000 faKy-1.0.0/faKy.egg-info/requires.txt
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        5 2023-06-06 08:35:58.000000 faKy-1.0.0/faKy.egg-info/top_level.txt
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)       38 2023-06-06 08:35:58.841128 faKy-1.0.0/setup.cfg
--rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     1084 2023-06-06 08:33:37.000000 faKy-1.0.0/setup.py
+drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 10:53:53.357383 faKy-1.2.0/
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      719 2023-06-06 10:53:53.357090 faKy-1.2.0/PKG-INFO
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      488 2023-06-06 09:01:46.000000 faKy-1.2.0/README.md
+drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 10:53:53.354189 faKy-1.2.0/faKy/
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        1 2023-06-06 08:19:35.000000 faKy-1.2.0/faKy/__init__.py
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)     8053 2023-06-06 08:14:25.000000 faKy-1.2.0/faKy/faKy.py
+drwxr-xr-x   0 sandrobarreshamers   (501) staff       (20)        0 2023-06-06 10:53:53.356616 faKy-1.2.0/faKy.egg-info/
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      719 2023-06-06 10:53:53.000000 faKy-1.2.0/faKy.egg-info/PKG-INFO
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      187 2023-06-06 10:53:53.000000 faKy-1.2.0/faKy.egg-info/SOURCES.txt
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        1 2023-06-06 10:53:53.000000 faKy-1.2.0/faKy.egg-info/dependency_links.txt
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      145 2023-06-06 10:53:53.000000 faKy-1.2.0/faKy.egg-info/requires.txt
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)        5 2023-06-06 10:53:53.000000 faKy-1.2.0/faKy.egg-info/top_level.txt
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)       38 2023-06-06 10:53:53.357504 faKy-1.2.0/setup.cfg
+-rw-r--r--   0 sandrobarreshamers   (501) staff       (20)      693 2023-06-06 10:51:30.000000 faKy-1.2.0/setup.py
```

### Comparing `faKy-1.0.0/faKy/faKy.py` & `faKy-1.2.0/faKy/faKy.py`

 * *Files identical despite different names*

