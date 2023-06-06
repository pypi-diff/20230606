# Comparing `tmp/mande_integration_gisel-1.0.1.tar.gz` & `tmp/mande_integration_gisel-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mande_integration_gisel-1.0.1.tar", max compression
+gzip compressed data, was "mande_integration_gisel-1.0.2.tar", max compression
```

## Comparing `mande_integration_gisel-1.0.1.tar` & `mande_integration_gisel-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    28691 2023-06-06 13:50:59.193637 mande_integration_gisel-1.0.1/mande_integration_gisel/__init__.py
--rw-r--r--   0        0        0      691 2022-07-01 09:57:35.000000 mande_integration_gisel-1.0.1/mande_integration_gisel/command.py
--rw-r--r--   0        0        0      188 2022-07-01 09:57:35.000000 mande_integration_gisel-1.0.1/mande_integration_gisel/config/__init__.py
--rw-r--r--   0        0        0      464 2022-10-27 15:42:43.000000 mande_integration_gisel-1.0.1/mande_integration_gisel/config/selectors.py
--rw-r--r--   0        0        0     2121 2023-06-06 13:20:48.039157 mande_integration_gisel-1.0.1/mande_integration_gisel/config/types.py
--rw-r--r--   0        0        0      185 2022-07-01 09:57:35.000000 mande_integration_gisel-1.0.1/mande_integration_gisel/config/variables.py
--rw-r--r--   0        0        0     2763 2023-06-06 13:29:20.189513 mande_integration_gisel-1.0.1/mande_integration_gisel/main.py
--rw-r--r--   0        0        0      229 2022-07-01 09:57:35.000000 mande_integration_gisel-1.0.1/mande_integration_gisel/organizations.py
--rw-r--r--   0        0        0     2037 2023-06-06 13:20:48.039133 mande_integration_gisel-1.0.1/mande_integration_gisel/utils/__init__.py
--rw-r--r--   0        0        0      718 2023-06-06 13:52:06.882872 mande_integration_gisel-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      680 1970-01-01 00:00:00.000000 mande_integration_gisel-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    28691 2023-06-06 13:50:59.193637 mande_integration_gisel-1.0.2/mande_integration_gisel/__init__.py
+-rw-r--r--   0        0        0      691 2022-07-01 09:57:35.000000 mande_integration_gisel-1.0.2/mande_integration_gisel/command.py
+-rw-r--r--   0        0        0      188 2022-07-01 09:57:35.000000 mande_integration_gisel-1.0.2/mande_integration_gisel/config/__init__.py
+-rw-r--r--   0        0        0      464 2022-10-27 15:42:43.000000 mande_integration_gisel-1.0.2/mande_integration_gisel/config/selectors.py
+-rw-r--r--   0        0        0     2128 2023-06-06 13:56:09.418815 mande_integration_gisel-1.0.2/mande_integration_gisel/config/types.py
+-rw-r--r--   0        0        0      185 2022-07-01 09:57:35.000000 mande_integration_gisel-1.0.2/mande_integration_gisel/config/variables.py
+-rw-r--r--   0        0        0     2763 2023-06-06 13:29:20.189513 mande_integration_gisel-1.0.2/mande_integration_gisel/main.py
+-rw-r--r--   0        0        0      229 2022-07-01 09:57:35.000000 mande_integration_gisel-1.0.2/mande_integration_gisel/organizations.py
+-rw-r--r--   0        0        0     2051 2023-06-06 13:56:16.539034 mande_integration_gisel-1.0.2/mande_integration_gisel/utils/__init__.py
+-rw-r--r--   0        0        0      725 2023-06-06 13:56:43.626912 mande_integration_gisel-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      680 1970-01-01 00:00:00.000000 mande_integration_gisel-1.0.2/PKG-INFO
```

### Comparing `mande_integration_gisel-1.0.1/mande_integration_gisel/__init__.py` & `mande_integration_gisel-1.0.2/mande_integration_gisel/__init__.py`

 * *Files identical despite different names*

### Comparing `mande_integration_gisel-1.0.1/mande_integration_gisel/command.py` & `mande_integration_gisel-1.0.2/mande_integration_gisel/command.py`

 * *Files identical despite different names*

### Comparing `mande_integration_gisel-1.0.1/mande_integration_gisel/config/types.py` & `mande_integration_gisel-1.0.2/mande_integration_gisel/config/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dataclasses import dataclass, InitVar, field
 from typing import Any, Dict, List, Union
-from mandeintegration.organizations import organizations
+from mande_integration_gisel.organizations import organizations
 from enum import Enum, auto
 
 @dataclass
 class ExpenditureReport:
     category: str
     lc_total: str
     usd_total: str
```

### Comparing `mande_integration_gisel-1.0.1/mande_integration_gisel/main.py` & `mande_integration_gisel-1.0.2/mande_integration_gisel/main.py`

 * *Files identical despite different names*

### Comparing `mande_integration_gisel-1.0.1/mande_integration_gisel/utils/__init__.py` & `mande_integration_gisel-1.0.2/mande_integration_gisel/utils/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import csv
 import os
 from bs4 import BeautifulSoup
 from typing import List
-from mandeintegration.config import __DIR__
-from mandeintegration.config.types import ExpenditureReport
+from mande_integration_gisel.config import __DIR__
+from mande_integration_gisel.config.types import ExpenditureReport
 
 def generate_report(code: str):
     report_file = __DIR__ / 'reports' / f"{code}_expenditure_report.html"
     with open(report_file, 'r') as f:
         html = f.read()
 
     soup = BeautifulSoup(html, 'html.parser')
```

### Comparing `mande_integration_gisel-1.0.1/pyproject.toml` & `mande_integration_gisel-1.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mande_integration_gisel"
-version = "1.0.1"
+version = "1.0.2"
 description = "This package Allows communication Between Mande and Gisel. Using WebScraping technics"
 authors = ["Sejen Developer <developer@sejen.ci>"]
 classifiers = [
   "Programming Language :: Python :: 3",
   "Operating System :: OS Independent",
 ]
 
@@ -18,12 +18,12 @@
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 flake8 = "^4.0.1"
 black = "^22.3.0"
 Sphinx = "^5.1.0"
 
 [tool.poetry.scripts]
-test = "mandeintegration.main:main"
+test = "mande_integration_gisel.main:main"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mande_integration_gisel-1.0.1/PKG-INFO` & `mande_integration_gisel-1.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mande-integration-gisel
-Version: 1.0.1
+Version: 1.0.2
 Summary: This package Allows communication Between Mande and Gisel. Using WebScraping technics
 Author: Sejen Developer
 Author-email: developer@sejen.ci
 Requires-Python: >=3.9,<4.0
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

