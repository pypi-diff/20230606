# Comparing `tmp/xtalx-1.0.1.tar.gz` & `tmp/xtalx-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtalx-1.0.1.tar", last modified: Sat Aug 21 01:53:16 2021, max compression
+gzip compressed data, was "xtalx-1.0.2.tar", last modified: Tue Jun  6 00:05:25 2023, max compression
```

## Comparing `xtalx-1.0.1.tar` & `xtalx-1.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2021-08-21 01:53:16.197777 xtalx-1.0.1/
--rw-r--r--   0 greent7    (502) staff       (20)     1092 2021-08-21 00:14:38.000000 xtalx-1.0.1/LICENSE
--rw-r--r--   0 greent7    (502) staff       (20)     3262 2021-08-21 01:53:16.198216 xtalx-1.0.1/PKG-INFO
--rw-r--r--   0 greent7    (502) staff       (20)     2190 2021-08-21 01:48:13.000000 xtalx-1.0.1/README.rst
--rw-r--r--   0 greent7    (502) staff       (20)      782 2021-08-21 01:53:16.199250 xtalx-1.0.1/setup.cfg
--rw-r--r--   0 greent7    (502) staff       (20)       38 2021-08-19 00:00:42.000000 xtalx-1.0.1/setup.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2021-08-21 01:53:16.191425 xtalx-1.0.1/xtalx/
--rw-r--r--   0 greent7    (502) staff       (20)      222 2021-08-21 00:17:21.000000 xtalx-1.0.1/xtalx/__init__.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2021-08-21 01:53:16.197165 xtalx-1.0.1/xtalx/tools/
--rw-r--r--   0 greent7    (502) staff       (20)        0 2021-08-20 03:33:29.000000 xtalx-1.0.1/xtalx/tools/__init__.py
--rw-r--r--   0 greent7    (502) staff       (20)      498 2021-08-21 00:12:15.000000 xtalx-1.0.1/xtalx/tools/discover.py
--rw-r--r--   0 greent7    (502) staff       (20)     1265 2021-08-21 01:34:44.000000 xtalx-1.0.1/xtalx/tools/xtalx_test_read.py
--rw-r--r--   0 greent7    (502) staff       (20)     1181 2021-08-21 01:34:44.000000 xtalx-1.0.1/xtalx/tools/xtalx_test_yield.py
--rw-r--r--   0 greent7    (502) staff       (20)    13712 2021-08-21 01:34:44.000000 xtalx-1.0.1/xtalx/xtalx.py
-drwxr-xr-x   0 greent7    (502) staff       (20)        0 2021-08-21 01:53:16.194951 xtalx-1.0.1/xtalx.egg-info/
--rw-r--r--   0 greent7    (502) staff       (20)     3262 2021-08-21 01:53:15.000000 xtalx-1.0.1/xtalx.egg-info/PKG-INFO
--rw-r--r--   0 greent7    (502) staff       (20)      357 2021-08-21 01:53:16.000000 xtalx-1.0.1/xtalx.egg-info/SOURCES.txt
--rw-r--r--   0 greent7    (502) staff       (20)        1 2021-08-21 01:53:15.000000 xtalx-1.0.1/xtalx.egg-info/dependency_links.txt
--rw-r--r--   0 greent7    (502) staff       (20)      111 2021-08-21 01:53:15.000000 xtalx-1.0.1/xtalx.egg-info/entry_points.txt
--rw-r--r--   0 greent7    (502) staff       (20)       26 2021-08-21 01:53:15.000000 xtalx-1.0.1/xtalx.egg-info/requires.txt
--rw-r--r--   0 greent7    (502) staff       (20)        6 2021-08-21 01:53:15.000000 xtalx-1.0.1/xtalx.egg-info/top_level.txt
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-06-06 00:05:25.361720 xtalx-1.0.2/
+-rw-r--r--   0 greent7    (502) staff       (20)     1092 2023-06-05 20:34:21.000000 xtalx-1.0.2/LICENSE
+-rw-r--r--   0 greent7    (502) staff       (20)     2685 2023-06-06 00:05:25.361777 xtalx-1.0.2/PKG-INFO
+-rw-r--r--   0 greent7    (502) staff       (20)     2190 2023-06-05 20:34:21.000000 xtalx-1.0.2/README.rst
+-rw-r--r--   0 greent7    (502) staff       (20)      782 2023-06-06 00:05:25.362029 xtalx-1.0.2/setup.cfg
+-rw-r--r--   0 greent7    (502) staff       (20)       38 2023-06-05 20:34:21.000000 xtalx-1.0.2/setup.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-06-06 00:05:25.360702 xtalx-1.0.2/xtalx/
+-rw-r--r--   0 greent7    (502) staff       (20)      222 2023-06-05 20:34:21.000000 xtalx-1.0.2/xtalx/__init__.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-06-06 00:05:25.361638 xtalx-1.0.2/xtalx/tools/
+-rw-r--r--   0 greent7    (502) staff       (20)        0 2023-06-05 20:34:21.000000 xtalx-1.0.2/xtalx/tools/__init__.py
+-rw-r--r--   0 greent7    (502) staff       (20)      498 2023-06-05 20:34:21.000000 xtalx-1.0.2/xtalx/tools/discover.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1265 2023-06-05 20:34:21.000000 xtalx-1.0.2/xtalx/tools/xtalx_test_read.py
+-rw-r--r--   0 greent7    (502) staff       (20)     1575 2023-06-05 20:54:27.000000 xtalx-1.0.2/xtalx/tools/xtalx_test_yield.py
+-rw-r--r--   0 greent7    (502) staff       (20)    13776 2023-06-05 20:56:37.000000 xtalx-1.0.2/xtalx/xtalx.py
+drwxr-xr-x   0 greent7    (502) staff       (20)        0 2023-06-06 00:05:25.361272 xtalx-1.0.2/xtalx.egg-info/
+-rw-r--r--   0 greent7    (502) staff       (20)     2685 2023-06-06 00:05:25.000000 xtalx-1.0.2/xtalx.egg-info/PKG-INFO
+-rw-r--r--   0 greent7    (502) staff       (20)      357 2023-06-06 00:05:25.000000 xtalx-1.0.2/xtalx.egg-info/SOURCES.txt
+-rw-r--r--   0 greent7    (502) staff       (20)        1 2023-06-06 00:05:25.000000 xtalx-1.0.2/xtalx.egg-info/dependency_links.txt
+-rw-r--r--   0 greent7    (502) staff       (20)      110 2023-06-06 00:05:25.000000 xtalx-1.0.2/xtalx.egg-info/entry_points.txt
+-rw-r--r--   0 greent7    (502) staff       (20)       26 2023-06-06 00:05:25.000000 xtalx-1.0.2/xtalx.egg-info/requires.txt
+-rw-r--r--   0 greent7    (502) staff       (20)        6 2023-06-06 00:05:25.000000 xtalx-1.0.2/xtalx.egg-info/top_level.txt
```

### Comparing `xtalx-1.0.1/LICENSE` & `xtalx-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xtalx-1.0.1/PKG-INFO` & `xtalx-1.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,87 +1,87 @@
 Metadata-Version: 2.1
 Name: xtalx
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python library for the XtalX sensor.
 Home-page: https://github.com/phasesensors/xtalx_python
 Author: Phase Advanced Sensor Systems Corp.
 Author-email: tgreeniaus@phasesensors.com
 License: MIT
