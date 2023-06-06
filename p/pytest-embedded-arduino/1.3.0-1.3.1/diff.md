# Comparing `tmp/pytest-embedded-arduino-1.3.0.tar.gz` & `tmp/pytest-embedded-arduino-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytest-embedded-arduino-1.3.0.tar", last modified: Wed May 31 13:09:03 2023, max compression
+gzip compressed data, was "pytest-embedded-arduino-1.3.1.tar", last modified: Tue Jun  6 08:56:26 2023, max compression
```

## Comparing `pytest-embedded-arduino-1.3.0.tar` & `pytest-embedded-arduino-1.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:09:03.000000 pytest-embedded-arduino-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-31 13:09:03.000000 pytest-embedded-arduino-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-31 13:08:52.000000 pytest-embedded-arduino-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:09:03.000000 pytest-embedded-arduino-1.3.0/pytest_embedded_arduino/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-31 13:08:52.000000 pytest-embedded-arduino-1.3.0/pytest_embedded_arduino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-31 13:08:52.000000 pytest-embedded-arduino-1.3.0/pytest_embedded_arduino/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-31 13:08:52.000000 pytest-embedded-arduino-1.3.0/pytest_embedded_arduino/serial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:09:03.000000 pytest-embedded-arduino-1.3.0/pytest_embedded_arduino.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-31 13:09:03.000000 pytest-embedded-arduino-1.3.0/pytest_embedded_arduino.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-31 13:09:03.000000 pytest-embedded-arduino-1.3.0/pytest_embedded_arduino.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 13:09:03.000000 pytest-embedded-arduino-1.3.0/pytest_embedded_arduino.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-31 13:09:03.000000 pytest-embedded-arduino-1.3.0/pytest_embedded_arduino.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-31 13:09:03.000000 pytest-embedded-arduino-1.3.0/pytest_embedded_arduino.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 13:09:03.000000 pytest-embedded-arduino-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-05-31 13:08:52.000000 pytest-embedded-arduino-1.3.0/setup.py
+drwxr-xr-x   0 fuhanxi   (1000) fuhanxi   (1000)        0 2023-06-06 08:56:26.685544 pytest-embedded-arduino-1.3.1/
+-rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)     1570 2023-06-06 08:56:26.685544 pytest-embedded-arduino-1.3.1/PKG-INFO
+-rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)      516 2023-06-06 08:04:34.000000 pytest-embedded-arduino-1.3.1/README.md
+drwxr-xr-x   0 fuhanxi   (1000) fuhanxi   (1000)        0 2023-06-06 08:56:26.685544 pytest-embedded-arduino-1.3.1/pytest_embedded_arduino/
+-rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)      116 2023-04-11 02:32:21.000000 pytest-embedded-arduino-1.3.1/pytest_embedded_arduino/__init__.py
+-rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)     1879 2023-06-06 08:04:34.000000 pytest-embedded-arduino-1.3.1/pytest_embedded_arduino/app.py
+-rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)     1870 2023-06-02 06:32:41.000000 pytest-embedded-arduino-1.3.1/pytest_embedded_arduino/serial.py
+drwxr-xr-x   0 fuhanxi   (1000) fuhanxi   (1000)        0 2023-06-06 08:56:26.685544 pytest-embedded-arduino-1.3.1/pytest_embedded_arduino.egg-info/
+-rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)     1570 2023-06-06 08:56:26.000000 pytest-embedded-arduino-1.3.1/pytest_embedded_arduino.egg-info/PKG-INFO
+-rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)      353 2023-06-06 08:56:26.000000 pytest-embedded-arduino-1.3.1/pytest_embedded_arduino.egg-info/SOURCES.txt
+-rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)        1 2023-06-06 08:56:26.000000 pytest-embedded-arduino-1.3.1/pytest_embedded_arduino.egg-info/dependency_links.txt
+-rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)       67 2023-06-06 08:56:26.000000 pytest-embedded-arduino-1.3.1/pytest_embedded_arduino.egg-info/requires.txt
+-rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)       24 2023-06-06 08:56:26.000000 pytest-embedded-arduino-1.3.1/pytest_embedded_arduino.egg-info/top_level.txt
+-rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)       38 2023-06-06 08:56:26.685544 pytest-embedded-arduino-1.3.1/setup.cfg
+-rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)     1901 2023-06-06 08:49:39.000000 pytest-embedded-arduino-1.3.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pytest-embedded-arduino-1.3.0/PKG-INFO` & `pytest-embedded-arduino-1.3.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 Metadata-Version: 2.1
 Name: pytest-embedded-arduino
-Version: 1.3.0
+Version: 1.3.1
 Summary: pytest embedded plugin for Arduino projects
 Home-page: https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Author: Abdelatif Guettouche
 Author-email: abdelatif.guettouche@espressif.com
 License: MIT
