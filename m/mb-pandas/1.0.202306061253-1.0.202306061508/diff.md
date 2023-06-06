# Comparing `tmp/mb_pandas-1.0.202306061253-py3-none-any.whl.zip` & `tmp/mb_pandas-1.0.202306061508-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 9938 bytes, number of entries: 13
+Zip file size: 9950 bytes, number of entries: 13
 -rw-rw-r--  2.0 unx      162 b- defN 23-Jun-06 12:24 mb_pandas/src/__init__.py
 -rw-rw-r--  2.0 unx     1612 b- defN 23-Jun-06 12:24 mb_pandas/src/aio.py
 -rw-rw-r--  2.0 unx      482 b- defN 23-Jun-06 12:24 mb_pandas/src/convert_data.py
 -rw-rw-r--  2.0 unx     3516 b- defN 23-Jun-06 12:24 mb_pandas/src/dfload.py
 -rw-rw-r--  2.0 unx     2418 b- defN 23-Jun-06 12:24 mb_pandas/src/profiler.py
 -rw-rw-r--  2.0 unx     8075 b- defN 23-Jun-06 12:25 mb_pandas/src/transform.py
--rw-rw-r--  2.0 unx      396 b- defN 23-Jun-06 12:53 mb_pandas/src/version.py
--rwxrwxr-x  2.0 unx     1618 b- defN 23-Jun-06 12:53 mb_pandas-1.0.202306061253.data/scripts/df_profile
--rwxrwxr-x  2.0 unx     3683 b- defN 23-Jun-06 12:53 mb_pandas-1.0.202306061253.data/scripts/df_view
--rw-rw-r--  2.0 unx      224 b- defN 23-Jun-06 12:53 mb_pandas-1.0.202306061253.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-06 12:53 mb_pandas-1.0.202306061253.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-Jun-06 12:53 mb_pandas-1.0.202306061253.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1128 b- defN 23-Jun-06 12:53 mb_pandas-1.0.202306061253.dist-info/RECORD
-13 files, 23416 bytes uncompressed, 8030 bytes compressed:  65.7%
+-rw-rw-r--  2.0 unx      396 b- defN 23-Jun-06 15:08 mb_pandas/src/version.py
+-rwxrwxr-x  2.0 unx     1654 b- defN 23-Jun-06 15:08 mb_pandas-1.0.202306061508.data/scripts/df_profile
+-rwxrwxr-x  2.0 unx     3683 b- defN 23-Jun-06 15:08 mb_pandas-1.0.202306061508.data/scripts/df_view
+-rw-rw-r--  2.0 unx      224 b- defN 23-Jun-06 15:08 mb_pandas-1.0.202306061508.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-06 15:08 mb_pandas-1.0.202306061508.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-Jun-06 15:08 mb_pandas-1.0.202306061508.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1128 b- defN 23-Jun-06 15:08 mb_pandas-1.0.202306061508.dist-info/RECORD
+13 files, 23452 bytes uncompressed, 8042 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: mb_pandas/src/transform.py
 Comment: 
 
 Filename: mb_pandas/src/version.py
 Comment: 
 
-Filename: mb_pandas-1.0.202306061253.data/scripts/df_profile
+Filename: mb_pandas-1.0.202306061508.data/scripts/df_profile
 Comment: 
 
-Filename: mb_pandas-1.0.202306061253.data/scripts/df_view
+Filename: mb_pandas-1.0.202306061508.data/scripts/df_view
 Comment: 
 
-Filename: mb_pandas-1.0.202306061253.dist-info/METADATA
+Filename: mb_pandas-1.0.202306061508.dist-info/METADATA
 Comment: 
 
-Filename: mb_pandas-1.0.202306061253.dist-info/WHEEL
+Filename: mb_pandas-1.0.202306061508.dist-info/WHEEL
 Comment: 
 
-Filename: mb_pandas-1.0.202306061253.dist-info/top_level.txt
+Filename: mb_pandas-1.0.202306061508.dist-info/top_level.txt
 Comment: 
 
-Filename: mb_pandas-1.0.202306061253.dist-info/RECORD
+Filename: mb_pandas-1.0.202306061508.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mb_pandas/src/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('06')
 VERSION_DAY = int('06')
