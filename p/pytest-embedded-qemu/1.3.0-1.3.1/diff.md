# Comparing `tmp/pytest-embedded-qemu-1.3.0.tar.gz` & `tmp/pytest-embedded-qemu-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytest-embedded-qemu-1.3.0.tar", last modified: Wed May 31 13:09:03 2023, max compression
+gzip compressed data, was "pytest-embedded-qemu-1.3.1.tar", last modified: Tue Jun  6 08:56:26 2023, max compression
```

## Comparing `pytest-embedded-qemu-1.3.0.tar` & `pytest-embedded-qemu-1.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:09:03.000000 pytest-embedded-qemu-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-31 13:09:03.000000 pytest-embedded-qemu-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-31 13:08:52.000000 pytest-embedded-qemu-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:09:03.000000 pytest-embedded-qemu-1.3.0/pytest_embedded_qemu/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-31 13:08:52.000000 pytest-embedded-qemu-1.3.0/pytest_embedded_qemu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-31 13:08:52.000000 pytest-embedded-qemu-1.3.0/pytest_embedded_qemu/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-31 13:08:52.000000 pytest-embedded-qemu-1.3.0/pytest_embedded_qemu/dut.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-31 13:08:52.000000 pytest-embedded-qemu-1.3.0/pytest_embedded_qemu/qemu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 13:09:03.000000 pytest-embedded-qemu-1.3.0/pytest_embedded_qemu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-31 13:09:03.000000 pytest-embedded-qemu-1.3.0/pytest_embedded_qemu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-31 13:09:03.000000 pytest-embedded-qemu-1.3.0/pytest_embedded_qemu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 13:09:03.000000 pytest-embedded-qemu-1.3.0/pytest_embedded_qemu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-31 13:09:03.000000 pytest-embedded-qemu-1.3.0/pytest_embedded_qemu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-31 13:09:03.000000 pytest-embedded-qemu-1.3.0/pytest_embedded_qemu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 13:09:03.000000 pytest-embedded-qemu-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-31 13:08:52.000000 pytest-embedded-qemu-1.3.0/setup.py
+drwxr-xr-x   0 fuhanxi   (1000) fuhanxi   (1000)        0 2023-06-06 08:56:26.382211 pytest-embedded-qemu-1.3.1/
+-rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)     1580 2023-06-06 08:56:26.382211 pytest-embedded-qemu-1.3.1/PKG-INFO
+-rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)      552 2023-06-06 08:04:34.000000 pytest-embedded-qemu-1.3.1/README.md
+drwxr-xr-x   0 fuhanxi   (1000) fuhanxi   (1000)        0 2023-06-06 08:56:26.382211 pytest-embedded-qemu-1.3.1/pytest_embedded_qemu/
+-rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)      295 2023-05-10 06:49:19.000000 pytest-embedded-qemu-1.3.1/pytest_embedded_qemu/__init__.py
+-rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)     3335 2023-06-02 06:32:41.000000 pytest-embedded-qemu-1.3.1/pytest_embedded_qemu/app.py
+-rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)      414 2023-06-02 06:32:41.000000 pytest-embedded-qemu-1.3.1/pytest_embedded_qemu/dut.py
+-rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)     2388 2023-06-02 06:32:41.000000 pytest-embedded-qemu-1.3.1/pytest_embedded_qemu/qemu.py
+drwxr-xr-x   0 fuhanxi   (1000) fuhanxi   (1000)        0 2023-06-06 08:56:26.382211 pytest-embedded-qemu-1.3.1/pytest_embedded_qemu.egg-info/
+-rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)     1580 2023-06-06 08:56:26.000000 pytest-embedded-qemu-1.3.1/pytest_embedded_qemu.egg-info/PKG-INFO
+-rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)      355 2023-06-06 08:56:26.000000 pytest-embedded-qemu-1.3.1/pytest_embedded_qemu.egg-info/SOURCES.txt
+-rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)        1 2023-06-06 08:56:26.000000 pytest-embedded-qemu-1.3.1/pytest_embedded_qemu.egg-info/dependency_links.txt
+-rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)       57 2023-06-06 08:56:26.000000 pytest-embedded-qemu-1.3.1/pytest_embedded_qemu.egg-info/requires.txt
+-rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)       21 2023-06-06 08:56:26.000000 pytest-embedded-qemu-1.3.1/pytest_embedded_qemu.egg-info/top_level.txt
+-rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)       38 2023-06-06 08:56:26.382211 pytest-embedded-qemu-1.3.1/setup.cfg
+-rw-r--r--   0 fuhanxi   (1000) fuhanxi   (1000)     1885 2023-06-06 08:49:39.000000 pytest-embedded-qemu-1.3.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pytest-embedded-qemu-1.3.0/PKG-INFO` & `pytest-embedded-qemu-1.3.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,46 @@
 Metadata-Version: 2.1
 Name: pytest-embedded-qemu
-Version: 1.3.0
+Version: 1.3.1
 Summary: pytest embedded plugin for qemu, not target chip
 Home-page: https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Author: Fu Hanxi
 Author-email: fuhanxi@espressif.com
 License: MIT
