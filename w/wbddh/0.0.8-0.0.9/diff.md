# Comparing `tmp/wbddh-0.0.8-py3-none-any.whl.zip` & `tmp/wbddh-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 9141 bytes, number of entries: 11
+Zip file size: 9103 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat      396 b- defN 23-May-15 19:53 wbddh/__init__.py
 -rw-rw-rw-  2.0 fat      990 b- defN 23-May-15 19:53 wbddh/exceptions.py
--rw-rw-rw-  2.0 fat     4157 b- defN 23-Jun-04 19:12 wbddh/request_manager.py
+-rw-rw-rw-  2.0 fat     4085 b- defN 23-Jun-06 02:31 wbddh/request_manager.py
 -rw-rw-rw-  2.0 fat     8796 b- defN 23-May-11 22:36 wbddh/session.py
 -rw-rw-rw-  2.0 fat     6218 b- defN 23-May-21 04:48 wbddh/session_manager.py
 -rw-rw-rw-  2.0 fat       50 b- defN 23-May-13 18:53 wbddh/test.py
 -rw-rw-rw-  2.0 fat     1318 b- defN 23-May-11 22:36 wbddh/utils.py
--rw-rw-rw-  2.0 fat      543 b- defN 23-Jun-04 19:15 wbddh-0.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-04 19:15 wbddh-0.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-Jun-04 19:15 wbddh-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      810 b- defN 23-Jun-04 19:15 wbddh-0.0.8.dist-info/RECORD
-11 files, 23376 bytes uncompressed, 7789 bytes compressed:  66.7%
+-rw-rw-rw-  2.0 fat      543 b- defN 23-Jun-06 02:32 wbddh-0.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-06 02:32 wbddh-0.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Jun-06 02:32 wbddh-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      810 b- defN 23-Jun-06 02:32 wbddh-0.0.9.dist-info/RECORD
+11 files, 23304 bytes uncompressed, 7751 bytes compressed:  66.7%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: wbddh/test.py
 Comment: 
 
 Filename: wbddh/utils.py
 Comment: 
 
-Filename: wbddh-0.0.8.dist-info/METADATA
+Filename: wbddh-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: wbddh-0.0.8.dist-info/WHEEL
+Filename: wbddh-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: wbddh-0.0.8.dist-info/top_level.txt
+Filename: wbddh-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: wbddh-0.0.8.dist-info/RECORD
+Filename: wbddh-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## wbddh/request_manager.py

```diff
@@ -26,28 +26,27 @@
     Additional arguments:
         num_try:        number of tries
         interval:       interval between tries in seconds
     '''
     count = 0
     while True:
         try:
+            count = count + 1
             if session:
                 session.check_tokens()
-                response = requests.get(get_endpoint(endpoint, session), params=params, verify=session.verify, headers=session.get_headers(headers))
+                return requests.get(get_endpoint(endpoint, session), params=params, verify=session.verify, headers=session.get_headers(headers))
             else:
-                response = requests.get(get_endpoint(endpoint), params=params)
-            count = count + 1
+                return requests.get(get_endpoint(endpoint), params=params)
         except requests.exceptions.RequestException as e:
             print (f"[{count} try] Error: ", e)
+            if count > num_try:
+                raise Exception(f"Request failed after {count} tries.")
+            continue
 
-        if response.status_code == 200:
-            return response
-        elif count > num_try:
-            raise Exception(f"Request failed after {count} tries.")
-
+    
 def post(endpoint, params=None, json=None, headers=None, session=None):
     '''Send a POST request
 
     Arguments:
         endpoint:		the endpoint (e.g., "dataset/listpage")
         json:			data object
         params:			query parameters
@@ -69,24 +68,23 @@
         num_try:        number of tries
         interval:       interval between tries in seconds
     '''
     if session:
         count = 0
         while True:
             try:
-                session.check_tokens()
-                response = requests.post(get_endpoint(endpoint, session), params=params, json=json, verify=session.verify, headers=session.get_headers(headers))
                 count = count + 1
+                session.check_tokens()
+                return requests.post(get_endpoint(endpoint, session), params=params, json=json, verify=session.verify, headers=session.get_headers(headers))
             except requests.exceptions.RequestException as e:
                 print (f"[{count} try] Error: ", e)
-
-            if response.status_code == 200:
-                return response
-            elif count > num_try:
-                raise Exception(f"Request failed after {count} tries.")
+                if count > num_try:
+                    raise Exception(f"Request failed after {count} tries.")
+                continue
+                        
     else:
         raise DDHSessionException("DDH POST request requires a session")
 
 def post_file(endpoint, files=None, headers=None, session=None):
     '''Send a POST request with file
 
     Arguments:
```

## Comparing `wbddh-0.0.8.dist-info/METADATA` & `wbddh-0.0.9.dist-info/METADATA`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbddh
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python wrapper for DDH Open API
 Home-page: https://github.com/WB-DECIS/WBDDH
 Author: DECIS
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Provides-Extra: admin
 Requires-Dist: msal ; extra == 'admin'
```

## Comparing `wbddh-0.0.8.dist-info/RECORD` & `wbddh-0.0.9.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 wbddh/__init__.py,sha256=Mzr-CFhoE5tVUGnBK0ErZp429LATAf-G0hBHW0NP4vE,396
 wbddh/exceptions.py,sha256=prNSwu_9o5NnGfRtZBe4OxifAcLM2eSlrgpiJkOz8-8,990
-wbddh/request_manager.py,sha256=CUFOqZO9idkUTgAtVV4itH3ObV-hCKO5qG_I3iwUAiw,4157
+wbddh/request_manager.py,sha256=77vKER7ddqJq9Y-zesEcU-fqlDk1fp8iFvHXOIE5tGs,4085
 wbddh/session.py,sha256=pW5SqU2LaWcsFqRlzYMjSDM3Dlag_7HsRQHDOufTeC0,8796
 wbddh/session_manager.py,sha256=Gtax6G_E5pbcjZGIvkEPYmc_mx2fKhu26vvMBnmHKc4,6218
 wbddh/test.py,sha256=tuUyiKBC5AHoFjelqqMXWX_TrlE80HB37gJ7GidUp7U,50
 wbddh/utils.py,sha256=UhNse6FN2NzOtqL2v_js-l48MxGWLJLc-jusWSe1Zt0,1318
-wbddh-0.0.8.dist-info/METADATA,sha256=biyMerUB6lUeajR4i0QUMabrSu1zcQxqyGzgyG2lsIQ,543
-wbddh-0.0.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-wbddh-0.0.8.dist-info/top_level.txt,sha256=QpvOJxdfZd0MJiwJGdLPwRZ_l998Zyc_HIJ2JF_3iTI,6
-wbddh-0.0.8.dist-info/RECORD,,
+wbddh-0.0.9.dist-info/METADATA,sha256=d4bdk-EmVh32Hh4s9W8qChE-yq0qgnnGQ_tK1pvfjxM,543
+wbddh-0.0.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+wbddh-0.0.9.dist-info/top_level.txt,sha256=QpvOJxdfZd0MJiwJGdLPwRZ_l998Zyc_HIJ2JF_3iTI,6
+wbddh-0.0.9.dist-info/RECORD,,
```

