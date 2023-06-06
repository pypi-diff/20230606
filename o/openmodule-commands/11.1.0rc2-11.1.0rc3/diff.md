# Comparing `tmp/openmodule_commands-11.1.0rc2.tar.gz` & `tmp/openmodule_commands-11.1.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmodule_commands-11.1.0rc2.tar", last modified: Tue Jun  6 09:20:33 2023, max compression
+gzip compressed data, was "openmodule_commands-11.1.0rc3.tar", last modified: Tue Jun  6 12:04:18 2023, max compression
```

## Comparing `openmodule_commands-11.1.0rc2.tar` & `openmodule_commands-11.1.0rc3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:20:33.230326 openmodule_commands-11.1.0rc2/
--rw-r--r--   0 root         (0) root         (0)      302 2023-06-06 09:20:33.000000 openmodule_commands-11.1.0rc2/AUTHORS
--rw-r--r--   0 root         (0) root         (0)     6505 2023-06-06 09:20:33.000000 openmodule_commands-11.1.0rc2/ChangeLog
--rw-r--r--   0 root         (0) root         (0)      621 2023-06-06 09:20:33.230326 openmodule_commands-11.1.0rc2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2826 2023-06-06 09:20:20.000000 openmodule_commands-11.1.0rc2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 09:20:33.230326 openmodule_commands-11.1.0rc2/openmodule_commands.egg-info/
--rw-r--r--   0 root         (0) root         (0)      621 2023-06-06 09:20:33.000000 openmodule_commands-11.1.0rc2/openmodule_commands.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      363 2023-06-06 09:20:33.000000 openmodule_commands-11.1.0rc2/openmodule_commands.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 09:20:33.000000 openmodule_commands-11.1.0rc2/openmodule_commands.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      232 2023-06-06 09:20:33.000000 openmodule_commands-11.1.0rc2/openmodule_commands.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 09:20:33.000000 openmodule_commands-11.1.0rc2/openmodule_commands.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       46 2023-06-06 09:20:33.000000 openmodule_commands-11.1.0rc2/openmodule_commands.egg-info/pbr.json
--rw-r--r--   0 root         (0) root         (0)       20 2023-06-06 09:20:33.000000 openmodule_commands-11.1.0rc2/openmodule_commands.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      850 2023-06-06 09:20:33.231325 openmodule_commands-11.1.0rc2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      529 2023-06-06 09:20:20.000000 openmodule_commands-11.1.0rc2/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     8162 2023-06-06 09:20:20.000000 openmodule_commands-11.1.0rc2/translate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 12:04:18.247446 openmodule_commands-11.1.0rc3/
+-rw-r--r--   0 root         (0) root         (0)      302 2023-06-06 12:04:18.000000 openmodule_commands-11.1.0rc3/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)     6537 2023-06-06 12:04:18.000000 openmodule_commands-11.1.0rc3/ChangeLog
+-rw-r--r--   0 root         (0) root         (0)      621 2023-06-06 12:04:18.247446 openmodule_commands-11.1.0rc3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2826 2023-06-06 12:04:05.000000 openmodule_commands-11.1.0rc3/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 12:04:18.247446 openmodule_commands-11.1.0rc3/openmodule_commands.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      621 2023-06-06 12:04:18.000000 openmodule_commands-11.1.0rc3/openmodule_commands.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      363 2023-06-06 12:04:18.000000 openmodule_commands-11.1.0rc3/openmodule_commands.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 12:04:18.000000 openmodule_commands-11.1.0rc3/openmodule_commands.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      232 2023-06-06 12:04:18.000000 openmodule_commands-11.1.0rc3/openmodule_commands.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 12:04:18.000000 openmodule_commands-11.1.0rc3/openmodule_commands.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       46 2023-06-06 12:04:18.000000 openmodule_commands-11.1.0rc3/openmodule_commands.egg-info/pbr.json
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-06 12:04:18.000000 openmodule_commands-11.1.0rc3/openmodule_commands.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      850 2023-06-06 12:04:18.248446 openmodule_commands-11.1.0rc3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      529 2023-06-06 12:04:05.000000 openmodule_commands-11.1.0rc3/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     8162 2023-06-06 12:04:05.000000 openmodule_commands-11.1.0rc3/translate.py
```

### Comparing `openmodule_commands-11.1.0rc2/ChangeLog` & `openmodule_commands-11.1.0rc3/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGES
 =======
 
+v11.1.0.rc3
+-----------
+
+* changed docs and requirements for schedule library until its a pip package
+
 v11.1.0.rc2
 -----------
 
 * added fork of schedule package
 
 v11.1.0.rc1
 -----------
@@ -157,8 +162,7 @@
 * drop support for python 3.7
 * cleanup and docs
 * testcases for the new test method
 * better logging for rpc requests, and added a function to the test framework to receive rpc responses async
 * moved config yaml path guesser to separate function, removed GUID again because its not a great idea after all
 * reduced warnings in the testcases
 * GUID type and rpc server changes to better support all pydantic models, in this case Union Types. DEVICE-891
-* fixes an issue in rpc server logging, and adds more debug log output
```

### Comparing `openmodule_commands-11.1.0rc2/PKG-INFO` & `openmodule_commands-11.1.0rc3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmodule_commands
-Version: 11.1.0rc2
+Version: 11.1.0rc3
 Summary: Commands for openmodule services
 Home-page: https://gitlab.com/arivo-public/device-python/openmodule.git
 Author: ARIVO
 Author-email: support@arivo.co
 License: GNU General Public License v2 (GPLv2)
 Keywords: arivo openmodule openmodule_commands commands
 Platform: UNKNOWN
```

### Comparing `openmodule_commands-11.1.0rc2/__init__.py` & `openmodule_commands-11.1.0rc3/__init__.py`

 * *Files identical despite different names*

### Comparing `openmodule_commands-11.1.0rc2/openmodule_commands.egg-info/PKG-INFO` & `openmodule_commands-11.1.0rc3/openmodule_commands.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmodule-commands
-Version: 11.1.0rc2
+Version: 11.1.0rc3
 Summary: Commands for openmodule services
 Home-page: https://gitlab.com/arivo-public/device-python/openmodule.git
 Author: ARIVO
 Author-email: support@arivo.co
 License: GNU General Public License v2 (GPLv2)
 Keywords: arivo openmodule openmodule_commands commands
 Platform: UNKNOWN
```

### Comparing `openmodule_commands-11.1.0rc2/setup.cfg` & `openmodule_commands-11.1.0rc3/setup.cfg`

 * *Files identical despite different names*

### Comparing `openmodule_commands-11.1.0rc2/setup.py` & `openmodule_commands-11.1.0rc3/setup.py`

 * *Files identical despite different names*

### Comparing `openmodule_commands-11.1.0rc2/translate.py` & `openmodule_commands-11.1.0rc3/translate.py`

 * *Files identical despite different names*

