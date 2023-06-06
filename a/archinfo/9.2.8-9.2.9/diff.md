# Comparing `tmp/archinfo-9.2.8.tar.gz` & `tmp/archinfo-9.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archinfo-9.2.8.tar", last modified: Tue Jun 28 17:02:03 2022, max compression
+gzip compressed data, was "archinfo-9.2.9.tar", last modified: Tue Jul  5 17:02:00 2022, max compression
```

## Comparing `archinfo-9.2.8.tar` & `archinfo-9.2.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:02:03.189423 archinfo-9.2.8/
--rw-r--r--   0 vsts      (1001) docker     (121)     1327 2022-06-28 17:01:14.000000 archinfo-9.2.8/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (121)       34 2022-06-28 17:01:14.000000 archinfo-9.2.8/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (121)      590 2022-06-28 17:02:03.189423 archinfo-9.2.8/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)      155 2022-06-28 17:01:14.000000 archinfo-9.2.8/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:02:03.189423 archinfo-9.2.8/archinfo/
--rw-r--r--   0 vsts      (1001) docker     (121)     1328 2022-06-28 17:01:35.000000 archinfo-9.2.8/archinfo/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)    34075 2022-06-28 17:01:14.000000 archinfo-9.2.8/archinfo/arch.py
--rw-r--r--   0 vsts      (1001) docker     (121)    18188 2022-06-28 17:01:14.000000 archinfo-9.2.8/archinfo/arch_aarch64.py
--rw-r--r--   0 vsts      (1001) docker     (121)    19092 2022-06-28 17:01:14.000000 archinfo-9.2.8/archinfo/arch_amd64.py
--rw-r--r--   0 vsts      (1001) docker     (121)    26283 2022-06-28 17:01:14.000000 archinfo-9.2.8/archinfo/arch_arm.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5974 2022-06-28 17:01:14.000000 archinfo-9.2.8/archinfo/arch_avr.py
--rw-r--r--   0 vsts      (1001) docker     (121)    12171 2022-06-28 17:01:14.000000 archinfo-9.2.8/archinfo/arch_mips32.py
--rw-r--r--   0 vsts      (1001) docker     (121)     9816 2022-06-28 17:01:14.000000 archinfo-9.2.8/archinfo/arch_mips64.py
--rw-r--r--   0 vsts      (1001) docker     (121)    15484 2022-06-28 17:01:14.000000 archinfo-9.2.8/archinfo/arch_ppc32.py
--rw-r--r--   0 vsts      (1001) docker     (121)    17014 2022-06-28 17:01:14.000000 archinfo-9.2.8/archinfo/arch_ppc64.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8537 2022-06-28 17:01:14.000000 archinfo-9.2.8/archinfo/arch_s390x.py
--rw-r--r--   0 vsts      (1001) docker     (121)    12037 2022-06-28 17:01:14.000000 archinfo-9.2.8/archinfo/arch_soot.py
--rw-r--r--   0 vsts      (1001) docker     (121)    12238 2022-06-28 17:01:14.000000 archinfo-9.2.8/archinfo/arch_x86.py
--rw-r--r--   0 vsts      (1001) docker     (121)       37 2022-06-28 17:01:14.000000 archinfo-9.2.8/archinfo/archerror.py
--rw-r--r--   0 vsts      (1001) docker     (121)   110051 2022-06-28 17:01:14.000000 archinfo-9.2.8/archinfo/defines.py
--rw-r--r--   0 vsts      (1001) docker     (121)        8 2022-06-28 17:01:14.000000 archinfo-9.2.8/archinfo/py.typed
--rw-r--r--   0 vsts      (1001) docker     (121)      999 2022-06-28 17:01:14.000000 archinfo-9.2.8/archinfo/tls.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-28 17:02:03.189423 archinfo-9.2.8/archinfo.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (121)      590 2022-06-28 17:02:02.000000 archinfo-9.2.8/archinfo.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)      546 2022-06-28 17:02:03.000000 archinfo-9.2.8/archinfo.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-06-28 17:02:02.000000 archinfo-9.2.8/archinfo.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        9 2022-06-28 17:02:03.000000 archinfo-9.2.8/archinfo.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       81 2022-06-28 17:01:35.000000 archinfo-9.2.8/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (121)      584 2022-06-28 17:02:03.189423 archinfo-9.2.8/setup.cfg
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:02:00.333090 archinfo-9.2.9/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1327 2022-07-05 17:01:12.000000 archinfo-9.2.9/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (121)       34 2022-07-05 17:01:12.000000 archinfo-9.2.9/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (121)      590 2022-07-05 17:02:00.333090 archinfo-9.2.9/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)      155 2022-07-05 17:01:12.000000 archinfo-9.2.9/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:02:00.333090 archinfo-9.2.9/archinfo/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1328 2022-07-05 17:01:34.000000 archinfo-9.2.9/archinfo/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    34075 2022-07-05 17:01:12.000000 archinfo-9.2.9/archinfo/arch.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    18188 2022-07-05 17:01:12.000000 archinfo-9.2.9/archinfo/arch_aarch64.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    19092 2022-07-05 17:01:12.000000 archinfo-9.2.9/archinfo/arch_amd64.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    26283 2022-07-05 17:01:12.000000 archinfo-9.2.9/archinfo/arch_arm.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5974 2022-07-05 17:01:12.000000 archinfo-9.2.9/archinfo/arch_avr.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    12171 2022-07-05 17:01:12.000000 archinfo-9.2.9/archinfo/arch_mips32.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     9816 2022-07-05 17:01:12.000000 archinfo-9.2.9/archinfo/arch_mips64.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    15484 2022-07-05 17:01:12.000000 archinfo-9.2.9/archinfo/arch_ppc32.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    17014 2022-07-05 17:01:12.000000 archinfo-9.2.9/archinfo/arch_ppc64.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     8537 2022-07-05 17:01:12.000000 archinfo-9.2.9/archinfo/arch_s390x.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    12037 2022-07-05 17:01:12.000000 archinfo-9.2.9/archinfo/arch_soot.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    12238 2022-07-05 17:01:12.000000 archinfo-9.2.9/archinfo/arch_x86.py
+-rw-r--r--   0 vsts      (1001) docker     (121)       37 2022-07-05 17:01:12.000000 archinfo-9.2.9/archinfo/archerror.py
+-rw-r--r--   0 vsts      (1001) docker     (121)   110051 2022-07-05 17:01:12.000000 archinfo-9.2.9/archinfo/defines.py
+-rw-r--r--   0 vsts      (1001) docker     (121)        8 2022-07-05 17:01:12.000000 archinfo-9.2.9/archinfo/py.typed
+-rw-r--r--   0 vsts      (1001) docker     (121)      999 2022-07-05 17:01:12.000000 archinfo-9.2.9/archinfo/tls.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-07-05 17:02:00.333090 archinfo-9.2.9/archinfo.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (121)      590 2022-07-05 17:02:00.000000 archinfo-9.2.9/archinfo.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)      546 2022-07-05 17:02:00.000000 archinfo-9.2.9/archinfo.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-07-05 17:02:00.000000 archinfo-9.2.9/archinfo.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        9 2022-07-05 17:02:00.000000 archinfo-9.2.9/archinfo.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)       81 2022-07-05 17:01:34.000000 archinfo-9.2.9/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (121)      584 2022-07-05 17:02:00.333090 archinfo-9.2.9/setup.cfg
```

### Comparing `archinfo-9.2.8/LICENSE` & `archinfo-9.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `archinfo-9.2.8/PKG-INFO` & `archinfo-9.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archinfo
-Version: 9.2.8
+Version: 9.2.9
 Summary: Classes with architecture-specific information useful to other projects.
 Home-page: https://github.com/angr/archinfo
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.8
```

