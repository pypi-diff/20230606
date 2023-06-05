# Comparing `tmp/intelicity-0.0.8-py3-none-any.whl.zip` & `tmp/intelicity-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,25 +1,25 @@
-Zip file size: 19280 bytes, number of entries: 23
+Zip file size: 19369 bytes, number of entries: 23
 -rw-rw-r--  2.0 unx      198 b- defN 23-Jun-02 15:43 intelicity/__init__.py
--rw-rw-r--  2.0 unx     2425 b- defN 23-Jun-01 15:15 intelicity/ai_object.py
+-rw-rw-r--  2.0 unx     2566 b- defN 23-Jun-05 23:01 intelicity/ai_object.py
 -rw-rw-r--  2.0 unx     6322 b- defN 23-May-31 16:18 intelicity/bound_box.py
 -rw-rw-r--  2.0 unx     3387 b- defN 23-Jun-05 21:47 intelicity/containers.py
--rw-rw-r--  2.0 unx     6812 b- defN 23-Jun-05 21:26 intelicity/contents.py
+-rw-rw-r--  2.0 unx     6826 b- defN 23-Jun-05 23:06 intelicity/contents.py
 -rw-rw-r--  2.0 unx     1227 b- defN 23-Jun-05 21:47 intelicity/file_header.py
 -rw-rw-r--  2.0 unx     2656 b- defN 23-Jun-01 14:37 intelicity/geo_location.py
 -rw-rw-r--  2.0 unx     1471 b- defN 23-Jun-01 15:59 intelicity/image.py
 -rw-rw-r--  2.0 unx     4411 b- defN 23-May-24 20:18 intelicity/main.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-02 13:45 src/__init__.py
 -rw-rw-r--  2.0 unx     2425 b- defN 23-Jun-01 15:15 src/ai_object.py
 -rw-rw-r--  2.0 unx     6322 b- defN 23-May-31 16:18 src/bound_box.py
 -rw-rw-r--  2.0 unx     3335 b- defN 23-Jun-02 13:23 src/containers.py
 -rw-rw-r--  2.0 unx     6699 b- defN 23-Jun-02 13:23 src/contents.py
 -rw-rw-r--  2.0 unx     1171 b- defN 23-Jun-02 13:24 src/file_header.py
 -rw-rw-r--  2.0 unx     2656 b- defN 23-Jun-01 14:37 src/geo_location.py
 -rw-rw-r--  2.0 unx     1471 b- defN 23-Jun-01 15:59 src/image.py
 -rw-rw-r--  2.0 unx     4411 b- defN 23-May-24 20:18 src/main.py
--rw-rw-r--  2.0 unx     1074 b- defN 23-Jun-05 21:51 intelicity-0.0.8.dist-info/LICENSE
--rw-rw-r--  2.0 unx      643 b- defN 23-Jun-05 21:51 intelicity-0.0.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-05 21:51 intelicity-0.0.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 23-Jun-05 21:51 intelicity-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1763 b- defN 23-Jun-05 21:51 intelicity-0.0.8.dist-info/RECORD
-23 files, 60982 bytes uncompressed, 16480 bytes compressed:  73.0%
+-rw-rw-r--  2.0 unx     1074 b- defN 23-Jun-05 23:07 intelicity-0.0.9.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      643 b- defN 23-Jun-05 23:07 intelicity-0.0.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-05 23:07 intelicity-0.0.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 23-Jun-05 23:07 intelicity-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1763 b- defN 23-Jun-05 23:07 intelicity-0.0.9.dist-info/RECORD
+23 files, 61137 bytes uncompressed, 16569 bytes compressed:  72.9%
```

## zipnote {}

```diff
@@ -48,23 +48,23 @@
 
 Filename: src/image.py
 Comment: 
 
 Filename: src/main.py
 Comment: 
 