-Description: ### pytest-embedded-qemu
-        
-        pytest embedded service for running tests on QEMU instead of the real target.
-        
-        Extra Functionalities:
-        
-        === "`pytest-embedded-idf` activated"
-        
-            - `app`: create the qemu bootable image automatically by the built binaries.
-            - `qemu`: enable the fixture
-            - `dut`: duplicate the `qemu` output to `pexpect_proc`.
-        
-        === "`pytest-embedded-idf` NOT activated"
-        
-            - `qemu`: enable the fixture
-            - `dut`: duplicate the `qemu` output to `pexpect_proc`.
-        
-        Used CLI Options:
-        
-        - `qemu-image-path`
-        - `qemu-prog-path`
-        - `qemu-cli-args`
-        - `qemu-cli-extra-args`
-        - `qemu-log-path`
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
 Provides-Extra: idf
+
+### pytest-embedded-qemu
+
+pytest embedded service for running tests on QEMU instead of the real target.
+
+Extra Functionalities:
+
+```{eval-rst}
+.. tabs::
+
+   .. group-tab:: `pytest-embedded-idf` activated
+
+        - `app`: create the qemu bootable image automatically by the built binaries.
+        - `qemu`: enable the fixture
+        - `dut`: duplicate the `qemu` output to `pexpect_proc`.
+
+   .. group-tab:: `pytest-embedded-idf` NOT activated
+
+        - `qemu`: enable the fixture
+        - `dut`: duplicate the `qemu` output to `pexpect_proc`.
+```
```

### Comparing `pytest-embedded-qemu-1.3.0/README.md` & `pytest-embedded-qemu-1.3.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 ### pytest-embedded-qemu
 
 pytest embedded service for running tests on QEMU instead of the real target.
 
 Extra Functionalities:
 
-=== "`pytest-embedded-idf` activated"
+```{eval-rst}
+.. tabs::
 
-    - `app`: create the qemu bootable image automatically by the built binaries.
-    - `qemu`: enable the fixture
-    - `dut`: duplicate the `qemu` output to `pexpect_proc`.
+   .. group-tab:: `pytest-embedded-idf` activated
 
-=== "`pytest-embedded-idf` NOT activated"
+        - `app`: create the qemu bootable image automatically by the built binaries.
+        - `qemu`: enable the fixture
+        - `dut`: duplicate the `qemu` output to `pexpect_proc`.
 
-    - `qemu`: enable the fixture
-    - `dut`: duplicate the `qemu` output to `pexpect_proc`.
+   .. group-tab:: `pytest-embedded-idf` NOT activated
 
-Used CLI Options:
-
-- `qemu-image-path`
-- `qemu-prog-path`
-- `qemu-cli-args`
-- `qemu-cli-extra-args`
-- `qemu-log-path`
+        - `qemu`: enable the fixture
+        - `dut`: duplicate the `qemu` output to `pexpect_proc`.
+```
```

### Comparing `pytest-embedded-qemu-1.3.0/pytest_embedded_qemu/app.py` & `pytest-embedded-qemu-1.3.1/pytest_embedded_qemu/app.py`

 * *Files identical despite different names*

### Comparing `pytest-embedded-qemu-1.3.0/pytest_embedded_qemu/qemu.py` & `pytest-embedded-qemu-1.3.1/pytest_embedded_qemu/qemu.py`

 * *Files identical despite different names*

### Comparing `pytest-embedded-qemu-1.3.0/pytest_embedded_qemu.egg-info/PKG-INFO` & `pytest-embedded-qemu-1.3.1/pytest_embedded_qemu.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,46 @@
 Metadata-Version: 2.1
 Name: pytest-embedded-qemu
-Version: 1.3.0
+Version: 1.3.1
 Summary: pytest embedded plugin for qemu, not target chip
 Home-page: https://docs.espressif.com/projects/pytest-embedded/en/latest/
 Author: Fu Hanxi
 Author-email: fuhanxi@espressif.com
 License: MIT
-Description: ### pytest-embedded-qemu
-        
-        pytest embedded service for running tests on QEMU instead of the real target.
-        
-        Extra Functionalities:
-        
-        === "`pytest-embedded-idf` activated"
-        
-            - `app`: create the qemu bootable image automatically by the built binaries.
-            - `qemu`: enable the fixture
-            - `dut`: duplicate the `qemu` output to `pexpect_proc`.
-        
-        === "`pytest-embedded-idf` NOT activated"
-        
-            - `qemu`: enable the fixture
-            - `dut`: duplicate the `qemu` output to `pexpect_proc`.
-        
-        Used CLI Options:
-        
-        - `qemu-image-path`
-        - `qemu-prog-path`
-        - `qemu-cli-args`
-        - `qemu-cli-extra-args`
-        - `qemu-log-path`
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
 Provides-Extra: idf
+
+### pytest-embedded-qemu
+
+pytest embedded service for running tests on QEMU instead of the real target.
+
+Extra Functionalities:
+
+```{eval-rst}
+.. tabs::
+
+   .. group-tab:: `pytest-embedded-idf` activated
+
+        - `app`: create the qemu bootable image automatically by the built binaries.
+        - `qemu`: enable the fixture
+        - `dut`: duplicate the `qemu` output to `pexpect_proc`.
+
+   .. group-tab:: `pytest-embedded-idf` NOT activated
+
+        - `qemu`: enable the fixture
+        - `dut`: duplicate the `qemu` output to `pexpect_proc`.
+```
```

### Comparing `pytest-embedded-qemu-1.3.0/setup.py` & `pytest-embedded-qemu-1.3.1/setup.py`

 * *Files 6% similar despite different names*

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