### Comparing `archinfo-9.2.8/archinfo/__init__.py` & `archinfo-9.2.9/archinfo/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 archinfo is a collection of classes that contain architecture-specific information.
 It is useful for cross-architecture tools (such as pyvex).
 """
 
-__version__ = "9.2.8"
+__version__ = "9.2.9"
 
 if bytes is str:
     raise Exception("This module is designed for python 3 only. Please install an older version to use python 2.")
 
 # NewType Declaration, see https://docs.python.org/3/library/typing.html#newtype
 from typing import NewType
 RegisterOffset = NewType('RegisterOffset', int)
```

### Comparing `archinfo-9.2.8/archinfo/arch.py` & `archinfo-9.2.9/archinfo/arch.py`

 * *Files identical despite different names*

### Comparing `archinfo-9.2.8/archinfo/arch_aarch64.py` & `archinfo-9.2.9/archinfo/arch_aarch64.py`

 * *Files identical despite different names*

### Comparing `archinfo-9.2.8/archinfo/arch_amd64.py` & `archinfo-9.2.9/archinfo/arch_amd64.py`

 * *Files identical despite different names*

### Comparing `archinfo-9.2.8/archinfo/arch_arm.py` & `archinfo-9.2.9/archinfo/arch_arm.py`

 * *Files identical despite different names*

### Comparing `archinfo-9.2.8/archinfo/arch_avr.py` & `archinfo-9.2.9/archinfo/arch_avr.py`

 * *Files identical despite different names*

### Comparing `archinfo-9.2.8/archinfo/arch_mips32.py` & `archinfo-9.2.9/archinfo/arch_mips32.py`

 * *Files identical despite different names*

### Comparing `archinfo-9.2.8/archinfo/arch_mips64.py` & `archinfo-9.2.9/archinfo/arch_mips64.py`

 * *Files identical despite different names*

### Comparing `archinfo-9.2.8/archinfo/arch_ppc32.py` & `archinfo-9.2.9/archinfo/arch_ppc32.py`

 * *Files identical despite different names*

### Comparing `archinfo-9.2.8/archinfo/arch_ppc64.py` & `archinfo-9.2.9/archinfo/arch_ppc64.py`

 * *Files identical despite different names*

### Comparing `archinfo-9.2.8/archinfo/arch_s390x.py` & `archinfo-9.2.9/archinfo/arch_s390x.py`

 * *Files identical despite different names*

### Comparing `archinfo-9.2.8/archinfo/arch_soot.py` & `archinfo-9.2.9/archinfo/arch_soot.py`

 * *Files identical despite different names*

### Comparing `archinfo-9.2.8/archinfo/arch_x86.py` & `archinfo-9.2.9/archinfo/arch_x86.py`

 * *Files identical despite different names*

### Comparing `archinfo-9.2.8/archinfo/defines.py` & `archinfo-9.2.9/archinfo/defines.py`

 * *Files identical despite different names*

### Comparing `archinfo-9.2.8/archinfo/tls.py` & `archinfo-9.2.9/archinfo/tls.py`

 * *Files identical despite different names*

### Comparing `archinfo-9.2.8/archinfo.egg-info/PKG-INFO` & `archinfo-9.2.9/archinfo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archinfo
-Version: 9.2.8
+Version: 9.2.9
 Summary: Classes with architecture-specific information useful to other projects.
 Home-page: https://github.com/angr/archinfo
 License: BSD 2 Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.8
```

### Comparing `archinfo-9.2.8/archinfo.egg-info/SOURCES.txt` & `archinfo-9.2.9/archinfo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `archinfo-9.2.8/setup.cfg` & `archinfo-9.2.9/setup.cfg`

 * *Files identical despite different names*

