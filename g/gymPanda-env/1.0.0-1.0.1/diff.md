# Comparing `tmp/gymPanda_env-1.0.0.tar.gz` & `tmp/gymPanda_env-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gymPanda_env-1.0.0.tar", last modified: Tue Jun  6 20:57:29 2023, max compression
+gzip compressed data, was "gymPanda_env-1.0.1.tar", last modified: Tue Jun  6 21:05:52 2023, max compression
```

## Comparing `gymPanda_env-1.0.0.tar` & `gymPanda_env-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 vvial     (1001) vvial     (1001)        0 2023-06-06 20:57:29.388549 gymPanda_env-1.0.0/
--rw-rw-r--   0 vvial     (1001) vvial     (1001)      219 2023-06-06 20:57:29.388549 gymPanda_env-1.0.0/PKG-INFO
--rw-rw-r--   0 vvial     (1001) vvial     (1001)       26 2023-06-06 20:19:48.000000 gymPanda_env-1.0.0/README.md
-drwxrwxr-x   0 vvial     (1001) vvial     (1001)        0 2023-06-06 20:57:29.380549 gymPanda_env-1.0.0/gymPanda_env/
--rw-rw-r--   0 vvial     (1001) vvial     (1001)      129 2023-06-06 20:56:24.000000 gymPanda_env-1.0.0/gymPanda_env/__init__.py
-drwxrwxr-x   0 vvial     (1001) vvial     (1001)        0 2023-06-06 20:57:29.388549 gymPanda_env-1.0.0/gymPanda_env/envs/
--rw-rw-r--   0 vvial     (1001) vvial     (1001)     3423 2023-06-06 20:13:51.000000 gymPanda_env-1.0.0/gymPanda_env/envs/GymEnv_panda.py
--rw-rw-r--   0 vvial     (1001) vvial     (1001)       56 2023-06-06 20:56:57.000000 gymPanda_env-1.0.0/gymPanda_env/envs/__init__.py
-drwxrwxr-x   0 vvial     (1001) vvial     (1001)        0 2023-06-06 20:57:29.384549 gymPanda_env-1.0.0/gymPanda_env.egg-info/
--rw-rw-r--   0 vvial     (1001) vvial     (1001)      219 2023-06-06 20:57:29.000000 gymPanda_env-1.0.0/gymPanda_env.egg-info/PKG-INFO
--rw-rw-r--   0 vvial     (1001) vvial     (1001)      286 2023-06-06 20:57:29.000000 gymPanda_env-1.0.0/gymPanda_env.egg-info/SOURCES.txt
--rw-rw-r--   0 vvial     (1001) vvial     (1001)        1 2023-06-06 20:57:29.000000 gymPanda_env-1.0.0/gymPanda_env.egg-info/dependency_links.txt
--rw-rw-r--   0 vvial     (1001) vvial     (1001)        4 2023-06-06 20:57:29.000000 gymPanda_env-1.0.0/gymPanda_env.egg-info/requires.txt
--rw-rw-r--   0 vvial     (1001) vvial     (1001)       13 2023-06-06 20:57:29.000000 gymPanda_env-1.0.0/gymPanda_env.egg-info/top_level.txt
--rw-rw-r--   0 vvial     (1001) vvial     (1001)       38 2023-06-06 20:57:29.388549 gymPanda_env-1.0.0/setup.cfg
--rw-rw-r--   0 vvial     (1001) vvial     (1001)      397 2023-06-06 20:55:03.000000 gymPanda_env-1.0.0/setup.py
+drwxrwxr-x   0 vvial     (1001) vvial     (1001)        0 2023-06-06 21:05:52.614011 gymPanda_env-1.0.1/
+-rw-rw-r--   0 vvial     (1001) vvial     (1001)      219 2023-06-06 21:05:52.614011 gymPanda_env-1.0.1/PKG-INFO
+-rw-rw-r--   0 vvial     (1001) vvial     (1001)       26 2023-06-06 20:19:48.000000 gymPanda_env-1.0.1/README.md
+drwxrwxr-x   0 vvial     (1001) vvial     (1001)        0 2023-06-06 21:05:52.610011 gymPanda_env-1.0.1/gymPanda_env/
+-rw-rw-r--   0 vvial     (1001) vvial     (1001)      123 2023-06-06 21:03:38.000000 gymPanda_env-1.0.1/gymPanda_env/__init__.py
+drwxrwxr-x   0 vvial     (1001) vvial     (1001)        0 2023-06-06 21:05:52.614011 gymPanda_env-1.0.1/gymPanda_env/envs/
+-rw-rw-r--   0 vvial     (1001) vvial     (1001)     3423 2023-06-06 20:13:51.000000 gymPanda_env-1.0.1/gymPanda_env/envs/GymEnv_panda.py
+-rw-rw-r--   0 vvial     (1001) vvial     (1001)       56 2023-06-06 20:56:57.000000 gymPanda_env-1.0.1/gymPanda_env/envs/__init__.py
+drwxrwxr-x   0 vvial     (1001) vvial     (1001)        0 2023-06-06 21:05:52.614011 gymPanda_env-1.0.1/gymPanda_env.egg-info/
+-rw-rw-r--   0 vvial     (1001) vvial     (1001)      219 2023-06-06 21:05:52.000000 gymPanda_env-1.0.1/gymPanda_env.egg-info/PKG-INFO
+-rw-rw-r--   0 vvial     (1001) vvial     (1001)      286 2023-06-06 21:05:52.000000 gymPanda_env-1.0.1/gymPanda_env.egg-info/SOURCES.txt
+-rw-rw-r--   0 vvial     (1001) vvial     (1001)        1 2023-06-06 21:05:52.000000 gymPanda_env-1.0.1/gymPanda_env.egg-info/dependency_links.txt
+-rw-rw-r--   0 vvial     (1001) vvial     (1001)        4 2023-06-06 21:05:52.000000 gymPanda_env-1.0.1/gymPanda_env.egg-info/requires.txt
+-rw-rw-r--   0 vvial     (1001) vvial     (1001)       13 2023-06-06 21:05:52.000000 gymPanda_env-1.0.1/gymPanda_env.egg-info/top_level.txt
+-rw-rw-r--   0 vvial     (1001) vvial     (1001)       38 2023-06-06 21:05:52.614011 gymPanda_env-1.0.1/setup.cfg
+-rw-rw-r--   0 vvial     (1001) vvial     (1001)      397 2023-06-06 21:05:48.000000 gymPanda_env-1.0.1/setup.py
```

### Comparing `gymPanda_env-1.0.0/gymPanda_env/envs/GymEnv_panda.py` & `gymPanda_env-1.0.1/gymPanda_env/envs/GymEnv_panda.py`

 * *Files identical despite different names*

