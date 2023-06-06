# Comparing `tmp/pipd-0.0.7.tar.gz` & `tmp/pipd-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipd-0.0.7.tar", last modified: Tue Jun  6 09:44:33 2023, max compression
+gzip compressed data, was "pipd-0.1.0.tar", last modified: Tue Jun  6 16:22:26 2023, max compression
```

## Comparing `pipd-0.0.7.tar` & `pipd-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:44:33.814887 pipd-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-06 09:44:33.814887 pipd-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-06-06 09:44:22.000000 pipd-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:44:33.810887 pipd-0.0.7/pipd/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-06 09:44:22.000000 pipd-0.0.7/pipd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8874 2023-06-06 09:44:22.000000 pipd-0.0.7/pipd/pipd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 09:44:33.814887 pipd-0.0.7/pipd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-06 09:44:33.000000 pipd-0.0.7/pipd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-06 09:44:33.000000 pipd-0.0.7/pipd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 09:44:33.000000 pipd-0.0.7/pipd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-06 09:44:33.000000 pipd-0.0.7/pipd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 09:44:33.814887 pipd-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-06 09:44:22.000000 pipd-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:22:26.189265 pipd-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-06 16:22:26.189265 pipd-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-06-06 16:22:12.000000 pipd-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:22:26.185265 pipd-0.1.0/pipd/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-06 16:22:12.000000 pipd-0.1.0/pipd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:22:26.185265 pipd-0.1.0/pipd/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-06 16:22:12.000000 pipd-0.1.0/pipd/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-06 16:22:12.000000 pipd-0.1.0/pipd/functions/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-06 16:22:12.000000 pipd-0.1.0/pipd/functions/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-06 16:22:12.000000 pipd-0.1.0/pipd/functions/filter_cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-06 16:22:12.000000 pipd-0.1.0/pipd/functions/limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-06 16:22:12.000000 pipd-0.1.0/pipd/functions/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-06-06 16:22:12.000000 pipd-0.1.0/pipd/functions/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-06 16:22:12.000000 pipd-0.1.0/pipd/functions/read_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-06 16:22:12.000000 pipd-0.1.0/pipd/functions/read_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-06 16:22:12.000000 pipd-0.1.0/pipd/functions/read_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-06 16:22:12.000000 pipd-0.1.0/pipd/functions/shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-06 16:22:12.000000 pipd-0.1.0/pipd/functions/side.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-06 16:22:12.000000 pipd-0.1.0/pipd/functions/sleep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-06 16:22:12.000000 pipd-0.1.0/pipd/functions/tqdm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-06 16:22:12.000000 pipd-0.1.0/pipd/functions/unbatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-06 16:22:12.000000 pipd-0.1.0/pipd/functions/write_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-06 16:22:12.000000 pipd-0.1.0/pipd/functions/write_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-06 16:22:12.000000 pipd-0.1.0/pipd/pipe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:22:26.185265 pipd-0.1.0/pipd/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 16:22:12.000000 pipd-0.1.0/pipd/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3745 2023-06-06 16:22:12.000000 pipd-0.1.0/pipd/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-06 16:22:12.000000 pipd-0.1.0/pipd/tests/test_pipe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:22:26.185265 pipd-0.1.0/pipd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-06 16:22:26.000000 pipd-0.1.0/pipd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-06 16:22:26.000000 pipd-0.1.0/pipd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 16:22:26.000000 pipd-0.1.0/pipd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-06 16:22:26.000000 pipd-0.1.0/pipd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 16:22:26.189265 pipd-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-06 16:22:12.000000 pipd-0.1.0/setup.py
```

### Comparing `pipd-0.0.7/README.md` & `pipd-0.1.0/README.md`

 * *Files identical despite different names*

