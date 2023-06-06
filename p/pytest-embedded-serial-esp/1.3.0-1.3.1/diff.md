# Comparing `tmp/pytest-embedded-serial-esp-1.3.0.tar.gz` & `tmp/pytest-embedded-serial-esp-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytest-embedded-serial-esp-1.3.0.tar", last modified: Wed May 31 13:09:02 2023, max compression
+gzip compressed data, was "dist/pytest-embedded-serial-esp-1.3.1.tar", last modified: Tue Jun  6 08:07:04 2023, max compression
```

## Comparing `pytest-embedded-serial-esp-1.3.0.tar` & `pytest-embedded-serial-esp-1.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:09:02.000000 pytest-embedded-serial-esp-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-31 13:09:02.000000 pytest-embedded-serial-esp-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-31 13:08:52.000000 pytest-embedded-serial-esp-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:09:02.000000 pytest-embedded-serial-esp-1.3.0/pytest_embedded_serial_esp/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-31 13:08:52.000000 pytest-embedded-serial-esp-1.3.0/pytest_embedded_serial_esp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-05-31 13:08:52.000000 pytest-embedded-serial-esp-1.3.0/pytest_embedded_serial_esp/serial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:09:02.000000 pytest-embedded-serial-esp-1.3.0/pytest_embedded_serial_esp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-31 13:09:02.000000 pytest-embedded-serial-esp-1.3.0/pytest_embedded_serial_esp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-31 13:09:02.000000 pytest-embedded-serial-esp-1.3.0/pytest_embedded_serial_esp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 13:09:02.000000 pytest-embedded-serial-esp-1.3.0/pytest_embedded_serial_esp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-31 13:09:02.000000 pytest-embedded-serial-esp-1.3.0/pytest_embedded_serial_esp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-31 13:09:02.000000 pytest-embedded-serial-esp-1.3.0/pytest_embedded_serial_esp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 13:09:02.000000 pytest-embedded-serial-esp-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-31 13:08:52.000000 pytest-embedded-serial-esp-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:07:04.000000 pytest-embedded-serial-esp-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-06 08:07:04.000000 pytest-embedded-serial-esp-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-06 08:06:48.000000 pytest-embedded-serial-esp-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:07:04.000000 pytest-embedded-serial-esp-1.3.1/pytest_embedded_serial_esp/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-06 08:06:48.000000 pytest-embedded-serial-esp-1.3.1/pytest_embedded_serial_esp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-06-06 08:06:48.000000 pytest-embedded-serial-esp-1.3.1/pytest_embedded_serial_esp/serial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:07:04.000000 pytest-embedded-serial-esp-1.3.1/pytest_embedded_serial_esp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-06 08:07:04.000000 pytest-embedded-serial-esp-1.3.1/pytest_embedded_serial_esp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-06 08:07:04.000000 pytest-embedded-serial-esp-1.3.1/pytest_embedded_serial_esp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 08:07:04.000000 pytest-embedded-serial-esp-1.3.1/pytest_embedded_serial_esp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-06 08:07:04.000000 pytest-embedded-serial-esp-1.3.1/pytest_embedded_serial_esp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-06 08:07:04.000000 pytest-embedded-serial-esp-1.3.1/pytest_embedded_serial_esp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 08:07:04.000000 pytest-embedded-serial-esp-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-06-06 08:06:48.000000 pytest-embedded-serial-esp-1.3.1/setup.py
```

### Comparing `pytest-embedded-serial-esp-1.3.0/PKG-INFO` & `pytest-embedded-serial-esp-1.3.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 Metadata-Version: 1.2
 Name: pytest-embedded-serial-esp
-Version: 1.3.0
+Version: 1.3.1
 Summary: pytest embedded plugin for testing espressif boards via serial ports
 Home-page: https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Author: Fu Hanxi
 Author-email: fuhanxi@espressif.com
 License: MIT
 Description: ### pytest-embedded-serial-esp
         
         pytest embedded service for testing espressif boards via serial ports
         
         Extra Functionalities:
         
         - `serial`: detect and confirm target and port by `esptool` automatically.
         
-        Used CLI Options:
-        
-        - `target`
-        
 Platform: UNKNOWN
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pytest-embedded-serial-esp-1.3.0/pytest_embedded_serial_esp/serial.py` & `pytest-embedded-serial-esp-1.3.1/pytest_embedded_serial_esp/serial.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,28 +158,23 @@
         if self.erase_all:
             self.erase_flash()
 
         super()._post_init()
 
     def use_esptool(hard_reset_after: bool = True, no_stub: bool = False):
         """
-        1. close the redirect serial process if exists
-        2. close the serial connection
-        3. use esptool to connect to the serial port and call `run_stub()`
-        4. call to the decorated function, could use `self.stub` inside the function as the stubbed loader
-        5. call `hard_reset()`
-        5. create the redirect serial process again
+        1. tell the redirect serial thread to stop reading from the `pyserial` instance
+        2. esptool reuse the `pyserial` instance and call `run_stub()`
+        3. call to the decorated function, could use `self.stub` inside the function as the stubbed loader
+        4. call `hard_reset()`, if `hard_reset_after` is True
+        5. tell the redirect serial thread to continue reading from serial
 
         Args:
             hard_reset_after: run hard reset after
             no_stub: disable launching the flasher stub
-
-        Warning:
-            the real `pyserial` object must be created inside `self._forward_io`,
-                The `pyserial` object can't be pickled when using multiprocessing.Process
         """
 
         def decorator(func):
             @functools.wraps(func)
             def wrapper(self, *args, **kwargs):
                 with self.disable_redirect_thread():
                     with contextlib.redirect_stdout(self._q):
```

### Comparing `pytest-embedded-serial-esp-1.3.0/pytest_embedded_serial_esp.egg-info/PKG-INFO` & `pytest-embedded-serial-esp-1.3.1/pytest_embedded_serial_esp.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 Metadata-Version: 1.2
 Name: pytest-embedded-serial-esp
-Version: 1.3.0
+Version: 1.3.1
 Summary: pytest embedded plugin for testing espressif boards via serial ports
 Home-page: https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Author: Fu Hanxi
 Author-email: fuhanxi@espressif.com
 License: MIT
 Description: ### pytest-embedded-serial-esp
         
         pytest embedded service for testing espressif boards via serial ports
         
         Extra Functionalities:
         
         - `serial`: detect and confirm target and port by `esptool` automatically.
         
-        Used CLI Options:
-        
-        - `target`
-        
 Platform: UNKNOWN
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pytest-embedded-serial-esp-1.3.0/setup.py` & `pytest-embedded-serial-esp-1.3.1/setup.py`

 * *Files identical despite different names*

