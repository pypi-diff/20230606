# Comparing `tmp/kili_common_storage-0.0.8-py3-none-any.whl.zip` & `tmp/kili_common_storage-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -7,12 +7,12 @@
 -rw-r--r--  2.0 unx    14567 b- defN 22-Dec-12 11:47 kili-common-storage/object_storage.py
 -rw-r--r--  2.0 unx       77 b- defN 22-Dec-12 11:48 kili_common_storage/__init__.py
 -rw-r--r--  2.0 unx     6852 b- defN 22-Dec-08 03:27 kili_common_storage/constants.py
 -rw-r--r--  2.0 unx     1320 b- defN 22-Dec-12 12:25 kili_common_storage/decorator.py
 -rw-r--r--  2.0 unx        0 b- defN 22-Dec-08 03:40 kili_common_storage/exceptions.py
 -rw-r--r--  2.0 unx     1273 b- defN 22-Dec-08 03:22 kili_common_storage/loggings.py
 -rw-r--r--  2.0 unx    16483 b- defN 23-Jan-06 03:00 kili_common_storage/object_storage.py
--rw-r--r--  2.0 unx      517 b- defN 23-Jan-06 05:38 kili_common_storage-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-06 05:38 kili_common_storage-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 23-Jan-06 05:38 kili_common_storage-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1413 b- defN 23-Jan-06 05:38 kili_common_storage-0.0.8.dist-info/RECORD
+-rw-r--r--  2.0 unx      517 b- defN 23-Jan-06 05:47 kili_common_storage-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jan-06 05:47 kili_common_storage-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 23-Jan-06 05:47 kili_common_storage-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1413 b- defN 23-Jan-06 05:47 kili_common_storage-0.0.9.dist-info/RECORD
 16 files, 52136 bytes uncompressed, 12263 bytes compressed:  76.5%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: kili_common_storage/loggings.py
 Comment: 
 
 Filename: kili_common_storage/object_storage.py
 Comment: 
 
-Filename: kili_common_storage-0.0.8.dist-info/METADATA
+Filename: kili_common_storage-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: kili_common_storage-0.0.8.dist-info/WHEEL
+Filename: kili_common_storage-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: kili_common_storage-0.0.8.dist-info/top_level.txt
+Filename: kili_common_storage-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: kili_common_storage-0.0.8.dist-info/RECORD
+Filename: kili_common_storage-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `kili_common_storage-0.0.8.dist-info/METADATA` & `kili_common_storage-0.0.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kili-common-storage
-Version: 0.0.8
+Version: 0.0.9
 Summary: A storage package for kilimall lite
 Home-page: 
 Author: Ken.Hu
 Author-email: ken.hu@kilimall.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `kili_common_storage-0.0.8.dist-info/RECORD` & `kili_common_storage-0.0.9.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -6,11 +6,11 @@
 kili-common-storage/object_storage.py,sha256=mRtbubapUvrYABdrHyPPcVTapoImvo4pnhmErDpCYgo,14567
 kili_common_storage/__init__.py,sha256=QgDewLcWo0CysHDDxOvv5ge3dC2iuhSWHqsNRqwtSlk,77
 kili_common_storage/constants.py,sha256=OR3A8p9WVfRVbgB-Xc01cQExVjuDp6s_zjeTuW0vKPc,6852
 kili_common_storage/decorator.py,sha256=NLUjmNdbc-jQW_cycnSwBgJWwADY39f20rppdrW1naI,1320
 kili_common_storage/exceptions.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 kili_common_storage/loggings.py,sha256=o7tR8raOXkDikx2YxiEgE-M3ApXW_nAHSqLcOpXk6k4,1273
 kili_common_storage/object_storage.py,sha256=I35jjWiqJDD0tdH5jCsr1oz1b8WJiVVWM7YTsE-b864,16483
-kili_common_storage-0.0.8.dist-info/METADATA,sha256=gpW0A8zUX77aBYSU9sR6_uk81XcIfgYkxYMWSc2SqP8,517
-kili_common_storage-0.0.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-kili_common_storage-0.0.8.dist-info/top_level.txt,sha256=1FTUpZs1YU23m8WO0a3Sl4Aaq-9oCGU44gYb18ribss,20
-kili_common_storage-0.0.8.dist-info/RECORD,,
+kili_common_storage-0.0.9.dist-info/METADATA,sha256=zt_cteEJTZNnsz_ZoQipeKcHP1f78CJIxWpCOiXbPtc,517
+kili_common_storage-0.0.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+kili_common_storage-0.0.9.dist-info/top_level.txt,sha256=1FTUpZs1YU23m8WO0a3Sl4Aaq-9oCGU44gYb18ribss,20
+kili_common_storage-0.0.9.dist-info/RECORD,,
```

