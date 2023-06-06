# Comparing `tmp/Scrapset-1.1.0-py3-none-any.whl.zip` & `tmp/Scrapset-1.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3749 bytes, number of entries: 7
+Zip file size: 4227 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat     4485 b- defN 23-Jun-05 15:51 Scrapset/Scrapset.py
--rw-rw-rw-  2.0 fat       67 b- defN 23-Jun-05 15:28 Scrapset/__init__.py
--rw-rw-rw-  2.0 fat     2789 b- defN 23-Jun-05 16:08 Scrapset-1.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-05 16:08 Scrapset-1.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      632 b- defN 23-Jun-05 16:08 Scrapset-1.1.0.dist-info/licence.txt
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-05 16:08 Scrapset-1.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      545 b- defN 23-Jun-05 16:08 Scrapset-1.1.0.dist-info/RECORD
-7 files, 8619 bytes uncompressed, 2779 bytes compressed:  67.8%
+-rw-rw-rw-  2.0 fat       18 b- defN 23-Jun-06 18:34 Scrapset/__init__.py
+-rw-rw-rw-  2.0 fat     4305 b- defN 23-Jun-06 18:37 Scrapset-1.2.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-06 18:37 Scrapset-1.2.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      632 b- defN 23-Jun-06 18:37 Scrapset-1.2.0.dist-info/licence.txt
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jun-06 18:37 Scrapset-1.2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      545 b- defN 23-Jun-06 18:37 Scrapset-1.2.0.dist-info/RECORD
+7 files, 10086 bytes uncompressed, 3257 bytes compressed:  67.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: Scrapset/Scrapset.py
 Comment: 
 
 Filename: Scrapset/__init__.py
 Comment: 
 
-Filename: Scrapset-1.1.0.dist-info/METADATA
+Filename: Scrapset-1.2.0.dist-info/METADATA
 Comment: 
 
-Filename: Scrapset-1.1.0.dist-info/WHEEL
+Filename: Scrapset-1.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: Scrapset-1.1.0.dist-info/licence.txt
+Filename: Scrapset-1.2.0.dist-info/licence.txt
 Comment: 
 
-Filename: Scrapset-1.1.0.dist-info/top_level.txt
+Filename: Scrapset-1.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: Scrapset-1.1.0.dist-info/RECORD
+Filename: Scrapset-1.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Scrapset/__init__.py

```diff
@@ -1,2 +1 @@
-from Scrapset import KaggleDataSet
-from Scrapset import DataDotGov
+import Scrapset
```

## Comparing `Scrapset-1.1.0.dist-info/licence.txt` & `Scrapset-1.2.0.dist-info/licence.txt`

 * *Files identical despite different names*

## Comparing `Scrapset-1.1.0.dist-info/RECORD` & `Scrapset-1.2.0.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 Scrapset/Scrapset.py,sha256=cpgoiFbf14lkLS5DR0X992HwU2r7o3jRc0fAZPiEqeE,4485
-Scrapset/__init__.py,sha256=_WwZDcTXBfm9fjdR6bFA36VcSgVsVmDVrf-fguj1UhQ,67
-Scrapset-1.1.0.dist-info/METADATA,sha256=caMjZg0NIBLA_vSWIoAK1ekl-2wmVk0WdGCJ3c7LQEI,2789
-Scrapset-1.1.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-Scrapset-1.1.0.dist-info/licence.txt,sha256=i79SE9-rWtU07j8Skpf29SRVwtEfuu34njYipmNzLGU,632
-Scrapset-1.1.0.dist-info/top_level.txt,sha256=DZOAmLHm1ITM5F5fGFEDfQ6NnQAwotBcWCwj5PdhqNw,9
-Scrapset-1.1.0.dist-info/RECORD,,
+Scrapset/__init__.py,sha256=WBq__Qf5KAi57ae195TDq8YgIjTgYGbIxiMD4OeMByI,18
+Scrapset-1.2.0.dist-info/METADATA,sha256=CiGAMplLAtm6Pzy6vG0qxrJWPxPHeDLOO4wKQrPRpOU,4305
+Scrapset-1.2.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+Scrapset-1.2.0.dist-info/licence.txt,sha256=i79SE9-rWtU07j8Skpf29SRVwtEfuu34njYipmNzLGU,632
+Scrapset-1.2.0.dist-info/top_level.txt,sha256=DZOAmLHm1ITM5F5fGFEDfQ6NnQAwotBcWCwj5PdhqNw,9
+Scrapset-1.2.0.dist-info/RECORD,,
```