-Description: ### pytest-embedded-arduino
-        
-        pytest embedded service for Arduino project
-        
-        Extra Functionalities:
-        
-        === "`pytest-embedded-serial-esp` activated"
-        
-            - `app`: Parse Arduino's build directory and gather more information.
-            - `serial`: Auto flash the built binary into the target board at the beginning when running test cases.
-        
-        === "`pytest-embedded-serial-esp` NOT activated"
-        
-            - `app`: Parse Arduino's build directory and gather more information.
-        
-Platform: UNKNOWN
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
+Description-Content-Type: text/markdown
 Provides-Extra: serial
+
+### pytest-embedded-arduino
+
+pytest embedded service for Arduino project
+
+Extra Functionalities:
+
+```{eval-rst}
+.. tabs::
+
+   .. group-tab:: `pytest-embedded-serial-esp` activated
+
+        - `app`: Parse Arduino's build directory and gather more information.
+        - `serial`: Auto flash the built binary into the target board at the beginning when running test cases.
+
+   .. group-tab:: `pytest-embedded-serial-esp` NOT activated
+
+        - `app`: Parse Arduino's build directory and gather more information.
+```
```

### Comparing `pytest-embedded-arduino-1.3.0/pytest_embedded_arduino/app.py` & `pytest-embedded-arduino-1.3.1/pytest_embedded_arduino/app.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,19 +10,20 @@
     Arduino App class
 
     Attributes:
         sketch (str): Sketch name.
         fqbn (str): Fully Qualified Board Name.
         target (str) : ESPxx chip.
         flash_files (List[Tuple[int, str, str]]): List of (offset, file path, encrypted) of files need to be flashed in.
-        flash_settings (dict[str, Any]): dict of flash settings
-        binary_offsets (dict[str, List[int, int, int]]): dict of binaries' offset.
     """
 
+    #: dict of flash settings
     flash_settings = {'flash_mode': 'dio', 'flash_size': 'detect', 'flash_freq': '80m'}
+
+    #: dict of binaries' offset.
     binary_offsets = {
         'esp32': [0x1000, 0x8000, 0x10000],
         'esp32s2': [0x1000, 0x8000, 0x10000],
         'esp32c3': [0x0, 0x8000, 0x10000],
         'esp32s3': [0x0, 0x8000, 0x10000],
     }
```

### Comparing `pytest-embedded-arduino-1.3.0/pytest_embedded_arduino/serial.py` & `pytest-embedded-arduino-1.3.1/pytest_embedded_arduino/serial.py`

 * *Files identical despite different names*

### Comparing `pytest-embedded-arduino-1.3.0/pytest_embedded_arduino.egg-info/PKG-INFO` & `pytest-embedded-arduino-1.3.1/pytest_embedded_arduino.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 Metadata-Version: 2.1
 Name: pytest-embedded-arduino
-Version: 1.3.0
+Version: 1.3.1
 Summary: pytest embedded plugin for Arduino projects
 Home-page: https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Author: Abdelatif Guettouche
 Author-email: abdelatif.guettouche@espressif.com
 License: MIT
-Description: ### pytest-embedded-arduino
-        
-        pytest embedded service for Arduino project
-        
-        Extra Functionalities:
-        
-        === "`pytest-embedded-serial-esp` activated"
-        
-            - `app`: Parse Arduino's build directory and gather more information.
-            - `serial`: Auto flash the built binary into the target board at the beginning when running test cases.
-        
-        === "`pytest-embedded-serial-esp` NOT activated"
-        
-            - `app`: Parse Arduino's build directory and gather more information.
-        
-Platform: UNKNOWN
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Testing
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
+Description-Content-Type: text/markdown
 Provides-Extra: serial
+
+### pytest-embedded-arduino
+
+pytest embedded service for Arduino project
+
+Extra Functionalities:
+
+```{eval-rst}
+.. tabs::
+
+   .. group-tab:: `pytest-embedded-serial-esp` activated
+
+        - `app`: Parse Arduino's build directory and gather more information.
+        - `serial`: Auto flash the built binary into the target board at the beginning when running test cases.
+
+   .. group-tab:: `pytest-embedded-serial-esp` NOT activated
+
+        - `app`: Parse Arduino's build directory and gather more information.
+```
```

### Comparing `pytest-embedded-arduino-1.3.0/setup.py` & `pytest-embedded-arduino-1.3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,22 +36,24 @@
     version=VERSION,
     author=AUTHOR,
     author_email=EMAIL,
     license=LICENSE,
     url=URL,
     description=SHORT_DESCRIPTION,
     long_description=read('README.md'),
+    long_description_content_type='text/markdown',
     packages=setuptools.find_packages(exclude='tests'),
     python_requires='>=3.7',
     install_requires=REQUIRES,
     extras_require=EXTRAS_REQUIRE,
     classifiers=[
         'Framework :: Pytest',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Testing',
+        'Development Status :: 5 - Production/Stable',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
```

