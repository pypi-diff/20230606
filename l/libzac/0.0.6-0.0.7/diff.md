# Comparing `tmp/libzac-0.0.6-py3-none-any.whl.zip` & `tmp/libzac-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 13424 bytes, number of entries: 13
+Zip file size: 13423 bytes, number of entries: 13
 -rw-rw-rw-  2.0 fat      134 b- defN 23-May-30 07:53 libzac/__init__.py
 -rw-rw-rw-  2.0 fat     4799 b- defN 23-Jun-06 01:57 libzac/bitfield.py
 -rw-rw-rw-  2.0 fat     1960 b- defN 23-May-17 07:50 libzac/dsp.py
 -rw-rw-rw-  2.0 fat     2392 b- defN 23-May-17 07:56 libzac/e.py
 -rw-rw-rw-  2.0 fat     3007 b- defN 23-May-17 07:56 libzac/io.py
 -rw-rw-rw-  2.0 fat     1510 b- defN 23-May-23 02:36 libzac/math.py
 -rw-rw-rw-  2.0 fat     3074 b- defN 23-May-17 08:19 libzac/plt.py
 -rw-rw-rw-  2.0 fat     8791 b- defN 23-Jun-05 08:39 libzac/reg.py
--rw-rw-rw-  2.0 fat     1088 b- defN 23-Jun-06 03:48 libzac-0.0.6.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1691 b- defN 23-Jun-06 03:48 libzac-0.0.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-06 03:48 libzac-0.0.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Jun-06 03:48 libzac-0.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      947 b- defN 23-Jun-06 03:48 libzac-0.0.6.dist-info/RECORD
-13 files, 29492 bytes uncompressed, 11882 bytes compressed:  59.7%
+-rw-rw-rw-  2.0 fat     1088 b- defN 23-Jun-06 03:49 libzac-0.0.7.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1691 b- defN 23-Jun-06 03:49 libzac-0.0.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-06 03:49 libzac-0.0.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Jun-06 03:49 libzac-0.0.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      947 b- defN 23-Jun-06 03:49 libzac-0.0.7.dist-info/RECORD
+13 files, 29492 bytes uncompressed, 11881 bytes compressed:  59.7%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: libzac/plt.py
 Comment: 
 
 Filename: libzac/reg.py
 Comment: 
 
-Filename: libzac-0.0.6.dist-info/LICENSE
+Filename: libzac-0.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: libzac-0.0.6.dist-info/METADATA
+Filename: libzac-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: libzac-0.0.6.dist-info/WHEEL
+Filename: libzac-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: libzac-0.0.6.dist-info/top_level.txt
+Filename: libzac-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: libzac-0.0.6.dist-info/RECORD
+Filename: libzac-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `libzac-0.0.6.dist-info/LICENSE` & `libzac-0.0.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `libzac-0.0.6.dist-info/METADATA` & `libzac-0.0.7.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libzac
-Version: 0.0.6
+Version: 0.0.7
 Summary: A private use library
 Author-email: ZinGer_KyoN <zinger.kyon@gmail.com>
 License: MIT License        
         Copyright (c) [year] [fullname]        
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

## Comparing `libzac-0.0.6.dist-info/RECORD` & `libzac-0.0.7.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -2,12 +2,12 @@
 libzac/bitfield.py,sha256=qKBJ6Es05ULe6TSruQaqYicWnGb8wGepFz6KQBXJSE0,4799
 libzac/dsp.py,sha256=F12mmzC1Jau5jcPKD5F20xaLrWww8n5UTaGtqFBRSbI,1960
 libzac/e.py,sha256=G_CDpCA2nuG6HXWKJhPtgQEqvzOEwpCJf86v-y8QnqQ,2392
 libzac/io.py,sha256=lSEeJcG4klFP_YMo339so68dk3OGEUBQz_RThesaItQ,3007
 libzac/math.py,sha256=6Vy5TNSOTsje93v5T2jVX3gqWo4NFX9mNnzBomI1ahQ,1510
 libzac/plt.py,sha256=hM9rXy5scVtrXJMjclhvQEds88raY97C6efYz7o8d1w,3074
 libzac/reg.py,sha256=wJafUSflRACnqiUZIDi3_UPG8XYMwv0RMUei6X1WnP0,8791
-libzac-0.0.6.dist-info/LICENSE,sha256=Qv2ilebwoUtMJnRsZwRy729xS5JZQzLauJ0tQzkAkTA,1088
-libzac-0.0.6.dist-info/METADATA,sha256=M_XXoVPEPSUum2TVUvaZybWjg8J30Dtiap1Ryko3Fkg,1691
-libzac-0.0.6.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-libzac-0.0.6.dist-info/top_level.txt,sha256=4aG8bWAEZg_5zIiME4cwpZVGHvRZzdameIcLGWTf950,7
-libzac-0.0.6.dist-info/RECORD,,
+libzac-0.0.7.dist-info/LICENSE,sha256=Qv2ilebwoUtMJnRsZwRy729xS5JZQzLauJ0tQzkAkTA,1088
+libzac-0.0.7.dist-info/METADATA,sha256=0Ap0_E-A-CnY-5mxhm4JucWzGAVh1FPDM4eOCdD3h0s,1691
+libzac-0.0.7.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+libzac-0.0.7.dist-info/top_level.txt,sha256=4aG8bWAEZg_5zIiME4cwpZVGHvRZzdameIcLGWTf950,7
+libzac-0.0.7.dist-info/RECORD,,
```

