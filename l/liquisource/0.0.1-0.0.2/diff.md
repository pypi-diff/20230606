# Comparing `tmp/liquisource-0.0.1.tar.gz` & `tmp/liquisource-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liquisource-0.0.1.tar", last modified: Mon Jun  5 15:30:29 2023, max compression
+gzip compressed data, was "liquisource-0.0.2.tar", last modified: Tue Jun  6 02:22:22 2023, max compression
```

## Comparing `liquisource-0.0.1.tar` & `liquisource-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,16 @@
-drwxr-xr-x   0 jiyi       (501) staff       (20)        0 2023-06-05 15:30:29.251185 liquisource-0.0.1/
--rw-r--r--   0 jiyi       (501) staff       (20)      240 2023-06-05 15:30:29.251012 liquisource-0.0.1/PKG-INFO
--rw-r--r--   0 jiyi       (501) staff       (20)     1122 2023-06-05 13:27:00.000000 liquisource-0.0.1/README.md
-drwxr-xr-x   0 jiyi       (501) staff       (20)        0 2023-06-05 15:30:29.250833 liquisource-0.0.1/liquisource.egg-info/
--rw-r--r--   0 jiyi       (501) staff       (20)      240 2023-06-05 15:30:29.000000 liquisource-0.0.1/liquisource.egg-info/PKG-INFO
--rw-r--r--   0 jiyi       (501) staff       (20)      192 2023-06-05 15:30:29.000000 liquisource-0.0.1/liquisource.egg-info/SOURCES.txt
--rw-r--r--   0 jiyi       (501) staff       (20)        1 2023-06-05 15:30:29.000000 liquisource-0.0.1/liquisource.egg-info/dependency_links.txt
--rw-r--r--   0 jiyi       (501) staff       (20)       50 2023-06-05 15:30:29.000000 liquisource-0.0.1/liquisource.egg-info/requires.txt
--rw-r--r--   0 jiyi       (501) staff       (20)        1 2023-06-05 15:30:29.000000 liquisource-0.0.1/liquisource.egg-info/top_level.txt
--rw-r--r--   0 jiyi       (501) staff       (20)       38 2023-06-05 15:30:29.251227 liquisource-0.0.1/setup.cfg
--rw-r--r--   0 jiyi       (501) staff       (20)      463 2023-06-05 15:29:43.000000 liquisource-0.0.1/setup.py
+drwxr-xr-x   0 jiyi       (501) staff       (20)        0 2023-06-06 02:22:22.910416 liquisource-0.0.2/
+-rw-r--r--   0 jiyi       (501) staff       (20)      240 2023-06-06 02:22:22.910241 liquisource-0.0.2/PKG-INFO
+-rw-r--r--   0 jiyi       (501) staff       (20)     1122 2023-06-05 13:27:00.000000 liquisource-0.0.2/README.md
+drwxr-xr-x   0 jiyi       (501) staff       (20)        0 2023-06-06 02:22:22.908968 liquisource-0.0.2/client/
+-rw-r--r--   0 jiyi       (501) staff       (20)      148 2023-06-06 02:18:51.000000 liquisource-0.0.2/client/__init__.py
+-rw-r--r--   0 jiyi       (501) staff       (20)      524 2023-06-05 14:35:13.000000 liquisource-0.0.2/client/ck_client.py
+-rw-r--r--   0 jiyi       (501) staff       (20)      496 2023-06-05 12:20:19.000000 liquisource-0.0.2/client/config.py
+-rw-r--r--   0 jiyi       (501) staff       (20)      287 2023-06-05 12:23:42.000000 liquisource-0.0.2/client/mongo_client.py
+drwxr-xr-x   0 jiyi       (501) staff       (20)        0 2023-06-06 02:22:22.910022 liquisource-0.0.2/liquisource.egg-info/
+-rw-r--r--   0 jiyi       (501) staff       (20)      240 2023-06-06 02:22:22.000000 liquisource-0.0.2/liquisource.egg-info/PKG-INFO
+-rw-r--r--   0 jiyi       (501) staff       (20)      271 2023-06-06 02:22:22.000000 liquisource-0.0.2/liquisource.egg-info/SOURCES.txt
+-rw-r--r--   0 jiyi       (501) staff       (20)        1 2023-06-06 02:22:22.000000 liquisource-0.0.2/liquisource.egg-info/dependency_links.txt
+-rw-r--r--   0 jiyi       (501) staff       (20)       50 2023-06-06 02:22:22.000000 liquisource-0.0.2/liquisource.egg-info/requires.txt
+-rw-r--r--   0 jiyi       (501) staff       (20)       19 2023-06-06 02:22:22.000000 liquisource-0.0.2/liquisource.egg-info/top_level.txt
+-rw-r--r--   0 jiyi       (501) staff       (20)       38 2023-06-06 02:22:22.910471 liquisource-0.0.2/setup.cfg
+-rw-r--r--   0 jiyi       (501) staff       (20)      495 2023-06-06 02:20:49.000000 liquisource-0.0.2/setup.py
```

### Comparing `liquisource-0.0.1/README.md` & `liquisource-0.0.2/README.md`

 * *Files identical despite different names*

