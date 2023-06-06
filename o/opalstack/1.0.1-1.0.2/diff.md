# Comparing `tmp/opalstack-1.0.1.tar.gz` & `tmp/opalstack-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/ryan/src/opalstack-python/dist/tmpphnuk2x7/opalstack-1.0.1.tar", last modified: Thu Oct 13 18:31:59 2022, max compression
+gzip compressed data, was "opalstack-1.0.2.tar", last modified: Tue Jun  6 21:57:12 2023, max compression
```

## Comparing `opalstack-1.0.1.tar` & `opalstack-1.0.2.tar`

### file list

```diff
@@ -1,37 +1,61 @@
-drwxrwxr-x   0 ryan      (1014) ryan      (1015)        0 2022-10-13 18:31:59.000000 opalstack-1.0.1/
--rw-rw-r--   0 ryan      (1014) ryan      (1015)      668 2022-10-13 18:31:59.000000 opalstack-1.0.1/setup.cfg
-drwxrwxr-x   0 ryan      (1014) ryan      (1015)        0 2022-10-13 18:31:59.000000 opalstack-1.0.1/src/
-drwxrwxr-x   0 ryan      (1014) ryan      (1015)        0 2022-10-13 18:31:59.000000 opalstack-1.0.1/src/opalstack.egg-info/
--rw-rw-r--   0 ryan      (1014) ryan      (1015)        1 2022-10-13 18:31:59.000000 opalstack-1.0.1/src/opalstack.egg-info/dependency_links.txt
--rw-rw-r--   0 ryan      (1014) ryan      (1015)       10 2022-10-13 18:31:59.000000 opalstack-1.0.1/src/opalstack.egg-info/top_level.txt
--rw-rw-r--   0 ryan      (1014) ryan      (1015)        9 2022-10-13 18:31:59.000000 opalstack-1.0.1/src/opalstack.egg-info/requires.txt
--rw-rw-r--   0 ryan      (1014) ryan      (1015)      805 2022-10-13 18:31:59.000000 opalstack-1.0.1/src/opalstack.egg-info/SOURCES.txt
--rw-rw-r--   0 ryan      (1014) ryan      (1015)    11359 2022-10-13 18:31:59.000000 opalstack-1.0.1/src/opalstack.egg-info/PKG-INFO
-drwxrwxr-x   0 ryan      (1014) ryan      (1015)        0 2022-10-13 18:31:59.000000 opalstack-1.0.1/src/opalstack/
--rw-rw-r--   0 ryan      (1014) ryan      (1015)      667 2022-10-10 04:50:38.000000 opalstack-1.0.1/src/opalstack/servers.py
--rw-rw-r--   0 ryan      (1014) ryan      (1015)     1255 2022-10-10 04:50:38.000000 opalstack-1.0.1/src/opalstack/psqldbs.py
--rw-rw-r--   0 ryan      (1014) ryan      (1015)     1246 2022-10-10 04:50:38.000000 opalstack-1.0.1/src/opalstack/tokens.py
--rw-rw-r--   0 ryan      (1014) ryan      (1015)      695 2022-10-10 04:50:38.000000 opalstack-1.0.1/src/opalstack/quarantinedmails.py
--rw-rw-r--   0 ryan      (1014) ryan      (1015)    17698 2022-10-10 04:50:38.000000 opalstack-1.0.1/src/opalstack/util.py
--rw-rw-r--   0 ryan      (1014) ryan      (1015)       62 2022-10-13 18:26:58.000000 opalstack-1.0.1/src/opalstack/__init__.py
--rw-rw-r--   0 ryan      (1014) ryan      (1015)     1271 2022-10-10 04:50:38.000000 opalstack-1.0.1/src/opalstack/mailusers.py
--rw-rw-r--   0 ryan      (1014) ryan      (1015)      655 2022-10-10 04:50:38.000000 opalstack-1.0.1/src/opalstack/ips.py
--rw-rw-r--   0 ryan      (1014) ryan      (1015)     7424 2022-10-10 04:50:38.000000 opalstack-1.0.1/src/opalstack/api.py
--rw-rw-r--   0 ryan      (1014) ryan      (1015)     1348 2022-10-10 04:50:38.000000 opalstack-1.0.1/src/opalstack/certs.py
--rw-rw-r--   0 ryan      (1014) ryan      (1015)     1249 2022-10-10 04:50:38.000000 opalstack-1.0.1/src/opalstack/sites.py
--rw-rw-r--   0 ryan      (1014) ryan      (1015)     1256 2022-10-10 04:50:38.000000 opalstack-1.0.1/src/opalstack/notices.py
--rw-rw-r--   0 ryan      (1014) ryan      (1015)     1261 2022-10-10 04:50:38.000000 opalstack-1.0.1/src/opalstack/psqlusers.py
--rw-rw-r--   0 ryan      (1014) ryan      (1015)     1264 2022-10-10 04:50:38.000000 opalstack-1.0.1/src/opalstack/mariausers.py
--rw-rw-r--   0 ryan      (1014) ryan      (1015)     1408 2022-10-10 04:50:38.000000 opalstack-1.0.1/src/opalstack/dnsrecords.py
--rw-rw-r--   0 ryan      (1014) ryan      (1015)     1368 2022-10-10 04:50:38.000000 opalstack-1.0.1/src/opalstack/osvars.py
--rw-rw-r--   0 ryan      (1014) ryan      (1015)     1246 2022-10-10 04:50:38.000000 opalstack-1.0.1/src/opalstack/apps.py
--rw-rw-r--   0 ryan      (1014) ryan      (1015)     8689 2022-10-10 04:50:38.000000 opalstack-1.0.1/src/opalstack/manager.py
--rw-rw-r--   0 ryan      (1014) ryan      (1015)     1038 2022-10-10 04:50:38.000000 opalstack-1.0.1/src/opalstack/domains.py
--rw-rw-r--   0 ryan      (1014) ryan      (1015)     1399 2022-10-10 04:50:38.000000 opalstack-1.0.1/src/opalstack/addresses.py
--rw-rw-r--   0 ryan      (1014) ryan      (1015)     1255 2022-10-10 04:50:38.000000 opalstack-1.0.1/src/opalstack/osusers.py
--rw-rw-r--   0 ryan      (1014) ryan      (1015)      843 2022-10-10 04:50:38.000000 opalstack-1.0.1/src/opalstack/accounts.py
--rw-rw-r--   0 ryan      (1014) ryan      (1015)     1258 2022-10-10 04:50:38.000000 opalstack-1.0.1/src/opalstack/mariadbs.py
--rw-rw-r--   0 ryan      (1014) ryan      (1015)    11359 2022-10-13 18:31:59.000000 opalstack-1.0.1/PKG-INFO
--rw-rw-r--   0 ryan      (1014) ryan      (1015)      104 2022-10-10 04:50:38.000000 opalstack-1.0.1/pyproject.toml
--rw-rw-r--   0 ryan      (1014) ryan      (1015)     1066 2022-10-10 04:50:38.000000 opalstack-1.0.1/LICENSE
--rw-rw-r--   0 ryan      (1014) ryan      (1015)    10809 2022-10-10 04:50:38.000000 opalstack-1.0.1/README.md
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-06-06 21:57:12.438273 opalstack-1.0.2/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1066 2023-06-06 20:03:46.000000 opalstack-1.0.2/LICENSE
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)    11322 2023-06-06 21:57:12.438273 opalstack-1.0.2/PKG-INFO
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)    10809 2023-06-06 20:03:46.000000 opalstack-1.0.2/README.md
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      104 2023-06-06 20:03:46.000000 opalstack-1.0.2/pyproject.toml
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      668 2023-06-06 21:57:12.438273 opalstack-1.0.2/setup.cfg
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-06-06 21:57:12.438273 opalstack-1.0.2/src/
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-06-06 21:57:12.438273 opalstack-1.0.2/src/opalstack/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)       62 2023-06-06 20:26:22.000000 opalstack-1.0.2/src/opalstack/__init__.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      843 2023-06-06 20:03:46.000000 opalstack-1.0.2/src/opalstack/accounts.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1399 2023-06-06 20:03:46.000000 opalstack-1.0.2/src/opalstack/addresses.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     7496 2023-06-06 20:24:30.000000 opalstack-1.0.2/src/opalstack/api.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1246 2023-06-06 20:03:46.000000 opalstack-1.0.2/src/opalstack/apps.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1348 2023-06-06 20:03:46.000000 opalstack-1.0.2/src/opalstack/certs.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1408 2023-06-06 20:03:46.000000 opalstack-1.0.2/src/opalstack/dnsrecords.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1038 2023-06-06 20:03:46.000000 opalstack-1.0.2/src/opalstack/domains.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      655 2023-06-06 20:03:46.000000 opalstack-1.0.2/src/opalstack/ips.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1271 2023-06-06 20:03:46.000000 opalstack-1.0.2/src/opalstack/mailusers.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     8689 2023-06-06 20:03:46.000000 opalstack-1.0.2/src/opalstack/manager.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1258 2023-06-06 20:03:46.000000 opalstack-1.0.2/src/opalstack/mariadbs.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1264 2023-06-06 20:03:46.000000 opalstack-1.0.2/src/opalstack/mariausers.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1256 2023-06-06 20:03:46.000000 opalstack-1.0.2/src/opalstack/notices.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1255 2023-06-06 20:03:46.000000 opalstack-1.0.2/src/opalstack/osusers.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1368 2023-06-06 20:03:46.000000 opalstack-1.0.2/src/opalstack/osvars.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1255 2023-06-06 20:03:46.000000 opalstack-1.0.2/src/opalstack/psqldbs.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1261 2023-06-06 20:03:46.000000 opalstack-1.0.2/src/opalstack/psqlusers.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      695 2023-06-06 20:03:46.000000 opalstack-1.0.2/src/opalstack/quarantinedmails.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      667 2023-06-06 20:03:46.000000 opalstack-1.0.2/src/opalstack/servers.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1249 2023-06-06 20:03:46.000000 opalstack-1.0.2/src/opalstack/sites.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1246 2023-06-06 20:03:46.000000 opalstack-1.0.2/src/opalstack/tokens.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      908 2023-06-06 20:23:55.000000 opalstack-1.0.2/src/opalstack/usage.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)    17698 2023-06-06 20:03:46.000000 opalstack-1.0.2/src/opalstack/util.py
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-06-06 21:57:12.438273 opalstack-1.0.2/src/opalstack.egg-info/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)    11322 2023-06-06 21:57:12.000000 opalstack-1.0.2/src/opalstack.egg-info/PKG-INFO
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1308 2023-06-06 21:57:12.000000 opalstack-1.0.2/src/opalstack.egg-info/SOURCES.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)        1 2023-06-06 21:57:12.000000 opalstack-1.0.2/src/opalstack.egg-info/dependency_links.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)        9 2023-06-06 21:57:12.000000 opalstack-1.0.2/src/opalstack.egg-info/requires.txt
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)       10 2023-06-06 21:57:12.000000 opalstack-1.0.2/src/opalstack.egg-info/top_level.txt
+drwxrwxr-x   0 ryan      (1000) ryan      (1000)        0 2023-06-06 21:57:12.438273 opalstack-1.0.2/tests/
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1859 2023-06-06 20:03:46.000000 opalstack-1.0.2/tests/test_accounts.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     4274 2023-06-06 20:03:46.000000 opalstack-1.0.2/tests/test_addresses.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     2911 2023-06-06 20:03:46.000000 opalstack-1.0.2/tests/test_apps.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     9302 2023-06-06 20:03:46.000000 opalstack-1.0.2/tests/test_certs.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     3813 2023-06-06 20:03:46.000000 opalstack-1.0.2/tests/test_dnsrecords.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1381 2023-06-06 20:03:46.000000 opalstack-1.0.2/tests/test_domains.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1207 2023-06-06 20:03:46.000000 opalstack-1.0.2/tests/test_ips.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     2972 2023-06-06 20:03:46.000000 opalstack-1.0.2/tests/test_mailusers.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     3838 2023-06-06 20:03:46.000000 opalstack-1.0.2/tests/test_mariadbs.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     2973 2023-06-06 20:03:46.000000 opalstack-1.0.2/tests/test_mariatool.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     3076 2023-06-06 20:03:46.000000 opalstack-1.0.2/tests/test_mariausers.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     2374 2023-06-06 20:03:46.000000 opalstack-1.0.2/tests/test_notices.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     2769 2023-06-06 20:03:46.000000 opalstack-1.0.2/tests/test_osusers.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     3407 2023-06-06 20:03:46.000000 opalstack-1.0.2/tests/test_osvars.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     3708 2023-06-06 20:03:46.000000 opalstack-1.0.2/tests/test_psqldbs.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     2970 2023-06-06 20:03:46.000000 opalstack-1.0.2/tests/test_psqltool.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     2994 2023-06-06 20:03:46.000000 opalstack-1.0.2/tests/test_psqlusers.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1175 2023-06-06 20:03:46.000000 opalstack-1.0.2/tests/test_servers.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     4129 2023-06-06 20:03:46.000000 opalstack-1.0.2/tests/test_sites.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     2976 2023-06-06 20:03:46.000000 opalstack-1.0.2/tests/test_ssh.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)     1995 2023-06-06 20:03:46.000000 opalstack-1.0.2/tests/test_tokens.py
+-rw-rw-r--   0 ryan      (1000) ryan      (1000)      721 2023-06-06 20:03:46.000000 opalstack-1.0.2/tests/testutil.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `opalstack-1.0.1/setup.cfg` & `opalstack-1.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = opalstack
-version = 1.0.1
+version = 1.0.2
 author = Opalstack
 author_email = support@opalstack.com
 description = Opalstack API Python Library
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/opalstack/opalstack-python
 project_urls =
```

