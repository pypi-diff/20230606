# Comparing `tmp/easydags-0.0.2.tar.gz` & `tmp/easydags-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easydags-0.0.2.tar", last modified: Tue Jun  6 07:12:09 2023, max compression
+gzip compressed data, was "easydags-0.0.3.tar", last modified: Tue Jun  6 08:01:24 2023, max compression
```

## Comparing `easydags-0.0.2.tar` & `easydags-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-06 07:12:09.696858 easydags-0.0.2/
--rw-r--r--   0 mateograciano   (501) staff       (20)    11357 2023-06-06 04:52:19.000000 easydags-0.0.2/LICENSE
--rw-r--r--   0 mateograciano   (501) staff       (20)      197 2023-06-06 07:12:09.696726 easydags-0.0.2/PKG-INFO
--rw-r--r--   0 mateograciano   (501) staff       (20)     4891 2023-06-06 06:48:15.000000 easydags-0.0.2/README.md
-drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-06 07:12:09.696030 easydags-0.0.2/easydags/
--rw-rw-r--   0 mateograciano   (501) staff       (20)      378 2023-06-06 05:16:43.000000 easydags-0.0.2/easydags/__init__.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)      463 2023-06-03 03:27:03.000000 easydags-0.0.2/easydags/config.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)    21593 2023-06-03 18:40:29.000000 easydags-0.0.2/easydags/dag.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)      273 2023-06-03 03:27:03.000000 easydags-0.0.2/easydags/errors.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)    10737 2023-06-03 09:24:23.000000 easydags-0.0.2/easydags/node.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)     3769 2023-06-06 04:57:26.000000 easydags-0.0.2/easydags/ops.py
-drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-06 07:12:09.696577 easydags-0.0.2/easydags.egg-info/
--rw-r--r--   0 mateograciano   (501) staff       (20)      197 2023-06-06 07:12:09.000000 easydags-0.0.2/easydags.egg-info/PKG-INFO
--rw-r--r--   0 mateograciano   (501) staff       (20)      308 2023-06-06 07:12:09.000000 easydags-0.0.2/easydags.egg-info/SOURCES.txt
--rw-r--r--   0 mateograciano   (501) staff       (20)        1 2023-06-06 07:12:09.000000 easydags-0.0.2/easydags.egg-info/dependency_links.txt
--rw-r--r--   0 mateograciano   (501) staff       (20)       76 2023-06-06 07:12:09.000000 easydags-0.0.2/easydags.egg-info/requires.txt
--rw-r--r--   0 mateograciano   (501) staff       (20)        9 2023-06-06 07:12:09.000000 easydags-0.0.2/easydags.egg-info/top_level.txt
--rw-r--r--   0 mateograciano   (501) staff       (20)      104 2023-06-06 06:01:41.000000 easydags-0.0.2/pyproject.toml
--rw-r--r--   0 mateograciano   (501) staff       (20)       38 2023-06-06 07:12:09.696897 easydags-0.0.2/setup.cfg
--rw-r--r--   0 mateograciano   (501) staff       (20)      756 2023-06-06 07:09:24.000000 easydags-0.0.2/setup.py
+drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-06 08:01:24.032981 easydags-0.0.3/
+-rw-r--r--   0 mateograciano   (501) staff       (20)    11357 2023-06-06 04:52:19.000000 easydags-0.0.3/LICENSE
+-rw-r--r--   0 mateograciano   (501) staff       (20)     9014 2023-06-06 08:01:24.032770 easydags-0.0.3/PKG-INFO
+-rw-r--r--   0 mateograciano   (501) staff       (20)     8775 2023-06-06 07:48:07.000000 easydags-0.0.3/README.md
+drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-06 08:01:24.031892 easydags-0.0.3/easydags/
+-rw-rw-r--   0 mateograciano   (501) staff       (20)      378 2023-06-06 05:16:43.000000 easydags-0.0.3/easydags/__init__.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)      463 2023-06-03 03:27:03.000000 easydags-0.0.3/easydags/config.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)    21593 2023-06-03 18:40:29.000000 easydags-0.0.3/easydags/dag.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)      273 2023-06-03 03:27:03.000000 easydags-0.0.3/easydags/errors.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)    10737 2023-06-03 09:24:23.000000 easydags-0.0.3/easydags/node.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)     3769 2023-06-06 04:57:26.000000 easydags-0.0.3/easydags/ops.py
+drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-06 08:01:24.032599 easydags-0.0.3/easydags.egg-info/
+-rw-r--r--   0 mateograciano   (501) staff       (20)     9014 2023-06-06 08:01:23.000000 easydags-0.0.3/easydags.egg-info/PKG-INFO
+-rw-r--r--   0 mateograciano   (501) staff       (20)      308 2023-06-06 08:01:24.000000 easydags-0.0.3/easydags.egg-info/SOURCES.txt
+-rw-r--r--   0 mateograciano   (501) staff       (20)        1 2023-06-06 08:01:24.000000 easydags-0.0.3/easydags.egg-info/dependency_links.txt
+-rw-r--r--   0 mateograciano   (501) staff       (20)       76 2023-06-06 08:01:24.000000 easydags-0.0.3/easydags.egg-info/requires.txt
+-rw-r--r--   0 mateograciano   (501) staff       (20)        9 2023-06-06 08:01:24.000000 easydags-0.0.3/easydags.egg-info/top_level.txt
+-rw-r--r--   0 mateograciano   (501) staff       (20)      104 2023-06-06 07:55:47.000000 easydags-0.0.3/pyproject.toml
+-rw-r--r--   0 mateograciano   (501) staff       (20)       38 2023-06-06 08:01:24.033019 easydags-0.0.3/setup.cfg
+-rw-r--r--   0 mateograciano   (501) staff       (20)     1011 2023-06-06 08:01:21.000000 easydags-0.0.3/setup.py
```

### Comparing `easydags-0.0.2/LICENSE` & `easydags-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `easydags-0.0.2/easydags/dag.py` & `easydags-0.0.3/easydags/dag.py`

 * *Files identical despite different names*

### Comparing `easydags-0.0.2/easydags/node.py` & `easydags-0.0.3/easydags/node.py`

 * *Files identical despite different names*

### Comparing `easydags-0.0.2/easydags/ops.py` & `easydags-0.0.3/easydags/ops.py`

 * *Files identical despite different names*

