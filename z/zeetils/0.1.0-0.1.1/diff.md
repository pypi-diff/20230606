# Comparing `tmp/zeetils-0.1.0.tar.gz` & `tmp/zeetils-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeetils-0.1.0.tar", max compression
+gzip compressed data, was "zeetils-0.1.1.tar", max compression
```

## Comparing `zeetils-0.1.0.tar` & `zeetils-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-06-05 21:00:32.826270 zeetils-0.1.0/README.md
--rw-r--r--   0        0        0      326 2023-06-05 21:00:52.914891 zeetils-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-05 21:00:32.826270 zeetils-0.1.0/zeetils/__init__.py
--rw-r--r--   0        0        0     1134 2023-06-05 21:19:11.132938 zeetils-0.1.0/zeetils/classes.py
--rw-r--r--   0        0        0      275 2023-06-05 21:22:12.807958 zeetils-0.1.0/zeetils/lists.py
--rw-r--r--   0        0        0     1146 2023-06-05 21:36:17.953710 zeetils-0.1.0/zeetils/misc.py
--rw-r--r--   0        0        0      439 1970-01-01 00:00:00.000000 zeetils-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-05 21:00:32.826270 zeetils-0.1.1/README.md
+-rw-r--r--   0        0        0      326 2023-06-05 21:58:57.154960 zeetils-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      103 2023-06-05 21:58:18.037540 zeetils-0.1.1/zeetils/__init__.py
+-rw-r--r--   0        0        0     1134 2023-06-05 21:19:11.132938 zeetils-0.1.1/zeetils/classes.py
+-rw-r--r--   0        0        0      275 2023-06-05 21:22:12.807958 zeetils-0.1.1/zeetils/lists.py
+-rw-r--r--   0        0        0     1146 2023-06-05 21:36:17.953710 zeetils-0.1.1/zeetils/misc.py
+-rw-r--r--   0        0        0      439 1970-01-01 00:00:00.000000 zeetils-0.1.1/PKG-INFO
```

### Comparing `zeetils-0.1.0/zeetils/classes.py` & `zeetils-0.1.1/zeetils/classes.py`

 * *Files identical despite different names*

### Comparing `zeetils-0.1.0/zeetils/misc.py` & `zeetils-0.1.1/zeetils/misc.py`

 * *Files identical despite different names*

