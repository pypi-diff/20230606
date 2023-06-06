# Comparing `tmp/pp_project_pkg-1.0.202306061458-py3-none-any.whl.zip` & `tmp/pp_project_pkg-1.0.202306061502-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 7287 bytes, number of entries: 12
+Zip file size: 7285 bytes, number of entries: 12
 -rw-rw-r--  2.0 unx       71 b- defN 23-Jun-06 14:15 pp_project_pkg/__init__.py
 -rw-rw-r--  2.0 unx      577 b- defN 23-Jun-06 14:14 pp_project_pkg/newsvendor.py
 -rw-rw-r--  2.0 unx     7115 b- defN 23-Jun-06 12:02 pp_project_pkg/pp_tables.py
--rw-rw-r--  2.0 unx     1193 b- defN 23-Jun-06 14:58 pp_project_pkg/utils.py
--rw-rw-r--  2.0 unx      396 b- defN 23-Jun-06 14:58 pp_project_pkg/version.py
+-rw-rw-r--  2.0 unx     1193 b- defN 23-Jun-06 15:01 pp_project_pkg/utils.py
+-rw-rw-r--  2.0 unx      396 b- defN 23-Jun-06 15:02 pp_project_pkg/version.py
 -rw-rw-r--  2.0 unx     4361 b- defN 23-Jun-06 12:06 pp_project_pkg/wrangling.py
--rwxrwxr-x  2.0 unx       65 b- defN 23-Jun-06 09:53 pp_project_pkg-1.0.202306061458.data/scripts/get_tables.py
--rwxrwxr-x  2.0 unx      508 b- defN 23-Jun-06 12:59 pp_project_pkg-1.0.202306061458.data/scripts/pp_project_run.py
--rw-rw-r--  2.0 unx      191 b- defN 23-Jun-06 14:58 pp_project_pkg-1.0.202306061458.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-06 14:58 pp_project_pkg-1.0.202306061458.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-06 14:58 pp_project_pkg-1.0.202306061458.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1094 b- defN 23-Jun-06 14:58 pp_project_pkg-1.0.202306061458.dist-info/RECORD
-12 files, 15678 bytes uncompressed, 5401 bytes compressed:  65.6%
+-rwxrwxr-x  2.0 unx       65 b- defN 23-Jun-06 09:53 pp_project_pkg-1.0.202306061502.data/scripts/get_tables.py
+-rwxrwxr-x  2.0 unx      508 b- defN 23-Jun-06 12:59 pp_project_pkg-1.0.202306061502.data/scripts/pp_project_run.py
+-rw-rw-r--  2.0 unx      191 b- defN 23-Jun-06 15:02 pp_project_pkg-1.0.202306061502.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-06 15:02 pp_project_pkg-1.0.202306061502.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-Jun-06 15:02 pp_project_pkg-1.0.202306061502.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1094 b- defN 23-Jun-06 15:02 pp_project_pkg-1.0.202306061502.dist-info/RECORD
+12 files, 15678 bytes uncompressed, 5399 bytes compressed:  65.6%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: pp_project_pkg/version.py
 Comment: 
 
 Filename: pp_project_pkg/wrangling.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306061458.data/scripts/get_tables.py
+Filename: pp_project_pkg-1.0.202306061502.data/scripts/get_tables.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306061458.data/scripts/pp_project_run.py
+Filename: pp_project_pkg-1.0.202306061502.data/scripts/pp_project_run.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306061458.dist-info/METADATA
+Filename: pp_project_pkg-1.0.202306061502.dist-info/METADATA
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306061458.dist-info/WHEEL
+Filename: pp_project_pkg-1.0.202306061502.dist-info/WHEEL
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306061458.dist-info/top_level.txt
+Filename: pp_project_pkg-1.0.202306061502.dist-info/top_level.txt
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306061458.dist-info/RECORD
+Filename: pp_project_pkg-1.0.202306061502.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pp_project_pkg/utils.py

