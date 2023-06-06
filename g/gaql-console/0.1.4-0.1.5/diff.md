# Comparing `tmp/gaql_console-0.1.4.tar.gz` & `tmp/gaql_console-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaql_console-0.1.4.tar", max compression
+gzip compressed data, was "gaql_console-0.1.5.tar", max compression
```

## Comparing `gaql_console-0.1.4.tar` & `gaql_console-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0      679 2023-02-27 18:07:15.599693 gaql_console-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       20 2023-02-27 18:07:15.599693 gaql_console-0.1.4/src/gaql_console/__init__.py
--rw-r--r--   0        0        0       49 2023-02-27 18:07:15.599693 gaql_console-0.1.4/src/gaql_console/__main__.py
--rw-r--r--   0        0        0     2164 2023-02-27 18:07:15.599693 gaql_console-0.1.4/src/gaql_console/api_client.py
--rw-r--r--   0        0        0     3028 2023-02-27 18:07:15.599693 gaql_console-0.1.4/src/gaql_console/console.py
--rw-r--r--   0        0        0     2832 2023-02-27 18:07:15.599693 gaql_console-0.1.4/src/gaql_console/context.py
--rw-r--r--   0        0        0      651 2023-02-27 18:07:15.599693 gaql_console-0.1.4/src/gaql_console/exceptions.py
--rw-r--r--   0        0        0     2945 2023-02-27 18:07:15.599693 gaql_console-0.1.4/src/gaql_console/grammar.py
--rw-r--r--   0        0        0      933 1970-01-01 00:00:00.000000 gaql_console-0.1.4/setup.py
--rw-r--r--   0        0        0      669 1970-01-01 00:00:00.000000 gaql_console-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      680 2023-06-06 16:57:17.678987 gaql_console-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       20 2023-06-06 16:57:17.678987 gaql_console-0.1.5/src/gaql_console/__init__.py
+-rw-r--r--   0        0        0       49 2023-06-06 16:57:17.678987 gaql_console-0.1.5/src/gaql_console/__main__.py
+-rw-r--r--   0        0        0     2164 2023-06-06 16:57:17.678987 gaql_console-0.1.5/src/gaql_console/api_client.py
+-rw-r--r--   0        0        0     3028 2023-06-06 16:57:17.678987 gaql_console-0.1.5/src/gaql_console/console.py
+-rw-r--r--   0        0        0     2832 2023-06-06 16:57:17.678987 gaql_console-0.1.5/src/gaql_console/context.py
+-rw-r--r--   0        0        0      651 2023-06-06 16:57:17.678987 gaql_console-0.1.5/src/gaql_console/exceptions.py
+-rw-r--r--   0        0        0     2945 2023-06-06 16:57:17.678987 gaql_console-0.1.5/src/gaql_console/grammar.py
+-rw-r--r--   0        0        0      669 1970-01-01 00:00:00.000000 gaql_console-0.1.5/PKG-INFO
```

### Comparing `gaql_console-0.1.4/pyproject.toml` & `gaql_console-0.1.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "gaql-console"
-version = "0.1.4"
+version = "0.1.5"
 description = "Google Ads Query Language Interactive Console"
 authors = ["Piotr Kilczuk <piotr@kilczuk.dev>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 prompt-toolkit = "^3.0.24"
 Pygments = "^2.11.2"
-google-ads = "^20.0.0"
+google-ads = "^21.1.0"
 click = "^8.0.3"
 toml = "^0.10.2"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.1.2"
-black = "^22.6.0"
-ipython = "^8.0.1"
+pytest = "^7.3.1"
+black = "^23.3.0"
+ipython = "^8.14.0"
 
 [tool.poetry.scripts]
 gaql = "gaql_console.console:main"
 
 [tool.black]
 line-length = 119
```

### Comparing `gaql_console-0.1.4/src/gaql_console/api_client.py` & `gaql_console-0.1.5/src/gaql_console/api_client.py`

 * *Files identical despite different names*

### Comparing `gaql_console-0.1.4/src/gaql_console/console.py` & `gaql_console-0.1.5/src/gaql_console/console.py`

 * *Files identical despite different names*

### Comparing `gaql_console-0.1.4/src/gaql_console/context.py` & `gaql_console-0.1.5/src/gaql_console/context.py`

 * *Files identical despite different names*

### Comparing `gaql_console-0.1.4/src/gaql_console/exceptions.py` & `gaql_console-0.1.5/src/gaql_console/exceptions.py`

 * *Files identical despite different names*

### Comparing `gaql_console-0.1.4/src/gaql_console/grammar.py` & `gaql_console-0.1.5/src/gaql_console/grammar.py`

 * *Files identical despite different names*

### Comparing `gaql_console-0.1.4/PKG-INFO` & `gaql_console-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: gaql-console
-Version: 0.1.4
+Version: 0.1.5
 Summary: Google Ads Query Language Interactive Console
 License: MIT
 Author: Piotr Kilczuk
 Author-email: piotr@kilczuk.dev
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Pygments (>=2.11.2,<3.0.0)
 Requires-Dist: click (>=8.0.3,<9.0.0)
-Requires-Dist: google-ads (>=20.0.0,<21.0.0)
+Requires-Dist: google-ads (>=21.1.0,<22.0.0)
 Requires-Dist: prompt-toolkit (>=3.0.24,<4.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
```

