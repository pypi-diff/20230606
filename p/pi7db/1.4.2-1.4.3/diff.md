# Comparing `tmp/pi7db-1.4.2-py3-none-any.whl.zip` & `tmp/pi7db-1.4.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 24901 bytes, number of entries: 20
+Zip file size: 24923 bytes, number of entries: 20
 -rw-rw-r--  2.0 unx    16140 b- defN 22-Nov-08 18:42 pi7db/__init__.py
 -rw-rw-r--  2.0 unx      455 b- defN 21-Apr-11 11:13 pi7db/operators.py
 -rw-rw-r--  2.0 unx      952 b- defN 21-Apr-11 11:13 pi7db/cryptopidb/__init__.py
 -rw-rw-r--  2.0 unx     1246 b- defN 22-Jun-25 08:35 pi7db/filelock/__init__.py
 -rw-rw-r--  2.0 unx     8860 b- defN 22-Jun-25 08:35 pi7db/filelock/_api.py
 -rw-rw-r--  2.0 unx      399 b- defN 22-Jun-25 08:35 pi7db/filelock/_error.py
 -rw-rw-r--  2.0 unx     1650 b- defN 22-Jun-25 08:35 pi7db/filelock/_soft.py
 -rw-rw-r--  2.0 unx     1658 b- defN 22-Jun-25 11:30 pi7db/filelock/_unix.py
 -rw-rw-r--  2.0 unx      594 b- defN 22-Jun-25 08:35 pi7db/filelock/_util.py
 -rw-rw-r--  2.0 unx     1890 b- defN 22-Jun-25 08:35 pi7db/filelock/_windows.py
 -rw-rw-r--  2.0 unx      142 b- defN 22-Jun-25 08:35 pi7db/filelock/version.py
 -rw-rw-r--  2.0 unx        0 b- defN 21-Apr-11 11:13 pi7db/functions/__init__.py
--rw-rw-r--  2.0 unx    12147 b- defN 22-Dec-25 09:14 pi7db/functions/functions.py
+-rw-rw-r--  2.0 unx    12227 b- defN 23-Jan-18 13:15 pi7db/functions/functions.py
 -rw-rw-r--  2.0 unx     1878 b- defN 21-May-26 14:07 pi7db/functions/subclass.py
 -rw-rw-r--  2.0 unx     1912 b- defN 22-Jun-25 10:14 pi7db/status/__init__.py
--rwxr-xr-x  2.0 unx     1074 b- defN 22-Dec-26 05:59 pi7db-1.4.2.dist-info/LICENSE
--rw-rw-r--  2.0 unx    25452 b- defN 22-Dec-26 05:59 pi7db-1.4.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Dec-26 05:59 pi7db-1.4.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx        6 b- defN 22-Dec-26 05:59 pi7db-1.4.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1586 b- defN 22-Dec-26 05:59 pi7db-1.4.2.dist-info/RECORD
-20 files, 78133 bytes uncompressed, 22339 bytes compressed:  71.4%
+-rwxr-xr-x  2.0 unx     1074 b- defN 23-Jan-18 13:17 pi7db-1.4.3.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    25452 b- defN 23-Jan-18 13:17 pi7db-1.4.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jan-18 13:17 pi7db-1.4.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        6 b- defN 23-Jan-18 13:17 pi7db-1.4.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1586 b- defN 23-Jan-18 13:17 pi7db-1.4.3.dist-info/RECORD
+20 files, 78213 bytes uncompressed, 22361 bytes compressed:  71.4%
```

## zipnote {}

```diff
@@ -39,23 +39,23 @@
 
 Filename: pi7db/functions/subclass.py
 Comment: 
 
 Filename: pi7db/status/__init__.py
 Comment: 
 
-Filename: pi7db-1.4.2.dist-info/LICENSE
+Filename: pi7db-1.4.3.dist-info/LICENSE
 Comment: 
 
-Filename: pi7db-1.4.2.dist-info/METADATA
+Filename: pi7db-1.4.3.dist-info/METADATA
 Comment: 
 
-Filename: pi7db-1.4.2.dist-info/WHEEL
+Filename: pi7db-1.4.3.dist-info/WHEEL
 Comment: 
 
-Filename: pi7db-1.4.2.dist-info/top_level.txt
+Filename: pi7db-1.4.3.dist-info/top_level.txt
 Comment: 
 
-Filename: pi7db-1.4.2.dist-info/RECORD
+Filename: pi7db-1.4.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pi7db/functions/functions.py

