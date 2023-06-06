# Comparing `tmp/pp_project_pkg-1.0.202306061423-py3-none-any.whl.zip` & `tmp/pp_project_pkg-1.0.202306061458-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,14 @@
-Zip file size: 6200 bytes, number of entries: 10
+Zip file size: 7287 bytes, number of entries: 12
 -rw-rw-r--  2.0 unx       71 b- defN 23-Jun-06 14:15 pp_project_pkg/__init__.py
 -rw-rw-r--  2.0 unx      577 b- defN 23-Jun-06 14:14 pp_project_pkg/newsvendor.py
 -rw-rw-r--  2.0 unx     7115 b- defN 23-Jun-06 12:02 pp_project_pkg/pp_tables.py
--rw-rw-r--  2.0 unx      593 b- defN 23-Jun-06 12:14 pp_project_pkg/utils.py
--rw-rw-r--  2.0 unx      396 b- defN 23-Jun-06 14:23 pp_project_pkg/version.py
+-rw-rw-r--  2.0 unx     1193 b- defN 23-Jun-06 14:58 pp_project_pkg/utils.py
+-rw-rw-r--  2.0 unx      396 b- defN 23-Jun-06 14:58 pp_project_pkg/version.py
 -rw-rw-r--  2.0 unx     4361 b- defN 23-Jun-06 12:06 pp_project_pkg/wrangling.py
--rw-rw-r--  2.0 unx      191 b- defN 23-Jun-06 14:23 pp_project_pkg-1.0.202306061423.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-06 14:23 pp_project_pkg-1.0.202306061423.dist-info/WHEEL
--rw-rw-r--  2.0 unx       15 b- defN 23-Jun-06 14:23 pp_project_pkg-1.0.202306061423.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      862 b- defN 23-Jun-06 14:23 pp_project_pkg-1.0.202306061423.dist-info/RECORD
-10 files, 14273 bytes uncompressed, 4706 bytes compressed:  67.0%
+-rwxrwxr-x  2.0 unx       65 b- defN 23-Jun-06 09:53 pp_project_pkg-1.0.202306061458.data/scripts/get_tables.py
+-rwxrwxr-x  2.0 unx      508 b- defN 23-Jun-06 12:59 pp_project_pkg-1.0.202306061458.data/scripts/pp_project_run.py
+-rw-rw-r--  2.0 unx      191 b- defN 23-Jun-06 14:58 pp_project_pkg-1.0.202306061458.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-06 14:58 pp_project_pkg-1.0.202306061458.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       15 b- defN 23-Jun-06 14:58 pp_project_pkg-1.0.202306061458.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1094 b- defN 23-Jun-06 14:58 pp_project_pkg-1.0.202306061458.dist-info/RECORD
+12 files, 15678 bytes uncompressed, 5401 bytes compressed:  65.6%
```

## zipnote {}

```diff
@@ -12,20 +12,26 @@
 
 Filename: pp_project_pkg/version.py
 Comment: 
 
 Filename: pp_project_pkg/wrangling.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306061423.dist-info/METADATA
+Filename: pp_project_pkg-1.0.202306061458.data/scripts/get_tables.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306061423.dist-info/WHEEL
+Filename: pp_project_pkg-1.0.202306061458.data/scripts/pp_project_run.py
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306061423.dist-info/top_level.txt
+Filename: pp_project_pkg-1.0.202306061458.dist-info/METADATA
 Comment: 
 
-Filename: pp_project_pkg-1.0.202306061423.dist-info/RECORD
+Filename: pp_project_pkg-1.0.202306061458.dist-info/WHEEL
+Comment: 
+
+Filename: pp_project_pkg-1.0.202306061458.dist-info/top_level.txt
+Comment: 
+
+Filename: pp_project_pkg-1.0.202306061458.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pp_project_pkg/utils.py

```diff
@@ -1,10 +1,12 @@
 import wml.visionml as wv
+import datetime
+import mb.pandas as pd
 
-__all__ = ['site_date_res']
+__all__ = ['site_date_res','check_if_valid_date']
 
 
 def site_date_res(site_id= 30607):
     """
     Get the site date report closure data
     Args:
         site_id : Site id for fetching the date wise result. Site_id : 30607 (Waldof)
@@ -13,8 +15,33 @@
         pd.DateFrame
     """
     q1 = """
     select s.start_date,s.id,s.meal_service_state, s.closed from pp_meal_service.view_current_state cs
                join pp_meal_service.view_service s on s.view_current_state_id = cs.id
 		       where cs.site_id = {} 
                """.format(site_id)
-    return wv.read_sql(q1,wv.ml_engine)
+    return wv.read_sql(q1,wv.ml_engine)
+
+def check_if_valid_date(site_res, date):
+    """
+    Check if the date (str) has closed the report.
+
+    Args:
+        site_res: complete report of the site_data_res
+        date: string value of date. format : '2023-06-06'
+    
+    Output:
+        Bool
+    """
+
+    k =datetime.datetime.strptime(date,'%Y-%m-%d').date()
+    l = site_res[site_res['start_date']==k]
+    
+    l_d = l['closed'].iloc[0]
+    
+    if pd.isnull(l_d):
+        return False
+    
+    if  (l_d).to_pydatetime().date() < l:
+        return False
+    
+    return True
```

## pp_project_pkg/version.py

```diff
@@ -1,11 +1,11 @@
 VERSION_YEAR = 2023
 VERSION_MONTH = int('06')
 VERSION_DAY = int('06')
 VERSION_HOUR = int('14')
-VERSION_MINUTE = int('23')
+VERSION_MINUTE = int('58')
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
-PATCH_VERSION = 202306061423
-version_date = '2023/06/06 14:23'
+PATCH_VERSION = 202306061458
+version_date = '2023/06/06 14:58'
 version = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 __all__  = ['MAJOR_VERSION', 'MINOR_VERSION', 'PATCH_VERSION', 'version_date', 'version']
```

