# Comparing `tmp/pytest-embedded-serial-1.3.0.tar.gz` & `tmp/pytest-embedded-serial-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytest-embedded-serial-1.3.0.tar", last modified: Wed May 31 13:09:02 2023, max compression
+gzip compressed data, was "dist/pytest-embedded-serial-1.3.1.tar", last modified: Tue Jun  6 08:07:04 2023, max compression
```

## Comparing `pytest-embedded-serial-1.3.0.tar` & `pytest-embedded-serial-1.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:09:02.000000 pytest-embedded-serial-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-31 13:09:02.000000 pytest-embedded-serial-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-31 13:08:52.000000 pytest-embedded-serial-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:09:02.000000 pytest-embedded-serial-1.3.0/pytest_embedded_serial/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-31 13:08:52.000000 pytest-embedded-serial-1.3.0/pytest_embedded_serial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-31 13:08:52.000000 pytest-embedded-serial-1.3.0/pytest_embedded_serial/dut.py
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-05-31 13:08:52.000000 pytest-embedded-serial-1.3.0/pytest_embedded_serial/serial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:09:02.000000 pytest-embedded-serial-1.3.0/pytest_embedded_serial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-31 13:09:02.000000 pytest-embedded-serial-1.3.0/pytest_embedded_serial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-31 13:09:02.000000 pytest-embedded-serial-1.3.0/pytest_embedded_serial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 13:09:02.000000 pytest-embedded-serial-1.3.0/pytest_embedded_serial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-31 13:09:02.000000 pytest-embedded-serial-1.3.0/pytest_embedded_serial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-31 13:09:02.000000 pytest-embedded-serial-1.3.0/pytest_embedded_serial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 13:09:02.000000 pytest-embedded-serial-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-31 13:08:52.000000 pytest-embedded-serial-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:07:04.000000 pytest-embedded-serial-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-06 08:07:04.000000 pytest-embedded-serial-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-06 08:06:48.000000 pytest-embedded-serial-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:07:04.000000 pytest-embedded-serial-1.3.1/pytest_embedded_serial/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-06 08:06:48.000000 pytest-embedded-serial-1.3.1/pytest_embedded_serial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-06 08:06:48.000000 pytest-embedded-serial-1.3.1/pytest_embedded_serial/dut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6113 2023-06-06 08:06:48.000000 pytest-embedded-serial-1.3.1/pytest_embedded_serial/serial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:07:04.000000 pytest-embedded-serial-1.3.1/pytest_embedded_serial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-06 08:07:04.000000 pytest-embedded-serial-1.3.1/pytest_embedded_serial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-06 08:07:04.000000 pytest-embedded-serial-1.3.1/pytest_embedded_serial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 08:07:04.000000 pytest-embedded-serial-1.3.1/pytest_embedded_serial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-06 08:07:04.000000 pytest-embedded-serial-1.3.1/pytest_embedded_serial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-06 08:07:04.000000 pytest-embedded-serial-1.3.1/pytest_embedded_serial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 08:07:04.000000 pytest-embedded-serial-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-06 08:06:48.000000 pytest-embedded-serial-1.3.1/setup.py
```

### Comparing `pytest-embedded-serial-1.3.0/PKG-INFO` & `pytest-embedded-serial-1.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 Metadata-Version: 1.2
 Name: pytest-embedded-serial
-Version: 1.3.0
+Version: 1.3.1
 Summary: pytest embedded plugin for testing serial ports
 Home-page: https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Author: Fu Hanxi
 Author-email: fuhanxi@espressif.com
 License: MIT
 Description: ### pytest-embedded-serial
         
         pytest embedded service for testing via serial ports
         
         Extra Functionalities:
         
         - `serial`: enable the fixture
         - `dut`: duplicate the `serial` output to `pexpect_proc`.
         
-        Used CLI Options:
-        
-        - `port`
-        
 Platform: UNKNOWN
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pytest-embedded-serial-1.3.0/pytest_embedded_serial/dut.py` & `pytest-embedded-serial-1.3.1/pytest_embedded_serial/dut.py`

 * *Files identical despite different names*

### Comparing `pytest-embedded-serial-1.3.0/pytest_embedded_serial/serial.py` & `pytest-embedded-serial-1.3.1/pytest_embedded_serial/serial.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,17 +19,15 @@
 
     Attributes:
         port (str): port address
         baud (int): baud rate
         proc (pyserial.Serial): process created by `serial.serial_for_url()`
 
     Warning:
-        - the real `pyserial` object must be created inside `self._forward_io`,
-          The `pyserial` object can't be pickled when using multiprocessing.Process
-        - make sure this `Serial` __init__ run the last in MRO, it would create and start the redirect serial process
+        - make sure this `Serial.__init__()` run the last in MRO, it would create and start the redirect serial process
     """
 
     DEFAULT_BAUDRATE = 115200
 
     DEFAULT_PORT_CONFIG = {
         'baudrate': DEFAULT_BAUDRATE,
         'bytesize': pyserial.EIGHTBITS,
@@ -94,14 +92,16 @@
 
         self.start_redirect_thread()
 
     def start_redirect_thread(self) -> None:
         if self._redirect_thread and self._redirect_thread.is_alive():
             return
 
+        # Here the reason why we're still using thread is,
+        # the `pyserial` object can't be pickled when using multiprocessing.Process
         self._redirect_thread = _SerialRedirectThread(self._q, self.proc)
         self._redirect_thread.start()
 
     def stop_redirect_thread(self) -> bool:
         killed = False
         if self._redirect_thread and self._redirect_thread.is_alive():
             self._redirect_thread.terminate()
```

### Comparing `pytest-embedded-serial-1.3.0/pytest_embedded_serial.egg-info/PKG-INFO` & `pytest-embedded-serial-1.3.1/pytest_embedded_serial.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 Metadata-Version: 1.2
 Name: pytest-embedded-serial
-Version: 1.3.0
+Version: 1.3.1
 Summary: pytest embedded plugin for testing serial ports
 Home-page: https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Author: Fu Hanxi
 Author-email: fuhanxi@espressif.com
 License: MIT
 Description: ### pytest-embedded-serial
         
         pytest embedded service for testing via serial ports
         
         Extra Functionalities:
         
         - `serial`: enable the fixture
         - `dut`: duplicate the `serial` output to `pexpect_proc`.
         
-        Used CLI Options:
-        
-        - `port`
-        
 Platform: UNKNOWN
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pytest-embedded-serial-1.3.0/setup.py` & `pytest-embedded-serial-1.3.1/setup.py`

 * *Files identical despite different names*

