# Comparing `tmp/jaclang-0.0.1.tar.gz` & `tmp/jaclang-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaclang-0.0.1.tar", last modified: Tue Jun  6 16:48:22 2023, max compression
+gzip compressed data, was "jaclang-2.0.0.tar", last modified: Tue Jun  6 16:46:30 2023, max compression
```

## Comparing `jaclang-0.0.1.tar` & `jaclang-2.0.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 ninja     (1000) ninja     (1000)        0 2023-06-06 16:48:22.342092 jaclang-0.0.1/
--rw-r--r--   0 ninja     (1000) ninja     (1000)      151 2023-06-06 16:48:22.342092 jaclang-0.0.1/PKG-INFO
--rw-r--r--   0 ninja     (1000) ninja     (1000)      376 2023-06-06 16:27:44.000000 jaclang-0.0.1/README.md
-drwxr-xr-x   0 ninja     (1000) ninja     (1000)        0 2023-06-06 16:48:22.342092 jaclang-0.0.1/jaclang.egg-info/
--rw-r--r--   0 ninja     (1000) ninja     (1000)      151 2023-06-06 16:48:22.000000 jaclang-0.0.1/jaclang.egg-info/PKG-INFO
--rw-r--r--   0 ninja     (1000) ninja     (1000)      142 2023-06-06 16:48:22.000000 jaclang-0.0.1/jaclang.egg-info/SOURCES.txt
--rw-r--r--   0 ninja     (1000) ninja     (1000)        1 2023-06-06 16:48:22.000000 jaclang-0.0.1/jaclang.egg-info/dependency_links.txt
--rw-r--r--   0 ninja     (1000) ninja     (1000)        1 2023-06-06 16:48:22.000000 jaclang-0.0.1/jaclang.egg-info/top_level.txt
--rw-r--r--   0 ninja     (1000) ninja     (1000)       38 2023-06-06 16:48:22.342092 jaclang-0.0.1/setup.cfg
--rw-r--r--   0 ninja     (1000) ninja     (1000)      410 2023-06-06 16:47:00.000000 jaclang-0.0.1/setup.py
+drwxr-xr-x   0 ninja     (1000) ninja     (1000)        0 2023-06-06 16:46:30.112150 jaclang-2.0.0/
+-rw-r--r--   0 ninja     (1000) ninja     (1000)      151 2023-06-06 16:46:30.112150 jaclang-2.0.0/PKG-INFO
+-rw-r--r--   0 ninja     (1000) ninja     (1000)      376 2023-06-06 16:27:44.000000 jaclang-2.0.0/README.md
+drwxr-xr-x   0 ninja     (1000) ninja     (1000)        0 2023-06-06 16:46:30.112150 jaclang-2.0.0/jaclang.egg-info/
+-rw-r--r--   0 ninja     (1000) ninja     (1000)      151 2023-06-06 16:46:30.000000 jaclang-2.0.0/jaclang.egg-info/PKG-INFO
+-rw-r--r--   0 ninja     (1000) ninja     (1000)      142 2023-06-06 16:46:30.000000 jaclang-2.0.0/jaclang.egg-info/SOURCES.txt
+-rw-r--r--   0 ninja     (1000) ninja     (1000)        1 2023-06-06 16:46:30.000000 jaclang-2.0.0/jaclang.egg-info/dependency_links.txt
+-rw-r--r--   0 ninja     (1000) ninja     (1000)        1 2023-06-06 16:46:30.000000 jaclang-2.0.0/jaclang.egg-info/top_level.txt
+-rw-r--r--   0 ninja     (1000) ninja     (1000)       38 2023-06-06 16:46:30.112150 jaclang-2.0.0/setup.cfg
+-rw-r--r--   0 ninja     (1000) ninja     (1000)      410 2023-06-06 16:28:24.000000 jaclang-2.0.0/setup.py
```