```diff
@@ -37,11 +37,11 @@
     l = site_res[site_res['start_date']==k]
     
     l_d = l['closed'].iloc[0]
     
     if pd.isnull(l_d):
         return False
     
-    if  (l_d).to_pydatetime().date() < l:
+    if  (l_d).to_pydatetime().date() < k:
         return False
     
     return True
```

## pp_project_pkg/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('06')
 VERSION_DAY = int('06')
-VERSION_HOUR = int('14')
-VERSION_MINUTE = int('58')
+VERSION_HOUR = int('15')
+VERSION_MINUTE = int('02')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202306061458
-version_date = '2023/06/06 14:58'
+PATCH_VERSION = 202306061502
+version_date = '2023/06/06 15:02'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

## Comparing `pp_project_pkg-1.0.202306061458.dist-info/RECORD` & `pp_project_pkg-1.0.202306061502.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 pp_project_pkg/__init__.py,sha256=9idX2X6SQKZg--ziGy6Ii9OB-kz9hOX1nEG9a0xEW9g,71
 pp_project_pkg/newsvendor.py,sha256=E6JHp0Vtmq63toKM6bO3xTAdCgwmAZzRua-w10wrc5Y,577
 pp_project_pkg/pp_tables.py,sha256=8rqVp4P9nF13UbBmN_R7vGK7MeY4BkeG2ibDa7jLRpg,7115
-pp_project_pkg/utils.py,sha256=f_FS6Yg5c3jIQa3HYPxGwfNptoVZF6zc6AkPZb8IiYg,1193
-pp_project_pkg/version.py,sha256=OFFiZi_a9yF7g5UYw5e7JL3fAqWcT2cV1vcDv7evVk8,396
+pp_project_pkg/utils.py,sha256=7sn8HlaQmT0Jl8uX0YGTXkf47J3bOhMv-V5Gx29ieuU,1193
+pp_project_pkg/version.py,sha256=lRm6kRpu1k8ZNXqiuTqOY8vaXMpn7N1noS6UsIm6Vg0,396
 pp_project_pkg/wrangling.py,sha256=rw_wSGpePnxH0SOWySSe5NGLgV_l2x-OJakyMQp653s,4361
-pp_project_pkg-1.0.202306061458.data/scripts/get_tables.py,sha256=E5FmW2bHAU9NPORQMG85RzGtXOGjjzbATEa5lLGjyk4,65
-pp_project_pkg-1.0.202306061458.data/scripts/pp_project_run.py,sha256=Zkx_1kezh3VicdBtZrwlnqh9IyccvvgUxL97lK8kZ_4,508
-pp_project_pkg-1.0.202306061458.dist-info/METADATA,sha256=eXra9L7BgYtgbdQIXOMg9pKZ9SiAcDELdelz9Ch39Ks,191
-pp_project_pkg-1.0.202306061458.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pp_project_pkg-1.0.202306061458.dist-info/top_level.txt,sha256=2V1bEC5qsYRo1f2gAotX3L3S5xl1nIUxjITUTeRd8yQ,15
-pp_project_pkg-1.0.202306061458.dist-info/RECORD,,
+pp_project_pkg-1.0.202306061502.data/scripts/get_tables.py,sha256=E5FmW2bHAU9NPORQMG85RzGtXOGjjzbATEa5lLGjyk4,65
+pp_project_pkg-1.0.202306061502.data/scripts/pp_project_run.py,sha256=Zkx_1kezh3VicdBtZrwlnqh9IyccvvgUxL97lK8kZ_4,508
+pp_project_pkg-1.0.202306061502.dist-info/METADATA,sha256=MdbFODAddMsyxnvLj4sXRQWydquRy6smxh70QhSAWpw,191
+pp_project_pkg-1.0.202306061502.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pp_project_pkg-1.0.202306061502.dist-info/top_level.txt,sha256=2V1bEC5qsYRo1f2gAotX3L3S5xl1nIUxjITUTeRd8yQ,15
+pp_project_pkg-1.0.202306061502.dist-info/RECORD,,
```