-Description: xtalx
-        =====
-        This package provides a library for interfacing with the XtalX pressure sensor.
-        Python version 3 is required.  The easiest way to install the xtalx library is
-        using pip::
-        
-            python3 -m pip install xtalx
-        
-        Note that you may wish to use sudo to install xtalx for all users on your
-        system::
-        
-            sudo python3 -m pip install xtalx
-        
-        You may also install the package from the source using::
-        
-            make install
-        
-        or::
-        
-            sudo make install
-        
-        The xtalx python libraries currently require the pyusb package to be installed
-        for communicating with the sensor; this requires the libusb back-end to be
-        installed on the target system.  On Linux-based systems libusb typically comes
-        pre-installed.  On macOS-based systems it can be installed via HomeBrew::
-        
-            brew install libusb
-        
-        On Windows-based systems, libusb releases are available at:
-        
-            https://github.com/libusb/libusb/releases
-        
-        with more information available here:
-        
-            https://github.com/libusb/libusb/wiki/Windows#How_to_use_libusb_on_Windows
-        
-        Since the XtalX sensor is plug-and-play compatible with the WinUSB driver, no
-        other special driver should be required for Windows compatibility.
-        
-        
-        xtalx_discover
-        ==============
-        
-        The xtalx package includes the xtalx_discover binary which can be used to list
-        all XtalX sensors that are attached to the system and their corresponding
-        firmware versions::
-        
-            ~$ xtalx_discover
-            ******************
-            Sensor SN: XTI-7-1000035
-             git SHA1: 61be0469c1162b755d02fd9156a2754bebf24f59.dirty
-               Version: 0x0107
-        
-        
-        xtalx_test
-        ==========
-        The xtalx package includes a simple test binary that will connect to an XtalX
-        sensor and continuously print the current pressure and temperature reading::
-        
-            ~$ xtalx_test
-            XtalX(XTI-7-1000035): 23.973375 PSI, 23.947930 C
-            XtalX(XTI-7-1000035): 23.973375 PSI, 23.947930 C
-            XtalX(XTI-7-1000035): 23.973375 PSI, 23.947930 C
-            XtalX(XTI-7-1000035): 23.963872 PSI, 23.947930 C
-            XtalX(XTI-7-1000035): 23.963872 PSI, 23.947930 C
-            XtalX(XTI-7-1000035): 23.954370 PSI, 23.947930 C
-            XtalX(XTI-7-1000035): 23.954370 PSI, 23.947930 C
-            XtalX(XTI-7-1000035): 23.973375 PSI, 23.947930 C
-            ...
-        
-        Terminate the program by pressing Ctrl-C.
-        
 Keywords: xtalx
-Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+xtalx
+=====
+This package provides a library for interfacing with the XtalX pressure sensor.
+Python version 3 is required.  The easiest way to install the xtalx library is
+using pip::
+
+    python3 -m pip install xtalx
+
+Note that you may wish to use sudo to install xtalx for all users on your
+system::
+
+    sudo python3 -m pip install xtalx
+
+You may also install the package from the source using::
+
+    make install
+
+or::
+
+    sudo make install
+
+The xtalx python libraries currently require the pyusb package to be installed
+for communicating with the sensor; this requires the libusb back-end to be
+installed on the target system.  On Linux-based systems libusb typically comes
+pre-installed.  On macOS-based systems it can be installed via HomeBrew::
+
+    brew install libusb
+
+On Windows-based systems, libusb releases are available at:
+
+    https://github.com/libusb/libusb/releases
+
+with more information available here:
+
+    https://github.com/libusb/libusb/wiki/Windows#How_to_use_libusb_on_Windows
+
+Since the XtalX sensor is plug-and-play compatible with the WinUSB driver, no
+other special driver should be required for Windows compatibility.
+
+
+xtalx_discover
+==============
+
+The xtalx package includes the xtalx_discover binary which can be used to list
+all XtalX sensors that are attached to the system and their corresponding
+firmware versions::
+
+    ~$ xtalx_discover
+    ******************
+    Sensor SN: XTI-7-1000035
+     git SHA1: 61be0469c1162b755d02fd9156a2754bebf24f59.dirty
+       Version: 0x0107
+
+
+xtalx_test
+==========
+The xtalx package includes a simple test binary that will connect to an XtalX
+sensor and continuously print the current pressure and temperature reading::
+
+    ~$ xtalx_test
+    XtalX(XTI-7-1000035): 23.973375 PSI, 23.947930 C
+    XtalX(XTI-7-1000035): 23.973375 PSI, 23.947930 C
+    XtalX(XTI-7-1000035): 23.973375 PSI, 23.947930 C
+    XtalX(XTI-7-1000035): 23.963872 PSI, 23.947930 C
+    XtalX(XTI-7-1000035): 23.963872 PSI, 23.947930 C
+    XtalX(XTI-7-1000035): 23.954370 PSI, 23.947930 C
+    XtalX(XTI-7-1000035): 23.954370 PSI, 23.947930 C
+    XtalX(XTI-7-1000035): 23.973375 PSI, 23.947930 C
+    ...
+
+Terminate the program by pressing Ctrl-C.
```

### Comparing `xtalx-1.0.1/README.rst` & `xtalx-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `xtalx-1.0.1/setup.cfg` & `xtalx-1.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = xtalx
-version = 1.0.1
+version = 1.0.2
 author = Phase Advanced Sensor Systems Corp.
 author_email = tgreeniaus@phasesensors.com
 description = Python library for the XtalX sensor.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 keywords = xtalx
 url = https://github.com/phasesensors/xtalx_python
```

### Comparing `xtalx-1.0.1/xtalx/tools/xtalx_test_read.py` & `xtalx-1.0.2/xtalx/tools/xtalx_test_read.py`

 * *Files identical despite different names*

### Comparing `xtalx-1.0.1/xtalx/tools/xtalx_test_yield.py` & `xtalx-1.0.2/xtalx/tools/xtalx_test_yield.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 #!/usr/bin/env python3
 # Copyright (c) 2020-2021 by Phase Advanced Sensor Systems Corp.
 import argparse
