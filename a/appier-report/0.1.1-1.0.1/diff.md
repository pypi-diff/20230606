# Comparing `tmp/appier_report-0.1.1.tar.gz` & `tmp/appier_report-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appier_report-0.1.1.tar", max compression
+gzip compressed data, was "appier_report-1.0.1.tar", max compression
```

## Comparing `appier_report-0.1.1.tar` & `appier_report-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0     1062 2023-06-06 05:52:33.624571 appier_report-0.1.1/LICENSE
--rw-r--r--   0        0        0      712 2023-06-06 05:52:33.624571 appier_report-0.1.1/README.md
--rw-r--r--   0        0        0     2550 2023-06-06 05:52:33.624571 appier_report-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       71 2023-06-06 05:52:33.624571 appier_report-0.1.1/src/__init__.py
--rw-r--r--   0        0        0      381 2023-06-06 05:52:33.624571 appier_report-0.1.1/src/example.py
--rw-r--r--   0        0        0       37 2023-06-06 05:52:33.624571 appier_report-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0      394 2023-06-06 05:52:33.624571 appier_report-0.1.1/tests/test_app.py
--rw-r--r--   0        0        0     2681 1970-01-01 00:00:00.000000 appier_report-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-06 11:16:29.688183 appier_report-1.0.1/LICENSE
+-rw-r--r--   0        0        0      712 2023-06-06 11:16:29.688183 appier_report-1.0.1/README.md
+-rw-r--r--   0        0        0       67 2023-06-06 11:16:29.688183 appier_report-1.0.1/appier_report/__init__.py
+-rw-r--r--   0        0        0     4194 2023-06-06 11:16:29.688183 appier_report-1.0.1/appier_report/cost_api.py
+-rw-r--r--   0        0        0        0 2023-06-06 11:16:29.688183 appier_report-1.0.1/appier_report/utils/__init__.py
+-rw-r--r--   0        0        0     1206 2023-06-06 11:16:29.688183 appier_report-1.0.1/appier_report/utils/date_utils.py
+-rw-r--r--   0        0        0     2560 2023-06-06 11:16:29.692183 appier_report-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-06-06 11:16:29.692183 appier_report-1.0.1/tests/__init__.py
+-rw-r--r--   0        0        0     1202 2023-06-06 11:16:29.692183 appier_report-1.0.1/tests/test_app.py
+-rw-r--r--   0        0        0     2681 1970-01-01 00:00:00.000000 appier_report-1.0.1/PKG-INFO
```

### Comparing `appier_report-0.1.1/LICENSE` & `appier_report-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `appier_report-0.1.1/README.md` & `appier_report-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `appier_report-0.1.1/pyproject.toml` & `appier_report-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool]
 [tool.poetry]
 name = "appier-report"
-version = "0.1.1"
+version = "1.0.1"
 homepage = "https://github.com/ikamedawn/appier-report"
 description = "Report APIs wrapper"
 authors = ["ikamedawn <minhpc@ikameglobal.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     'Development Status :: 2 - Pre-Alpha',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: MIT License',
     'Natural Language :: English',
     'Programming Language :: Python :: 3.10',
 ]
 packages = [
-    { include = "src" },
+    { include = "appier_report" },
     { include = "tests", format = "sdist" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.10, <3.12"
 
 black = { version = "^23.3.0", optional = true }
```

### Comparing `appier_report-0.1.1/PKG-INFO` & `appier_report-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appier-report
-Version: 0.1.1
+Version: 1.0.1
 Summary: Report APIs wrapper
 Home-page: https://github.com/ikamedawn/appier-report
 License: MIT
 Author: ikamedawn
 Author-email: minhpc@ikameglobal.com
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 2 - Pre-Alpha
```

