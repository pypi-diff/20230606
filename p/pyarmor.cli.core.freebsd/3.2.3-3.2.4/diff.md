# Comparing `tmp/pyarmor.cli.core.freebsd-3.2.3-cp39-none-any.whl.zip` & `tmp/pyarmor.cli.core.freebsd-3.2.4-cp39-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,9 @@
-Zip file size: 709019 bytes, number of entries: 6
--rwxr-xr-x  2.0 unx   684272 b- defN 23-Jun-05 05:57 pyarmor/cli/core/freebsd/x86_64/pyarmor_runtime.so
--rwxr-xr-x  2.0 unx   743024 b- defN 23-Jun-05 05:57 pyarmor/cli/core/freebsd/x86_64/pytransform3.so
--rw-r--r--  2.0 unx      773 b- defN 23-Jun-05 05:57 pyarmor.cli.core.freebsd-3.2.3.dist-info/METADATA
--rw-r--r--  2.0 unx       93 b- defN 23-Jun-05 05:57 pyarmor.cli.core.freebsd-3.2.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jun-05 05:57 pyarmor.cli.core.freebsd-3.2.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      579 b- defN 23-Jun-05 05:57 pyarmor.cli.core.freebsd-3.2.3.dist-info/RECORD
-6 files, 1428749 bytes uncompressed, 707955 bytes compressed:  50.4%
+Zip file size: 709239 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-06 05:21 pyarmor/cli/core/freebsd/__init__.py
+-rwxr-xr-x  2.0 unx   684272 b- defN 23-Jun-06 05:21 pyarmor/cli/core/freebsd/x86_64/pyarmor_runtime.so
+-rwxr-xr-x  2.0 unx   743024 b- defN 23-Jun-06 05:21 pyarmor/cli/core/freebsd/x86_64/pytransform3.so
+-rw-r--r--  2.0 unx      773 b- defN 23-Jun-06 05:21 pyarmor.cli.core.freebsd-3.2.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       93 b- defN 23-Jun-06 05:21 pyarmor.cli.core.freebsd-3.2.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-06 05:21 pyarmor.cli.core.freebsd-3.2.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      670 b- defN 23-Jun-06 05:21 pyarmor.cli.core.freebsd-3.2.4.dist-info/RECORD
+7 files, 1428862 bytes uncompressed, 708027 bytes compressed:  50.4%
```

## zipnote {}

```diff
@@ -1,19 +1,22 @@
+Filename: pyarmor/cli/core/freebsd/__init__.py
+Comment: 
+
 Filename: pyarmor/cli/core/freebsd/x86_64/pyarmor_runtime.so
 Comment: 
 
 Filename: pyarmor/cli/core/freebsd/x86_64/pytransform3.so
 Comment: 
 
-Filename: pyarmor.cli.core.freebsd-3.2.3.dist-info/METADATA
+Filename: pyarmor.cli.core.freebsd-3.2.4.dist-info/METADATA
 Comment: 
 
-Filename: pyarmor.cli.core.freebsd-3.2.3.dist-info/WHEEL
+Filename: pyarmor.cli.core.freebsd-3.2.4.dist-info/WHEEL
 Comment: 
 
-Filename: pyarmor.cli.core.freebsd-3.2.3.dist-info/top_level.txt
+Filename: pyarmor.cli.core.freebsd-3.2.4.dist-info/top_level.txt
 Comment: 
 
-Filename: pyarmor.cli.core.freebsd-3.2.3.dist-info/RECORD
+Filename: pyarmor.cli.core.freebsd-3.2.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pyarmor.cli.core.freebsd-3.2.3.dist-info/METADATA` & `pyarmor.cli.core.freebsd-3.2.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyarmor.cli.core.freebsd
-Version: 3.2.3
+Version: 3.2.4
 Summary: Provide extension module pytransform3 for Pyarmor
 Home-page: https://github.com/dashingsoft/pyarmor
 Author: Jondy Zhao
 Author-email: pyarmor@163.com
 License: Free To Use But Restricted
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `pyarmor.cli.core.freebsd-3.2.3.dist-info/RECORD` & `pyarmor.cli.core.freebsd-3.2.4.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,6 +1,7 @@
+pyarmor/cli/core/freebsd/__init__.py,sha256=i0qFbMNWvhebNbg445IUw_soDao0BpkSqsustwfRQ1M,22
 pyarmor/cli/core/freebsd/x86_64/pyarmor_runtime.so,sha256=nunUQQ0Orobpgfd_1kGVz8HIdrZCfaaJX_Nbj0X-bB8,684272
 pyarmor/cli/core/freebsd/x86_64/pytransform3.so,sha256=k6Bnat_Y5p4YmQ0xskiL_skBJcfx1y1HDBXVUUXSyxw,743024
-pyarmor.cli.core.freebsd-3.2.3.dist-info/METADATA,sha256=wc5_wzz7IcyPQzGY4Dk3wcUxpWN8NZ143rcz_gC7unk,773
-pyarmor.cli.core.freebsd-3.2.3.dist-info/WHEEL,sha256=QbbyyBnlPXzoGKd-349G69XkCwSd1NFnt4kuAN58gNs,93
-pyarmor.cli.core.freebsd-3.2.3.dist-info/top_level.txt,sha256=UE1ovZ_90YzwF_lZ3LV7o8HKLe-RgzUaUUvdH5UTUus,8
-pyarmor.cli.core.freebsd-3.2.3.dist-info/RECORD,,
+pyarmor.cli.core.freebsd-3.2.4.dist-info/METADATA,sha256=GFN66Xy_DBdywh_sWSJTGmarwkn1CawMw9kJGs27WGI,773
+pyarmor.cli.core.freebsd-3.2.4.dist-info/WHEEL,sha256=QbbyyBnlPXzoGKd-349G69XkCwSd1NFnt4kuAN58gNs,93
+pyarmor.cli.core.freebsd-3.2.4.dist-info/top_level.txt,sha256=UE1ovZ_90YzwF_lZ3LV7o8HKLe-RgzUaUUvdH5UTUus,8
+pyarmor.cli.core.freebsd-3.2.4.dist-info/RECORD,,
```

