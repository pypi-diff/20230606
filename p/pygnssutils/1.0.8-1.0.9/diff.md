# Comparing `tmp/pygnssutils-1.0.8.tar.gz` & `tmp/pygnssutils-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygnssutils-1.0.8.tar", last modified: Mon May  8 08:43:22 2023, max compression
+gzip compressed data, was "pygnssutils-1.0.9.tar", last modified: Tue May 23 15:08:19 2023, max compression
```

## Comparing `pygnssutils-1.0.8.tar` & `pygnssutils-1.0.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-08 08:43:22.555854 pygnssutils-1.0.8/
--rw-r--r--   0 steve      (501) staff       (20)     1613 2022-05-26 12:22:57.000000 pygnssutils-1.0.8/LICENSE
--rw-r--r--   0 steve      (501) staff       (20)       64 2022-05-26 12:22:57.000000 pygnssutils-1.0.8/MANIFEST.in
--rw-r--r--   0 steve      (501) staff       (20)    24113 2023-05-08 08:43:22.555703 pygnssutils-1.0.8/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)    21117 2023-03-23 11:19:25.000000 pygnssutils-1.0.8/README.md
--rw-r--r--   0 steve      (501) staff       (20)     2957 2023-05-08 08:36:54.000000 pygnssutils-1.0.8/pyproject.toml
--rw-r--r--   0 steve      (501) staff       (20)       38 2023-05-08 08:43:22.555898 pygnssutils-1.0.8/setup.cfg
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-08 08:43:22.551882 pygnssutils-1.0.8/src/
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-08 08:43:22.554160 pygnssutils-1.0.8/src/pygnssutils/
--rw-r--r--   0 steve      (501) staff       (20)      704 2023-04-25 08:36:15.000000 pygnssutils-1.0.8/src/pygnssutils/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)      161 2023-05-08 08:36:54.000000 pygnssutils-1.0.8/src/pygnssutils/_version.py
--rw-r--r--   0 steve      (501) staff       (20)      297 2023-03-23 22:14:27.000000 pygnssutils-1.0.8/src/pygnssutils/exceptions.py
--rw-r--r--   0 steve      (501) staff       (20)     1743 2023-05-08 08:36:54.000000 pygnssutils-1.0.8/src/pygnssutils/globals.py
--rw-r--r--   0 steve      (501) staff       (20)    26375 2023-05-08 08:36:54.000000 pygnssutils-1.0.8/src/pygnssutils/gnssdump.py
--rw-r--r--   0 steve      (501) staff       (20)    17785 2023-05-08 08:36:54.000000 pygnssutils-1.0.8/src/pygnssutils/gnssmqttclient.py
--rw-r--r--   0 steve      (501) staff       (20)    25271 2023-05-08 08:36:54.000000 pygnssutils-1.0.8/src/pygnssutils/gnssntripclient.py
--rw-r--r--   0 steve      (501) staff       (20)    14710 2023-05-08 08:36:54.000000 pygnssutils-1.0.8/src/pygnssutils/gnssserver.py
--rw-r--r--   0 steve      (501) staff       (20)     5440 2023-05-08 08:36:54.000000 pygnssutils-1.0.8/src/pygnssutils/helpers.py
--rw-r--r--   0 steve      (501) staff       (20)    13171 2023-05-08 08:36:54.000000 pygnssutils-1.0.8/src/pygnssutils/socket_server.py
--rw-r--r--   0 steve      (501) staff       (20)     8924 2023-04-25 08:36:15.000000 pygnssutils-1.0.8/src/pygnssutils/ubxload.py
--rw-r--r--   0 steve      (501) staff       (20)    10943 2023-04-25 08:36:15.000000 pygnssutils-1.0.8/src/pygnssutils/ubxsave.py
--rw-r--r--   0 steve      (501) staff       (20)     7008 2023-04-25 08:36:15.000000 pygnssutils-1.0.8/src/pygnssutils/ubxsetrate.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-08 08:43:22.554983 pygnssutils-1.0.8/src/pygnssutils.egg-info/
--rw-r--r--   0 steve      (501) staff       (20)    24113 2023-05-08 08:43:22.000000 pygnssutils-1.0.8/src/pygnssutils.egg-info/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)      755 2023-05-08 08:43:22.000000 pygnssutils-1.0.8/src/pygnssutils.egg-info/SOURCES.txt
--rw-r--r--   0 steve      (501) staff       (20)        1 2023-05-08 08:43:22.000000 pygnssutils-1.0.8/src/pygnssutils.egg-info/dependency_links.txt
--rw-r--r--   0 steve      (501) staff       (20)      307 2023-05-08 08:43:22.000000 pygnssutils-1.0.8/src/pygnssutils.egg-info/entry_points.txt
--rw-r--r--   0 steve      (501) staff       (20)      181 2023-05-08 08:43:22.000000 pygnssutils-1.0.8/src/pygnssutils.egg-info/requires.txt
--rw-r--r--   0 steve      (501) staff       (20)       12 2023-05-08 08:43:22.000000 pygnssutils-1.0.8/src/pygnssutils.egg-info/top_level.txt
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-08 08:43:22.555515 pygnssutils-1.0.8/tests/
--rw-r--r--   0 steve      (501) staff       (20)     9075 2023-04-25 08:36:15.000000 pygnssutils-1.0.8/tests/test_gnssdump.py
--rw-r--r--   0 steve      (501) staff       (20)    27167 2023-04-25 08:36:15.000000 pygnssutils-1.0.8/tests/test_sourcetable.py
--rw-r--r--   0 steve      (501) staff       (20)     5508 2023-05-08 08:36:54.000000 pygnssutils-1.0.8/tests/test_static.py
--rw-r--r--   0 steve      (501) staff       (20)     3492 2023-04-25 08:36:15.000000 pygnssutils-1.0.8/tests/test_stream.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-23 15:08:19.303458 pygnssutils-1.0.9/
+-rw-r--r--   0 steve      (501) staff       (20)     1613 2022-05-26 12:22:57.000000 pygnssutils-1.0.9/LICENSE
+-rw-r--r--   0 steve      (501) staff       (20)       64 2022-05-26 12:22:57.000000 pygnssutils-1.0.9/MANIFEST.in
+-rw-r--r--   0 steve      (501) staff       (20)    24113 2023-05-23 15:08:19.303303 pygnssutils-1.0.9/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)    21117 2023-03-23 11:19:25.000000 pygnssutils-1.0.9/README.md
+-rw-r--r--   0 steve      (501) staff       (20)     2957 2023-05-23 15:05:29.000000 pygnssutils-1.0.9/pyproject.toml
+-rw-r--r--   0 steve      (501) staff       (20)       38 2023-05-23 15:08:19.303497 pygnssutils-1.0.9/setup.cfg
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-23 15:08:19.299019 pygnssutils-1.0.9/src/
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-23 15:08:19.301834 pygnssutils-1.0.9/src/pygnssutils/
+-rw-r--r--   0 steve      (501) staff       (20)      704 2023-04-25 08:36:15.000000 pygnssutils-1.0.9/src/pygnssutils/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)      161 2023-05-23 15:05:29.000000 pygnssutils-1.0.9/src/pygnssutils/_version.py
+-rw-r--r--   0 steve      (501) staff       (20)      297 2023-03-23 22:14:27.000000 pygnssutils-1.0.9/src/pygnssutils/exceptions.py
+-rw-r--r--   0 steve      (501) staff       (20)     1743 2023-05-23 12:18:44.000000 pygnssutils-1.0.9/src/pygnssutils/globals.py
+-rw-r--r--   0 steve      (501) staff       (20)    26406 2023-05-23 15:05:29.000000 pygnssutils-1.0.9/src/pygnssutils/gnssdump.py
+-rw-r--r--   0 steve      (501) staff       (20)    17813 2023-05-23 15:05:29.000000 pygnssutils-1.0.9/src/pygnssutils/gnssmqttclient.py
+-rw-r--r--   0 steve      (501) staff       (20)    25299 2023-05-23 15:05:29.000000 pygnssutils-1.0.9/src/pygnssutils/gnssntripclient.py
+-rw-r--r--   0 steve      (501) staff       (20)    14741 2023-05-23 15:05:29.000000 pygnssutils-1.0.9/src/pygnssutils/gnssserver.py
+-rw-r--r--   0 steve      (501) staff       (20)     5440 2023-05-08 08:36:54.000000 pygnssutils-1.0.9/src/pygnssutils/helpers.py
+-rw-r--r--   0 steve      (501) staff       (20)    13171 2023-05-08 08:36:54.000000 pygnssutils-1.0.9/src/pygnssutils/socket_server.py
+-rw-r--r--   0 steve      (501) staff       (20)     8924 2023-04-25 08:36:15.000000 pygnssutils-1.0.9/src/pygnssutils/ubxload.py
+-rw-r--r--   0 steve      (501) staff       (20)    10943 2023-04-25 08:36:15.000000 pygnssutils-1.0.9/src/pygnssutils/ubxsave.py
+-rw-r--r--   0 steve      (501) staff       (20)     7008 2023-04-25 08:36:15.000000 pygnssutils-1.0.9/src/pygnssutils/ubxsetrate.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-23 15:08:19.302641 pygnssutils-1.0.9/src/pygnssutils.egg-info/
+-rw-r--r--   0 steve      (501) staff       (20)    24113 2023-05-23 15:08:19.000000 pygnssutils-1.0.9/src/pygnssutils.egg-info/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)      755 2023-05-23 15:08:19.000000 pygnssutils-1.0.9/src/pygnssutils.egg-info/SOURCES.txt
+-rw-r--r--   0 steve      (501) staff       (20)        1 2023-05-23 15:08:19.000000 pygnssutils-1.0.9/src/pygnssutils.egg-info/dependency_links.txt
+-rw-r--r--   0 steve      (501) staff       (20)      307 2023-05-23 15:08:19.000000 pygnssutils-1.0.9/src/pygnssutils.egg-info/entry_points.txt
+-rw-r--r--   0 steve      (501) staff       (20)      181 2023-05-23 15:08:19.000000 pygnssutils-1.0.9/src/pygnssutils.egg-info/requires.txt
+-rw-r--r--   0 steve      (501) staff       (20)       12 2023-05-23 15:08:19.000000 pygnssutils-1.0.9/src/pygnssutils.egg-info/top_level.txt
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-05-23 15:08:19.303108 pygnssutils-1.0.9/tests/
+-rw-r--r--   0 steve      (501) staff       (20)     9075 2023-04-25 08:36:15.000000 pygnssutils-1.0.9/tests/test_gnssdump.py
+-rw-r--r--   0 steve      (501) staff       (20)    27167 2023-04-25 08:36:15.000000 pygnssutils-1.0.9/tests/test_sourcetable.py
+-rw-r--r--   0 steve      (501) staff       (20)     5508 2023-05-08 08:36:54.000000 pygnssutils-1.0.9/tests/test_static.py
+-rw-r--r--   0 steve      (501) staff       (20)     3492 2023-04-25 08:36:15.000000 pygnssutils-1.0.9/tests/test_stream.py
```

### Comparing `pygnssutils-1.0.8/LICENSE` & `pygnssutils-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pygnssutils-1.0.8/PKG-INFO` & `pygnssutils-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygnssutils
-Version: 1.0.8
+Version: 1.0.9
 Summary: GNSS Command Line Utilities
 Author-email: semuadmin <semuadmin@semuconsulting.com>
 Maintainer-email: semuadmin <semuadmin@semuconsulting.com>
 License: BSD 3-Clause License ("BSD License 2.0", "Revised BSD License", "New BSD License", or "Modified BSD License")
         
         Copyright (c) 2020, SEMU Consulting
         All rights reserved.
