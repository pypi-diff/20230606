# Comparing `tmp/nashbanksync-0.1.80.tar.gz` & `tmp/nashbanksync-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nashbanksync-0.1.80.tar", last modified: Tue Jun  6 12:59:38 2023, max compression
+gzip compressed data, was "dist\nashbanksync-0.1.9.tar", last modified: Wed Jan 18 20:04:09 2023, max compression
```

## Comparing `nashbanksync-0.1.80.tar` & `nashbanksync-0.1.9.tar`

### file list

```diff
@@ -1,56 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 12:59:38.602010 nashbanksync-0.1.80/
--rw-rw-rw-   0        0        0    35821 2023-05-24 17:00:06.000000 nashbanksync-0.1.80/LICENSE
--rw-rw-rw-   0        0        0     1044 2023-06-06 12:59:38.601008 nashbanksync-0.1.80/PKG-INFO
--rw-rw-rw-   0        0        0      486 2023-05-24 17:00:06.000000 nashbanksync-0.1.80/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 12:59:38.530083 nashbanksync-0.1.80/bank_sync/
-drwxrwxrwx   0        0        0        0 2023-06-06 12:59:38.536081 nashbanksync-0.1.80/bank_sync/APIs/
--rw-rw-rw-   0        0        0       13 2023-05-24 18:13:46.000000 nashbanksync-0.1.80/bank_sync/APIs/__init__.py
--rw-rw-rw-   0        0        0     9775 2023-05-25 13:58:31.000000 nashbanksync-0.1.80/bank_sync/APIs/api_format.py
-drwxrwxrwx   0        0        0        0 2023-06-06 12:59:38.540085 nashbanksync-0.1.80/bank_sync/APIs/utils/
--rw-rw-rw-   0        0        0       14 2023-05-24 18:13:46.000000 nashbanksync-0.1.80/bank_sync/APIs/utils/__init__.py
--rw-rw-rw-   0        0        0     1023 2023-05-24 18:13:46.000000 nashbanksync-0.1.80/bank_sync/APIs/utils/generate_code.py
-drwxrwxrwx   0        0        0        0 2023-06-06 12:59:38.545234 nashbanksync-0.1.80/bank_sync/Nash/
--rw-rw-rw-   0        0        0       13 2023-05-24 18:13:46.000000 nashbanksync-0.1.80/bank_sync/Nash/__init__.py
--rw-rw-rw-   0        0        0     2635 2023-05-24 18:13:46.000000 nashbanksync-0.1.80/bank_sync/Nash/nash.py
-drwxrwxrwx   0        0        0        0 2023-06-06 12:59:38.557236 nashbanksync-0.1.80/bank_sync/Resources/
--rw-rw-rw-   0        0        0        0 2023-05-24 18:13:46.000000 nashbanksync-0.1.80/bank_sync/Resources/__init__.py
--rw-rw-rw-   0        0        0    37113 2023-06-06 12:57:56.000000 nashbanksync-0.1.80/bank_sync/Resources/accounts.py
--rw-rw-rw-   0        0        0    19878 2023-05-25 14:00:05.000000 nashbanksync-0.1.80/bank_sync/Resources/banks.py
--rw-rw-rw-   0        0        0      555 2023-05-24 18:13:46.000000 nashbanksync-0.1.80/bank_sync/Resources/helpers.py
--rw-rw-rw-   0        0        0    14484 2023-05-31 10:15:24.000000 nashbanksync-0.1.80/bank_sync/Resources/operations.py
--rw-rw-rw-   0        0        0    50744 2023-06-05 04:58:52.000000 nashbanksync-0.1.80/bank_sync/Resources/payments.py
--rw-rw-rw-   0        0        0    46648 2023-05-25 13:01:19.000000 nashbanksync-0.1.80/bank_sync/Resources/resource.py
--rw-rw-rw-   0        0        0        0 2023-05-24 18:13:46.000000 nashbanksync-0.1.80/bank_sync/__init__.py
--rw-rw-rw-   0        0        0      306 2023-05-24 18:13:46.000000 nashbanksync-0.1.80/bank_sync/admin.py
--rw-rw-rw-   0        0        0      155 2023-05-24 18:13:46.000000 nashbanksync-0.1.80/bank_sync/apps.py
-drwxrwxrwx   0        0        0        0 2023-06-06 12:59:38.560967 nashbanksync-0.1.80/bank_sync/middlewares/
--rw-rw-rw-   0        0        0        0 2023-05-24 18:13:46.000000 nashbanksync-0.1.80/bank_sync/middlewares/__init__.py
--rw-rw-rw-   0        0        0     2653 2023-05-25 14:00:32.000000 nashbanksync-0.1.80/bank_sync/middlewares/logs.py
-drwxrwxrwx   0        0        0        0 2023-06-06 12:59:38.595013 nashbanksync-0.1.80/bank_sync/migrations/
--rw-rw-rw-   0        0        0     1017 2023-05-24 18:13:46.000000 nashbanksync-0.1.80/bank_sync/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      415 2023-05-24 18:13:46.000000 nashbanksync-0.1.80/bank_sync/migrations/0002_alter_callbacks_reference.py
--rw-rw-rw-   0        0        0      990 2023-05-24 18:13:46.000000 nashbanksync-0.1.80/bank_sync/migrations/0003_requestlogs.py
--rw-rw-rw-   0        0        0      400 2023-05-24 18:13:46.000000 nashbanksync-0.1.80/bank_sync/migrations/0004_requestlogs_error.py
--rw-rw-rw-   0        0        0      419 2023-05-24 18:13:46.000000 nashbanksync-0.1.80/bank_sync/migrations/0005_alter_requestlogs_error.py
--rw-rw-rw-   0        0        0      470 2023-05-24 18:13:46.000000 nashbanksync-0.1.80/bank_sync/migrations/0006_requestlogs_log_time.py
--rw-rw-rw-   0        0        0      728 2023-05-24 18:13:46.000000 nashbanksync-0.1.80/bank_sync/migrations/0007_responselogs.py
--rw-rw-rw-   0        0        0      425 2023-05-24 18:13:46.000000 nashbanksync-0.1.80/bank_sync/migrations/0008_responselogs_ip.py
--rw-rw-rw-   0        0        0      416 2023-05-24 18:13:46.000000 nashbanksync-0.1.80/bank_sync/migrations/0009_responselogs_error.py
--rw-rw-rw-   0        0        0     1560 2023-05-24 18:13:46.000000 nashbanksync-0.1.80/bank_sync/migrations/0010_auto_20221117_1406.py
--rw-rw-rw-   0        0        0      943 2023-05-24 18:13:46.000000 nashbanksync-0.1.80/bank_sync/migrations/0011_ipndata.py
--rw-rw-rw-   0        0        0      414 2023-05-24 18:13:46.000000 nashbanksync-0.1.80/bank_sync/migrations/0012_alter_ipn_account_number.py
--rw-rw-rw-   0        0        0      495 2023-05-24 18:13:46.000000 nashbanksync-0.1.80/bank_sync/migrations/0013_alter_ipndata_ipn.py
--rw-rw-rw-   0        0        0      743 2023-05-24 18:13:46.000000 nashbanksync-0.1.80/bank_sync/migrations/0014_auto_20230125_1119.py
--rw-rw-rw-   0        0        0      992 2023-05-24 18:13:46.000000 nashbanksync-0.1.80/bank_sync/migrations/0015_auto_20230209_1410.py
--rw-rw-rw-   0        0        0      460 2023-05-24 18:13:46.000000 nashbanksync-0.1.80/bank_sync/migrations/0016_ipn_statement_url.py
--rw-rw-rw-   0        0        0      395 2023-05-24 18:13:46.000000 nashbanksync-0.1.80/bank_sync/migrations/0017_alter_ipn_statement_url.py
--rw-rw-rw-   0        0        0        0 2023-05-24 18:13:46.000000 nashbanksync-0.1.80/bank_sync/migrations/__init__.py
--rw-rw-rw-   0        0        0     5016 2023-05-24 18:13:46.000000 nashbanksync-0.1.80/bank_sync/models.py
--rw-rw-rw-   0        0        0     1010 2023-05-24 18:13:46.000000 nashbanksync-0.1.80/bank_sync/tests.py
-drwxrwxrwx   0        0        0        0 2023-06-06 12:59:38.599975 nashbanksync-0.1.80/nashbanksync.egg-info/
--rw-rw-rw-   0        0        0     1044 2023-06-06 12:59:38.000000 nashbanksync-0.1.80/nashbanksync.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1564 2023-06-06 12:59:38.000000 nashbanksync-0.1.80/nashbanksync.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 12:59:38.000000 nashbanksync-0.1.80/nashbanksync.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-06 12:59:38.000000 nashbanksync-0.1.80/nashbanksync.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 12:59:38.602010 nashbanksync-0.1.80/setup.cfg
--rw-rw-rw-   0        0        0      770 2023-06-06 12:58:57.000000 nashbanksync-0.1.80/setup.py
+drwxrwxrwx   0        0        0        0 2023-01-18 20:04:09.245108 nashbanksync-0.1.9/
+-rw-rw-rw-   0        0        0    35821 2022-08-31 12:58:39.000000 nashbanksync-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0      871 2023-01-18 20:04:09.244103 nashbanksync-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2022-08-31 12:58:39.000000 nashbanksync-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-01-18 20:04:09.191954 nashbanksync-0.1.9/bank_sync/
+drwxrwxrwx   0        0        0        0 2023-01-18 20:04:09.193954 nashbanksync-0.1.9/bank_sync/APIs/
+-rw-rw-rw-   0        0        0       13 2022-08-31 12:58:40.000000 nashbanksync-0.1.9/bank_sync/APIs/__init__.py
+-rw-rw-rw-   0        0        0     7516 2023-01-16 16:36:50.000000 nashbanksync-0.1.9/bank_sync/APIs/api_format.py
+drwxrwxrwx   0        0        0        0 2023-01-18 20:04:09.197059 nashbanksync-0.1.9/bank_sync/APIs/utils/
+-rw-rw-rw-   0        0        0       14 2022-08-31 12:58:40.000000 nashbanksync-0.1.9/bank_sync/APIs/utils/__init__.py
+-rw-rw-rw-   0        0        0     1023 2023-01-08 19:43:19.000000 nashbanksync-0.1.9/bank_sync/APIs/utils/generate_code.py
+drwxrwxrwx   0        0        0        0 2023-01-18 20:04:09.200058 nashbanksync-0.1.9/bank_sync/Nash/
+-rw-rw-rw-   0        0        0       13 2022-08-31 12:58:40.000000 nashbanksync-0.1.9/bank_sync/Nash/__init__.py
+-rw-rw-rw-   0        0        0     1456 2022-08-31 12:58:40.000000 nashbanksync-0.1.9/bank_sync/Nash/nash.py
+drwxrwxrwx   0        0        0        0 2023-01-18 20:04:09.208772 nashbanksync-0.1.9/bank_sync/Resources/
+-rw-rw-rw-   0        0        0        0 2022-08-31 12:58:40.000000 nashbanksync-0.1.9/bank_sync/Resources/__init__.py
+-rw-rw-rw-   0        0        0    28300 2023-01-18 19:57:42.000000 nashbanksync-0.1.9/bank_sync/Resources/accounts.py
+-rw-rw-rw-   0        0        0    13110 2023-01-16 16:36:50.000000 nashbanksync-0.1.9/bank_sync/Resources/banks.py
+-rw-rw-rw-   0        0        0    13483 2023-01-07 22:05:26.000000 nashbanksync-0.1.9/bank_sync/Resources/operations.py
+-rw-rw-rw-   0        0        0    45030 2023-01-12 18:34:03.000000 nashbanksync-0.1.9/bank_sync/Resources/payments.py
+-rw-rw-rw-   0        0        0    39264 2023-01-18 18:14:57.000000 nashbanksync-0.1.9/bank_sync/Resources/resource.py
+-rw-rw-rw-   0        0        0        0 2022-08-31 12:58:40.000000 nashbanksync-0.1.9/bank_sync/__init__.py
+-rw-rw-rw-   0        0        0      306 2022-11-24 16:31:07.000000 nashbanksync-0.1.9/bank_sync/admin.py
+-rw-rw-rw-   0        0        0      155 2022-08-31 12:58:40.000000 nashbanksync-0.1.9/bank_sync/apps.py
+drwxrwxrwx   0        0        0        0 2023-01-18 20:04:09.211771 nashbanksync-0.1.9/bank_sync/middlewares/
+-rw-rw-rw-   0        0        0        0 2022-11-24 16:31:07.000000 nashbanksync-0.1.9/bank_sync/middlewares/__init__.py
+-rw-rw-rw-   0        0        0     2643 2022-12-08 16:31:16.000000 nashbanksync-0.1.9/bank_sync/middlewares/logs.py
+drwxrwxrwx   0        0        0        0 2023-01-18 20:04:09.231770 nashbanksync-0.1.9/bank_sync/migrations/
+-rw-rw-rw-   0        0        0     1017 2022-08-31 12:58:40.000000 nashbanksync-0.1.9/bank_sync/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      415 2022-11-24 16:31:07.000000 nashbanksync-0.1.9/bank_sync/migrations/0002_alter_callbacks_reference.py
+-rw-rw-rw-   0        0        0      990 2022-11-24 16:31:07.000000 nashbanksync-0.1.9/bank_sync/migrations/0003_requestlogs.py
+-rw-rw-rw-   0        0        0      400 2022-11-24 16:31:07.000000 nashbanksync-0.1.9/bank_sync/migrations/0004_requestlogs_error.py
+-rw-rw-rw-   0        0        0      419 2022-11-24 16:31:07.000000 nashbanksync-0.1.9/bank_sync/migrations/0005_alter_requestlogs_error.py
+-rw-rw-rw-   0        0        0      470 2022-11-24 16:31:07.000000 nashbanksync-0.1.9/bank_sync/migrations/0006_requestlogs_log_time.py
+-rw-rw-rw-   0        0        0      728 2022-11-24 16:31:07.000000 nashbanksync-0.1.9/bank_sync/migrations/0007_responselogs.py
+-rw-rw-rw-   0        0        0      425 2022-11-24 16:31:07.000000 nashbanksync-0.1.9/bank_sync/migrations/0008_responselogs_ip.py
+-rw-rw-rw-   0        0        0      416 2022-11-24 16:31:07.000000 nashbanksync-0.1.9/bank_sync/migrations/0009_responselogs_error.py
+-rw-rw-rw-   0        0        0     1560 2022-11-24 16:31:07.000000 nashbanksync-0.1.9/bank_sync/migrations/0010_auto_20221117_1406.py
+-rw-rw-rw-   0        0        0      943 2022-11-24 16:31:07.000000 nashbanksync-0.1.9/bank_sync/migrations/0011_ipndata.py
+-rw-rw-rw-   0        0        0      414 2022-11-24 16:31:07.000000 nashbanksync-0.1.9/bank_sync/migrations/0012_alter_ipn_account_number.py
+-rw-rw-rw-   0        0        0      495 2022-11-24 16:31:07.000000 nashbanksync-0.1.9/bank_sync/migrations/0013_alter_ipndata_ipn.py
+-rw-rw-rw-   0        0        0        0 2022-08-31 12:58:40.000000 nashbanksync-0.1.9/bank_sync/migrations/__init__.py
+-rw-rw-rw-   0        0        0     4256 2023-01-08 19:40:25.000000 nashbanksync-0.1.9/bank_sync/models.py
+-rw-rw-rw-   0        0        0     1010 2023-01-12 18:34:03.000000 nashbanksync-0.1.9/bank_sync/tests.py
+drwxrwxrwx   0        0        0        0 2023-01-18 20:04:09.241770 nashbanksync-0.1.9/nashbanksync.egg-info/
+-rw-rw-rw-   0        0        0      871 2023-01-18 20:04:09.000000 nashbanksync-0.1.9/nashbanksync.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1337 2023-01-18 20:04:09.000000 nashbanksync-0.1.9/nashbanksync.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-01-18 20:04:09.000000 nashbanksync-0.1.9/nashbanksync.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-01-18 20:04:09.000000 nashbanksync-0.1.9/nashbanksync.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-01-18 20:04:09.245108 nashbanksync-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      769 2023-01-18 20:03:46.000000 nashbanksync-0.1.9/setup.py
```

### Comparing `nashbanksync-0.1.80/LICENSE` & `nashbanksync-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nashbanksync-0.1.80/PKG-INFO` & `nashbanksync-0.1.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,29 @@
 Metadata-Version: 2.1
 Name: nashbanksync
