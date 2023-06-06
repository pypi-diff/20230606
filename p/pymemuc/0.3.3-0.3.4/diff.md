# Comparing `tmp/pymemuc-0.3.3.tar.gz` & `tmp/pymemuc-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymemuc-0.3.3.tar", max compression
+gzip compressed data, was "pymemuc-0.3.4.tar", max compression
```

## Comparing `pymemuc-0.3.3.tar` & `pymemuc-0.3.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1057 2023-05-31 21:37:17.272523 pymemuc-0.3.3/LICENSE
--rw-r--r--   0        0        0     1586 2023-05-31 21:37:17.272523 pymemuc-0.3.3/README.md
--rw-r--r--   0        0        0      386 2023-05-31 21:37:17.272523 pymemuc-0.3.3/pymemuc/__init__.py
--rw-r--r--   0        0        0    22761 2023-05-31 21:37:17.272523 pymemuc-0.3.3/pymemuc/_command.py
--rw-r--r--   0        0        0      465 2023-05-31 21:37:17.272523 pymemuc-0.3.3/pymemuc/_constants.py
--rw-r--r--   0        0        0     4984 2023-05-31 21:37:17.272523 pymemuc-0.3.3/pymemuc/_control.py
--rw-r--r--   0        0        0     1214 2023-05-31 21:37:17.272523 pymemuc-0.3.3/pymemuc/_decorators.py
--rw-r--r--   0        0        0    13670 2023-05-31 21:37:17.276523 pymemuc-0.3.3/pymemuc/_manage.py
--rw-r--r--   0        0        0     4066 2023-05-31 21:37:17.276523 pymemuc-0.3.3/pymemuc/_memuc.py
--rw-r--r--   0        0        0      891 2023-05-31 21:37:17.276523 pymemuc-0.3.3/pymemuc/exceptions.py
--rw-r--r--   0        0        0     2899 2023-05-31 21:37:17.276523 pymemuc-0.3.3/pymemuc/pymemuc.py
--rw-r--r--   0        0        0      379 2023-05-31 21:37:17.276523 pymemuc-0.3.3/pymemuc/vminfo.py
--rw-r--r--   0        0        0     1665 2023-05-31 21:37:41.072504 pymemuc-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     2394 1970-01-01 00:00:00.000000 pymemuc-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1057 2023-06-06 18:09:50.890067 pymemuc-0.3.4/LICENSE
+-rw-r--r--   0        0        0     1586 2023-06-06 18:09:50.890067 pymemuc-0.3.4/README.md
+-rw-r--r--   0        0        0      386 2023-06-06 18:09:50.894067 pymemuc-0.3.4/pymemuc/__init__.py
+-rw-r--r--   0        0        0    22761 2023-06-06 18:09:50.894067 pymemuc-0.3.4/pymemuc/_command.py
+-rw-r--r--   0        0        0      465 2023-06-06 18:09:50.894067 pymemuc-0.3.4/pymemuc/_constants.py
+-rw-r--r--   0        0        0     4984 2023-06-06 18:09:50.894067 pymemuc-0.3.4/pymemuc/_control.py
+-rw-r--r--   0        0        0     1214 2023-06-06 18:09:50.894067 pymemuc-0.3.4/pymemuc/_decorators.py
+-rw-r--r--   0        0        0    13670 2023-06-06 18:09:50.894067 pymemuc-0.3.4/pymemuc/_manage.py
+-rw-r--r--   0        0        0     4096 2023-06-06 18:09:50.894067 pymemuc-0.3.4/pymemuc/_memuc.py
+-rw-r--r--   0        0        0      891 2023-06-06 18:09:50.894067 pymemuc-0.3.4/pymemuc/exceptions.py
+-rw-r--r--   0        0        0     2899 2023-06-06 18:09:50.894067 pymemuc-0.3.4/pymemuc/pymemuc.py
+-rw-r--r--   0        0        0      379 2023-06-06 18:09:50.894067 pymemuc-0.3.4/pymemuc/vminfo.py
+-rw-r--r--   0        0        0     1665 2023-06-06 18:10:10.714555 pymemuc-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     2394 1970-01-01 00:00:00.000000 pymemuc-0.3.4/PKG-INFO
```

### Comparing `pymemuc-0.3.3/LICENSE` & `pymemuc-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pymemuc-0.3.3/README.md` & `pymemuc-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `pymemuc-0.3.3/pymemuc/_command.py` & `pymemuc-0.3.4/pymemuc/_command.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.3.3/pymemuc/_control.py` & `pymemuc-0.3.4/pymemuc/_control.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.3.3/pymemuc/_decorators.py` & `pymemuc-0.3.4/pymemuc/_decorators.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.3.3/pymemuc/_manage.py` & `pymemuc-0.3.4/pymemuc/_manage.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.3.3/pymemuc/_memuc.py` & `pymemuc-0.3.4/pymemuc/_memuc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 """This module contains functions for directly interacting with memuc.exe."""
 from contextlib import suppress
 from os.path import join, normpath
-from subprocess import (
-    PIPE,
-    STARTUPINFO,
-    STDOUT,
-    CalledProcessError,
-    Popen,
-    TimeoutExpired,
-)
+from subprocess import PIPE, STDOUT, CalledProcessError, Popen, TimeoutExpired
 from typing import TYPE_CHECKING, Tuple
 
 from ._constants import WIN32, WINREG_EN
 from .exceptions import PyMemucError, PyMemucException, PyMemucTimeoutExpired
 
 if WINREG_EN:
     # pylint: disable=import-error
     from winreg import HKEY_LOCAL_MACHINE, ConnectRegistry, OpenKey, QueryValueEx
 
-ST_INFO = STARTUPINFO()
-
+ST_INFO = None
 if WIN32:
-    from subprocess import REALTIME_PRIORITY_CLASS, STARTF_USESHOWWINDOW, SW_HIDE
+    from subprocess import (
+        REALTIME_PRIORITY_CLASS,
+        STARTF_USESHOWWINDOW,
+        STARTUPINFO,
+        SW_HIDE,
+    )
 
+    ST_INFO = STARTUPINFO()
     ST_INFO.dwFlags |= STARTF_USESHOWWINDOW
     ST_INFO.dwFlags |= REALTIME_PRIORITY_CLASS
     ST_INFO.wShowWindow = SW_HIDE
 
 
 if TYPE_CHECKING:
     from pymemuc import PyMemuc
```

### Comparing `pymemuc-0.3.3/pymemuc/exceptions.py` & `pymemuc-0.3.4/pymemuc/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.3.3/pymemuc/pymemuc.py` & `pymemuc-0.3.4/pymemuc/pymemuc.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.3.3/pyproject.toml` & `pymemuc-0.3.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pymemuc"
-version = "v0.3.3"
+version = "v0.3.4"
 description = "A Memuc.exe wrapper for Python"
 readme = "README.md"
 authors = ["Martin Miglio <code@martinmiglio.dev>"]
 license = "MIT"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `pymemuc-0.3.3/PKG-INFO` & `pymemuc-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymemuc
-Version: 0.3.3
+Version: 0.3.4
 Summary: A Memuc.exe wrapper for Python
 Home-page: https://github.com/martinmiglio/pymemuc
 License: MIT
 Keywords: memu,memuc,wrapper,api
 Author: Martin Miglio
 Author-email: code@martinmiglio.dev
 Requires-Python: >=3.9,<4.0
```