```

### Comparing `pygnssutils-1.0.8/README.md` & `pygnssutils-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pygnssutils-1.0.8/pyproject.toml` & `pygnssutils-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 authors = [
     {name = "semuadmin", email = "semuadmin@semuconsulting.com"},
 ]
 maintainers = [
   {name = "semuadmin", email = "semuadmin@semuconsulting.com"}
 ]
 description = "GNSS Command Line Utilities"
-version = "1.0.8"
+version = "1.0.9"
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Operating System :: OS Independent",
     "Development Status :: 5 - Production/Stable",
     "Environment :: MacOS X",
```

### Comparing `pygnssutils-1.0.8/src/pygnssutils/__init__.py` & `pygnssutils-1.0.9/src/pygnssutils/__init__.py`

 * *Files identical despite different names*

### Comparing `pygnssutils-1.0.8/src/pygnssutils/globals.py` & `pygnssutils-1.0.9/src/pygnssutils/globals.py`

 * *Files identical despite different names*

### Comparing `pygnssutils-1.0.8/src/pygnssutils/gnssdump.py` & `pygnssutils-1.0.9/src/pygnssutils/gnssdump.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,14 +185,15 @@
             self._errcount = 0
             self._validargs = True
             self._loglines = 0
             self._output = None
             self._stopevent = False
             self._outputhandler = None
             self._errorhandler = None
