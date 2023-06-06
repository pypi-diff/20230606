# Comparing `tmp/mb_sql-1.0.202306061249-py3-none-any.whl.zip` & `tmp/mb_sql-1.0.202306061653-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 10800 bytes, number of entries: 12
+Zip file size: 11082 bytes, number of entries: 12
 -rw-rw-r--  2.0 unx       43 b- defN 23-May-30 16:26 mb_sql/__init__.py
 -rw-rw-r--  2.0 unx     3148 b- defN 23-May-30 16:26 mb_sql/conn.py
--rw-rw-r--  2.0 unx        0 b- defN 23-May-30 16:26 mb_sql/slack.py
+-rw-rw-r--  2.0 unx      519 b- defN 23-Jun-06 16:40 mb_sql/slack.py
 -rw-rw-r--  2.0 unx     3667 b- defN 23-May-30 16:26 mb_sql/sql.py
 -rw-rw-r--  2.0 unx     1669 b- defN 23-May-30 16:26 mb_sql/tables.py
 -rw-rw-r--  2.0 unx    23143 b- defN 23-May-30 16:26 mb_sql/update.py
 -rw-rw-r--  2.0 unx     5381 b- defN 23-May-30 16:26 mb_sql/utils.py
--rw-rw-r--  2.0 unx      396 b- defN 23-Jun-06 12:49 mb_sql/version.py
--rw-rw-r--  2.0 unx      239 b- defN 23-Jun-06 12:49 mb_sql-1.0.202306061249.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-06 12:49 mb_sql-1.0.202306061249.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Jun-06 12:49 mb_sql-1.0.202306061249.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      911 b- defN 23-Jun-06 12:49 mb_sql-1.0.202306061249.dist-info/RECORD
-12 files, 38696 bytes uncompressed, 9282 bytes compressed:  76.0%
+-rw-rw-r--  2.0 unx      396 b- defN 23-Jun-06 16:53 mb_sql/version.py
+-rw-rw-r--  2.0 unx      239 b- defN 23-Jun-06 16:53 mb_sql-1.0.202306061653.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-06 16:53 mb_sql-1.0.202306061653.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Jun-06 16:53 mb_sql-1.0.202306061653.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      913 b- defN 23-Jun-06 16:53 mb_sql-1.0.202306061653.dist-info/RECORD
+12 files, 39217 bytes uncompressed, 9564 bytes compressed:  75.6%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: mb_sql/utils.py
 Comment: 
 
 Filename: mb_sql/version.py
 Comment: 
 
-Filename: mb_sql-1.0.202306061249.dist-info/METADATA
+Filename: mb_sql-1.0.202306061653.dist-info/METADATA
 Comment: 
 
-Filename: mb_sql-1.0.202306061249.dist-info/WHEEL
+Filename: mb_sql-1.0.202306061653.dist-info/WHEEL
 Comment: 
 
-Filename: mb_sql-1.0.202306061249.dist-info/top_level.txt
+Filename: mb_sql-1.0.202306061653.dist-info/top_level.txt
 Comment: 
 
-Filename: mb_sql-1.0.202306061249.dist-info/RECORD
+Filename: mb_sql-1.0.202306061653.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mb_sql/slack.py

