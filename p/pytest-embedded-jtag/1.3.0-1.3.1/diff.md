# Comparing `tmp/pytest-embedded-jtag-1.3.0.tar.gz` & `tmp/pytest-embedded-jtag-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytest-embedded-jtag-1.3.0.tar", last modified: Wed May 31 13:09:03 2023, max compression
+gzip compressed data, was "dist/pytest-embedded-jtag-1.3.1.tar", last modified: Tue Jun  6 08:07:05 2023, max compression
```

## Comparing `pytest-embedded-jtag-1.3.0.tar` & `pytest-embedded-jtag-1.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:09:03.000000 pytest-embedded-jtag-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-31 13:09:03.000000 pytest-embedded-jtag-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-31 13:08:52.000000 pytest-embedded-jtag-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:09:03.000000 pytest-embedded-jtag-1.3.0/pytest_embedded_jtag/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-31 13:08:52.000000 pytest-embedded-jtag-1.3.0/pytest_embedded_jtag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-31 13:08:52.000000 pytest-embedded-jtag-1.3.0/pytest_embedded_jtag/gdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-31 13:08:52.000000 pytest-embedded-jtag-1.3.0/pytest_embedded_jtag/openocd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:09:03.000000 pytest-embedded-jtag-1.3.0/pytest_embedded_jtag.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-31 13:09:03.000000 pytest-embedded-jtag-1.3.0/pytest_embedded_jtag.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-31 13:09:03.000000 pytest-embedded-jtag-1.3.0/pytest_embedded_jtag.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 13:09:03.000000 pytest-embedded-jtag-1.3.0/pytest_embedded_jtag.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-31 13:09:03.000000 pytest-embedded-jtag-1.3.0/pytest_embedded_jtag.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-31 13:09:03.000000 pytest-embedded-jtag-1.3.0/pytest_embedded_jtag.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 13:09:03.000000 pytest-embedded-jtag-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-31 13:08:52.000000 pytest-embedded-jtag-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:07:05.000000 pytest-embedded-jtag-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-06 08:07:05.000000 pytest-embedded-jtag-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-06 08:06:48.000000 pytest-embedded-jtag-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:07:05.000000 pytest-embedded-jtag-1.3.1/pytest_embedded_jtag/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-06 08:06:48.000000 pytest-embedded-jtag-1.3.1/pytest_embedded_jtag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-06 08:06:48.000000 pytest-embedded-jtag-1.3.1/pytest_embedded_jtag/gdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-06-06 08:06:48.000000 pytest-embedded-jtag-1.3.1/pytest_embedded_jtag/openocd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 08:07:05.000000 pytest-embedded-jtag-1.3.1/pytest_embedded_jtag.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-06 08:07:05.000000 pytest-embedded-jtag-1.3.1/pytest_embedded_jtag.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-06 08:07:05.000000 pytest-embedded-jtag-1.3.1/pytest_embedded_jtag.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 08:07:05.000000 pytest-embedded-jtag-1.3.1/pytest_embedded_jtag.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-06 08:07:05.000000 pytest-embedded-jtag-1.3.1/pytest_embedded_jtag.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-06 08:07:05.000000 pytest-embedded-jtag-1.3.1/pytest_embedded_jtag.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 08:07:05.000000 pytest-embedded-jtag-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-06-06 08:06:48.000000 pytest-embedded-jtag-1.3.1/setup.py
```

### Comparing `pytest-embedded-jtag-1.3.0/PKG-INFO` & `pytest-embedded-jtag-1.3.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pytest-embedded-jtag
-Version: 1.3.0
+Version: 1.3.1
 Summary: pytest embedded plugin for testing with jtag
 Home-page: https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Author: Fu Hanxi
 Author-email: fuhanxi@espressif.com
 License: MIT
 Description: ### pytest-embedded-jtag
         
@@ -12,21 +12,14 @@
         
         Extra Functionalities:
         
         - `openocd`: enable the fixture
         - `gdb`: enable the fixture
         - `dut`: duplicate the `openocd` output and the `gdb` output to `dut.pexpect_proc`.
         
-        Used CLI Options:
-        
-        - `gdb-prog-path`
-        - `gdb-cli-args`
-        - `openocd-prog-path`
-        - `openocd-cli-args`
-        
 Platform: UNKNOWN
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pytest-embedded-jtag-1.3.0/pytest_embedded_jtag/gdb.py` & `pytest-embedded-jtag-1.3.1/pytest_embedded_jtag/gdb.py`

 * *Files identical despite different names*

### Comparing `pytest-embedded-jtag-1.3.0/pytest_embedded_jtag/openocd.py` & `pytest-embedded-jtag-1.3.1/pytest_embedded_jtag/openocd.py`

 * *Files identical despite different names*

### Comparing `pytest-embedded-jtag-1.3.0/pytest_embedded_jtag.egg-info/PKG-INFO` & `pytest-embedded-jtag-1.3.1/pytest_embedded_jtag.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pytest-embedded-jtag
-Version: 1.3.0
+Version: 1.3.1
 Summary: pytest embedded plugin for testing with jtag
 Home-page: https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Author: Fu Hanxi
 Author-email: fuhanxi@espressif.com
 License: MIT
 Description: ### pytest-embedded-jtag
         
@@ -12,21 +12,14 @@
         
         Extra Functionalities:
         
         - `openocd`: enable the fixture
         - `gdb`: enable the fixture
         - `dut`: duplicate the `openocd` output and the `gdb` output to `dut.pexpect_proc`.
         
-        Used CLI Options:
-        
-        - `gdb-prog-path`
-        - `gdb-cli-args`
-        - `openocd-prog-path`
-        - `openocd-cli-args`
-        
 Platform: UNKNOWN
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `pytest-embedded-jtag-1.3.0/setup.py` & `pytest-embedded-jtag-1.3.1/setup.py`

 * *Files identical despite different names*

