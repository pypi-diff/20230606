# Comparing `tmp/eidolon-0.1.1.tar.gz` & `tmp/eidolon-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eidolon-0.1.1.tar", max compression
+gzip compressed data, was "eidolon-0.1.2.tar", max compression
```

## Comparing `eidolon-0.1.1.tar` & `eidolon-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      116 2023-06-06 19:51:32.894643 eidolon-0.1.1/README.md
--rw-r--r--   0        0        0     4861 2023-06-06 19:30:56.508608 eidolon-0.1.1/eidolon/__init__.py
--rw-r--r--   0        0        0     3174 2023-06-06 20:01:33.035631 eidolon-0.1.1/eidolon/api_request.py
--rw-r--r--   0        0        0      549 2023-06-06 17:58:02.453446 eidolon-0.1.1/eidolon/tracker.py
--rw-r--r--   0        0        0      495 2023-06-06 20:05:10.338654 eidolon-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      814 1970-01-01 00:00:00.000000 eidolon-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1053 2023-06-06 20:22:19.935316 eidolon-0.1.2/LICENSE.md
+-rw-r--r--   0        0        0     1344 2023-06-06 20:18:33.530135 eidolon-0.1.2/README.md
+-rw-r--r--   0        0        0     4861 2023-06-06 19:30:56.508608 eidolon-0.1.2/eidolon/__init__.py
+-rw-r--r--   0        0        0     3174 2023-06-06 20:01:33.035631 eidolon-0.1.2/eidolon/api_request.py
+-rw-r--r--   0        0        0      549 2023-06-06 17:58:02.453446 eidolon-0.1.2/eidolon/tracker.py
+-rw-r--r--   0        0        0      495 2023-06-06 20:23:33.962520 eidolon-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2042 1970-01-01 00:00:00.000000 eidolon-0.1.2/PKG-INFO
```

### Comparing `eidolon-0.1.1/eidolon/__init__.py` & `eidolon-0.1.2/eidolon/__init__.py`

 * *Files identical despite different names*

### Comparing `eidolon-0.1.1/eidolon/api_request.py` & `eidolon-0.1.2/eidolon/api_request.py`

 * *Files identical despite different names*

### Comparing `eidolon-0.1.1/eidolon/tracker.py` & `eidolon-0.1.2/eidolon/tracker.py`

 * *Files identical despite different names*