-Filename: intelicity-0.0.8.dist-info/LICENSE
+Filename: intelicity-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: intelicity-0.0.8.dist-info/METADATA
+Filename: intelicity-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: intelicity-0.0.8.dist-info/WHEEL
+Filename: intelicity-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: intelicity-0.0.8.dist-info/top_level.txt
+Filename: intelicity-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: intelicity-0.0.8.dist-info/RECORD
+Filename: intelicity-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## intelicity/ai_object.py

```diff
@@ -50,16 +50,17 @@
     @classmethod
     def get_object_name(cls, ai_id : int) -> str:
         if ai_id in cls.object_table.keys():
             return cls.get_object_name_or_default(ai_id)
         else:
             raise Exception(cls.get_object_name_or_default(ai_id))
 
-    def __init__(self, global_ai_id : int):
+    def __init__(self, global_ai_id : int, name=""):
         self.ai_id = global_ai_id
+        self.name = name
 
     @classmethod
     def create_from_local_id(cls, local_object_id: int, local_root_object_id: int) -> "AiObject":
         ai_object = AiObject(local_object_id + local_root_object_id)
         return ai_object
 
     @classmethod
@@ -69,12 +70,15 @@
 
     def get_local_id(self, local_root_object_id: int) -> int:
         return self.ai_id - local_root_object_id
 
     def get_global_id(self) -> int:
         return self.ai_id
 
+    def get_name(self):
+        return self.get_object_name(self.ai_id) if self.name is "" else self.name
+
     def __eq__(self, other):
         if isinstance(other, AiObject):
             return self.ai_id == other.ai_id
         else:
             return False
```

## intelicity/contents.py

```diff
@@ -24,16 +24,16 @@
         [7] latitude\n
         [8] longitude\n
     """
     @classmethod
     def create_from_line(cls, string: str):
 
         segments = cls.parse(string)
-
-        ai_object = AiObject.create_from_global_id(int(segments[0]))
+        ai_name = segments[6]
+        ai_object = AiObject(int(segments[0]), ai_name)
         pixel_space_center_x = int(segments[1])
         pixel_space_center_y = int(segments[2])
         pixel_space_size_x = int(segments[3])
         pixel_space_size_y = int(segments[4])
         trust = float(segments[5])
 
         geo_location = GeoLocation.create_from_string(segments[7], segments[8])
@@ -118,22 +118,20 @@
         self.screen_bound_box = screen_bound_box
         self.trust = trust
 
     @classmethod
     def create_from_line(cls, string: str, local_root_object_id=0) -> "NetworkOutputContent":
 
         segments = cls.parse(string)
-
         ai_object = AiObject.create_from_local_id(int(segments[0]),local_root_object_id)
         screen_space_center_x = float(segments[1])
         screen_space_center_y = float(segments[2])
         screen_space_size_x = float(segments[3])
         screen_space_size_y = float(segments[4])
         trust = float(segments[5])
-
         screen_bound_box = BoundBox(screen_space_center_x, screen_space_center_y, screen_space_size_x, screen_space_size_y)
         return cls(ai_object, screen_bound_box, trust)
 
     def __str__(self):
         return f"{self.ai_object.get_global_id()} {str(self.screen_bound_box)} {self.trust}"
 
     def __repr__(self):
```

## Comparing `intelicity-0.0.8.dist-info/LICENSE` & `intelicity-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `intelicity-0.0.8.dist-info/METADATA` & `intelicity-0.0.9.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intelicity
-Version: 0.0.8
+Version: 0.0.9
 Summary: a library for reading and managing data from the Intelicity server
 Author: Me
 Author-email: Felipe Rodrigues Peixoto da Silva <frps2003@gmail.com>
 License: MIT
 Project-URL: Homepage, https://inteli.city/
 Project-URL: project, https://github.com/Comunalti/Intelicity_Library
 Classifier: Programming Language :: Python :: 3
