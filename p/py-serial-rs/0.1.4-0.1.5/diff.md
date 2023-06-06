# Comparing `tmp/py_serial_rs-0.1.4.tar.gz` & `tmp/py_serial_rs-0.1.5.tar.gz`

## Comparing `py_serial_rs-0.1.4.tar` & `py_serial_rs-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,28 @@
--rw-r--r--   0        0        0      305 1970-01-01 00:00:00.000000 py_serial_rs-0.1.4/Cargo.toml
--rw-r--r--   0     1000     1000       88 2023-05-22 21:12:11.000000 py_serial_rs-0.1.4/.envrc
--rw-r--r--   0     1000     1000      413 2023-05-20 07:54:26.000000 py_serial_rs-0.1.4/.github/workflows/rust.yml
--rw-r--r--   0     1000     1000      694 2023-05-25 20:55:00.000000 py_serial_rs-0.1.4/.gitignore
--rw-r--r--   0     1000     1000      684 2023-05-25 21:39:49.000000 py_serial_rs-0.1.4/.readthedocs.yaml
--rw-r--r--   0     1000     1000     1069 2023-05-20 07:54:26.000000 py_serial_rs-0.1.4/LICENSE
--rw-r--r--   0     1000     1000     1573 2023-05-26 20:20:31.000000 py_serial_rs-0.1.4/Readme.rst
--rw-r--r--   0     1000     1000      638 2023-05-21 08:31:33.000000 py_serial_rs-0.1.4/docs/Makefile
--rw-r--r--   0     1000     1000      804 2023-05-21 08:31:33.000000 py_serial_rs-0.1.4/docs/make.bat
--rw-r--r--   0     1000     1000     1330 2023-05-25 21:05:27.000000 py_serial_rs-0.1.4/docs/source/conf.py
--rw-r--r--   0     1000     1000     1592 2023-05-26 20:20:31.000000 py_serial_rs-0.1.4/docs/source/index.rst
--rw-r--r--   0     1000     1000      771 2023-05-26 20:20:31.000000 py_serial_rs-0.1.4/pyproject.toml
--rwxr-xr-x   0     1000     1000      872 2023-05-21 08:38:25.000000 py_serial_rs-0.1.4/python/demo.py
--rwxr-xr-x   0     1000     1000     1275 2023-05-25 20:36:59.000000 py_serial_rs-0.1.4/python/demo_threads.py
--rw-r--r--   0     1000     1000      166 2023-05-25 21:04:59.000000 py_serial_rs-0.1.4/requirements.txt
--rw-r--r--   0     1000     1000      392 2023-05-20 07:54:26.000000 py_serial_rs-0.1.4/shell.nix
--rw-r--r--   0     1000     1000     4699 2023-05-25 21:36:52.000000 py_serial_rs-0.1.4/src/lib.rs
--rw-r--r--   0     1000     1000    15416 2023-05-26 20:20:34.000000 py_serial_rs-0.1.4/Cargo.lock
--rw-r--r--   0        0        0     2229 1970-01-01 00:00:00.000000 py_serial_rs-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      305 1970-01-01 00:00:00.000000 py_serial_rs-0.1.5/Cargo.toml
+-rw-r--r--   0     1000     1000       88 2023-06-06 19:51:15.000000 py_serial_rs-0.1.5/.envrc
+-rw-r--r--   0     1000     1000      413 2023-05-20 07:54:26.000000 py_serial_rs-0.1.5/.github/workflows/rust.yml
+-rw-r--r--   0     1000     1000      694 2023-06-06 19:10:46.000000 py_serial_rs-0.1.5/.gitignore
+-rw-r--r--   0     1000     1000      684 2023-05-25 21:39:49.000000 py_serial_rs-0.1.5/.readthedocs.yaml
+-rw-r--r--   0     1000     1000       94 2023-06-06 20:00:32.000000 py_serial_rs-0.1.5/Dockerfile
+-rw-r--r--   0     1000     1000     1069 2023-05-20 07:54:26.000000 py_serial_rs-0.1.5/LICENSE
+-rw-r--r--   0     1000     1000     1573 2023-05-26 20:20:31.000000 py_serial_rs-0.1.5/Readme.rst
+-rw-r--r--   0     1000     1000     3288 2023-05-26 20:40:49.000000 py_serial_rs-0.1.5/default_12248338248752268114_0_187658.profraw
+-rw-r--r--   0     1000     1000   531960 2023-05-26 20:40:49.000000 py_serial_rs-0.1.5/default_17441304742884545305_0_187658.profraw
+-rw-r--r--   0     1000     1000   612704 2023-05-26 20:32:28.000000 py_serial_rs-0.1.5/default_8445587411051284602_0_186101.profraw
+-rw-r--r--   0     1000     1000   612704 2023-05-26 20:39:21.000000 py_serial_rs-0.1.5/default_8445587411051284602_0_186595.profraw
+-rw-r--r--   0     1000     1000   612704 2023-05-26 20:40:49.000000 py_serial_rs-0.1.5/default_8445587411051284602_0_187749.profraw
+-rwxr-xr-x   0     1000     1000       39 2023-05-26 22:47:42.000000 py_serial_rs-0.1.5/docker-build.sh
+-rwxr-xr-x   0     1000     1000       99 2023-06-06 19:58:40.000000 py_serial_rs-0.1.5/docker-run.sh
+-rw-r--r--   0     1000     1000      638 2023-05-21 08:31:33.000000 py_serial_rs-0.1.5/docs/Makefile
+-rw-r--r--   0     1000     1000      804 2023-05-21 08:31:33.000000 py_serial_rs-0.1.5/docs/make.bat
+-rw-r--r--   0     1000     1000     1330 2023-05-25 21:05:27.000000 py_serial_rs-0.1.5/docs/source/conf.py
+-rw-r--r--   0     1000     1000     1592 2023-05-26 20:20:31.000000 py_serial_rs-0.1.5/docs/source/index.rst
+-rw-r--r--   0     1000     1000   265128 2023-05-26 20:40:49.000000 py_serial_rs-0.1.5/json5format.profdata
+-rw-r--r--   0     1000     1000      771 2023-05-26 20:20:31.000000 py_serial_rs-0.1.5/pyproject.toml
+-rwxr-xr-x   0     1000     1000      872 2023-05-21 08:38:25.000000 py_serial_rs-0.1.5/python/demo.py
+-rwxr-xr-x   0     1000     1000     1275 2023-05-25 20:36:59.000000 py_serial_rs-0.1.5/python/demo_threads.py
+-rw-r--r--   0     1000     1000      176 2023-06-06 19:36:16.000000 py_serial_rs-0.1.5/requirements.txt
+-rw-r--r--   0     1000     1000      392 2023-06-06 19:35:23.000000 py_serial_rs-0.1.5/shell.nix
+-rw-r--r--   0     1000     1000     5077 2023-06-06 19:36:16.000000 py_serial_rs-0.1.5/src/lib.rs
+-rw-r--r--   0     1000     1000    15416 2023-06-06 19:36:16.000000 py_serial_rs-0.1.5/Cargo.lock
+-rw-r--r--   0        0        0     2229 1970-01-01 00:00:00.000000 py_serial_rs-0.1.5/PKG-INFO
```

### Comparing `py_serial_rs-0.1.4/.gitignore` & `py_serial_rs-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `py_serial_rs-0.1.4/.readthedocs.yaml` & `py_serial_rs-0.1.5/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `py_serial_rs-0.1.4/LICENSE` & `py_serial_rs-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `py_serial_rs-0.1.4/Readme.rst` & `py_serial_rs-0.1.5/Readme.rst`

 * *Files identical despite different names*

