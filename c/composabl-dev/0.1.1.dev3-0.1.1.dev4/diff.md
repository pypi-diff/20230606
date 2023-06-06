# Comparing `tmp/composabl_dev-0.1.1.dev3-cp38-cp38-manylinux_2_35_x86_64.whl.zip` & `tmp/composabl_dev-0.1.1.dev4-cp38-cp38-manylinux_2_35_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -45,12 +45,12 @@
 -rwxr-xr-x  2.0 unx   143232 b- defN 80-Jan-01 00:00 composabl/utils/exception_handler_grpc_server.cpython-38-x86_64-linux-gnu.so
 -rwxr-xr-x  2.0 unx   226872 b- defN 80-Jan-01 00:00 composabl/utils/json_encoder.cpython-38-x86_64-linux-gnu.so
 -rwxr-xr-x  2.0 unx   209688 b- defN 80-Jan-01 00:00 composabl/utils/logger.cpython-38-x86_64-linux-gnu.so
 -rwxr-xr-x  2.0 unx   257096 b- defN 80-Jan-01 00:00 composabl/utils/serializer.cpython-38-x86_64-linux-gnu.so
 -rwxr-xr-x  2.0 unx   712632 b- defN 80-Jan-01 00:00 composabl/utils/serializer_datatype.cpython-38-x86_64-linux-gnu.so
 -rwxr-xr-x  2.0 unx   169392 b- defN 80-Jan-01 00:00 composabl/utils/serializer_gym_env.cpython-38-x86_64-linux-gnu.so
 -rwxr-xr-x  2.0 unx   652960 b- defN 80-Jan-01 00:00 composabl/utils/serializer_gym_space.cpython-38-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx     3304 b- defN 80-Jan-01 00:00 composabl_dev-0.1.1.dev3.dist-info/METADATA
--rw-r--r--  2.0 unx      108 b- defN 80-Jan-01 00:00 composabl_dev-0.1.1.dev3.dist-info/WHEEL
--rw-r--r--  2.0 unx       44 b- defN 80-Jan-01 00:00 composabl_dev-0.1.1.dev3.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     6414 b- defN 16-Jan-01 00:00 composabl_dev-0.1.1.dev3.dist-info/RECORD
+-rw-r--r--  2.0 unx     3304 b- defN 80-Jan-01 00:00 composabl_dev-0.1.1.dev4.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 80-Jan-01 00:00 composabl_dev-0.1.1.dev4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       44 b- defN 80-Jan-01 00:00 composabl_dev-0.1.1.dev4.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     6414 b- defN 16-Jan-01 00:00 composabl_dev-0.1.1.dev4.dist-info/RECORD
 54 files, 14718309 bytes uncompressed, 5865232 bytes compressed:  60.2%
```

## zipnote {}

```diff
@@ -144,20 +144,20 @@
 
 Filename: composabl/utils/serializer_gym_env.cpython-38-x86_64-linux-gnu.so
 Comment: 
 
 Filename: composabl/utils/serializer_gym_space.cpython-38-x86_64-linux-gnu.so
 Comment: 
 
-Filename: composabl_dev-0.1.1.dev3.dist-info/METADATA
+Filename: composabl_dev-0.1.1.dev4.dist-info/METADATA
 Comment: 
 
-Filename: composabl_dev-0.1.1.dev3.dist-info/WHEEL
+Filename: composabl_dev-0.1.1.dev4.dist-info/WHEEL
 Comment: 
 
-Filename: composabl_dev-0.1.1.dev3.dist-info/entry_points.txt
+Filename: composabl_dev-0.1.1.dev4.dist-info/entry_points.txt
 Comment: 
 
-Filename: composabl_dev-0.1.1.dev3.dist-info/RECORD
+Filename: composabl_dev-0.1.1.dev4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `composabl_dev-0.1.1.dev3.dist-info/METADATA` & `composabl_dev-0.1.1.dev4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composabl-dev
-Version: 0.1.1.dev3
+Version: 0.1.1.dev4
 Summary: 
 Author: Xavier Geerinck
 Author-email: xavier.geerinck@gmail.com
 Requires-Python: >=3.8.13,<3.9.0
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: autorom[accept-rom-license] (>=0.4.2,<0.5.0)
 Requires-Dist: dapr (>=1.9.1,<2.0.0)
```

## Comparing `composabl_dev-0.1.1.dev3.dist-info/RECORD` & `composabl_dev-0.1.1.dev4.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -44,11 +44,11 @@
 composabl/utils/exception_handler_grpc_server.cpython-38-x86_64-linux-gnu.so,sha256=E7CTRJHrv1m3nTnz3g8mUshiiyQei_Zg2kEGjR05w8A,143232
 composabl/utils/json_encoder.cpython-38-x86_64-linux-gnu.so,sha256=c2gLalPFTXnWcaghsa5FBGtkMJz0o6R8QEzXGPonUU0,226872
 composabl/utils/logger.cpython-38-x86_64-linux-gnu.so,sha256=5ZCJhDa2y3ZXXt7SvS1cr7n4Jz3q8ZpayOu8w8929V0,209688
 composabl/utils/serializer.cpython-38-x86_64-linux-gnu.so,sha256=K_zhg6serdXJb9ir3ak-iQcHjPfYVY56DkFumh082ns,257096
 composabl/utils/serializer_datatype.cpython-38-x86_64-linux-gnu.so,sha256=CV0YycT6al6MmTfmWSoPaxA3GevanQf9jCNLJVYeRGQ,712632
 composabl/utils/serializer_gym_env.cpython-38-x86_64-linux-gnu.so,sha256=pT54U9LA3czxcrZSY92LMp0-ouv9SdvGCWhD91vqwQg,169392
 composabl/utils/serializer_gym_space.cpython-38-x86_64-linux-gnu.so,sha256=_fDapH1J-S8xYMMRrad7X-wGcmAr9jntuceCjGQmNJk,652960
-composabl_dev-0.1.1.dev3.dist-info/METADATA,sha256=nGQvrX59nF31kMWoWvUg_y-wNwhUMqcrhvai3-mhJKA,3304
-composabl_dev-0.1.1.dev3.dist-info/WHEEL,sha256=wJ5EmkVmmHzta13pO66XP-ZMLpAN-mgq2dZFJPyoTIM,108
-composabl_dev-0.1.1.dev3.dist-info/entry_points.txt,sha256=OLAf-cR2A5jEaGfSoF7vgN--QKl2-ibC_9Uspebb4wI,44
-composabl_dev-0.1.1.dev3.dist-info/RECORD,,
+composabl_dev-0.1.1.dev4.dist-info/METADATA,sha256=ePAJQQhuuZXQnszowqIVFU9CtabE26NnQP-JMaORsF8,3304
+composabl_dev-0.1.1.dev4.dist-info/WHEEL,sha256=wJ5EmkVmmHzta13pO66XP-ZMLpAN-mgq2dZFJPyoTIM,108
+composabl_dev-0.1.1.dev4.dist-info/entry_points.txt,sha256=OLAf-cR2A5jEaGfSoF7vgN--QKl2-ibC_9Uspebb4wI,44
+composabl_dev-0.1.1.dev4.dist-info/RECORD,,
```

