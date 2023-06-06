# Comparing `tmp/vsiew-2.2.0.tar.gz` & `tmp/vsiew-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsiew-2.2.0.tar", last modified: Mon Jun  5 20:46:33 2023, max compression
+gzip compressed data, was "vsiew-2.2.1.tar", last modified: Tue Jun  6 11:16:25 2023, max compression
```

## Comparing `vsiew-2.2.0.tar` & `vsiew-2.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:33.976798 vsiew-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-05 20:46:08.000000 vsiew-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-05 20:46:33.976798 vsiew-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-05 20:46:08.000000 vsiew-2.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 20:46:33.976798 vsiew-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-05 20:46:08.000000 vsiew-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:33.972798 vsiew-2.2.0/vsiew/
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-05 20:46:08.000000 vsiew-2.2.0/vsiew/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-05 20:46:08.000000 vsiew-2.2.0/vsiew/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-05 20:46:08.000000 vsiew-2.2.0/vsiew/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-06-05 20:46:08.000000 vsiew-2.2.0/vsiew/init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:46:33.976798 vsiew-2.2.0/vsiew.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-05 20:46:33.000000 vsiew-2.2.0/vsiew.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-05 20:46:33.000000 vsiew-2.2.0/vsiew.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 20:46:33.000000 vsiew-2.2.0/vsiew.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-05 20:46:33.000000 vsiew-2.2.0/vsiew.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-05 20:46:33.000000 vsiew-2.2.0/vsiew.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 20:46:33.000000 vsiew-2.2.0/vsiew.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:16:25.953033 vsiew-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-06 11:15:51.000000 vsiew-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-06 11:16:25.953033 vsiew-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-06 11:15:51.000000 vsiew-2.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 11:16:25.953033 vsiew-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-06 11:15:51.000000 vsiew-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:16:25.953033 vsiew-2.2.1/vsiew/
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-06 11:15:51.000000 vsiew-2.2.1/vsiew/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-06 11:15:51.000000 vsiew-2.2.1/vsiew/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-06 11:15:51.000000 vsiew-2.2.1/vsiew/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-06-06 11:15:51.000000 vsiew-2.2.1/vsiew/init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 11:16:25.953033 vsiew-2.2.1/vsiew.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-06 11:16:25.000000 vsiew-2.2.1/vsiew.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-06 11:16:25.000000 vsiew-2.2.1/vsiew.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 11:16:25.000000 vsiew-2.2.1/vsiew.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-06 11:16:25.000000 vsiew-2.2.1/vsiew.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-06 11:16:25.000000 vsiew-2.2.1/vsiew.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-06 11:16:25.000000 vsiew-2.2.1/vsiew.egg-info/top_level.txt
```

### Comparing `vsiew-2.2.0/LICENSE` & `vsiew-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vsiew-2.2.0/PKG-INFO` & `vsiew-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsiew
-Version: 2.2.0
+Version: 2.2.1
 Summary: VapourSynth packages from Irrational Encoding Wizardry
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
```

### Comparing `vsiew-2.2.0/setup.py` & `vsiew-2.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `vsiew-2.2.0/vsiew/__init__.py` & `vsiew-2.2.1/vsiew/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # flake8: noqa
 
-import sys
 import inspect
+import sys
+from pathlib import Path
 from typing import TYPE_CHECKING
 
 update_check = False
 
 
 if TYPE_CHECKING:
     __all__ = [
@@ -50,14 +51,16 @@
         'self' in t.f_locals and type(t.f_locals['self']).__name__ == 'EntryPoint'
         and t.f_locals['self'].value == 'vsiew:update_packages'
     ) or (
         'pkg_main_name' in t.f_locals and t.f_locals['pkg_main_name'] == 'vsiew.__main__'
     ):
         update_check = True
         break
+else:
+    update_check = len(sys.argv) > 0 and (Path(sys.executable).parent / 'Scripts') in Path(sys.argv[0]).parents
 
 
 if update_check:
     __all__.append('update_packages')
 
     # vsiew
     def update_packages() -> None:
```

### Comparing `vsiew-2.2.0/vsiew/init.py` & `vsiew-2.2.1/vsiew/init.py`

 * *Files identical despite different names*

### Comparing `vsiew-2.2.0/vsiew.egg-info/PKG-INFO` & `vsiew-2.2.1/vsiew.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsiew
-Version: 2.2.0
+Version: 2.2.1
 Summary: VapourSynth packages from Irrational Encoding Wizardry
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry
 Project-URL: Contact, https://discord.gg/qxTxVJGtst
```

