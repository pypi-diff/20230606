# Comparing `tmp/codat-bankfeeds-0.6.4.tar.gz` & `tmp/codat-bankfeeds-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codat-bankfeeds-0.6.4.tar", last modified: Wed Mar 22 17:24:07 2023, max compression
+gzip compressed data, was "codat-bankfeeds-0.8.5.tar", last modified: Wed Apr  5 09:29:36 2023, max compression
```

## Comparing `codat-bankfeeds-0.6.4.tar` & `codat-bankfeeds-0.8.5.tar`

### file list

```diff
@@ -1,32 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:24:07.730814 codat-bankfeeds-0.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-03-22 17:24:07.730814 codat-bankfeeds-0.6.4/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2460 2023-03-22 17:23:57.000000 codat-bankfeeds-0.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 17:24:07.730814 codat-bankfeeds-0.6.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1108 2023-03-22 17:23:57.000000 codat-bankfeeds-0.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:24:07.722814 codat-bankfeeds-0.6.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:24:07.726814 codat-bankfeeds-0.6.4/src/codat/
--rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-03-22 17:23:57.000000 codat-bankfeeds-0.6.4/src/codat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:24:07.726814 codat-bankfeeds-0.6.4/src/codat/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-03-22 17:23:57.000000 codat-bankfeeds-0.6.4/src/codat/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:24:07.726814 codat-bankfeeds-0.6.4/src/codat/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4442 2023-03-22 17:23:57.000000 codat-bankfeeds-0.6.4/src/codat/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3501 2023-03-22 17:23:57.000000 codat-bankfeeds-0.6.4/src/codat/models/operations/create_bank_feed.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22699 2023-03-22 17:23:57.000000 codat-bankfeeds-0.6.4/src/codat/models/operations/get_bank_account_push_options.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3329 2023-03-22 17:23:57.000000 codat-bankfeeds-0.6.4/src/codat/models/operations/get_bank_feeds.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9085 2023-03-22 17:23:57.000000 codat-bankfeeds-0.6.4/src/codat/models/operations/list_bank_account_transactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17297 2023-03-22 17:23:57.000000 codat-bankfeeds-0.6.4/src/codat/models/operations/post_bank_transactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3676 2023-03-22 17:23:57.000000 codat-bankfeeds-0.6.4/src/codat/models/operations/update_bank_feed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:24:07.730814 codat-bankfeeds-0.6.4/src/codat/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)      124 2023-03-22 17:23:57.000000 codat-bankfeeds-0.6.4/src/codat/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      337 2023-03-22 17:23:57.000000 codat-bankfeeds-0.6.4/src/codat/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10473 2023-03-22 17:23:57.000000 codat-bankfeeds-0.6.4/src/codat/sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:24:07.730814 codat-bankfeeds-0.6.4/src/codat/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-03-22 17:23:57.000000 codat-bankfeeds-0.6.4/src/codat/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-03-22 17:23:57.000000 codat-bankfeeds-0.6.4/src/codat/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24799 2023-03-22 17:23:57.000000 codat-bankfeeds-0.6.4/src/codat/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 17:24:07.730814 codat-bankfeeds-0.6.4/src/codat_bankfeeds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-03-22 17:24:07.000000 codat-bankfeeds-0.6.4/src/codat_bankfeeds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-03-22 17:24:07.000000 codat-bankfeeds-0.6.4/src/codat_bankfeeds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 17:24:07.000000 codat-bankfeeds-0.6.4/src/codat_bankfeeds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-22 17:24:07.000000 codat-bankfeeds-0.6.4/src/codat_bankfeeds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-22 17:24:07.000000 codat-bankfeeds-0.6.4/src/codat_bankfeeds.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:29:36.895137 codat-bankfeeds-0.8.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-04-05 09:29:36.895137 codat-bankfeeds-0.8.5/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2505 2023-04-05 09:29:29.000000 codat-bankfeeds-0.8.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 09:29:36.895137 codat-bankfeeds-0.8.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1108 2023-04-05 09:29:29.000000 codat-bankfeeds-0.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:29:36.891137 codat-bankfeeds-0.8.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:29:36.891137 codat-bankfeeds-0.8.5/src/codat/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-04-05 09:29:29.000000 codat-bankfeeds-0.8.5/src/codat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:29:36.891137 codat-bankfeeds-0.8.5/src/codat/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-05 09:29:29.000000 codat-bankfeeds-0.8.5/src/codat/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:29:36.891137 codat-bankfeeds-0.8.5/src/codat/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      668 2023-04-05 09:29:29.000000 codat-bankfeeds-0.8.5/src/codat/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1138 2023-04-05 09:29:29.000000 codat-bankfeeds-0.8.5/src/codat/models/operations/create_bank_feed.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1829 2023-04-05 09:29:29.000000 codat-bankfeeds-0.8.5/src/codat/models/operations/create_bank_transactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      965 2023-04-05 09:29:29.000000 codat-bankfeeds-0.8.5/src/codat/models/operations/get_bank_feeds.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1137 2023-04-05 09:29:29.000000 codat-bankfeeds-0.8.5/src/codat/models/operations/get_create_bank_account_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2173 2023-04-05 09:29:29.000000 codat-bankfeeds-0.8.5/src/codat/models/operations/list_bank_account_transactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1309 2023-04-05 09:29:29.000000 codat-bankfeeds-0.8.5/src/codat/models/operations/update_bank_feed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:29:36.895137 codat-bankfeeds-0.8.5/src/codat/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1222 2023-04-05 09:29:29.000000 codat-bankfeeds-0.8.5/src/codat/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4290 2023-04-05 09:29:29.000000 codat-bankfeeds-0.8.5/src/codat/models/shared/bankfeedaccount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5068 2023-04-05 09:29:29.000000 codat-bankfeeds-0.8.5/src/codat/models/shared/banktransactionline.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1725 2023-04-05 09:29:29.000000 codat-bankfeeds-0.8.5/src/codat/models/shared/banktransactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1217 2023-04-05 09:29:29.000000 codat-bankfeeds-0.8.5/src/codat/models/shared/banktransactionsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      611 2023-04-05 09:29:29.000000 codat-bankfeeds-0.8.5/src/codat/models/shared/banktransactiontype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6457 2023-04-05 09:29:29.000000 codat-bankfeeds-0.8.5/src/codat/models/shared/createbanktransactionsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1875 2023-04-05 09:29:29.000000 codat-bankfeeds-0.8.5/src/codat/models/shared/datatype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      500 2023-04-05 09:29:29.000000 codat-bankfeeds-0.8.5/src/codat/models/shared/href.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1013 2023-04-05 09:29:29.000000 codat-bankfeeds-0.8.5/src/codat/models/shared/links.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      316 2023-04-05 09:29:29.000000 codat-bankfeeds-0.8.5/src/codat/models/shared/pushchangetype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      809 2023-04-05 09:29:29.000000 codat-bankfeeds-0.8.5/src/codat/models/shared/pushfieldvalidation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1102 2023-04-05 09:29:29.000000 codat-bankfeeds-0.8.5/src/codat/models/shared/pushoperationchange.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      810 2023-04-05 09:29:29.000000 codat-bankfeeds-0.8.5/src/codat/models/shared/pushoperationref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      318 2023-04-05 09:29:29.000000 codat-bankfeeds-0.8.5/src/codat/models/shared/pushoperationstatus_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1909 2023-04-05 09:29:29.000000 codat-bankfeeds-0.8.5/src/codat/models/shared/pushoption.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1389 2023-04-05 09:29:29.000000 codat-bankfeeds-0.8.5/src/codat/models/shared/pushoptionchoice.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1747 2023-04-05 09:29:29.000000 codat-bankfeeds-0.8.5/src/codat/models/shared/pushoptionproperty.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      355 2023-04-05 09:29:29.000000 codat-bankfeeds-0.8.5/src/codat/models/shared/pushoptiontype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      877 2023-04-05 09:29:29.000000 codat-bankfeeds-0.8.5/src/codat/models/shared/pushvalidationinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      337 2023-04-05 09:29:29.000000 codat-bankfeeds-0.8.5/src/codat/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1027 2023-04-05 09:29:29.000000 codat-bankfeeds-0.8.5/src/codat/models/shared/validation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      884 2023-04-05 09:29:29.000000 codat-bankfeeds-0.8.5/src/codat/models/shared/validationitem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10240 2023-04-05 09:29:29.000000 codat-bankfeeds-0.8.5/src/codat/sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:29:36.895137 codat-bankfeeds-0.8.5/src/codat/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-04-05 09:29:29.000000 codat-bankfeeds-0.8.5/src/codat/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-04-05 09:29:29.000000 codat-bankfeeds-0.8.5/src/codat/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24799 2023-04-05 09:29:29.000000 codat-bankfeeds-0.8.5/src/codat/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:29:36.895137 codat-bankfeeds-0.8.5/src/codat_bankfeeds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-04-05 09:29:36.000000 codat-bankfeeds-0.8.5/src/codat_bankfeeds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-05 09:29:36.000000 codat-bankfeeds-0.8.5/src/codat_bankfeeds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 09:29:36.000000 codat-bankfeeds-0.8.5/src/codat_bankfeeds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-05 09:29:36.000000 codat-bankfeeds-0.8.5/src/codat_bankfeeds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-05 09:29:36.000000 codat-bankfeeds-0.8.5/src/codat_bankfeeds.egg-info/top_level.txt
```

### Comparing `codat-bankfeeds-0.6.4/PKG-INFO` & `codat-bankfeeds-0.8.5/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codat-bankfeeds
-Version: 0.6.4
+Version: 0.8.5
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -30,71 +30,71 @@
         auth_header="YOUR_API_KEY_HERE",
     ),
 )
 
 
 req = operations.CreateBankFeedRequest(
     request_body=[
-        operations.CreateBankFeedBankFeedBankAccount(
-            account_name="deserunt",
-            account_number="porro",
-            account_type="nulla",
+        shared.BankFeedAccount(
+            account_name="provident",
+            account_number="distinctio",
+            account_type="quibusdam",
             balance=6027.63,
-            currency="vero",
-            feed_start_date="perspiciatis",
-            id="nulla",
-            modified_date="nihil",
-            sort_code="fuga",
-            status="facilis",
+            currency="nulla",
+            feed_start_date="2022-10-23T00:00:00Z",
+            id="corrupti",
+            modified_date="2022-10-23T00:00:00Z",
+            sort_code="illum",
+            status="vel",
         ),
-        operations.CreateBankFeedBankFeedBankAccount(
-            account_name="eum",
-            account_number="iusto",
-            account_type="ullam",
-            balance=8917.73,
-            currency="inventore",
-            feed_start_date="sapiente",
-            id="enim",
-            modified_date="eum",
-            sort_code="voluptatum",
-            status="autem",
+        shared.BankFeedAccount(
+            account_name="error",
+            account_number="deserunt",
+            account_type="suscipit",
+            balance=4375.87,
+            currency="magnam",
+            feed_start_date="2022-10-23T00:00:00Z",
+            id="debitis",
+            modified_date="2022-10-23T00:00:00Z",
+            sort_code="ipsa",
+            status="delectus",
         ),
-        operations.CreateBankFeedBankFeedBankAccount(
-            account_name="vel",
-            account_number="non",
-            account_type="deleniti",
-            balance=5680.45,
-            currency="reprehenderit",
-            feed_start_date="molestiae",
-            id="quo",
-            modified_date="quasi",
-            sort_code="laboriosam",
-            status="dicta",
+        shared.BankFeedAccount(
+            account_name="tempora",
+            account_number="suscipit",
+            account_type="molestiae",
+            balance=7917.25,
+            currency="placeat",
+            feed_start_date="2022-10-23T00:00:00Z",
+            id="voluptatum",
+            modified_date="2022-10-23T00:00:00Z",
+            sort_code="iusto",
+            status="excepturi",
         ),
     ],
     company_id="8a210b68-6988-11ed-a1eb-0242ac120002",
     connection_id="2e9d2c44-f675-40ba-8049-353bfcb5e171",
 )
     
 res = s.create_bank_feed(req)
 
-if res.bank_feed_bank_accounts is not None:
+if res.bank_feed_accounts is not None:
     # handle response
 ```
 <!-- End SDK Example Usage -->
 
 <!-- Start SDK Available Operations -->
-## SDK Available Operations
+## Available Resources and Operations
 
 ### Codat SDK
 
 * `create_bank_feed` - Create bank feed bank accounts
-* `get_bank_account_push_options` - List push options for bank account bank transactions
+* `create_bank_transactions` - Create bank transactions
 * `get_bank_feeds` - List bank feed bank accounts
+* `get_create_bank_account_model` - List push options for bank account bank transactions
 * `list_bank_account_transactions` - List bank transactions for bank account
-* `post_bank_transactions` - Create bank transactions
 * `update_bank_feed` - Update bank feed bank account
 <!-- End SDK Available Operations -->
 
 ### SDK Generated by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)
```

### Comparing `codat-bankfeeds-0.6.4/README.md` & `codat-bankfeeds-0.8.5/src/codat_bankfeeds.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: codat-bankfeeds
+Version: 0.8.5
+Summary: Python Client SDK Generated by Speakeasy
+Home-page: UNKNOWN
+Author: Speakeasy
+License: UNKNOWN
+Platform: UNKNOWN
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+
 # codat-bankfeeds
 
 <!-- Start SDK Installation -->
 ## SDK Installation
 
 ```bash
 pip install codat-bankfeeds
@@ -19,69 +30,71 @@
         auth_header="YOUR_API_KEY_HERE",
     ),
 )
 
 
 req = operations.CreateBankFeedRequest(
     request_body=[
-        operations.CreateBankFeedBankFeedBankAccount(
-            account_name="deserunt",
-            account_number="porro",
-            account_type="nulla",
+        shared.BankFeedAccount(
+            account_name="provident",
+            account_number="distinctio",
+            account_type="quibusdam",
             balance=6027.63,
-            currency="vero",
-            feed_start_date="perspiciatis",
-            id="nulla",
-            modified_date="nihil",
-            sort_code="fuga",
-            status="facilis",
+            currency="nulla",
+            feed_start_date="2022-10-23T00:00:00Z",
+            id="corrupti",
+            modified_date="2022-10-23T00:00:00Z",
+            sort_code="illum",
+            status="vel",
         ),
-        operations.CreateBankFeedBankFeedBankAccount(
-            account_name="eum",
-            account_number="iusto",
-            account_type="ullam",
-            balance=8917.73,
-            currency="inventore",
-            feed_start_date="sapiente",
-            id="enim",
-            modified_date="eum",
-            sort_code="voluptatum",
-            status="autem",
+        shared.BankFeedAccount(
+            account_name="error",
+            account_number="deserunt",
+            account_type="suscipit",
+            balance=4375.87,
+            currency="magnam",
+            feed_start_date="2022-10-23T00:00:00Z",
+            id="debitis",
+            modified_date="2022-10-23T00:00:00Z",
+            sort_code="ipsa",
+            status="delectus",
         ),
-        operations.CreateBankFeedBankFeedBankAccount(
-            account_name="vel",
-            account_number="non",
-            account_type="deleniti",
-            balance=5680.45,
-            currency="reprehenderit",
-            feed_start_date="molestiae",
-            id="quo",
-            modified_date="quasi",
-            sort_code="laboriosam",
-            status="dicta",
+        shared.BankFeedAccount(
+            account_name="tempora",
+            account_number="suscipit",
+            account_type="molestiae",
+            balance=7917.25,
+            currency="placeat",
+            feed_start_date="2022-10-23T00:00:00Z",
+            id="voluptatum",
+            modified_date="2022-10-23T00:00:00Z",
+            sort_code="iusto",
+            status="excepturi",
         ),
     ],
     company_id="8a210b68-6988-11ed-a1eb-0242ac120002",
     connection_id="2e9d2c44-f675-40ba-8049-353bfcb5e171",
 )
     
 res = s.create_bank_feed(req)
 
-if res.bank_feed_bank_accounts is not None:
+if res.bank_feed_accounts is not None:
     # handle response
 ```
 <!-- End SDK Example Usage -->
 
 <!-- Start SDK Available Operations -->
-## SDK Available Operations
+## Available Resources and Operations
 
 ### Codat SDK
 
 * `create_bank_feed` - Create bank feed bank accounts
-* `get_bank_account_push_options` - List push options for bank account bank transactions
+* `create_bank_transactions` - Create bank transactions
 * `get_bank_feeds` - List bank feed bank accounts
+* `get_create_bank_account_model` - List push options for bank account bank transactions
 * `list_bank_account_transactions` - List bank transactions for bank account
-* `post_bank_transactions` - Create bank transactions
 * `update_bank_feed` - Update bank feed bank account
 <!-- End SDK Available Operations -->
 
 ### SDK Generated by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)
+
+
```

### Comparing `codat-bankfeeds-0.6.4/setup.py` & `codat-bankfeeds-0.8.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="codat-bankfeeds",
-    version="0.6.4",
+    version="0.8.5",
     author="Speakeasy",
     description="Python Client SDK Generated by Speakeasy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi==2022.12.07",
```

### Comparing `codat-bankfeeds-0.6.4/src/codat/models/operations/get_bank_feeds.py` & `codat-bankfeeds-0.8.5/src/codat/models/shared/pushoptionproperty.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,53 +1,24 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-import requests as requests_http
+from ..shared import pushoptionchoice as shared_pushoptionchoice
+from ..shared import pushoptiontype_enum as shared_pushoptiontype_enum
+from ..shared import pushvalidationinfo as shared_pushvalidationinfo
 from codat import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
-@dataclasses.dataclass
-class GetBankFeedsRequest:
-    
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
-    connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})  
-    
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetBankFeedsBankFeedBankAccount:
-    r"""The target bank account in a supported accounting package for ingestion into a bank feed."""
-    
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    r"""Unique ID for the BankFeedBankAccount"""  
-    account_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountName'), 'exclude': lambda f: f is None }})
-    r"""The bank account name"""  
-    account_number: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountNumber'), 'exclude': lambda f: f is None }})
-    r"""The account number"""  
-    account_type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountType'), 'exclude': lambda f: f is None }})
-    r"""The type of bank account e.g. Credit"""  
-    balance: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('balance'), 'exclude': lambda f: f is None }})
-    r"""The latest balance for the bank account"""  
-    currency: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currency'), 'exclude': lambda f: f is None }})
-    r"""The currency e.g. USD"""  
-    feed_start_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('feedStartDate'), 'exclude': lambda f: f is None }})
-    r"""null"""  
-    modified_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedDate'), 'exclude': lambda f: f is None }})
-    r"""The last date the bank account was modified"""  
-    sort_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sortCode'), 'exclude': lambda f: f is None }})
-    r"""The sort code"""  
-    status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
-    r"""null"""  
-    
-
-@dataclasses.dataclass
-class GetBankFeedsResponse:
+class PushOptionProperty:
     
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
-    bank_feed_bank_accounts: Optional[list[GetBankFeedsBankFeedBankAccount]] = dataclasses.field(default=None)
-    r"""Success"""  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
+    description: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description') }})  
+    display_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('displayName') }})  
+    required: bool = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('required') }})  
+    type: shared_pushoptiontype_enum.PushOptionTypeEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})  
+    options: Optional[list[shared_pushoptionchoice.PushOptionChoice]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('options'), 'exclude': lambda f: f is None }})  
+    properties: Optional[dict[str, PushOptionProperty]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('properties'), 'exclude': lambda f: f is None }})  
+    validation: Optional[shared_pushvalidationinfo.PushValidationInfo] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('validation'), 'exclude': lambda f: f is None }})
```

### Comparing `codat-bankfeeds-0.6.4/src/codat/sdk.py` & `codat-bankfeeds-0.8.5/src/codat/sdk.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 class Codat:
     r"""Bank Feeds API enables your SMB users to set up bank feeds from accounts in your application to supported accounting platforms.
     
     A bank feed is a connection between a source bank account—in your application—and a target bank account in a supported accounting package.
     
     [Read more...](https://docs.codat.io/bank-feeds-api/overview)
     
-    [See our OpenAPI spec](https://github.com/codatio/oas) 
+    [See our OpenAPI spec](https://github.com/codatio/oas)
     """
 
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str = SERVERS[0]
     _language: str = "python"
