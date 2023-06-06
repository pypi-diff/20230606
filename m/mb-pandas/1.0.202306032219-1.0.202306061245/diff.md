# Comparing `tmp/mb_pandas-1.0.202306032219-py3-none-any.whl.zip` & `tmp/mb_pandas-1.0.202306061245-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 9953 bytes, number of entries: 13
--rw-rw-r--  2.0 unx      162 b- defN 23-May-25 03:48 mb_pandas/src/__init__.py
--rw-rw-r--  2.0 unx     1612 b- defN 23-May-25 03:36 mb_pandas/src/aio.py
--rw-rw-r--  2.0 unx      482 b- defN 23-May-25 03:36 mb_pandas/src/convert_data.py
--rw-rw-r--  2.0 unx     3516 b- defN 23-May-29 10:17 mb_pandas/src/dfload.py
--rw-rw-r--  2.0 unx     2418 b- defN 23-May-25 03:36 mb_pandas/src/profiler.py
--rw-rw-r--  2.0 unx     8085 b- defN 23-Jun-03 22:18 mb_pandas/src/transform.py
--rw-rw-r--  2.0 unx      396 b- defN 23-Jun-03 22:19 mb_pandas/src/version.py
--rwxrwxr-x  2.0 unx     1671 b- defN 23-Jun-03 22:19 mb_pandas-1.0.202306032219.data/scripts/df_profile
--rwxrwxr-x  2.0 unx     3683 b- defN 23-Jun-03 22:19 mb_pandas-1.0.202306032219.data/scripts/df_view
--rw-rw-r--  2.0 unx      224 b- defN 23-Jun-03 22:19 mb_pandas-1.0.202306032219.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-03 22:19 mb_pandas-1.0.202306032219.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-Jun-03 22:19 mb_pandas-1.0.202306032219.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1128 b- defN 23-Jun-03 22:19 mb_pandas-1.0.202306032219.dist-info/RECORD
-13 files, 23479 bytes uncompressed, 8045 bytes compressed:  65.7%
+Zip file size: 9950 bytes, number of entries: 13
+-rw-rw-r--  2.0 unx      162 b- defN 23-Jun-06 12:24 mb_pandas/src/__init__.py
+-rw-rw-r--  2.0 unx     1612 b- defN 23-Jun-06 12:24 mb_pandas/src/aio.py
+-rw-rw-r--  2.0 unx      482 b- defN 23-Jun-06 12:24 mb_pandas/src/convert_data.py
+-rw-rw-r--  2.0 unx     3516 b- defN 23-Jun-06 12:24 mb_pandas/src/dfload.py
+-rw-rw-r--  2.0 unx     2418 b- defN 23-Jun-06 12:24 mb_pandas/src/profiler.py
+-rw-rw-r--  2.0 unx     8075 b- defN 23-Jun-06 12:25 mb_pandas/src/transform.py
+-rw-rw-r--  2.0 unx      396 b- defN 23-Jun-06 12:45 mb_pandas/src/version.py
+-rwxrwxr-x  2.0 unx     1660 b- defN 23-Jun-06 12:46 mb_pandas-1.0.202306061245.data/scripts/df_profile
+-rwxrwxr-x  2.0 unx     3683 b- defN 23-Jun-06 12:46 mb_pandas-1.0.202306061245.data/scripts/df_view
+-rw-rw-r--  2.0 unx      224 b- defN 23-Jun-06 12:46 mb_pandas-1.0.202306061245.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-06 12:46 mb_pandas-1.0.202306061245.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-Jun-06 12:46 mb_pandas-1.0.202306061245.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1128 b- defN 23-Jun-06 12:46 mb_pandas-1.0.202306061245.dist-info/RECORD
+13 files, 23458 bytes uncompressed, 8042 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: mb_pandas/src/transform.py
 Comment: 
 
 Filename: mb_pandas/src/version.py
 Comment: 
 
-Filename: mb_pandas-1.0.202306032219.data/scripts/df_profile
+Filename: mb_pandas-1.0.202306061245.data/scripts/df_profile
 Comment: 
 
-Filename: mb_pandas-1.0.202306032219.data/scripts/df_view
+Filename: mb_pandas-1.0.202306061245.data/scripts/df_view
 Comment: 
 
-Filename: mb_pandas-1.0.202306032219.dist-info/METADATA
+Filename: mb_pandas-1.0.202306061245.dist-info/METADATA
 Comment: 
 
-Filename: mb_pandas-1.0.202306032219.dist-info/WHEEL
+Filename: mb_pandas-1.0.202306061245.dist-info/WHEEL
 Comment: 
 
-Filename: mb_pandas-1.0.202306032219.dist-info/top_level.txt
+Filename: mb_pandas-1.0.202306061245.dist-info/top_level.txt
 Comment: 
 
-Filename: mb_pandas-1.0.202306032219.dist-info/RECORD
+Filename: mb_pandas-1.0.202306061245.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mb_pandas/src/transform.py