### Comparing `opalstack-1.0.1/src/opalstack.egg-info/PKG-INFO` & `opalstack-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: opalstack
-Version: 1.0.1
+Version: 1.0.2
 Summary: Opalstack API Python Library
 Home-page: https://github.com/opalstack/opalstack-python
 Author: Opalstack
 Author-email: support@opalstack.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/opalstack/opalstack-python/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -315,9 +313,7 @@
 # Delete the created site, app, osuser, and domain
 #
 opalapi.sites.delete([created_site])
 opalapi.apps.delete([created_app])
 opalapi.osusers.delete([created_osuser])
 opalapi.domains.delete([created_domain])
 ```
-
-
```

### Comparing `opalstack-1.0.1/src/opalstack/servers.py` & `opalstack-1.0.2/src/opalstack/servers.py`

 * *Files identical despite different names*

### Comparing `opalstack-1.0.1/src/opalstack/psqldbs.py` & `opalstack-1.0.2/src/opalstack/psqldbs.py`

 * *Files identical despite different names*

### Comparing `opalstack-1.0.1/src/opalstack/tokens.py` & `opalstack-1.0.2/src/opalstack/tokens.py`

 * *Files identical despite different names*

### Comparing `opalstack-1.0.1/src/opalstack/quarantinedmails.py` & `opalstack-1.0.2/src/opalstack/quarantinedmails.py`

 * *Files identical despite different names*

