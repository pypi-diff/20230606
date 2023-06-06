# Comparing `tmp/bluepy3-1.6.3.tar.gz` & `tmp/bluepy3-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bluepy3-1.6.3.tar", last modified: Sun Jun  4 09:14:23 2023, max compression
+gzip compressed data, was "bluepy3-1.6.4.tar", last modified: Tue Jun  6 06:52:01 2023, max compression
```

## Comparing `bluepy3-1.6.3.tar` & `bluepy3-1.6.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 maurice    (501) staff       (20)        0 2023-06-04 09:14:23.539191 bluepy3-1.6.3/
--rw-r--r--   0 maurice    (501) staff       (20)     1084 2023-04-29 09:30:37.000000 bluepy3-1.6.3/LICENSE
--rw-r--r--   0 maurice    (501) staff       (20)     5536 2023-06-04 09:14:23.539261 bluepy3-1.6.3/PKG-INFO
--rw-r--r--   0 maurice    (501) staff       (20)     3650 2023-06-04 07:33:33.000000 bluepy3-1.6.3/README.md
-drwxr-xr-x   0 maurice    (501) staff       (20)        0 2023-06-04 09:14:23.538346 bluepy3-1.6.3/bluepy3/
--rw-r--r--   0 maurice    (501) staff       (20)     1571 2023-04-29 09:30:37.000000 bluepy3-1.6.3/bluepy3/Makefile
--rwxr-xr-x   0 maurice    (501) staff       (20)      135 2023-04-29 09:30:37.000000 bluepy3-1.6.3/bluepy3/__init__.py
--rwxr-xr-x   0 maurice    (501) staff       (20)     4732 2023-06-04 08:43:19.000000 bluepy3-1.6.3/bluepy3/blescan.py
--rw-r--r--   0 maurice    (501) staff       (20)    58458 2023-04-29 09:30:37.000000 bluepy3-1.6.3/bluepy3/bluepy3-helper.c
--rwxr-xr-x   0 maurice    (501) staff       (20)    36910 2023-06-04 08:43:37.000000 bluepy3-1.6.3/bluepy3/btle.py
--rw-r--r--   0 maurice    (501) staff       (20)     4167 2023-04-29 09:30:37.000000 bluepy3-1.6.3/bluepy3/config.5.47.h
--rw-r--r--   0 maurice    (501) staff       (20)     4317 2023-04-29 09:30:37.000000 bluepy3-1.6.3/bluepy3/config.5.50.h
--rw-r--r--   0 maurice    (501) staff       (20)     4317 2023-04-29 09:30:37.000000 bluepy3-1.6.3/bluepy3/config.5.60.h
--rw-r--r--   0 maurice    (501) staff       (20)     4317 2023-04-29 09:30:37.000000 bluepy3-1.6.3/bluepy3/config.5.66.h
--rwxr-xr-x   0 maurice    (501) staff       (20)     9749 2023-06-04 08:43:19.000000 bluepy3-1.6.3/bluepy3/get_services.py
--rwxr-xr-x   0 maurice    (501) staff       (20)      690 2023-04-29 09:30:37.000000 bluepy3-1.6.3/bluepy3/scan_fuzz.py
--rwxr-xr-x   0 maurice    (501) staff       (20)      454 2023-04-29 09:30:37.000000 bluepy3-1.6.3/bluepy3/scanner.py
--rwxr-xr-x   0 maurice    (501) staff       (20)    16627 2023-06-04 08:43:19.000000 bluepy3-1.6.3/bluepy3/sensortag.py
--rwxr-xr-x   0 maurice    (501) staff       (20)    34902 2023-06-04 08:43:19.000000 bluepy3-1.6.3/bluepy3/thingy52.py
--rw-r--r--   0 maurice    (501) staff       (20)    37880 2023-04-29 09:30:37.000000 bluepy3-1.6.3/bluepy3/uuids.json
--rw-r--r--   0 maurice    (501) staff       (20)      125 2023-04-29 09:30:37.000000 bluepy3-1.6.3/bluepy3/version.h
-drwxr-xr-x   0 maurice    (501) staff       (20)        0 2023-06-04 09:14:23.539071 bluepy3-1.6.3/bluepy3.egg-info/
--rw-r--r--   0 maurice    (501) staff       (20)     5536 2023-06-04 09:14:23.000000 bluepy3-1.6.3/bluepy3.egg-info/PKG-INFO
--rw-r--r--   0 maurice    (501) staff       (20)      521 2023-06-04 09:14:23.000000 bluepy3-1.6.3/bluepy3.egg-info/SOURCES.txt
--rw-r--r--   0 maurice    (501) staff       (20)        1 2023-06-04 09:14:23.000000 bluepy3-1.6.3/bluepy3.egg-info/dependency_links.txt
--rw-r--r--   0 maurice    (501) staff       (20)      117 2023-06-04 09:14:23.000000 bluepy3-1.6.3/bluepy3.egg-info/entry_points.txt
--rw-r--r--   0 maurice    (501) staff       (20)        8 2023-06-04 09:14:23.000000 bluepy3-1.6.3/bluepy3.egg-info/top_level.txt
--rw-r--r--   0 maurice    (501) staff       (20)       94 2023-06-04 09:14:23.539488 bluepy3-1.6.3/setup.cfg
--rw-r--r--   0 maurice    (501) staff       (20)     3424 2023-06-04 09:14:02.000000 bluepy3-1.6.3/setup.py
+drwxr-xr-x   0 maurice    (501) staff       (20)        0 2023-06-06 06:52:01.678108 bluepy3-1.6.4/
+-rw-r--r--   0 maurice    (501) staff       (20)     1084 2023-04-29 09:30:37.000000 bluepy3-1.6.4/LICENSE
+-rw-r--r--   0 maurice    (501) staff       (20)     5536 2023-06-06 06:52:01.678196 bluepy3-1.6.4/PKG-INFO
+-rw-r--r--   0 maurice    (501) staff       (20)     3650 2023-06-04 07:33:33.000000 bluepy3-1.6.4/README.md
+drwxr-xr-x   0 maurice    (501) staff       (20)        0 2023-06-06 06:52:01.677207 bluepy3-1.6.4/bluepy3/
+-rw-r--r--   0 maurice    (501) staff       (20)     1571 2023-04-29 09:30:37.000000 bluepy3-1.6.4/bluepy3/Makefile
+-rwxr-xr-x   0 maurice    (501) staff       (20)      135 2023-04-29 09:30:37.000000 bluepy3-1.6.4/bluepy3/__init__.py
+-rwxr-xr-x   0 maurice    (501) staff       (20)     4732 2023-06-04 08:43:19.000000 bluepy3-1.6.4/bluepy3/blescan.py
+-rw-r--r--   0 maurice    (501) staff       (20)    58458 2023-04-29 09:30:37.000000 bluepy3-1.6.4/bluepy3/bluepy3-helper.c
+-rwxr-xr-x   0 maurice    (501) staff       (20)    36910 2023-06-04 08:43:37.000000 bluepy3-1.6.4/bluepy3/btle.py
+-rw-r--r--   0 maurice    (501) staff       (20)     4167 2023-04-29 09:30:37.000000 bluepy3-1.6.4/bluepy3/config.5.47.h
+-rw-r--r--   0 maurice    (501) staff       (20)     4317 2023-04-29 09:30:37.000000 bluepy3-1.6.4/bluepy3/config.5.50.h
+-rw-r--r--   0 maurice    (501) staff       (20)     4317 2023-04-29 09:30:37.000000 bluepy3-1.6.4/bluepy3/config.5.60.h
+-rw-r--r--   0 maurice    (501) staff       (20)     4317 2023-04-29 09:30:37.000000 bluepy3-1.6.4/bluepy3/config.5.66.h
+-rwxr-xr-x   0 maurice    (501) staff       (20)     9749 2023-06-04 08:43:19.000000 bluepy3-1.6.4/bluepy3/get_services.py
+-rwxr-xr-x   0 maurice    (501) staff       (20)      690 2023-04-29 09:30:37.000000 bluepy3-1.6.4/bluepy3/scan_fuzz.py
+-rwxr-xr-x   0 maurice    (501) staff       (20)      454 2023-04-29 09:30:37.000000 bluepy3-1.6.4/bluepy3/scanner.py
+-rwxr-xr-x   0 maurice    (501) staff       (20)    16627 2023-06-04 08:43:19.000000 bluepy3-1.6.4/bluepy3/sensortag.py
+-rwxr-xr-x   0 maurice    (501) staff       (20)    34902 2023-06-04 08:43:19.000000 bluepy3-1.6.4/bluepy3/thingy52.py
+-rw-r--r--   0 maurice    (501) staff       (20)    37880 2023-04-29 09:30:37.000000 bluepy3-1.6.4/bluepy3/uuids.json
+-rw-r--r--   0 maurice    (501) staff       (20)      125 2023-04-29 09:30:37.000000 bluepy3-1.6.4/bluepy3/version.h
+drwxr-xr-x   0 maurice    (501) staff       (20)        0 2023-06-06 06:52:01.677888 bluepy3-1.6.4/bluepy3.egg-info/
+-rw-r--r--   0 maurice    (501) staff       (20)     5536 2023-06-06 06:52:01.000000 bluepy3-1.6.4/bluepy3.egg-info/PKG-INFO
+-rw-r--r--   0 maurice    (501) staff       (20)      521 2023-06-06 06:52:01.000000 bluepy3-1.6.4/bluepy3.egg-info/SOURCES.txt
+-rw-r--r--   0 maurice    (501) staff       (20)        1 2023-06-06 06:52:01.000000 bluepy3-1.6.4/bluepy3.egg-info/dependency_links.txt
+-rw-r--r--   0 maurice    (501) staff       (20)      117 2023-06-06 06:52:01.000000 bluepy3-1.6.4/bluepy3.egg-info/entry_points.txt
+-rw-r--r--   0 maurice    (501) staff       (20)        8 2023-06-06 06:52:01.000000 bluepy3-1.6.4/bluepy3.egg-info/top_level.txt
+-rw-r--r--   0 maurice    (501) staff       (20)       94 2023-06-06 06:52:01.678428 bluepy3-1.6.4/setup.cfg
+-rw-r--r--   0 maurice    (501) staff       (20)     3467 2023-06-06 06:51:38.000000 bluepy3-1.6.4/setup.py
```

### Comparing `bluepy3-1.6.3/LICENSE` & `bluepy3-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.3/PKG-INFO` & `bluepy3-1.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluepy3
-Version: 1.6.3
+Version: 1.6.4
 Summary: Python module for interfacing with BLE devices through Bluez
 Home-page: https://github.com/Mausy5043/bluepy3
 Download-URL: https://github.com/Mausy5043/bluepy3
 Author: mausy5043
 Keywords: Bluetooth,Bluetooth Smart,BLE,Bluetooth Low Energy,Raspberry Pi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bluepy3-1.6.3/README.md` & `bluepy3-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.3/bluepy3/Makefile` & `bluepy3-1.6.4/bluepy3/Makefile`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.3/bluepy3/blescan.py` & `bluepy3-1.6.4/bluepy3/blescan.py`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.3/bluepy3/bluepy3-helper.c` & `bluepy3-1.6.4/bluepy3/bluepy3-helper.c`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.3/bluepy3/btle.py` & `bluepy3-1.6.4/bluepy3/btle.py`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.3/bluepy3/config.5.47.h` & `bluepy3-1.6.4/bluepy3/config.5.47.h`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.3/bluepy3/config.5.50.h` & `bluepy3-1.6.4/bluepy3/config.5.50.h`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.3/bluepy3/config.5.60.h` & `bluepy3-1.6.4/bluepy3/config.5.60.h`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.3/bluepy3/config.5.66.h` & `bluepy3-1.6.4/bluepy3/config.5.66.h`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.3/bluepy3/get_services.py` & `bluepy3-1.6.4/bluepy3/get_services.py`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.3/bluepy3/scan_fuzz.py` & `bluepy3-1.6.4/bluepy3/scan_fuzz.py`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.3/bluepy3/sensortag.py` & `bluepy3-1.6.4/bluepy3/sensortag.py`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.3/bluepy3/thingy52.py` & `bluepy3-1.6.4/bluepy3/thingy52.py`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.3/bluepy3/uuids.json` & `bluepy3-1.6.4/bluepy3/uuids.json`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.3/bluepy3.egg-info/PKG-INFO` & `bluepy3-1.6.4/bluepy3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bluepy3
-Version: 1.6.3
+Version: 1.6.4
 Summary: Python module for interfacing with BLE devices through Bluez
 Home-page: https://github.com/Mausy5043/bluepy3
 Download-URL: https://github.com/Mausy5043/bluepy3
 Author: mausy5043
 Keywords: Bluetooth,Bluetooth Smart,BLE,Bluetooth Low Energy,Raspberry Pi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bluepy3-1.6.3/bluepy3.egg-info/SOURCES.txt` & `bluepy3-1.6.4/bluepy3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bluepy3-1.6.3/setup.py` & `bluepy3-1.6.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,34 +4,34 @@
 import shlex
 import subprocess
 import sys
 
 from setuptools import setup
 from setuptools.command.build_py import build_py
 
-# VERSION = "1.5.1"   # latest version for testing
-VERSION = "1.6.3"  # latest version for production
+# VERSION = "1.7.1"  # latest version for testing
+VERSION = "1.6.4"  # latest version for production
 MAKEFILE = "bluepy3/Makefile"
 VERSION_FILE = "bluepy3/version.h"
 BLUEZ_VERSION = "(unknown)"
 
 
 def pre_install():
     """Do the custom compiling of the bluepy3-helper executable from the makefile"""
-    global BLUEZ_VERSION
+    global BLUEZ_VERSION  # noqa
     cmd = ""
     try:
         print("\n\n*** Executing pre-install ***\n")
         print(f"Working dir is {os.getcwd()}")
-        with open(MAKEFILE, "r") as makefile:
+        with open(MAKEFILE, "r", encoding="utf-8") as makefile:
             lines = makefile.readlines()
             for line in lines:
                 if line.startswith("BLUEZ_VERSION"):
                     BLUEZ_VERSION = line.split("=")[1].strip()
-        with open(VERSION_FILE, "w") as verfile:
+        with open(VERSION_FILE, "w", encoding="utf-8") as verfile:
             verfile.write(f'#define VERSION_STRING "{VERSION}-{BLUEZ_VERSION}"\n')
         for cmd in ["make -dC bluepy3 clean", "make -dC bluepy3 -j1"]:
             print(f"\nexecute {cmd}")
             msgs = subprocess.check_output(shlex.split(cmd), stderr=subprocess.STDOUT)  # noqa
         print("\n\n*** Finished pre-install ***\n\n")
     except subprocess.CalledProcessError as e:
         print("Failed to compile bluepy3-helper. Exiting install.")
```

