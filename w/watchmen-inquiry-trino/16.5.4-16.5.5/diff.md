# Comparing `tmp/watchmen_inquiry_trino-16.5.4.tar.gz` & `tmp/watchmen_inquiry_trino-16.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_inquiry_trino-16.5.4.tar", max compression
+gzip compressed data, was "watchmen_inquiry_trino-16.5.5.tar", max compression
```

## Comparing `watchmen_inquiry_trino-16.5.4.tar` & `watchmen_inquiry_trino-16.5.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1061 2023-06-06 01:45:59.129402 watchmen_inquiry_trino-16.5.4/LICENSE
--rw-r--r--   0        0        0      482 2023-06-06 01:45:59.129402 watchmen_inquiry_trino-16.5.4/pyproject.toml
--rw-r--r--   0        0        0      150 2023-06-06 01:45:59.129402 watchmen_inquiry_trino-16.5.4/src/watchmen_inquiry_trino/__init__.py
--rw-r--r--   0        0        0       46 2023-06-06 01:45:59.129402 watchmen_inquiry_trino-16.5.4/src/watchmen_inquiry_trino/exception.py
--rw-r--r--   0        0        0     1169 2023-06-06 01:45:59.129402 watchmen_inquiry_trino-16.5.4/src/watchmen_inquiry_trino/settings.py
--rw-r--r--   0        0        0    37618 2023-06-06 01:45:59.129402 watchmen_inquiry_trino-16.5.4/src/watchmen_inquiry_trino/trino_storage.py
--rw-r--r--   0        0        0      257 2023-06-06 01:45:59.129402 watchmen_inquiry_trino-16.5.4/src/watchmen_inquiry_trino/trino_storage_helper.py
--rw-r--r--   0        0        0     7247 2023-06-06 01:45:59.129402 watchmen_inquiry_trino-16.5.4/src/watchmen_inquiry_trino/trino_storage_spi.py
--rw-r--r--   0        0        0      535 1970-01-01 00:00:00.000000 watchmen_inquiry_trino-16.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-06 07:52:17.089011 watchmen_inquiry_trino-16.5.5/LICENSE
+-rw-r--r--   0        0        0      482 2023-06-06 07:52:17.089011 watchmen_inquiry_trino-16.5.5/pyproject.toml
+-rw-r--r--   0        0        0      150 2023-06-06 07:52:17.089011 watchmen_inquiry_trino-16.5.5/src/watchmen_inquiry_trino/__init__.py
+-rw-r--r--   0        0        0       46 2023-06-06 07:52:17.089011 watchmen_inquiry_trino-16.5.5/src/watchmen_inquiry_trino/exception.py
+-rw-r--r--   0        0        0     1169 2023-06-06 07:52:17.089011 watchmen_inquiry_trino-16.5.5/src/watchmen_inquiry_trino/settings.py
+-rw-r--r--   0        0        0    37618 2023-06-06 07:52:17.089011 watchmen_inquiry_trino-16.5.5/src/watchmen_inquiry_trino/trino_storage.py
+-rw-r--r--   0        0        0      257 2023-06-06 07:52:17.089011 watchmen_inquiry_trino-16.5.5/src/watchmen_inquiry_trino/trino_storage_helper.py
+-rw-r--r--   0        0        0     7247 2023-06-06 07:52:17.089011 watchmen_inquiry_trino-16.5.5/src/watchmen_inquiry_trino/trino_storage_spi.py
+-rw-r--r--   0        0        0      535 1970-01-01 00:00:00.000000 watchmen_inquiry_trino-16.5.5/PKG-INFO
```

### Comparing `watchmen_inquiry_trino-16.5.4/LICENSE` & `watchmen_inquiry_trino-16.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_trino-16.5.4/src/watchmen_inquiry_trino/settings.py` & `watchmen_inquiry_trino-16.5.5/src/watchmen_inquiry_trino/settings.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_trino-16.5.4/src/watchmen_inquiry_trino/trino_storage.py` & `watchmen_inquiry_trino-16.5.5/src/watchmen_inquiry_trino/trino_storage.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_trino-16.5.4/src/watchmen_inquiry_trino/trino_storage_spi.py` & `watchmen_inquiry_trino-16.5.5/src/watchmen_inquiry_trino/trino_storage_spi.py`

 * *Files identical despite different names*

### Comparing `watchmen_inquiry_trino-16.5.4/PKG-INFO` & `watchmen_inquiry_trino-16.5.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: watchmen-inquiry-trino
-Version: 16.5.4
+Version: 16.5.5
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: trino (>=0.312.0,<0.313.0)
-Requires-Dist: watchmen-data-kernel (==16.5.4)
+Requires-Dist: watchmen-data-kernel (==16.5.5)
```