### Comparing `opalstack-1.0.1/src/opalstack/util.py` & `opalstack-1.0.2/src/opalstack/util.py`

 * *Files identical despite different names*

### Comparing `opalstack-1.0.1/src/opalstack/mailusers.py` & `opalstack-1.0.2/src/opalstack/mailusers.py`

 * *Files identical despite different names*

### Comparing `opalstack-1.0.1/src/opalstack/ips.py` & `opalstack-1.0.2/src/opalstack/ips.py`

 * *Files identical despite different names*

### Comparing `opalstack-1.0.1/src/opalstack/api.py` & `opalstack-1.0.2/src/opalstack/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from .psqldbs import PsqldbsManager
 from .psqlusers import PsqlusersManager
 from .certs import CertsManager
 from .sites import SitesManager
 from .addresses import AddressesManager
 from .mailusers import MailusersManager
 from .quarantinedmails import QuarantinedmailsManager
+from .usage import UsageManager
 
 API_URL = 'https://my.opalstack.com/api/v1'
 
 log = logging.getLogger(__name__)
 
 class Api():
     def __init__(self, token):
@@ -52,14 +53,15 @@
         self.psqldbs = PsqldbsManager(self)
         self.mariausers = MariausersManager(self)
         self.mariadbs = MariadbsManager(self)
         self.certs = CertsManager(self)
         self.sites = SitesManager(self)
         self.mailusers= MailusersManager(self)
         self.addresses = AddressesManager(self)
