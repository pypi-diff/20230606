# Comparing `tmp/mb_utils-1.0.202306061511-py3-none-any.whl.zip` & `tmp/mb_utils-1.0.202306061514-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,16 @@
-Zip file size: 7911 bytes, number of entries: 15
--rw-rw-r--  2.0 unx        0 b- defN 23-May-30 16:38 mb_utils/__init__.py
--rw-rw-r--  2.0 unx      288 b- defN 23-Jun-06 15:11 mb_utils/src/__init__.py
+Zip file size: 7760 bytes, number of entries: 14
+-rw-rw-r--  2.0 unx      311 b- defN 23-Jun-06 15:13 mb_utils/src/__init__.py
 -rw-rw-r--  2.0 unx     3330 b- defN 23-May-30 16:38 mb_utils/src/deprecated.py
 -rw-rw-r--  2.0 unx     1318 b- defN 23-May-30 16:38 mb_utils/src/extra.py
 -rw-rw-r--  2.0 unx     1813 b- defN 23-May-30 16:38 mb_utils/src/logging.py
 -rw-rw-r--  2.0 unx      664 b- defN 23-May-30 16:38 mb_utils/src/path_checker.py
 -rw-rw-r--  2.0 unx     1306 b- defN 23-May-30 16:38 mb_utils/src/retry_decorator.py
 -rw-rw-r--  2.0 unx     3093 b- defN 23-May-30 16:38 mb_utils/src/s3.py
 -rw-rw-r--  2.0 unx      777 b- defN 23-May-30 16:38 mb_utils/src/terminal.py
 -rw-rw-r--  2.0 unx     1821 b- defN 23-May-30 16:38 mb_utils/src/verify_image.py
--rw-rw-r--  2.0 unx      396 b- defN 23-Jun-06 15:11 mb_utils/src/version.py
--rw-rw-r--  2.0 unx      251 b- defN 23-Jun-06 15:11 mb_utils-1.0.202306061511.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-06 15:11 mb_utils-1.0.202306061511.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-Jun-06 15:11 mb_utils-1.0.202306061511.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1230 b- defN 23-Jun-06 15:11 mb_utils-1.0.202306061511.dist-info/RECORD
-15 files, 16388 bytes uncompressed, 5865 bytes compressed:  64.2%
+-rw-rw-r--  2.0 unx      396 b- defN 23-Jun-06 15:14 mb_utils/src/version.py
+-rw-rw-r--  2.0 unx      251 b- defN 23-Jun-06 15:14 mb_utils-1.0.202306061514.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-06 15:14 mb_utils-1.0.202306061514.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-Jun-06 15:14 mb_utils-1.0.202306061514.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1156 b- defN 23-Jun-06 15:14 mb_utils-1.0.202306061514.dist-info/RECORD
+14 files, 16337 bytes uncompressed, 5830 bytes compressed:  64.3%
```

## zipnote {}

```diff
@@ -1,10 +1,7 @@
-Filename: mb_utils/__init__.py
-Comment: 
-
 Filename: mb_utils/src/__init__.py
 Comment: 
 
 Filename: mb_utils/src/deprecated.py
 Comment: 
 
 Filename: mb_utils/src/extra.py
@@ -27,20 +24,20 @@
 
 Filename: mb_utils/src/verify_image.py
 Comment: 
 
 Filename: mb_utils/src/version.py
 Comment: 
 
-Filename: mb_utils-1.0.202306061511.dist-info/METADATA
+Filename: mb_utils-1.0.202306061514.dist-info/METADATA
 Comment: 
 
-Filename: mb_utils-1.0.202306061511.dist-info/WHEEL
+Filename: mb_utils-1.0.202306061514.dist-info/WHEEL
 Comment: 
 
-Filename: mb_utils-1.0.202306061511.dist-info/top_level.txt
+Filename: mb_utils-1.0.202306061514.dist-info/top_level.txt
 Comment: 
 
