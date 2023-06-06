# Comparing `tmp/magicpy-0.1.3.1.tar.gz` & `tmp/magicpy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/magicpy-0.1.3.1.tar", last modified: Tue Sep  6 12:25:39 2022, max compression
+gzip compressed data, was "dist/magicpy-0.1.4.tar", last modified: Tue Jun  6 12:00:38 2023, max compression
```

## Comparing `magicpy-0.1.3.1.tar` & `magicpy-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-06 12:25:39.000000 magicpy-0.1.3.1/
--rwxrwxrwx   0 root         (0) root         (0)    32473 2022-09-06 12:25:29.000000 magicpy-0.1.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5935 2022-09-06 12:25:39.000000 magicpy-0.1.3.1/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     4982 2022-09-06 12:25:29.000000 magicpy-0.1.3.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-06 12:25:39.000000 magicpy-0.1.3.1/magicpy/
--rwxrwxrwx   0 root         (0) root         (0)      106 2022-09-06 12:25:29.000000 magicpy-0.1.3.1/magicpy/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    64520 2022-09-06 12:25:29.000000 magicpy-0.1.3.1/magicpy/magicpy.py
--rwxrwxrwx   0 root         (0) root         (0)     1336 2022-09-06 12:25:29.000000 magicpy-0.1.3.1/magicpy/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-06 12:25:39.000000 magicpy-0.1.3.1/magicpy.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5935 2022-09-06 12:25:39.000000 magicpy-0.1.3.1/magicpy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      236 2022-09-06 12:25:39.000000 magicpy-0.1.3.1/magicpy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-06 12:25:39.000000 magicpy-0.1.3.1/magicpy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2022-09-06 12:25:39.000000 magicpy-0.1.3.1/magicpy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2022-09-06 12:25:39.000000 magicpy-0.1.3.1/magicpy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-09-06 12:25:39.000000 magicpy-0.1.3.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1660 2022-09-06 12:25:29.000000 magicpy-0.1.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 12:00:38.000000 magicpy-0.1.4/
+-rwxrwxrwx   0 root         (0) root         (0)    32473 2023-06-06 10:57:29.000000 magicpy-0.1.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5606 2023-06-06 12:00:38.000000 magicpy-0.1.4/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     4655 2023-06-06 10:57:29.000000 magicpy-0.1.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 12:00:38.000000 magicpy-0.1.4/magicpy/
+-rwxrwxrwx   0 root         (0) root         (0)      104 2023-06-06 11:59:20.000000 magicpy-0.1.4/magicpy/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    64561 2023-06-06 10:57:29.000000 magicpy-0.1.4/magicpy/magicpy.py
+-rwxrwxrwx   0 root         (0) root         (0)     1374 2023-06-06 10:57:29.000000 magicpy-0.1.4/magicpy/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 12:00:38.000000 magicpy-0.1.4/magicpy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5606 2023-06-06 12:00:38.000000 magicpy-0.1.4/magicpy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      236 2023-06-06 12:00:38.000000 magicpy-0.1.4/magicpy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 12:00:38.000000 magicpy-0.1.4/magicpy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-06-06 12:00:38.000000 magicpy-0.1.4/magicpy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-06 12:00:38.000000 magicpy-0.1.4/magicpy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 12:00:38.000000 magicpy-0.1.4/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1660 2023-06-06 10:57:29.000000 magicpy-0.1.4/setup.py
```

### Comparing `magicpy-0.1.3.1/LICENSE` & `magicpy-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `magicpy-0.1.3.1/PKG-INFO` & `magicpy-0.1.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magicpy
-Version: 0.1.3.1
+Version: 0.1.4
 Summary: Toolbox to control MagVenture TMS stimulators
 Home-page: UNKNOWN
 Author: Ole Numssen
 Author-email: numssen@posteo.de
 License: UNKNOWN
 Project-URL: Home, https://gitlab.gwdg.de/tms-localization/utils/magicpy
 Project-URL: Docs, https://magicpy.readthedocs.io/
@@ -20,17 +20,14 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MagicPy
-[![Latest Release](https://gitlab.gwdg.de/tms-localization/utils/magicpy/-/badges/release.svg)](https://pypi.org/project/magicpy/)
-[![pipeline status](https://gitlab.gwdg.de/tms-localization/utils/magicpy/badges/-/pipeline.svg?ignore_skipped=true)](https://gitlab.gwdg.de/tms-localization/utils/magicpy/commits/master)
-[![coverage report](https://gitlab.gwdg.de/tms-localization/utils/magicpy/badges/main/coverage.svg)](https://tms-localization.pages.gwdg.de/pynibs/)
 
 This toolbox can be used to communicate with MagVenture TMS stimulators via python.  
 For the most part it's just a python translation of the Magventure part of the MAGIC toolbox (https://github.com/nigelrogasch/MAGIC). If you use this toolbox, please also cite the original MAGIC toolbox.
 
 This is no official tool, for use at own risk.
 
 ## Installation
@@ -113,8 +110,12 @@
 ``` python
 stimulator = mp.MagVenture('/dev/ttyS0', wait_s=3, wait_l=8)  # Set waittime to 3 seconds and 8 seconds
 ```
 
 ### Stimulator stops responding to commands sent via serial until restart
 - This seems to happen if malformed commands are sent to the stimulator. This might be a bug in this toolbox or due to newer stimulator fimware versions. Feel free to open an issue about it.
 
+# Citation
+Please cite this software when using magicPy in your studies:  
+*Numssen, O. (2022). magicPy. DOI: 10.13140/RG.2.2.15964.46722.*
+
```