+            self._logfile = ""
 
             # flag to signify beginning of JSON array
             self._jsontop = True
 
             self._setup_output_handlers(**kwargs)
 
         except (ParameterError, ValueError, TypeError) as err:
@@ -541,28 +542,28 @@
         :param int loglevel: log level for this message (0,1,2)
         """
 
         msg = f"{datetime.now()}: {message}"
         if self._verbosity >= loglevel:
             if self._logtofile:
                 self._cycle_log()
-                with open(self._logpath, "a", encoding="UTF-8") as log:
+                with open(self._logfile, "a", encoding="UTF-8") as log:
                     log.write(msg + "\n")
                     self._loglines += 1
             else:
                 print(msg)
 
     def _cycle_log(self):
         """
         Generate new timestamped logfile path.
         """
 
         if not self._loglines % LOGLIMIT:
             tim = datetime.now().strftime("%Y%m%d%H%M%S")
-            self._logpath = os.path.join(self._logpath, f"gnssdump-{tim}.log")
+            self._logfile = os.path.join(self._logpath, f"gnssdump-{tim}.log")
             self._loglines = 0
 
     def _do_json(self, parsed: object) -> str:
         """
         If outputting JSON for this protocol, each message
         in array is terminated by comma except the last
         [{msg1},{msg2},...,[lastmsg]]
