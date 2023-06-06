# Comparing `tmp/clvm_tools_rs-0.1.8-cp37-abi3-win_amd64.whl.zip` & `tmp/clvm_tools_rs-0.1.9-cp37-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 627574 bytes, number of entries: 5
--rw-r--r--  4.6 unx     1935 b- defN 22-Apr-13 20:15 clvm_tools_rs-0.1.8.dist-info/METADATA
--rw-r--r--  4.6 unx       96 b- defN 22-Apr-13 20:15 clvm_tools_rs-0.1.8.dist-info/WHEEL
--rw-r--r--  4.6 unx       62 b- defN 22-Apr-13 20:15 clvm_tools_rs/__init__.py
--rwxr-xr-x  4.6 unx  1675776 b- defN 22-Apr-13 20:15 clvm_tools_rs/clvm_tools_rs.pyd
--rw-r--r--  4.6 unx      395 b- defN 22-Apr-13 20:15 clvm_tools_rs-0.1.8.dist-info/RECORD
-5 files, 1678264 bytes uncompressed, 626842 bytes compressed:  62.6%
+Zip file size: 699267 bytes, number of entries: 5
+-rw-r--r--  4.6 unx     2077 b- defN 22-May-03 14:08 clvm_tools_rs-0.1.9.dist-info/METADATA
+-rw-r--r--  4.6 unx       96 b- defN 22-May-03 14:08 clvm_tools_rs-0.1.9.dist-info/WHEEL
+-rw-r--r--  4.6 unx       62 b- defN 22-May-03 14:08 clvm_tools_rs/__init__.py
+-rwxr-xr-x  4.6 unx  1870336 b- defN 22-May-03 14:08 clvm_tools_rs/clvm_tools_rs.pyd
+-rw-r--r--  4.6 unx      395 b- defN 22-May-03 14:08 clvm_tools_rs-0.1.9.dist-info/RECORD
+5 files, 1872966 bytes uncompressed, 698535 bytes compressed:  62.7%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: clvm_tools_rs-0.1.8.dist-info/METADATA
+Filename: clvm_tools_rs-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: clvm_tools_rs-0.1.8.dist-info/WHEEL
+Filename: clvm_tools_rs-0.1.9.dist-info/WHEEL
 Comment: 
 
 Filename: clvm_tools_rs/__init__.py
 Comment: 
 
 Filename: clvm_tools_rs/clvm_tools_rs.pyd
 Comment: 
 
-Filename: clvm_tools_rs-0.1.8.dist-info/RECORD
+Filename: clvm_tools_rs-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `clvm_tools_rs-0.1.8.dist-info/METADATA` & `clvm_tools_rs-0.1.9.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clvm_tools_rs
-Version: 0.1.8
+Version: 0.1.9
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 clvm_tools_rs
 =
 
 This is a second-hand port of chia's [clvm tools](https://github.com/Chia-Network/clvm_tools/) to rust via the work of
 ChiaMineJP porting to typescript.  This would have been a lot harder to
@@ -41,14 +41,20 @@
                      the original chia repo.
                     
     src/compiler <-- a newer compiler (ochialisp) with a simpler
                      structure.  Select new style compilation by
                      including a `(include *standard-cl-21*)`
                      form in your toplevel `mod` form.
 
+Mac M1
+===
+
+Use ```cargo build --no-default-features``` due to differences in how mac m1 and
+other platforms handle python extensions.
+
 Use with chia-blockchain
 ===
 
     # Activate your venv, then
     $ maturin develop --release
```