-    _sdk_version: str = "0.6.4"
-    _gen_version: str = "2.13.0"
+    _sdk_version: str = "0.8.5"
+    _gen_version: str = "2.16.7"
 
     def __init__(self,
                  security: shared.Security = None,
                  server_url: str = None,
                  url_params: dict[str, str] = None,
                  client: requests_http.Session = None
                  ) -> None:
@@ -81,40 +81,48 @@
         http_res = client.request('PUT', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.CreateBankFeedResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[list[operations.CreateBankFeedBankFeedBankAccount]])
-                res.bank_feed_bank_accounts = out
+                out = utils.unmarshal_json(http_res.text, Optional[list[shared.BankFeedAccount]])
+                res.bank_feed_accounts = out
 
         return res
 
-    def get_bank_account_push_options(self, request: operations.GetBankAccountPushOptionsRequest) -> operations.GetBankAccountPushOptionsResponse:
-        r"""List push options for bank account bank transactions
-        Gets the options of pushing bank account transactions.
+    def create_bank_transactions(self, request: operations.CreateBankTransactionsRequest) -> operations.CreateBankTransactionsResponse:
+        r"""Create bank transactions
+        Posts bank transactions to the accounting package for a given company.
+        
+        > **Supported Integrations**
+        > 
+        > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=bankTransactions) for integrations that support POST methods.
         """
         base_url = self._server_url
         
-        url = utils.generate_url(operations.GetBankAccountPushOptionsRequest, base_url, '/companies/{companyId}/connections/{connectionId}/options/bankAccounts/{accountId}/bankTransactions', request)
+        url = utils.generate_url(operations.CreateBankTransactionsRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/bankAccounts/{accountId}/bankTransactions', request)
         
-        query_params = utils.get_query_params(operations.GetBankAccountPushOptionsRequest, request)
+        headers = {}
+        req_content_type, data, form = utils.serialize_request_body(request, "bank_transactions", 'json')
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
+        query_params = utils.get_query_params(operations.CreateBankTransactionsRequest, request)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params)
+        http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetBankAccountPushOptionsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.CreateBankTransactionsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetBankAccountPushOptionsPushOption])
-                res.push_option = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.CreateBankTransactionsResponse])
+                res.create_bank_transactions_response = out
 
         return res
 
     def get_bank_feeds(self, request: operations.GetBankFeedsRequest) -> operations.GetBankFeedsResponse:
         r"""List bank feed bank accounts
         Get BankFeed BankAccounts for a single data source connected to a single company.
         """
@@ -128,96 +136,87 @@
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetBankFeedsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[list[operations.GetBankFeedsBankFeedBankAccount]])
-                res.bank_feed_bank_accounts = out
+                out = utils.unmarshal_json(http_res.text, Optional[list[shared.BankFeedAccount]])
+                res.bank_feed_accounts = out
 
         return res
 
-    def list_bank_account_transactions(self, request: operations.ListBankAccountTransactionsRequest) -> operations.ListBankAccountTransactionsResponse:
-        r"""List bank transactions for bank account
-        Gets bank transactions for a given bank account ID
+    def get_create_bank_account_model(self, request: operations.GetCreateBankAccountModelRequest) -> operations.GetCreateBankAccountModelResponse:
+        r"""List push options for bank account bank transactions
+        Gets the options of pushing bank account transactions.
         """
         base_url = self._server_url
         
