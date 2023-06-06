# Comparing `tmp/mande_integration_gisel-1.0.4.tar.gz` & `tmp/mande_integration_gisel-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mande_integration_gisel-1.0.4.tar", max compression
+gzip compressed data, was "mande_integration_gisel-1.0.5.tar", max compression
```

## Comparing `mande_integration_gisel-1.0.4.tar` & `mande_integration_gisel-1.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    28930 2023-06-06 15:14:34.248656 mande_integration_gisel-1.0.4/mande_integration_gisel/__init__.py
--rw-r--r--   0        0        0      691 2022-07-01 09:57:35.000000 mande_integration_gisel-1.0.4/mande_integration_gisel/command.py
--rw-r--r--   0        0        0      188 2022-07-01 09:57:35.000000 mande_integration_gisel-1.0.4/mande_integration_gisel/config/__init__.py
--rw-r--r--   0        0        0      464 2022-10-27 15:42:43.000000 mande_integration_gisel-1.0.4/mande_integration_gisel/config/selectors.py
--rw-r--r--   0        0        0     2128 2023-06-06 13:56:09.418815 mande_integration_gisel-1.0.4/mande_integration_gisel/config/types.py
--rw-r--r--   0        0        0      185 2022-07-01 09:57:35.000000 mande_integration_gisel-1.0.4/mande_integration_gisel/config/variables.py
--rw-r--r--   0        0        0     2763 2023-06-06 13:29:20.189513 mande_integration_gisel-1.0.4/mande_integration_gisel/main.py
--rw-r--r--   0        0        0      229 2022-07-01 09:57:35.000000 mande_integration_gisel-1.0.4/mande_integration_gisel/organizations.py
--rw-r--r--   0        0        0     2051 2023-06-06 13:56:16.539034 mande_integration_gisel-1.0.4/mande_integration_gisel/utils/__init__.py
--rw-r--r--   0        0        0      725 2023-06-06 15:14:45.441256 mande_integration_gisel-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      680 1970-01-01 00:00:00.000000 mande_integration_gisel-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0    28945 2023-06-06 15:29:49.410283 mande_integration_gisel-1.0.5/mande_integration_gisel/__init__.py
+-rw-r--r--   0        0        0      691 2022-07-01 09:57:35.000000 mande_integration_gisel-1.0.5/mande_integration_gisel/command.py
+-rw-r--r--   0        0        0      188 2022-07-01 09:57:35.000000 mande_integration_gisel-1.0.5/mande_integration_gisel/config/__init__.py
+-rw-r--r--   0        0        0      464 2022-10-27 15:42:43.000000 mande_integration_gisel-1.0.5/mande_integration_gisel/config/selectors.py
+-rw-r--r--   0        0        0     2128 2023-06-06 13:56:09.418815 mande_integration_gisel-1.0.5/mande_integration_gisel/config/types.py
+-rw-r--r--   0        0        0      185 2022-07-01 09:57:35.000000 mande_integration_gisel-1.0.5/mande_integration_gisel/config/variables.py
+-rw-r--r--   0        0        0     2763 2023-06-06 13:29:20.189513 mande_integration_gisel-1.0.5/mande_integration_gisel/main.py
+-rw-r--r--   0        0        0      229 2022-07-01 09:57:35.000000 mande_integration_gisel-1.0.5/mande_integration_gisel/organizations.py
+-rw-r--r--   0        0        0     2051 2023-06-06 13:56:16.539034 mande_integration_gisel-1.0.5/mande_integration_gisel/utils/__init__.py
+-rw-r--r--   0        0        0      725 2023-06-06 15:32:44.215379 mande_integration_gisel-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      680 1970-01-01 00:00:00.000000 mande_integration_gisel-1.0.5/PKG-INFO
```

### Comparing `mande_integration_gisel-1.0.4/mande_integration_gisel/__init__.py` & `mande_integration_gisel-1.0.5/mande_integration_gisel/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -501,18 +501,18 @@
         expenditure_report[category_name] = []
         category_content_body_row = self.get_detail_report_body_row(category_content)
         
         for row in category_content_body_row:
             row_data = row.find_elements(By.TAG_NAME, 'td')[1:]
             report = self.add_report_body_content_name(row_data)
             report_row_data = self.add_report_body_content(row_data)
-            print('📩 Adding report body row data...')
-            print(report_row_data, "report_row_data ===>")
-            print('🟢 Report body row data added!')
-            expenditure_report[category_name].append(report)
+            # print('📩 Adding report body row data...')
+            # print(report_row_data, "report_row_data ===>")
+            # print('🟢 Report body row data added!')
+            expenditure_report[category_name].append(report_row_data)
 
         return expenditure_report
 
     
     
     # Edit summary report for all category
     def edit_summary_report(self, category: str, category_value: str, exch_rate: str) -> None:
```

### Comparing `mande_integration_gisel-1.0.4/mande_integration_gisel/command.py` & `mande_integration_gisel-1.0.5/mande_integration_gisel/command.py`

 * *Files identical despite different names*

### Comparing `mande_integration_gisel-1.0.4/mande_integration_gisel/config/types.py` & `mande_integration_gisel-1.0.5/mande_integration_gisel/config/types.py`

 * *Files identical despite different names*

### Comparing `mande_integration_gisel-1.0.4/mande_integration_gisel/main.py` & `mande_integration_gisel-1.0.5/mande_integration_gisel/main.py`

 * *Files identical despite different names*

### Comparing `mande_integration_gisel-1.0.4/mande_integration_gisel/utils/__init__.py` & `mande_integration_gisel-1.0.5/mande_integration_gisel/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mande_integration_gisel-1.0.4/pyproject.toml` & `mande_integration_gisel-1.0.5/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mande_integration_gisel"
-version = "1.0.4"
+version = "1.0.5"
 description = "This package Allows communication Between Mande and Gisel. Using WebScraping technics"
 authors = ["Sejen Developer <developer@sejen.ci>"]
 classifiers = [
   "Programming Language :: Python :: 3",
   "Operating System :: OS Independent",
 ]
```

### Comparing `mande_integration_gisel-1.0.4/PKG-INFO` & `mande_integration_gisel-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mande-integration-gisel
-Version: 1.0.4
+Version: 1.0.5
 Summary: This package Allows communication Between Mande and Gisel. Using WebScraping technics
 Author: Sejen Developer
 Author-email: developer@sejen.ci
 Requires-Python: >=3.9,<4.0
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

