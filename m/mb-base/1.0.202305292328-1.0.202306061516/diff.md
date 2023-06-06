# Comparing `tmp/mb_base-1.0.202305292328-py3-none-any.whl.zip` & `tmp/mb_base-1.0.202306061516-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 4977 bytes, number of entries: 10
--rw-rw-r--  2.0 unx      323 b- defN 23-May-25 00:28 mb/numpy/__init__.py
--rw-rw-r--  2.0 unx       49 b- defN 23-May-25 00:31 mb/pandas/__init__.py
--rw-rw-r--  2.0 unx       54 b- defN 23-May-25 20:10 mb/plt/__init__.py
--rw-rw-r--  2.0 unx     8004 b- defN 23-May-29 22:58 mb/plt/emb_viz.py
--rw-rw-r--  2.0 unx       65 b- defN 23-May-29 11:27 mb/utils/__init__.py
--rw-rw-r--  2.0 unx      739 b- defN 23-May-29 11:18 mb/utils/pip_update.py
--rw-rw-r--  2.0 unx      302 b- defN 23-May-29 23:28 mb_base-1.0.202305292328.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-29 23:28 mb_base-1.0.202305292328.dist-info/WHEEL
--rw-rw-r--  2.0 unx        3 b- defN 23-May-29 23:28 mb_base-1.0.202305292328.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      792 b- defN 23-May-29 23:28 mb_base-1.0.202305292328.dist-info/RECORD
-10 files, 10423 bytes uncompressed, 3615 bytes compressed:  65.3%
+Zip file size: 4985 bytes, number of entries: 10
+-rw-rw-r--  2.0 unx      323 b- defN 23-May-30 16:26 mb/numpy/__init__.py
+-rw-rw-r--  2.0 unx       49 b- defN 23-May-30 16:26 mb/pandas/__init__.py
+-rw-rw-r--  2.0 unx       54 b- defN 23-May-30 16:26 mb/plt/__init__.py
+-rw-rw-r--  2.0 unx     8004 b- defN 23-May-30 16:26 mb/plt/emb_viz.py
+-rw-rw-r--  2.0 unx       65 b- defN 23-May-30 16:26 mb/utils/__init__.py
+-rw-rw-r--  2.0 unx      751 b- defN 23-Jun-06 15:16 mb/utils/pip_update.py
+-rw-rw-r--  2.0 unx      302 b- defN 23-Jun-06 15:16 mb_base-1.0.202306061516.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-06 15:16 mb_base-1.0.202306061516.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        3 b- defN 23-Jun-06 15:16 mb_base-1.0.202306061516.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      792 b- defN 23-Jun-06 15:16 mb_base-1.0.202306061516.dist-info/RECORD
+10 files, 10435 bytes uncompressed, 3623 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: mb/utils/__init__.py
 Comment: 
 
 Filename: mb/utils/pip_update.py
 Comment: 
 
-Filename: mb_base-1.0.202305292328.dist-info/METADATA
+Filename: mb_base-1.0.202306061516.dist-info/METADATA
 Comment: 
 
-Filename: mb_base-1.0.202305292328.dist-info/WHEEL
+Filename: mb_base-1.0.202306061516.dist-info/WHEEL
 Comment: 
 
-Filename: mb_base-1.0.202305292328.dist-info/top_level.txt
+Filename: mb_base-1.0.202306061516.dist-info/top_level.txt
 Comment: 
 
-Filename: mb_base-1.0.202305292328.dist-info/RECORD
+Filename: mb_base-1.0.202306061516.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mb/utils/pip_update.py

```diff
@@ -1,9 +1,9 @@
 import subprocess
-from mb.utils import logger
+from mb_utils.src.logging import logger
 
 __all__ = ['update_package']
 
 def update_package(package_name):
     # Check if package is up-to-date
     result = subprocess.run(['pip', 'check', package_name], capture_output=True, text=True)
     if 'up-to-date' in result.stdout:
```