+import time
 
 import xtalx
 
 
 VERBOSE = False
 
 
-def xtalx_cb(m):
+def xtalx_cb(m, csv_file):
     print(m.tostring(VERBOSE))
+    if csv_file:
+        csv_file.write('%.6f,%.2f,%.5f\n' % (
+            time.time(), m.temp_c, m.pressure_psi))
 
 
 def main(args):
     global VERBOSE
     VERBOSE = args.verbose
 
     if args.serial_number is not None:
@@ -31,22 +35,30 @@
     if len(sensors) != 1:
         print('Matching sensors:')
         for s in sensors:
             print('    %s' % s.serial_number)
         return
     d = sensors[0]
 
+    if args.csv_file:
+        csv_file = open(  # pylint: disable=R1732
+            args.csv_file, 'a', encoding='utf8')
+        csv_file.write('time,temp_c,pressure_psi\n')
+    else:
+        csv_file = None
+
     for m in xtalx.XtalX(d).yield_measurements():
-        xtalx_cb(m)
+        xtalx_cb(m, csv_file)
 
 
 def _main():
     parser = argparse.ArgumentParser()
     parser.add_argument('--serial-number', '-s')
     parser.add_argument('--verbose', '-v', action='store_true')
+    parser.add_argument('--csv-file')
     try:
         main(parser.parse_args())
     except KeyboardInterrupt:
         print()
 
 
 if __name__ == '__main__':
```

### Comparing `xtalx-1.0.1/xtalx/xtalx.py` & `xtalx-1.0.2/xtalx/xtalx.py`

 * *Files 7% similar despite different names*

```diff
@@ -195,14 +195,18 @@
             else:
                 t = '%f' % self.temp_c
             s += '%s PSI, %s C' % (p, t)
 
         return s
 
 
+class XtalXException(Exception):
+    pass
+
+
 class XtalX:
     '''
     Given a USB device handle acquired via find() or find_one(), creates an
     XtalX object that can be used to communicate with a sensor.
     '''
     def __init__(self, usb_dev):
         self.usb_dev     = usb_dev
@@ -212,15 +216,15 @@
 
         try:
             self.serial_num = usb_dev.serial_number
             self.git_sha1   = usb.util.get_string(usb_dev, 6)
             self.fw_version = usb_dev.bcdDevice
         except ValueError as e:
             if str(e) == 'The device has no langid':