```

### Comparing `pygnssutils-1.0.8/src/pygnssutils/gnssmqttclient.py` & `pygnssutils-1.0.9/src/pygnssutils/gnssmqttclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,14 +98,15 @@
         self._logtofile = int(kwargs.get("logtofile", 0))
         self._logpath = kwargs.get("logpath", ".")
         self._loglines = 0
         self._socket = None
         self._connected = False
         self._stopevent = Event()
         self._mqtt_thread = None
+        self._logfile = ""
 
     def __enter__(self):
         """
         Context manager enter routine.
         """
 
         return self
@@ -403,29 +404,29 @@
             message = f"{datetime.now()}: {str(message)}"
         else:
             message = str(message)
 
         if self._verbosity >= loglevel:
             if self._logtofile:
                 self._cycle_log()
-                with open(self._logpath, "a", encoding="UTF-8") as log:
+                with open(self._logfile, "a", encoding="UTF-8") as log:
                     log.write(message + "\n")
                     self._loglines += 1
             else:
                 print(message)
 
     def _cycle_log(self):
         """
         THREADED
         Generate new timestamped logfile path.
         """
 
         if not self._loglines % LOGLIMIT:
             tim = datetime.now().strftime("%Y%m%d%H%M%S")
-            self._logpath = path.join(self._logpath, f"gnssspartnclient-{tim}.log")
+            self._logfile = path.join(self._logpath, f"gnssspartnclient-{tim}.log")
             self._loglines = 0
 
 
 def main():
     """
     CLI Entry point.
```

### Comparing `pygnssutils-1.0.8/src/pygnssutils/gnssntripclient.py` & `pygnssutils-1.0.9/src/pygnssutils/gnssntripclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,14 +113,15 @@
             self._validargs = False
 
         self._socket = None
         self._connected = False
         self._stopevent = Event()
         self._ntrip_thread = None
         self._last_gga = datetime.fromordinal(1)
+        self._logfile = ""
 
     def __enter__(self):
         """
         Context manager enter routine.
         """
 
         return self
@@ -593,29 +594,29 @@
             message = f"{datetime.now()}: {str(message)}"
         else:
             message = str(message)
 
         if self._verbosity >= loglevel:
             if self._logtofile:
                 self._cycle_log()
-                with open(self._logpath, "a", encoding="UTF-8") as log:
+                with open(self._logfile, "a", encoding="UTF-8") as log:
                     log.write(message + "\n")
                     self._loglines += 1
             else:
                 print(message)
 
     def _cycle_log(self):
         """
         THREADED
         Generate new timestamped logfile path.
         """
 
         if not self._loglines % LOGLIMIT:
             tim = datetime.now().strftime("%Y%m%d%H%M%S")
-            self._logpath = os.path.join(self._logpath, f"gnssntripclient-{tim}.log")
+            self._logfile = os.path.join(self._logpath, f"gnssntripclient-{tim}.log")
             self._loglines = 0
 
 
 def main():
     """
     CLI Entry point.