```

## Comparing `intelicity-0.0.8.dist-info/RECORD` & `intelicity-0.0.9.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 intelicity/__init__.py,sha256=9altPjTiEzAuopDxqZp8lxcRVVQy6ljkePJykZhhKGs,198
-intelicity/ai_object.py,sha256=3o5XYoWvj3v0onvcF0gVkmYmXb-YM3BKSDB-vMPovNc,2425
+intelicity/ai_object.py,sha256=Szk7kj6aVuyltb8pN_iFhAqZc9Ufz8IoRdLx5eCF0l8,2566
 intelicity/bound_box.py,sha256=XvsWJz0R_dq3Mf8BdZc6mAARlOUgagbm3ZsiVFHW_sE,6322
 intelicity/containers.py,sha256=tah1soBkAWdcFNY6TU7Zu1WYeFKflawQ7DrIQ_binrI,3387
-intelicity/contents.py,sha256=HZLC6swlVvt8b50JUkSMPpsNhq1iU2fBdMdI__9y66o,6812
+intelicity/contents.py,sha256=TDADk2Kk-BV7ictJ_qC459TwMKrmxB3rqfudTdkDRfQ,6826
 intelicity/file_header.py,sha256=buYfFX4j_FEYda4RaKUC2lceVWZG7fyuUDYp8W13aLY,1227
 intelicity/geo_location.py,sha256=r7oxnWKtIYavuGAySgQhhYpKNB3o-bs7-NnPq_ykvqY,2656
 intelicity/image.py,sha256=F8s6myDP8KlWPgRfW9PObH-mFqUjxPMSrW7e6W3MQPg,1471
 intelicity/main.py,sha256=lWFAod5cs5XuGfR63v-81omq_dzKtghlisJRf6DDrF8,4411
 src/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 src/ai_object.py,sha256=3o5XYoWvj3v0onvcF0gVkmYmXb-YM3BKSDB-vMPovNc,2425
 src/bound_box.py,sha256=XvsWJz0R_dq3Mf8BdZc6mAARlOUgagbm3ZsiVFHW_sE,6322
 src/containers.py,sha256=lmFi2ycZdA2iwqrY0vWsZG89QY81kEdsoVlP0IWJwRY,3335
 src/contents.py,sha256=8OQTCisgAt7W8kV0Kbz5Qeo7PhtwobRM4Ssmw1vFAY0,6699
 src/file_header.py,sha256=PpvZii5xMJhZMlVOlg2vmKHApM8kQvFB-ck-dV3j-bk,1171
 src/geo_location.py,sha256=r7oxnWKtIYavuGAySgQhhYpKNB3o-bs7-NnPq_ykvqY,2656
 src/image.py,sha256=F8s6myDP8KlWPgRfW9PObH-mFqUjxPMSrW7e6W3MQPg,1471
 src/main.py,sha256=lWFAod5cs5XuGfR63v-81omq_dzKtghlisJRf6DDrF8,4411
-intelicity-0.0.8.dist-info/LICENSE,sha256=7EI8xVBu6h_7_JlVw-yPhhOZlpY9hP8wal7kHtqKT_E,1074
-intelicity-0.0.8.dist-info/METADATA,sha256=MlLRKuxkHD4pM0o1u31QsyKhybmxfQ77WifV84L0Hk0,643
-intelicity-0.0.8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-intelicity-0.0.8.dist-info/top_level.txt,sha256=xHp1PhuI3caIPBFop84FTTiU1c_X4APlwoYvQkmTBcw,11
-intelicity-0.0.8.dist-info/RECORD,,
+intelicity-0.0.9.dist-info/LICENSE,sha256=7EI8xVBu6h_7_JlVw-yPhhOZlpY9hP8wal7kHtqKT_E,1074
+intelicity-0.0.9.dist-info/METADATA,sha256=HxPyxhmQckctBFr6r8HTJu5tckOI9BHmznNKPyPpbTo,643
+intelicity-0.0.9.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+intelicity-0.0.9.dist-info/top_level.txt,sha256=xHp1PhuI3caIPBFop84FTTiU1c_X4APlwoYvQkmTBcw,11
+intelicity-0.0.9.dist-info/RECORD,,
```