-                raise Exception(
+                raise XtalXException(
                     'Device has no langid, ensure running as root!') from e
 
         if self.usb_dev.bcdDevice >= 0x0103:
             try:
                 self.report_id = usb.util.get_string(usb_dev, 15)
             except ValueError:
                 self.report_id = None
@@ -340,12 +344,12 @@
     Returns a single USB device handle for an XtalX sensor if only a single
     sensor is attached.  If multiple sensors are found, an exception is raised.
     **kwargs can be any keyword argument accepted by usb.core.find(); typically
     you will leave it empty.
     '''
     usb_devs = find(**kwargs)
     if len(usb_devs) > 1:
-        raise Exception('Multiple matching devices: %s' %
-                        ', '.join(ud.serial_number for ud in usb_devs))
+        raise XtalXException('Multiple matching devices: %s' %
+                             ', '.join(ud.serial_number for ud in usb_devs))
     if not usb_devs:
-        raise Exception('No matching devices.')
+        raise XtalXException('No matching devices.')
     return usb_devs[0]
```

### Comparing `xtalx-1.0.1/xtalx.egg-info/PKG-INFO` & `xtalx-1.0.2/xtalx.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,87 +1,87 @@
 Metadata-Version: 2.1
 Name: xtalx
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python library for the XtalX sensor.
 Home-page: https://github.com/phasesensors/xtalx_python
 Author: Phase Advanced Sensor Systems Corp.
 Author-email: tgreeniaus@phasesensors.com
 License: MIT
-Description: xtalx
-        =====
-        This package provides a library for interfacing with the XtalX pressure sensor.
-        Python version 3 is required.  The easiest way to install the xtalx library is
-        using pip::
-        
-            python3 -m pip install xtalx
-        
-        Note that you may wish to use sudo to install xtalx for all users on your
-        system::
-        
-            sudo python3 -m pip install xtalx
-        
-        You may also install the package from the source using::
-        
-            make install
-        
-        or::
-        
-            sudo make install
-        
-        The xtalx python libraries currently require the pyusb package to be installed
-        for communicating with the sensor; this requires the libusb back-end to be
-        installed on the target system.  On Linux-based systems libusb typically comes
-        pre-installed.  On macOS-based systems it can be installed via HomeBrew::
-        
-            brew install libusb
-        
-        On Windows-based systems, libusb releases are available at:
-        
-            https://github.com/libusb/libusb/releases
-        
-        with more information available here:
-        
-            https://github.com/libusb/libusb/wiki/Windows#How_to_use_libusb_on_Windows
-        
-        Since the XtalX sensor is plug-and-play compatible with the WinUSB driver, no
-        other special driver should be required for Windows compatibility.
-        
-        
-        xtalx_discover
-        ==============
-        
-        The xtalx package includes the xtalx_discover binary which can be used to list
-        all XtalX sensors that are attached to the system and their corresponding
-        firmware versions::
-        
-            ~$ xtalx_discover
-            ******************
-            Sensor SN: XTI-7-1000035
-             git SHA1: 61be0469c1162b755d02fd9156a2754bebf24f59.dirty
-               Version: 0x0107
-        
-        
-        xtalx_test
-        ==========
-        The xtalx package includes a simple test binary that will connect to an XtalX
-        sensor and continuously print the current pressure and temperature reading::
-        
-            ~$ xtalx_test
-            XtalX(XTI-7-1000035): 23.973375 PSI, 23.947930 C
-            XtalX(XTI-7-1000035): 23.973375 PSI, 23.947930 C
-            XtalX(XTI-7-1000035): 23.973375 PSI, 23.947930 C
-            XtalX(XTI-7-1000035): 23.963872 PSI, 23.947930 C
-            XtalX(XTI-7-1000035): 23.963872 PSI, 23.947930 C
-            XtalX(XTI-7-1000035): 23.954370 PSI, 23.947930 C
-            XtalX(XTI-7-1000035): 23.954370 PSI, 23.947930 C
-            XtalX(XTI-7-1000035): 23.973375 PSI, 23.947930 C
-            ...
-        
-        Terminate the program by pressing Ctrl-C.
-        
 Keywords: xtalx
-Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+xtalx
+=====
+This package provides a library for interfacing with the XtalX pressure sensor.
+Python version 3 is required.  The easiest way to install the xtalx library is
+using pip::
+
+    python3 -m pip install xtalx
+
+Note that you may wish to use sudo to install xtalx for all users on your
+system::
+
+    sudo python3 -m pip install xtalx
+
+You may also install the package from the source using::
+
+    make install
+
+or::
+
+    sudo make install
+
+The xtalx python libraries currently require the pyusb package to be installed
+for communicating with the sensor; this requires the libusb back-end to be
+installed on the target system.  On Linux-based systems libusb typically comes
+pre-installed.  On macOS-based systems it can be installed via HomeBrew::
+
+    brew install libusb
+
+On Windows-based systems, libusb releases are available at:
+
+    https://github.com/libusb/libusb/releases
+
+with more information available here:
+
+    https://github.com/libusb/libusb/wiki/Windows#How_to_use_libusb_on_Windows
+
+Since the XtalX sensor is plug-and-play compatible with the WinUSB driver, no
+other special driver should be required for Windows compatibility.
+
+
+xtalx_discover
+==============
+
+The xtalx package includes the xtalx_discover binary which can be used to list
+all XtalX sensors that are attached to the system and their corresponding
+firmware versions::
+
+    ~$ xtalx_discover
+    ******************
+    Sensor SN: XTI-7-1000035
+     git SHA1: 61be0469c1162b755d02fd9156a2754bebf24f59.dirty
+       Version: 0x0107
+
+
+xtalx_test
+==========
+The xtalx package includes a simple test binary that will connect to an XtalX
+sensor and continuously print the current pressure and temperature reading::
+
+    ~$ xtalx_test
+    XtalX(XTI-7-1000035): 23.973375 PSI, 23.947930 C
+    XtalX(XTI-7-1000035): 23.973375 PSI, 23.947930 C
+    XtalX(XTI-7-1000035): 23.973375 PSI, 23.947930 C
+    XtalX(XTI-7-1000035): 23.963872 PSI, 23.947930 C
+    XtalX(XTI-7-1000035): 23.963872 PSI, 23.947930 C
+    XtalX(XTI-7-1000035): 23.954370 PSI, 23.947930 C
+    XtalX(XTI-7-1000035): 23.954370 PSI, 23.947930 C
+    XtalX(XTI-7-1000035): 23.973375 PSI, 23.947930 C
+    ...
+
+Terminate the program by pressing Ctrl-C.
```