### Comparing `magicpy-0.1.3.1/README.md` & `magicpy-0.1.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 # MagicPy
-[![Latest Release](https://gitlab.gwdg.de/tms-localization/utils/magicpy/-/badges/release.svg)](https://pypi.org/project/magicpy/)
-[![pipeline status](https://gitlab.gwdg.de/tms-localization/utils/magicpy/badges/-/pipeline.svg?ignore_skipped=true)](https://gitlab.gwdg.de/tms-localization/utils/magicpy/commits/master)
-[![coverage report](https://gitlab.gwdg.de/tms-localization/utils/magicpy/badges/main/coverage.svg)](https://tms-localization.pages.gwdg.de/pynibs/)
 
 This toolbox can be used to communicate with MagVenture TMS stimulators via python.  
 For the most part it's just a python translation of the Magventure part of the MAGIC toolbox (https://github.com/nigelrogasch/MAGIC). If you use this toolbox, please also cite the original MAGIC toolbox.
 
 This is no official tool, for use at own risk.
 
 ## Installation
@@ -87,7 +84,11 @@
 - Increase the waittime after sending a command to the stimulator before reading the response. Use the `wait_s` and `wait_l` parameters while initializing the stimulator object:
 ``` python
 stimulator = mp.MagVenture('/dev/ttyS0', wait_s=3, wait_l=8)  # Set waittime to 3 seconds and 8 seconds
 ```
 
 ### Stimulator stops responding to commands sent via serial until restart
 - This seems to happen if malformed commands are sent to the stimulator. This might be a bug in this toolbox or due to newer stimulator fimware versions. Feel free to open an issue about it.
+
+# Citation
+Please cite this software when using magicPy in your studies:  
+*Numssen, O. (2022). magicPy. DOI: 10.13140/RG.2.2.15964.46722.*
```

### Comparing `magicpy-0.1.3.1/magicpy/magicpy.py` & `magicpy-0.1.4/magicpy/magicpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,16 @@
 
         p.bytesize = serial.EIGHTBITS
         p.parity = serial.PARITY_NONE
         p.stopbits = serial.STOPBITS_ONE
         p.timeout = 3
 
         self.port = p
-        self.coil_types = {62: 'MCF-B65'}
+        self.coil_types = {62: 'MCF-B65',
+                           82: 'MC-B70'}
         self.show_coil_hint = True
         self.flush_before_cmd = flush_before_cmd
         self.sleep_short = wait_s
         self.sleep_long = wait_l
 
         if ttl_port is not None:
             self.ttl_port = TriggerPort(ttl_port)
```

### Comparing `magicpy-0.1.3.1/magicpy/utils.py` & `magicpy-0.1.4/magicpy/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     """
 
     ports = serial.tools.list_ports.comports()
     print(f"{'port': <13}|{'description': <22}| {'hwid': <34} | subsystem")
     print('-' * 84)
     for p in sorted(ports):
         port, desc, hwid = p
-        subsys = p.subsystem
+        subsys = p.subsystem if hasattr(p, "subsystem") else "n/a"
         print(f"{port: <13}| {desc: <20} | {hwid: <34} | {subsys}")
     return ports
 
 
 class TriggerPort:
     """
     Just a wrapper to pyparallel port to send a TTL pulse.
```

### Comparing `magicpy-0.1.3.1/magicpy.egg-info/PKG-INFO` & `magicpy-0.1.4/magicpy.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magicpy
-Version: 0.1.3.1
+Version: 0.1.4
 Summary: Toolbox to control MagVenture TMS stimulators
 Home-page: UNKNOWN
 Author: Ole Numssen
 Author-email: numssen@posteo.de
 License: UNKNOWN
 Project-URL: Home, https://gitlab.gwdg.de/tms-localization/utils/magicpy
 Project-URL: Docs, https://magicpy.readthedocs.io/
@@ -20,17 +20,14 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MagicPy
-[![Latest Release](https://gitlab.gwdg.de/tms-localization/utils/magicpy/-/badges/release.svg)](https://pypi.org/project/magicpy/)
-[![pipeline status](https://gitlab.gwdg.de/tms-localization/utils/magicpy/badges/-/pipeline.svg?ignore_skipped=true)](https://gitlab.gwdg.de/tms-localization/utils/magicpy/commits/master)
-[![coverage report](https://gitlab.gwdg.de/tms-localization/utils/magicpy/badges/main/coverage.svg)](https://tms-localization.pages.gwdg.de/pynibs/)
 
 This toolbox can be used to communicate with MagVenture TMS stimulators via python.  
 For the most part it's just a python translation of the Magventure part of the MAGIC toolbox (https://github.com/nigelrogasch/MAGIC). If you use this toolbox, please also cite the original MAGIC toolbox.
 
 This is no official tool, for use at own risk.
 
 ## Installation
@@ -113,8 +110,12 @@
 ``` python
 stimulator = mp.MagVenture('/dev/ttyS0', wait_s=3, wait_l=8)  # Set waittime to 3 seconds and 8 seconds
 ```
 
 ### Stimulator stops responding to commands sent via serial until restart
 - This seems to happen if malformed commands are sent to the stimulator. This might be a bug in this toolbox or due to newer stimulator fimware versions. Feel free to open an issue about it.
 
+# Citation
+Please cite this software when using magicPy in your studies:  
+*Numssen, O. (2022). magicPy. DOI: 10.13140/RG.2.2.15964.46722.*
+
```

### Comparing `magicpy-0.1.3.1/setup.py` & `magicpy-0.1.4/setup.py`

 * *Files identical despite different names*