### Comparing `py_serial_rs-0.1.4/docs/Makefile` & `py_serial_rs-0.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `py_serial_rs-0.1.4/docs/make.bat` & `py_serial_rs-0.1.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `py_serial_rs-0.1.4/docs/source/conf.py` & `py_serial_rs-0.1.5/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `py_serial_rs-0.1.4/docs/source/index.rst` & `py_serial_rs-0.1.5/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `py_serial_rs-0.1.4/pyproject.toml` & `py_serial_rs-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py_serial_rs-0.1.4/python/demo.py` & `py_serial_rs-0.1.5/python/demo.py`

 * *Files identical despite different names*

### Comparing `py_serial_rs-0.1.4/python/demo_threads.py` & `py_serial_rs-0.1.5/python/demo_threads.py`

 * *Files identical despite different names*

### Comparing `py_serial_rs-0.1.4/src/lib.rs` & `py_serial_rs-0.1.5/src/lib.rs`

 * *Files 7% similar despite different names*

```diff
@@ -127,14 +127,24 @@
     ///     int: the number of bytes written
     fn write(&mut self, data: &[u8]) -> PyResult<usize> {
         Ok(self.serial.write(data)?)
     }
 
     /// Close the connection to the serial port (handled internally)
     fn close(&mut self) {}
+
+    /// Clear the input buffer. Any pending input will be discarded.
+    fn reset_input_buffer(&mut self) {
+        if self.serial.clear(serialport::ClearBuffer::Input).is_ok() {}
+    }
+
+    /// Clear the output buffer. Any pending output will be discarded.
+    fn reset_output_buffer(&mut self) {
+        if self.serial.clear(serialport::ClearBuffer::Output).is_ok() {}
+    }
 }
 
 #[pymodule]
 fn py_serial_rs(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_class::<PySerial>()?;
     Ok(())
 }
```

### Comparing `py_serial_rs-0.1.4/Cargo.lock` & `py_serial_rs-0.1.5/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -259,15 +259,15 @@
 checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "py_serial_rs"
-version = "0.1.4"
+version = "0.1.5"
 dependencies = [
  "clippy",
  "pyo3",
  "serialport",
  "time",
 ]
```

### Comparing `py_serial_rs-0.1.4/PKG-INFO` & `py_serial_rs-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_serial_rs
-Version: 0.1.4
+Version: 0.1.5
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Read and write data over the serial ports
 Author: Jürgen Hahn
 Author-email: mail.jhahn@googlemail.com
```

