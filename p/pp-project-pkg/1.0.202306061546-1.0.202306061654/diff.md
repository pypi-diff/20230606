# Comparing `tmp/pp_project_pkg-1.0.202306061546-py3-none-any.whl.zip` & `tmp/pp_project_pkg-1.0.202306061654-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 7574 bytes, number of entries: 12
+Zip file size: 7568 bytes, number of entries: 12
 -rw-rw-r--  2.0 unx       71 b- defN 23-Jun-06 14:15 pp_project_pkg/__init__.py
 -rw-rw-r--  2.0 unx      577 b- defN 23-Jun-06 14:14 pp_project_pkg/newsvendor.py
 -rw-rw-r--  2.0 unx     7115 b- defN 23-Jun-06 15:26 pp_project_pkg/pp_tables.py
 -rw-rw-r--  2.0 unx     1203 b- defN 23-Jun-06 15:46 pp_project_pkg/utils.py
--rw-rw-r--  2.0 unx      396 b- defN 23-Jun-06 15:46 pp_project_pkg/version.py
+-rw-rw-r--  2.0 unx      396 b- defN 23-Jun-06 16:54 pp_project_pkg/version.py
 -rw-rw-r--  2.0 unx     4391 b- defN 23-Jun-06 15:29 pp_project_pkg/wrangling.py
--rwxrwxr-x  2.0 unx       65 b- defN 23-Jun-06 09:53 pp_project_pkg-1.0.202306061546.data/scripts/get_tables.py
--rwxrwxr-x  2.0 unx     1328 b- defN 23-Jun-06 15:30 pp_project_pkg-1.0.202306061546.data/scripts/pp_project_run.py
--rw-rw-r--  2.0 unx      191 b- defN 23-Jun-06 15:46 pp_project_pkg-1.0.202306061546.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-06 15:46 pp_project_pkg-1.0.202306061546.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-06 15:46 pp_project_pkg-1.0.202306061546.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1095 b- defN 23-Jun-06 15:46 pp_project_pkg-1.0.202306061546.dist-info/RECORD
-12 files, 16539 bytes uncompressed, 5688 bytes compressed:  65.6%
+-rwxrwxr-x  2.0 unx       65 b- defN 23-Jun-06 09:53 pp_project_pkg-1.0.202306061654.data/scripts/get_tables.py
+-rwxrwxr-x  2.0 unx     1316 b- defN 23-Jun-06 15:48 pp_project_pkg-1.0.202306061654.data/scripts/pp_project_run.py
+-rw-rw-r--  2.0 unx      191 b- defN 23-Jun-06 16:54 pp_project_pkg-1.0.202306061654.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-06 16:54 pp_project_pkg-1.0.202306061654.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-Jun-06 16:54 pp_project_pkg-1.0.202306061654.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1095 b- defN 23-Jun-06 16:54 pp_project_pkg-1.0.202306061654.dist-info/RECORD
+12 files, 16527 bytes uncompressed, 5682 bytes compressed:  65.6%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: pp_project_pkg/version.py
 Comment: 
 
 Filename: pp_project_pkg/wrangling.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306061546.data/scripts/get_tables.py
+Filename: pp_project_pkg-1.0.202306061654.data/scripts/get_tables.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306061546.data/scripts/pp_project_run.py
+Filename: pp_project_pkg-1.0.202306061654.data/scripts/pp_project_run.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306061546.dist-info/METADATA
+Filename: pp_project_pkg-1.0.202306061654.dist-info/METADATA
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306061546.dist-info/WHEEL
+Filename: pp_project_pkg-1.0.202306061654.dist-info/WHEEL
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306061546.dist-info/top_level.txt
+Filename: pp_project_pkg-1.0.202306061654.dist-info/top_level.txt
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306061546.dist-info/RECORD
+Filename: pp_project_pkg-1.0.202306061654.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pp_project_pkg/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('06')
 VERSION_DAY = int('06')
