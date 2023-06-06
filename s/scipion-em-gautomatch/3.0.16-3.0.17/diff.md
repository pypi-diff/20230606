# Comparing `tmp/scipion-em-gautomatch-3.0.16.tar.gz` & `tmp/scipion-em-gautomatch-3.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-gautomatch-3.0.16.tar", last modified: Sun Aug 28 18:36:12 2022, max compression
+gzip compressed data, was "scipion-em-gautomatch-3.0.17.tar", last modified: Tue Jun  6 12:33:24 2023, max compression
```

## Comparing `scipion-em-gautomatch-3.0.16.tar` & `scipion-em-gautomatch-3.0.17.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 18:36:12.846934 scipion-em-gautomatch-3.0.16/
--rw-r--r--   0 runner    (1001) docker     (121)      714 2022-08-28 18:34:32.000000 scipion-em-gautomatch-3.0.16/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (121)    35147 2022-08-28 18:34:32.000000 scipion-em-gautomatch-3.0.16/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-08-28 18:34:32.000000 scipion-em-gautomatch-3.0.16/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4132 2022-08-28 18:36:12.846934 scipion-em-gautomatch-3.0.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2757 2022-08-28 18:34:32.000000 scipion-em-gautomatch-3.0.16/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 18:36:12.846934 scipion-em-gautomatch-3.0.16/gautomatch/
--rw-r--r--   0 runner    (1001) docker     (121)     3969 2022-08-28 18:34:32.000000 scipion-em-gautomatch-3.0.16/gautomatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1585 2022-08-28 18:34:32.000000 scipion-em-gautomatch-3.0.16/gautomatch/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (121)     1303 2022-08-28 18:34:32.000000 scipion-em-gautomatch-3.0.16/gautomatch/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    10193 2022-08-28 18:34:32.000000 scipion-em-gautomatch-3.0.16/gautomatch/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 18:36:12.846934 scipion-em-gautomatch-3.0.16/gautomatch/protocols/
--rw-r--r--   0 runner    (1001) docker     (121)     1173 2022-08-28 18:34:32.000000 scipion-em-gautomatch-3.0.16/gautomatch/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    29926 2022-08-28 18:34:32.000000 scipion-em-gautomatch-3.0.16/gautomatch/protocols/protocol_gautomatch.py
--rw-r--r--   0 runner    (1001) docker     (121)     5329 2022-08-28 18:34:32.000000 scipion-em-gautomatch-3.0.16/gautomatch/protocols.conf
--rwxr-xr-x   0 runner    (1001) docker     (121)     1463 2022-08-28 18:34:32.000000 scipion-em-gautomatch-3.0.16/gautomatch/run_gautomatch.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 18:36:12.846934 scipion-em-gautomatch-3.0.16/gautomatch/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-08-28 18:34:32.000000 scipion-em-gautomatch-3.0.16/gautomatch/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6609 2022-08-28 18:34:32.000000 scipion-em-gautomatch-3.0.16/gautomatch/tests/test_protocols_gautomatch.py
--rw-r--r--   0 runner    (1001) docker     (121)     7879 2022-08-28 18:34:32.000000 scipion-em-gautomatch-3.0.16/gautomatch/viewers.py
--rw-r--r--   0 runner    (1001) docker     (121)     8906 2022-08-28 18:34:32.000000 scipion-em-gautomatch-3.0.16/gautomatch/wizards.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-28 18:36:12.846934 scipion-em-gautomatch-3.0.16/scipion_em_gautomatch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4132 2022-08-28 18:36:12.000000 scipion-em-gautomatch-3.0.16/scipion_em_gautomatch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      664 2022-08-28 18:36:12.000000 scipion-em-gautomatch-3.0.16/scipion_em_gautomatch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-28 18:36:12.000000 scipion-em-gautomatch-3.0.16/scipion_em_gautomatch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-08-28 18:36:12.000000 scipion-em-gautomatch-3.0.16/scipion_em_gautomatch.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-08-28 18:36:12.000000 scipion-em-gautomatch-3.0.16/scipion_em_gautomatch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-08-28 18:36:12.000000 scipion-em-gautomatch-3.0.16/scipion_em_gautomatch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-28 18:36:12.846934 scipion-em-gautomatch-3.0.16/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     8534 2022-08-28 18:34:32.000000 scipion-em-gautomatch-3.0.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:33:24.354408 scipion-em-gautomatch-3.0.17/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-06 12:31:33.000000 scipion-em-gautomatch-3.0.17/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-06-06 12:31:33.000000 scipion-em-gautomatch-3.0.17/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-06 12:31:33.000000 scipion-em-gautomatch-3.0.17/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-06 12:33:24.354408 scipion-em-gautomatch-3.0.17/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-06-06 12:31:33.000000 scipion-em-gautomatch-3.0.17/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:33:24.354408 scipion-em-gautomatch-3.0.17/gautomatch/
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-06-06 12:31:33.000000 scipion-em-gautomatch-3.0.17/gautomatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-06 12:31:33.000000 scipion-em-gautomatch-3.0.17/gautomatch/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-06 12:31:33.000000 scipion-em-gautomatch-3.0.17/gautomatch/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10193 2023-06-06 12:31:33.000000 scipion-em-gautomatch-3.0.17/gautomatch/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:33:24.354408 scipion-em-gautomatch-3.0.17/gautomatch/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-06 12:31:33.000000 scipion-em-gautomatch-3.0.17/gautomatch/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29926 2023-06-06 12:31:33.000000 scipion-em-gautomatch-3.0.17/gautomatch/protocols/protocol_gautomatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-06-06 12:31:33.000000 scipion-em-gautomatch-3.0.17/gautomatch/protocols.conf
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1463 2023-06-06 12:31:33.000000 scipion-em-gautomatch-3.0.17/gautomatch/run_gautomatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:33:24.354408 scipion-em-gautomatch-3.0.17/gautomatch/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-06 12:31:33.000000 scipion-em-gautomatch-3.0.17/gautomatch/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6609 2023-06-06 12:31:33.000000 scipion-em-gautomatch-3.0.17/gautomatch/tests/test_protocols_gautomatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-06-06 12:31:33.000000 scipion-em-gautomatch-3.0.17/gautomatch/viewers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-06-06 12:31:33.000000 scipion-em-gautomatch-3.0.17/gautomatch/wizards.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 12:33:24.354408 scipion-em-gautomatch-3.0.17/scipion_em_gautomatch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-06 12:33:24.000000 scipion-em-gautomatch-3.0.17/scipion_em_gautomatch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-06 12:33:24.000000 scipion-em-gautomatch-3.0.17/scipion_em_gautomatch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 12:33:24.000000 scipion-em-gautomatch-3.0.17/scipion_em_gautomatch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-06 12:33:24.000000 scipion-em-gautomatch-3.0.17/scipion_em_gautomatch.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-06 12:33:24.000000 scipion-em-gautomatch-3.0.17/scipion_em_gautomatch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-06 12:33:24.000000 scipion-em-gautomatch-3.0.17/scipion_em_gautomatch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 12:33:24.354408 scipion-em-gautomatch-3.0.17/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8534 2023-06-06 12:31:33.000000 scipion-em-gautomatch-3.0.17/setup.py
```

### Comparing `scipion-em-gautomatch-3.0.16/CHANGES.txt` & `scipion-em-gautomatch-3.0.17/CHANGES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+3.0.17 - fix missing import
 3.0.16 - add possible outputs, use logging, allow pointers
 3.0.15 - minor changes
 3.0.14 - minor changes
 3.0.13:
     - better error handling
     - use abs link for tmp files
     - omit output box files