+        self.usage = UsageManager(self)
 
         ## Not live yet ##
         # self.quarantinedmails = QuarantinedmailsManager(self)
 
     def request(self, urlpath, method, dataObj, ensure_status=[200]):
         if method not in ('GET', 'POST'): raise ValueError(f'Invalid request method {method}')
         if method == 'GET':
```

### Comparing `opalstack-1.0.1/src/opalstack/certs.py` & `opalstack-1.0.2/src/opalstack/certs.py`

 * *Files identical despite different names*

### Comparing `opalstack-1.0.1/src/opalstack/sites.py` & `opalstack-1.0.2/src/opalstack/sites.py`

 * *Files identical despite different names*

### Comparing `opalstack-1.0.1/src/opalstack/notices.py` & `opalstack-1.0.2/src/opalstack/notices.py`

 * *Files identical despite different names*

### Comparing `opalstack-1.0.1/src/opalstack/psqlusers.py` & `opalstack-1.0.2/src/opalstack/psqlusers.py`

 * *Files identical despite different names*

### Comparing `opalstack-1.0.1/src/opalstack/mariausers.py` & `opalstack-1.0.2/src/opalstack/mariausers.py`

 * *Files identical despite different names*

### Comparing `opalstack-1.0.1/src/opalstack/dnsrecords.py` & `opalstack-1.0.2/src/opalstack/dnsrecords.py`

 * *Files identical despite different names*

### Comparing `opalstack-1.0.1/src/opalstack/osvars.py` & `opalstack-1.0.2/src/opalstack/osvars.py`

 * *Files identical despite different names*

### Comparing `opalstack-1.0.1/src/opalstack/apps.py` & `opalstack-1.0.2/src/opalstack/apps.py`

 * *Files identical despite different names*

### Comparing `opalstack-1.0.1/src/opalstack/manager.py` & `opalstack-1.0.2/src/opalstack/manager.py`

 * *Files identical despite different names*

### Comparing `opalstack-1.0.1/src/opalstack/domains.py` & `opalstack-1.0.2/src/opalstack/domains.py`

 * *Files identical despite different names*

### Comparing `opalstack-1.0.1/src/opalstack/addresses.py` & `opalstack-1.0.2/src/opalstack/addresses.py`

 * *Files identical despite different names*

### Comparing `opalstack-1.0.1/src/opalstack/osusers.py` & `opalstack-1.0.2/src/opalstack/osusers.py`

 * *Files identical despite different names*

### Comparing `opalstack-1.0.1/src/opalstack/accounts.py` & `opalstack-1.0.2/src/opalstack/accounts.py`

 * *Files identical despite different names*

### Comparing `opalstack-1.0.1/src/opalstack/mariadbs.py` & `opalstack-1.0.2/src/opalstack/mariadbs.py`

 * *Files identical despite different names*

### Comparing `opalstack-1.0.1/PKG-INFO` & `opalstack-1.0.2/src/opalstack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: opalstack
-Version: 1.0.1
+Version: 1.0.2
 Summary: Opalstack API Python Library
 Home-page: https://github.com/opalstack/opalstack-python
 Author: Opalstack
 Author-email: support@opalstack.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/opalstack/opalstack-python/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -315,9 +313,7 @@
 # Delete the created site, app, osuser, and domain
 #
 opalapi.sites.delete([created_site])
 opalapi.apps.delete([created_app])
 opalapi.osusers.delete([created_osuser])
 opalapi.domains.delete([created_domain])
 ```
-
-
```

### Comparing `opalstack-1.0.1/LICENSE` & `opalstack-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `opalstack-1.0.1/README.md` & `opalstack-1.0.2/README.md`

 * *Files identical despite different names*

