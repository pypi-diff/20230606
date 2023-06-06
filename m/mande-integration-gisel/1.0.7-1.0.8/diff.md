# Comparing `tmp/mande_integration_gisel-1.0.7.tar.gz` & `tmp/mande_integration_gisel-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mande_integration_gisel-1.0.7.tar", max compression
+gzip compressed data, was "mande_integration_gisel-1.0.8.tar", max compression
```

## Comparing `mande_integration_gisel-1.0.7.tar` & `mande_integration_gisel-1.0.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    28964 2023-06-06 17:28:28.365919 mande_integration_gisel-1.0.7/mande_integration_gisel/__init__.py
--rw-r--r--   0        0        0      691 2022-07-01 09:57:35.000000 mande_integration_gisel-1.0.7/mande_integration_gisel/command.py
--rw-r--r--   0        0        0      188 2022-07-01 09:57:35.000000 mande_integration_gisel-1.0.7/mande_integration_gisel/config/__init__.py
--rw-r--r--   0        0        0      464 2022-10-27 15:42:43.000000 mande_integration_gisel-1.0.7/mande_integration_gisel/config/selectors.py
--rw-r--r--   0        0        0     2128 2023-06-06 13:56:09.418815 mande_integration_gisel-1.0.7/mande_integration_gisel/config/types.py
--rw-r--r--   0        0        0      185 2022-07-01 09:57:35.000000 mande_integration_gisel-1.0.7/mande_integration_gisel/config/variables.py
--rw-r--r--   0        0        0     2763 2023-06-06 13:29:20.189513 mande_integration_gisel-1.0.7/mande_integration_gisel/main.py
--rw-r--r--   0        0        0      229 2022-07-01 09:57:35.000000 mande_integration_gisel-1.0.7/mande_integration_gisel/organizations.py
--rw-r--r--   0        0        0     2051 2023-06-06 13:56:16.539034 mande_integration_gisel-1.0.7/mande_integration_gisel/utils/__init__.py
--rw-r--r--   0        0        0      725 2023-06-06 17:28:51.837603 mande_integration_gisel-1.0.7/pyproject.toml
--rw-r--r--   0        0        0      680 1970-01-01 00:00:00.000000 mande_integration_gisel-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0    29116 2023-06-06 20:23:58.952254 mande_integration_gisel-1.0.8/mande_integration_gisel/__init__.py
+-rw-r--r--   0        0        0      691 2022-07-01 09:57:35.000000 mande_integration_gisel-1.0.8/mande_integration_gisel/command.py
+-rw-r--r--   0        0        0      188 2022-07-01 09:57:35.000000 mande_integration_gisel-1.0.8/mande_integration_gisel/config/__init__.py
+-rw-r--r--   0        0        0      464 2022-10-27 15:42:43.000000 mande_integration_gisel-1.0.8/mande_integration_gisel/config/selectors.py
+-rw-r--r--   0        0        0     2128 2023-06-06 13:56:09.418815 mande_integration_gisel-1.0.8/mande_integration_gisel/config/types.py
+-rw-r--r--   0        0        0      185 2022-07-01 09:57:35.000000 mande_integration_gisel-1.0.8/mande_integration_gisel/config/variables.py
+-rw-r--r--   0        0        0     2763 2023-06-06 13:29:20.189513 mande_integration_gisel-1.0.8/mande_integration_gisel/main.py
+-rw-r--r--   0        0        0      229 2022-07-01 09:57:35.000000 mande_integration_gisel-1.0.8/mande_integration_gisel/organizations.py
+-rw-r--r--   0        0        0     2051 2023-06-06 13:56:16.539034 mande_integration_gisel-1.0.8/mande_integration_gisel/utils/__init__.py
+-rw-r--r--   0        0        0      725 2023-06-06 20:24:12.050526 mande_integration_gisel-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0      680 1970-01-01 00:00:00.000000 mande_integration_gisel-1.0.8/PKG-INFO
```

### Comparing `mande_integration_gisel-1.0.7/mande_integration_gisel/__init__.py` & `mande_integration_gisel-1.0.8/mande_integration_gisel/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import os
 from tkinter.tix import Tree
 from typing import Any, Dict, List, Tuple, Union
 from dataclasses import dataclass, field
 from selenium.webdriver import Chrome, Safari, Firefox, Edge
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support import expected_conditions as EC
@@ -397,23 +398,23 @@
     def add_report_body_content_name(self, row_data: Any) -> Any:
         return row_data[0].find_element(By.TAG_NAME, 'textarea').get_attribute('value').strip().lower()
     
     def add_report_body_content(self, row_data: Any) -> ExpenditureReportDetail:
         """_summary_
         """
         report = ExpenditureReportDetail(
-                description=row_data[0].find_element(By.TAG_NAME, 'textarea').get_attribute('value'),
-                narrative=row_data[1].find_element(By.TAG_NAME, 'textarea').get_attribute('value'),
-                lc_total=row_data[2].find_element(By.TAG_NAME, 'input').get_attribute('value'),
-                usd_total=row_data[3].find_element(By.TAG_NAME, 'input').get_attribute('value'),
-                percent_by_category=row_data[4].find_element(By.TAG_NAME, 'input').get_attribute('value'),
-                unexpended_balance=row_data[5].find_element(By.TAG_NAME, 'input').get_attribute('value'),
-                current_spend_lc=row_data[6].find_element(By.TAG_NAME, 'input').get_attribute('value'),
-                spend_to_date=row_data[7].find_element(By.TAG_NAME, 'input').get_attribute('value'),
-                exch_rate=row_data[8].find_element(By.TAG_NAME, 'input').get_attribute('value'),
+                description=row_data[0].find_element(By.TAG_NAME, 'textarea').get_attribute('value').strip().lower(),
+                narrative=row_data[1].find_element(By.TAG_NAME, 'textarea').get_attribute('value').strip().lower(),
+                lc_total=row_data[2].find_element(By.TAG_NAME, 'input').get_attribute('value').strip().lower(),
+                usd_total=row_data[3].find_element(By.TAG_NAME, 'input').get_attribute('value').strip().lower(),
+                percent_by_category=row_data[4].find_element(By.TAG_NAME, 'input').get_attribute('value').strip().lower(),
+                unexpended_balance=row_data[5].find_element(By.TAG_NAME, 'input').get_attribute('value').strip().lower(),
+                current_spend_lc=row_data[6].find_element(By.TAG_NAME, 'input').get_attribute('value').strip().lower(),
+                spend_to_date=row_data[7].find_element(By.TAG_NAME, 'input').get_attribute('value').strip().lower(),
+                exch_rate=row_data[8].find_element(By.TAG_NAME, 'input').get_attribute('value').strip().lower(),
         )
         
         return report
     
     def add_report_footer_content(self, row_data) -> ExpenditureReportDetail:
         report_total = ExpenditureReportDetail(
             description=row_data[0].find_element(By.TAG_NAME, 'input').get_attribute('value'),
@@ -499,19 +500,19 @@
             raise NotFoundError('Category not found')
 
         expenditure_report[category_name] = []
         category_content_body_row = self.get_detail_report_body_row(category_content)
         
         for row in category_content_body_row:
             row_data = row.find_elements(By.TAG_NAME, 'td')[1:]
-            report_name = self.add_report_body_content_name(row_data)
+            # report_name = self.add_report_body_content_name(row_data)
             report_row_data = self.add_report_body_content(row_data)
             # dct = {i: i.value for i in report_row_data}
             # print(dct)
-            expenditure_report[category_name].append({report_name: report_row_data})
+            expenditure_report[category_name].append(report_row_data.__dict__)
 
         print("🟢 Expenditure report data retrieved!")
         print(expenditure_report)
 
         return expenditure_report
```

### Comparing `mande_integration_gisel-1.0.7/mande_integration_gisel/command.py` & `mande_integration_gisel-1.0.8/mande_integration_gisel/command.py`

 * *Files identical despite different names*

### Comparing `mande_integration_gisel-1.0.7/mande_integration_gisel/config/types.py` & `mande_integration_gisel-1.0.8/mande_integration_gisel/config/types.py`

 * *Files identical despite different names*

### Comparing `mande_integration_gisel-1.0.7/mande_integration_gisel/main.py` & `mande_integration_gisel-1.0.8/mande_integration_gisel/main.py`

 * *Files identical despite different names*

### Comparing `mande_integration_gisel-1.0.7/mande_integration_gisel/utils/__init__.py` & `mande_integration_gisel-1.0.8/mande_integration_gisel/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mande_integration_gisel-1.0.7/pyproject.toml` & `mande_integration_gisel-1.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mande_integration_gisel"
-version = "1.0.7"
+version = "1.0.8"
 description = "This package Allows communication Between Mande and Gisel. Using WebScraping technics"
 authors = ["Sejen Developer <developer@sejen.ci>"]
 classifiers = [
   "Programming Language :: Python :: 3",
   "Operating System :: OS Independent",
 ]
```

### Comparing `mande_integration_gisel-1.0.7/PKG-INFO` & `mande_integration_gisel-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mande-integration-gisel
-Version: 1.0.7
+Version: 1.0.8
 Summary: This package Allows communication Between Mande and Gisel. Using WebScraping technics
 Author: Sejen Developer
 Author-email: developer@sejen.ci
 Requires-Python: >=3.9,<4.0
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

