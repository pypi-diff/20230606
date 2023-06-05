# Comparing `tmp/openseespywin-3.4.0.8-py3-none-any.whl.zip` & `tmp/openseespywin-3.5.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5808569 bytes, number of entries: 8
+Zip file size: 6019946 bytes, number of entries: 8
 -rw-rw----  2.0 unx     1073 b- defN 22-Jul-18 00:07 openseespywin/LICENSE.md
--rw-r--r--  2.0 unx      762 b- defN 22-Nov-28 19:43 openseespywin/__init__.py
--rw-rw----  2.0 unx 14628352 b- defN 23-Apr-03 20:30 openseespywin/opensees.pyd
+-rw-r--r--  2.0 unx      776 b- defN 23-Jun-05 19:41 openseespywin/__init__.py
+-rwxrwxrwx  2.0 unx 15136256 b- defN 23-Jun-06 03:30 openseespywin/opensees.pyd
 -rw-r--r--  2.0 unx        0 b- defN 22-Jul-18 00:07 openseespywin/lib/__init__.py
--rw-r--r--  2.0 unx     1014 b- defN 23-Apr-15 01:55 openseespywin-3.4.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-15 01:55 openseespywin-3.4.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Apr-15 01:55 openseespywin-3.4.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      662 b- defN 23-Apr-15 01:55 openseespywin-3.4.0.8.dist-info/RECORD
-8 files, 14631969 bytes uncompressed, 5807411 bytes compressed:  60.3%
+-rw-r--r--  2.0 unx     1016 b- defN 23-Jun-05 21:57 openseespywin-3.5.1.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-05 21:57 openseespywin-3.5.1.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-Jun-05 21:57 openseespywin-3.5.1.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      662 b- defN 23-Jun-05 21:57 openseespywin-3.5.1.2.dist-info/RECORD
+8 files, 15139889 bytes uncompressed, 6018788 bytes compressed:  60.2%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: openseespywin/opensees.pyd
 Comment: 
 
 Filename: openseespywin/lib/__init__.py
 Comment: 
 
-Filename: openseespywin-3.4.0.8.dist-info/METADATA
+Filename: openseespywin-3.5.1.2.dist-info/METADATA
 Comment: 
 
-Filename: openseespywin-3.4.0.8.dist-info/WHEEL
+Filename: openseespywin-3.5.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: openseespywin-3.4.0.8.dist-info/top_level.txt
+Filename: openseespywin-3.5.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: openseespywin-3.4.0.8.dist-info/RECORD
+Filename: openseespywin-3.5.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## openseespywin/__init__.py

```diff
@@ -4,26 +4,26 @@
 # only work for 64 bit system
 if sys.maxsize < 2**31:
     raise RuntimeError('64 bit system is required')
 
 # platform dependent
 if sys.platform.startswith('win'):
 
-    if sys.version_info[0] == 3 and sys.version_info[1] == 9:
-        dll_path = ''
-        for path in sys.path:
-            if 'DLLs' in path:
-                dll_path = path
-                break
-        ctypes.cdll.LoadLibrary(dll_path + '\\tcl86t.dll')
+    if sys.version_info[0] == 3 and sys.version_info[1] == 10:
+        # dll_path = ''
+        # for path in sys.path:
+        #     if 'DLLs' in path:
+        #         dll_path = path
+        #         break
+        # ctypes.cdll.LoadLibrary(dll_path + '\\tcl86t.dll')
 
         try:
             from openseespywin.opensees import *
         except:
             raise RuntimeError('Failed to import openseespy on Windows.')
     else:
         raise RuntimeError(
-            'Python version 3.9 is needed for Windows')
+            'Python version 3.10 is needed for Windows')
 
 else:
 
     raise RuntimeError('This package is for Windows only')
```

## Comparing `openseespywin-3.4.0.8.dist-info/METADATA` & `openseespywin-3.5.1.2.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: openseespywin
-Version: 3.4.0.8
+Version: 3.5.1.2
 Summary: A OpenSeesPy Windows package
 Home-page: https://github.com/zhuminjie/openseespy
 Author: Minjie Zhu
 Author-email: zhum@oregonstate.edu
 License: LICENSE.md
 Platform: Windows
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: Microsoft :: Windows
-Requires-Python: ~= 3.9.0
+Requires-Python: ~= 3.10.0
 Description-Content-Type: text/markdown
 
 # OpenSeesPy Windows
 
 Pip Package for OpenSeesPy Windows
 
 ## Installation
```

