# Comparing `tmp/chima-0.0.3.tar.gz` & `tmp/chima-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chima-0.0.3.tar", max compression
+gzip compressed data, was "chima-0.0.4.tar", max compression
```

## Comparing `chima-0.0.3.tar` & `chima-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0        0 2023-06-05 22:22:42.121203 chima-0.0.3/README.md
--rw-r--r--   0        0        0      365 2023-06-05 22:22:42.121203 chima-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      191 2023-06-05 22:22:42.121203 chima-0.0.3/src/chima/__init__.py
--rw-r--r--   0        0        0     4966 2023-06-05 22:22:42.121203 chima-0.0.3/src/chima/client.py
--rw-r--r--   0        0        0      348 2023-06-05 22:22:42.121203 chima-0.0.3/src/chima/core/__init__.py
--rw-r--r--   0        0        0      426 2023-06-05 22:22:42.121203 chima-0.0.3/src/chima/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-06-05 22:22:42.121203 chima-0.0.3/src/chima/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-06-05 22:22:42.121203 chima-0.0.3/src/chima/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-06-05 22:22:42.121203 chima-0.0.3/src/chima/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      159 2023-06-05 22:22:42.121203 chima-0.0.3/src/chima/environment.py
--rw-r--r--   0        0        0        0 2023-06-05 22:22:42.121203 chima-0.0.3/src/chima/py.typed
--rw-r--r--   0        0        0      139 2023-06-05 22:22:42.121203 chima-0.0.3/src/chima/types/__init__.py
--rw-r--r--   0        0        0      920 2023-06-05 22:22:42.121203 chima-0.0.3/src/chima/types/search_response.py
--rw-r--r--   0        0        0      502 1970-01-01 00:00:00.000000 chima-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2253 2023-06-06 02:28:41.301787 chima-0.0.4/README.md
+-rw-r--r--   0        0        0      365 2023-06-06 02:28:41.301787 chima-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      191 2023-06-06 02:28:41.301787 chima-0.0.4/src/chima/__init__.py
+-rw-r--r--   0        0        0     4966 2023-06-06 02:28:41.301787 chima-0.0.4/src/chima/client.py
+-rw-r--r--   0        0        0      348 2023-06-06 02:28:41.301787 chima-0.0.4/src/chima/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-06-06 02:28:41.301787 chima-0.0.4/src/chima/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-06-06 02:28:41.301787 chima-0.0.4/src/chima/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-06-06 02:28:41.301787 chima-0.0.4/src/chima/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-06-06 02:28:41.301787 chima-0.0.4/src/chima/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      159 2023-06-06 02:28:41.301787 chima-0.0.4/src/chima/environment.py
+-rw-r--r--   0        0        0        0 2023-06-06 02:28:41.301787 chima-0.0.4/src/chima/py.typed
+-rw-r--r--   0        0        0      139 2023-06-06 02:28:41.301787 chima-0.0.4/src/chima/types/__init__.py
+-rw-r--r--   0        0        0      920 2023-06-06 02:28:41.301787 chima-0.0.4/src/chima/types/search_response.py
+-rw-r--r--   0        0        0     2683 1970-01-01 00:00:00.000000 chima-0.0.4/PKG-INFO
```

### Comparing `chima-0.0.3/src/chima/client.py` & `chima-0.0.4/src/chima/client.py`

 * *Files identical despite different names*

### Comparing `chima-0.0.3/src/chima/core/datetime_utils.py` & `chima-0.0.4/src/chima/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `chima-0.0.3/src/chima/core/jsonable_encoder.py` & `chima-0.0.4/src/chima/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `chima-0.0.3/src/chima/types/search_response.py` & `chima-0.0.4/src/chima/types/search_response.py`

 * *Files identical despite different names*

