# Comparing `tmp/TDXLib-0.4.3.tar.gz` & `tmp/TDXLib-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TDXLib-0.4.3.tar", last modified: Fri Mar 31 21:58:42 2023, max compression
+gzip compressed data, was "TDXLib-0.5.0.tar", last modified: Tue Jun  6 19:19:28 2023, max compression
```

## Comparing `TDXLib-0.4.3.tar` & `TDXLib-0.5.0.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 21:58:42.588462 TDXLib-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-31 21:58:31.000000 TDXLib-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-31 21:58:31.000000 TDXLib-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-03-31 21:58:42.588462 TDXLib-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-03-31 21:58:31.000000 TDXLib-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 21:58:42.588462 TDXLib-0.4.3/TDXLib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-03-31 21:58:42.000000 TDXLib-0.4.3/TDXLib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-03-31 21:58:42.000000 TDXLib-0.4.3/TDXLib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 21:58:42.000000 TDXLib-0.4.3/TDXLib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-31 21:58:42.000000 TDXLib-0.4.3/TDXLib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-31 21:58:42.000000 TDXLib-0.4.3/TDXLib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-31 21:58:31.000000 TDXLib-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 21:58:42.588462 TDXLib-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-03-31 21:58:31.000000 TDXLib-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 21:58:42.588462 TDXLib-0.4.3/tdxlib/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-03-31 21:58:31.000000 TDXLib-0.4.3/tdxlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-03-31 21:58:31.000000 TDXLib-0.4.3/tdxlib/tdx_api_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    53997 2023-03-31 21:58:31.000000 TDXLib-0.4.3/tdxlib/tdx_asset_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    50477 2023-03-31 21:58:31.000000 TDXLib-0.4.3/tdxlib/tdx_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-03-31 21:58:31.000000 TDXLib-0.4.3/tdxlib/tdx_ticket.py
--rw-r--r--   0 runner    (1001) docker     (123)    45930 2023-03-31 21:58:31.000000 TDXLib-0.4.3/tdxlib/tdx_ticket_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-03-31 21:58:31.000000 TDXLib-0.4.3/tdxlib/tdx_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 21:58:42.588462 TDXLib-0.4.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-03-31 21:58:31.000000 TDXLib-0.4.3/test/test_tdx_ticket_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:19:28.824928 TDXLib-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-06 19:19:17.000000 TDXLib-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-06 19:19:17.000000 TDXLib-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14078 2023-06-06 19:19:28.824928 TDXLib-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13683 2023-06-06 19:19:17.000000 TDXLib-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:19:28.820928 TDXLib-0.5.0/TDXLib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14078 2023-06-06 19:19:28.000000 TDXLib-0.5.0/TDXLib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-06-06 19:19:28.000000 TDXLib-0.5.0/TDXLib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 19:19:28.000000 TDXLib-0.5.0/TDXLib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-06 19:19:28.000000 TDXLib-0.5.0/TDXLib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-06 19:19:28.000000 TDXLib-0.5.0/TDXLib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-06 19:19:17.000000 TDXLib-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 19:19:28.824928 TDXLib-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-06 19:19:17.000000 TDXLib-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:19:28.820928 TDXLib-0.5.0/tdxlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-06 19:19:17.000000 TDXLib-0.5.0/tdxlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-06 19:19:17.000000 TDXLib-0.5.0/tdxlib/tdx_api_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54083 2023-06-06 19:19:17.000000 TDXLib-0.5.0/tdxlib/tdx_asset_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-06-06 19:19:17.000000 TDXLib-0.5.0/tdxlib/tdx_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-06 19:19:17.000000 TDXLib-0.5.0/tdxlib/tdx_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40351 2023-06-06 19:19:17.000000 TDXLib-0.5.0/tdxlib/tdx_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-06-06 19:19:17.000000 TDXLib-0.5.0/tdxlib/tdx_ticket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46059 2023-06-06 19:19:17.000000 TDXLib-0.5.0/tdxlib/tdx_ticket_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-06 19:19:17.000000 TDXLib-0.5.0/tdxlib/tdx_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 19:19:28.820928 TDXLib-0.5.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-06 19:19:17.000000 TDXLib-0.5.0/test/test_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-06-06 19:19:17.000000 TDXLib-0.5.0/test/test_tdx_ticket_integration.py
```

### Comparing `TDXLib-0.4.3/LICENSE` & `TDXLib-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `TDXLib-0.4.3/PKG-INFO` & `TDXLib-0.5.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: TDXLib
-Version: 0.4.3
-Summary: a python library for interacting with the TeamDynamix Web API
-Home-page: https://github.com/cedarville-university/tdxlib
-Author: Nat Biggs, Stephen Gaines, Josiah Lansford
-Author-email: tdxlib@cedarville.edu
-License: GNU General Public License v3.0
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![Upload Python Package](https://github.com/cedarville-university/tdxlib/workflows/Upload%20Python%20Package/badge.svg)
 # TDXLib (TeamDynamix Python SDK)
 
 TDXLib is a suite of Python libraries originally designed to take input from Google Sheets and create tickets in [TeamDynamix](https://teamdynamix.com) based on the contents of the sheets. The scope of the project has broadened past its humble beginnings, and continues to do so whenever there's a feature we need that it doesn't currently support.
 
 ## Quick Links
 * [ReadTheDocs.io Documentation](https://tdxlib.readthedocs.io) - TDXLib Class & Method descriptions
@@ -121,50 +109,90 @@
         
         Initial settings saved to: tdxlib.ini
        </pre>
 
     The generated file will look something like this:
 
         [TDX API Settings]
-        'orgname': 'myuniversity',
-        'fullhost': 'its.myuniversity.edu',
+        'org_name': 'myuniversity',
+        'full_host': 'its.myuniversity.edu',
         'sandbox': True,
         'username': 'myuser@university.edu',
         'password': 'Prompt',
-        'ticketAppId': '123',
-        'assetAppId': '456',
+        'ticket_app_id': '123',
+        'asset_app_id': '456',
         'caching': True,
         'log_level': 'ERROR'
      
-    * The `orgname` field is whatever subdomain your organization uses to access TeamDynamix. For example, `https://myuniversity.teamdynamix.com`.
+    * The `org_name` field is whatever subdomain your organization uses to access TeamDynamix. For example, `https://myuniversity.teamdynamix.com`.
 
     * The `sandbox` field specifies whether TDXLib should interact with a sandbox version of the TDX Environment, which is written over by production monthly. It is recommended to use the sandbox environment when first getting familiar with the API environment.
 
     * The `username` and `password` fields are the login credentials for an account to be used with the TeamDynamix API. Many API endpoints (such as creating objects in TDX) require elevated permissions beyond the average user. You may need to create a user specifically for use with TDXLib and grant permissions based on what you need to do.
     
     * If the `password` field is set to `'Prompt'`, then whenever a new integration object is made, it will request a password, and dispose of the password after getting an API token: 
     
        <pre>Enter the TDX Password for user myuser@myuniversity.edu (this password will not be stored):   </pre>
 
-    * The `ticketAppId` and `assetAppId` fields are the numbers that appear after `Apps` in your TeamDynamix URL, and are specific to your organization. You can find these ID's in the URLs in the following locations when using a TDX Tickets or Assets app through TDNext in your browser: 
+    * The `ticket_app_id` and `asset_app_id` fields are the numbers that appear after `Apps` in your TeamDynamix URL, and are specific to your organization. You can find these ID's in the URLs in the following locations when using a TDX Tickets or Assets app through TDNext in your browser: 
     
       * Tickets: `https://myuniversity.teamdynamix.com/TDNext/Apps/{ticketAppId}/Tickets/...`  
       * Assets: `https://myuniversity.teamdynamix.com/TDNext/Apps/{assetAppId}/Assets/...`
 
     * The `caching` field specifies whether or not TDXLib should cache TeamDynamix objects such as valid ticket types, statuses and priorities. Setting this option to `True` reduces the volume of API calls and allows TDXLib to perform some batch operations much faster.
+    
+    * The `log_level` field specifies the python logging level that TDXLib will log at.
 
-    * You can optionally specify an alternative configuration file that TDXLib should search for in your working directory. By default, it will look for `tdxlib.ini`.
+    * The `timezone` field specifies the timezone you'd like TDXLib to operate in. TDXLib will translate date/time objects from TeamDyanmix in UTC to this timezone.
+    
+  * You can optionally specify an alternative configuration file that TDXLib should search for in your working directory. By default, it will look for `tdxlib.ini`.
 
           >>> tdx = tdx_ticket_integration.TDXTicketIntegration("specialconfig.ini")
 
-    * Depending on your `tdxlib.ini` settings, you may be prompted for a password to authenticate into the TeamDynamix API. Once everything is working, go ahead and test out a method:
+  * Depending on your `tdxlib.ini` settings, you may be prompted for a password to authenticate into the TeamDynamix API. Once everything is working, go ahead and test out a method:
 
           >>> accounts = tdx.get_all_accounts()
 
