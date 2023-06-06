# Comparing `tmp/appier_report-1.0.1.tar.gz` & `tmp/appier_report-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appier_report-1.0.1.tar", max compression
+gzip compressed data, was "appier_report-1.0.2.tar", max compression
```

## Comparing `appier_report-1.0.1.tar` & `appier_report-1.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1062 2023-06-06 11:16:29.688183 appier_report-1.0.1/LICENSE
--rw-r--r--   0        0        0      712 2023-06-06 11:16:29.688183 appier_report-1.0.1/README.md
--rw-r--r--   0        0        0       67 2023-06-06 11:16:29.688183 appier_report-1.0.1/appier_report/__init__.py
--rw-r--r--   0        0        0     4194 2023-06-06 11:16:29.688183 appier_report-1.0.1/appier_report/cost_api.py
--rw-r--r--   0        0        0        0 2023-06-06 11:16:29.688183 appier_report-1.0.1/appier_report/utils/__init__.py
--rw-r--r--   0        0        0     1206 2023-06-06 11:16:29.688183 appier_report-1.0.1/appier_report/utils/date_utils.py
--rw-r--r--   0        0        0     2560 2023-06-06 11:16:29.692183 appier_report-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       37 2023-06-06 11:16:29.692183 appier_report-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0     1202 2023-06-06 11:16:29.692183 appier_report-1.0.1/tests/test_app.py
--rw-r--r--   0        0        0     2681 1970-01-01 00:00:00.000000 appier_report-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-06 11:27:55.672820 appier_report-1.0.2/LICENSE
+-rw-r--r--   0        0        0      712 2023-06-06 11:27:55.672820 appier_report-1.0.2/README.md
+-rw-r--r--   0        0        0       67 2023-06-06 11:27:55.672820 appier_report-1.0.2/appier_report/__init__.py
+-rw-r--r--   0        0        0     4190 2023-06-06 11:27:55.672820 appier_report-1.0.2/appier_report/cost_api.py
+-rw-r--r--   0        0        0        0 2023-06-06 11:27:55.672820 appier_report-1.0.2/appier_report/utils/__init__.py
+-rw-r--r--   0        0        0     1206 2023-06-06 11:27:55.672820 appier_report-1.0.2/appier_report/utils/date_utils.py
+-rw-r--r--   0        0        0     2560 2023-06-06 11:27:55.672820 appier_report-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-06-06 11:27:55.672820 appier_report-1.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     1202 2023-06-06 11:27:55.672820 appier_report-1.0.2/tests/test_app.py
+-rw-r--r--   0        0        0     2681 1970-01-01 00:00:00.000000 appier_report-1.0.2/PKG-INFO
```

### Comparing `appier_report-1.0.1/LICENSE` & `appier_report-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `appier_report-1.0.1/README.md` & `appier_report-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `appier_report-1.0.1/appier_report/cost_api.py` & `appier_report-1.0.2/appier_report/cost_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,16 +43,16 @@
         retry_interval: int = 30,
         **kwargs,
     ) -> list[dict]:
         """
         Get campaign report data from Appier Cost API.
 
         Args:
-            start_date: Format: YYYY-MM-DD
-            end_date: Format: YYYY-MM-DD
+            start_date: Format YYYY-MM-DD
+            end_date: Format YYYY-MM-DD
             timezone: Timezone offset in hours.
             max_retries: Number of retries before giving up.
             retry_interval: Time to wait between retries.
             **kwargs: Other parameters
 
         Note:
             The **start_date** and **end_date** should be near each other (about 5 days apart),
@@ -97,16 +97,16 @@
         retry_interval: int = 30,
         **kwargs,
     ) -> list[dict]:
         """
         Wrapper for _get_report() to get report data from Appier Cost API.
 
         Args:
-            start_date: Format: YYYY-MM-DD
-            end_date: Format: YYYY-MM-DD
+            start_date: Format YYYY-MM-DD
+            end_date: Format YYYY-MM-DD
             date_interval: Number of days between each request.
             timezone: Timezone offset in hours.
             max_retries: Number of retries before giving up.
             retry_interval: Time to wait between retries.
             **kwargs: Other parameters
 
         Returns:
```

### Comparing `appier_report-1.0.1/appier_report/utils/date_utils.py` & `appier_report-1.0.2/appier_report/utils/date_utils.py`

 * *Files identical despite different names*

### Comparing `appier_report-1.0.1/pyproject.toml` & `appier_report-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "appier-report"
-version = "1.0.1"
+version = "1.0.2"
 homepage = "https://github.com/ikamedawn/appier-report"
 description = "Report APIs wrapper"
 authors = ["ikamedawn <minhpc@ikameglobal.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `appier_report-1.0.1/tests/test_app.py` & `appier_report-1.0.2/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `appier_report-1.0.1/PKG-INFO` & `appier_report-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appier-report
-Version: 1.0.1
+Version: 1.0.2
 Summary: Report APIs wrapper
 Home-page: https://github.com/ikamedawn/appier-report
 License: MIT
 Author: ikamedawn
 Author-email: minhpc@ikameglobal.com
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 2 - Pre-Alpha
```

