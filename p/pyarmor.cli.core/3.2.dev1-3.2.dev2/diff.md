# Comparing `tmp/pyarmor.cli.core-3.2.dev1-cp39-none-win_amd64.whl.zip` & `tmp/pyarmor.cli.core-3.2.dev2-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 660557 bytes, number of entries: 8
+Zip file size: 660831 bytes, number of entries: 8
 -rw-r--r--  2.0 unx     3857 b- defN 23-Apr-14 09:43 pyarmor/cli/core/__init__.py
 -rw-r--r--  2.0 unx     2394 b- defN 23-Apr-14 09:46 pyarmor/cli/core/fixup.py
--rwxr-xr-x  2.0 unx   611328 b- defN 23-Apr-29 01:11 pyarmor/cli/core/pyarmor_runtime.pyd
--rwxr-xr-x  2.0 unx   711168 b- defN 23-Apr-29 01:11 pyarmor/cli/core/pytransform3.pyd
--rw-r--r--  2.0 unx     1892 b- defN 23-Apr-29 01:11 pyarmor.cli.core-3.2.dev1.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Apr-29 01:11 pyarmor.cli.core-3.2.dev1.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-29 01:11 pyarmor.cli.core-3.2.dev1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      699 b- defN 23-Apr-29 01:11 pyarmor.cli.core-3.2.dev1.dist-info/RECORD
-8 files, 1331445 bytes uncompressed, 659331 bytes compressed:  50.5%
+-rwxr-xr-x  2.0 unx   611840 b- defN 23-May-01 02:25 pyarmor/cli/core/pyarmor_runtime.pyd
+-rwxr-xr-x  2.0 unx   711168 b- defN 23-May-01 02:25 pyarmor/cli/core/pytransform3.pyd
+-rw-r--r--  2.0 unx     1892 b- defN 23-May-01 02:25 pyarmor.cli.core-3.2.dev2.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-May-01 02:25 pyarmor.cli.core-3.2.dev2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-May-01 02:25 pyarmor.cli.core-3.2.dev2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      699 b- defN 23-May-01 02:25 pyarmor.cli.core-3.2.dev2.dist-info/RECORD
+8 files, 1331957 bytes uncompressed, 659605 bytes compressed:  50.5%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: pyarmor/cli/core/pyarmor_runtime.pyd
 Comment: 
 
 Filename: pyarmor/cli/core/pytransform3.pyd
 Comment: 
 
-Filename: pyarmor.cli.core-3.2.dev1.dist-info/METADATA
+Filename: pyarmor.cli.core-3.2.dev2.dist-info/METADATA
 Comment: 
 
-Filename: pyarmor.cli.core-3.2.dev1.dist-info/WHEEL
+Filename: pyarmor.cli.core-3.2.dev2.dist-info/WHEEL
 Comment: 
 
-Filename: pyarmor.cli.core-3.2.dev1.dist-info/top_level.txt
+Filename: pyarmor.cli.core-3.2.dev2.dist-info/top_level.txt
 Comment: 
 
-Filename: pyarmor.cli.core-3.2.dev1.dist-info/RECORD
+Filename: pyarmor.cli.core-3.2.dev2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pyarmor.cli.core-3.2.dev1.dist-info/METADATA` & `pyarmor.cli.core-3.2.dev2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyarmor.cli.core
-Version: 3.2.dev1
+Version: 3.2.dev2
 Summary: Provide extension module pytransform3 for Pyarmor
 Home-page: https://github.com/dashingsoft/pyarmor
 Author: Jondy Zhao
 Author-email: pyarmor@163.com
 License: Free To Use But Restricted
 Keywords: protect obfuscate encrypt obfuscation distribute
 Platform: UNKNOWN
```

## Comparing `pyarmor.cli.core-3.2.dev1.dist-info/RECORD` & `pyarmor.cli.core-3.2.dev2.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 pyarmor/cli/core/__init__.py,sha256=oEE-hBsK8-oMw5Te5qrTK87rXnr6S3ItT5WahwOJEcU,3857
 pyarmor/cli/core/fixup.py,sha256=d9lgNUr7Bo0dNSjgrA3k4kKKQhi_uDElaAIyAtIaIjE,2394
-pyarmor/cli/core/pyarmor_runtime.pyd,sha256=DgK9yT8AdpCaDhgpwDYYI9Ggnk-CnekbHh6XjcCHYts,611328
-pyarmor/cli/core/pytransform3.pyd,sha256=IxUgH4lqBEZwgRiECw9oRYdHGfV5qPdikgNdoCJ5j8Q,711168
-pyarmor.cli.core-3.2.dev1.dist-info/METADATA,sha256=NN1VTKQPsE2SHlriAklVsq9HaZfy8aRuIvPTx2WMHUg,1892
-pyarmor.cli.core-3.2.dev1.dist-info/WHEEL,sha256=WMUqmIDVU_pzZFcU1pw1VFuQinSxJ4OGE6gHt3acQbA,99
-pyarmor.cli.core-3.2.dev1.dist-info/top_level.txt,sha256=UE1ovZ_90YzwF_lZ3LV7o8HKLe-RgzUaUUvdH5UTUus,8
-pyarmor.cli.core-3.2.dev1.dist-info/RECORD,,
+pyarmor/cli/core/pyarmor_runtime.pyd,sha256=MTABme9XWZ2O-U0LSTppjZoSz7Wp6gOn-U2dtLKJH4E,611840
+pyarmor/cli/core/pytransform3.pyd,sha256=eG2GqOH2y3YTvMpy3Z1h3mS9bf-7M3YvHmOqHsxmN9U,711168
+pyarmor.cli.core-3.2.dev2.dist-info/METADATA,sha256=6hoesmXSwLNb0zdZbByqM2xQQZQXWm5KQr73gFKuPwA,1892
+pyarmor.cli.core-3.2.dev2.dist-info/WHEEL,sha256=WMUqmIDVU_pzZFcU1pw1VFuQinSxJ4OGE6gHt3acQbA,99
+pyarmor.cli.core-3.2.dev2.dist-info/top_level.txt,sha256=UE1ovZ_90YzwF_lZ3LV7o8HKLe-RgzUaUUvdH5UTUus,8
+pyarmor.cli.core-3.2.dev2.dist-info/RECORD,,
```