-VERSION_HOUR = int('15')
-VERSION_MINUTE = int('46')
+VERSION_HOUR = int('16')
+VERSION_MINUTE = int('54')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202306061546
-version_date = '2023/06/06 15:46'
+PATCH_VERSION = 202306061654
+version_date = '2023/06/06 16:54'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `pp_project_pkg-1.0.202306061546.data/scripts/pp_project_run.py` & `pp_project_pkg-1.0.202306061654.data/scripts/pp_project_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 ## Running the pp_project.py script
 
-import os
 import argparse
 from ..pp_project_pkg.utils import check_if_valid_date,site_date_res
 from ..pp_project_pkg.pp_tables import queries
 from ..pp_project_pkg.wrangling import wrangling_data
 
 def main(args,logger=None):
     if logger:
@@ -30,16 +29,14 @@
 
     wrangling_res = wrangling_data(queries_res=queries_res,site_data=site_data,logger=logger)
 
     return wrangling_res
 
 
 
-
-
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(
         description="Pp_project training Script")
     parser.add_argument("-d","--date", type=str, default='2023-06-06' , help="Date for getting the waste/production plan for. Default : 2023-06-06")
     parser.add_argument("-s","--site_id", type=int,default=30607, help="Site id. Default: 30607")
     args = parser.parse_args()
     main(args)
```

## Comparing `pp_project_pkg-1.0.202306061546.dist-info/RECORD` & `pp_project_pkg-1.0.202306061654.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 pp_project_pkg/__init__.py,sha256=9idX2X6SQKZg--ziGy6Ii9OB-kz9hOX1nEG9a0xEW9g,71
 pp_project_pkg/newsvendor.py,sha256=E6JHp0Vtmq63toKM6bO3xTAdCgwmAZzRua-w10wrc5Y,577
 pp_project_pkg/pp_tables.py,sha256=8rqVp4P9nF13UbBmN_R7vGK7MeY4BkeG2ibDa7jLRpg,7115
 pp_project_pkg/utils.py,sha256=nwTUL_AZDxjX12AjAQm5Fe1Wn5u7Gffn4QvmlwVfGXk,1203
-pp_project_pkg/version.py,sha256=UlLdQ0z64OquKBkNiFySw3h2i7KvZiVQ9OhiXrlUARA,396
+pp_project_pkg/version.py,sha256=BPlGImS9GxVl35jcgzvte57Y_Hzu01zBUdMt-G7Mllw,396
 pp_project_pkg/wrangling.py,sha256=rTDhW4hNytVSargqNoJlub_wyN37zPElVtKNc2TaRlw,4391
-pp_project_pkg-1.0.202306061546.data/scripts/get_tables.py,sha256=E5FmW2bHAU9NPORQMG85RzGtXOGjjzbATEa5lLGjyk4,65
-pp_project_pkg-1.0.202306061546.data/scripts/pp_project_run.py,sha256=F-kn5wEurC77sXw6WpdUADgPfLdpTlJc1q6XIGmcxxY,1328
-pp_project_pkg-1.0.202306061546.dist-info/METADATA,sha256=RwlIjN6Sjd7tlRwYMunIpsID6Hp1a-8YF1y2nDd5LXQ,191
-pp_project_pkg-1.0.202306061546.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pp_project_pkg-1.0.202306061546.dist-info/top_level.txt,sha256=2V1bEC5qsYRo1f2gAotX3L3S5xl1nIUxjITUTeRd8yQ,15
-pp_project_pkg-1.0.202306061546.dist-info/RECORD,,
+pp_project_pkg-1.0.202306061654.data/scripts/get_tables.py,sha256=E5FmW2bHAU9NPORQMG85RzGtXOGjjzbATEa5lLGjyk4,65
+pp_project_pkg-1.0.202306061654.data/scripts/pp_project_run.py,sha256=hNrYjtDlo7nX9pwMbM7un9R7ToKRdjVosBt3qErKtaA,1316
+pp_project_pkg-1.0.202306061654.dist-info/METADATA,sha256=v9oBfmXmB3Iu05TJahj5ibnl4jBk8nsa-Jr0SB28l4M,191
+pp_project_pkg-1.0.202306061654.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pp_project_pkg-1.0.202306061654.dist-info/top_level.txt,sha256=2V1bEC5qsYRo1f2gAotX3L3S5xl1nIUxjITUTeRd8yQ,15
+pp_project_pkg-1.0.202306061654.dist-info/RECORD,,
```

