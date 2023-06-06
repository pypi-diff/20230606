# Comparing `tmp/mfrc522-python-0.0.5.dev3.tar.gz` & `tmp/mfrc522-python-0.0.5.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mfrc522-python-0.0.5.dev3.tar", last modified: Mon Apr 24 08:16:37 2023, max compression
+gzip compressed data, was "mfrc522-python-0.0.5.dev4.tar", last modified: Tue Apr 25 08:31:02 2023, max compression
```

## Comparing `mfrc522-python-0.0.5.dev3.tar` & `mfrc522-python-0.0.5.dev4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 08:16:37.216541 mfrc522-python-0.0.5.dev3/
--rw-rw-rw-   0        0        0    35823 2023-04-15 05:57:40.000000 mfrc522-python-0.0.5.dev3/LICENSE
--rw-rw-rw-   0        0        0     3018 2023-04-24 08:16:37.207886 mfrc522-python-0.0.5.dev3/PKG-INFO
--rw-rw-rw-   0        0        0     2433 2023-04-17 10:38:04.000000 mfrc522-python-0.0.5.dev3/README.md
--rw-rw-rw-   0        0        0      665 2023-04-24 08:15:30.000000 mfrc522-python-0.0.5.dev3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-24 08:16:37.216541 mfrc522-python-0.0.5.dev3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-24 08:16:35.339265 mfrc522-python-0.0.5.dev3/src/
-drwxrwxrwx   0        0        0        0 2023-04-24 08:16:37.158364 mfrc522-python-0.0.5.dev3/src/mfrc522/
--rw-rw-rw-   0        0        0     5688 2023-04-24 08:14:25.000000 mfrc522-python-0.0.5.dev3/src/mfrc522/BasicMFRC522.py
--rw-rw-rw-   0        0        0    22655 2023-04-17 12:07:31.000000 mfrc522-python-0.0.5.dev3/src/mfrc522/MFRC522.py
--rw-rw-rw-   0        0        0     3281 2023-04-24 08:12:53.000000 mfrc522-python-0.0.5.dev3/src/mfrc522/SimpleMFRC522.py
--rw-rw-rw-   0        0        0      130 2023-04-24 08:10:04.000000 mfrc522-python-0.0.5.dev3/src/mfrc522/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 08:16:37.207886 mfrc522-python-0.0.5.dev3/src/mfrc522_python.egg-info/
--rw-rw-rw-   0        0        0     3018 2023-04-24 08:16:35.000000 mfrc522-python-0.0.5.dev3/src/mfrc522_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2023-04-24 08:16:35.000000 mfrc522-python-0.0.5.dev3/src/mfrc522_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 08:16:35.000000 mfrc522-python-0.0.5.dev3/src/mfrc522_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-24 08:16:35.000000 mfrc522-python-0.0.5.dev3/src/mfrc522_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-25 08:31:02.557840 mfrc522-python-0.0.5.dev4/
+-rw-rw-rw-   0        0        0    35823 2023-04-15 05:57:40.000000 mfrc522-python-0.0.5.dev4/LICENSE
+-rw-rw-rw-   0        0        0     3018 2023-04-25 08:31:02.557840 mfrc522-python-0.0.5.dev4/PKG-INFO
+-rw-rw-rw-   0        0        0     2433 2023-04-17 10:38:04.000000 mfrc522-python-0.0.5.dev4/README.md
+-rw-rw-rw-   0        0        0      665 2023-04-25 08:27:56.000000 mfrc522-python-0.0.5.dev4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-25 08:31:02.557840 mfrc522-python-0.0.5.dev4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-25 08:31:02.501807 mfrc522-python-0.0.5.dev4/src/
+drwxrwxrwx   0        0        0        0 2023-04-25 08:31:02.533808 mfrc522-python-0.0.5.dev4/src/mfrc522/
+-rw-rw-rw-   0        0        0     5831 2023-04-25 08:20:53.000000 mfrc522-python-0.0.5.dev4/src/mfrc522/BasicMFRC522.py
+-rw-rw-rw-   0        0        0    22655 2023-04-17 12:07:31.000000 mfrc522-python-0.0.5.dev4/src/mfrc522/MFRC522.py
+-rw-rw-rw-   0        0        0     3294 2023-04-25 08:22:12.000000 mfrc522-python-0.0.5.dev4/src/mfrc522/SimpleMFRC522.py
+-rw-rw-rw-   0        0        0      130 2023-04-24 08:10:04.000000 mfrc522-python-0.0.5.dev4/src/mfrc522/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-25 08:31:02.557840 mfrc522-python-0.0.5.dev4/src/mfrc522_python.egg-info/
+-rw-rw-rw-   0        0        0     3018 2023-04-25 08:31:02.000000 mfrc522-python-0.0.5.dev4/src/mfrc522_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2023-04-25 08:31:02.000000 mfrc522-python-0.0.5.dev4/src/mfrc522_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-25 08:31:02.000000 mfrc522-python-0.0.5.dev4/src/mfrc522_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-25 08:31:02.000000 mfrc522-python-0.0.5.dev4/src/mfrc522_python.egg-info/top_level.txt
```

### Comparing `mfrc522-python-0.0.5.dev3/LICENSE` & `mfrc522-python-0.0.5.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `mfrc522-python-0.0.5.dev3/PKG-INFO` & `mfrc522-python-0.0.5.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfrc522-python
-Version: 0.0.5.dev3
+Version: 0.0.5.dev4
 Summary: The mfrc522 library is used to interact with RFID readers that use the MFRC522 chip
 Author: Aditya
 Project-URL: Homepage, https://github.com/1AdityaX/mfrc522-python
 Project-URL: Bug Tracker, https://github.com/1AdityaX/mfrc522-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `mfrc522-python-0.0.5.dev3/README.md` & `mfrc522-python-0.0.5.dev4/README.md`

 * *Files identical despite different names*

### Comparing `mfrc522-python-0.0.5.dev3/pyproject.toml` & `mfrc522-python-0.0.5.dev4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mfrc522-python"
-version = "0.0.5.dev3"
+version = "0.0.5.dev4"
 authors = [
   { name="Aditya"},
 ]
 description = "The mfrc522 library is used to interact with RFID readers that use the MFRC522 chip"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `mfrc522-python-0.0.5.dev3/src/mfrc522/BasicMFRC522.py` & `mfrc522-python-0.0.5.dev4/src/mfrc522/BasicMFRC522.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,14 +135,19 @@
 
     def clear_sector(self, trailer_block):
         id = self.clear_no_sector(trailer_block)
         while not id:
             id = self.clear_no_sector(trailer_block)
         return id
 
+    def clear_sectors(self, trailer_blocks=[]):
+        for i in trailer_blocks:
+            id = self.clear_sector(i)
+        return id
+
     def uid_to_num(self, uid):
         n = 0
         for i in range(0, 5):
             n = n * 256 + uid[i]
         return n
 
     def split_string(self, s):
```