```

### Comparing `pygnssutils-1.0.8/src/pygnssutils/gnssserver.py` & `pygnssutils-1.0.9/src/pygnssutils/gnssserver.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,14 +106,15 @@
             self._socket_server = None
             self._streamer = None
             self._in_thread = None
             self._out_thread = None
             self._clients = 0
             self._validargs = True
             self._logpath = ""
+            self._logfile = ""
             self._loglines = 0
 
         except ValueError as err:
             self._do_log(
                 f"Invalid input arguments {kwargs}\n{err}",
                 VERBOSITY_LOW,
             )
@@ -276,28 +277,28 @@
         :param int loglevel: log level for this message (0,1,2)
         """
 
         msg = f"{datetime.now()}: {message}"
         if self._kwargs["verbosity"] >= loglevel:
             if self._kwargs["logtofile"]:
                 self._cycle_log()
-                with open(self._logpath, "a", encoding="utf-8") as log:
+                with open(self._logfile, "a", encoding="utf-8") as log:
                     log.write(msg + "\n")
                     self._loglines += 1
             else:
                 print(msg)
 
     def _cycle_log(self):
         """
         Generate new timestamped logfile path.
         """
 
         if not self._loglines % LOGLIMIT:
             tim = datetime.now().strftime("%Y%m%d%H%M%S")
-            self._logpath = os.path.join(
+            self._logfile = os.path.join(
                 self._kwargs["logpath"], f"gnssserver-{tim}.log"
             )
             self._loglines = 0
 
 
 def main():
     """
```

### Comparing `pygnssutils-1.0.8/src/pygnssutils/helpers.py` & `pygnssutils-1.0.9/src/pygnssutils/helpers.py`

 * *Files identical despite different names*

### Comparing `pygnssutils-1.0.8/src/pygnssutils/socket_server.py` & `pygnssutils-1.0.9/src/pygnssutils/socket_server.py`

 * *Files identical despite different names*

### Comparing `pygnssutils-1.0.8/src/pygnssutils/ubxload.py` & `pygnssutils-1.0.9/src/pygnssutils/ubxload.py`

 * *Files identical despite different names*

### Comparing `pygnssutils-1.0.8/src/pygnssutils/ubxsave.py` & `pygnssutils-1.0.9/src/pygnssutils/ubxsave.py`

 * *Files identical despite different names*

### Comparing `pygnssutils-1.0.8/src/pygnssutils/ubxsetrate.py` & `pygnssutils-1.0.9/src/pygnssutils/ubxsetrate.py`

 * *Files identical despite different names*

### Comparing `pygnssutils-1.0.8/src/pygnssutils.egg-info/PKG-INFO` & `pygnssutils-1.0.9/src/pygnssutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygnssutils
-Version: 1.0.8
+Version: 1.0.9
 Summary: GNSS Command Line Utilities
 Author-email: semuadmin <semuadmin@semuconsulting.com>
 Maintainer-email: semuadmin <semuadmin@semuconsulting.com>
 License: BSD 3-Clause License ("BSD License 2.0", "Revised BSD License", "New BSD License", or "Modified BSD License")
         
         Copyright (c) 2020, SEMU Consulting
         All rights reserved.
```

### Comparing `pygnssutils-1.0.8/src/pygnssutils.egg-info/SOURCES.txt` & `pygnssutils-1.0.9/src/pygnssutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygnssutils-1.0.8/tests/test_gnssdump.py` & `pygnssutils-1.0.9/tests/test_gnssdump.py`

 * *Files identical despite different names*

### Comparing `pygnssutils-1.0.8/tests/test_sourcetable.py` & `pygnssutils-1.0.9/tests/test_sourcetable.py`

 * *Files identical despite different names*

### Comparing `pygnssutils-1.0.8/tests/test_static.py` & `pygnssutils-1.0.9/tests/test_static.py`

 * *Files identical despite different names*

### Comparing `pygnssutils-1.0.8/tests/test_stream.py` & `pygnssutils-1.0.9/tests/test_stream.py`

 * *Files identical despite different names*