-        url = utils.generate_url(operations.ListBankAccountTransactionsRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/bankAccounts/{accountId}/bankTransactions', request)
+        url = utils.generate_url(operations.GetCreateBankAccountModelRequest, base_url, '/companies/{companyId}/connections/{connectionId}/options/bankAccounts/{accountId}/bankTransactions', request)
         
-        query_params = utils.get_query_params(operations.ListBankAccountTransactionsRequest, request)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params)
+        http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.ListBankAccountTransactionsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetCreateBankAccountModelResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.ListBankAccountTransactionsLinks])
-                res.links = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.PushOption])
+                res.push_option = out
 
         return res
 
-    def post_bank_transactions(self, request: operations.PostBankTransactionsRequest) -> operations.PostBankTransactionsResponse:
-        r"""Create bank transactions
-        Posts bank transactions to the accounting package for a given company.
-        
-        > **Supported Integrations**
-        > 
-        > Check out our [Knowledge UI](https://knowledge.codat.io/supported-features/accounting?view=tab-by-data-type&dataType=bankTransactions) for integrations that support POST methods.
+    def list_bank_account_transactions(self, request: operations.ListBankAccountTransactionsRequest) -> operations.ListBankAccountTransactionsResponse:
+        r"""List bank transactions for bank account
+        Gets bank transactions for a given bank account ID
         """
         base_url = self._server_url
         
-        url = utils.generate_url(operations.PostBankTransactionsRequest, base_url, '/companies/{companyId}/connections/{connectionId}/push/bankAccounts/{accountId}}/bankTransactions', request)
+        url = utils.generate_url(operations.ListBankAccountTransactionsRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/bankAccounts/{accountId}/bankTransactions', request)
         
-        headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
-        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
-        query_params = utils.get_query_params(operations.PostBankTransactionsRequest, request)
+        query_params = utils.get_query_params(operations.ListBankAccountTransactionsRequest, request)
         
         client = self._security_client
         
-        http_res = client.request('POST', url, params=query_params, data=data, files=form, headers=headers)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.PostBankTransactionsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.ListBankAccountTransactionsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.PostBankTransactions200ApplicationJSON])
-                res.post_bank_transactions_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.BankTransactionsResponse])
+                res.bank_transactions_response = out
 
         return res
 
     def update_bank_feed(self, request: operations.UpdateBankFeedRequest) -> operations.UpdateBankFeedResponse:
         r"""Update bank feed bank account
         Update a single BankFeed BankAccount for a single data source connected to a single company.
         """
         base_url = self._server_url
         
-        url = utils.generate_url(operations.UpdateBankFeedRequest, base_url, '/companies/{companyId}/connections/{connectionId}/connectionInfo/bankFeedAccounts/{bankAccountId}', request)
+        url = utils.generate_url(operations.UpdateBankFeedRequest, base_url, '/companies/{companyId}/connections/{connectionId}/connectionInfo/bankFeedAccounts/{accountId}', request)
         
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, "bank_feed_account", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         
         client = self._security_client
         
         http_res = client.request('PATCH', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.UpdateBankFeedResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.UpdateBankFeedBankFeedBankAccount])
-                res.bank_feed_bank_account = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.BankFeedAccount])
+                res.bank_feed_account = out
 
         return res
```

### Comparing `codat-bankfeeds-0.6.4/src/codat/utils/retries.py` & `codat-bankfeeds-0.8.5/src/codat/utils/retries.py`

 * *Files identical despite different names*

### Comparing `codat-bankfeeds-0.6.4/src/codat/utils/utils.py` & `codat-bankfeeds-0.8.5/src/codat/utils/utils.py`

 * *Files identical despite different names*

### Comparing `codat-bankfeeds-0.6.4/src/codat_bankfeeds.egg-info/PKG-INFO` & `codat-bankfeeds-0.8.5/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: codat-bankfeeds
-Version: 0.6.4
-Summary: Python Client SDK Generated by Speakeasy
-Home-page: UNKNOWN
-Author: Speakeasy
-License: UNKNOWN
-Platform: UNKNOWN
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-
 # codat-bankfeeds
 
 <!-- Start SDK Installation -->
 ## SDK Installation
 
 ```bash
 pip install codat-bankfeeds
@@ -30,71 +19,69 @@
         auth_header="YOUR_API_KEY_HERE",
     ),
 )
 
 
 req = operations.CreateBankFeedRequest(
     request_body=[
-        operations.CreateBankFeedBankFeedBankAccount(
-            account_name="deserunt",
-            account_number="porro",
-            account_type="nulla",
+        shared.BankFeedAccount(
+            account_name="provident",
+            account_number="distinctio",
+            account_type="quibusdam",
             balance=6027.63,
-            currency="vero",
-            feed_start_date="perspiciatis",
-            id="nulla",
-            modified_date="nihil",
-            sort_code="fuga",
-            status="facilis",
+            currency="nulla",
+            feed_start_date="2022-10-23T00:00:00Z",
+            id="corrupti",
+            modified_date="2022-10-23T00:00:00Z",
+            sort_code="illum",
+            status="vel",
         ),
-        operations.CreateBankFeedBankFeedBankAccount(
-            account_name="eum",
-            account_number="iusto",
-            account_type="ullam",
-            balance=8917.73,
-            currency="inventore",
-            feed_start_date="sapiente",
-            id="enim",
-            modified_date="eum",
-            sort_code="voluptatum",
-            status="autem",
+        shared.BankFeedAccount(
+            account_name="error",
+            account_number="deserunt",
+            account_type="suscipit",
+            balance=4375.87,
+            currency="magnam",
+            feed_start_date="2022-10-23T00:00:00Z",
+            id="debitis",
+            modified_date="2022-10-23T00:00:00Z",
+            sort_code="ipsa",
+            status="delectus",
         ),
-        operations.CreateBankFeedBankFeedBankAccount(
-            account_name="vel",
-            account_number="non",
-            account_type="deleniti",
-            balance=5680.45,
-            currency="reprehenderit",
-            feed_start_date="molestiae",
-            id="quo",
-            modified_date="quasi",
-            sort_code="laboriosam",
-            status="dicta",
+        shared.BankFeedAccount(
+            account_name="tempora",
+            account_number="suscipit",
+            account_type="molestiae",
+            balance=7917.25,
+            currency="placeat",
+            feed_start_date="2022-10-23T00:00:00Z",
+            id="voluptatum",
+            modified_date="2022-10-23T00:00:00Z",
+            sort_code="iusto",
+            status="excepturi",
         ),
     ],
     company_id="8a210b68-6988-11ed-a1eb-0242ac120002",
     connection_id="2e9d2c44-f675-40ba-8049-353bfcb5e171",
 )
     
 res = s.create_bank_feed(req)
 
-if res.bank_feed_bank_accounts is not None:
+if res.bank_feed_accounts is not None:
     # handle response
 ```
 <!-- End SDK Example Usage -->
 
 <!-- Start SDK Available Operations -->
-## SDK Available Operations
+## Available Resources and Operations
 
 ### Codat SDK
 
 * `create_bank_feed` - Create bank feed bank accounts
-* `get_bank_account_push_options` - List push options for bank account bank transactions
+* `create_bank_transactions` - Create bank transactions
 * `get_bank_feeds` - List bank feed bank accounts
+* `get_create_bank_account_model` - List push options for bank account bank transactions
 * `list_bank_account_transactions` - List bank transactions for bank account
-* `post_bank_transactions` - Create bank transactions
 * `update_bank_feed` - Update bank feed bank account
 <!-- End SDK Available Operations -->
 
 ### SDK Generated by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)
-
-
```

