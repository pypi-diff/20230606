# Comparing `tmp/pyipatcher-1.0.5.tar.gz` & `tmp/pyipatcher-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyipatcher-1.0.5.tar", max compression
+gzip compressed data, was "pyipatcher-1.0.6.tar", max compression
```

## Comparing `pyipatcher-1.0.5.tar` & `pyipatcher-1.0.6.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0    35149 2023-01-21 18:12:04.952658 pyipatcher-1.0.5/LICENSE
--rw-r--r--   0        0        0      991 2023-01-22 15:55:31.045107 pyipatcher-1.0.5/README.md
--rw-r--r--   0        0        0      173 2023-01-21 18:12:04.954768 pyipatcher-1.0.5/pyipatcher/__init__.py
--rw-r--r--   0        0        0      334 2023-01-21 18:12:04.955147 pyipatcher-1.0.5/pyipatcher/__main__.py
--rw-r--r--   0        0        0     2229 2023-01-22 15:40:24.344856 pyipatcher-1.0.5/pyipatcher/cli/kernelpatcher.py
--rw-r--r--   0        0        0     1588 2023-01-22 16:06:48.774489 pyipatcher-1.0.5/pyipatcher/cli/ramdiskpatcher.py
--rw-r--r--   0        0        0     1107 2023-01-22 10:05:39.128257 pyipatcher-1.0.5/pyipatcher/logger.py
--rw-r--r--   0        0        0     1455 2023-01-22 16:05:29.884437 pyipatcher-1.0.5/pyipatcher/patchfinder/asrpatchfinder.py
--rw-r--r--   0        0        0     3184 2023-01-22 15:36:57.104765 pyipatcher-1.0.5/pyipatcher/patchfinder/ibootpatchfinder.py
--rwxr-xr-x   0        0        0     6238 2023-01-22 15:52:50.492114 pyipatcher-1.0.5/pyipatcher/patchfinder/kernelpatchfinder.py
--rw-r--r--   0        0        0     4707 2023-01-22 16:10:42.903531 pyipatcher-1.0.5/pyipatcher/patchfinder/patchfinder64.py
--rw-r--r--   0        0        0     2024 2023-01-22 16:20:49.590354 pyipatcher-1.0.5/pyipatcher/patchfinder/rextpatchfinder.py
--rw-r--r--   0        0        0      892 2023-01-22 16:21:42.253588 pyipatcher-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     1893 1970-01-01 00:00:00.000000 pyipatcher-1.0.5/setup.py
--rw-r--r--   0        0        0     1893 1970-01-01 00:00:00.000000 pyipatcher-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-01-21 18:12:04.000000 pyipatcher-1.0.6/LICENSE
+-rw-r--r--   0        0        0     1002 2023-01-22 16:23:12.000000 pyipatcher-1.0.6/README.md
+-rw-r--r--   0        0        0      173 2023-01-21 18:12:04.000000 pyipatcher-1.0.6/pyipatcher/__init__.py
+-rw-r--r--   0        0        0      272 2023-06-06 04:42:59.642132 pyipatcher-1.0.6/pyipatcher/__main__.py
+-rw-r--r--   0        0        0     2217 2023-06-06 04:51:58.874729 pyipatcher-1.0.6/pyipatcher/cli/ibootpatcher.py
+-rw-r--r--   0        0        0     2229 2023-01-22 15:40:24.000000 pyipatcher-1.0.6/pyipatcher/cli/kernelpatcher.py
+-rw-r--r--   0        0        0     1588 2023-01-22 16:06:48.000000 pyipatcher-1.0.6/pyipatcher/cli/ramdiskpatcher.py
+-rw-r--r--   0        0        0     1140 2023-01-29 13:19:23.000000 pyipatcher-1.0.6/pyipatcher/logger.py
+-rw-r--r--   0        0        0     1455 2023-01-22 16:05:29.000000 pyipatcher-1.0.6/pyipatcher/patchfinder/asrpatchfinder.py
+-rw-r--r--   0        0        0    20092 2023-06-06 04:26:00.166826 pyipatcher-1.0.6/pyipatcher/patchfinder/ibootpatchfinder.py
+-rw-r--r--   0        0        0     6116 2023-02-23 03:14:47.000000 pyipatcher-1.0.6/pyipatcher/patchfinder/insn.py
+-rwxr-xr-x   0        0        0     6238 2023-01-22 15:52:50.000000 pyipatcher-1.0.6/pyipatcher/patchfinder/kernelpatchfinder.py
+-rw-r--r--   0        0        0     5541 2023-02-08 15:02:31.000000 pyipatcher-1.0.6/pyipatcher/patchfinder/patchfinder64.py
+-rw-r--r--   0        0        0     2024 2023-01-22 16:20:49.000000 pyipatcher-1.0.6/pyipatcher/patchfinder/rextpatchfinder.py
+-rw-r--r--   0        0        0      892 2023-06-06 06:23:09.521876 pyipatcher-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1904 1970-01-01 00:00:00.000000 pyipatcher-1.0.6/PKG-INFO
```

### Comparing `pyipatcher-1.0.5/LICENSE` & `pyipatcher-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyipatcher-1.0.5/README.md` & `pyipatcher-1.0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Incomplete iOS bootchain patchers in Python
 ## Notes
 * ~~It will be pushed to pip as a package later~~
 * You can now install it locally (see Installation)
 * patchfinder64 is ported from [xerub's patchfinder](https://github.com/xerub/patchfinder64)
 * kernelpatcher is ported from [palera1n team's fork of Kernel64Patcher](https://github.com/palera1n/Kernel64Patcher)
 ## Installation
-* Install from PyPI:
+* Install from PyPI (bug-free):
 ```
 python3 -m pip install pyipatcher
 ```
 * Install locally (receive updates more often):
 ```
 git clone https://github.com/Mini-Exploit/pyipatcher
 cd pyipatcher
```

### Comparing `pyipatcher-1.0.5/pyipatcher/cli/kernelpatcher.py` & `pyipatcher-1.0.6/pyipatcher/cli/kernelpatcher.py`

 * *Files identical despite different names*

### Comparing `pyipatcher-1.0.5/pyipatcher/cli/ramdiskpatcher.py` & `pyipatcher-1.0.6/pyipatcher/cli/ramdiskpatcher.py`

 * *Files identical despite different names*

### Comparing `pyipatcher-1.0.5/pyipatcher/logger.py` & `pyipatcher-1.0.6/pyipatcher/logger.py`

 * *Files 25% similar despite different names*

```diff
@@ -19,16 +19,16 @@
     }
 
     def format(self, record):
         log_fmt = self.FORMATS.get(record.levelno)
         formatter = logging.Formatter(log_fmt)
         return formatter.format(record)
 
-def get_my_logger(verbose):
-    logger = logging.getLogger(inspect.stack()[1][3])
+def get_my_logger(verbose, name=None):
+    logger = logging.getLogger(inspect.stack()[1][3] if not name else name)
     logger.setLevel(logging.DEBUG)
     ch = logging.StreamHandler()
     if verbose:
         ch.setLevel(logging.DEBUG)
     else:
         ch.setLevel(logging.INFO)
     ch.setFormatter(MyFormatter())
```

### Comparing `pyipatcher-1.0.5/pyipatcher/patchfinder/asrpatchfinder.py` & `pyipatcher-1.0.6/pyipatcher/patchfinder/asrpatchfinder.py`

 * *Files identical despite different names*

### Comparing `pyipatcher-1.0.5/pyipatcher/patchfinder/kernelpatchfinder.py` & `pyipatcher-1.0.6/pyipatcher/patchfinder/kernelpatchfinder.py`

 * *Files identical despite different names*

### Comparing `pyipatcher-1.0.5/pyipatcher/patchfinder/patchfinder64.py` & `pyipatcher-1.0.6/pyipatcher/patchfinder/patchfinder64.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,62 +1,74 @@
 import struct
 import ctypes
 import sys
+import binascii
 
 def BIT_RANGE(v, begin, end):   return (v >> begin) % (1 << (end - begin + 1))
 def BIT_AT(v, pos): return (v >> pos) % 2
 def SET_BITS(v, begin): return v << begin
 
-
 def arm64_branch_instruction(_from, to):
     _from = ctypes.c_ulonglong(_from).value
     to = ctypes.c_ulonglong(to).value
     return ctypes.c_uint(int(0x18000000 - (_from - to) / 4 if _from > to else 0x14000000 + (to - _from) / 4)).value
 
 class patchfinder64:
     def __init__(self, buf):
         self._buf = bytearray(buf)
         self.size = len(buf)
         if self.size % 4 != 0:
             raise Exception('arm64 file size not divisible by 4')
 
-    def memmem(self, needle, end=False):
+    def memmem(self, needle, start_loc=0, end=False):
         if end:
-            return self._buf.find(needle)+len(needle)
+            return self._buf.find(needle, start_loc, self.size)+len(needle)
         else:
-            return self._buf.find(needle)
+            return self._buf.find(needle, start_loc, self.size)
 
     def get_str(self, start, size, end=False):
-        where = self.memmem(start, end)
+        where = self.memmem(start, end=end)
         return self._buf[where:where+size]
 
     def get_insn(self, where):
         if self.size - where < 4:
             raise Exception('offset reached end of file')
         return struct.unpack("<I", self._buf[where:where+4])[0]
-        
+
+    def get_ptr_loc(self, where):
+        if self.size - where < 8:
+            raise Exception('offset reached end of file')
+        return struct.unpack("<Q", self._buf[where:where+8])[0]
+
     def step(self, start, length, what, mask):
         end = start + length
         while start < end:
             x = struct.unpack("<I", self._buf[start:start+4])[0]
             if (x & mask) == what:
                 return start
             start += 4
         return 0
      
-    def step_back(self, start, length, what, mask):
+    def step_back(self, start, length, what, mask, reversed=False):
         end = start - length
         while start >= end:
             x = struct.unpack("<I", self._buf[start:start+4])[0]
-            if (x & mask) == what:
-                return start
-            start -= 4
+            if not reversed:
+                if (x & mask) == what:
+                    return start
+                start -= 4
+            else:
+                if (x & mask) == what:
+                    start -= 4
+                else:
+                    return start
         return 0
 
-    def bof(self, start, where):
+    def bof(self, where):
+        start = 0
         while where >= start:
             op = struct.unpack("<I", self._buf[where:where+4])[0]
             if (op & 0xFFC003FF) == 0x910003FD:
                 delta = (op >> 10) & 0xFFF
                 if (delta & 0xF) == 0:
                     prev = where - ((delta >> 4) + 1) * 4
                     au = struct.unpack("<I", self._buf[prev:prev+4])[0]
@@ -111,14 +123,24 @@
                 value[reg] = ctypes.c_ulonglong((adr >> 11) + i).value
             elif (op & 0xFF000000) == 0x58000000:
                 value[reg] = adr + i
             if value[reg] == what:
                 return i
         return 0
 
+    def xrefcode(self, what, start=0, end=0):
+        end = self.size & ~3 if not end else end & ~3
+        for i in range(0, end, 4):
+            op = struct.unpack("<I", self._buf[i:i+4])[0]
+            if op & 0x7C000000 == 0x14000000:
+                where = self.follow_call(i)
+                if where == what:
+                    return i
+        return 0
+
     def apply_patch(self, where, patch):
         self._buf[where:where+len(patch)] = patch
 
 
 def test():
     set_package_name("test")
     kernel = open("kcache.raw", "rb").read()
```

### Comparing `pyipatcher-1.0.5/pyipatcher/patchfinder/rextpatchfinder.py` & `pyipatcher-1.0.6/pyipatcher/patchfinder/rextpatchfinder.py`

 * *Files identical despite different names*

### Comparing `pyipatcher-1.0.5/pyproject.toml` & `pyipatcher-1.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyipatcher"
-version = "1.0.5"
+version = "1.0.6"
 description = "iOS ARM64 patchfinder & iOS ARM64 bootchain patcher"
 authors = ["mini_exploit <61931266+Mini-Exploit@users.noreply.github.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/Mini-Exploit/pyipatcher"
 
 [tool.poetry.dependencies]
```

### Comparing `pyipatcher-1.0.5/PKG-INFO` & `pyipatcher-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyipatcher
-Version: 1.0.5
+Version: 1.0.6
 Summary: iOS ARM64 patchfinder & iOS ARM64 bootchain patcher
 Home-page: https://github.com/Mini-Exploit/pyipatcher
 License: GPL-3.0-only
 Author: mini_exploit
 Author-email: 61931266+Mini-Exploit@users.noreply.github.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -23,15 +23,15 @@
 Incomplete iOS bootchain patchers in Python
 ## Notes
 * ~~It will be pushed to pip as a package later~~
 * You can now install it locally (see Installation)
 * patchfinder64 is ported from [xerub's patchfinder](https://github.com/xerub/patchfinder64)
 * kernelpatcher is ported from [palera1n team's fork of Kernel64Patcher](https://github.com/palera1n/Kernel64Patcher)
 ## Installation
-* Install from PyPI:
+* Install from PyPI (bug-free):
 ```
 python3 -m pip install pyipatcher
 ```
 * Install locally (receive updates more often):
 ```
 git clone https://github.com/Mini-Exploit/pyipatcher
 cd pyipatcher
```

