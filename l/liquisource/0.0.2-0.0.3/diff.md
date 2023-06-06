# Comparing `tmp/liquisource-0.0.2.tar.gz` & `tmp/liquisource-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liquisource-0.0.2.tar", last modified: Tue Jun  6 02:22:22 2023, max compression
+gzip compressed data, was "liquisource-0.0.3.tar", last modified: Tue Jun  6 02:45:40 2023, max compression
```

## Comparing `liquisource-0.0.2.tar` & `liquisource-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 jiyi       (501) staff       (20)        0 2023-06-06 02:22:22.910416 liquisource-0.0.2/
--rw-r--r--   0 jiyi       (501) staff       (20)      240 2023-06-06 02:22:22.910241 liquisource-0.0.2/PKG-INFO
--rw-r--r--   0 jiyi       (501) staff       (20)     1122 2023-06-05 13:27:00.000000 liquisource-0.0.2/README.md
-drwxr-xr-x   0 jiyi       (501) staff       (20)        0 2023-06-06 02:22:22.908968 liquisource-0.0.2/client/
--rw-r--r--   0 jiyi       (501) staff       (20)      148 2023-06-06 02:18:51.000000 liquisource-0.0.2/client/__init__.py
--rw-r--r--   0 jiyi       (501) staff       (20)      524 2023-06-05 14:35:13.000000 liquisource-0.0.2/client/ck_client.py
--rw-r--r--   0 jiyi       (501) staff       (20)      496 2023-06-05 12:20:19.000000 liquisource-0.0.2/client/config.py
--rw-r--r--   0 jiyi       (501) staff       (20)      287 2023-06-05 12:23:42.000000 liquisource-0.0.2/client/mongo_client.py
-drwxr-xr-x   0 jiyi       (501) staff       (20)        0 2023-06-06 02:22:22.910022 liquisource-0.0.2/liquisource.egg-info/
--rw-r--r--   0 jiyi       (501) staff       (20)      240 2023-06-06 02:22:22.000000 liquisource-0.0.2/liquisource.egg-info/PKG-INFO
--rw-r--r--   0 jiyi       (501) staff       (20)      271 2023-06-06 02:22:22.000000 liquisource-0.0.2/liquisource.egg-info/SOURCES.txt
--rw-r--r--   0 jiyi       (501) staff       (20)        1 2023-06-06 02:22:22.000000 liquisource-0.0.2/liquisource.egg-info/dependency_links.txt
--rw-r--r--   0 jiyi       (501) staff       (20)       50 2023-06-06 02:22:22.000000 liquisource-0.0.2/liquisource.egg-info/requires.txt
--rw-r--r--   0 jiyi       (501) staff       (20)       19 2023-06-06 02:22:22.000000 liquisource-0.0.2/liquisource.egg-info/top_level.txt
--rw-r--r--   0 jiyi       (501) staff       (20)       38 2023-06-06 02:22:22.910471 liquisource-0.0.2/setup.cfg
--rw-r--r--   0 jiyi       (501) staff       (20)      495 2023-06-06 02:20:49.000000 liquisource-0.0.2/setup.py
+drwxr-xr-x   0 jiyi       (501) staff       (20)        0 2023-06-06 02:45:40.850237 liquisource-0.0.3/
+-rw-r--r--   0 jiyi       (501) staff       (20)      240 2023-06-06 02:45:40.850087 liquisource-0.0.3/PKG-INFO
+-rw-r--r--   0 jiyi       (501) staff       (20)     1122 2023-06-05 13:27:00.000000 liquisource-0.0.3/README.md
+drwxr-xr-x   0 jiyi       (501) staff       (20)        0 2023-06-06 02:45:40.849360 liquisource-0.0.3/client/
+-rw-r--r--   0 jiyi       (501) staff       (20)      148 2023-06-06 02:18:51.000000 liquisource-0.0.3/client/__init__.py
+-rw-r--r--   0 jiyi       (501) staff       (20)      524 2023-06-05 14:35:13.000000 liquisource-0.0.3/client/ck_client.py
+-rw-r--r--   0 jiyi       (501) staff       (20)      496 2023-06-05 12:20:19.000000 liquisource-0.0.3/client/config.py
+-rw-r--r--   0 jiyi       (501) staff       (20)      287 2023-06-05 12:23:42.000000 liquisource-0.0.3/client/mongo_client.py
+drwxr-xr-x   0 jiyi       (501) staff       (20)        0 2023-06-06 02:45:40.849923 liquisource-0.0.3/liquisource.egg-info/
+-rw-r--r--   0 jiyi       (501) staff       (20)      240 2023-06-06 02:45:40.000000 liquisource-0.0.3/liquisource.egg-info/PKG-INFO
+-rw-r--r--   0 jiyi       (501) staff       (20)      271 2023-06-06 02:45:40.000000 liquisource-0.0.3/liquisource.egg-info/SOURCES.txt
+-rw-r--r--   0 jiyi       (501) staff       (20)        1 2023-06-06 02:45:40.000000 liquisource-0.0.3/liquisource.egg-info/dependency_links.txt
+-rw-r--r--   0 jiyi       (501) staff       (20)       50 2023-06-06 02:45:40.000000 liquisource-0.0.3/liquisource.egg-info/requires.txt
+-rw-r--r--   0 jiyi       (501) staff       (20)       19 2023-06-06 02:45:40.000000 liquisource-0.0.3/liquisource.egg-info/top_level.txt
+-rw-r--r--   0 jiyi       (501) staff       (20)       38 2023-06-06 02:45:40.850286 liquisource-0.0.3/setup.cfg
+-rw-r--r--   0 jiyi       (501) staff       (20)      582 2023-06-06 02:45:36.000000 liquisource-0.0.3/setup.py
```

### Comparing `liquisource-0.0.2/README.md` & `liquisource-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `liquisource-0.0.2/client/ck_client.py` & `liquisource-0.0.3/client/ck_client.py`

 * *Files identical despite different names*

