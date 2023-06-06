# Comparing `tmp/extrapy-0.1.5.tar.gz` & `tmp/extrapy-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extrapy-0.1.5.tar", max compression
+gzip compressed data, was "extrapy-0.1.6.tar", max compression
```

## Comparing `extrapy-0.1.5.tar` & `extrapy-0.1.6.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      813 2023-06-06 14:34:36.874400 extrapy-0.1.5/extrapy/__init__.py
--rw-r--r--   0        0        0      388 2023-06-06 14:34:41.738390 extrapy-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      588 2023-06-06 14:34:54.937355 extrapy-0.1.5/setup.py
--rw-r--r--   0        0        0      320 2023-06-06 14:34:54.937645 extrapy-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      835 2023-06-06 14:38:05.209956 extrapy-0.1.6/extrapy/__init__.py
+-rw-r--r--   0        0        0      388 2023-06-06 14:38:09.913946 extrapy-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      588 2023-06-06 14:38:21.591526 extrapy-0.1.6/setup.py
+-rw-r--r--   0        0        0      320 2023-06-06 14:38:21.591854 extrapy-0.1.6/PKG-INFO
```

### Comparing `extrapy-0.1.5/extrapy/__init__.py` & `extrapy-0.1.6/extrapy/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-__version__ = '0.1.5'
+__version__ = '0.1.6'
 
 import time,random
 from os import system,name
 import sys
 import os
 from time import sleep
+import time
+import colorama
 from colorama import Fore as F
 from colorama import Style as S
 from os import system as syst
 from replit import db
 bright = S.BRIGHT
 normal = S.NORMAL
 blue = F.BLUE
@@ -35,9 +37,9 @@
     
 def write(words):
   for i in (F.WHITE + words):
     sys.stdout.write(i)
     sys.stdout.flush()
     sleep(.03)
     
-def wait(time):
-  time.sleep(time)
+def wait(t):
+  time.sleep(t)
```

### Comparing `extrapy-0.1.5/setup.py` & `extrapy-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['extrapy']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'extrapy',
-    'version': '0.1.5',
+    'version': '0.1.6',
     'description': 'Adding in simple things that are tedious to add in on your own, with one simple line you can unlock easiness.',
     'long_description': None,
     'author': 'SalladShooter',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