### Comparing `mfrc522-python-0.0.5.dev3/src/mfrc522/MFRC522.py` & `mfrc522-python-0.0.5.dev4/src/mfrc522/MFRC522.py`

 * *Files identical despite different names*

### Comparing `mfrc522-python-0.0.5.dev3/src/mfrc522/SimpleMFRC522.py` & `mfrc522-python-0.0.5.dev4/src/mfrc522/SimpleMFRC522.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 class SimpleMFRC522:
     def __init__(self):
         self.MFRC522 = MFRC522()
         self.KEY = [0xFF, 0xFF, 0xFF, 0xFF, 0xFF, 0xFF]
         self.BLOCK_ADDRS = [8, 9, 10]
-
+    
     def read(self):
         id, text = self.read_no_block()
         while not id:
             id, text = self.read_no_block()
         return id, text
 
     def read_id(self):
@@ -40,15 +40,15 @@
         status = self.MFRC522.Authenticate(
             self.MFRC522.PICC_AUTHENT1A, 11, self.KEY, uid)
         try:
             data = []
             text_read = ''
             if status == self.MFRC522.MI_OK:
                 for block_num in self.BLOCK_ADDRS:
-                    block = self.MFRC522.Read(block_num)
+                    block = self.MFRC522.ReadTag(block_num)
                     if block:
                         data += block
                 if data:
                     text_read = ''.join(chr(i) for i in data)
             self.MFRC522.StopCrypto1()
             return id, text_read
         except:
@@ -69,22 +69,22 @@
         if status != self.MFRC522.MI_OK:
             return None, None
         id = self.uid_to_num(uid)
         self.MFRC522.SelectTag(uid)
         status = self.MFRC522.Authenticate(
             self.MFRC522.PICC_AUTHENT1A, 11, self.KEY, uid)
         try:
-            self.MFRC522.Read(11)
+            self.MFRC522.ReadTag(11)
             if status == self.MFRC522.MI_OK:
                 data = bytearray()
                 data.extend(bytearray(text.ljust(
                     len(self.BLOCK_ADDRS) * 16).encode('ascii')))
                 i = 0
                 for block_num in self.BLOCK_ADDRS:
-                    self.MFRC522.Write(block_num, data[(i*16):(i+1)*16])
+                    self.MFRC522.WriteTag(block_num, data[(i*16):(i+1)*16])
                     i += 1
             self.MFRC522.StopCrypto1()
             return id, text[0:(len(self.BLOCK_ADDRS) * 16)]
         except:
             self.MFRC522.StopCrypto1()
             return None, None
```

### Comparing `mfrc522-python-0.0.5.dev3/src/mfrc522_python.egg-info/PKG-INFO` & `mfrc522-python-0.0.5.dev4/src/mfrc522_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfrc522-python
-Version: 0.0.5.dev3
+Version: 0.0.5.dev4
 Summary: The mfrc522 library is used to interact with RFID readers that use the MFRC522 chip
 Author: Aditya
 Project-URL: Homepage, https://github.com/1AdityaX/mfrc522-python
 Project-URL: Bug Tracker, https://github.com/1AdityaX/mfrc522-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
```

