# Comparing `tmp/mande_integration_gisel-1.0.0.tar.gz` & `tmp/mande_integration_gisel-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mande_integration_gisel-1.0.0.tar", max compression
+gzip compressed data, was "mande_integration_gisel-1.0.1.tar", max compression
```

## Comparing `mande_integration_gisel-1.0.0.tar` & `mande_integration_gisel-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    28670 2023-06-06 13:20:48.039608 mande_integration_gisel-1.0.0/mande_integration_gisel/__init__.py
--rw-r--r--   0        0        0      691 2022-07-01 09:57:35.000000 mande_integration_gisel-1.0.0/mande_integration_gisel/command.py
--rw-r--r--   0        0        0      188 2022-07-01 09:57:35.000000 mande_integration_gisel-1.0.0/mande_integration_gisel/config/__init__.py
--rw-r--r--   0        0        0      464 2022-10-27 15:42:43.000000 mande_integration_gisel-1.0.0/mande_integration_gisel/config/selectors.py
--rw-r--r--   0        0        0     2121 2023-06-06 13:20:48.039157 mande_integration_gisel-1.0.0/mande_integration_gisel/config/types.py
--rw-r--r--   0        0        0      185 2022-07-01 09:57:35.000000 mande_integration_gisel-1.0.0/mande_integration_gisel/config/variables.py
--rw-r--r--   0        0        0     2763 2023-06-06 13:29:20.189513 mande_integration_gisel-1.0.0/mande_integration_gisel/main.py
--rw-r--r--   0        0        0      229 2022-07-01 09:57:35.000000 mande_integration_gisel-1.0.0/mande_integration_gisel/organizations.py
--rw-r--r--   0        0        0     2037 2023-06-06 13:20:48.039133 mande_integration_gisel-1.0.0/mande_integration_gisel/utils/__init__.py
--rw-r--r--   0        0        0      719 2023-06-06 13:28:31.357316 mande_integration_gisel-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      681 1970-01-01 00:00:00.000000 mande_integration_gisel-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    28691 2023-06-06 13:50:59.193637 mande_integration_gisel-1.0.1/mande_integration_gisel/__init__.py
+-rw-r--r--   0        0        0      691 2022-07-01 09:57:35.000000 mande_integration_gisel-1.0.1/mande_integration_gisel/command.py
+-rw-r--r--   0        0        0      188 2022-07-01 09:57:35.000000 mande_integration_gisel-1.0.1/mande_integration_gisel/config/__init__.py
+-rw-r--r--   0        0        0      464 2022-10-27 15:42:43.000000 mande_integration_gisel-1.0.1/mande_integration_gisel/config/selectors.py
+-rw-r--r--   0        0        0     2121 2023-06-06 13:20:48.039157 mande_integration_gisel-1.0.1/mande_integration_gisel/config/types.py
+-rw-r--r--   0        0        0      185 2022-07-01 09:57:35.000000 mande_integration_gisel-1.0.1/mande_integration_gisel/config/variables.py
+-rw-r--r--   0        0        0     2763 2023-06-06 13:29:20.189513 mande_integration_gisel-1.0.1/mande_integration_gisel/main.py
+-rw-r--r--   0        0        0      229 2022-07-01 09:57:35.000000 mande_integration_gisel-1.0.1/mande_integration_gisel/organizations.py
+-rw-r--r--   0        0        0     2037 2023-06-06 13:20:48.039133 mande_integration_gisel-1.0.1/mande_integration_gisel/utils/__init__.py
+-rw-r--r--   0        0        0      718 2023-06-06 13:52:06.882872 mande_integration_gisel-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      680 1970-01-01 00:00:00.000000 mande_integration_gisel-1.0.1/PKG-INFO
```

### Comparing `mande_integration_gisel-1.0.0/mande_integration_gisel/__init__.py` & `mande_integration_gisel-1.0.1/mande_integration_gisel/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 from selenium.webdriver import ChromeOptions, FirefoxOptions, EdgeOptions
 from selenium.webdriver.safari.options import Options as SafariOptions
 from webdriver_manager.chrome import ChromeDriverManager
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.common.exceptions import NoSuchElementException
 from selenium.common.exceptions import StaleElementReferenceException
 
-from mandeintegration.config import LOGIN_URL, __DIR__
-from mandeintegration.config.selectors import BrowserSelector
-from mandeintegration.config.types import ExpenditureReport, ExpenditureReportDetail, Project, PaginationDirection
+from mande_integration_gisel.config import LOGIN_URL, __DIR__
+from mande_integration_gisel.config.selectors import BrowserSelector
+from mande_integration_gisel.config.types import ExpenditureReport, ExpenditureReportDetail, Project, PaginationDirection
 from datetime import datetime
 import time
 
 # __version__ = '0.1.5'
 
 class NotFoundError(Exception):
     pass
```

### Comparing `mande_integration_gisel-1.0.0/mande_integration_gisel/command.py` & `mande_integration_gisel-1.0.1/mande_integration_gisel/command.py`

 * *Files identical despite different names*

### Comparing `mande_integration_gisel-1.0.0/mande_integration_gisel/config/types.py` & `mande_integration_gisel-1.0.1/mande_integration_gisel/config/types.py`

 * *Files identical despite different names*

### Comparing `mande_integration_gisel-1.0.0/mande_integration_gisel/main.py` & `mande_integration_gisel-1.0.1/mande_integration_gisel/main.py`

 * *Files identical despite different names*

### Comparing `mande_integration_gisel-1.0.0/mande_integration_gisel/utils/__init__.py` & `mande_integration_gisel-1.0.1/mande_integration_gisel/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mande_integration_gisel-1.0.0/pyproject.toml` & `mande_integration_gisel-1.0.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "mande_integration_gisel"
-version = "1.0.0"
-description = "This package Allows communication Between Mande and Gisel. Using WebScrpaping technics"
+version = "1.0.1"
+description = "This package Allows communication Between Mande and Gisel. Using WebScraping technics"
 authors = ["Sejen Developer <developer@sejen.ci>"]
 classifiers = [
   "Programming Language :: Python :: 3",
   "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `mande_integration_gisel-1.0.0/PKG-INFO` & `mande_integration_gisel-1.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mande-integration-gisel
-Version: 1.0.0
-Summary: This package Allows communication Between Mande and Gisel. Using WebScrpaping technics
+Version: 1.0.1
+Summary: This package Allows communication Between Mande and Gisel. Using WebScraping technics
 Author: Sejen Developer
 Author-email: developer@sejen.ci
 Requires-Python: >=3.9,<4.0
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