-9. Congratulations! You now have the power of the TeamDynamix API at your fingertips. For more detailed tutorials on how to use TDXLib to manipulate Tickets and Asset, as well as for information on the methods and classes included with TDXLib, check out our documentation on [ReadtheDocs.io](http://tdxlib.readthedocs.io).
+8. TDXLib can also be configured directly by a python dictionary. 
+
+    Settings passed in as a dictionary are overwritten by any values in a filename (and if no file name is passed, the default configuration file, `tdxlib.ini` in the working directory)
+   
+    Use the following format for the dictionary configuration:
+    <pre>
+    config = {
+         "org_name": "exampleorg",
+         "sandbox": true,
+         "auth_type": "password",
+         "username": "someone@example.edu",
+         "password": "a password",
+         "ticket_app_id": 300,
+         "asset_app_id": "",
+         "caching": true,
+         "timezone": "-0500",
+         "log_level": "ERROR"
+     }
+    </pre>
+    The only required settings in this are `org_name` and either `asset_app_id` or `ticket_app_id` if you're creating `TDXAssetIntegration` or `TDXTicketIntegration` objects. If you set `auth_type` to `password` a username is also required.
+    Unset settings will be defaulted per the values in `tdxlib.tdx_constants.default_config`.
+9. TDXLib can also be configured via Environment variables. Any values passed in via dictionary, from a file, or in the default configuration file (`tdxlib.ini` in the working directory) override any values passed in as environment variables. 
+
+    Here's a sample of environment variables you can use (they are the same as the config values for dictionary config, but uppercase and prefixed with `TDXLIB_`): 
+    <pre>
+        export TDXLIB_ORG_NAME=exampleorg
+        export TDXLIB_SANDBOX=true
+        export TDXLIB_AUTH_TYPE=password
+        export TDXLIB_USERNAME=someon@example.edu
+        export TDXLIB_PASSWORD=mypassword
+        export TDXLIB_TICKET_APP_ID=300
+        export TDXLIB_ASSET_APP_ID=400
+        export TDXLIB_CACHING=true
+        export TDXLIB_TIMEZONE=-0500
+        export TDXLIB_LOG_LEVEL=ERROR
+   </pre>
+10. Congratulations! You now have the power of the TeamDynamix API at your fingertips. For more detailed tutorials on how to use TDXLib to manipulate Tickets and Asset, as well as for information on the methods and classes included with TDXLib, check out our documentation on [ReadtheDocs.io](http://tdxlib.readthedocs.io).
     
 
 ##  TDXLib Implementation status and Future Plans
 
 * ### TDXIntegration:
 
     This base class that contains the methods necessary to authenticate to Teamdynamix. This class also contains methods to interact with TeamDyanamix objects that are universal across various Apps (Locations, People, Accounts, etc.)
@@ -260,8 +288,8 @@
         * Creating
         * Editing
     * **Product Models**
         * Editing
     * **Vendors**
         * Editing
         * Deleting
-    * **Accepting Suggestions...** (Submit an Issue!)
+    * **Accepting Suggestions...** (Submit an Issue!)
```

### Comparing `TDXLib-0.4.3/README.md` & `TDXLib-0.5.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: TDXLib
+Version: 0.5.0
+Summary: a python library for interacting with the TeamDynamix Web API
+Home-page: https://github.com/cedarville-university/tdxlib
+Author: Nat Biggs, Stephen Gaines, Josiah Lansford
+Author-email: tdxlib@cedarville.edu
+License: GNU General Public License v3.0
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![Upload Python Package](https://github.com/cedarville-university/tdxlib/workflows/Upload%20Python%20Package/badge.svg)
 # TDXLib (TeamDynamix Python SDK)
 
 TDXLib is a suite of Python libraries originally designed to take input from Google Sheets and create tickets in [TeamDynamix](https://teamdynamix.com) based on the contents of the sheets. The scope of the project has broadened past its humble beginnings, and continues to do so whenever there's a feature we need that it doesn't currently support.
 
 ## Quick Links
 * [ReadTheDocs.io Documentation](https://tdxlib.readthedocs.io) - TDXLib Class & Method descriptions
@@ -109,50 +121,90 @@
         
         Initial settings saved to: tdxlib.ini
        </pre>
 
     The generated file will look something like this:
 
         [TDX API Settings]
-        'orgname': 'myuniversity',
-        'fullhost': 'its.myuniversity.edu',
+        'org_name': 'myuniversity',
+        'full_host': 'its.myuniversity.edu',
         'sandbox': True,
         'username': 'myuser@university.edu',
         'password': 'Prompt',
-        'ticketAppId': '123',
-        'assetAppId': '456',
+        'ticket_app_id': '123',
+        'asset_app_id': '456',
         'caching': True,
         'log_level': 'ERROR'
      
-    * The `orgname` field is whatever subdomain your organization uses to access TeamDynamix. For example, `https://myuniversity.teamdynamix.com`.
+    * The `org_name` field is whatever subdomain your organization uses to access TeamDynamix. For example, `https://myuniversity.teamdynamix.com`.
 
     * The `sandbox` field specifies whether TDXLib should interact with a sandbox version of the TDX Environment, which is written over by production monthly. It is recommended to use the sandbox environment when first getting familiar with the API environment.
 
     * The `username` and `password` fields are the login credentials for an account to be used with the TeamDynamix API. Many API endpoints (such as creating objects in TDX) require elevated permissions beyond the average user. You may need to create a user specifically for use with TDXLib and grant permissions based on what you need to do.
     
     * If the `password` field is set to `'Prompt'`, then whenever a new integration object is made, it will request a password, and dispose of the password after getting an API token: 
     
        <pre>Enter the TDX Password for user myuser@myuniversity.edu (this password will not be stored):   </pre>
 
-    * The `ticketAppId` and `assetAppId` fields are the numbers that appear after `Apps` in your TeamDynamix URL, and are specific to your organization. You can find these ID's in the URLs in the following locations when using a TDX Tickets or Assets app through TDNext in your browser: 
+    * The `ticket_app_id` and `asset_app_id` fields are the numbers that appear after `Apps` in your TeamDynamix URL, and are specific to your organization. You can find these ID's in the URLs in the following locations when using a TDX Tickets or Assets app through TDNext in your browser: 
     
       * Tickets: `https://myuniversity.teamdynamix.com/TDNext/Apps/{ticketAppId}/Tickets/...`  
       * Assets: `https://myuniversity.teamdynamix.com/TDNext/Apps/{assetAppId}/Assets/...`
 
     * The `caching` field specifies whether or not TDXLib should cache TeamDynamix objects such as valid ticket types, statuses and priorities. Setting this option to `True` reduces the volume of API calls and allows TDXLib to perform some batch operations much faster.
+    
+    * The `log_level` field specifies the python logging level that TDXLib will log at.
 
-    * You can optionally specify an alternative configuration file that TDXLib should search for in your working directory. By default, it will look for `tdxlib.ini`.
+    * The `timezone` field specifies the timezone you'd like TDXLib to operate in. TDXLib will translate date/time objects from TeamDyanmix in UTC to this timezone.
+    
+  * You can optionally specify an alternative configuration file that TDXLib should search for in your working directory. By default, it will look for `tdxlib.ini`.
 
           >>> tdx = tdx_ticket_integration.TDXTicketIntegration("specialconfig.ini")
 
-    * Depending on your `tdxlib.ini` settings, you may be prompted for a password to authenticate into the TeamDynamix API. Once everything is working, go ahead and test out a method:
+  * Depending on your `tdxlib.ini` settings, you may be prompted for a password to authenticate into the TeamDynamix API. Once everything is working, go ahead and test out a method:
 
           >>> accounts = tdx.get_all_accounts()
 
-9. Congratulations! You now have the power of the TeamDynamix API at your fingertips. For more detailed tutorials on how to use TDXLib to manipulate Tickets and Asset, as well as for information on the methods and classes included with TDXLib, check out our documentation on [ReadtheDocs.io](http://tdxlib.readthedocs.io).
+8. TDXLib can also be configured directly by a python dictionary. 
+
+    Settings passed in as a dictionary are overwritten by any values in a filename (and if no file name is passed, the default configuration file, `tdxlib.ini` in the working directory)
+   
+    Use the following format for the dictionary configuration:
+    <pre>
+    config = {
+         "org_name": "exampleorg",
+         "sandbox": true,
+         "auth_type": "password",
+         "username": "someone@example.edu",
+         "password": "a password",
+         "ticket_app_id": 300,
+         "asset_app_id": "",
+         "caching": true,
+         "timezone": "-0500",
+         "log_level": "ERROR"
+     }
+    </pre>
+    The only required settings in this are `org_name` and either `asset_app_id` or `ticket_app_id` if you're creating `TDXAssetIntegration` or `TDXTicketIntegration` objects. If you set `auth_type` to `password` a username is also required.
+    Unset settings will be defaulted per the values in `tdxlib.tdx_constants.default_config`.
+9. TDXLib can also be configured via Environment variables. Any values passed in via dictionary, from a file, or in the default configuration file (`tdxlib.ini` in the working directory) override any values passed in as environment variables. 
+
+    Here's a sample of environment variables you can use (they are the same as the config values for dictionary config, but uppercase and prefixed with `TDXLIB_`): 
+    <pre>
+        export TDXLIB_ORG_NAME=exampleorg
+        export TDXLIB_SANDBOX=true
+        export TDXLIB_AUTH_TYPE=password
+        export TDXLIB_USERNAME=someon@example.edu
+        export TDXLIB_PASSWORD=mypassword
+        export TDXLIB_TICKET_APP_ID=300
+        export TDXLIB_ASSET_APP_ID=400
+        export TDXLIB_CACHING=true
+        export TDXLIB_TIMEZONE=-0500
+        export TDXLIB_LOG_LEVEL=ERROR
+   </pre>
+10. Congratulations! You now have the power of the TeamDynamix API at your fingertips. For more detailed tutorials on how to use TDXLib to manipulate Tickets and Asset, as well as for information on the methods and classes included with TDXLib, check out our documentation on [ReadtheDocs.io](http://tdxlib.readthedocs.io).
     
 
 ##  TDXLib Implementation status and Future Plans
 
 * ### TDXIntegration:
 
     This base class that contains the methods necessary to authenticate to Teamdynamix. This class also contains methods to interact with TeamDyanamix objects that are universal across various Apps (Locations, People, Accounts, etc.)
@@ -248,8 +300,8 @@
         * Creating
         * Editing
     * **Product Models**
         * Editing
     * **Vendors**
         * Editing
         * Deleting
-    * **Accepting Suggestions...** (Submit an Issue!)
+    * **Accepting Suggestions...** (Submit an Issue!)
```

### Comparing `TDXLib-0.4.3/TDXLib.egg-info/PKG-INFO` & `TDXLib-0.5.0/TDXLib.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TDXLib
-Version: 0.4.3
+Version: 0.5.0
 Summary: a python library for interacting with the TeamDynamix Web API
 Home-page: https://github.com/cedarville-university/tdxlib
 Author: Nat Biggs, Stephen Gaines, Josiah Lansford
 Author-email: tdxlib@cedarville.edu
 License: GNU General Public License v3.0
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -121,50 +121,90 @@
         
         Initial settings saved to: tdxlib.ini
        </pre>
 
     The generated file will look something like this:
 
         [TDX API Settings]
-        'orgname': 'myuniversity',
-        'fullhost': 'its.myuniversity.edu',
+        'org_name': 'myuniversity',
+        'full_host': 'its.myuniversity.edu',
         'sandbox': True,
         'username': 'myuser@university.edu',
         'password': 'Prompt',
-        'ticketAppId': '123',
-        'assetAppId': '456',
+        'ticket_app_id': '123',
+        'asset_app_id': '456',
         'caching': True,
         'log_level': 'ERROR'
      
-    * The `orgname` field is whatever subdomain your organization uses to access TeamDynamix. For example, `https://myuniversity.teamdynamix.com`.
+    * The `org_name` field is whatever subdomain your organization uses to access TeamDynamix. For example, `https://myuniversity.teamdynamix.com`.
 
     * The `sandbox` field specifies whether TDXLib should interact with a sandbox version of the TDX Environment, which is written over by production monthly. It is recommended to use the sandbox environment when first getting familiar with the API environment.
 
     * The `username` and `password` fields are the login credentials for an account to be used with the TeamDynamix API. Many API endpoints (such as creating objects in TDX) require elevated permissions beyond the average user. You may need to create a user specifically for use with TDXLib and grant permissions based on what you need to do.
     
     * If the `password` field is set to `'Prompt'`, then whenever a new integration object is made, it will request a password, and dispose of the password after getting an API token: 
     
        <pre>Enter the TDX Password for user myuser@myuniversity.edu (this password will not be stored):   </pre>
 
-    * The `ticketAppId` and `assetAppId` fields are the numbers that appear after `Apps` in your TeamDynamix URL, and are specific to your organization. You can find these ID's in the URLs in the following locations when using a TDX Tickets or Assets app through TDNext in your browser: 
+    * The `ticket_app_id` and `asset_app_id` fields are the numbers that appear after `Apps` in your TeamDynamix URL, and are specific to your organization. You can find these ID's in the URLs in the following locations when using a TDX Tickets or Assets app through TDNext in your browser: 
     
       * Tickets: `https://myuniversity.teamdynamix.com/TDNext/Apps/{ticketAppId}/Tickets/...`  
       * Assets: `https://myuniversity.teamdynamix.com/TDNext/Apps/{assetAppId}/Assets/...`
 
     * The `caching` field specifies whether or not TDXLib should cache TeamDynamix objects such as valid ticket types, statuses and priorities. Setting this option to `True` reduces the volume of API calls and allows TDXLib to perform some batch operations much faster.
+    
+    * The `log_level` field specifies the python logging level that TDXLib will log at.
 
-    * You can optionally specify an alternative configuration file that TDXLib should search for in your working directory. By default, it will look for `tdxlib.ini`.
+    * The `timezone` field specifies the timezone you'd like TDXLib to operate in. TDXLib will translate date/time objects from TeamDyanmix in UTC to this timezone.
+    
+  * You can optionally specify an alternative configuration file that TDXLib should search for in your working directory. By default, it will look for `tdxlib.ini`.
 
           >>> tdx = tdx_ticket_integration.TDXTicketIntegration("specialconfig.ini")
 
-    * Depending on your `tdxlib.ini` settings, you may be prompted for a password to authenticate into the TeamDynamix API. Once everything is working, go ahead and test out a method:
+  * Depending on your `tdxlib.ini` settings, you may be prompted for a password to authenticate into the TeamDynamix API. Once everything is working, go ahead and test out a method:
 
           >>> accounts = tdx.get_all_accounts()
 
-9. Congratulations! You now have the power of the TeamDynamix API at your fingertips. For more detailed tutorials on how to use TDXLib to manipulate Tickets and Asset, as well as for information on the methods and classes included with TDXLib, check out our documentation on [ReadtheDocs.io](http://tdxlib.readthedocs.io).
+8. TDXLib can also be configured directly by a python dictionary. 
+
+    Settings passed in as a dictionary are overwritten by any values in a filename (and if no file name is passed, the default configuration file, `tdxlib.ini` in the working directory)
+   
+    Use the following format for the dictionary configuration:
+    <pre>
+    config = {
+         "org_name": "exampleorg",
+         "sandbox": true,
+         "auth_type": "password",
+         "username": "someone@example.edu",
+         "password": "a password",
+         "ticket_app_id": 300,
+         "asset_app_id": "",
+         "caching": true,
+         "timezone": "-0500",
+         "log_level": "ERROR"
+     }
+    </pre>
+    The only required settings in this are `org_name` and either `asset_app_id` or `ticket_app_id` if you're creating `TDXAssetIntegration` or `TDXTicketIntegration` objects. If you set `auth_type` to `password` a username is also required.
+    Unset settings will be defaulted per the values in `tdxlib.tdx_constants.default_config`.
+9. TDXLib can also be configured via Environment variables. Any values passed in via dictionary, from a file, or in the default configuration file (`tdxlib.ini` in the working directory) override any values passed in as environment variables. 
+
+    Here's a sample of environment variables you can use (they are the same as the config values for dictionary config, but uppercase and prefixed with `TDXLIB_`): 
+    <pre>
+        export TDXLIB_ORG_NAME=exampleorg
+        export TDXLIB_SANDBOX=true
+        export TDXLIB_AUTH_TYPE=password
+        export TDXLIB_USERNAME=someon@example.edu
+        export TDXLIB_PASSWORD=mypassword
+        export TDXLIB_TICKET_APP_ID=300
+        export TDXLIB_ASSET_APP_ID=400
+        export TDXLIB_CACHING=true
+        export TDXLIB_TIMEZONE=-0500
+        export TDXLIB_LOG_LEVEL=ERROR
+   </pre>
+10. Congratulations! You now have the power of the TeamDynamix API at your fingertips. For more detailed tutorials on how to use TDXLib to manipulate Tickets and Asset, as well as for information on the methods and classes included with TDXLib, check out our documentation on [ReadtheDocs.io](http://tdxlib.readthedocs.io).
     
 
 ##  TDXLib Implementation status and Future Plans
 
 * ### TDXIntegration:
 
     This base class that contains the methods necessary to authenticate to Teamdynamix. This class also contains methods to interact with TeamDyanamix objects that are universal across various Apps (Locations, People, Accounts, etc.)
```

### Comparing `TDXLib-0.4.3/setup.py` & `TDXLib-0.5.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", 'r', encoding='utf-8"') as fh:
     outer_long_description = fh.read()
 
 setup(
     name='TDXLib',
     description='a python library for interacting with the TeamDynamix Web API',
-    version='0.4.3',
+    version='0.5.0',
     author='Nat Biggs, Stephen Gaines, Josiah Lansford',
     author_email='tdxlib@cedarville.edu',
     packages=['tdxlib'],
     url='https://github.com/cedarville-university/tdxlib',
     license='GNU General Public License v3.0',
     long_description_content_type='text/markdown',
     long_description=outer_long_description,
```

### Comparing `TDXLib-0.4.3/tdxlib/tdx_asset_integration.py` & `TDXLib-0.5.0/tdxlib/tdx_asset_integration.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,40 +5,40 @@
 from typing import Union
 from tdxlib.tdx_api_exceptions import *
 
 
 class TDXAssetIntegration(tdxlib.tdx_integration.TDXIntegration):
     def __init__(self, filename: str = None):
         tdxlib.tdx_integration.TDXIntegration.__init__(self, filename)
-        if self.asset_app_id is None:
-            raise ValueError("Asset App Id is required. Check your INI file for 'assetappid = 000'")
+        if self.config.asset_app_id is None:
+            raise RuntimeError("Asset App Id is required. Check your configuration.")
         
         self.clean_cache()
 
     def clean_cache(self) -> None:
         """
         Internal method to refresh the cache in a tdxlib object.
         """
         super().clean_cache()
-        if not self.caching:
+        if not self.config.caching:
             return
         self.cache['product_model'] = {}
         self.cache['product_type'] = {}
         self.cache['vendor'] = {}
         self.cache['asset_form'] = {}
         self.cache['asset_status'] = {}
         self.cache['custom_attributes'] = self.get_all_asset_custom_attributes()
         self.cache['custom_attributes'].append(self.get_all_custom_attributes(
-            tdxlib.tdx_integration.TDXIntegration.component_ids['configuration_item'], app_id=self.asset_app_id))
+            tdxlib.tdx_integration.TDXIntegration.component_ids['configuration_item'], app_id=self.config.asset_app_id))
 
     def _make_asset_call(self, url: str, action: str, post_body: Union[dict, list] = None) -> Union[list, dict]:
         """
         Internal method to make a http call using the assets endpoints and the provided HTTP verb.
         """
-        url_string = '/' + str(self.asset_app_id) + '/assets'
+        url_string = '/' + str(self.config.asset_app_id) + '/assets'
         if len(url) > 0:
             url_string += '/' + url
         if action == 'get':
             return self.make_get(url_string)
         if action == 'delete':
             return self.make_delete(url_string)
         if action == 'post' and post_body:
@@ -53,15 +53,15 @@
         """
         Makes an HTTP call using the Assets API information.
 
         :param url: The URL (everything after assets/) to call
         :param action: The HTTP action (get, put, post, delete, patch) to perform.
         :param post_body: A python dict of the information to post, put, or patch. Not used for get/delete.
 
-        :return: the API's response as a python dict or list
+        :return: the API response as a python dict or list
 
         """
         return self._make_asset_call(url, action, post_body)
 
     def get_all_asset_forms(self) -> list:
         """
         Gets a list asset forms
@@ -153,15 +153,15 @@
         """
         Creates a new Product Type with the information provided.
 
         :param name: The name of the new product type
         :param description: A description of the type (optional)
         :param parent: A Type (dict) or Type ID to set as the parent type of this type (creates a subtype)(optional)
         :param order: Sort order for this type (optional, defaults to 1)
-        :param active: Boolean indicating whether or not the new type should be active (optional, default True)
+        :param active: Boolean indicating whether the new type should be active (optional, default True)
 
         :return: dict of created product type
 
         """
 
         data = {'Name': name, 'IsActive': active, 'Order': order}
         if parent:
@@ -272,15 +272,15 @@
         Creates a new Product Model with the information provided.
 
         :param name: The name of the new product model
         :param product_type: A Type (dict) or Type ID to set as the product type of this model
         :param source: The manufacturer or vendor the model is sourced from
         :param description: A description of the model (optional)
         :param part_number: Part number for this model (optional)
-        :param active: Boolean indicating whether or not the new model should be active (optional, default True)
+        :param active: Boolean indicating whether the new model should be active (optional, default True)
         :param attributes: Dict of custom attributes to set on the new model (no validation yet -- build this by hand)
 
         :return: dict of created product type
 
         """
 
         data = {'Name': name, 'IsActive': active}
@@ -375,15 +375,15 @@
     def add_asset_user(self, asset_id: str, user_uid: str) -> dict:
         """
         Adds a users to an asset
 
         :param asset_id: the ID of the asset to get users
         :param user_uid: the UID of the person to add
 
-        :return: the API's response (success/failure only)
+        :return: the API response (success/failure only)
         """
         return self.make_call(f'{asset_id}/users/{user_uid}', 'post', {'data': None})
 
     def get_asset_users(self, asset_id: str) -> list:
         """
         Gets users of an asset
 
@@ -600,15 +600,15 @@
 
     def get_assets_by_requesting_department(self, dept: Union[dict, str], max_results: int = 25,
                                             full_record: bool = False, retired: bool = False, disposed: bool = False,
                                             all_statuses: bool = False) -> list:
         """
         Gets all assets requested by a particular account/department in TDX
 
-        :param dept: the name or email of a account/department, or a dict containing its information
+        :param dept: the name or email of an account/department, or a dict containing its information
         :param max_results: an integer indicating the maximum number of results that should be returned (default: 25)
         :param full_record: boolean indicating whether to fetch the full Asset record, or just summary info
         :param retired: include retired assets in search if true
         :param disposed: include disposed assets in search if true
         :param all_statuses: gets assets, regardless of what their status is (default: False)
 
         :return: a list of assets requested by that department
@@ -821,35 +821,37 @@
         else:
             raise TdxApiObjectTypeError(
                 f"Department of type {str(type(new_dept))} not searchable."
             )
         return self.update_assets(asset, changed_attributes)
 
     def get_all_asset_custom_attributes(self):
-        return self.get_all_custom_attributes(TDXAssetIntegration.component_ids['asset'], app_id=self.asset_app_id)
+        return self.get_all_custom_attributes(TDXAssetIntegration.component_ids['asset'],
+                                              app_id=self.config.asset_app_id)
 
     def get_asset_custom_attribute_by_name_id(self, key: str) -> dict:
         """
         Gets a specific Asset Custom Attribute object
 
         :param key: name or id of the Custom Attribute. This must be the exact name, no partial searching.
 
         :return: dict of custom attribute data
 
         """
         search_key = str(key) + "_asset_ci"
-        if self.caching and search_key in self.cache['ca_search']:
+        if self.config.caching and search_key in self.cache['ca_search']:
             return self.cache['ca_search'][search_key]
         # There is no API for searching attributes -- the only way is to get them all.
-        if self.caching:
+        if self.config.caching:
             custom_attributes = self.cache['custom_attributes']
         else:
             custom_attributes = self.get_all_asset_custom_attributes()
             custom_attributes.append(self.get_all_custom_attributes(
-                tdxlib.tdx_integration.TDXIntegration.component_ids['configuration_item'], app_id=self.asset_app_id))
+                tdxlib.tdx_integration.TDXIntegration.component_ids['configuration_item'],
+                app_id=self.config.asset_app_id))
         for item in custom_attributes:
             if type(item) == dict:
                 if str(key).lower() == item['Name'].lower() or str(key) == str(item['ID']):
                     self.cache['ca_search'][search_key] = item
                     return item
         raise TdxApiObjectNotFoundError(
             "No custom asset or CI attribute found for " + str(key))
@@ -1050,15 +1052,15 @@
         :rtype: dict
 
         """
         # set defaults
         if not acquisition_date:
             acquisition_date = datetime.datetime.today()
         if not requester:
-            requester = self.username
+            requester = self.config.username
         if not external_id:
             external_id = serial_number
 
         # Required or defaulted parameters
         data = dict()
         data['Name'] = asset_name
         data['SerialNumber'] = serial_number
@@ -1123,15 +1125,15 @@
         return data
 
     def create_asset(self, asset: dict, check_duplicate: bool = True) -> dict:
         """
         Creates an asset
 
         :param asset: a dict of asset info (maybe from make_asset_json()) to use in creation
-        :param check_duplicate: boolean of whether or not we should check to see if this is a duplicate asset
+        :param check_duplicate: boolean of whether we should check to see if this is a duplicate asset
 
         :return: dict of created asset details
 
         """
         if check_duplicate:
             duplicate = None
             serial = asset['SerialNumber']
```

### Comparing `TDXLib-0.4.3/tdxlib/tdx_integration.py` & `TDXLib-0.5.0/tdxlib/tdx_integration.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,356 +1,111 @@
-import configparser
 import requests
 import json
-import getpass
 import tdxlib.tdx_api_exceptions
+import tdxlib.tdx_constants
+import tdxlib.tdx_config
 import datetime
 import time
 from typing import BinaryIO
 import jwt
 import logging
 
 
 class TDXIntegration:
+    component_ids = tdxlib.tdx_constants.component_ids
 
-    # Hard-coded into TDX
-    component_ids = {
-        'account': 14,
-        'asset': 27,
-        'configuration_item': 63,
-        'contract': 29,
-        'file_cabinet': 8,
-        'issue': 3,
-        'opportunity': 11,
-        'person': 31,
-        'product': 37,
-        'product_model': 30,
-        'project': 1,
-        'ticket': 9,
-        'vendor': 28
-    }
-    default_config = {
-        'filename': 'tdxlib.ini',
-        # 'orgname': '',
-        # 'sandbox': True,
-        # 'authType': 'password',
-        # 'ticketAppId': '',
-        # 'assetAppId': '',
-        'caching': False,
-        'timezone': '-0500',
-        'logLevel': 'ERROR'
-    }
-
-    def __init__(self, filename=None, config=None):
-        self.config_filename = None
-        self.settings = None
-        self.api_url = None
-        self.token = None
-        self.token_exp = None
-        self.timezone = None
-        self.log_level = None
-        self.caching = True
-        self.sandbox = True
-        self.username = None
-        self.password = None
-        self.org_name = None
-        self.auth_type = None
-        self.ticket_app_id = None
-        self.asset_app_id = None
+    def __init__(self, filename: str = None, config: dict = None):
         self.cache = dict()
         self.logger = logging.getLogger('tdx_integration')
-        self.config = configparser.ConfigParser()
-
-        self.load_config_from_file(filename)
-
-        if 'TDX API Settings' not in self.config:
-            self.set_config(config)
-            self.run_setup_wizard()
-
-        self.config_to_attributes()
-        # Default to UTC -- for backwards compatibility
-        self.setup_from_loaded_config()
+        self.config = tdxlib.tdx_config.TDXConfig(filename, config)
+        self.setup_logs()
         self.clean_cache()
+        self.check_auth_init()
 
-    def config_to_attributes(self):
-        # Read settings in
-        self.settings = self.config['TDX API Settings']
-        self.org_name = self.settings.get('orgname')
-        
-        self.sandbox = self.settings.getboolean('sandbox')
-        self.auth_type = self.settings.get('authType')
-        if not self.auth_type or self.auth_type == 'password':
-            self.username = self.settings.get('username')
-            self.password = self.settings.get('password')
-        self.ticket_app_id = self.settings.get('ticketAppId')
-        self.asset_app_id = self.settings.get('assetAppId')
-        self.caching = self.settings.getboolean('caching')
-        self.timezone = self.settings.get('timezone')
-
-    def setup_from_loaded_config(self):
-        if not self.timezone:
-            self.timezone = 'Z'
-
-        if self.sandbox:
-            api_end = '/SBTDWebApi/api'
-        else:
-            api_end = '/TDWebApi/api'
-
-        full_host = self.settings.get('full_host', None)
-        if full_host is None:
-            self.api_url = 'https://' + self.org_name + '.teamdynamix.com' + api_end
-        else:
-            self.api_url = 'https://' + full_host + api_end
-
-        if not self.auth_type or self.auth_type == 'password':
-            if self.password == 'Prompt':
-                pass_prompt = 'Enter the TDX Password for user ' + self.username + \
-                              ' (this password will not be stored): '
-                self.password = getpass.getpass(pass_prompt)
-
-        if self.log_level:
+    def setup_logs(self):
+        if self.config.log_level:
             self.logger = logging.getLogger('tdx_integration')
-            self.logger.setLevel(logging.getLevelName(self.log_level))
+            self.logger.setLevel(logging.getLevelName(self.config.log_level))
 
-        if not self.auth_type or self.auth_type == 'password':
+    def check_auth_init(self):
+        if not self.config.auth_type or self.config.auth_type == 'password':
             if not self.auth():
-                self.logger.error(f"Login Failed. Username or password in {self.config_filename} likely incorrect.")
-        elif self.auth_type == 'token':
-            if self.token is None:
-                self.token_exp = time.time()
+                self.logger.error(f"Login Failed. Username or password in {self.config.filename} likely incorrect.")
+        elif self.config.auth_type == 'token':
+            if self.config.token is None:
+                self.config.token_exp = time.time()
                 self.logger.info("Skipping initial authentication, no token provided yet.")
             else:
                 if not (self.auth()):
-                    self.logger.error(f"Login Failed. Username or password in {self.config_filename} likely incorrect.")
-
-    def load_config_from_file(self, filename: str):
-        # Read in configuration
-        if filename is None:
-            filename = self.default_config["filename"]
-        self.config.read(filename)
-        return
-
-    def set_config(self, config: dict):
-        if not config:
-            config = self.default_config
-        
-        self.config['TDX API Settings'] = config
+                    self.logger.error(f"Login Failed. Username or password in {self.config.filename} likely incorrect.")
 
-    def run_setup_wizard(self):
-        # Initialization wizard
-        print("\nNo configuration file found. Please enter the following information: ")
-
-        self.set_fqdn_wizard()
-        self.set_sandbox_wizard()
-        self.set_auth_type_wizard()
-        self.set_ticket_app_id_wizard()
-        self.set_asset_app_id_wizard()
-        self.set_caching_wizard()
-        self.set_timezone_wizard()
-        self.set_logging_wizard()
-        self.save_config_wizard()
-    
-    def set_fqdn_wizard(self):
-        fqdn_invalid = True
-        fqdn = False
-        while fqdn_invalid:
-            fqdn_choice = input("\nUse a Fully-Qualified DNS Name for your TDX Instance "
-                                "(if not *.teamdynamix.com)? [Y/N]: ")
-            if fqdn_choice.lower() in ['y', 'ye', 'yes', 'true']:
-                fqdn = True
-                fqdn_invalid = False
-            elif fqdn_choice.lower() in ['n', 'no', 'false']:
-                fqdn_invalid = False
-        if fqdn:
-            print("Enter the fully qualified DNS name of your TDX instance.")
-            init_full_host = input("FQDN (its.myuniversity.edu): ")
-            self.config.set('TDX API Settings', 'full_host', init_full_host)
-        else:
-            print("\n\nPlease enter your TeamDynamix organization name.")
-            print("This is the teamdynamix.com subdomain that you use to access TeamDynamix.")
-            init_org_name = input("Organization Name/FQDN (<orgname>.teamdynamix.com/<FQDN>): ")
-            self.config.set('TDX API Settings', 'orgname', init_org_name)
-
-    def set_sandbox_wizard(self):
-        sandbox_invalid = True
-        while sandbox_invalid:
-            sandbox_choice = input("\nUse TeamDynamix Sandbox? [Y/N]: ")
-            if sandbox_choice.lower() in ['y', 'ye', 'yes', 'true']:
-                self.config.set('TDX API Settings', 'sandbox', 'true')
-                sandbox_invalid = False
-            elif sandbox_choice.lower() in ['n', 'no', 'false']:
-                self.config.set('TDX API Settings', 'sandbox', 'false')
-                sandbox_invalid = False
-
-    def set_token_wizard(self):
-        provided_token = input("\nInput token now, or leave blank to fill programatically later: ")
-        if provided_token != "":
-            self.token = provided_token
-
-    def set_password_wizard(self):
-        init_username = input("\nTDX API Username (tdxuser@orgname.com): ")
-        self.config.set('TDX API Settings', 'username', init_username)
-        print("\nTDXLib can store the password for the API user in the configuration file.")
-        print("This is convenient, but not very secure.")
-        password_invalid = True
-        while password_invalid:
-            password_choice = input("Store password for " + init_username + "? [Y/N]: ")
-            if password_choice.lower() in ['y', 'ye', 'yes', 'true']:
-                password_prompt = '\nEnter Password for ' + init_username + ": "
-                init_password = getpass.getpass(password_prompt)
-                self.config.set('TDX API Settings', 'password', init_password)
-                password_invalid = False
-            elif password_choice.lower() in ['n', 'no', 'false']:
-                self.config.set('TDX API Settings', 'password', 'Prompt')
-                password_invalid = False
-            if password_invalid:
-                print("\nInvalid Response.")
-
-    def set_auth_type_wizard(self):
-        auth_type_invalid = True
-        auth_type = "password"
-        while auth_type_invalid:
-            auth_type = input("\nAuthentication Type (Only password and token currently supported) [password]: ")
-            if auth_type == '':
-                auth_type = 'password'
-            if auth_type == "password":
-                self.set_password_wizard()
-                auth_type_invalid = False
-            elif auth_type == "token":
-                self.set_token_wizard()
-                auth_type_invalid = False
-        self.config.set("TDX API Settings", "authType", auth_type)
-
-    def set_asset_app_id_wizard(self):
-        init_asset_id = input("\nAssets App ID (optional): ")
-        self.config.set('TDX API Settings', 'assetAppId', init_asset_id)
-    
-    def set_ticket_app_id_wizard(self):
-        init_ticket_id = input("\nTickets App ID (optional): ")
-        self.config.set('TDX API Settings', 'ticketAppId', init_ticket_id)
-
-    def set_caching_wizard(self):
-        print("\nTDXLib uses intelligent caching to speed up API calls on repetitive operations.")
-        print("In very dynamic environments, TDXLib's caching can cause issues.")
-        caching_invalid = True
-        while caching_invalid:
-            caching_choice = input("Disable Caching? Y/N [N]: ")
-            if caching_choice == '' or caching_choice.lower() in ['y', 'ye', 'yes', 'true']:
-                self.config.set('TDX API Settings', 'caching', 'true')
-                self.caching = False
-                caching_invalid = False
-            elif caching_choice.lower() in ['n', 'no', 'false']:
-                self.config.set('TDX API Settings', 'caching', 'false')
-                self.caching = True
-                caching_invalid = False
-            if caching_invalid:
-                print("Invalid Response.")
-                
-    def set_timezone_wizard(self):
-        print("\nWhat timezone would you like to set for this integration (default: '-0500')?")
-        timezone_invalid = True
-        while timezone_invalid:
-            timezone_choice = input(f"Timezone (default: {self.default_config['timezone']} ) [+/-0000]: ")
-            if len(timezone_choice) == 5 and timezone_choice[:1] in ["+", "-"] and timezone_choice[1:].isdigit():
-                self.config.set('TDX API Settings', 'timezone', timezone_choice)
-                self.timezone = timezone_choice
-                timezone_invalid = False
-            if len(timezone_choice) == 0:
-                self.config.set('TDX API Settings', 'timezone', '-0500')
-                self.timezone = self.default_config['timezone']
-                timezone_invalid = False
-            if timezone_invalid:
-                print("Invalid Reponse.")
-
-    def set_logging_wizard(self):
-        logging_invalid = False
-        while logging_invalid:
-            logging_choice = input(f"Log Level (default: {self.default_config['logging_level']}) "
-                                   f"[CRITICAL, ERROR, WARNING, INFO, DEBUG]: ")
-            if logging_choice in ["WARNING", "ERROR", "INFO", "DEBUG", "CRITICAL"]:
-                self.config.set('TDX API Settings', 'logLevel', logging_choice)
-                self.log_level = logging_choice
-                logging_invalid = False
-            if len(logging_choice) == 0:
-                self.config.set('TDX API Settings', 'logLevel', 'ERROR')
-                self.log_level = self.default_config['logging_level']
-                logging_invalid = False
-            if logging_invalid:
-                print("Invalid Reponse")
-    
-    def save_config_wizard(self):
-        filename = input(f"Enter config filename (default: {self.default_config['filename']}): ")
-        if filename == "":
-            filename = self.default_config['filename']
-        with open(filename, 'w') as configfile:
-            self.config.write(configfile)
-        print(f'\nSettings saved to {filename}')
-        self.config_filename = filename
+    def set_token(self, token: str):
+        self.config.token = token
 
     def auth(self) -> bool:
         """
         Internal method to authenticate to the TDX api using the selected method
         Stores a token in the token property, used for future calls. Returns true for success, false for failure.
         """
-        if not self.auth_type or self.auth_type == 'password':
+        if not self.config.auth_type or self.config.auth_type == 'password':
             try:
                 response = requests.post(
-                    url=str(self.api_url) + '/auth',
+                    url=str(self.config.api_url) + '/auth',
                     headers={
                         "Content-Type": "application/json; charset=utf-8",
                     },
                     data=json.dumps({
-                        "username": self.username,
-                        "password": self.password
+                        "username": self.config.username,
+                        "password": self.config.password
                     })
                 )
                 if response.status_code != 200:
                     raise tdxlib.tdx_api_exceptions.TdxApiHTTPError(" Response code: " + str(response.status_code) +
                                                                     " " + response.reason + " " + " Returned: " +
                                                                     response.text)
                 else:
-                    self.token = response.text
+                    self.config.token = response.text
                     time.sleep(1)
                     # Decode token to identify expiration date
-                    decoded = jwt.decode(self.token,
+                    decoded = jwt.decode(self.config.token,
                                          algorithms=['HS256'],
                                          options={'verify_signature': False},
                                          audience="https://www.teamdynamix.com/")
-                    self.token_exp = decoded['exp']
+                    self.config.token_exp = decoded['exp']
                     return True
 
             except requests.exceptions.RequestException as e:
                 self.logger.warning(f"Auth request Failed. Exception: {str(e)}")
                 return False
             except tdxlib.tdx_api_exceptions.TdxApiHTTPError as e:
                 self.logger.error(str(e))
                 return False
-        elif self.auth_type == 'token':
-            if self.token is None:
-                self.token_exp = time.time()
+        elif self.config.auth_type == 'token':
+            if self.config.token is None:
+                self.config.token_exp = time.time()
                 self.logger.info("Skipping initial authentication, no token provided yet.")
             # Decode token to identify expiration date
-            decoded = jwt.decode(self.token,
+            decoded = jwt.decode(self.config.token,
                                  algorithms=['HS256'],
                                  options={'verify_signature': False},
                                  audience="https://www.teamdynamix.com/")
-            self.token_exp = decoded['exp']
+            self.config.token_exp = decoded['exp']
             return True
         else:
             return False
 
     def _check_auth_exp(self) -> bool:
         """
         Internal method to check the expiration of the stored access token.
         If it is expired, call auth() to get a new token.
         """
         # If token is expired or will expire in the next minute, get new token
-        if self.token_exp:
-            if self.token_exp < time.time() + 60:
-                self.logger.info(f"Token expires at {str(datetime.datetime.utcfromtimestamp(self.token_exp))}. "
+        if self.config.token_exp:
+            if self.config.token_exp < time.time() + 60:
+                self.logger.info(f"Token expires at {str(datetime.datetime.utcfromtimestamp(self.config.token_exp))}. "
                                  f"Getting new token...")
                 return self.auth()
             else:
                 return True
         else:
             return self.auth()
 
@@ -370,35 +125,35 @@
                         sleep_time = difference + datetime.timedelta(0, skew_mitigation_secs)
                         self.logger.info("Rate-limited by TeamDynamix. Sleeping "
                                          + str(sleep_time.seconds) + " seconds.")
                         time.sleep(sleep_time.seconds)
 
     def make_get(self, request_url: str, retries: int = 3):
         """
-        Makes a HTTP GET request to the TDX Api.
+        Makes an HTTP GET request to the TDX Api.
 
         :param request_url: the path (everything after /TDWebAPI/api/) to call
         :param retries: the number of times to retry a failed request (defaults to 3)
 
         :return: the API's response as a python dict or list
 
         """
         self._rate_limit()
-        get_url = self.api_url + request_url
+        get_url = self.config.api_url + request_url
         response = None
         attempts = 0
         while attempts < retries:
             try:
                 if not (self._check_auth_exp()):
                     raise tdxlib.tdx_api_exceptions.TdxApiHTTPError(
                         f"Login Failed. Username or password in config likely incorrect.")
                 response = requests.get(
                     url=get_url,
                     headers={
-                        "Authorization": 'Bearer ' + self.token,
+                        "Authorization": 'Bearer ' + self.config.token,
                         "Content-Type": "application/json; charset=utf-8",
                     }
                 )
                 if response.status_code != 200:
                     err_string = " Response code: " + str(response.status_code) + \
                         " " + response.reason + " " + " Returned: " + response.text
                     raise tdxlib.tdx_api_exceptions.TdxApiHTTPError(err_string)
@@ -418,33 +173,33 @@
                     message += response.text
                 self.logger.error(f"{message}")
             finally:
                 attempts += 1
 
     def make_post(self, request_url: str, body: dict):
         """
-        Makes a HTTP POST request to the TDX Api
+        Makes an HTTP POST request to the TDX Api
 
         :param request_url: the path (everything after /TDWebAPI/api/) to call
         :param body: dumped JSON data to send with the POST
 
         :return: the API's response as a python dict or list
 
         """
         self._rate_limit()
-        post_url = self.api_url + request_url
+        post_url = self.config.api_url + request_url
         response = None
         try:
             if not (self._check_auth_exp()):
                 raise tdxlib.tdx_api_exceptions.TdxApiHTTPError(
                     f"Login Failed. Username or password in config likely incorrect.")
             response = requests.post(
                 url=post_url,
                 headers={
-                    "Authorization": 'Bearer ' + self.token,
+                    "Authorization": 'Bearer ' + self.config.token,
                     "Content-Type": "application/json; charset=utf-8",
                 },
                 data=json.dumps(body))
             if response.status_code not in [200, 201]:
                 raise tdxlib.tdx_api_exceptions.TdxApiHTTPError(
                     " Response code: " + str(response.status_code) + " " +
                     response.reason + "\n" + "Returned: " + response.text)
@@ -464,41 +219,41 @@
             message = 'Invalid JSON received POST to ' + post_url + ':\n'
             if response:
                 message += response.text
             self.logger.error(f"{message}")
 
     def make_file_post(self, request_url: str, file: BinaryIO, filename: str = None):
         """
-        Makes a HTTP POST request to the TDX Api with a Multipart-Encoded File
+        Makes an HTTP POST request to the TDX Api with a Multipart-Encoded File
         
         :param request_url: the path (everything after /TDWebApi/api/) to call
         :param file: BinaryIO object opened in read mode to upload as attachment.
         (read documentation at requests.readthedocs.io/en/master/user/quickstart/#post-a-multipart-encoded-file)
         :param filename: (optional), allows to explicitly specify filename header. If None, requests will determine
         from passed-in file object.
         This is useful for if you want to upload a file in memory without a filename, which is required
         for uploading to TeamDynamix.
 
         :return: the API's response as a python dict
         """
         self._rate_limit()
-        post_url = self.api_url + request_url
+        post_url = self.config.api_url + request_url
         response = None
         if filename:
             files = {'file': (filename, file)}
         else:
             files = {'file': file}
         try:
             if not (self._check_auth_exp()):
                 raise tdxlib.tdx_api_exceptions.TdxApiHTTPError(
                     f"Login Failed. Username or password in config likely incorrect.")
             response = requests.post(
                 url=post_url,
                 headers={
-                    "Authorization": 'Bearer ' + self.token,
+                    "Authorization": 'Bearer ' + self.config.token,
                 },
                 files=files
             )
             if response.status_code not in [200, 201]:
                 raise tdxlib.tdx_api_exceptions.TdxApiHTTPError(
                     " Response code: " + str(response.status_code) + " " +
                     response.reason + "\n" + "Returned: " + response.text)
@@ -524,24 +279,24 @@
         :param request_url: the path (everything after /TDWebAPI/api/) to call
         :param body: dumped JSON data to send with the PUT
 
         :return: the API's response as a python dict or list
 
         """
         self._rate_limit()
-        put_url = self.api_url + request_url
+        put_url = self.config.api_url + request_url
         response = None
         try:
             if not (self._check_auth_exp()):
                 raise tdxlib.tdx_api_exceptions.TdxApiHTTPError(
                     f"Login Failed. Username or password in config likely incorrect.")
             response = requests.put(
                 url=put_url,
                 headers={
-                    "Authorization": 'Bearer ' + self.token,
+                    "Authorization": 'Bearer ' + self.config.token,
                     "Content-Type": "application/json; charset=utf-8",
                 },
                 data=json.dumps(body))
             if response.status_code not in [200, 201, 202, 204]:
                 raise tdxlib.tdx_api_exceptions.TdxApiHTTPError(
                     " Response code: " + str(response.status_code) + " " +
                     response.reason + "\n" + "Returned: " + response.text)
@@ -567,23 +322,23 @@
         :param request_url: the path (everything after /TDWebAPI/api/) to call
 
         :return: None
 
         """
         self._rate_limit()
 
-        delete_url = self.api_url + request_url
+        delete_url = self.config.api_url + request_url
         try:
             if not (self._check_auth_exp()):
                 raise tdxlib.tdx_api_exceptions.TdxApiHTTPError(
                     f"Login Failed. Username or password in config likely incorrect.")
             response = requests.delete(
                 url=delete_url,
                 headers={
-                    "Authorization": 'Bearer ' + self.token,
+                    "Authorization": 'Bearer ' + self.config.token,
                     "Content-Type": "application/json; charset=utf-8",
                 })
             if response.status_code not in [200, 201]:
                 raise tdxlib.tdx_api_exceptions.TdxApiHTTPError(
                     " Response code: " + str(response.status_code) + " " +
                     response.reason + "\n" + "Returned: " + response.text)
             self.cache['rate_limit']['remaining'] = int(response.headers['X-RateLimit-Remaining'])
@@ -594,35 +349,35 @@
         except tdxlib.tdx_api_exceptions.TdxApiHTTPError as e:
             self.logger.error(f"DELETE to {request_url} returned non-success code. {str(e)}")
 
     def make_patch(self, request_url: str, body: dict):
         """
         Makes an HTTP PATCH request to the TDX API.
 
-        The TeamDyanmix API supports limited PATCH functionality. Since TDX data is highly structured, items are
+        The TeamDynamix API supports limited PATCH functionality. Since TDX data is highly structured, items are
         referenced explicitly by their TDX ID, and not by their order in the object. Likewise, since the fields
         in a TDX object are all predefined, a PATCH call cannot add or remove any fields in the object.
 
         :param request_url: the path (everything after /TDWebAPI/api/) to call
         :param body: a list of PATCH operations as dictionaries, each including the keys "op", "path", and "value"
 
         :return: the API's response, as a python dict or list
 
         """
         self._rate_limit()
-        patch_url = self.api_url + request_url
+        patch_url = self.config.api_url + request_url
         response = None
         try:
             if not (self._check_auth_exp()):
                 raise tdxlib.tdx_api_exceptions.TdxApiHTTPError(
                     f"Login Failed. Username or password in config likely incorrect.")
             response = requests.patch(
                 url=patch_url,
                 headers={
-                    "Authorization": 'Bearer ' + self.token,
+                    "Authorization": 'Bearer ' + self.config.token,
                     "Content-Type": "application/json; charset=utf-8",
                 },
                 data=json.dumps(body)
             )
 
             if response.status_code not in [200, 201]:
                 raise tdxlib.tdx_api_exceptions.TdxApiHTTPError(
@@ -710,15 +465,15 @@
 
         :rtype: dict
         """
         return self.get_tdx_item_by_id('groups', group_id)
 
     def get_person_by_uid(self, uid: str) -> dict:
         """
-        Gets a a person by their UID.
+        Gets a person by their UID.
 
         :param uid: UID string corresponding to a person
 
         :return: dict of person data
 
         :rtype: dict
         """
@@ -895,15 +650,15 @@
     def get_custom_attribute_by_name_id(self, key: str, object_type: int) -> dict:
         """
         Gets a custom attribute for the component type.
         See https://solutions.teamdynamix.com/TDClient/KB/ArticleDet?ID=22203 for possible values for component_type.
 
         *NOTE: The best way to assign CA's is to test for an existing value (for choice-based CA's) using
         get_custom_attribute_value_by_name, and then if it returns false, directly assign the desired value to the CA.
-        Because of this, date-type and other format-specific attributes need to be in a TDX-acceptible format, this
+        Because of this, date-type and other format-specific attributes need to be in a TDX-acceptable format, this
         means that a field designated to hold person objects needs to be set to a UID.*
 
         :param key: a partial or full name of the custom attribute to search for
         :param object_type: the object type ID to get attributes for
 
         :return: the attribute as a dict, with all choice items included
 
@@ -924,19 +679,19 @@
             "No custom attribute found for " + str(key) + ' and object type ' + str(object_type))
 
     def get_custom_attribute_choice_by_name_id(self, attribute, key):
         """
         Gets the choice item from a custom attribute, maybe from get_custom_attribute_by_name()
 
         *NOTE: The best way to assign CA's is to test for an existing value (for choice-based CA's), and then if this
-        method returns false, directly assign the desired value to the CA. Because of this, date-type and other format-
-        specific attributes need to be in a TDX-acceptible format, this means that a field designated to hold person
+        method returns false, directly assign the desired value to the CA. Because of this, date-type and other format
+        specific attributes need to be in a TDX-acceptable format, this means that a field designated to hold person
         objects needs to be set to a UID.*
 
-        :param key: a partial or full name name of the choice to look for
+        :param key: a partial or full name of the choice to look for
         :param attribute: a dict of custom attribute data (as retrieved from get_attribute_by_name())
 
         :return: the the choice object from this attribute whose name matches 'key', or False if none matches.
 
         :rtype: dict
 
         """
@@ -944,15 +699,15 @@
             for i in attribute['Choices']:
                 if str(key).lower() == str(i['Name']).lower() or str(key) == str(i['ID']):
                     return i
             raise tdxlib.tdx_api_exceptions.TdxApiObjectNotFoundError(
                 f"No custom attribute choice \"{str(key)}\" found in CA {attribute['Name']}")
         elif attribute['FieldType'] == 'datefield':
             value = tdxlib.tdx_utils.import_tdx_date(key)
-            return tdxlib.tdx_utils.export_tdx_date(value, self.timezone)
+            return tdxlib.tdx_utils.export_tdx_date(value, self.config.timezone)
         else:
             return str(key)
 
     def get_all_locations(self) -> list:
         """
         Gets all locations in TDX.
 
@@ -1000,15 +755,15 @@
     def get_room_by_name(location: dict, room: str) -> dict:
         """
         Gets a room by searching its name in location information, maybe from get_location_by_name().
 
         :param location: dict of location info
         :param room: partial or full name of a room to search for
 
-        :return: a dict with all the the information regarding the room. Use this to retrieve the ID attribute.
+        :return: a dict with all the information regarding the room. Use this to retrieve the ID attribute.
 
         :rtype: dict
 
         """
         for i in location['Rooms']:
             if str(room).lower() in i['Name'].lower():
                 return i
```

### Comparing `TDXLib-0.4.3/tdxlib/tdx_ticket.py` & `TDXLib-0.5.0/tdxlib/tdx_ticket.py`

 * *Files identical despite different names*

### Comparing `TDXLib-0.4.3/tdxlib/tdx_ticket_integration.py` & `TDXLib-0.5.0/tdxlib/tdx_ticket_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,16 @@
         'Cancelled': 4,
         'OnHold': 5,
         'Requested': 6
     }
 
     def __init__(self, filename: str = None, config=None):
         tdxlib.tdx_integration.TDXIntegration.__init__(self, filename, config)
-        if self.ticket_app_id is None:
-            raise ValueError("Ticket App Id is required. Check your config file for 'ticketappid = 000'")
+        if self.config.ticket_app_id is None:
+            raise RuntimeError("Ticket App Id is required. Check your configuration.")
         self.clean_cache()
 
     def clean_cache(self):
         """
         Clears the tdx_ticket_integration cache.
 
         :return:  None
@@ -48,15 +48,15 @@
         self.cache['ticket_priority'] = {}
         self.cache['ticket_urgency'] = {}
         self.cache['ticket_impact'] = {}
         self.cache['ticket_source'] = {}
         self.cache['ticket_form'] = {}
 
     def get_url_string(self):
-        return '/' + str(self.ticket_app_id) + '/tickets'
+        return '/' + str(self.config.ticket_app_id) + '/tickets'
 
     def _make_ticket_call(self, url: str, action: str, post_body: dict = None):
         url_string = self.get_url_string()
         if len(url) > 0:
             url_string += '/' + url
         if action == 'get':
             return self.make_get(url_string)
@@ -74,21 +74,22 @@
         """
         Makes an HTTP call using the Tickets API information.
 
         :param url: The URL (everything after tickets/) to call
         :param action: The HTTP action (get, put, post, delete, patch) to perform.
         :param post_body: A dict of the information to post, put, or patch. Not used for get/delete.
 
-        :return: the API's response as a python dict or list
+        :return: the API response as a python dict or list
 
         """
         return self._make_ticket_call(url, action, post_body)
 
     def get_all_ticket_custom_attributes(self):
-        return self.get_all_custom_attributes(TDXTicketIntegration.component_ids['ticket'], app_id=self.ticket_app_id)
+        return self.get_all_custom_attributes(TDXTicketIntegration.component_ids['ticket'],
+                                              app_id=self.config.ticket_app_id)
 
     def get_ticket_custom_attribute_by_name_id(self, key: str) -> dict:
         """
         Gets a ticket custom attribute based on its name or ID. This includes hard-coded the component ID for tickets.
 
         :param key: A full or partial name of the CA to get.
 
@@ -123,16 +124,16 @@
         if len(ca['Choices']) > 0:
             ca_choice = self.get_custom_attribute_choice_by_name_id(ca, value)
             value = ca_choice['ID']
         if isinstance(value, datetime.datetime):
             value = tdxlib.tdx_utils.export_tdx_date(value)
         return {'ID': ca['ID'], 'Value': value}
 
-    def change_ticket_custom_attribute_value(self, ticket: Union[dict, str, int, list], custom_attributes: list) \
-        -> Union[tdxlib.tdx_ticket.TDXTicket,list]:
+    def change_ticket_custom_attribute_value(self, ticket: Union[dict, str, int, list],
+                                             custom_attributes: list) -> Union[tdxlib.tdx_ticket.TDXTicket, list]:
         """
         Takes a correctly formatted list of CA's (from build_ticket_custom_attribute_value, for instance)
         and updates one or more assets with the new values.
 
         :param ticket: ticket/Ticket ID to update (doesn't have to be full record), or list of same
         :param custom_attributes: List of ID/Value dicts (from build_ticket_custom_attribute_value())
         :return: list of updated ticket in dict format
@@ -347,17 +348,17 @@
     def update_ticket(self, ticket_id: Union[str, int], comments: str, new_status: str = None, notify: list = None,
                       private: bool = True) -> dict:
         """
         Sends an update to a ticket feed.
 
         :param ticket_id: the ticket ID whose task to update
         :param comments: a string to provide as a comment to the update.
-        :param new_status: The name of the new status to set for the ticket (Default:
+        :param new_status: The name of the new status to set for the ticket (Default: The status whose ID is 0)
         :param notify: a list of strings containing email addresses to notify regarding this ticket. Default: None
-        :param private: boolean indicating whether or not the update to the task should be private. Default: True
+        :param private: boolean indicating whether the update to the task should be private. Default: True
 
         :return: python dict containing created ticket update information
 
         :rtype: dict
 
         """
         if not notify:
@@ -560,15 +561,15 @@
                 return ticket_priority
             if str(key).lower() in ticket_priority['Name'].lower():
                 return ticket_priority
         raise tdxlib.tdx_api_exceptions.TdxApiObjectNotFoundError(f'No priority found for {key}')
 
     def get_all_ticket_urgencies(self) -> list:
         """
-        Gets all ticket urgencies from the tickets app.
+        Gets all ticket urgencies from the Tickets app.
 
         :return: list of priorities in python dict
 
         :rtype: dict
 
         """
         url_string = "urgencies"
@@ -668,15 +669,15 @@
         Creates a custom ticket status.
 
         :param name:            A string containing the name of the new status. (Required)
         :param order:           A float containing the order number for sorting purposes.
         :param status_class:    A name of a status class. These values are hard-coded into the TDWebApi, and stored in
                                 this class as a class variable.
         :param description:     A string containing the description of the new status. (Default: Empty String)
-        :param active:          A bool indicating whether or not this new status should be active. (Default: True)
+        :param active:          A bool indicating whether this new status should be active. (Default: True)
 
         :return:                The new ticket status as a dict
 
         :rtype: dict
 
         """
         url_string = "statuses"
@@ -788,15 +789,15 @@
                     f"Attribute {k} not a writeable ticket task attribute"
                 )
 
     def edit_ticket_task(self, ticket_id: int, task: Union[str, int, dict], changed_attributes: dict) -> dict:
         """
         Edits a ticket task with a set of new values.
 
-        :param ticket_id: The ticket Id on which the ticket task exists.
+        :param ticket_id: The ticket ID on which the ticket task exists.
         :param task: a single ticket task in dict (maybe from get_ticket_task_by_id), or a task ID
         :param changed_attributes: The new values ot set on the ticket task.
 
         :return: The modified ticket task as a dict, if the operation was successful
 
         :rtype: dict
 
@@ -814,28 +815,28 @@
         url_string = f'{ticket_id}/tasks/{full_task["ID"]}'
         return self.make_call(url_string, 'put', full_task)
 
     def delete_ticket_task(self, ticket_id: str, task_id: str) -> None:
         """
         Deletes a ticket task by ID
 
-        :param ticket_id: The ticket Id on which the ticket task exists.
+        :param ticket_id: The ticket ID on which the ticket task exists.
         :param task_id: The task ID of the task you want to delete.
 
         :return: none
 
         """
         url_string = f'{ticket_id}/tasks/{task_id}'
         self.make_call(url_string, 'delete')
 
     def reassign_ticket_task(self, ticket_id: int, task: Union[str, dict, int], responsible: str, group=False) -> dict:
         """
         Reassigns a ticket task to a person or group
 
-        :param ticket_id: The ticket Id on which the ticket task exists.
+        :param ticket_id: The ticket ID on which the ticket task exists.
         :param task: a single ticket task in dict (maybe from get_ticket_task_by_id), or a task ID
         :param responsible: a username, email, Full Name, or ID number to use to search for a person, or a group name.
         :param group: If this parameter is True, assign to group instead of individual
 
         :return: The modified ticket task as a dict, if the operation was successful
 
         :rtype: dict
@@ -849,45 +850,45 @@
 
     def reschedule_ticket_task(self, ticket_id, task,
                                start_date: datetime.datetime = None,
                                end_date: datetime.datetime = None) -> dict:
         """
         Sets the start date and end date for a ticket task. This will affect the start & end dates of the parent ticket.
 
-        :param ticket_id: The ticket Id on which the ticket task exists.
+        :param ticket_id: The ticket ID on which the ticket task exists.
         :param task: a single ticket task in dict (maybe from get_ticket_task_by_id), or a task ID
         :param start_date: datetime.datetime object to use as the starting date for a task, defaults to now.
         :param end_date: datetime.datetime object to use as the starting date for a task, defaults to now + 1 day.
 
         :return: The modified ticket task as a dict, if the operation was successful
 
         :rtype: dict
 
         """
         if not start_date:
             start_date = datetime.datetime.utcnow()
         if not end_date:
             end_date = datetime.datetime.utcnow() + datetime.timedelta(days=1)
         new_dates = {
-            'StartDate': tdxlib.tdx_utils.export_tdx_date(start_date, self.timezone),
-            'EndDate': tdxlib.tdx_utils.export_tdx_date(end_date, self.timezone)
+            'StartDate': tdxlib.tdx_utils.export_tdx_date(start_date, self.config.timezone),
+            'EndDate': tdxlib.tdx_utils.export_tdx_date(end_date, self.config.timezone)
         }
         return self.edit_ticket_task(ticket_id, task, new_dates)
 
     def update_ticket_task(self, ticket_id: int, task_id: int, percent: int, comments: str = '',
                            notify: list = None, private: bool = True) -> dict:
         """
         Sends an update to a ticket task.
 
         :param ticket_id: the ticket ID whose task to update
         :param task_id: the ID of the task to update
         :param percent: the percent complete to set the task to after update
         :param comments: a string to provide as a comment to the update. Defaults to empty string.
         :param notify: a list of strings containing email addresses to notify regarding this ticket. Default: None
-        :param private: boolean indicating whether or not the update to the task should be private. Default: True
+        :param private: boolean indicating whether the update to the task should be private. Default: True
 
         :return: dict of update info
 
         :rtype: dict
 
         """
         if not notify:
@@ -972,27 +973,27 @@
         :param room: Room name of location (optional) Will not set room if location not included.
         :param active_days: number of days before due date to assign start date, default is 5
         :param priority: name of priority of ticket, default "Low"
         :param status: name of status for new ticket, default "New"
         :param requestor: name or email for requester of the ticket, defaults to username of integration (optional)
         :param classification: name of classification name for new ticket, default "Incident" (optional)
         :param form: name or ID of a form to use for the new ticket
-        :param responsible_is_group: Boolean indicating whether or not 'responsible' refers to a group. (Default: False)
+        :param responsible_is_group: Boolean indicating whether 'responsible' refers to a group. (Default: False)
         :param custom_attributes: dict of attribute names and values
 
         :return: TdxTicket object ready to be created via create_ticket()
 
         :rtype: tdxlib.tdx_ticket.TDXTicket
 
         """
         # Required by TDX for a new ticket: Type, Title, Account, Status, Priority, Requestor
 
         # set defaults
         if not requestor:
-            requestor = self.username
+            requestor = self.config.username
 
         # Required or defaulted parameters
         data = dict()
         data['TypeID'] = self.get_ticket_type_by_name_id(ticket_type)['ID']
         data['Classification'] = self.get_ticket_classification_id_by_name(classification)
         data['AccountID'] = self.get_account_by_name(account)['ID']
         data['StatusID'] = self.search_ticket_status(status)['ID']
@@ -1033,16 +1034,16 @@
 
         if due_date:
             if isinstance(due_date, datetime.datetime):
                 target_date = due_date
             else:
                 target_date = tdxlib.tdx_utils.import_tdx_date(due_date)
             start_date = target_date - datetime.timedelta(days=active_days)
-            data['StartDate'] = tdxlib.tdx_utils.export_tdx_date(start_date, self.timezone)
-            data['EndDate'] = tdxlib.tdx_utils.export_tdx_date(target_date, self.timezone)
+            data['StartDate'] = tdxlib.tdx_utils.export_tdx_date(start_date, self.config.timezone)
+            data['EndDate'] = tdxlib.tdx_utils.export_tdx_date(target_date, self.config.timezone)
 
         if location:
             building = self.get_location_by_name(location)
             data['LocationID'] = building['ID']
             if room:
                 data['LocationRoomID'] = self.get_room_by_name(building, room)['ID']
 
@@ -1080,16 +1081,16 @@
 
         """
         data = dict({'Title': title})
         data['EstimatedMinutes'] = est_minutes
         if description:
             data['Description'] = description
         if start and end:
-            data['StartDate'] = tdxlib.tdx_utils.export_tdx_date(start, self.timezone)
-            data['EndDate'] = tdxlib.tdx_utils.export_tdx_date(end, self.timezone)
+            data['StartDate'] = tdxlib.tdx_utils.export_tdx_date(start, self.config.timezone)
+            data['EndDate'] = tdxlib.tdx_utils.export_tdx_date(end, self.config.timezone)
         if completion_minutes:
             data['CompleteWithinMinutes'] = completion_minutes
         if group:
             data['ResponsibleGroupID'] = self.get_group_by_name(responsible)['ID']
         else:
             data['ResponsibleUid'] = self.get_person_by_name_email(responsible)['UID']
         if predecessor:
```

### Comparing `TDXLib-0.4.3/tdxlib/tdx_utils.py` & `TDXLib-0.5.0/tdxlib/tdx_utils.py`

 * *Files identical despite different names*

### Comparing `TDXLib-0.4.3/test/test_tdx_ticket_integration.py` & `TDXLib-0.5.0/test/test_tdx_ticket_integration.py`

 * *Files identical despite different names*

