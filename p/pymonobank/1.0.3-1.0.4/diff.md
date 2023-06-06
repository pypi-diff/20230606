# Comparing `tmp/pymonobank-1.0.3.tar.gz` & `tmp/pymonobank-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymonobank-1.0.3.tar", max compression
+gzip compressed data, was "pymonobank-1.0.4.tar", max compression
```

## Comparing `pymonobank-1.0.3.tar` & `pymonobank-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       85 2023-06-06 17:54:51.686637 pymonobank-1.0.3/README.md
--rw-r--r--   0        0        0      242 2023-06-06 18:57:40.436318 pymonobank-1.0.3/pymonobank/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 19:52:55.238124 pymonobank-1.0.3/pymonobank/core/__init__.py
--rw-r--r--   0        0        0     3772 2023-06-06 18:57:40.426319 pymonobank-1.0.3/pymonobank/core/api.py
--rw-r--r--   0        0        0       56 2023-06-05 20:33:24.324334 pymonobank-1.0.3/pymonobank/core/invoice/__init__.py
--rw-r--r--   0        0        0     1207 2023-06-06 18:57:40.432985 pymonobank-1.0.3/pymonobank/core/invoice/invoice.py
--rw-r--r--   0        0        0      682 2023-06-06 18:57:40.449651 pymonobank-1.0.3/pymonobank/core/invoice/schemas.py
--rw-r--r--   0        0        0       24 2023-06-05 20:53:41.469690 pymonobank-1.0.3/pymonobank/core/merchant/__init__.py
--rw-r--r--   0        0        0      509 2023-06-06 18:57:40.446318 pymonobank-1.0.3/pymonobank/core/merchant/merchant.py
--rw-r--r--   0        0        0       61 2023-06-05 19:57:10.270516 pymonobank-1.0.3/pymonobank/request/__init__.py
--rw-r--r--   0        0        0      115 2023-06-05 20:19:08.704472 pymonobank-1.0.3/pymonobank/request/exceptions.py
--rw-r--r--   0        0        0      284 2023-06-05 19:57:10.263849 pymonobank-1.0.3/pymonobank/request/methods.py
--rw-r--r--   0        0        0       32 2023-06-05 20:06:43.357645 pymonobank-1.0.3/pymonobank/schemas/__init__.py
--rw-r--r--   0        0        0      143 2023-06-05 20:06:43.364311 pymonobank-1.0.3/pymonobank/schemas/base.py
--rw-r--r--   0        0        0        0 2023-06-05 20:20:54.611108 pymonobank-1.0.3/pymonobank/utils/__init__.py
--rw-r--r--   0        0        0      121 2023-06-05 20:28:53.212483 pymonobank-1.0.3/pymonobank/utils/currencies/__init__.py
--rw-r--r--   0        0        0      397 2023-06-06 18:57:46.242663 pymonobank-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      677 1970-01-01 00:00:00.000000 pymonobank-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0       85 2023-06-06 17:54:51.686637 pymonobank-1.0.4/README.md
+-rw-r--r--   0        0        0      242 2023-06-06 18:57:40.436318 pymonobank-1.0.4/pymonobank/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 19:52:55.238124 pymonobank-1.0.4/pymonobank/core/__init__.py
+-rw-r--r--   0        0        0     3772 2023-06-06 18:57:40.426319 pymonobank-1.0.4/pymonobank/core/api.py
+-rw-r--r--   0        0        0       56 2023-06-05 20:33:24.324334 pymonobank-1.0.4/pymonobank/core/invoice/__init__.py
+-rw-r--r--   0        0        0     1207 2023-06-06 18:57:40.432985 pymonobank-1.0.4/pymonobank/core/invoice/invoice.py
+-rw-r--r--   0        0        0      682 2023-06-06 18:57:40.449651 pymonobank-1.0.4/pymonobank/core/invoice/schemas.py
+-rw-r--r--   0        0        0       24 2023-06-05 20:53:41.469690 pymonobank-1.0.4/pymonobank/core/merchant/__init__.py
+-rw-r--r--   0        0        0      509 2023-06-06 18:57:40.446318 pymonobank-1.0.4/pymonobank/core/merchant/merchant.py
+-rw-r--r--   0        0        0       61 2023-06-05 19:57:10.270516 pymonobank-1.0.4/pymonobank/request/__init__.py
+-rw-r--r--   0        0        0      115 2023-06-05 20:19:08.704472 pymonobank-1.0.4/pymonobank/request/exceptions.py
+-rw-r--r--   0        0        0      284 2023-06-05 19:57:10.263849 pymonobank-1.0.4/pymonobank/request/methods.py
+-rw-r--r--   0        0        0       32 2023-06-05 20:06:43.357645 pymonobank-1.0.4/pymonobank/schemas/__init__.py
+-rw-r--r--   0        0        0      143 2023-06-05 20:06:43.364311 pymonobank-1.0.4/pymonobank/schemas/base.py
+-rw-r--r--   0        0        0        0 2023-06-05 20:20:54.611108 pymonobank-1.0.4/pymonobank/utils/__init__.py
+-rw-r--r--   0        0        0      121 2023-06-05 20:28:53.212483 pymonobank-1.0.4/pymonobank/utils/currencies/__init__.py
+-rw-r--r--   0        0        0      454 2023-06-06 19:10:12.075828 pymonobank-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      797 1970-01-01 00:00:00.000000 pymonobank-1.0.4/PKG-INFO
```

### Comparing `pymonobank-1.0.3/pymonobank/core/api.py` & `pymonobank-1.0.4/pymonobank/core/api.py`

 * *Files identical despite different names*

### Comparing `pymonobank-1.0.3/pymonobank/core/invoice/invoice.py` & `pymonobank-1.0.4/pymonobank/core/invoice/invoice.py`

 * *Files identical despite different names*

### Comparing `pymonobank-1.0.3/pymonobank/core/invoice/schemas.py` & `pymonobank-1.0.4/pymonobank/core/invoice/schemas.py`

 * *Files identical despite different names*

### Comparing `pymonobank-1.0.3/PKG-INFO` & `pymonobank-1.0.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: pymonobank
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python client for Monobank API
+Home-page: https://github.com/Alex-Stulen/pymonobank
 Author: Alex Stulen
 Author-email: ookno16@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: certifi (==2023.5.7)
 Requires-Dist: charset-normalizer (==3.1.0)
 Requires-Dist: idna (==3.4)
 Requires-Dist: requests (==2.31.0)
 Requires-Dist: urllib3 (==2.0.2)
+Project-URL: Repository, https://github.com/Alex-Stulen/pymonobank
 Description-Content-Type: text/markdown
 
 # Python client for [Monobank API](https://api.monobank.ua/docs/acquiring.html)
 
 ---
```

