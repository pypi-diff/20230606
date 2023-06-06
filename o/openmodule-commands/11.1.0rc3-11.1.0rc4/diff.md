# Comparing `tmp/openmodule_commands-11.1.0rc3.tar.gz` & `tmp/openmodule_commands-11.1.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmodule_commands-11.1.0rc3.tar", last modified: Tue Jun  6 12:04:18 2023, max compression
+gzip compressed data, was "openmodule_commands-11.1.0rc4.tar", last modified: Tue Jun  6 13:05:01 2023, max compression
```

## Comparing `openmodule_commands-11.1.0rc3.tar` & `openmodule_commands-11.1.0rc4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 12:04:18.247446 openmodule_commands-11.1.0rc3/
--rw-r--r--   0 root         (0) root         (0)      302 2023-06-06 12:04:18.000000 openmodule_commands-11.1.0rc3/AUTHORS
--rw-r--r--   0 root         (0) root         (0)     6537 2023-06-06 12:04:18.000000 openmodule_commands-11.1.0rc3/ChangeLog
--rw-r--r--   0 root         (0) root         (0)      621 2023-06-06 12:04:18.247446 openmodule_commands-11.1.0rc3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2826 2023-06-06 12:04:05.000000 openmodule_commands-11.1.0rc3/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 12:04:18.247446 openmodule_commands-11.1.0rc3/openmodule_commands.egg-info/
--rw-r--r--   0 root         (0) root         (0)      621 2023-06-06 12:04:18.000000 openmodule_commands-11.1.0rc3/openmodule_commands.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      363 2023-06-06 12:04:18.000000 openmodule_commands-11.1.0rc3/openmodule_commands.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 12:04:18.000000 openmodule_commands-11.1.0rc3/openmodule_commands.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      232 2023-06-06 12:04:18.000000 openmodule_commands-11.1.0rc3/openmodule_commands.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 12:04:18.000000 openmodule_commands-11.1.0rc3/openmodule_commands.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       46 2023-06-06 12:04:18.000000 openmodule_commands-11.1.0rc3/openmodule_commands.egg-info/pbr.json
--rw-r--r--   0 root         (0) root         (0)       20 2023-06-06 12:04:18.000000 openmodule_commands-11.1.0rc3/openmodule_commands.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      850 2023-06-06 12:04:18.248446 openmodule_commands-11.1.0rc3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      529 2023-06-06 12:04:05.000000 openmodule_commands-11.1.0rc3/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     8162 2023-06-06 12:04:05.000000 openmodule_commands-11.1.0rc3/translate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 13:05:01.503665 openmodule_commands-11.1.0rc4/
+-rw-r--r--   0 root         (0) root         (0)      302 2023-06-06 13:05:01.000000 openmodule_commands-11.1.0rc4/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)     6035 2023-06-06 13:05:01.000000 openmodule_commands-11.1.0rc4/ChangeLog
+-rw-r--r--   0 root         (0) root         (0)      621 2023-06-06 13:05:01.503665 openmodule_commands-11.1.0rc4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2826 2023-06-06 13:04:48.000000 openmodule_commands-11.1.0rc4/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 13:05:01.503665 openmodule_commands-11.1.0rc4/openmodule_commands.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      621 2023-06-06 13:05:01.000000 openmodule_commands-11.1.0rc4/openmodule_commands.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      363 2023-06-06 13:05:01.000000 openmodule_commands-11.1.0rc4/openmodule_commands.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 13:05:01.000000 openmodule_commands-11.1.0rc4/openmodule_commands.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      232 2023-06-06 13:05:01.000000 openmodule_commands-11.1.0rc4/openmodule_commands.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 13:05:01.000000 openmodule_commands-11.1.0rc4/openmodule_commands.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       46 2023-06-06 13:05:01.000000 openmodule_commands-11.1.0rc4/openmodule_commands.egg-info/pbr.json
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-06 13:05:01.000000 openmodule_commands-11.1.0rc4/openmodule_commands.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      850 2023-06-06 13:05:01.503665 openmodule_commands-11.1.0rc4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      529 2023-06-06 13:04:48.000000 openmodule_commands-11.1.0rc4/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     8162 2023-06-06 13:04:48.000000 openmodule_commands-11.1.0rc4/translate.py
```

### Comparing `openmodule_commands-11.1.0rc3/ChangeLog` & `openmodule_commands-11.1.0rc4/ChangeLog`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 CHANGES
 =======
 
+v11.1.0.rc4
+-----------
+
+* arivo-schedule in public pip
+* use temporary arivo-schedule package
+
 v11.1.0.rc3
 -----------
 
 * changed docs and requirements for schedule library until its a pip package
 
 v11.1.0.rc2
 -----------
@@ -143,16 +149,14 @@
 * do not write default Legacy-0 matching scheme to disk if not existing but use StringIO instead
 * Fixed get\_gateway\_states returning an empty IoState if the given Gateway was offline for 5 seconds. Added method descriptions to all callable IoListener methods
 * Added last\_timestamp to IoState. Renamed get\_state in IoListener to get\_io\_state. it now returns an IoState with all values 0. Added is\_pin\_valid, get\_gateway\_states and is\_gateway\_valid to IoListener. Added testcases for changes/new additions
 * Added Test case for SigTERM signal
 * Added a SigTERM interrupt handler, that simply raises a KeyboardInterrupt(). The handler is set in init\_openmodule and can be told not to start by setting catch\_sigterm=False at method call. The two arguments the signal hanlder receives (signal number, frame stack) are ignored (using \*\_)
 * added raise\_handler\_errors bool to IoListener for listener.handler exceptions moved message = message.dict() to just before listener calls
 * Added OpenModuleModel as inheritance to IoState and moved it to models/io.py
-* Added a gateway filter test
-* Moved IoListener from io-modbus to openmodule. Added the IoMessage model to models. (only IoMessage and nothing else) Changed IoListener to require registering listeners using add\_listener\_edge\_\* IoListener still collects all pin states. listeners are handled like dispatcher listeners. Changed IoListener tests to work with the changes. Simplified IoSimulator and added a generate\_example\_states for ease of use
 
 v8.0.1
 ------
 
 * fixed loading empty yamls fixes rpc server not logging info in debug log
 
 v8.0.0
@@ -160,9 +164,7 @@
 
 * fix in ci job
 * drop support for python 3.7
 * cleanup and docs
 * testcases for the new test method
 * better logging for rpc requests, and added a function to the test framework to receive rpc responses async
 * moved config yaml path guesser to separate function, removed GUID again because its not a great idea after all
-* reduced warnings in the testcases
-* GUID type and rpc server changes to better support all pydantic models, in this case Union Types. DEVICE-891
```

