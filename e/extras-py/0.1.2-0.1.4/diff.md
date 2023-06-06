# Comparing `tmp/extras-py-0.1.2.tar.gz` & `tmp/extras-py-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extras-py-0.1.2.tar", max compression
+gzip compressed data, was "extras-py-0.1.4.tar", max compression
```

## Comparing `extras-py-0.1.2.tar` & `extras-py-0.1.4.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      813 2023-06-05 21:57:03.899668 extras-py-0.1.2/extras_py/__init__.py
--rw-r--r--   0        0        0      390 2023-06-05 21:57:08.387656 extras-py-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      592 2023-06-05 21:57:21.794008 extras-py-0.1.2/setup.py
--rw-r--r--   0        0        0      322 2023-06-05 21:57:21.794423 extras-py-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      813 2023-06-06 14:21:32.863850 extras-py-0.1.4/extras_py/__init__.py
+-rw-r--r--   0        0        0      390 2023-06-06 14:22:22.339782 extras-py-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      592 2023-06-06 14:22:39.864600 extras-py-0.1.4/setup.py
+-rw-r--r--   0        0        0      322 2023-06-06 14:22:39.864937 extras-py-0.1.4/PKG-INFO
```

### Comparing `extras-py-0.1.2/extras_py/__init__.py` & `extras-py-0.1.4/extras_py/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.1.2'
+__version__ = '0.1.4'
 
 import time,random
 from os import system,name
 import sys
 import os
 from time import sleep
 from colorama import Fore as F
```

### Comparing `extras-py-0.1.2/setup.py` & `extras-py-0.1.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['extras_py']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'extras-py',
-    'version': '0.1.2',
+    'version': '0.1.4',
     'description': 'Adding in simple things that are tedious to add in on your own, with one simple line you can unlock easiness.',
     'long_description': None,
     'author': 'SalladShooter',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

