# Comparing `tmp/python_flirt-0.8.6-cp39-none-win_amd64.whl.zip` & `tmp/python_flirt-0.8.7-cp37-none-win32.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 211996 bytes, number of entries: 6
--rw-r--r--  4.6 unx     7762 b- defN 22-Dec-13 12:56 python_flirt-0.8.6.dist-info/METADATA
--rw-r--r--  4.6 unx       95 b- defN 22-Dec-13 12:56 python_flirt-0.8.6.dist-info/WHEEL
--rw-r--r--  4.6 unx    11551 b- defN 22-Dec-13 12:56 python_flirt-0.8.6.dist-info/license_files/LICENSE.txt
--rw-r--r--  4.6 unx      103 b- defN 22-Dec-13 12:56 flirt/__init__.py
--rwxr-xr-x  4.6 unx   445952 b- defN 22-Dec-13 12:56 flirt/flirt.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      495 b- defN 22-Dec-13 12:56 python_flirt-0.8.6.dist-info/RECORD
-6 files, 465958 bytes uncompressed, 211104 bytes compressed:  54.7%
+Zip file size: 197690 bytes, number of entries: 6
+-rw-r--r--  4.6 unx     7760 b- defN 23-Jun-06 13:53 python_flirt-0.8.7.dist-info/METADATA
+-rw-r--r--  4.6 unx       91 b- defN 23-Jun-06 13:53 python_flirt-0.8.7.dist-info/WHEEL
+-rw-r--r--  4.6 unx    11551 b- defN 23-Jun-06 13:53 python_flirt-0.8.7.dist-info/license_files/LICENSE.txt
+-rw-r--r--  4.6 unx      103 b- defN 23-Jun-06 13:53 flirt/__init__.py
+-rwxr-xr-x  4.6 unx   377856 b- defN 23-Jun-06 13:53 flirt/flirt.pyd
+-rw-r--r--  4.6 unx      480 b- defN 23-Jun-06 13:53 python_flirt-0.8.7.dist-info/RECORD
+6 files, 397841 bytes uncompressed, 196828 bytes compressed:  50.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: python_flirt-0.8.6.dist-info/METADATA
+Filename: python_flirt-0.8.7.dist-info/METADATA
 Comment: 
 
-Filename: python_flirt-0.8.6.dist-info/WHEEL
+Filename: python_flirt-0.8.7.dist-info/WHEEL
 Comment: 
 
-Filename: python_flirt-0.8.6.dist-info/license_files/LICENSE.txt
+Filename: python_flirt-0.8.7.dist-info/license_files/LICENSE.txt
 Comment: 
 
 Filename: flirt/__init__.py
 Comment: 
 
-Filename: flirt/flirt.cp39-win_amd64.pyd
+Filename: flirt/flirt.pyd
 Comment: 
 
-Filename: python_flirt-0.8.6.dist-info/RECORD
+Filename: python_flirt-0.8.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `python_flirt-0.8.6.dist-info/METADATA` & `python_flirt-0.8.7.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-flirt
-Version: 0.8.6
+Version: 0.8.7
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Disassemblers
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Rust
@@ -58,17 +58,17 @@
 ```python
 import flirt
 
 BUF = bytes([
     # utcutil.dll
     #  MD5 abc9ea116498feb8f1de45f60d595af6
     #  SHA-1 2f1ba350237b74c454caf816b7410490f5994c59
-    #  SHA-256 7607897638e9dae406f0840dbae68e879c3bb2f08da350c6734e4e2ef8d61ac2 
+    #  SHA-256 7607897638e9dae406f0840dbae68e879c3bb2f08da350c6734e4e2ef8d61ac2
     # __EH_prolog3_catch_align
-    
+
     0x51,0x8b,0x4c,0x24,0x0c,0x89,0x5c,0x24,0x0c,0x8d,0x5c,0x24,0x0c,0x50,0x8d,0x44,
     0x24,0x08,0xf7,0xd9,0x23,0xc1,0x8d,0x60,0xf8,0x8b,0x43,0xf0,0x89,0x04,0x24,0x8b,
     0x43,0xf8,0x50,0x8b,0x43,0xfc,0x8b,0x4b,0xf4,0x89,0x6c,0x24,0x0c,0x8d,0x6c,0x24,
     0x0c,0xc7,0x44,0x24,0x08,0xff,0xff,0xff,0xff,0x51,0x53,0x2b,0xe0,0x56,0x57,0xa1,
     0x70,0x14,0x01,0x10,0x33,0xc5,0x50,0x89,0x65,0xf0,0x8b,0x43,0x04,0x89,0x45,0x04,
     0xff,0x75,0xf4,0x64,0xa1,0x00,0x00,0x00,0x00,0x89,0x45,0xf4,0x8d,0x45,0xf4,0x64,
     0xa3,0x00,0x00,0x00,0x00,0xf2,0xc3
@@ -90,15 +90,15 @@
 matcher = flirt.compile(sigs)
 
 # match the signatures against the given buffer, starting at offset 0.
 # results in a list of rule instances with a field `name` tuple like:
 #
 #     ("__EH_prolog3_catch_align", "public", 0)
 for m in matcher.match(BUF):
-    print("match: " + m.names[0])
+    print(f"match: {m.names[0][0]}")
 ```
 
 expected output:
 
 ```
 match: __EH_prolog3_catch_align
 ```
```

## Comparing `python_flirt-0.8.6.dist-info/license_files/LICENSE.txt` & `python_flirt-0.8.7.dist-info/license_files/LICENSE.txt`

 * *Files identical despite different names*