### Comparing `openmodule_commands-11.1.0rc3/PKG-INFO` & `openmodule_commands-11.1.0rc4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmodule_commands
-Version: 11.1.0rc3
+Version: 11.1.0rc4
 Summary: Commands for openmodule services
 Home-page: https://gitlab.com/arivo-public/device-python/openmodule.git
 Author: ARIVO
 Author-email: support@arivo.co
 License: GNU General Public License v2 (GPLv2)
 Keywords: arivo openmodule openmodule_commands commands
 Platform: UNKNOWN
```

### Comparing `openmodule_commands-11.1.0rc3/__init__.py` & `openmodule_commands-11.1.0rc4/__init__.py`

 * *Files identical despite different names*

### Comparing `openmodule_commands-11.1.0rc3/openmodule_commands.egg-info/PKG-INFO` & `openmodule_commands-11.1.0rc4/openmodule_commands.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmodule-commands
-Version: 11.1.0rc3
+Version: 11.1.0rc4
 Summary: Commands for openmodule services
 Home-page: https://gitlab.com/arivo-public/device-python/openmodule.git
 Author: ARIVO
 Author-email: support@arivo.co
 License: GNU General Public License v2 (GPLv2)
 Keywords: arivo openmodule openmodule_commands commands
 Platform: UNKNOWN
```

### Comparing `openmodule_commands-11.1.0rc3/setup.cfg` & `openmodule_commands-11.1.0rc4/setup.cfg`

 * *Files identical despite different names*

### Comparing `openmodule_commands-11.1.0rc3/setup.py` & `openmodule_commands-11.1.0rc4/setup.py`

 * *Files identical despite different names*

### Comparing `openmodule_commands-11.1.0rc3/translate.py` & `openmodule_commands-11.1.0rc4/translate.py`

 * *Files identical despite different names*

