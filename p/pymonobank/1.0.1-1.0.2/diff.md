# Comparing `tmp/pymonobank-1.0.1.tar.gz` & `tmp/pymonobank-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymonobank-1.0.1.tar", max compression
+gzip compressed data, was "pymonobank-1.0.2.tar", max compression
```

## Comparing `pymonobank-1.0.1.tar` & `pymonobank-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       85 2023-06-06 17:54:51.686637 pymonobank-1.0.1/README.md
--rw-r--r--   0        0        0        0 2023-06-06 18:14:14.104875 pymonobank-1.0.1/pymonobank/__init__.py
--rw-r--r--   0        0        0        0 2023-06-05 19:52:55.238124 pymonobank-1.0.1/pymonobank/core/__init__.py
--rw-r--r--   0        0        0     3766 2023-06-06 13:44:04.662926 pymonobank-1.0.1/pymonobank/core/api.py
--rw-r--r--   0        0        0       56 2023-06-05 20:33:24.324334 pymonobank-1.0.1/pymonobank/core/invoice/__init__.py
--rw-r--r--   0        0        0     1195 2023-06-06 13:38:48.747785 pymonobank-1.0.1/pymonobank/core/invoice/invoice.py
--rw-r--r--   0        0        0      670 2023-06-05 20:55:54.452138 pymonobank-1.0.1/pymonobank/core/invoice/schemas.py
--rw-r--r--   0        0        0       24 2023-06-05 20:53:41.469690 pymonobank-1.0.1/pymonobank/core/merchant/__init__.py
--rw-r--r--   0        0        0      497 2023-06-06 13:38:48.741119 pymonobank-1.0.1/pymonobank/core/merchant/merchant.py
--rw-r--r--   0        0        0       61 2023-06-05 19:57:10.270516 pymonobank-1.0.1/pymonobank/request/__init__.py
--rw-r--r--   0        0        0      115 2023-06-05 20:19:08.704472 pymonobank-1.0.1/pymonobank/request/exceptions.py
--rw-r--r--   0        0        0      284 2023-06-05 19:57:10.263849 pymonobank-1.0.1/pymonobank/request/methods.py
--rw-r--r--   0        0        0       32 2023-06-05 20:06:43.357645 pymonobank-1.0.1/pymonobank/schemas/__init__.py
--rw-r--r--   0        0        0      143 2023-06-05 20:06:43.364311 pymonobank-1.0.1/pymonobank/schemas/base.py
--rw-r--r--   0        0        0        0 2023-06-05 20:20:54.611108 pymonobank-1.0.1/pymonobank/utils/__init__.py
--rw-r--r--   0        0        0      121 2023-06-05 20:28:53.212483 pymonobank-1.0.1/pymonobank/utils/currencies/__init__.py
--rw-r--r--   0        0        0     1286 2023-06-06 18:47:44.054608 pymonobank-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2146 1970-01-01 00:00:00.000000 pymonobank-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       85 2023-06-06 17:54:51.686637 pymonobank-1.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-06 18:14:14.104875 pymonobank-1.0.2/pymonobank/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-05 19:52:55.238124 pymonobank-1.0.2/pymonobank/core/__init__.py
+-rw-r--r--   0        0        0     3766 2023-06-06 13:44:04.662926 pymonobank-1.0.2/pymonobank/core/api.py
+-rw-r--r--   0        0        0       56 2023-06-05 20:33:24.324334 pymonobank-1.0.2/pymonobank/core/invoice/__init__.py
+-rw-r--r--   0        0        0     1195 2023-06-06 13:38:48.747785 pymonobank-1.0.2/pymonobank/core/invoice/invoice.py
+-rw-r--r--   0        0        0      670 2023-06-05 20:55:54.452138 pymonobank-1.0.2/pymonobank/core/invoice/schemas.py
+-rw-r--r--   0        0        0       24 2023-06-05 20:53:41.469690 pymonobank-1.0.2/pymonobank/core/merchant/__init__.py
+-rw-r--r--   0        0        0      497 2023-06-06 13:38:48.741119 pymonobank-1.0.2/pymonobank/core/merchant/merchant.py
+-rw-r--r--   0        0        0       61 2023-06-05 19:57:10.270516 pymonobank-1.0.2/pymonobank/request/__init__.py
+-rw-r--r--   0        0        0      115 2023-06-05 20:19:08.704472 pymonobank-1.0.2/pymonobank/request/exceptions.py
+-rw-r--r--   0        0        0      284 2023-06-05 19:57:10.263849 pymonobank-1.0.2/pymonobank/request/methods.py
+-rw-r--r--   0        0        0       32 2023-06-05 20:06:43.357645 pymonobank-1.0.2/pymonobank/schemas/__init__.py
+-rw-r--r--   0        0        0      143 2023-06-05 20:06:43.364311 pymonobank-1.0.2/pymonobank/schemas/base.py
+-rw-r--r--   0        0        0        0 2023-06-05 20:20:54.611108 pymonobank-1.0.2/pymonobank/utils/__init__.py
+-rw-r--r--   0        0        0      121 2023-06-05 20:28:53.212483 pymonobank-1.0.2/pymonobank/utils/currencies/__init__.py
+-rw-r--r--   0        0        0      397 2023-06-06 18:53:23.724566 pymonobank-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      677 1970-01-01 00:00:00.000000 pymonobank-1.0.2/PKG-INFO
```

### Comparing `pymonobank-1.0.1/pymonobank/core/api.py` & `pymonobank-1.0.2/pymonobank/core/api.py`

 * *Files identical despite different names*

### Comparing `pymonobank-1.0.1/pymonobank/core/invoice/invoice.py` & `pymonobank-1.0.2/pymonobank/core/invoice/invoice.py`

 * *Files identical despite different names*

### Comparing `pymonobank-1.0.1/pymonobank/core/invoice/schemas.py` & `pymonobank-1.0.2/pymonobank/core/invoice/schemas.py`

 * *Files identical despite different names*

