# Comparing `tmp/watchmen_utilities-16.5.3.tar.gz` & `tmp/watchmen_utilities-16.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_utilities-16.5.3.tar", max compression
+gzip compressed data, was "watchmen_utilities-16.5.4.tar", max compression
```

## Comparing `watchmen_utilities-16.5.3.tar` & `watchmen_utilities-16.5.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      451 2023-06-05 01:29:03.572124 watchmen_utilities-16.5.3/pyproject.toml
--rw-r--r--   0        0        0     1151 2023-06-05 01:29:03.572124 watchmen_utilities-16.5.3/src/watchmen_utilities/__init__.py
--rw-r--r--   0        0        0     6628 2023-06-05 01:29:03.572124 watchmen_utilities-16.5.3/src/watchmen_utilities/array_helper.py
--rw-r--r--   0        0        0    20763 2023-06-05 01:29:03.572124 watchmen_utilities-16.5.3/src/watchmen_utilities/datetime_helper.py
--rw-r--r--   0        0        0      188 2023-06-05 01:29:03.572124 watchmen_utilities-16.5.3/src/watchmen_utilities/json_helper.py
--rw-r--r--   0        0        0     2143 2023-06-05 01:29:03.572124 watchmen_utilities-16.5.3/src/watchmen_utilities/logger.py
--rw-r--r--   0        0        0      954 2023-06-05 01:29:03.572124 watchmen_utilities-16.5.3/src/watchmen_utilities/numeric_helper.py
--rw-r--r--   0        0        0      352 2023-06-05 01:29:03.572124 watchmen_utilities-16.5.3/src/watchmen_utilities/string_helper.py
--rw-r--r--   0        0        0     8884 2023-06-05 01:29:03.572124 watchmen_utilities-16.5.3/src/watchmen_utilities/value_expression.py
--rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 watchmen_utilities-16.5.3/PKG-INFO
+-rw-r--r--   0        0        0      451 2023-06-06 01:45:59.169403 watchmen_utilities-16.5.4/pyproject.toml
+-rw-r--r--   0        0        0     1151 2023-06-06 01:45:59.169403 watchmen_utilities-16.5.4/src/watchmen_utilities/__init__.py
+-rw-r--r--   0        0        0     6628 2023-06-06 01:45:59.169403 watchmen_utilities-16.5.4/src/watchmen_utilities/array_helper.py
+-rw-r--r--   0        0        0    20763 2023-06-06 01:45:59.169403 watchmen_utilities-16.5.4/src/watchmen_utilities/datetime_helper.py
+-rw-r--r--   0        0        0      188 2023-06-06 01:45:59.169403 watchmen_utilities-16.5.4/src/watchmen_utilities/json_helper.py
+-rw-r--r--   0        0        0     2143 2023-06-06 01:45:59.169403 watchmen_utilities-16.5.4/src/watchmen_utilities/logger.py
+-rw-r--r--   0        0        0      954 2023-06-06 01:45:59.169403 watchmen_utilities-16.5.4/src/watchmen_utilities/numeric_helper.py
+-rw-r--r--   0        0        0      352 2023-06-06 01:45:59.169403 watchmen_utilities-16.5.4/src/watchmen_utilities/string_helper.py
+-rw-r--r--   0        0        0     8884 2023-06-06 01:45:59.169403 watchmen_utilities-16.5.4/src/watchmen_utilities/value_expression.py
+-rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 watchmen_utilities-16.5.4/PKG-INFO
```

### Comparing `watchmen_utilities-16.5.3/src/watchmen_utilities/__init__.py` & `watchmen_utilities-16.5.4/src/watchmen_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `watchmen_utilities-16.5.3/src/watchmen_utilities/array_helper.py` & `watchmen_utilities-16.5.4/src/watchmen_utilities/array_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_utilities-16.5.3/src/watchmen_utilities/datetime_helper.py` & `watchmen_utilities-16.5.4/src/watchmen_utilities/datetime_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_utilities-16.5.3/src/watchmen_utilities/logger.py` & `watchmen_utilities-16.5.4/src/watchmen_utilities/logger.py`

 * *Files identical despite different names*

### Comparing `watchmen_utilities-16.5.3/src/watchmen_utilities/numeric_helper.py` & `watchmen_utilities-16.5.4/src/watchmen_utilities/numeric_helper.py`

 * *Files identical despite different names*

### Comparing `watchmen_utilities-16.5.3/src/watchmen_utilities/value_expression.py` & `watchmen_utilities-16.5.4/src/watchmen_utilities/value_expression.py`

 * *Files identical despite different names*

### Comparing `watchmen_utilities-16.5.3/PKG-INFO` & `watchmen_utilities-16.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: watchmen-utilities
-Version: 16.5.3
+Version: 16.5.4
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