```diff
@@ -78,15 +78,17 @@
           else:
            for x in d_dict[key]:
             for xx in value:
               if isinstance(xx, set):
                for xxx in xx:x.pop(xxx)
               elif "$where" and "$keys" in xx:
                if findDiff(xx['$where'],x):
-                for xk in xx['$keys']:x.pop(xk)
+                for xk in xx['$keys']:
+                  if xk in x:
+                    x.pop(xk)
               else:nes_trash(x,xx)
            [d_dict[key].remove(x) for x in d_dict[key] if len(x) == 0]
     return d_dict
 
 def trashbyfilter(dic_data,key_name,config):
  if len(dic_data):
   all_trash = []
@@ -238,15 +240,15 @@
 
 def checkli_stin(l1,l2,config):
   return all([True if any(string_filter(x,item,config) for item in l2) else False for x in l1])
 
 def string_filter(d1,d2,config):
    try:
     if "senstive_case" in config and config["senstive_case"] == False:d1,d2=d1.lower(),d2.lower()
-    if d1[-2:] == '*' and d1[:2] == '*':
+    if d1[-2:] == '**' and d1[:2] == '**':
         if d1[:-2][2:] in d2:return True
     elif d1[-2:] == '**':return d2.startswith(d1[:-2])
     elif d1[:2] == '**':return d2.endswith(d1[2:])
     elif d1 == d2:return True
     else:return False
    except:return False
 
@@ -269,21 +271,22 @@
           if findDiff(d1[key],d2[key]) is False:return False
         elif type(d1[key]) is list:
           if all(isinstance(s, dict) for s in d1[key]):
             if checklist(d1[key],d2[key]) is False:return False
           if all(isinstance(s, str) for s in d1[key]) or all(isinstance(i, int) for i in d1[key]):
             if not checkli_stin(d1[key],d2[key],config):return False
         else:
+          # <,> = Operators
           if isinstance(d1[key],tuple):
             if not check_GT_LT(d1[key],d2[key]):return False
           # STRING FILTER
           elif isinstance(d1[key],str):
             if not string_filter(d1[key],d2[key],config):return False
           elif d1[key] == d2[key]:pass
           else:return False
     return True
     
 def andfilter(command_tup,all_data,kwargs):
   return [x for x in all_data if findDiff(command_tup,x,kwargs) is True][kwargs['f_a']:kwargs['l_a']]
 
 def create_coll(path):
-  if not os.path.exists(path):os.mkdir(path)
+  if not os.path.exists(path):os.mkdir(path)
```

## Comparing `pi7db-1.4.2.dist-info/LICENSE` & `pi7db-1.4.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pi7db-1.4.2.dist-info/METADATA` & `pi7db-1.4.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pi7db
-Version: 1.4.2
+Version: 1.4.3
 Summary: pi7db Is A Fast And Powerfull Directory Based Database Built In Python3.
 Home-page: https://github.com/shivjeetbhullar/pi7db
 Author: Shivjeet Singh Bhullar
 Author-email: bhullarshivjeet@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `pi7db-1.4.2.dist-info/RECORD` & `pi7db-1.4.3.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 pi7db/filelock/_error.py,sha256=Gaxp2TfdmgdvYFkllGCBOE37vYIXnHKKW3RYfKH7DYM,399
 pi7db/filelock/_soft.py,sha256=rSpmt4Oi0Eb4JeKzyWImeqf5MYCJR0Dyc_kUN3kHj7Y,1650
 pi7db/filelock/_unix.py,sha256=HxVsgsDy4aUku9phZF_QBe3LbIIhXaFVtAxdd_MM1go,1658
 pi7db/filelock/_util.py,sha256=BZKOAYTQdmcHmF34-Ft4kMdEvk3a8NGtsAhe6kfxZuU,594
 pi7db/filelock/_windows.py,sha256=wvg-_SfJEDyxDeDVH8wBqxbPquXaycoYXgXJOBmm-G4,1890
 pi7db/filelock/version.py,sha256=9aLd-KoN-y8Y2gRKw7z6WVYrMEaHPtFGPxC-kvG_yik,142
 pi7db/functions/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pi7db/functions/functions.py,sha256=P7_g0mIBsCxnfHMzktIkWcgfyzNIa69Ni5DFDcrXUD8,12147
+pi7db/functions/functions.py,sha256=OfR4tiXAfStMlLzWGFjkbJiDRJ68VcDoDrGwt_B_HL8,12227
 pi7db/functions/subclass.py,sha256=MZ4f6Z-xQ0_2vODyR4tbzVXP5wOIwEkS1AP3iMOHgKM,1878
 pi7db/status/__init__.py,sha256=tXUyEU7qnCGhvGwYxlWPvkY8l35yeuDwRpXeoioGrxc,1912
-pi7db-1.4.2.dist-info/LICENSE,sha256=7EI8xVBu6h_7_JlVw-yPhhOZlpY9hP8wal7kHtqKT_E,1074
-pi7db-1.4.2.dist-info/METADATA,sha256=rFsGzfz0TN383pSQk5Ao6KrtzlK0zrWWODhpRr3JrkA,25452
-pi7db-1.4.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pi7db-1.4.2.dist-info/top_level.txt,sha256=lwaKdaztFKNGMAtSZecvPaPs9bLoyvujfhMB4seDAiw,6
-pi7db-1.4.2.dist-info/RECORD,,
+pi7db-1.4.3.dist-info/LICENSE,sha256=7EI8xVBu6h_7_JlVw-yPhhOZlpY9hP8wal7kHtqKT_E,1074
+pi7db-1.4.3.dist-info/METADATA,sha256=tQgooo0xNe15B025H59sVQODg_mKDTGWI-NItCplHZs,25452
+pi7db-1.4.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pi7db-1.4.3.dist-info/top_level.txt,sha256=lwaKdaztFKNGMAtSZecvPaPs9bLoyvujfhMB4seDAiw,6
+pi7db-1.4.3.dist-info/RECORD,,
```