-Filename: mb_utils-1.0.202306061511.dist-info/RECORD
+Filename: mb_utils-1.0.202306061514.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mb_utils/src/__init__.py

```diff
@@ -1,12 +1,13 @@
 from .version import version
 from .deprecated import *
 from .extra import *
 from .s3 import *
 from .terminal import *
+from .logging import *
 from .verify_image import *
 from .path_checker import *
 from .retry_decorator import *
 
 
 # import logging
 # logging.getLogger(__name__).addHandler(logging.NullHandler())
```

## mb_utils/src/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('06')
 VERSION_DAY = int('06')
 VERSION_HOUR = int('15')
-VERSION_MINUTE = int('11')
+VERSION_MINUTE = int('14')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202306061511
-version_date = '2023/06/06 15:11'
+PATCH_VERSION = 202306061514
+version_date = '2023/06/06 15:14'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `mb_utils-1.0.202306061511.dist-info/RECORD` & `mb_utils-1.0.202306061514.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-mb_utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mb_utils/src/__init__.py,sha256=pf7s7GPun-_cXQqMRIfE86xBZG8Z8FljZ-8ErDm7_vk,288
+mb_utils/src/__init__.py,sha256=DkLZ1-4phWsDQ8DArT12K-4JIuXT2AogzJ5p9xVcLbw,311
 mb_utils/src/deprecated.py,sha256=yHz0JrDjGJDVT71gILr2JIYu6x1wWyENcUf4-lkuv10,3330
 mb_utils/src/extra.py,sha256=NP5JlU0oktw7j2cn_-W3rAMzjMYDKwzBeiSjpg-Evh4,1318
 mb_utils/src/logging.py,sha256=bwkKDej4pI1WzNKrQs9rTRx73z-EyZkB7UCPsYHnbs0,1813
 mb_utils/src/path_checker.py,sha256=MrE3P2hkDjOIWyZJ-Lh1X3wODKRnJk_nfVgKW0nQEMU,664
 mb_utils/src/retry_decorator.py,sha256=1lotNMXwALWFgb0ikrK9B-flOOMj9tTlOQgYCb-ejwY,1306
 mb_utils/src/s3.py,sha256=jxNla2kvFu39k79bAW0x_ZoqUWBhvSaQaH8A-Af5xCY,3093
 mb_utils/src/terminal.py,sha256=_1l8K9CwAFYx4UgfkwOWfgeZ2bZu4s-71gnyxWJc2xA,777
 mb_utils/src/verify_image.py,sha256=L_XAlYBsdAhTkMSVcMpgwS0Ea8I9r-ZjoChjL0GHT38,1821
-mb_utils/src/version.py,sha256=MHKlaqK0GKSBGwjJiMRIYxXYfFKniKmrTzv75XJ9llw,396
-mb_utils-1.0.202306061511.dist-info/METADATA,sha256=DvIhqG8146Vj6Zj1Yc-gYPs1oRQ50fdj7K2Zzs7rpfo,251
-mb_utils-1.0.202306061511.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-mb_utils-1.0.202306061511.dist-info/top_level.txt,sha256=xeK1qEZ7uoXfZyNlYlurb_F_T8trKUaTU_Fm_UpKhyg,9
-mb_utils-1.0.202306061511.dist-info/RECORD,,
+mb_utils/src/version.py,sha256=e7hhFoPO01ShpXOb2ZFci6M4vbCZyWAcCFSM_zPxzDE,396
+mb_utils-1.0.202306061514.dist-info/METADATA,sha256=sKZ2bzXXpFybwGJy5bVeFqjX0GJPq_zlPqpYsP0Ie_Y,251
+mb_utils-1.0.202306061514.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+mb_utils-1.0.202306061514.dist-info/top_level.txt,sha256=xeK1qEZ7uoXfZyNlYlurb_F_T8trKUaTU_Fm_UpKhyg,9
+mb_utils-1.0.202306061514.dist-info/RECORD,,
```

