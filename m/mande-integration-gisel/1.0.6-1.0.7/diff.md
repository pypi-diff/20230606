# Comparing `tmp/mande_integration_gisel-1.0.6.tar.gz` & `tmp/mande_integration_gisel-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mande_integration_gisel-1.0.6.tar", max compression
+gzip compressed data, was "mande_integration_gisel-1.0.7.tar", max compression
```

## Comparing `mande_integration_gisel-1.0.6.tar` & `mande_integration_gisel-1.0.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    28795 2023-06-06 16:26:53.977774 mande_integration_gisel-1.0.6/mande_integration_gisel/__init__.py
--rw-r--r--   0        0        0      691 2022-07-01 09:57:35.000000 mande_integration_gisel-1.0.6/mande_integration_gisel/command.py
--rw-r--r--   0        0        0      188 2022-07-01 09:57:35.000000 mande_integration_gisel-1.0.6/mande_integration_gisel/config/__init__.py
--rw-r--r--   0        0        0      464 2022-10-27 15:42:43.000000 mande_integration_gisel-1.0.6/mande_integration_gisel/config/selectors.py
--rw-r--r--   0        0        0     2128 2023-06-06 13:56:09.418815 mande_integration_gisel-1.0.6/mande_integration_gisel/config/types.py
--rw-r--r--   0        0        0      185 2022-07-01 09:57:35.000000 mande_integration_gisel-1.0.6/mande_integration_gisel/config/variables.py
--rw-r--r--   0        0        0     2763 2023-06-06 13:29:20.189513 mande_integration_gisel-1.0.6/mande_integration_gisel/main.py
--rw-r--r--   0        0        0      229 2022-07-01 09:57:35.000000 mande_integration_gisel-1.0.6/mande_integration_gisel/organizations.py
--rw-r--r--   0        0        0     2051 2023-06-06 13:56:16.539034 mande_integration_gisel-1.0.6/mande_integration_gisel/utils/__init__.py
--rw-r--r--   0        0        0      725 2023-06-06 16:26:59.872486 mande_integration_gisel-1.0.6/pyproject.toml
--rw-r--r--   0        0        0      680 1970-01-01 00:00:00.000000 mande_integration_gisel-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0    28964 2023-06-06 17:28:28.365919 mande_integration_gisel-1.0.7/mande_integration_gisel/__init__.py
+-rw-r--r--   0        0        0      691 2022-07-01 09:57:35.000000 mande_integration_gisel-1.0.7/mande_integration_gisel/command.py
+-rw-r--r--   0        0        0      188 2022-07-01 09:57:35.000000 mande_integration_gisel-1.0.7/mande_integration_gisel/config/__init__.py
+-rw-r--r--   0        0        0      464 2022-10-27 15:42:43.000000 mande_integration_gisel-1.0.7/mande_integration_gisel/config/selectors.py
+-rw-r--r--   0        0        0     2128 2023-06-06 13:56:09.418815 mande_integration_gisel-1.0.7/mande_integration_gisel/config/types.py
+-rw-r--r--   0        0        0      185 2022-07-01 09:57:35.000000 mande_integration_gisel-1.0.7/mande_integration_gisel/config/variables.py
+-rw-r--r--   0        0        0     2763 2023-06-06 13:29:20.189513 mande_integration_gisel-1.0.7/mande_integration_gisel/main.py
+-rw-r--r--   0        0        0      229 2022-07-01 09:57:35.000000 mande_integration_gisel-1.0.7/mande_integration_gisel/organizations.py
+-rw-r--r--   0        0        0     2051 2023-06-06 13:56:16.539034 mande_integration_gisel-1.0.7/mande_integration_gisel/utils/__init__.py
+-rw-r--r--   0        0        0      725 2023-06-06 17:28:51.837603 mande_integration_gisel-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0      680 1970-01-01 00:00:00.000000 mande_integration_gisel-1.0.7/PKG-INFO
```

### Comparing `mande_integration_gisel-1.0.6/mande_integration_gisel/__init__.py` & `mande_integration_gisel-1.0.7/mande_integration_gisel/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import json
 import os
 from tkinter.tix import Tree
 from typing import Any, Dict, List, Tuple, Union
 from dataclasses import dataclass, field
 from selenium.webdriver import Chrome, Safari, Firefox, Edge
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support import expected_conditions as EC
@@ -500,17 +499,22 @@
             raise NotFoundError('Category not found')
 
         expenditure_report[category_name] = []
         category_content_body_row = self.get_detail_report_body_row(category_content)
         
         for row in category_content_body_row:
             row_data = row.find_elements(By.TAG_NAME, 'td')[1:]
-            # report = self.add_report_body_content_name(row_data)
+            report_name = self.add_report_body_content_name(row_data)
             report_row_data = self.add_report_body_content(row_data)
-            expenditure_report[category_name].append(json.dumps(report_row_data))
+            # dct = {i: i.value for i in report_row_data}
+            # print(dct)
+            expenditure_report[category_name].append({report_name: report_row_data})
+
+        print("🟢 Expenditure report data retrieved!")
+        print(expenditure_report)
 
         return expenditure_report
 
     
     
     # Edit summary report for all category
     def edit_summary_report(self, category: str, category_value: str, exch_rate: str) -> None:
```

### Comparing `mande_integration_gisel-1.0.6/mande_integration_gisel/command.py` & `mande_integration_gisel-1.0.7/mande_integration_gisel/command.py`

 * *Files identical despite different names*

### Comparing `mande_integration_gisel-1.0.6/mande_integration_gisel/config/types.py` & `mande_integration_gisel-1.0.7/mande_integration_gisel/config/types.py`

 * *Files identical despite different names*

### Comparing `mande_integration_gisel-1.0.6/mande_integration_gisel/main.py` & `mande_integration_gisel-1.0.7/mande_integration_gisel/main.py`

 * *Files identical despite different names*

### Comparing `mande_integration_gisel-1.0.6/mande_integration_gisel/utils/__init__.py` & `mande_integration_gisel-1.0.7/mande_integration_gisel/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mande_integration_gisel-1.0.6/pyproject.toml` & `mande_integration_gisel-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mande_integration_gisel"
-version = "1.0.6"
+version = "1.0.7"
 description = "This package Allows communication Between Mande and Gisel. Using WebScraping technics"
 authors = ["Sejen Developer <developer@sejen.ci>"]
 classifiers = [
   "Programming Language :: Python :: 3",
   "Operating System :: OS Independent",
 ]
```

### Comparing `mande_integration_gisel-1.0.6/PKG-INFO` & `mande_integration_gisel-1.0.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mande-integration-gisel
-Version: 1.0.6
+Version: 1.0.7
 Summary: This package Allows communication Between Mande and Gisel. Using WebScraping technics
 Author: Sejen Developer
 Author-email: developer@sejen.ci
 Requires-Python: >=3.9,<4.0
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