-VERSION_HOUR = int('12')
-VERSION_MINUTE = int('53')
+VERSION_HOUR = int('15')
+VERSION_MINUTE = int('08')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202306061253
-version_date = '2023/06/06 12:53'
+PATCH_VERSION = 202306061508
+version_date = '2023/06/06 15:08'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `mb_pandas-1.0.202306061253.data/scripts/df_profile` & `mb_pandas-1.0.202306061508.data/scripts/df_profile`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 # -*- coding: utf-8 -*-
 
 ##This script is used to profile the dataframe and save it in the local folder.
 
 import os
 from mb_pandas.src import dfload,profiler
 import argparse
+from mb_utils.src.logging import logger
 
 #get file
 #make a new folder
 
-def main(args,logger=None):
+def main(args,logger):
+
     logger.info("Starting loading dataframe from file: '{}'.".format(args.df_filepath))
     df = dfload.load_any_df(args.df_filepath,logger=logger)
     target=args.target if len(args.target)>0 else []
 
     logger.info("Target columns: {}".format(target))
     loc = args.folder_name + args.file_name
     if not os.path.exists(args.folder_name):
```

## Comparing `mb_pandas-1.0.202306061253.data/scripts/df_view` & `mb_pandas-1.0.202306061508.data/scripts/df_view`

 * *Files identical despite different names*

## Comparing `mb_pandas-1.0.202306061253.dist-info/RECORD` & `mb_pandas-1.0.202306061508.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 mb_pandas/src/__init__.py,sha256=WU80RSEXwgPXneLCZV_JyaMkKzAGEvYo9Icq0QzfBJE,162
 mb_pandas/src/aio.py,sha256=UK3o2TMFDeNQvhiFAulAyd1fKJPjrShEbK-Y-85tlsM,1612
 mb_pandas/src/convert_data.py,sha256=Wp1yDT9Ie-lBZGE7WmsMXB7nN3mv0MwbiloInr1aoc0,482
 mb_pandas/src/dfload.py,sha256=Yet5dq8R0NDi69UXiUAfQMwbWqhLRGjXqhUvJI5pBSw,3516
 mb_pandas/src/profiler.py,sha256=iX_nAksh-HzjyhQLnbutvEtNVGfVwja2CsQ1zaYZbeA,2418
 mb_pandas/src/transform.py,sha256=_sIJQwkGUjBuFIB20GQh3gADvO2AuyqUNgHXik3NwqE,8075
-mb_pandas/src/version.py,sha256=_sGGsV6IGvFF_52__bS83mcz4zEooObKn2hAwwCjfCw,396
-mb_pandas-1.0.202306061253.data/scripts/df_profile,sha256=rRSXEIuXCLDICx3dqBBogggRcStZTlorDyntkPiP3RI,1618
-mb_pandas-1.0.202306061253.data/scripts/df_view,sha256=BbS_rNgrPl7Raz_zVmTBqw_dvyAhc3-KqS4W2LV0_yo,3683
-mb_pandas-1.0.202306061253.dist-info/METADATA,sha256=JnxURTeRnKDmOb0-23pH83x_fC0Jc5bnSNzxlCyNKec,224
-mb_pandas-1.0.202306061253.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-mb_pandas-1.0.202306061253.dist-info/top_level.txt,sha256=5JkDz2-6yNAp6GiwpeR4FpxqXVysaksS5MD1iAvfMgo,10
-mb_pandas-1.0.202306061253.dist-info/RECORD,,
+mb_pandas/src/version.py,sha256=GHQV1qL0zFCi9p-q0JzDYarZBTP8nGSwqEsz-GZpZOs,396
+mb_pandas-1.0.202306061508.data/scripts/df_profile,sha256=OIsI7_Xhdo9VvT9AipHlwv55_YS7cKVM-Jx7HBQbj24,1654
+mb_pandas-1.0.202306061508.data/scripts/df_view,sha256=BbS_rNgrPl7Raz_zVmTBqw_dvyAhc3-KqS4W2LV0_yo,3683
+mb_pandas-1.0.202306061508.dist-info/METADATA,sha256=UoByq2IUbPcAg1iZpDP96zz09Q_-ndcqxE7d5176qOM,224
+mb_pandas-1.0.202306061508.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+mb_pandas-1.0.202306061508.dist-info/top_level.txt,sha256=5JkDz2-6yNAp6GiwpeR4FpxqXVysaksS5MD1iAvfMgo,10
+mb_pandas-1.0.202306061508.dist-info/RECORD,,
```