```

### Comparing `scipion-em-gautomatch-3.0.16/LICENSE` & `scipion-em-gautomatch-3.0.17/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-gautomatch-3.0.16/PKG-INFO` & `scipion-em-gautomatch-3.0.17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-gautomatch
-Version: 3.0.16
+Version: 3.0.17
 Summary: Plugin to use Gautomatch program within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-gautomatch
 Author: Grigory Sharov, J.M. De la Rosa Trevin
 Author-email: sharov.grigory@gmail.com, delarosatrevin@scilifelab.se
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-gautomatch/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-gautomatch/
```

### Comparing `scipion-em-gautomatch-3.0.16/README.rst` & `scipion-em-gautomatch-3.0.17/README.rst`

 * *Files identical despite different names*

### Comparing `scipion-em-gautomatch-3.0.16/gautomatch/__init__.py` & `scipion-em-gautomatch-3.0.17/gautomatch/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 import pwem
 import pyworkflow.utils as pwutils
 from pwem.emlib.image import ImageHandler
 
 from .constants import *
 
 
-__version__ = '3.0.16'
+__version__ = '3.0.17'
 _logo = "gautomatch_logo.png"
 _references = ['Zhang']
 
 
 class Plugin(pwem.Plugin):
     _homeVar = GAUTOMATCH_HOME
     _pathVars = [GAUTOMATCH_HOME]