-Version: 0.1.80
+Version: 0.1.9
 Summary: Python library for connecting to the Nash Banks Framework
 Home-page: https://github.com/NashInc/NashSync.git
 Author: Dansol Obondo
 Author-email: dansol@nashafrica.co
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Nasheq Bank Sync Standardized A.P.I.s Python Integrations
+# Nasheq E.R.P. Standardized A.P.I.s python integrations
 
 ## Quick Guide
 Below are the steps on how to get the web app up and running
 
-1.	Install Dependencies:
-```bash
-    pip install requests
-    pip install django-compression-middleware
-    pip install djangorestframework
-```
-2.	Install Nash Sync ERP Library:
+1.	Install it:
 ```bash
     pip install nashbanksync
 ```
-3.	View get started documentation:
+2.	View get started documentation:
 ```bash
     https://nashbanksuite.readme.io/v1.2.0/docs
 ```
-4.	Start Coding
+3.	Start Coding
```

### Comparing `nashbanksync-0.1.80/bank_sync/APIs/api_format.py` & `nashbanksync-0.1.9/bank_sync/APIs/api_format.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import json
 import requests
-from datetime import datetime, timezone, timedelta
+from datetime import datetime,timezone,timedelta
 from rest_framework import status
 try:
     from django.conf import settings
 except Exception as e:
     pass
 # This is a class that is designed to include all methods and functions one needs to make an A.P.I. call
-
 class API(object):
 
+    _base_url = "https://dev.bankingservices.nashglobal.co/api/banks"
+    _base_url_third_party_banking = "https://dev.3p.bankingservices.nashglobal.co/api"
+
     _auth_token_url = None
-    _oauth2_client_id = None
+    _client_id = None
     _client_secret = None
     _identity_token = None
     _auth_scope = None
-    _is_identity_config_set = False
-    _error = False
 
     global_session = requests.Session()
 
     try:
-        _oauth2_client_id = getattr(
-            settings, 'OAUTH2_CLIENT_ID', _oauth2_client_id)
+        _client_id = getattr(
+            settings, 'OAUTH2_CLIENT_ID', _client_id)
         _client_secret = getattr(
             settings, 'CLIENT_SECRET', _client_secret)
         _auth_token_url = getattr(
             settings, 'OAUTH2_TOKEN_URL', _auth_token_url)
         _auth_scope = getattr(
             settings, 'OAUTH2_SCOPE', _auth_scope)
     except Exception as e:
@@ -38,130 +38,111 @@
     _headers = None
     _params = None
     _payload = None
 
     # You always expect a response from A.P.I. calls
     _response = {}
 
-    # You always expect a response code from A.P.I. calls
-    _response_code = -1
-
     # When using this class to create an A.P.I. class, each API should have an optional name and code
     # but must have headers and any required parameters
     def __init__(self, name=None, headers=None, params=None, code=None):
         self._name = name
         self._code = code
 
         self._headers = headers
         self._params = params
 
         requests.packages.urllib3.disable_warnings()
 
-    def execute_get_identity_token(self):
-        refresh_token = False
+    def set_identity_token(self,identity_token):
+        self._identity_token = identity_token
+        return self
+
+    def refresh_identity_token(self):
+        refresh_token=False
         # check if an Authorization header was set in the global token
         if self.global_session.headers.get('Authorization'):
-            # check when it was set to expire which is set in '%Y:%m:%d %H:%M:%S %z'
-            auth_expires_in = self.global_session.headers.get(
-                'auth_expires_in')
-            # convert the string '%Y:%m:%d %H:%M:%S %z' to time
-            auth_expires_in = datetime.strptime(
-                auth_expires_in, '%Y:%m:%d %H:%M:%S %z')
-            # get the current time and add ten minutes to it, so that we refresh the token 5 minutes before its expiry
-            current_time = datetime.now(timezone.utc) + timedelta(minutes=5)
-            # if current time plus 5 minutes is more than when the auth needs to expire
+            # check when it was set to expire which is set in '%H:%M:%S'
+            auth_expires_in=self.global_session.headers.get('auth_expires_in')
+            # convert the string '%H:%M:%S' to time
+            auth_expires_in=datetime.strptime(auth_expires_in, '%H:%M:%S').time()
+            # get the current time and add ten minutes to it, so that we refresh the token 10 minutes before its expiry
+            current_time=(datetime.now(timezone.utc) + timedelta(minutes=5)).time()
+            # if current time plus 10 minutes is more than when the auth needs to expire
             # refresh the token
             if current_time > auth_expires_in:
                 # first set the Authorization to an empty string
                 self.global_session.headers.update({'Authorization': ''})
-                refresh_token = True
+                refresh_token=True
         # If the Authorization header was not set in the global token
         else:
-            refresh_token = True
-
-        return refresh_token
-
-    def fetch_identity_token(self):
-        try:
-            if self.execute_get_identity_token():
-                _payload = {
-                    'grant_type': 'client_credentials',
-                    'scope': self._auth_scope,
-                    'client_id': self._oauth2_client_id,
-                    'client_secret': self._client_secret
-                }
-                self._identity_token = requests.request(
-                    "POST", self._auth_token_url, data=_payload)
-                if self._identity_token.status_code == 200:
-                    self.global_session.headers.update({
-                        'Authorization': f"{self._identity_token.json().get('access_token',None)}",
-                        'auth_expires_in': (datetime.now(timezone.utc) + timedelta(seconds=self._identity_token.json().get('expires_in', 0))).strftime("%Y:%m:%d %H:%M:%S %z")
-                    })
-                    print("Identity Log In Successful")
-                else:
-                    raise Exception(self._identity_token.text)
-        except Exception as e:
-            raise Exception(
-                f'Failed to Authenticate the User: {str(e)} self._identity_token" {self._identity_token} self._identity_token.content" {self._identity_token.content}')
+            refresh_token=True
+            
+        if refresh_token:
+            _payload = {
+                'grant_type': 'client_credentials',
+                'scope': self._auth_scope,
+                'client_id': self._client_id,
+                'client_secret': self._client_secret
+            }
+            self._identity_token = requests.request(
+                "POST", self._auth_token_url, data=_payload)                
+                
+            if self._identity_token.status_code == 200:                
+                self.global_session.headers.update({
+                    'Authorization':f"{self._identity_token.json().get('access_token',None)}",
+                    'auth_expires_in':(datetime.now(timezone.utc) + timedelta(seconds=self._identity_token.json().get('expires_in',0))).strftime("%H:%M:%S")
+                })  
 
-        return self
+                print(f'auth_expires_in: {self.global_session.headers["auth_expires_in"]}')
 
     # There are 3 types of API requests that most APIs use, POST, GET and PUT
     # This method will take the payload or data to be sent and send it to the required API url
     # using the desired method and returns the response
-    def api_request(self, payload, method, verify=False, files=None):
-
+    def api_request(self, payload, method, verify = False, files = None):
+        # Authenticate this service on the Nash Identity Server
+        self.refresh_identity_token()
+        
         if payload == "null":
-            self._payload = json.dumps({})
+            self._payload=json.dumps({})
         else:
             self._payload = payload
-
+        
+        if self._headers is not None and self.global_session.headers.get('Authorization'):
+            self._headers.update({
+                'Authorization':f"Bearer {self.global_session.headers.get('Authorization')}"
+            })
+        
         try:
-            # Authenticate this service on the Nash Identity Server
-            self.fetch_identity_token()
-
-            if self._headers is not None and self.global_session.headers.get('Authorization'):
-                self._headers.update({
-                    'Authorization': f"Bearer {self.global_session.headers.get('Authorization')}"
-                })
-            print(f'api_request self._headers: {self._headers}')
             if method == 'POST':
                 self._response = requests.post(self.get_full_url(), headers=self._headers, params=self._params,
-                                               data=self._payload, json=self._payload, verify=verify, files=files)
+                                           data=self._payload, json=self._payload, verify=verify,files=files)
             elif method == 'PUT':
                 self._response = requests.put(self.get_full_url(), headers=self._headers, params=self._params,
-                                              data=self._payload, json=self._payload, verify=verify)
+                                           data=self._payload, json=self._payload, verify=verify)
             elif method == 'GET':
                 self._response = requests.get(self.get_full_url(), headers=self._headers, params=self._params,
-                                              data=self._payload, json=self._payload, verify=verify)
+                                           data=self._payload, json=self._payload, verify=verify)
             elif method == 'DELETE':
                 self._response = requests.delete(self.get_full_url(), headers=self._headers, params=self._params,
-                                                 data=self._payload, json=self._payload, verify=verify)
+                                           data=self._payload, json=self._payload, verify=verify)
+
             try:
                 if self._response.status_code == status.HTTP_200_OK:
-                    # If the URL we called returns a response
-                    if len(self._response.text):
-                        self._response = json.loads(self._response.text)
-                    # If the url we called returned no response return the default response below which holds the status code
-                    else:
-                        self._response = {'code': self._response.status_code}
+                    self._response = json.loads(self._response.text)
                 else:
                     if status.is_server_error(self._response.status_code):
-                        self._response = {
-                            'error': f'Bank Core Server Error: HTTP Error Code {self._response.status_code}'}
+                        self._response['error'] = f'Internal Server Error: HTTP Error Code {self._response.status_code}'
                     elif status.is_client_error(self._response.status_code):
-                        self._response = {
-                            'error': f'Bank Sync Service Server Error: HTTP Error Code {self._response.status_code}: {self.get_full_url()}'}
+                        self._response['error'] = f'Client Server Error: HTTP Error Code {self._response.status_code}: {self.get_full_url()}'
             except ValueError as e:
-                print(f'Bank Sync Error: {str(e)}')
-                self._response = {'error': f'Bank Sync Error: {str(e)} : Response {self._response}'}
+                self._response['error'] = self._response.text
 
         except Exception as e:
-            print(f'Exception: {str(e)}')
-            self._response = {'error': f'Bank Sync Error: {str(e)}'}
+            self._response['error'] = f'Internal Server Error: {e}'
         finally:
             return self._response
 
     # Method used to get the repsonse returned by an API instead of calling the API again
     def get_response(self):
         return self._response
 
@@ -185,59 +166,16 @@
 
     def get_full_url(self):
         return self._full_url
 
     def get_payload(self):
         return self._payload
 
-    def get_response_code(self):
-        return self._response_code
-
-    def set_response_code(self, response_code):
-        self._response_code = response_code
-        return self
-
-    def set_identity_token(self, identity_token):
-        self._identity_token = identity_token
-        return self
-
-    def set_oauth2_client_id(self, oauth2_client_id):
-        self._oauth2_client_id = oauth2_client_id
-        return self
-
-    def get_oauth2_client_id(self):
-        return self._oauth2_client_id
-
-    def set_client_secret(self, client_secret):
-        self._client_secret = client_secret
-        return self
-
-    def get_client_secret(self):
-        return self._client_secret
+    def get_base_url(self):
+        return self._base_url
 
-    def set_auth_token_url(self, auth_token_url):
-        self._auth_token_url = auth_token_url
-        return self
-
-    def get_auth_token_url(self):
-        return self._auth_token_url
-
-    def set_auth_scope(self, auth_scope):
-        self._auth_scope = auth_scope
-        return self
-
-    def set_error(self, error):
-        self._response = {"error": error}
-        return self
-
-    def get_auth_scope(self):
-        return self._auth_scope
-
-    def is_identity_config_set(self):
-        if self.get_oauth2_client_id() and self.get_client_secret() and self.get_auth_token_url() and self.get_auth_scope():
-            return True
-        else:
-            return False
+    def get_base_url_third_party_banking(self):
+        return self._base_url_third_party_banking
 
     @property
     def get_identity_token(self):
-        return self._identity_token
+        return self._identity_token
```

### Comparing `nashbanksync-0.1.80/bank_sync/APIs/utils/generate_code.py` & `nashbanksync-0.1.9/bank_sync/APIs/utils/generate_code.py`

 * *Files identical despite different names*

### Comparing `nashbanksync-0.1.80/bank_sync/Resources/accounts.py` & `nashbanksync-0.1.9/bank_sync/Resources/accounts.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from bank_sync.Resources.resource import Resource
 from bank_sync.APIs.utils.generate_code import get_code
-from datetime import datetime, date
+from datetime import datetime
+from datetime import date
 import json
 try:
     from django.conf import settings
 except Exception as e:
     pass
 
 import logging
@@ -21,20 +22,20 @@
         "date": "",
         "description": "",
         "transaction_id": "",
         "reference": "",
         "value_date": "",
         "posted_date": "",
         "service_point": "",
-        "running_cleared_balance": "0",
-        "debit_limit": "0",
+        "running_cleared_balance": "",
+        "debit_limit": 0,
         "limit_expiry_date": "",
         "serial": "",
-        "amount": "0",
-        "type": ""
+        "amount": "",
+        "type": "",
     }
 
     try:
         bank_sync_call_back = getattr(
             settings, 'BANK_SYNC_CALL_BACK_URLS', bank_sync_call_back)
     except Exception as e:
         pass
@@ -129,51 +130,56 @@
                     "accountIds": [payload.get("account_number", "")]
                 })
 
         elif operation == super().FULL_STATEMENT:
             # If bank_id is COOP
             if super().get_bank_id() == super().COOP:
                 data.update({
-                    "MessageReference": payload.get("reference", get_code(length=14)),
-                    "AccountNumber": f'{payload.get("account_number", "")}',
-                    "StartDate": payload.get("start_date", ""),
-                    "EndDate": payload.get("end_date", ""),
-                    "page": int(payload.get("page", 1)),
+                    "MessageReference": f'{get_code(length=14)}'
+                })
+                data.update({
+                    "AccountNumber": f'{payload.get("account_number", "")}'
+                })
+                data.update({
+                    "StartDate": payload.get("start_date", "")
+                })
+                data.update({
+                    "EndDate": payload.get("end_date", "")
                 })
             # If bank_id is EQUITY
             elif super().get_bank_id() == super().EQUITY:
                 data.update({
-                    "country_code": payload.get("country_code", ""),
-                    "account_number": f'{payload.get("account_number", "")}',
-                    "start_date": payload.get("start_date", ""),
-                    "end_date": payload.get("end_date", ""),
-                    "page": int(payload.get("page", 1)),
-                    "reference": payload.get("reference", get_code(length=14))
+                    "country_code": payload.get("country_code", "")
                 })
-            # If bank_id is NCBA
-            elif super().get_bank_id() == super().NCBA:
                 data.update({
-                    "account_number": f'{payload.get("account_number", "")}',
-                    "start_date": payload.get("start_date", ""),
-                    "end_date": payload.get("end_date", ""),
-                    "page": int(payload.get("page", 1)),
-                    "reference": payload.get("reference", get_code(length=14))
+                    "account_number": f'{payload.get("account_number", "")}'
                 })
