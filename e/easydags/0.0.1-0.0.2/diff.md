# Comparing `tmp/easydags-0.0.1.tar.gz` & `tmp/easydags-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easydags-0.0.1.tar", last modified: Tue Jun  6 05:53:43 2023, max compression
+gzip compressed data, was "easydags-0.0.2.tar", last modified: Tue Jun  6 07:12:09 2023, max compression
```

## Comparing `easydags-0.0.1.tar` & `easydags-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-06 05:53:43.760800 easydags-0.0.1/
--rw-r--r--   0 mateograciano   (501) staff       (20)    11357 2023-06-06 04:52:19.000000 easydags-0.0.1/LICENSE
--rw-r--r--   0 mateograciano   (501) staff       (20)      263 2023-06-06 05:53:43.760855 easydags-0.0.1/PKG-INFO
--rw-r--r--   0 mateograciano   (501) staff       (20)        0 2023-06-06 05:42:45.000000 easydags-0.0.1/README.md
-drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-06 05:53:43.759970 easydags-0.0.1/easydags/
--rw-rw-r--   0 mateograciano   (501) staff       (20)      378 2023-06-06 05:16:43.000000 easydags-0.0.1/easydags/__init__.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)      463 2023-06-03 03:27:03.000000 easydags-0.0.1/easydags/config.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)    21593 2023-06-03 18:40:29.000000 easydags-0.0.1/easydags/dag.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)      273 2023-06-03 03:27:03.000000 easydags-0.0.1/easydags/errors.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)    10737 2023-06-03 09:24:23.000000 easydags-0.0.1/easydags/node.py
--rw-rw-r--   0 mateograciano   (501) staff       (20)     3769 2023-06-06 04:57:26.000000 easydags-0.0.1/easydags/ops.py
-drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-06 05:53:43.760684 easydags-0.0.1/easydags.egg-info/
--rw-r--r--   0 mateograciano   (501) staff       (20)      263 2023-06-06 05:53:43.000000 easydags-0.0.1/easydags.egg-info/PKG-INFO
--rw-r--r--   0 mateograciano   (501) staff       (20)      278 2023-06-06 05:53:43.000000 easydags-0.0.1/easydags.egg-info/SOURCES.txt
--rw-r--r--   0 mateograciano   (501) staff       (20)        1 2023-06-06 05:53:43.000000 easydags-0.0.1/easydags.egg-info/dependency_links.txt
--rw-r--r--   0 mateograciano   (501) staff       (20)        9 2023-06-06 05:53:43.000000 easydags-0.0.1/easydags.egg-info/top_level.txt
--rw-r--r--   0 mateograciano   (501) staff       (20)      103 2023-06-06 05:45:08.000000 easydags-0.0.1/pyproject.toml
--rw-r--r--   0 mateograciano   (501) staff       (20)      371 2023-06-06 05:53:43.761121 easydags-0.0.1/setup.cfg
+drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-06 07:12:09.696858 easydags-0.0.2/
+-rw-r--r--   0 mateograciano   (501) staff       (20)    11357 2023-06-06 04:52:19.000000 easydags-0.0.2/LICENSE
+-rw-r--r--   0 mateograciano   (501) staff       (20)      197 2023-06-06 07:12:09.696726 easydags-0.0.2/PKG-INFO
+-rw-r--r--   0 mateograciano   (501) staff       (20)     4891 2023-06-06 06:48:15.000000 easydags-0.0.2/README.md
+drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-06 07:12:09.696030 easydags-0.0.2/easydags/
+-rw-rw-r--   0 mateograciano   (501) staff       (20)      378 2023-06-06 05:16:43.000000 easydags-0.0.2/easydags/__init__.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)      463 2023-06-03 03:27:03.000000 easydags-0.0.2/easydags/config.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)    21593 2023-06-03 18:40:29.000000 easydags-0.0.2/easydags/dag.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)      273 2023-06-03 03:27:03.000000 easydags-0.0.2/easydags/errors.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)    10737 2023-06-03 09:24:23.000000 easydags-0.0.2/easydags/node.py
+-rw-rw-r--   0 mateograciano   (501) staff       (20)     3769 2023-06-06 04:57:26.000000 easydags-0.0.2/easydags/ops.py
+drwxr-xr-x   0 mateograciano   (501) staff       (20)        0 2023-06-06 07:12:09.696577 easydags-0.0.2/easydags.egg-info/
+-rw-r--r--   0 mateograciano   (501) staff       (20)      197 2023-06-06 07:12:09.000000 easydags-0.0.2/easydags.egg-info/PKG-INFO
+-rw-r--r--   0 mateograciano   (501) staff       (20)      308 2023-06-06 07:12:09.000000 easydags-0.0.2/easydags.egg-info/SOURCES.txt
+-rw-r--r--   0 mateograciano   (501) staff       (20)        1 2023-06-06 07:12:09.000000 easydags-0.0.2/easydags.egg-info/dependency_links.txt
+-rw-r--r--   0 mateograciano   (501) staff       (20)       76 2023-06-06 07:12:09.000000 easydags-0.0.2/easydags.egg-info/requires.txt
+-rw-r--r--   0 mateograciano   (501) staff       (20)        9 2023-06-06 07:12:09.000000 easydags-0.0.2/easydags.egg-info/top_level.txt
+-rw-r--r--   0 mateograciano   (501) staff       (20)      104 2023-06-06 06:01:41.000000 easydags-0.0.2/pyproject.toml
+-rw-r--r--   0 mateograciano   (501) staff       (20)       38 2023-06-06 07:12:09.696897 easydags-0.0.2/setup.cfg
+-rw-r--r--   0 mateograciano   (501) staff       (20)      756 2023-06-06 07:09:24.000000 easydags-0.0.2/setup.py
```

### Comparing `easydags-0.0.1/LICENSE` & `easydags-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `easydags-0.0.1/easydags/dag.py` & `easydags-0.0.2/easydags/dag.py`

 * *Files identical despite different names*

### Comparing `easydags-0.0.1/easydags/node.py` & `easydags-0.0.2/easydags/node.py`

 * *Files identical despite different names*

### Comparing `easydags-0.0.1/easydags/ops.py` & `easydags-0.0.2/easydags/ops.py`

 * *Files identical despite different names*