```

### Comparing `scipion-em-gautomatch-3.0.16/gautomatch/bibtex.py` & `scipion-em-gautomatch-3.0.17/gautomatch/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-gautomatch-3.0.16/gautomatch/constants.py` & `scipion-em-gautomatch-3.0.17/gautomatch/constants.py`

 * *Files identical despite different names*

### Comparing `scipion-em-gautomatch-3.0.16/gautomatch/convert.py` & `scipion-em-gautomatch-3.0.17/gautomatch/convert.py`

 * *Files identical despite different names*

### Comparing `scipion-em-gautomatch-3.0.16/gautomatch/protocols/__init__.py` & `scipion-em-gautomatch-3.0.17/gautomatch/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-gautomatch-3.0.16/gautomatch/protocols/protocol_gautomatch.py` & `scipion-em-gautomatch-3.0.17/gautomatch/protocols/protocol_gautomatch.py`

 * *Files identical despite different names*

### Comparing `scipion-em-gautomatch-3.0.16/gautomatch/protocols.conf` & `scipion-em-gautomatch-3.0.17/gautomatch/protocols.conf`

 * *Files identical despite different names*

### Comparing `scipion-em-gautomatch-3.0.16/gautomatch/run_gautomatch.py` & `scipion-em-gautomatch-3.0.17/gautomatch/run_gautomatch.py`

 * *Files identical despite different names*

### Comparing `scipion-em-gautomatch-3.0.16/gautomatch/tests/test_protocols_gautomatch.py` & `scipion-em-gautomatch-3.0.17/gautomatch/tests/test_protocols_gautomatch.py`

 * *Files identical despite different names*

### Comparing `scipion-em-gautomatch-3.0.16/gautomatch/viewers.py` & `scipion-em-gautomatch-3.0.17/gautomatch/viewers.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 """
 
 from pwem.objects import SetOfCoordinates
 from pyworkflow.protocol.params import *
 from pyworkflow.viewer import ProtocolViewer, DESKTOP_TKINTER, WEB_DJANGO
 from pwem.viewers import ObjectView
 import pyworkflow.utils as pwutils
+import os
 
 from gautomatch.protocols import ProtGautomatch
 
 
 class GautomatchViewer(ProtocolViewer):
     """ Visualization of Gautomatch results. """
```

### Comparing `scipion-em-gautomatch-3.0.16/gautomatch/wizards.py` & `scipion-em-gautomatch-3.0.17/gautomatch/wizards.py`

 * *Files identical despite different names*

### Comparing `scipion-em-gautomatch-3.0.16/scipion_em_gautomatch.egg-info/PKG-INFO` & `scipion-em-gautomatch-3.0.17/scipion_em_gautomatch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-gautomatch
-Version: 3.0.16
+Version: 3.0.17
 Summary: Plugin to use Gautomatch program within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-gautomatch
 Author: Grigory Sharov, J.M. De la Rosa Trevin
 Author-email: sharov.grigory@gmail.com, delarosatrevin@scilifelab.se
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-gautomatch/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-gautomatch/
```

### Comparing `scipion-em-gautomatch-3.0.16/scipion_em_gautomatch.egg-info/SOURCES.txt` & `scipion-em-gautomatch-3.0.17/scipion_em_gautomatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-gautomatch-3.0.16/setup.py` & `scipion-em-gautomatch-3.0.17/setup.py`

 * *Files identical despite different names*