+                data.update({
+                    "start_date": payload.get("start_date", "")
+                })
+                data.update({
+                    "end_date": payload.get("end_date", "")
+                })
+                data.update({
+                    "limit": payload.get("limit", 3)
+                })
+            # If bank_id is NCBA
+            elif super().get_bank_id() == super().NCBA:
+                pass
             # If bank_id is UBA
             elif super().get_bank_id() == super().UBA:
                 data.update({
-                    "page": int(payload.get("page", 1)),
                     "PROCESSING_CODE": 93,
                     "COUNTRY_CODE": payload.get("country_code", ""),
                     "DR_ACCT_NUM": payload.get("account_number", ""),
                     "TRAN_CRNCY_CODE": payload.get("currency_code", ""),
                     "STMT_QUERY_PARAMS": {
                         "START_DATE": payload.get("start_date", date.today().strftime('%Y%m%d')).replace("-", ""),
                         "END_DATE": payload.get("end_date", date.today().strftime('%Y%m%d')).replace("-", ""),
-                        "NUM_TRANS": payload.get("limit", 200)
+                        "NUM_TRANS": payload.get("limit", 5)
                     }
                 })
 
         elif operation == super().ACCOUNT_TRANSACTIONS:
             # If bank_id is COOP
             if super().get_bank_id() == super().COOP:
                 data.update({
@@ -211,23 +217,17 @@
                 data['bank_sync_call_back'] = payload.get("callback_url", None)
 
         elif operation == super().FOREX_RATE:
             if super().get_bank_id() == super().EQUITY:
                 data.update({
                     "accountNumber": payload.get("account_number", ""),
                     "countryCode": payload.get("country_code", ""),
-                    "currencyCode": payload.get("from_currency", ""),
+                    "currencyCode": payload.get("currency_code", ""),
                     "toCurrency": payload.get("to_currency", ""),
-                    "amount": f'{round(float(payload.get("amount", 1)), 2)}',
-                })
-            elif super().get_bank_id() == super().COOP:
-                data.update({
-                    "MessageReference": payload.get("reference", get_code(length=20)),
-                    "FromCurrencyCode": payload.get("from_currency", ""),
-                    "ToCurrencyCode": payload.get("to_currency", "")
+                    "amount": round(float(payload.get("amount", 0)), 2),
                 })
 
         data.update(payload.get("additional_properties", {}))
 
         return data
 
     def get_full_statement_transaction_dict(self):
@@ -235,465 +235,380 @@
 
     def response(self):
 
         data = {}
 
         response_data = super().response()
 
-        try:
+        if super().get_operation() == super().BALANCE:
+
+            data.update({
+                "message": "",
+                "code": -111111,
+                "balance": 0,
+                "balance_time": "",
+                "account_type": "",
+                "cleared_balance": "",
+                "booked_balance": "",
+                "blocked_balance": "",
+                "arrears_amount": "",
+                "branch_name": "",
+                "branch_code": "",
+                "average_balance": "",
+                "uncleared_balance": "",
+                "over_draft_limit": "",
+                "credit_limit": "",
+            })
 
-            if super().get_operation() == super().BALANCE:
+            if super().get_bank_id() == super().COOP:
 
-                data.update({
-                    "message": "",
-                    "code": "-111111",
-                    "balance": "0",
-                    "balance_time": "",
-                    "account_type": "",
-                    "cleared_balance": "0",
-                    "booked_balance": "0",
-                    "blocked_balance": "0",
-                    "arrears_amount": "0",
-                    "branch_name": "",
-                    "branch_code": "",
-                    "average_balance": "0",
-                    "uncleared_balance": "0",
-                    "over_draft_limit": "0",
-                    "credit_limit": "0",
-                })
-
-                if super().get_bank_id() == super().COOP:
-
-                    data["message"] = response_data.get("MessageDescription", "")
-                    data["code"] = f'{response_data.get("MessageCode", "-111111")}'
-                    data["balance"] = f'{response_data.get("AvailableBalance", "0")}'
-                    data["balance_time"] = response_data.get("MessageDateTime", "")
-
-                    data["account_type"] = response_data.get("ProductName", "")
-                    data["cleared_balance"] = f'{response_data.get("ClearedBalance", "0")}'
-                    data["booked_balance"] = f'{response_data.get("BookedBalance", "0")}'
-                    data["blocked_balance"] = f'{response_data.get("BlockedBalance", "0")}'
-                    data["arrears_amount"] = f'{response_data.get("ArrearsAmount", "0")}'
-                    data["branch_name"] = response_data.get("BranchName", "")
-                    data["branch_code"] = response_data.get("BranchSortCode", "")
-                    data["average_balance"] = f'{response_data.get("AverageBalance", "0")}'
-                    data["uncleared_balance"] = f'{response_data.get("UnclearedBalance", "0")}'
-                    data["over_draft_limit"] = f'{response_data.get("ODLimit", "0")}'
-                    data["credit_limit"] = f'{response_data.get("CreditLimit", "0")}'
+                data["message"] = response_data.get("MessageDescription", "")
+                data["code"] = int(response_data.get("MessageCode", -111111))
+                data["balance"] = response_data.get("AvailableBalance", "")
+                data["balance_time"] = response_data.get("MessageDateTime", "")
+
+                data["account_type"] = response_data.get("ProductName", "")
+                data["cleared_balance"] = response_data.get(
+                    "ClearedBalance", "")
+                data["booked_balance"] = response_data.get("BookedBalance", "")
+                data["blocked_balance"] = response_data.get(
+                    "BlockedBalance", "")
+                data["arrears_amount"] = response_data.get("ArrearsAmount", "")
+                data["branch_name"] = response_data.get("BranchName", "")
+                data["branch_code"] = response_data.get("BranchSortCode", "")
+                data["average_balance"] = response_data.get(
+                    "AverageBalance", "")
+                data["uncleared_balance"] = response_data.get(
+                    "UnclearedBalance", "")
+                data["over_draft_limit"] = response_data.get("ODLimit", "")
+                data["credit_limit"] = response_data.get("CreditLimit", "")
 
-                elif super().get_bank_id() == super().EQUITY:
+            elif super().get_bank_id() == super().EQUITY:
 
-                    data["message"] = response_data.get("message", "")
-                    data["code"] = f'{response_data.get("code", "-111111")}'
-                    data["balance_time"] = response_data.get("statement_time", "")
+                data["message"] = response_data.get("message", "")
+                data["code"] = response_data.get("code", -111111)
+                data["balance_time"] = response_data.get("response_time", "")
+
+                data["balance"] = 0
+
+                balances = response_data.get("data", {}).get("balances", [])
+                if bool(balances):
+                    if balances[0].get('type', '') == 'Available':
+                        data["balance"] = balances[0].get("amount", -1)
+                    if balances[1].get('type', '') == 'Current':
+                        data["cleared_balance"] = balances[1].get("amount", -1)
+            # If bank_id is UBA
+            elif super().get_bank_id() == super().UBA:
 
-                    data["balance"] = "0"
+                data["message"] = ''
+                data["code"] = int(float(response_data.get("sendTransactionResponse", {}).get(
+                    "return", {}).get("C24TRANRES", {}).get("ACTION_CODE", "-111111")))
+                data["balance"] = float(response_data.get("sendTransactionResponse", {}).get(
+                    "return", {}).get("C24TRANRES", {}).get("AVAILABLE_BALANCE", -1))
+                data["balance_time"] = datetime.strptime(f'{response_data.get("sendTransactionResponse", {}).get("return", {}).get("C24TRANRES", {}).get("TRAN_DATE_TIME",)}', '%Y%d%m%H%M%S').strftime('%Y-%m-%d %H:%M:%S')
+                if data["code"]:
+                    data["message"] = "Transaction Failed"
+                else:
+                    data["message"] = "Success"
 
-                    balances = response_data.get("data", {}).get("balances", [])
-                    if bool(balances):
-                        if balances[0].get('type', '') == 'Available':
-                            data["balance"] = f'{balances[0].get("amount", "0")}'
-                        if balances[1].get('type', '') == 'Current':
-                            data["cleared_balance"] = f'{balances[1].get("amount", "0")}'
-                # If bank_id is UBA
-                elif super().get_bank_id() == super().UBA:
-
-                    data["message"] = ''
-                    data["code"] = f'{int(float(response_data.get("sendTransactionResponse", {}).get("return", {}).get("C24TRANRES", {}).get("ACTION_CODE", "-111111")))}'
-                    data["balance"] = f'{float(response_data.get("sendTransactionResponse", {}).get("return", {}).get("C24TRANRES", {}).get("AVAILABLE_BALANCE", "0"))}'
-                    data["balance_time"] = datetime.strptime(f'{response_data.get("sendTransactionResponse", {}).get("return", {}).get("C24TRANRES", {}).get("TRAN_DATE_TIME",)}', '%Y%d%m%H%M%S').strftime('%Y-%m-%d %H:%M:%S')
-                    if int(data["code"]):
-                        data["message"] = "Transaction Failed"
-                    else:
-                        data["message"] = "Success"
+        elif super().get_operation() == super().MINI_STATEMENT or super().get_operation() == super().ACCOUNT_TRANSACTIONS:
 
-            elif super().get_operation() == super().MINI_STATEMENT or super().get_operation() == super().ACCOUNT_TRANSACTIONS:
+            if super().get_bank_id() == super().COOP:
+
+                data["message"] = response_data.get("MessageDescription", "")
+                data["code"] = response_data.get("MessageCode", "-111111")
+                data["transactions"] = []
+
+                transactions = response_data.get("Transactions", [])
+
+                for i in range(len(transactions)):
+                    transaction = {
+                        "currency_code": "KES",
+                        "date": transactions[i].get("TransactionDate", ""),
+                        "description": transactions[i].get("Narration", ""),
+                        "reference": transactions[i].get("TransactionReference", "")
+                    }
 
-                if super().get_bank_id() == super().COOP:
+                    if transactions[i].get("TransactionType", "") == "D":
+                        transaction["amount"] = transactions[i].get(
+                            "DebitAmount", "")
+                        transaction["type"] = "Debit"
 
-                    data["message"] = response_data.get("MessageDescription", "")
-                    data["code"] = f'{response_data.get("MessageCode", "-111111")}'
+                    elif transactions[i].get("TransactionType", "") == "C":
+                        transaction["amount"] = transactions[i].get(
+                            "CreditAmount", "")
+                        transaction["type"] = "Credit"
+
+                    data["transactions"].append(transaction)
+
+            if super().get_operation() == super().MINI_STATEMENT:
+
+                if super().get_bank_id() == super().EQUITY:
+
+                    data["message"] = response_data.get("message", "")
+                    data["code"] = f'{response_data.get("code", -111111)}'
                     data["transactions"] = []
-                    data["transactions_count"] = f'{len(response_data.get("Transactions", []))}'
 
-                    transactions = response_data.get("Transactions", [])
+                    transactions = response_data.get(
+                        "data", {}).get("transactions", [])
 
                     for i in range(len(transactions)):
+
                         transaction = {
-                            "currency_code": "KES",
-                            "date": transactions[i].get("TransactionDate", ""),
-                            "description": transactions[i].get("Narration", ""),
-                            "reference": transactions[i].get("TransactionReference", "")
+                            "currency_code": response_data.get("data", {}).get("currency", "KES"),
+                            "date": datetime.fromisoformat(
+                                transactions[i].get(
+                                    "postedDateTime", "") + '+00:00'
+                            ).strftime('%Y-%m-%d %H:%M:%S'),
+                            "description": transactions[i].get("description", ""),
+                            "amount":  transactions[i].get("amount", ""),
+                            "type":  transactions[i].get("type", "")
                         }
 
-                        if transactions[i].get("TransactionType", "") == "D":
-                            transaction["amount"] = f'{transactions[i].get("DebitAmount", "0")}'
-                            transaction["type"] = "Debit"
-
-                        elif transactions[i].get("TransactionType", "") == "C":
-                            transaction["amount"] = f'{transactions[i].get("CreditAmount", "0")}'
-                            transaction["type"] = "Credit"
-
                         data["transactions"].append(transaction)
 
-                if super().get_operation() == super().MINI_STATEMENT:
-
-                    if super().get_bank_id() == super().EQUITY:
+        elif super().get_operation() == super().ACCOUNT_VALIDATION:
 
-                        data["message"] = response_data.get("message", "")
-                        data["code"] = f'{response_data.get("code", "-111111")}'
-                        data["transactions"] = []
-                        data["transactions_count"] = f'{len(response_data.get("data", {}).get("transactions", []))}'
-
-                        transactions = response_data.get(
-                            "data", {}).get("transactions", [])
-
-                        for i in range(len(transactions)):
-
-                            transaction = {
-                                "currency_code": response_data.get("data", {}).get("currency", "KES"),
-                                "date": datetime.fromisoformat(
-                                    transactions[i].get(
-                                        "date", "").replace(" ","") + '+00:00'
-                                ).strftime('%Y-%m-%d %H:%M:%S'),
-                                "description": transactions[i].get("description", ""),
-                                "amount":  f'{transactions[i].get("amount", "0")}',
-                                "type":  transactions[i].get("type", "")
-                            }
-
-                            data["transactions"].append(transaction)
-
-            elif super().get_operation() == super().ACCOUNT_VALIDATION:
+            if super().get_bank_id() == super().COOP:
 
-                if super().get_bank_id() == super().COOP:
+                data["message"] = response_data.get("MessageDescription", "")
+                data["code"] = response_data.get("MessageCode", "-111111")
+                data["account_name"] = ""
 
-                    data["message"] = response_data.get("MessageDescription", "")
-                    data["code"] = f'{response_data.get("MessageCode", "-111111")}'
-                    data["account_name"] = ""
+            elif super().get_bank_id() == super().EQUITY:
 
-                elif super().get_bank_id() == super().EQUITY:
+                data["message"] = response_data.get("message", "")
+                data["code"] = f'{response_data.get("code", -111111)}'
+                data["account_name"] = ""
+                customer = response_data.get("data", {}).get("customer", [])
+                if len(customer) > 0:
+                    data["account_name"] = customer[0].get("name", "")
 
-                    data["message"] = response_data.get("message", "")
-                    data["code"] = f'{response_data.get("code", "-111111")}'
+            # If bank_id is DTB
+            elif super().get_bank_id() == super().DTB:
+                if isinstance(response_data, list):
+                    data["message"] = response_data[0]
+                    data["code"] = -111111
                     data["account_name"] = ""
-                    customer = response_data.get("data", {}).get("customer", [])
-                    if len(customer) > 0:
-                        data["account_name"] = customer[0].get("name", "")
-
-                # If bank_id is DTB
-                elif super().get_bank_id() == super().DTB:
-                    if isinstance(response_data, list):
-                        data["message"] = response_data[0]
-                        data["code"] = '-111111'
-                        data["account_name"] = ""
-                    else:
-                        data["message"] = response_data.get(
-                            "content", {}).get("account_description", "")
-                        data["code"] = '0'
-                        data["account_name"] = response_data.get(
-                            "content", {}).get("customer_name", "")
-
-            elif super().get_operation() == super().FULL_STATEMENT:
-
-                if super().get_bank_id() == super().COOP:
-
-                    data["message"] = response_data.get("MessageDescription", "")
-                    data["code"] = f'{response_data.get("MessageCode", "-111111")}'
-                    data["statement_time"] = datetime.fromisoformat(response_data.get("MessageDateTime", "") + '+00:00').strftime('%Y-%m-%d %H:%M:%S')
-                    data["statement_reference"] = response_data.get("MessageReference", "")
-
-                    data["total_transactions"] = f'{response_data.get("total_transactions", "0")}'
-                    data["num_pages"] = f'{response_data.get("num_pages", "0")}'
-                    data["page_has_next"] = response_data.get("page_has_next", False)
-                    data["transactions_count"] = f'{len(response_data.get("data", {}).get("transactions", []))}'
-                    data["transactions"] = []
+                else:
+                    data["message"] = response_data.get(
+                        "content", {}).get("account_description", "")
+                    data["code"] = 0
+                    data["account_name"] = response_data.get(
+                        "content", {}).get("customer_name", "")
 
-                    transactions = response_data.get("data", {}).get("transactions", [])
+        elif super().get_operation() == super().FULL_STATEMENT:
+            transaction = self.get_full_statement_transaction_dict()
 
-                    for i in range(len(transactions)):
-                        transaction={}
-                        transaction.update(self.get_full_statement_transaction_dict())
-                        
-                        # the reference below is a callback reference sent with the fullstatememt
-                        # if the fullstatement sent is one that relates to a callback reference 
-                        # linked to a payment request made earlier
-
-                        # Basically it is used to identify payment transactions that were made with a reference
-                        # that show up on the full statement 
-                        if 'nash_reference' in transactions[i].keys():
-                            transaction['nash_reference']=transactions[i].get("nash_reference")
-
-                        transaction.update(
-                            {
-                                "currency_code": response_data.get("currency_code", ""),
-                                "date": datetime.fromisoformat(transactions[i].get("TransactionDate", "")).strftime('%Y-%m-%d %H:%M:%S'),
-                                "description": transactions[i].get("Narration", ""),
-                                "transaction_id": transactions[i].get("TransactionID", transactions[i].get("TransactionId", "")),
-                                "value_date": datetime.fromisoformat(transactions[i].get("ValueDate", "")).strftime('%Y-%m-%d %H:%M:%S'),
-                                "service_point": transactions[i].get("ServicePoint", ""),
-                                "running_cleared_balance": f'{transactions[i].get("RunningClearedBalance", "0")}',
-                                "debit_limit": f'{float(transactions[i].get("DebitLimit", "0"))}',
-                                "limit_expiry_date": datetime.fromisoformat(transactions[i].get("LimitExpiry", transactions[i].get("LimitExpiryDate", ""))).strftime('%Y-%m-%d %H:%M:%S'),
-                            }
-                        )
+            if super().get_bank_id() == super().COOP:
 
-                        if transactions[i].get("TransactionType", "") == "D":
-                            transaction["amount"] = f'{transactions[i].get("DebitAmount", "0")}'
-                            transaction["type"] = "Debit"
-
-                        elif transactions[i].get("TransactionType", "") == "C":
-                            transaction["amount"] = f'{transactions[i].get("CreditAmount", "0")}'
-                            transaction["type"] = "Credit"
+                data["message"] = response_data.get("MessageDescription", "")
+                data["code"] = response_data.get("MessageCode", "-111111")
+                data["statement_time"] = response_data.get(
+                    "MessageDateTime", "")
+                data["statement_reference"] = response_data.get(
+                    "MessageReference", "")
+                data["transactions"] = []
 
-                        transaction["reference"] = transactions[i].get("TransactionReference", "")
-                        transaction["running_balance"] = f'{transactions[i].get("RunningBookBalance", "0")}'
+                transactions = response_data.get("Transactions", [])
 
-                        data["transactions"].append(transaction)
+                for i in range(len(transactions)):
 
-                # If bank_id is EQUITY
-                elif super().get_bank_id() == super().EQUITY:
+                    transaction.update(
+                        {
+                            "currency_code": "KES",
+                            "date": transactions[i].get("TransactionDate", ""),
+                            "description": transactions[i].get("Narration", ""),
+                            "transaction_id": transactions[i].get("TransactionID", ""),
+                            "value_date": transactions[i].get("ValueDate", ""),
+                            "service_point": transactions[i].get("ServicePoint", ""),
+                            "running_cleared_balance": transactions[i].get("RunningClearedBalance", ""),
+                            "debit_limit": float(transactions[i].get("DebitLimit", -1)),
+                            "limit_expiry_date": transactions[i].get("LimitExpiryDate", ""),
+                        }
+                    )
 
-                    # This is implemented since equity sometimes sends data as a truncated JSON String 
-                    try:
-                        if isinstance(response_data, str):
-                            # get the JOSN response and complete the JSON String by appending the missing closing brackets
-                            response_data = '{}{}'.format(response_data, '"}]}}')
-                            # convert the completed JSON String to JSON
-                            response_data = json.loads(response_data)
-                    except Exception as e:
-                        data['error'] = str(e)
-
-                    if isinstance(response_data, dict):
-                        data["message"] = response_data.get("message", "")
-                        data["code"] = f'{response_data.get("code", "-111111")}'
-                        data["statement_time"] = response_data.get("statement_time", "")
-
-                        data["total_transactions"] = f'{response_data.get("total_transactions", "0")}'
-                        data["num_pages"] = f'{response_data.get("num_pages", "0")}'
-                        data["page_has_next"] = response_data.get("page_has_next", False)
-
-                        data["statement_reference"] = response_data.get("statement_reference", "")
-                        data["transactions_count"] = f'{len(response_data.get("data", {}).get("transactions", []))}'
-                        data["transactions"] = []
-
-                        transactions = response_data.get("data", {}).get("transactions", [])
-
-                        for i in range(len(transactions)):
-                            transaction={}
-                            transaction.update(self.get_full_statement_transaction_dict())
-                        
-                        # the reference below is a callback reference sent with the fullstatememt
-                        # if the fullstatement sent is one that relates to a callback reference 
-                        # linked to a payment request made earlier
-
-                        # Basically it is used to identify payment transactions that were made with a reference
-                        # that show up on the full statement 
-                            if 'nash_reference' in transactions[i].keys():
-                                transaction['nash_reference']=transactions[i].get("nash_reference")
-
-                            transaction.update({
-                                "currency_code": transactions[i].get("runningBalance", {}).get("currency", "KES"),
-                                "date": datetime.fromisoformat(transactions[i].get("date", "") + '+00:00').strftime('%Y-%m-%d %H:%M:%S'),
-                                "description": transactions[i].get("description", ""),
-                                "amount":  f'{transactions[i].get("amount", "0")}',
-                                "type":  transactions[i].get("type", ""),
-                                "serial":  transactions[i].get("serial", ""),
-                                "reference":  transactions[i].get("reference", ""),
-                                "running_balance":  f'{transactions[i].get("runningBalance", {}).get("amount", "0")}',
-                                "posted_date": datetime.fromisoformat(
-                                    transactions[i].get(
-                                        "postedDateTime", "") + '+00:00'
-                                ).strftime('%Y-%m-%d %H:%M:%S'),
-                            })
+                    if transactions[i].get("TransactionType", "") == "D":
+                        transaction["amount"] = transactions[i].get(
+                            "DebitAmount", "")
+                        transaction["type"] = "Debit"
+
+                    elif transactions[i].get("TransactionType", "") == "C":
+                        transaction["amount"] = transactions[i].get(
+                            "CreditAmount", "")
+                        transaction["type"] = "Credit"
+
+                    transaction["reference"] = transactions[i].get(
+                        "TransactionReference", "")
+                    transaction["running_balance"] = transactions[i].get(
+                        "RunningBookBalance", "")
 
-                            data["transactions"].append(transaction)
-                    else:
-                        data['response'] = response_data
+                    data["transactions"].append(transaction)
 
-                # If bank_id is UBA
-                elif super().get_bank_id() == super().UBA:
+            elif super().get_bank_id() == super().EQUITY:
 
-                    data["message"] = response_data.get("message", '' )
-                    data["code"] = response_data.get("code", '-111111' )
-                    data["statement_reference"] = response_data.get("statement_reference", '' )
-                    data["statement_time"] = response_data.get("statement_time", "")
-
-                    data["total_transactions"] = f'{response_data.get("total_transactions", "0")}'
-                    data["num_pages"] = f'{response_data.get("num_pages", "0")}'
-                    data["page_has_next"] = response_data.get("page_has_next", False)
-                    data["transactions_count"] = f'{len(response_data.get("data", {}).get("transactions", []))}'
+                try:
+                    if isinstance(response_data, str):
+                        response_data = '{}{}'.format(response_data, '"}]}}')
+                        response_data = json.loads(response_data)
+                except Exception as e:
+                    data['error'] = e
 
-                    if int(data["code"]):
-                        data["message"] = "Transaction Failed"
-                    else:
-                        data["message"] = "Success"
+                if isinstance(response_data, dict):
+                    data["message"] = response_data.get("message", "")
+                    data["code"] = f'{response_data.get("code", -111111)}'
+                    data["statement_time"] = response_data.get(
+                        "response_time", "")
+                    data["statement_reference"] = ""
+                    data["transactions"] = []
 
-                    transactions = response_data.get("data", {}).get("transactions", [])
+                    transactions = response_data.get(
+                        "data", {}).get("transactions", [])
 
-                    data["transactions"] = []
                     for i in range(len(transactions)):
-                        transaction={}
-                        transaction.update(self.get_full_statement_transaction_dict())
 
                         transaction.update({
-                            "currency_code": response_data.get("currency_code", ""),
-                            "date": datetime.strptime(f'{transactions[i].get("TRAN_DATE", None)}', '%Y%d%m').strftime('%Y-%m-%d %H:%M:%S'),
-
-                            "description": transactions[i].get("NARRATION", ""),
-                            "amount": f'{transactions[i].get("TRAN_AMT", "0")}',
-                            "running_balance": f'{transactions[i].get("BALANCE", "0")}',
-
-                            "transaction_id": transactions[i].get("TRAN_ID", ""),
-                            "serial": f'{transactions[i].get("TRAN_SNUM", "")}',
-                            "value_date": datetime.strptime(f'{transactions[i].get("VALUE_DATE", None)}', '%Y%d%m').strftime('%Y-%m-%d %H:%M:%S'),
-                            "posted_date": datetime.strptime(f'{transactions[i].get("DATE_POSTED", None)}', '%Y%d%m%H%M%S').strftime('%Y-%m-%d %H:%M:%S'),
+                            "currency_code": response_data.get("data", {}).get("currency", "KES"),
+                            "date": datetime.fromisoformat(
+                                transactions[i].get(
+                                    "date", "") + '+00:00'
+                            ).strftime('%Y-%m-%d %H:%M:%S'),
+                            "description": transactions[i].get("description", ""),
+                            "amount":  f'{transactions[i].get("amount", "")}',
+                            "type":  transactions[i].get("type", ""),
+                            "serial":  transactions[i].get("serial", ""),
+                            "reference":  transactions[i].get("reference", ""),
+                            "running_balance":  f'{transactions[i].get("runningBalance", {}).get("amount", "")}',
+                            "posted_date": datetime.fromisoformat(
+                                transactions[i].get(
+                                    "postedDateTime", "") + '+00:00'
+                            ).strftime('%Y-%m-%d %H:%M:%S'),
                         })
 
-                        if transactions[i].get("PART_TRAN_TYPE", "") == "D":
-                            transaction["type"] = "Debit"
-                        elif transactions[i].get("PART_TRAN_TYPE", "") == "C":
-                            transaction["type"] = "Credit"
+                        data["transactions"].append(transaction)
+                else:
+                    data['response'] = response_data
 
-                        if transactions[i].get("REF_NUM", {}).get("@null", "true") == "true":
-                            transaction["reference"] = ""
+            # If bank_id is UBA
+            elif super().get_bank_id() == super().UBA:
 
-                        data["transactions"].append(transaction)
-                                # If bank_id is UBA
-                
-                elif super().get_bank_id() == super().NCBA:
+                data["message"] = ''
+                data["code"] = int(float(response_data.get("sendTransactionResponse", {}).get(
+                    "return", {}).get("C24TRANRES", {}).get("ACTION_CODE", "-111111")))
+                data["statement_reference"] = f'{response_data.get("sendTransactionResponse", {}).get("return", {}).get("C24TRANRES", {}).get("STAN", "")}'
+                if data["code"]:
+                    data["message"] = "Transaction Failed"
+                else:
+                    data["message"] = "Success"
+                data["transactions"] = []
+
+                transactions = response_data.get("sendTransactionResponse", {}).get("return", {}).get(
+                    "C24TRANRES", {}).get("TRANS_INFO", {}).get("TRAN", {}).get("element", [])
+
+                for i in range(len(transactions)):
+                    transaction.update({
+                        "currency_code": response_data.get("sendTransactionResponse", {}).get(
+                            "return", {}).get("C24TRANRES", {}).get("BALANCE_CURRENCY", "NGN"),
+                        "date": datetime.strptime(f'{transactions[i].get("TRAN_DATE", None)}', '%Y%d%m').strftime('%Y-%m-%d'),
+
+                        "description": transactions[i].get("NARRATION", ""),
+                        "amount": transactions[i].get("TRAN_AMT", -1),
+                        "running_balance": transactions[i].get("BALANCE", -1),
+
+                        "transaction_id": transactions[i].get("TRAN_ID", ""),
+                        "serial": f'{transactions[i].get("TRAN_SNUM", "")}',
+                        "value_date": datetime.strptime(f'{transactions[i].get("VALUE_DATE", None)}', '%Y%d%m').strftime('%Y-%m-%d'),
+                        "posted_date": datetime.strptime(f'{transactions[i].get("DATE_POSTED", None)}', '%Y%d%m%H%M%S').strftime('%Y-%m-%d %H:%M:%S'),
+                    })
 
-                    data["message"] = response_data.get("message", "")
-                    data["code"] = f'{response_data.get("code", "-111111")}'
-                    data["statement_time"] = response_data.get("statement_time", "")
-                    data["statement_reference"] = response_data.get("statement_reference", "")
-
-                    data["total_transactions"] = f'{response_data.get("total_transactions", "0")}'
-                    data["num_pages"] = f'{response_data.get("num_pages", "0")}'
-                    data["page_has_next"] = response_data.get("page_has_next", False)
-                    data["transactions_count"] = f'{len(response_data.get("data", {}).get("transactions", []))}'
-                    data["transactions"] = []
+                    if transactions[i].get("PART_TRAN_TYPE", "") == "D":
+                        transaction["type"] = "Debit"
+                    elif transactions[i].get("PART_TRAN_TYPE", "") == "C":
+                        transaction["type"] = "Credit"
+
+                    if transactions[i].get("REF_NUM", {}).get("@null", "true") == "true":
+                        transaction["reference"] = ""
+
+                    data["transactions"].append(transaction)
+
+        elif super().get_operation() == super().PDF_TO_JSON or super().get_operation() == super().GET_JSON_PDF:
+            data = self.standardize_pdf_to_json(response_data=response_data)
+
+        elif super().get_operation() == super().FOREX_RATE:
+
+            if isinstance(response_data, dict):
+                data["message"] = response_data.get("message", "")
+                data["code"] = f'{response_data.get("code", -111111)}'
+
+                if 'data' in response_data.keys():
+                    data['data'] = {
+                        "converted_amount": response_data.get('data', {}).get("convertedAmount", -1),
+                        "rate": response_data.get('data', {}).get("rate", -1),
+                        "from_amount": response_data.get('data', {}).get("fromAmount", -1),
+                        "rate_code": response_data.get('data', {}).get("rateCode", "")
+                    }
 
-                    transactions = response_data.get("data", {}).get("transactions", [])
+            else:
+                data['response'] = response_data
 
-                    for i in range(len(transactions)):
-                        transaction={}
-                        transaction.update(self.get_full_statement_transaction_dict())
-                        
-                        # The reference below is a callback reference sent with the full statememt
-                        # if the fullstatement sent, is one that relates to a callback reference 
-                        # linked to a payment request made earlier.
-
-                        # Ideally the logic above is why we have to code below.
-                        # but NCBA does not have a fullstatement API, the data being returned is from the IPN alerts
-                        # that will be standardized to a full statement response.
-
-                        # Therefore this means that the reference we get back from the alerts will always be a reference initiated by Nash
-                        if transactions[i].get("reference", None)!=None:
-                            transaction['nash_reference']=transactions[i].get("reference")
-
-                        transaction.update(
-                            {
-                                "currency_code": response_data.get("currency_code", ""),
-                                "reference": transactions[i].get("reference",None),                               
-                                "date": transactions[i].get("date", ""),
-                                "description": f'{transactions[i].get("status", "")} {transactions[i].get("narrative", "")} {transactions[i].get("customer_name", "")}',
-                                "transaction_id": transactions[i].get("trans_id",transactions[i].get("transaction_id","")),
-                                "value_date": transactions[i].get("date", ""),
-                                "posted_date": transactions[i].get("date", ""),
-                                "amount": f'{round(float(transactions[i].get("trans_ammount", "0.00")),2)}',
-                                "type": f'{transactions[i].get("type", "")}',
-                            }
-                        )
+        elif super().get_operation() == super().JOBS_ACCOUNT_BALANCES:
+            data = []
+            if super().get_bank_id() == super().COOP:
+                for account_balance_data in response_data.get('data', []):
+                    data.append({
+                        "status": account_balance_data.get("status", -1),
+                        "created_at": account_balance_data.get("created_at", ''),
+                        "available_balance": account_balance_data.get('account_balance_response', {}).get("AvailableBalance", ''),
+                    })
 
-                        if float(transaction['amount'])<0:
-                            transaction['amount']=f"{float(transaction['amount'])*-1}"
+                    if account_balance_data.get("status", -1) != 0:
+                        data["available_balance_error"] = account_balance_data.get(
+                            'account_balance_response', {})
 
-                        data["transactions"].append(transaction)
+        elif super().get_operation() == super().JOBS_ACCOUNT_STATEMENT:
+            data = []
+            if super().get_bank_id() == super().COOP:
 
-            elif super().get_operation() == super().PDF_TO_JSON or super().get_operation() == super().GET_JSON_PDF:
-                data = self.standardize_pdf_to_json(response_data=response_data)
+                for account_statement_data in response_data.get('data', []):
+                    data.append({
+                        "status": account_statement_data.get("status", -1),
+                        "created_at": account_statement_data.get("created_at", ''),
+                        "transactions": [],
+                    })
 
-            elif super().get_operation() == super().FOREX_RATE:
-                data["code"] = "-111111"
-                data['message'] = response_data
-                if isinstance(response_data, dict):                    
-                    if super().get_bank_id() == super().EQUITY:
-                        data["message"] = response_data.get("message", "")
-                        data["code"] = f'{response_data.get("code", "-111111")}'
-                        data['rate'] = f'{response_data.get("data", {}).get("rate", "-1")}'
-                        data['rate_type'] = f'{response_data.get("data", {}).get("rateCode", "")}'
-                    elif super().get_bank_id() == super().COOP:
-                        data["message"] = response_data.get("MessageDescription", "")
-                        data["code"] = f'{response_data.get("MessageCode", "-111111")}'
-                        data['rate'] = f'{response_data.get("Rate", "-1")}'
-                        data['rate_type'] = f'{response_data.get("RateType", "")}'
-                        if data["code"] == 'S_001':
-                            data["code"] = "0"
-                        else:
-                            data["code"] = "-111111"
-                            data['message'] = response_data                    
-
-            elif super().get_operation() == super().JOBS_ACCOUNT_BALANCES:
-                data = []
-                if super().get_bank_id() == super().COOP:
-                    for account_balance_data in response_data.get('data', []):
-                        data.append({
-                            "status": f'{account_balance_data.get("status", "-1")}',
-                            "created_at": account_balance_data.get("created_at", ''),
-                            "available_balance": f'{account_balance_data.get("account_balance_response", {}).get("AvailableBalance", "0")}',
-                        })
+                    if account_statement_data.get("status", -1) != 0:
+                        data[-1]["transaction_error"] = account_statement_data.get(
+                            'account_statement_response', {})
 
-                        if account_balance_data.get("status", -1) != 0:
-                            data["available_balance_error"] = account_balance_data.get(
-                                'account_balance_response', {})
-
-            elif super().get_operation() == super().JOBS_ACCOUNT_STATEMENT:
-                data = []
-                if super().get_bank_id() == super().COOP:
-
-                    for account_statement_data in response_data.get('data', []):
-                        data.append({
-                            "status": account_statement_data.get("status", -1),
-                            "created_at": account_statement_data.get("created_at", ''),
-                            "transactions": [],
-                        })
+                    else:
+                        transactions_data = account_statement_data.get(
+                            'account_statement_response', {}).get("Transactions", [])
+                        for transaction in transactions_data:
+                            transaction_data = {
+                                "date": transaction.get("TransactionDate", ''),
+                                "description": transaction.get("Narration", ''),
+                                "reference": transaction.get("TransactionReference", ''),
+                            }
 
-                        if account_statement_data.get("status", -1) != 0:
-                            data[-1]["transaction_error"] = account_statement_data.get(
-                                'account_statement_response', {})
-
-                        else:
-                            transactions_data = account_statement_data.get(
-                                'account_statement_response', {}).get("Transactions", [])
-                            for transaction in transactions_data:
-                                transaction_data = {
-                                    "date": transaction.get("TransactionDate", ''),
-                                    "description": transaction.get("Narration", ''),
-                                    "reference": transaction.get("TransactionReference", ''),
-                                }
-
-                                if transaction.get("TransactionType", "") == "D":
-                                    transaction_data["amount"] = f'{transaction.get("DebitAmount", "0")}'
-                                    transaction_data["type"] = "Debit"
-
-                                elif transaction.get("TransactionType", "") == "C":
-                                    transaction_data["amount"] = f'{transaction.get("CreditAmount", "0")}'
-                                    transaction_data["type"] = "Credit"
-
-                                data[-1].get("transactions", []
-                                            ).append(transaction_data)
-
-            if bool(data):
-                if isinstance(data, dict):
-                    if 'transactions' in data.keys() and 'code' in data.keys():
-                        if len(data["transactions"]) == 0 and int(data["code"]) == "-111111":
-                            data['error'] = response_data
-                return data
-            if super().get_bank_id() in super().THIRD_PARTY_BANKING.keys():
-                return response_data
-        except Exception as e:
-            data['code']="-111111"
-            data['sync_error']=str(e)
-            data['bank_core_response']=response_data
+                            if transaction.get("TransactionType", "") == "D":
+                                transaction_data["amount"] = transaction.get(
+                                    "DebitAmount", "")
+                                transaction_data["type"] = "Debit"
+
+                            elif transaction.get("TransactionType", "") == "C":
+                                transaction_data["amount"] = transaction.get(
+                                    "CreditAmount", "")
+                                transaction_data["type"] = "Credit"
+
+                            data[-1].get("transactions", []
+                                         ).append(transaction_data)
+
+        if bool(data):
+            if isinstance(data, dict):
+                if 'transactions' in data.keys() and 'code' in data.keys():
+                    if len(data["transactions"]) == 0 and int(data["code"]) == -111111:
+                        data['error'] = response_data
             return data
+        if super().get_bank_id() in super().THIRD_PARTY_BANKING.keys():
+            return response_data
 
         return response_data
```

### Comparing `nashbanksync-0.1.80/bank_sync/Resources/operations.py` & `nashbanksync-0.1.9/bank_sync/Resources/operations.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 class Operations(object):
 
     # These are the banking integrations
     # Each with a unique ID
-    AUTHENTICATE = -1
-    GLOBAL = AUTHENTICATE + 1
+    GLOBAL = 0
     COOP = GLOBAL + 1
     EQUITY = COOP + 1
     NCBA = EQUITY + 1
     DAPI = NCBA + 1
     MONO = DAPI + 1
     PLAID = MONO + 1
     STITCH = PLAID + 1
@@ -15,16 +14,16 @@
     UBA = DTB + 1
     KCB = UBA + 1
     SCB = KCB + 1
     SAFCOM = SCB + 1
     FAULU = SAFCOM + 1
     CONSOLIDATED = FAULU + 1
     STANBIC = CONSOLIDATED + 1
-    FAMILY = STANBIC + 1
-    NCBA_LOOP = FAMILY + 1
+    FAMILY=STANBIC + 1
+    NCBA_LOOP=FAMILY + 1
 
     # These are the operations to be performed in Banking Identity
     # Each with a unique incremental ID
 
     # Returns Sample Data
     OPERATIONS = -2
     SAMPLE_DATA = OPERATIONS + 1
@@ -51,53 +50,22 @@
     BANKS_BY_ID = BANKS_BY_CODE + 1
     PDF_TO_JSON = BANKS_BY_ID + 1
     GET_JSON_PDF = PDF_TO_JSON + 1
     IPN_REGISTER = GET_JSON_PDF + 1
     IPN_GET = IPN_REGISTER + 1
     IPN_UPDATE = IPN_GET + 1
     IPN_DELETE = IPN_UPDATE + 1
-    IPN_DEACTIVATE = IPN_DELETE + 1
-    IPN_GENERATE_CLIENT_SECRET = IPN_DEACTIVATE + 1
+    IPN_GENERATE_CLIENT_SECRET = IPN_DELETE + 1
     JOBS_ACCOUNT_BALANCES = IPN_GENERATE_CLIENT_SECRET + 1
     JOBS_ACCOUNT_STATEMENT = JOBS_ACCOUNT_BALANCES + 1
 
-    AUTH_GET_TOKEN = JOBS_ACCOUNT_STATEMENT + 1
-    AUTH_AUTHORIZE = AUTH_GET_TOKEN + 1
-
-    # Equity Bank Payment Modes
-    POLARIS_CHANNEL = AUTH_AUTHORIZE + 1
-    MISYS = POLARIS_CHANNEL + 1
-
-    BANK_PAYMENT_MODES = {
-        IFT: 'IFT',
-        MOBILE_WALLET: 'MOBILE_WALLET',
-        PESALINK_TO_BANK: 'PESALINK_TO_BANK',
-        PESALINK_TO_MOBILE: 'PESALINK_TO_MOBILE',
-        RTGS: 'RTGS',
-        SWIFT: 'SWIFT',
-        EFT: 'EFT',
-        OMN: 'OMN',
-        POLARIS_CHANNEL: 'POLARIS_CHANNEL',
-        MISYS: 'MISYS'
-    }
-
     # All end points are placed in the BANKS_CONF
     # This is to allow easy standardization of the base url, endpoint and operations
     # When calling the APIs, in this case this is done in the resource class read function
     BANKS_CONF = {
-        AUTHENTICATE: {
-            "url": "https://authserver.dev.nashservices.nashglobal.co",
-            "read": {
-                "operations": {
-                    AUTH_GET_TOKEN: ("connect/token", "POST"),
-                    AUTH_AUTHORIZE: ("connect/authorize", "POST"),
-                }
-            }
-
-        },
         GLOBAL: {
             "url": "https://dev.bankingservices.nashglobal.co",
             "read": {
                 "endpoint": f"api/banks",
                 "operations": {
                     OPERATIONS: ("operations", "GET"),
                     SAMPLE_DATA: ("sample_payload", "POST"),
@@ -105,29 +73,28 @@
                     BANKS_BY_CODE: ("banks/by_code", "GET"),
                     BANKS_BY_ID: ("banks/by_id", "GET"),
                     COUNTRIES: ("countries", "GET"),
                     IPN_REGISTER: ("ipn/register", "POST"),
                     IPN_GET: ("ipn/get", "POST"),
                     IPN_UPDATE: ("ipn/update", "POST"),
                     IPN_DELETE: ("ipn/delete", "POST"),
-                    IPN_DEACTIVATE: ("ipn/deactivate", "POST"),
                     IPN_GENERATE_CLIENT_SECRET: ("ipn/generate_client_secret", "POST"),
                     JOBS_ACCOUNT_BALANCES: ("jobs/account_balances", "POST"),
                     JOBS_ACCOUNT_STATEMENT: ("jobs/account_statement", "POST"),
                 }
             }
 
         },
         UBA: {
             "url": "https://dev.bankingservices.nashglobal.co",
             "accounts": {
                 "endpoint": f"api/banks/accounts/{UBA}",
                 "operations": {
-                    BALANCE: ("balance", "POST"),
-                    FULL_STATEMENT: ("full_statement", "POST"),
+                    BALANCE: ("get_balance", "POST"),
+                    FULL_STATEMENT: ("get_full_statement", "POST"),
                 }
             },
             "payment": {
                 "endpoint": f"api/banks/payment/{UBA}",
                 "operations": {
                     IFT: ("ift", "POST"),
                 }
@@ -135,39 +102,39 @@
 
         },
         DTB: {
             "url": "https://dev.bankingservices.nashglobal.co",
             "accounts": {
                 "endpoint": f"api/banks/accounts/{DTB}",
                 "operations": {
-                    ACCOUNT_VALIDATION: ("validation", "POST"),
+                    ACCOUNT_VALIDATION: ("get_validation", "POST"),
                     PDF_TO_JSON: ("pdf_to_json", "POST"),
                     GET_JSON_PDF: ("uploaded_pdf_json", "POST"),
                 }
             },
             "payment": {
                 "endpoint": f"api/banks/payment/{DTB}",
                 "operations": {
                     IFT: ("ift", "POST"),
                     MOBILE_WALLET: ("mobile_wallet", "POST"),
-                    TRANSACTION_STATUS: ("transaction_status", "POST"),
+                    TRANSACTION_STATUS: ("get_transaction_status", "POST"),
                     STK_PUSH: ("c2b_stk_push", "POST"),
                 }
             }
 
         },
         EQUITY: {
             "url": "https://dev.bankingservices.nashglobal.co",
             "accounts": {
                 "endpoint": f"api/banks/accounts/{EQUITY}",
                 "operations": {
-                    BALANCE: ("balance", "POST"),
-                    MINI_STATEMENT: ("mini_statement", "POST"),
-                    ACCOUNT_VALIDATION: ("validation", "POST"),
-                    FULL_STATEMENT: ("full_statement", "POST"),
+                    BALANCE: ("get_balance", "POST"),
+                    MINI_STATEMENT: ("get_mini_statement", "POST"),
+                    ACCOUNT_VALIDATION: ("get_validation", "POST"),
+                    FULL_STATEMENT: ("get_full_statement", "POST"),
                     PDF_TO_JSON: ("pdf_to_json", "POST"),
                     GET_JSON_PDF: ("uploaded_pdf_json", "POST"),
                     FOREX_RATE: ("forex_rate", "POST")
                 }
             },
             "payment": {
                 "endpoint": f"api/banks/payment/{EQUITY}",
@@ -175,65 +142,63 @@
                     IFT: ("ift", "POST"),
                     MOBILE_WALLET: ("mobile_wallet", "POST"),
                     RTGS: ("rtgs", "POST"),
                     SWIFT: ("swift", "POST"),
                     EFT: ("eft", "POST"),
                     PESALINK_TO_BANK: ("pesalink/bank", "POST"),
                     PESALINK_TO_MOBILE: ("pesalink/mobile", "POST"),
-                    TRANSACTION_STATUS: ("transaction_status", "POST"),
+                    TRANSACTION_STATUS: ("get_transaction_status", "POST"),
                 }
             }
 
         },
         COOP: {
             "url": "https://dev.bankingservices.nashglobal.co",
             "accounts": {
                 "endpoint": f"api/banks/accounts/{COOP}",
                 "operations": {
-                    BALANCE: ("balance", "POST"),
-                    MINI_STATEMENT: ("mini_statement", "POST"),
-                    ACCOUNT_VALIDATION: ("validation", "POST"),
-                    FULL_STATEMENT: ("full_statement", "POST"),
-                    ACCOUNT_TRANSACTIONS: ("transactions", "POST"),
+                    BALANCE: ("get_balance", "POST"),
+                    MINI_STATEMENT: ("get_mini_statement", "POST"),
+                    ACCOUNT_VALIDATION: ("get_validation", "POST"),
+                    FULL_STATEMENT: ("get_full_statement", "POST"),
+                    ACCOUNT_TRANSACTIONS: ("get_transactions", "POST"),
                     PDF_TO_JSON: ("pdf_to_json", "POST"),
                     GET_JSON_PDF: ("uploaded_pdf_json", "POST"),
-                    FOREX_RATE: ("forex_rate", "POST")
                 }
             },
             "payment": {
                 "endpoint": f"api/banks/payment/{COOP}",
                 "operations": {
                     IFT: ("ift", "POST"),
                     MOBILE_WALLET: ("mobile_wallet", "POST"),
                     PESALINK_TO_BANK: ("pesalink/bank", "POST"),
                     PESALINK_TO_MOBILE: ("pesalink/mobile", "POST"),
-                    TRANSACTION_STATUS: ("transaction_status", "POST"),
+                    TRANSACTION_STATUS: ("get_transaction_status", "POST"),
                 }
             }
 
         },
         NCBA: {
             "url": "https://dev.bankingservices.nashglobal.co",
             "accounts": {
                 "endpoint": f"api/banks/accounts/{NCBA}",
                 "operations": {
                     PDF_TO_JSON: ("pdf_to_json", "POST"),
                     GET_JSON_PDF: ("uploaded_pdf_json", "POST"),
-                    FULL_STATEMENT: ("full_statement", "POST"),
                 }
             },
             "payment": {
                 "endpoint": f"api/banks/payment/{NCBA}",
                 "operations": {
                     IFT: ("ift", "POST"),
                     MOBILE_WALLET: ("mobile_wallet", "POST"),
                     RTGS: ("rtgs", "POST"),
                     EFT: ("eft", "POST"),
                     PESALINK_TO_BANK: ("pesalink/bank", "POST"),
-                    TRANSACTION_STATUS: ("transaction_status", "POST"),
+                    TRANSACTION_STATUS: ("get_transaction_status", "POST"),
                 }
             }
         },
         SAFCOM: {
             "url": "https://dev.bankingservices.nashglobal.co",
             "accounts": {
                 "endpoint": f"api/banks/accounts/{SAFCOM}",
@@ -325,65 +290,65 @@
 
     THIRD_PARTY_BANKING = {
         DAPI: {
             "url": "https://dev.3p.bankingservices.nashglobal.co",
             "accounts": {
                 "endpoint": f"api/v1/Dapi",
                 "operations": {
-                    BALANCE:  ("balance", "POST"),
-                    ACCOUNT_TRANSACTIONS: ("transactions", "POST")
-                }
+                    BALANCE:  ("get_balance", "POST"),
+                    ACCOUNT_TRANSACTIONS: ("get_transactions", "POST")
+                }                
             },
             "payment": {
                 "endpoint": f"api/v1/Dapi",
                 "operations": {
                     INITIATE_PAYMENT: ("initiate_payment", "POST"),
                 }
             }
         },
         MONO: {
             "url": "https://dev.3p.bankingservices.nashglobal.co",
             "accounts": {
                 "endpoint": f"api/v1/Mono",
                 "operations": {
-                    BALANCE:  ("balance", "POST"),
-                    ACCOUNT_TRANSACTIONS: ("transactions", "POST")
-                }
+                    BALANCE:  ("get_balance", "POST"),
+                    ACCOUNT_TRANSACTIONS: ("get_transactions", "POST")
+                }                
             },
             "payment": {
                 "endpoint": f"api/v1/Mono",
                 "operations": {
                     INITIATE_PAYMENT: ("initiate_payment", "POST"),
                 }
             }
         },
         PLAID: {
             "url": "https://dev.3p.bankingservices.nashglobal.co",
             "accounts": {
                 "endpoint": f"api/v1/Plaid",
                 "operations": {
-                    BALANCE:  ("balance", "POST"),
-                    ACCOUNT_TRANSACTIONS: ("transactions", "POST")
-                }
+                    BALANCE:  ("get_balance", "POST"),
+                    ACCOUNT_TRANSACTIONS: ("get_transactions", "POST")
+                }                
             },
             "payment": {
                 "endpoint": f"api/v1/Plaid",
                 "operations": {
                     INITIATE_PAYMENT: ("initiate_payment", "POST"),
                 }
             }
         },
         STITCH: {
             "url": "https://dev.3p.bankingservices.nashglobal.co",
             "accounts": {
                 "endpoint": f"api/v1/Stitch",
                 "operations": {
-                    BALANCE:  ("balance", "POST"),
-                    ACCOUNT_TRANSACTIONS: ("transactions", "POST")
-                }
+                    BALANCE:  ("get_balance", "POST"),
+                    ACCOUNT_TRANSACTIONS: ("get_transactions", "POST")
+                }                
             },
             "payment": {
                 "endpoint": f"api/v1/Stitch",
                 "operations": {
                     INITIATE_PAYMENT: ("initiate_payment", "POST"),
                 }
             }
```

### Comparing `nashbanksync-0.1.80/bank_sync/Resources/payments.py` & `nashbanksync-0.1.9/bank_sync/Resources/payments.py`

 * *Files 19% similar despite different names*

```diff
@@ -20,46 +20,46 @@
 
     def set_bank_id(self, bank_id):
         # This is done to help with URL standardization in the operations and resource classes
         super().set_action(action='payment')
         return super().set_bank_id(bank_id)
 
     def ift(self, payload=None):
-        return self.execute_payment(payload=payload)
+        self.register_callback()
+        return super().read(payload=payload)
 
     def eft(self, payload=None):
-        return self.execute_payment(payload=payload)
+        self.register_callback()
+        return super().read(payload=payload)
 
     def rtgs(self, payload=None):
-        return self.execute_payment(payload=payload)
+        self.register_callback()
+        return super().read(payload=payload)
 
     def swift(self, payload=None):
-        return self.execute_payment(payload=payload)
+        self.register_callback()
+        return super().read(payload=payload)
 
     def transaction_status(self, payload=None):
+
         return super().read(payload=payload)
 
     def mobile_wallet(self, payload=None):
-        return self.execute_payment(payload=payload)
+        self.register_callback()
+        return super().read(payload=payload)
 
     def pesalink_to_bank(self, payload=None):
-        return self.execute_payment(payload=payload)
+        self.register_callback()
+        return super().read(payload=payload)
 
     def pesalink_to_mobile(self, payload=None):
-        return self.execute_payment(payload=payload)
-
-    def execute_payment(self, payload=None):
-        try:
-            self.register_callback()
-            return super().read(payload=payload)
-        except Exception as e:
-            return super().set_error(str(e))
+        self.register_callback()
+        return super().read(payload=payload)
 
     # API Endpoint used by third party integrations
-
     def initiate_payment(self, payload=None):
 
         return super().read(payload=payload)
 
     def serialize(self, payload=None, operation=None):
         # Set the Operation being executed
         # Set the Original request sent before serialization
@@ -82,15 +82,15 @@
                 })
                 data.update({
                     "CallBackUrl": self.bank_sync_call_back.get("payments", "")
                 })
                 data.update({
                     "Source": {
                         "AccountNumber": payload.get("source", {}).get("account_number", None),
-                        "Amount": f'{payload.get("source", {}).get("amount", None)}',
+                        "Amount": payload.get("source", {}).get("amount", None),
                         "TransactionCurrency": payload.get("transfer", {}).get("currency_code", None),
                         "Narration": payload.get("transfer", {}).get("description", "")
                     }
                 })
 
                 destinations = payload.get("destinations", [])
 
@@ -102,15 +102,15 @@
 
                     data["Destinations"].append(
                         {
                             "ReferenceNumber": f'{default_reference}_1',
                             "AccountNumber": destinations[i].get("account_number", None),
                             "BankCode": payload.get("transfer", {}).get("bank_code", None),
                             "BranchCode": payload.get("transfer", {}).get("branch_code", None),
-                            "Amount": f'{destinations[i].get("amount", None)}',
+                            "Amount": destinations[i].get("amount", None),
                             "TransactionCurrency": payload.get("transfer", {}).get("currency_code", None),
                             "Narration": payload.get("transfer", {}).get("description", "")
                         }
                     )
             # If bank_id is EQUITY
             elif super().get_bank_id() == super().EQUITY:
                 data.update({
@@ -127,70 +127,68 @@
 
                     data.update({
                         "destination": {
                             "type": "bank",
                             "countryCode": destination.get("country_code", None),
                             "name": destination.get("name", None),
                             "accountNumber": destination.get("account_number", None),
-                            "mobileNumber": destination.get("mobile_number", None),
                         }
                     })
 
                     data.update({
                         "transfer": {
                             "type": "InternalFundsTransfer",
                             "amount": f'{destination.get("amount",None)}',
                             "currencyCode": payload.get("transfer", {}).get("currency_code", None),
-                            "reference": f'{default_reference}',
+                            "reference": payload.get("transfer", {}).get("reference", None),
                             "date": payload.get("transfer", {}).get("date", None),
                             "description": payload.get("transfer", {}).get("description", ""),
                         }
                     })
             # If bank_id is NCBA
             elif super().get_bank_id() == super().NCBA:
 
                 destinations = payload.get("destinations", [])
                 if len(destinations) > 0:
                     destination = destinations[0]
 
                     data.update({
-                        "account_number": payload.get("source", {}).get("account_number", None),
                         "BankCode": payload.get("transfer", {}).get("bank_code", None),
                         "BankSwiftCode": payload.get("transfer", {}).get("bank_swift_code", None),
                         "BranchCode": payload.get("transfer", {}).get("branch_code", None),
-                        "BeneficiaryAccountName": destination.get("name", None),
+                        "BeneficiaryAccountName": payload.get("destination", {}).get("name", None),
                         "Country": payload.get("transfer", {}).get("country", None),
                         "Reference": f'{default_reference}',
                         "Currency": payload.get("transfer", {}).get("currency_code", None),
                         "Account": destination.get("account_number", None),
-                        "Amount": float(destination.get("amount", 0)),
+                        "Amount": destination.get("amount", None),
                         "Narration": payload.get("transfer", {}).get("description", None),
                         "Transaction Date": payload.get("transfer", {}).get("date", date.today().strftime('%Y%m%d')).replace("-", ""),
                     })
             # If bank_id is DTB
             elif super().get_bank_id() == super().DTB:
                 destinations = payload.get("destinations", [])
                 if len(destinations) > 0:
                     destination = destinations[0]
                     data.update({
                         "identifier": {
-                            "xref": f'API-{default_reference}',
+                            "xref": f'API-{payload.get("transfer", {}).get("reference", get_code())}',
                             "channel": "API",
                             "bank_code": payload.get("transfer", {}).get("bank_code", ""),
                         },
                         "content": {
-                            "source_reference": f'{default_reference}',
+                            "source_reference": payload.get("transfer", {}).get("reference", get_code()),
                             "product": "FTIN",
                             "transaction_branch": payload.get("transfer", {}).get("branch_code", ""),
                             "debit_party": payload.get("source", {}).get("account_number", ""),
                             "credit_party": destination.get("account_number", ""),
                             "debit_currency": payload.get("transfer", {}).get("currency_code", ""),
                             "credit_currency": payload.get("transfer", {}).get("currency_code", ""),
                             "exchange_rate": 1,
-                            "transaction_amount": f'{destination.get("amount", 0)}',
+                            "transaction_amount": destination.get("amount", 0),
                             "transaction_date": payload.get("transfer", {}).get("date", ""),
                             "value_date": payload.get("transfer", {}).get("date", ""),
                             "narration": payload.get("transfer", {}).get("description", ""),
                             "udf": [
                                 {
                                     "field_name": "ACUMEN_CODE",
                                     "field_value": "NONE"
@@ -230,15 +228,15 @@
                 })
                 data.update({
                     "CallBackUrl": self.bank_sync_call_back.get("payments", "")
                 })
                 data.update({
                     "Source": {
                         "AccountNumber": f'{payload.get("source", {}).get("account_number", None)}',
-                        "Amount": f'{payload.get("source", {}).get("amount", None)}',
+                        "Amount": payload.get("source", {}).get("amount", None),
                         "TransactionCurrency": payload.get("transfer", {}).get("currency_code", None),
                         "Narration": payload.get("transfer", {}).get("description", "")
                     }
                 })
 
                 destinations = payload.get("destinations", [])
 
@@ -248,15 +246,15 @@
                             "Destinations": []
                         })
 
                     data["Destinations"].append(
                         {
                             "ReferenceNumber": f'{default_reference}_1',
                             "MobileNumber": f'{destinations[i].get("mobile_number",None)}',
-                            "Amount": f'{destinations[i].get("amount", None)}',
+                            "Amount": destinations[i].get("amount", None),
                             "Narration": payload.get("transfer", {}).get("description", "")
                         }
                     )
             # If bank_id is EQUITY
             elif super().get_bank_id() == super().EQUITY:
                 data.update({
                     "source": {
@@ -272,76 +270,76 @@
 
                     data.update({
                         "destination": {
                             "type": "mobile",
                             "countryCode": destination.get("country_code", None),
                             "name": destination.get("name", None),
                             "mobileNumber": destination.get("mobile_number", None),
-                            "walletName": destination.get("operator", None),
+                            "walletName": destination.get("wallet_name", None),
                         }
                     })
 
                     data.update({
                         "transfer": {
                             "type": "MobileWallet",
                             "amount": f'{destination.get("amount",None)}',
                             "currencyCode": payload.get("transfer", {}).get("currency_code", None),
-                            "reference": f'{default_reference}',
+                            "reference": payload.get("transfer", {}).get("reference", None),
                             "date": payload.get("transfer", {}).get("date", None),
                             "description": payload.get("transfer", {}).get("description", ""),
                             "callbackUrl": self.bank_sync_call_back.get("payments", ""),
                         }
                     })
             # If bank_id is DTB
             elif super().get_bank_id() == super().DTB:
                 destinations = payload.get("destinations", [])
                 if len(destinations) > 0:
                     destination = destinations[0]
 
                     data.update({
-                        "operator": destination.get("operator", ""),
+                        "operator": destination.get("wallet_name", ""),
                         "identifier": {
-                            "xref": f'API-{default_reference}',
+                            "xref": f'API-{payload.get("transfer", {}).get("reference", get_code())}',
                             "channel": "API",
                             "bank_code": payload.get("transfer", {}).get("bank_code", ""),
                         },
                         "content": {
-                            "cbs_reference": get_code(),
-                            "transaction_amount": f'{float(destination.get("amount", 0))}',
+                            "cbs_reference": payload.get("transfer", {}).get("ift_reference", ""),
+                            "transaction_amount": int(float(destination.get("amount", 0))),
                             "credit_party": payload.get("source", {}).get("account_number", ""),
                             "customer_msisdn": destination.get("mobile_number", ""),
                             "customer_name": destination.get("name", ""),
-                            "account_reference": f'{default_reference}',
+                            "account_reference": payload.get("transfer", {}).get("reference", ""),
                             "invoice_number": payload.get("transfer", {}).get("invoice_id", ""),
                             "narration": payload.get("transfer", {}).get("description", ""),
                             "transaction_type": payload.get("transfer", {}).get("type", ""),
                         }
                     })
 
             # If bank_id is NCBA
             elif super().get_bank_id() == super().NCBA:
 
                 destinations = payload.get("destinations", [])
                 if len(destinations) > 0:
                     destination = destinations[0]
 
                     data.update({
-                        "account_number": payload.get("source", {}).get("account_number", None),
-                        "TranType": destination.get("operator", ""),
                         "BankCode": payload.get("transfer", {}).get("bank_code", None),
                         "BankSwiftCode": payload.get("transfer", {}).get("bank_swift_code", None),
                         "BranchCode": payload.get("transfer", {}).get("branch_code", None),
                         "BeneficiaryAccountName": destination.get("name", None),
                         "Country": payload.get("transfer", {}).get("country", None),
+                        "TranType": "Mpesa",
                         "Reference": f'{default_reference}',
                         "Currency": payload.get("transfer", {}).get("currency_code", None),
                         "Account": destination.get("mobile_number", None),
-                        "Amount": float(destination.get("amount", 0)),
+                        "Amount": destination.get("amount", None),
                         "Narration": payload.get("transfer", {}).get("description", None),
-                        "Transaction Date": payload.get("transfer", {}).get("date", date.today().strftime('%Y%m%d')).replace("-", "")
+                        "Transaction Date": payload.get("transfer", {}).get("date", date.today().strftime('%Y%m%d')).replace("-", ""),
+                        "Validation ID": f'{default_reference}',
                     })
         elif operation == super().RTGS:
 
             # If bank_id is COOP
             if super().get_bank_id() == super().COOP:
                 pass
             elif super().get_bank_id() == super().EQUITY:
@@ -369,56 +367,43 @@
                     })
 
                     data.update({
                         "transfer": {
                             "type": "RTGS",
                             "amount": f'{destination.get("amount",None)}',
                             "currencyCode": payload.get("transfer", {}).get("currency_code", None),
-                            "reference": f'{default_reference}',
+                            "reference": payload.get("transfer", {}).get("reference", None),
                             "date": payload.get("transfer", {}).get("date", None),
                             "description": payload.get("transfer", {}).get("description", ""),
                         }
                     })
             # If bank_id is NCBA
             elif super().get_bank_id() == super().NCBA:
 
                 destinations = payload.get("destinations", [])
                 if len(destinations) > 0:
                     destination = destinations[0]
 
                     data.update({
-                        "account_number": payload.get("source", {}).get("account_number", None),
                         "BankCode": payload.get("transfer", {}).get("bank_code", None),
                         "BankSwiftCode": payload.get("transfer", {}).get("bank_swift_code", None),
                         "BranchCode": payload.get("transfer", {}).get("branch_code", None),
                         "BeneficiaryAccountName": destination.get("name", None),
                         "Country": payload.get("transfer", {}).get("country", None),
+                        "TranType": "RTGS",
                         "Reference": f'{default_reference}',
                         "Currency": payload.get("transfer", {}).get("currency_code", None),
                         "Account": destination.get("account_number", None),
-                        "Amount": float(destination.get("amount", None)),
+                        "Amount": destination.get("amount", None),
                         "Narration": payload.get("transfer", {}).get("description", None),
                         "Transaction Date": payload.get("transfer", {}).get("date", date.today().strftime('%Y%m%d')).replace("-", ""),
-
-                        # These will be required fields as per the new NCBA Docs
-                        # The API works well without them for now.
-                        # NCBA adviced they are not required for now
-
-                        # "SenderName": payload.get("source", {}).get("name", None),
-                        # "Purpose of Payment": payload.get("transfer", {}).get("description", None),
-                        # "Sender Principle Activity": payload.get("source", {}).get("sender_principle_activity", None),
-                        # "Sender Address": payload.get("source", {}).get("address", None),
-                        # "Receiver Address": destination.get("address", None),
-                        # "Receiver ID": destination.get("receiver_id", None),
-                        # "Sender ID": payload.get("source", {}).get("sender_id", None),
-                        # "BeneficiaryName": destination.get("name", None),
                     })
         elif operation == super().SWIFT:
 
-            # If bank_id is EQUITY
+            # If bank_id is COOP
             if super().get_bank_id() == super().EQUITY:
                 data.update({
                     "source": {
                         "countryCode": payload.get("source", {}).get("country_code", None),
                         "name": payload.get("source", {}).get("name", None),
                         "accountNumber": payload.get("source", {}).get("account_number", None),
                         "sourceCurrency": payload.get("source", {}).get("currency_code", None),
@@ -442,15 +427,15 @@
                     })
 
                     data.update({
                         "transfer": {
                             "type": "SWIFT",
                             "amount": f'{destination.get("amount",None)}',
                             "currencyCode": payload.get("transfer", {}).get("currency_code", None),
-                            "reference": f'{default_reference}',
+                            "reference": payload.get("transfer", {}).get("reference", None),
                             "date": payload.get("transfer", {}).get("date", None),
                             "description": payload.get("transfer", {}).get("description", ""),
                             "chargeOption": "SELF"
                         }
                     })
         elif operation == super().EFT:
 
@@ -463,54 +448,41 @@
             elif super().get_bank_id() == super().NCBA:
 
                 destinations = payload.get("destinations", [])
                 if len(destinations) > 0:
                     destination = destinations[0]
 
                     data.update({
-                        "account_number": payload.get("source", {}).get("account_number", None),
                         "BankCode": payload.get("transfer", {}).get("bank_code", None),
                         "BankSwiftCode": payload.get("transfer", {}).get("bank_swift_code", None),
                         "BranchCode": payload.get("transfer", {}).get("branch_code", None),
                         "BeneficiaryAccountName": destination.get("name", None),
+                        "BeneficiaryName": destination.get("name", None),
                         "Country": payload.get("transfer", {}).get("country", None),
                         "Reference": f'{default_reference}',
                         "Currency": payload.get("transfer", {}).get("currency_code", None),
                         "Account": destination.get("account_number", None),
-                        "Amount": float(destination.get("amount", 0)),
+                        "Amount": f'{destination.get("amount", None)}',
                         "Narration": payload.get("transfer", {}).get("description", None),
                         "Transaction Date": payload.get("transfer", {}).get("date", date.today().strftime('%Y%m%d')).replace("-", ""),
-
-                        # These will be required fields as per the new NCBA Docs
-                        # The API works well without them for now.
-                        # TODO Confirm the above assertion
-
-                        # "SenderName": payload.get("source", {}).get("name", None),
-                        # "Purpose of Payment": payload.get("transfer", {}).get("description", None),
-                        # "Sender Principle Activity": payload.get("source", {}).get("sender_principle_activity", None),
-                        # "Sender Address": payload.get("source", {}).get("address", None),
-                        # "Receiver Address": destination.get("address", None),
-                        # "Receiver ID": destination.get("receiver_id", None),
-                        # "Sender ID": payload.get("source", {}).get("sender_id", None),
-                        # "BeneficiaryName": destination.get("name", None),
                     })
         elif operation == super().PESALINK_TO_BANK:
 
             # If bank_id is COOP
             if super().get_bank_id() == super().COOP:
                 data.update({
                     "MessageReference": f'{default_reference}'
                 })
                 data.update({
                     "CallBackUrl": self.bank_sync_call_back.get("payments", "")
                 })
                 data.update({
                     "Source": {
                         "AccountNumber": payload.get("source", {}).get("account_number", None),
-                        "Amount": f'{payload.get("source", {}).get("amount", None)}',
+                        "Amount": payload.get("source", {}).get("amount", None),
                         "TransactionCurrency": payload.get("transfer", {}).get("currency_code", None),
                         "Narration": payload.get("transfer", {}).get("description", "")
                     }
                 })
 
                 destinations = payload.get("destinations", [])
 
@@ -521,15 +493,15 @@
                         })
 
                     data["Destinations"].append(
                         {
                             "ReferenceNumber": f'{default_reference}_1',
                             "AccountNumber": destinations[i].get("account_number", None),
                             "BankCode": payload.get("transfer", {}).get("bank_code", None),
-                            "Amount": f'{destinations[i].get("amount", None)}',
+                            "Amount": destinations[i].get("amount", None),
                             "TransactionCurrency": payload.get("transfer", {}).get("currency_code", None),
                             "Narration": payload.get("transfer", {}).get("description", "")
                         }
                     )
             # If bank_id is EQUITY
             elif super().get_bank_id() == super().EQUITY:
                 data.update({
@@ -556,68 +528,53 @@
                     })
 
                     data.update({
                         "transfer": {
                             "type": "PesaLink",
                             "amount": f'{destination.get("amount",None)}',
                             "currencyCode": payload.get("transfer", {}).get("currency_code", None),
-                            "reference": f'{default_reference}',
+                            "reference": payload.get("transfer", {}).get("reference", None),
                             "date": payload.get("transfer", {}).get("date", None),
                             "description": payload.get("transfer", {}).get("description", ""),
                         }
                     })
             # If bank_id is NCBA
             elif super().get_bank_id() == super().NCBA:
 
                 destinations = payload.get("destinations", [])
                 if len(destinations) > 0:
                     destination = destinations[0]
 
                     data.update({
-                        "account_number": payload.get("source", {}).get("account_number", None),
-                        "BankCode": "404",
+                        "BankCode": payload.get("transfer", {}).get("bank_code", None),
                         "BankSwiftCode": payload.get("transfer", {}).get("bank_swift_code", None),
-                        "BranchCode": payload.get("transfer", {}).get("bank_code", None),
+                        "BranchCode": payload.get("transfer", {}).get("branch_code", None),
                         "BeneficiaryAccountName": destination.get("name", None),
-                        "BeneficiaryName": destination.get("name", None),
                         "Country": payload.get("transfer", {}).get("country", None),
                         "Reference": f'{default_reference}',
                         "Currency": payload.get("transfer", {}).get("currency_code", None),
                         "Account": destination.get("account_number", None),
-                        "Amount": float(destination.get("amount", None)),
+                        "Amount": destination.get("amount", None),
                         "Narration": payload.get("transfer", {}).get("description", None),
                         "Transaction Date": payload.get("transfer", {}).get("date", date.today().strftime('%Y%m%d')).replace("-", ""),
-
-                        # These will be required fields as per the new NCBA Docs
-                        # The API works well without them for now.
-                        # TODO Confirm the above assertion
-
-                        # "SenderName": payload.get("source", {}).get("name", None),
-                        # "Purpose of Payment": payload.get("transfer", {}).get("description", None),
-                        # "Sender Principle Activity": payload.get("source", {}).get("sender_principle_activity", None),
-                        # "Sender Address": payload.get("source", {}).get("address", None),
-                        # "Receiver Address": destination.get("address", None),
-                        # "Receiver ID": destination.get("receiver_id", None),
-                        # "Sender ID": payload.get("source", {}).get("sender_id", None),
-                        # "BeneficiaryName": destination.get("name", None),
                     })
         elif operation == super().PESALINK_TO_MOBILE:
 
             # If bank_id is COOP
             if super().get_bank_id() == super().COOP:
                 data.update({
                     "MessageReference": f'{default_reference}'
                 })
                 data.update({
                     "CallBackUrl": self.bank_sync_call_back.get("payments", "")
                 })
                 data.update({
                     "Source": {
                         "AccountNumber": payload.get("source", {}).get("account_number", None),
-                        "Amount": f'{payload.get("source", {}).get("amount", None)}',
+                        "Amount": payload.get("source", {}).get("amount", None),
                         "TransactionCurrency": payload.get("transfer", {}).get("currency_code", None),
                         "Narration": payload.get("transfer", {}).get("description", "")
                     }
                 })
 
                 destinations = payload.get("destinations", [])
 
@@ -627,15 +584,15 @@
                             "Destinations": []
                         })
 
                     data["Destinations"].append(
                         {
                             "ReferenceNumber": f'{default_reference}_1',
                             "PhoneNumber": destinations[i].get("mobile_number", None),
-                            "Amount": f'{destinations[i].get("amount", None)}',
+                            "Amount": destinations[i].get("amount", None),
                             "TransactionCurrency": payload.get("transfer", {}).get("currency_code", None),
                             "Narration": payload.get("transfer", {}).get("description", "")
                         }
                     )
             # If bank_id is EQUITY
             elif super().get_bank_id() == super().EQUITY:
                 data.update({
@@ -652,25 +609,24 @@
 
                     data.update({
                         "destination": {
                             "type": "mobile",
                             "countryCode": destination.get("country_code", None),
                             "name": destination.get("name", None),
                             "mobileNumber": destination.get("mobile_number", None),
-                            "accountNumber": destination.get("account_number", None),
                             "bankCode": payload.get("transfer", {}).get("bank_code", None),
                         }
                     })
 
                     data.update({
                         "transfer": {
                             "type": "PesaLink",
                             "amount": f'{destination.get("amount",None)}',
                             "currencyCode": payload.get("transfer", {}).get("currency_code", None),
-                            "reference": f'{default_reference}',
+                            "reference": payload.get("transfer", {}).get("reference", None),
                             "date": payload.get("transfer", {}).get("date", None),
                             "description": payload.get("transfer", {}).get("description", ""),
                         }
                     })
             # If bank_id is NCBA
             elif super().get_bank_id() == super().NCBA:
                 pass
@@ -685,17 +641,16 @@
             elif super().get_bank_id() == super().EQUITY:
                 data.update({
                     "reference": payload.get("reference", None)
                 })
             # If bank_id is NCBA
             elif super().get_bank_id() == super().NCBA:
                 data.update({
-                    "account_number": payload.get("account_number", None),
-                    "ReferenceNumber": payload.get("reference", None),
-                    "Country": payload.get("country", None)
+                    "reference_number": payload.get("reference", None),
+                    "country": payload.get("country", None)
                 })
             # If bank_id is DTB
             elif super().get_bank_id() == super().DTB:
                 data.update({
                     "identifier": {
                         "xref": get_code(),
                         "channel": "API",
@@ -718,17 +673,17 @@
                         data = {
                             "secret": payload.get("transfer", {}).get("secret", ""),
                             "clientId": payload.get("transfer", {}).get("client_id", ""),
                             "receiptName": destination.get("name", ""),
                             "targetAccount": destination.get("account_number", ""),
                             "sortCode": payload.get("transfer", {}).get("sort_code", ""),
                             "currency": payload.get("transfer", {}).get("currency_code", ""),
-                            "value": f'{destination.get("amount", 0)}',
-                            "referenceID": f'{default_reference}',
-                            "referenceMetaData": f'{default_reference}',
+                            "value": destination.get("amount", 0),
+                            "referenceID": payload.get("transfer", {}).get("reference", ""),
+                            "referenceMetaData": payload.get("transfer", {}).get("reference", ""),
                             "type":  payload.get("transfer", {}).get("type", ""),
                             "description": payload.get("transfer", {}).get("description", ""),
                             "nickname": destination.get("name", ""),
                             "country": payload.get("transfer", {}).get("country", ""),
                             "branchAddress": payload.get("transfer", {}).get("branch_address", ""),
                             "branchName": payload.get("transfer", {}).get("branch_name", ""),
                             "swiftCode": payload.get("transfer", {}).get("bank_swift_code", ""),
@@ -749,190 +704,161 @@
             # If bank_id is DTB
             if super().get_bank_id() == super().DTB:
                 destinations = payload.get("destinations", [])
                 if len(destinations) > 0:
                     destination = destinations[0]
 
                     data.update({
-                        "operator": destination.get("operator", ""),
+                        "operator": destination.get("wallet_name", ""),
                         "identifier": {
-                            "xref": f'API-{default_reference}',
+                            "xref": f'API-{payload.get("transfer", {}).get("reference", get_code())}',
                             "channel": "API",
                             "bank_code": payload.get("transfer", {}).get("bank_code", ""),
                         },
                         "content": {
                             "timestamp": payload.get("transfer", {}).get("timestamp", ""),
-                            "transaction_amount": f'{float(destination.get("amount", 0))}',
+                            "transaction_amount": int(float(destination.get("amount", 0))),
                             "credit_party": payload.get("source", {}).get("account_number", ""),
                             "debit_party": destination.get("mobile_number", ""),
                             "customer_msisdn": destination.get("mobile_number", ""),
                             "customer_name": destination.get("name", ""),
-                            "account_reference": f'{default_reference}',
+                            "account_reference": payload.get("transfer", {}).get("reference", ""),
                             "narration": payload.get("transfer", {}).get("description", ""),
                             "transaction_type": "CustomerPayBillOnline",
                         }
                     })
 
         data.update(payload.get("additional_properties", {}))
-        # The data updates below are used to track the callbacks to be made
         data.update({
             "bank_id": super().get_bank_id(),
-            "account_number": payload.get("source", {}).get("account_number", payload.get("account_number", "-1")),
             "type": super().get_operation(),
             "bank_sync_call_back": self.bank_sync_call_back.get("payments", ""),
             "reference": default_reference
         })
 
         return data
 
     def response(self):
         return self.standardize_response(response_data=super().response())
 
     def standardize_response(self, response_data):
+
         data = {
             "bank_id": super().get_bank_id(),
             "type": super().get_operation(),
-            "date": date.today().strftime('%Y-%m-%d %H:%M:%S'),
-            "transaction_reference": "",
+            "date":date.today().strftime('%d/%m/%y %H:%M:%S'),
+            "transaction_reference":"",
         }
 
-        if not isinstance(response_data, dict):
-            data["response"] = response_data
+        if not isinstance(response_data,dict):
+            data["response"]=response_data
 
-        try:
+        if super().get_bank_id() == super().COOP:
 
-            if super().get_bank_id() == super().COOP:
+            data["message"] = response_data.get("MessageDescription", "")
+            data["code"] = int(response_data.get("MessageCode", -1111111))
 
-                data["message"] = response_data.get("MessageDescription", "")
-                data["code"] = f'{response_data.get("MessageCode", "-111111")}'
+            if 'MessageDescription' in response_data.keys():
+                if response_data.get("MessageDescription", "") == "Full Success":
+                    data["message"] = "success"
+                else:
+                    data["message"] = response_data.get(
+                        "MessageDescription", "")
 
-                if 'MessageDescription' in response_data.keys():
-                    if response_data.get("MessageDescription", "") == "Full Success":
-                        data["message"] = "success"
-                    else:
-                        data["message"] = response_data.get(
-                            "MessageDescription", "")
-
-                if 'MessageCode' in response_data.keys():
-                    data["code"] = f'{response_data.get("MessageCode", "-111111")}'
-
-                if 'Destinations' in response_data.keys():
-                    if response_data.get("Destinations", [{}]) is not None:
-
-                        data["transaction_id"] = response_data.get(
-                            "Destinations", [{}])[0].get("TransactionID", "")
-
-                if 'MessageDateTime' in response_data.keys():
-                    data["date"] = response_data.get(
-                        "MessageDateTime", date.today().strftime('%Y-%m-%d %H:%M:%S'))
-
-                if 'messageDescription' in response_data.keys():
-                    if response_data.get("messageDescription", "") == "Full Success":
-                        data["message"] = "success"
-                    else:
-                        data["message"] = response_data.get(
-                            "messageDescription", "")
-
-                if 'messageCode' in response_data.keys():
-                    data["code"] = f'{response_data.get("messageCode", "-111111")}'
-
-                if 'destination' in response_data.keys():
-                    if response_data.get("destination", {}) is not None:
-                        data["transaction_id"] = response_data.get(
-                            "destination", {}).get("transactionID", "")
-
-                if 'messageDateTime' in response_data.keys():
-                    data["date"] = response_data.get(
-                        "messageDateTime", date.today().strftime('%Y-%m-%d %H:%M:%S'))
+            if 'MessageCode' in response_data.keys():
+                data["code"] = int(response_data.get("MessageCode", -1111111))
+
+            if 'Destinations' in response_data.keys():
+                if response_data.get("Destinations", [{}]) is not None:
 
-            elif super().get_bank_id() == super().EQUITY:
-                data["message"] = response_data.get("message", "")
-                data["code"] = f'{response_data.get("code", "-111111")}'
-                if 'mobileMoneyInfo' in response_data.keys():
                     data["transaction_id"] = response_data.get(
-                        "mobileMoneyInfo", {}).get("ThirdPartyTranID", "")
+                        "Destinations", [{}])[0].get("TransactionID", "")
+
+            if 'MessageDateTime' in response_data.keys():
+                data["date"] = response_data.get(
+                    "MessageDateTime", date.today().strftime('%d/%m/%y %H:%M:%S'))
+
+            if 'messageDescription' in response_data.keys():
+                if response_data.get("messageDescription", "") == "Full Success":
+                    data["message"] = "success"
                 else:
-                    data["transaction_id"] = response_data.get("data", {}).get("transactionId", response_data.get("transactionId", response_data.get("transactionId ", "")))
-                data["date"] = response_data.get("date", response_data.get(
-                    "response_time", date.today().strftime('%Y-%m-%d %H:%M:%S')))
-            # If bank_id is DTB
-            elif super().get_bank_id() == super().DTB:
-                if super().get_operation() == super().IFT:
-                    data["message"] = response_data.get("message", "")
-                    data["code"] = f'{int(float(response_data.get("content", {}).get("response_code"," -111111")))}'
-                    data["transaction_id"] = response_data.get(
-                        "identifier", {}).get("trace_audit_number", "")
-                    data["transaction_reference"] = response_data.get(
-                        "content", {}).get("transaction_reference", "")
-                    data["date"] = date.today().strftime('%Y-%m-%d %H:%M:%S')
-                    if int(data["code"]):
-                        data["message"] = "Transaction Failed"
-                    else:
-                        data["message"] = "Success"
-                elif super().get_operation() == super().MOBILE_WALLET:
                     data["message"] = response_data.get(
-                        "content", {}).get("response_description", "")
-                    data["code"] = f'{int(float(response_data.get("content", {}).get("response_code", "-111111")))}'
-                    data["transaction_id"] = response_data.get(
-                        "content", {}).get("conversation_id", "")
-                    data["transaction_reference"] = response_data.get(
-                        "content", {}).get("service_reference", "")
-                elif super().get_operation() == super().STK_PUSH:
-                    data["message"] = response_data.get(
-                        "content", {}).get("response_description", "")
-                    data["code"] = f'{int(float(response_data.get("content", {}).get("response_code", "-111111")))}'
+                        "messageDescription", "")
+
+            if 'messageCode' in response_data.keys():
+                data["code"] = int(response_data.get("messageCode", -1111111))
+
+            if 'destination' in response_data.keys():
+                if response_data.get("destination", {}) is not None:
                     data["transaction_id"] = response_data.get(
-                        "content", {}).get("merchant_request_id", "")
-                    data["transaction_reference"] = response_data.get(
-                        "content", {}).get("service_reference", "")
-            # If bank_id is UBA
-            elif super().get_bank_id() == super().UBA:
-                if super().get_operation() == super().IFT:
-                    resp_object = response_data.get("sendTransactionResponse", {}).get(
-                        "return", {}).get("C24TRANRES", {})
-                    data["code"] = f'{int(float(resp_object.get("ACTION_CODE", "-111111")))}'
-                    data["transaction_id"] = resp_object.get("STAN", "")
-                    data["transaction_reference"] = resp_object.get("STAN", "")
-                    data["date"] = datetime.strptime(
-                        f'{resp_object.get("TRAN_DATE_TIME", None)}', '%Y%m%d%H%M%S').strftime('%Y-%m-%d %H:%M:%S')
-                    if int(data["code"]):
-                        data["message"] = "Transaction Failed"
-                    else:
-                        data["message"] = "Success"
+                        "destination", {}).get("transactionID", "")
 
-             # If bank_id is NCBA
-            elif super().get_bank_id() == super().NCBA:
-                data["message"] = f'{response_data.get("Description", response_data.get("Message", ""))} {response_data.get("Reference", "")}'
-                data["code"] = f'{response_data.get("Response Code", response_data.get("Code", "-111111"))}'
-                data["transaction_id"] = response_data.get("Reference", response_data.get("Transaction", {}).get("CBSReference", ""))
-                data["transaction_reference"] = response_data.get("Transaction", {}).get("CustomerReference", "")
-                if 'Date' in response_data.get("Transaction", {}).keys(): 
-                    # NCBA's Transaction Query API Returns the date in the formart: '5/19/2023 1:55:44 PM'
-                    # The above format is not supported in python datetime.strptime
-                    # Where the month and hour have no zero leading.
-                    # We will therefore wrtie logic to convert it to '05/19/2023 01:55:44 PM'
-                    transaction_date=response_data.get("Transaction", {}).get("Date").split(' ')
-                    if len(transaction_date[0].split('/')[0])<2:
-                        transaction_date[0]=f'0{transaction_date[0]}'
-                    
-                    if transaction_date[2].lower()=='pm':
-                        transaction_date[1]=f"{int(transaction_date[1].split(':')[0])+12}:{transaction_date[1].split(':')[1]}:{transaction_date[1].split(':')[2]}"
-
-                    if len(transaction_date[1])<2:
-                        transaction_date[1]=f'0{transaction_date[1]}'
-                    
-                    data["date"] = datetime.strptime(' '.join(transaction_date), '%m/%d/%Y %H:%M:%S %p').strftime('%Y-%m-%d %H:%M:%S')
-
-            if 'error' in response_data.keys(): 
-                data["message"] = response_data.get("error", "")
-
-            if bool(data):
-                # save the data returned to be sent back to a callback
-                self.simulate_callback(response=data)
-                return data
-
-        except Exception as e:
-            data["message"] = str(e)
-            data["bank_sync_error"] = str(e)
-            data["bank_core_response"] = super().response()
+            if 'messageDateTime' in response_data.keys():
+                data["date"] = response_data.get(
+                    "messageDateTime", date.today().strftime('%d/%m/%y %H:%M:%S'))
+
+        elif super().get_bank_id() == super().EQUITY:
+            data["message"] = response_data.get("message", "")
+            data["code"] = response_data.get("code", -1111111)
+            if 'mobileMoneyInfo' in response_data.keys():
+                data["transaction_id"] = response_data.get(
+                    "mobileMoneyInfo", {}).get("ThirdPartyTranID", "")
+            else:
+                data["transaction_id"] = response_data.get(
+                    "data", {}).get("transactionId", response_data.get("transactionId", response_data.get("transactionId ", "")))
+            data["date"] = response_data.get(
+                "date", date.today().strftime('%d/%m/%y %H:%M:%S'))
+        # If bank_id is DTB
+        elif super().get_bank_id() == super().DTB:
+            if super().get_operation() == super().IFT:
+                data["message"] = response_data.get("message", "")
+                data["code"] = int(float(response_data.get(
+                    "content", {}).get("response_code", -1111111)))
+                data["transaction_id"] = response_data.get(
+                    "identifier", {}).get("trace_audit_number", "")
+                data["transaction_reference"] = response_data.get(
+                    "content", {}).get("transaction_reference", "")
+                data["date"] = date.today().strftime('%d/%m/%y %H:%M:%S')
+                if data["code"]:
+                    data["message"] = "Transaction Failed"
+                else:
+                    data["message"] = "Success"
+            elif super().get_operation() == super().MOBILE_WALLET:
+                data["message"] = response_data.get(
+                    "content", {}).get("response_description", "")
+                data["code"] = int(float(response_data.get(
+                    "content", {}).get("response_code", -1111111)))
+                data["transaction_id"] = response_data.get(
+                    "content", {}).get("conversation_id", "")
+                data["transaction_reference"] = response_data.get(
+                    "content", {}).get("service_reference", "")
+            elif super().get_operation() == super().STK_PUSH:
+                data["message"] = response_data.get(
+                    "content", {}).get("response_description", "")
+                data["code"] = int(float(response_data.get(
+                    "content", {}).get("response_code", -1111111)))
+                data["transaction_id"] = response_data.get(
+                    "content", {}).get("merchant_request_id", "")
+                data["transaction_reference"] = response_data.get(
+                    "content", {}).get("service_reference", "")
+        # If bank_id is UBA
+        elif super().get_bank_id() == super().UBA:
+            if super().get_operation() == super().IFT:
+                resp_object = response_data.get("sendTransactionResponse", {}).get(
+                    "return", {}).get("C24TRANRES", {})
+                data["code"] = int(
+                    float(resp_object.get("ACTION_CODE", -1111111)))
+                data["transaction_id"] = resp_object.get("STAN", "")
+                data["transaction_reference"] = resp_object.get("STAN", "")
+                data["date"] = datetime.strptime(
+                    f'{resp_object.get("TRAN_DATE_TIME", None)}', '%Y%m%d%H%M%S').strftime('%d/%m/%y %H:%M:%S')
+                if data["code"]:
+                    data["message"] = "Transaction Failed"
+                else:
+                    data["message"] = "Success"
+
+        if bool(data):
+            # save the data returned to be sent back to a callback
+            self.simulate_callback(response=data)
+            return data
 
         return super().response()
```

### Comparing `nashbanksync-0.1.80/bank_sync/middlewares/logs.py` & `nashbanksync-0.1.9/bank_sync/middlewares/logs.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,24 +45,24 @@
 
             if len(request.body):
                 request_logs.body = literal_eval(request.body.decode("utf-8").replace("false","False").replace("true","True").replace("null","None"))
                 request_logs.save()
                 connections.close_all()
         except Exception as e:
             if request_logs is not None:
-                request_logs.error = str(e)
+                request_logs.error = e
                 request_logs.save()
                 connections.close_all()
 
     def log_response(self, response, ip):  
         response_logs = None      
         try:
             response_logs = ResponseLogs.objects.create(ip=ip,headers=dict(response.headers))
             if len(response.data):
                 response_logs.content = response.data
                 response_logs.save()
                 connections.close_all()
         except Exception as e:
             if response_logs is not None:
-                response_logs.error = str(e)
+                response_logs.error = e
                 response_logs.save()
                 connections.close_all()
```

### Comparing `nashbanksync-0.1.80/bank_sync/migrations/0001_initial.py` & `nashbanksync-0.1.9/bank_sync/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `nashbanksync-0.1.80/bank_sync/migrations/0003_requestlogs.py` & `nashbanksync-0.1.9/bank_sync/migrations/0003_requestlogs.py`

 * *Files identical despite different names*

### Comparing `nashbanksync-0.1.80/bank_sync/migrations/0007_responselogs.py` & `nashbanksync-0.1.9/bank_sync/migrations/0007_responselogs.py`

 * *Files identical despite different names*

### Comparing `nashbanksync-0.1.80/bank_sync/migrations/0010_auto_20221117_1406.py` & `nashbanksync-0.1.9/bank_sync/migrations/0010_auto_20221117_1406.py`

 * *Files identical despite different names*

### Comparing `nashbanksync-0.1.80/bank_sync/migrations/0011_ipndata.py` & `nashbanksync-0.1.9/bank_sync/migrations/0011_ipndata.py`

 * *Files identical despite different names*

### Comparing `nashbanksync-0.1.80/bank_sync/models.py` & `nashbanksync-0.1.9/bank_sync/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 from django.db import models
 from django.utils import timezone
 
 
 class Callbacks(models.Model):
-    tenant_id = models.UUIDField(default=None, null=True, editable=False)
-    business_id = models.UUIDField(default=None, null=True, editable=False)
-    counter_party_type = models.CharField(max_length=500, default=None, null=True, editable=False)
     bank_id = models.IntegerField()
     type_code = models.IntegerField()
     reference = models.CharField(max_length=100, unique=True)
     callback = models.TextField()
     request = models.JSONField(default=dict)
     response = models.JSONField(default=dict)
     request_time = models.DateTimeField(default=timezone.now)
@@ -19,15 +16,15 @@
         verbose_name = "Callback"
         verbose_name_plural = "Callbacks"
 
     def __str__(self):
         return self.reference
 
     def __repr__(self):
-        return f'Callbacks(tenant_id="{self.tenant_id}",business_id="{self.business_id}",reference="{self.reference}",callback="{self.callback}", request={self.request}, response={self.response})'
+        return f'Callbacks(reference="{self.reference}",callback="{self.callback}", request={self.request}, response={self.response})'
 
 
 class RequestLogs(models.Model):
     ip = models.CharField(max_length=50)
     method = models.CharField(max_length=10)
     path = models.CharField(max_length=100)
     content_type = models.CharField(max_length=50)
@@ -66,25 +63,20 @@
         verbose_name = "Response Log"
         verbose_name_plural = "Response Logs"
 
 # This class is used to create/save user I.P.N. callbacks that are to listen on any changes on a specified bank and account number
 
 
 class IPN(models.Model):
-    tenant_id = models.UUIDField(default=None, null=True, editable=False)
-    business_id = models.UUIDField(default=None, null=True, editable=False)
     client_id = models.CharField(max_length=200, unique=True)
     signature = models.CharField(max_length=200, unique=True)
     bank_id = models.IntegerField()
     country_code = models.CharField(max_length=5, default='KE')
-    currency_code = models.CharField(max_length=5, default='KES')
     account_number = models.CharField(max_length=200, unique=True)
     url = models.URLField()
-    # We will use this field to save the url we are to send a reply to if a statement contains the callback that was awaited
-    statement_url = models.URLField()
 
     IPNSTATUS = [
         (True, 'Active'),
         (False, 'Inactive')
     ]
     status = models.BooleanField(choices=IPNSTATUS, default=True)
 
@@ -97,15 +89,15 @@
     ipn_type = models.IntegerField(choices=IPNTYPE,
                                    default=0,)
 
     def __str__(self):
         return f'{self.client_id} : I.P.N. Type - {[i[1] for i in self.IPNTYPE if i[0] == self.ipn_type][0]} : Status - {[i[1] for i in self.IPNSTATUS if i[0] == self.status][0]}'
 
     def __repr__(self):
-        return f'IPN(tenant_id="{self.tenant_id}",business_id="{self.business_id}",client_id="{self.client_id}", bank_id="{self.bank_id}", country_code="{self.country_code}", account_number="{self.account_number}", ipn_type={self.ipn_type}, status={self.status})'
+        return f'IPN(client_id="{self.client_id}", bank_id="{self.bank_id}", country_code="{self.country_code}", account_number="{self.account_number}", ipn_type={self.ipn_type}, status={self.status})'
 
 
 # This class is used to create/save user I.P.N. data sent back
 class IPNData(models.Model):
     ipn = models.ForeignKey(IPN, on_delete=models.CASCADE)
     response = models.JSONField(default=dict)
     response_time = models.DateTimeField(default=timezone.now)
```

### Comparing `nashbanksync-0.1.80/bank_sync/tests.py` & `nashbanksync-0.1.9/bank_sync/tests.py`

 * *Files identical despite different names*

### Comparing `nashbanksync-0.1.80/nashbanksync.egg-info/PKG-INFO` & `nashbanksync-0.1.9/nashbanksync.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,29 @@
 Metadata-Version: 2.1
 Name: nashbanksync
-Version: 0.1.80
+Version: 0.1.9
 Summary: Python library for connecting to the Nash Banks Framework
 Home-page: https://github.com/NashInc/NashSync.git
 Author: Dansol Obondo
 Author-email: dansol@nashafrica.co
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Nasheq Bank Sync Standardized A.P.I.s Python Integrations
+# Nasheq E.R.P. Standardized A.P.I.s python integrations
 
 ## Quick Guide
 Below are the steps on how to get the web app up and running
 
-1.	Install Dependencies:
-```bash
-    pip install requests
-    pip install django-compression-middleware
-    pip install djangorestframework
-```
-2.	Install Nash Sync ERP Library:
+1.	Install it:
 ```bash
     pip install nashbanksync
 ```
-3.	View get started documentation:
+2.	View get started documentation:
 ```bash
     https://nashbanksuite.readme.io/v1.2.0/docs
 ```
-4.	Start Coding
+3.	Start Coding
```

### Comparing `nashbanksync-0.1.80/nashbanksync.egg-info/SOURCES.txt` & `nashbanksync-0.1.9/nashbanksync.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 bank_sync/APIs/utils/__init__.py
 bank_sync/APIs/utils/generate_code.py
 bank_sync/Nash/__init__.py
 bank_sync/Nash/nash.py
 bank_sync/Resources/__init__.py
 bank_sync/Resources/accounts.py
 bank_sync/Resources/banks.py
-bank_sync/Resources/helpers.py
 bank_sync/Resources/operations.py
 bank_sync/Resources/payments.py
 bank_sync/Resources/resource.py
 bank_sync/middlewares/__init__.py
 bank_sync/middlewares/logs.py
 bank_sync/migrations/0001_initial.py
 bank_sync/migrations/0002_alter_callbacks_reference.py
@@ -30,16 +29,12 @@
 bank_sync/migrations/0007_responselogs.py
 bank_sync/migrations/0008_responselogs_ip.py
 bank_sync/migrations/0009_responselogs_error.py
 bank_sync/migrations/0010_auto_20221117_1406.py
 bank_sync/migrations/0011_ipndata.py
 bank_sync/migrations/0012_alter_ipn_account_number.py
 bank_sync/migrations/0013_alter_ipndata_ipn.py
-bank_sync/migrations/0014_auto_20230125_1119.py
-bank_sync/migrations/0015_auto_20230209_1410.py
-bank_sync/migrations/0016_ipn_statement_url.py
-bank_sync/migrations/0017_alter_ipn_statement_url.py
 bank_sync/migrations/__init__.py
 nashbanksync.egg-info/PKG-INFO
 nashbanksync.egg-info/SOURCES.txt
 nashbanksync.egg-info/dependency_links.txt
 nashbanksync.egg-info/top_level.txt
```

### Comparing `nashbanksync-0.1.80/setup.py` & `nashbanksync-0.1.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nashbanksync",
-    version="0.1.80",
+    version="0.1.9",
     author="Dansol Obondo",
     author_email="dansol@nashafrica.co",
     description='Python library for connecting to the Nash Banks Framework',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/NashInc/NashSync.git",
     packages=setuptools.find_packages(),
```