```diff
@@ -1,11 +1,10 @@
 ##Pandas file checker
 
 import pandas as pd
-import os
 from .dfload import load_any_df
 from mb_utils.src.logging import logger
 import numpy as np
 import cv2
 
 __all__ = ['check_null','remove_unnamed','rename_columns','check_drop_duplicates','get_dftype','merge_chunk','merge_dask']
```

## mb_pandas/src/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('06')
-VERSION_DAY = int('03')
-VERSION_HOUR = int('22')
-VERSION_MINUTE = int('19')
+VERSION_DAY = int('06')
+VERSION_HOUR = int('12')
+VERSION_MINUTE = int('45')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202306032219
-version_date = '2023/06/03 22:19'
+PATCH_VERSION = 202306061245
+version_date = '2023/06/06 12:45'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `mb_pandas-1.0.202306032219.data/scripts/df_profile` & `mb_pandas-1.0.202306061245.data/scripts/df_profile`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #!python
 # -*- coding: utf-8 -*-
 
 ##This script is used to profile the dataframe and save it in the local folder.
 
 import os
-import sys
 from mb_pandas.src import dfload,profiler
 from mb_utils.src.logging import logger
 import argparse
 
 #get file
 #make a new folder
```

## Comparing `mb_pandas-1.0.202306032219.data/scripts/df_view` & `mb_pandas-1.0.202306061245.data/scripts/df_view`

 * *Files identical despite different names*

## Comparing `mb_pandas-1.0.202306032219.dist-info/RECORD` & `mb_pandas-1.0.202306061245.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 mb_pandas/src/__init__.py,sha256=WU80RSEXwgPXneLCZV_JyaMkKzAGEvYo9Icq0QzfBJE,162
 mb_pandas/src/aio.py,sha256=UK3o2TMFDeNQvhiFAulAyd1fKJPjrShEbK-Y-85tlsM,1612
 mb_pandas/src/convert_data.py,sha256=Wp1yDT9Ie-lBZGE7WmsMXB7nN3mv0MwbiloInr1aoc0,482
 mb_pandas/src/dfload.py,sha256=Yet5dq8R0NDi69UXiUAfQMwbWqhLRGjXqhUvJI5pBSw,3516
 mb_pandas/src/profiler.py,sha256=iX_nAksh-HzjyhQLnbutvEtNVGfVwja2CsQ1zaYZbeA,2418
-mb_pandas/src/transform.py,sha256=7fsxapQO7rlGQGUbeVG4ViKyw3uEH5X6HZAlLpXn9eA,8085
-mb_pandas/src/version.py,sha256=6eN9rhYZzn42brr8hyq45lFmZ_e8YEmEL8ErAU32jaQ,396
-mb_pandas-1.0.202306032219.data/scripts/df_profile,sha256=zi4GRNQ6P5_JEB_0wMYB1KzLRG59eHXxRZG_I84lTYQ,1671
-mb_pandas-1.0.202306032219.data/scripts/df_view,sha256=BbS_rNgrPl7Raz_zVmTBqw_dvyAhc3-KqS4W2LV0_yo,3683
-mb_pandas-1.0.202306032219.dist-info/METADATA,sha256=0JWP8I-JzhAx1hOChtM978iNkE7IsNgZvR6misyMNFM,224
-mb_pandas-1.0.202306032219.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-mb_pandas-1.0.202306032219.dist-info/top_level.txt,sha256=5JkDz2-6yNAp6GiwpeR4FpxqXVysaksS5MD1iAvfMgo,10
-mb_pandas-1.0.202306032219.dist-info/RECORD,,
+mb_pandas/src/transform.py,sha256=_sIJQwkGUjBuFIB20GQh3gADvO2AuyqUNgHXik3NwqE,8075
+mb_pandas/src/version.py,sha256=7M4CL2isKIGyTAkJWeZ5QK4fhHFj7lUo0-OEFT75gHo,396
+mb_pandas-1.0.202306061245.data/scripts/df_profile,sha256=ulHzSMSMsCKE_GrB51wCLwWwYUdJapFLD5Jlg-Bd0zo,1660
+mb_pandas-1.0.202306061245.data/scripts/df_view,sha256=BbS_rNgrPl7Raz_zVmTBqw_dvyAhc3-KqS4W2LV0_yo,3683
+mb_pandas-1.0.202306061245.dist-info/METADATA,sha256=oM92JzUIHw4LgRvN8vS9ulTXRsh_O-iqly6dgZWyhd8,224
+mb_pandas-1.0.202306061245.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+mb_pandas-1.0.202306061245.dist-info/top_level.txt,sha256=5JkDz2-6yNAp6GiwpeR4FpxqXVysaksS5MD1iAvfMgo,10
+mb_pandas-1.0.202306061245.dist-info/RECORD,,
```