```diff
@@ -0,0 +1,33 @@
+00000000: 696d 706f 7274 2072 6571 7565 7374 730a  import requests.
+00000010: 696d 706f 7274 206a 736f 6e0a 0a5f 5f61  import json..__a
+00000020: 6c6c 5f5f 203d 205b 2773 6c61 636b 5f6d  ll__ = ['slack_m
+00000030: 7367 275d 0a0a 6465 6620 736c 6163 6b5f  sg']..def slack_
+00000040: 6d73 6728 7765 6268 6f6f 6b2c 6d73 672c  msg(webhook,msg,
+00000050: 6c6f 6767 6572 3d4e 6f6e 6529 3a0a 2020  logger=None):.  
+00000060: 2020 2222 220a 2020 2020 5365 6e64 2061    """.    Send a
+00000070: 206d 6573 7361 6765 2074 6f20 6120 736c   message to a sl
+00000080: 6163 6b20 6368 616e 6e65 6c0a 2020 2020  ack channel.    
+00000090: 4172 6773 3a0a 2020 2020 2020 2020 7765  Args:.        we
+000000a0: 6268 6f6f 6b20 2873 7472 293a 2053 6c61  bhook (str): Sla
+000000b0: 636b 2077 6562 686f 6f6b 2055 524c 0a20  ck webhook URL. 
+000000c0: 2020 2020 2020 206d 7367 2028 7374 7229         msg (str)
+000000d0: 3a20 4d65 7373 6167 6520 746f 2073 656e  : Message to sen
+000000e0: 640a 2020 2020 2020 2020 6c6f 6767 6572  d.        logger
+000000f0: 2028 6c6f 6767 696e 672e 4c6f 6767 6572   (logging.Logger
+00000100: 293a 204c 6f67 6765 7220 746f 2075 7365  ): Logger to use
+00000110: 0a20 2020 2052 6574 7572 6e73 3a0a 2020  .    Returns:.  
+00000120: 2020 2020 2020 4e6f 6e65 0a20 2020 2022        None.    "
+00000130: 2222 0a20 2020 200a 2020 2020 7265 7370  "".    .    resp
+00000140: 6f6e 7365 203d 2072 6571 7565 7374 732e  onse = requests.
+00000150: 706f 7374 280a 2020 2020 2020 2020 7572  post(.        ur
+00000160: 6c3d 7765 6268 6f6f 6b2c 0a20 2020 2020  l=webhook,.     
+00000170: 2020 2064 6174 613d 6a73 6f6e 2e64 756d     data=json.dum
+00000180: 7073 286d 7367 292c 0a20 2020 2020 2020  ps(msg),.       
+00000190: 2068 6561 6465 7273 3d7b 2743 6f6e 7465   headers={'Conte
+000001a0: 6e74 2d54 7970 6527 3a20 2761 7070 6c69  nt-Type': 'appli
+000001b0: 6361 7469 6f6e 2f6a 736f 6e27 7d29 0a0a  cation/json'})..
+000001c0: 2020 2020 6966 206c 6f67 6765 723a 0a20      if logger:. 
+000001d0: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
+000001e0: 666f 2827 536c 6163 6b20 7265 7370 6f6e  fo('Slack respon
+000001f0: 7365 3a20 2573 272c 2072 6573 706f 6e73  se: %s', respons
+00000200: 652e 7465 7874 29                        e.text)
```

## mb_sql/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('06')
 VERSION_DAY = int('06')
-VERSION_HOUR = int('12')
-VERSION_MINUTE = int('49')
+VERSION_HOUR = int('16')
+VERSION_MINUTE = int('53')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202306061249
-version_date = '2023/06/06 12:49'
+PATCH_VERSION = 202306061653
+version_date = '2023/06/06 16:53'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `mb_sql-1.0.202306061249.dist-info/RECORD` & `mb_sql-1.0.202306061653.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 mb_sql/__init__.py,sha256=16ZetnIdcpfU3bmRa_MNC07b0I9bZWeJLSvN4UvCEHk,43
 mb_sql/conn.py,sha256=xL8QqVKd96tsXOdtXR7wVOWrmsRdffFFr3Tf2SFltU0,3148
-mb_sql/slack.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+mb_sql/slack.py,sha256=ReoopG_NXhT1qdY_Ip5RrBwJ1Y27HuZBE2tfw3JXP14,519
 mb_sql/sql.py,sha256=hiSImhnoNGJvAkIAJYA5Vfjqkz-i0yHEXcIQel7JDK4,3667
 mb_sql/tables.py,sha256=xECYrXJKvdGvCPZo9vT1o7-HO0LoFjaD8602BQo4oO4,1669
 mb_sql/update.py,sha256=FpMA4KagDGS4bBGO83oGwYlwtry6KroriwWiJcz9bwE,23143
 mb_sql/utils.py,sha256=uYZSUhzFPKtu-yQuQFc4iRo9_f1FoUxm7HzWLiSezH0,5381
-mb_sql/version.py,sha256=YLd3VzTFBGxIL7U2me45470VEWG04gSRrB2j29MpMjo,396
-mb_sql-1.0.202306061249.dist-info/METADATA,sha256=i-Nu-CKR7NT_hvgs6JvoYV2vpqkkNzgXVcMUKrYXfYY,239
-mb_sql-1.0.202306061249.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-mb_sql-1.0.202306061249.dist-info/top_level.txt,sha256=kO-6iZIJ_roadVPFvRH3vYSLJLMRKKCnXon2FncAa64,7
-mb_sql-1.0.202306061249.dist-info/RECORD,,
+mb_sql/version.py,sha256=A_K4mCesjmYX6gu8KdzvPh8zoSTGTURGOuRe9B1uLDo,396
+mb_sql-1.0.202306061653.dist-info/METADATA,sha256=EoPp2yIEcFRSMrx2C4CfQ5DuRGxERi6JGo8fG0RT9UU,239
+mb_sql-1.0.202306061653.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+mb_sql-1.0.202306061653.dist-info/top_level.txt,sha256=kO-6iZIJ_roadVPFvRH3vYSLJLMRKKCnXon2FncAa64,7
+mb_sql-1.0.202306061653.dist-info/RECORD,,
```

