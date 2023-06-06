# Comparing `tmp/mb_sql-1.0.202305250344-py3-none-any.whl.zip` & `tmp/mb_sql-1.0.202306061249-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 10801 bytes, number of entries: 12
--rw-rw-r--  2.0 unx       43 b- defN 23-May-25 03:43 mb_sql/__init__.py
--rw-rw-r--  2.0 unx     3148 b- defN 23-May-23 16:18 mb_sql/conn.py
--rw-rw-r--  2.0 unx        0 b- defN 23-May-10 12:55 mb_sql/slack.py
--rw-rw-r--  2.0 unx     3667 b- defN 23-May-16 14:53 mb_sql/sql.py
--rw-rw-r--  2.0 unx     1669 b- defN 23-May-16 14:28 mb_sql/tables.py
--rw-rw-r--  2.0 unx    23143 b- defN 23-May-23 15:58 mb_sql/update.py
--rw-rw-r--  2.0 unx     5381 b- defN 23-May-17 01:01 mb_sql/utils.py
--rw-rw-r--  2.0 unx      396 b- defN 23-May-25 03:44 mb_sql/version.py
--rw-rw-r--  2.0 unx      239 b- defN 23-May-25 03:44 mb_sql-1.0.202305250344.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-25 03:44 mb_sql-1.0.202305250344.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-May-25 03:44 mb_sql-1.0.202305250344.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      911 b- defN 23-May-25 03:44 mb_sql-1.0.202305250344.dist-info/RECORD
-12 files, 38696 bytes uncompressed, 9283 bytes compressed:  76.0%
+Zip file size: 10800 bytes, number of entries: 12
+-rw-rw-r--  2.0 unx       43 b- defN 23-May-30 16:26 mb_sql/__init__.py
+-rw-rw-r--  2.0 unx     3148 b- defN 23-May-30 16:26 mb_sql/conn.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-May-30 16:26 mb_sql/slack.py
+-rw-rw-r--  2.0 unx     3667 b- defN 23-May-30 16:26 mb_sql/sql.py
+-rw-rw-r--  2.0 unx     1669 b- defN 23-May-30 16:26 mb_sql/tables.py
+-rw-rw-r--  2.0 unx    23143 b- defN 23-May-30 16:26 mb_sql/update.py
+-rw-rw-r--  2.0 unx     5381 b- defN 23-May-30 16:26 mb_sql/utils.py
+-rw-rw-r--  2.0 unx      396 b- defN 23-Jun-06 12:49 mb_sql/version.py
+-rw-rw-r--  2.0 unx      239 b- defN 23-Jun-06 12:49 mb_sql-1.0.202306061249.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-06 12:49 mb_sql-1.0.202306061249.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Jun-06 12:49 mb_sql-1.0.202306061249.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      911 b- defN 23-Jun-06 12:49 mb_sql-1.0.202306061249.dist-info/RECORD
+12 files, 38696 bytes uncompressed, 9282 bytes compressed:  76.0%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: mb_sql/utils.py
 Comment: 
 
 Filename: mb_sql/version.py
 Comment: 
 
-Filename: mb_sql-1.0.202305250344.dist-info/METADATA
+Filename: mb_sql-1.0.202306061249.dist-info/METADATA
 Comment: 
 
-Filename: mb_sql-1.0.202305250344.dist-info/WHEEL
+Filename: mb_sql-1.0.202306061249.dist-info/WHEEL
 Comment: 
 
-Filename: mb_sql-1.0.202305250344.dist-info/top_level.txt
+Filename: mb_sql-1.0.202306061249.dist-info/top_level.txt
 Comment: 
 
-Filename: mb_sql-1.0.202305250344.dist-info/RECORD
+Filename: mb_sql-1.0.202306061249.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mb_sql/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
-VERSION_MONTH = int('05')
-VERSION_DAY = int('25')
-VERSION_HOUR = int('03')
-VERSION_MINUTE = int('44')
+VERSION_MONTH = int('06')
+VERSION_DAY = int('06')
+VERSION_HOUR = int('12')
+VERSION_MINUTE = int('49')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202305250344
-version_date = '2023/05/25 03:44'
+PATCH_VERSION = 202306061249
+version_date = '2023/06/06 12:49'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `mb_sql-1.0.202305250344.dist-info/RECORD` & `mb_sql-1.0.202306061249.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 mb_sql/__init__.py,sha256=16ZetnIdcpfU3bmRa_MNC07b0I9bZWeJLSvN4UvCEHk,43
 mb_sql/conn.py,sha256=xL8QqVKd96tsXOdtXR7wVOWrmsRdffFFr3Tf2SFltU0,3148
 mb_sql/slack.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mb_sql/sql.py,sha256=hiSImhnoNGJvAkIAJYA5Vfjqkz-i0yHEXcIQel7JDK4,3667
 mb_sql/tables.py,sha256=xECYrXJKvdGvCPZo9vT1o7-HO0LoFjaD8602BQo4oO4,1669
 mb_sql/update.py,sha256=FpMA4KagDGS4bBGO83oGwYlwtry6KroriwWiJcz9bwE,23143
 mb_sql/utils.py,sha256=uYZSUhzFPKtu-yQuQFc4iRo9_f1FoUxm7HzWLiSezH0,5381
-mb_sql/version.py,sha256=uloKYX8UaccIhLXRTMSuQhSaBPb4h8xDBgTMRj1DVGc,396
-mb_sql-1.0.202305250344.dist-info/METADATA,sha256=oDQM8AwzzGlXPsRppDCu3YmxNA9W02qL1K8D8hSbY0c,239
-mb_sql-1.0.202305250344.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-mb_sql-1.0.202305250344.dist-info/top_level.txt,sha256=kO-6iZIJ_roadVPFvRH3vYSLJLMRKKCnXon2FncAa64,7
-mb_sql-1.0.202305250344.dist-info/RECORD,,
+mb_sql/version.py,sha256=YLd3VzTFBGxIL7U2me45470VEWG04gSRrB2j29MpMjo,396
+mb_sql-1.0.202306061249.dist-info/METADATA,sha256=i-Nu-CKR7NT_hvgs6JvoYV2vpqkkNzgXVcMUKrYXfYY,239
+mb_sql-1.0.202306061249.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+mb_sql-1.0.202306061249.dist-info/top_level.txt,sha256=kO-6iZIJ_roadVPFvRH3vYSLJLMRKKCnXon2FncAa64,7
+mb_sql-1.0.202306061249.dist-info/RECORD,,
```

