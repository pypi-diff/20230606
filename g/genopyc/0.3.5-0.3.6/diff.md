# Comparing `tmp/genopyc-0.3.5-py3-none-any.whl.zip` & `tmp/genopyc-0.3.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 18393 bytes, number of entries: 7
--rwxrwxrwx  2.0 unx      881 b- defN 23-May-31 11:38 genopyc/__init__.py
+Zip file size: 18390 bytes, number of entries: 7
+-rwxrwxrwx  2.0 unx      881 b- defN 23-Jun-06 08:23 genopyc/__init__.py
 -rwxrwxrwx  2.0 unx    24058 b- defN 23-May-31 11:38 genopyc/genopyc.py
--rwxrwxrwx  2.0 unx    34523 b- defN 23-May-31 11:39 genopyc-0.3.5.dist-info/LICENSE.txt
--rwxrwxrwx  2.0 unx      463 b- defN 23-May-31 11:39 genopyc-0.3.5.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 23-May-31 11:39 genopyc-0.3.5.dist-info/WHEEL
--rwxrwxrwx  2.0 unx        8 b- defN 23-May-31 11:39 genopyc-0.3.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      540 b- defN 23-May-31 11:39 genopyc-0.3.5.dist-info/RECORD
-7 files, 60565 bytes uncompressed, 17439 bytes compressed:  71.2%
+-rwxrwxrwx  2.0 unx    34523 b- defN 23-Jun-06 08:24 genopyc-0.3.6.dist-info/LICENSE.txt
+-rwxrwxrwx  2.0 unx      463 b- defN 23-Jun-06 08:24 genopyc-0.3.6.dist-info/METADATA
+-rwxrwxrwx  2.0 unx       92 b- defN 23-Jun-06 08:24 genopyc-0.3.6.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx        8 b- defN 23-Jun-06 08:24 genopyc-0.3.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      540 b- defN 23-Jun-06 08:24 genopyc-0.3.6.dist-info/RECORD
+7 files, 60565 bytes uncompressed, 17436 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: genopyc/__init__.py
 Comment: 
 
 Filename: genopyc/genopyc.py
 Comment: 
 
-Filename: genopyc-0.3.5.dist-info/LICENSE.txt
+Filename: genopyc-0.3.6.dist-info/LICENSE.txt
 Comment: 
 
-Filename: genopyc-0.3.5.dist-info/METADATA
+Filename: genopyc-0.3.6.dist-info/METADATA
 Comment: 
 
-Filename: genopyc-0.3.5.dist-info/WHEEL
+Filename: genopyc-0.3.6.dist-info/WHEEL
 Comment: 
 
-Filename: genopyc-0.3.5.dist-info/top_level.txt
+Filename: genopyc-0.3.6.dist-info/top_level.txt
 Comment: 
 
-Filename: genopyc-0.3.5.dist-info/RECORD
+Filename: genopyc-0.3.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## genopyc/__init__.py

```diff
@@ -12,9 +12,9 @@
 from genopyc.genopyc import grch_liftover
 from genopyc.genopyc import get_eqtl_variant
 from genopyc.genopyc import get_variant_info
 from genopyc.genopyc import get_variant_info_many
 from genopyc.genopyc import get_eqtl_df
 from genopyc.genopyc import GetLDMatrix
 from genopyc.genopyc import PairwiseLD
-from genopyc.genopyc import ConvertVariantsforOT
+from genopyc.genopyc import ConvertVariantsForOT
 from genopyc.genopyc import OT_L2G
```

## Comparing `genopyc-0.3.5.dist-info/LICENSE.txt` & `genopyc-0.3.6.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `genopyc-0.3.5.dist-info/RECORD` & `genopyc-0.3.6.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-genopyc/__init__.py,sha256=ArAdiVFj7X9ySAYMBXsWWsq2s5bOHrBFpXLa-9GxvJA,881
+genopyc/__init__.py,sha256=3z4lkHm96s2STIaZSzjDJbKJNwvyQvZAOZnIW6scDZI,881
 genopyc/genopyc.py,sha256=Ug4T7TXnYZrtTBW4yydKTrFH0maIDgUOApJwrUHwm18,24058
-genopyc-0.3.5.dist-info/LICENSE.txt,sha256=hIahDEOTzuHCU5J2nd07LWwkLW7Hko4UFO__ffsvB-8,34523
-genopyc-0.3.5.dist-info/METADATA,sha256=TuZFm5a849uORNLj5ov8FlvJ20YtUmIG5O2UItYuM8A,463
-genopyc-0.3.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-genopyc-0.3.5.dist-info/top_level.txt,sha256=Wo4uco8QIcmZcoQJmxDYvrDatX_GrmASBAr5wSeBevA,8
-genopyc-0.3.5.dist-info/RECORD,,
+genopyc-0.3.6.dist-info/LICENSE.txt,sha256=hIahDEOTzuHCU5J2nd07LWwkLW7Hko4UFO__ffsvB-8,34523
+genopyc-0.3.6.dist-info/METADATA,sha256=jtmek9abhOzq6X_t5PIQze0O_AY3xQN6AgUkgA4n4q4,463
+genopyc-0.3.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+genopyc-0.3.6.dist-info/top_level.txt,sha256=Wo4uco8QIcmZcoQJmxDYvrDatX_GrmASBAr5wSeBevA,8
+genopyc-0.3.6.dist-info/RECORD,,
```

