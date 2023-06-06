# Comparing `tmp/codat-banking-0.5.1.tar.gz` & `tmp/codat-banking-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codat-banking-0.5.1.tar", last modified: Fri Mar 17 05:39:38 2023, max compression
+gzip compressed data, was "codat-banking-0.8.4.tar", last modified: Wed Apr  5 09:31:22 2023, max compression
```

## Comparing `codat-banking-0.5.1.tar` & `codat-banking-0.8.4.tar`

### file list

```diff
@@ -1,38 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 05:39:38.866188 codat-banking-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-03-17 05:39:38.866188 codat-banking-0.5.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     1433 2023-03-17 05:39:30.000000 codat-banking-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 05:39:38.866188 codat-banking-0.5.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1030 2023-03-17 05:39:30.000000 codat-banking-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 05:39:38.862188 codat-banking-0.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 05:39:38.862188 codat-banking-0.5.1/src/codat/
--rwxr-xr-x   0 runner    (1001) docker     (123)       19 2023-03-17 05:39:30.000000 codat-banking-0.5.1/src/codat/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1999 2023-03-17 05:39:30.000000 codat-banking-0.5.1/src/codat/account_balances.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3002 2023-03-17 05:39:30.000000 codat-banking-0.5.1/src/codat/accounts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 05:39:38.862188 codat-banking-0.5.1/src/codat/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 05:39:30.000000 codat-banking-0.5.1/src/codat/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 05:39:38.862188 codat-banking-0.5.1/src/codat/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3325 2023-03-17 05:39:30.000000 codat-banking-0.5.1/src/codat/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3129 2023-03-17 05:39:30.000000 codat-banking-0.5.1/src/codat/models/operations/get_bank_transaction_category.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6836 2023-03-17 05:39:30.000000 codat-banking-0.5.1/src/codat/models/operations/get_banking_account.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5291 2023-03-17 05:39:30.000000 codat-banking-0.5.1/src/codat/models/operations/get_banking_transaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6155 2023-03-17 05:39:30.000000 codat-banking-0.5.1/src/codat/models/operations/list_all_banking_transactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6456 2023-03-17 05:39:30.000000 codat-banking-0.5.1/src/codat/models/operations/list_bank_transaction_categories.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6667 2023-03-17 05:39:30.000000 codat-banking-0.5.1/src/codat/models/operations/list_banking_account_balances.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10128 2023-03-17 05:39:30.000000 codat-banking-0.5.1/src/codat/models/operations/list_banking_accounts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6254 2023-03-17 05:39:30.000000 codat-banking-0.5.1/src/codat/models/operations/list_banking_transactions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 05:39:38.862188 codat-banking-0.5.1/src/codat/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)       48 2023-03-17 05:39:30.000000 codat-banking-0.5.1/src/codat/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      254 2023-03-17 05:39:30.000000 codat-banking-0.5.1/src/codat/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3311 2023-03-17 05:39:30.000000 codat-banking-0.5.1/src/codat/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3218 2023-03-17 05:39:30.000000 codat-banking-0.5.1/src/codat/transaction_categories.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4368 2023-03-17 05:39:30.000000 codat-banking-0.5.1/src/codat/transactions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 05:39:38.866188 codat-banking-0.5.1/src/codat/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-03-17 05:39:30.000000 codat-banking-0.5.1/src/codat/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3629 2023-03-17 05:39:30.000000 codat-banking-0.5.1/src/codat/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24723 2023-03-17 05:39:30.000000 codat-banking-0.5.1/src/codat/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 05:39:38.866188 codat-banking-0.5.1/src/codat_banking.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-03-17 05:39:38.000000 codat-banking-0.5.1/src/codat_banking.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-03-17 05:39:38.000000 codat-banking-0.5.1/src/codat_banking.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 05:39:38.000000 codat-banking-0.5.1/src/codat_banking.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-17 05:39:38.000000 codat-banking-0.5.1/src/codat_banking.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-17 05:39:38.000000 codat-banking-0.5.1/src/codat_banking.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:31:22.634432 codat-banking-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-05 09:31:22.634432 codat-banking-0.8.4/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1433 2023-04-05 09:31:14.000000 codat-banking-0.8.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 09:31:22.634432 codat-banking-0.8.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1106 2023-04-05 09:31:14.000000 codat-banking-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:31:22.630432 codat-banking-0.8.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:31:22.630432 codat-banking-0.8.4/src/codat/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-04-05 09:31:14.000000 codat-banking-0.8.4/src/codat/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2133 2023-04-05 09:31:14.000000 codat-banking-0.8.4/src/codat/account_balances.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3011 2023-04-05 09:31:14.000000 codat-banking-0.8.4/src/codat/accounts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:31:22.630432 codat-banking-0.8.4/src/codat/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-05 09:31:14.000000 codat-banking-0.8.4/src/codat/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:31:22.630432 codat-banking-0.8.4/src/codat/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      811 2023-04-05 09:31:14.000000 codat-banking-0.8.4/src/codat/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1091 2023-04-05 09:31:14.000000 codat-banking-0.8.4/src/codat/models/operations/get_account.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1134 2023-04-05 09:31:14.000000 codat-banking-0.8.4/src/codat/models/operations/get_transaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1225 2023-04-05 09:31:14.000000 codat-banking-0.8.4/src/codat/models/operations/get_transaction_category.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1932 2023-04-05 09:31:14.000000 codat-banking-0.8.4/src/codat/models/operations/list_account_balances.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1882 2023-04-05 09:31:14.000000 codat-banking-0.8.4/src/codat/models/operations/list_accounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1777 2023-04-05 09:31:14.000000 codat-banking-0.8.4/src/codat/models/operations/list_bank_transactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1974 2023-04-05 09:31:14.000000 codat-banking-0.8.4/src/codat/models/operations/list_transaction_categories.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1910 2023-04-05 09:31:14.000000 codat-banking-0.8.4/src/codat/models/operations/list_transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:31:22.630432 codat-banking-0.8.4/src/codat/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1036 2023-04-05 09:31:14.000000 codat-banking-0.8.4/src/codat/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5520 2023-04-05 09:31:14.000000 codat-banking-0.8.4/src/codat/models/shared/account.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4808 2023-04-05 09:31:14.000000 codat-banking-0.8.4/src/codat/models/shared/accountbalance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1344 2023-04-05 09:31:14.000000 codat-banking-0.8.4/src/codat/models/shared/accountbalanceamounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1200 2023-04-05 09:31:14.000000 codat-banking-0.8.4/src/codat/models/shared/accountbalances.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2500 2023-04-05 09:31:14.000000 codat-banking-0.8.4/src/codat/models/shared/accountidentifiers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-04-05 09:31:14.000000 codat-banking-0.8.4/src/codat/models/shared/accountidentifiertype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      889 2023-04-05 09:31:14.000000 codat-banking-0.8.4/src/codat/models/shared/accountinstitution.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1165 2023-04-05 09:31:14.000000 codat-banking-0.8.4/src/codat/models/shared/accounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      517 2023-04-05 09:31:14.000000 codat-banking-0.8.4/src/codat/models/shared/accounttype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      500 2023-04-05 09:31:14.000000 codat-banking-0.8.4/src/codat/models/shared/href.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1013 2023-04-05 09:31:14.000000 codat-banking-0.8.4/src/codat/models/shared/links.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      337 2023-04-05 09:31:14.000000 codat-banking-0.8.4/src/codat/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7113 2023-04-05 09:31:14.000000 codat-banking-0.8.4/src/codat/models/shared/transaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1226 2023-04-05 09:31:14.000000 codat-banking-0.8.4/src/codat/models/shared/transactioncategories.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3838 2023-04-05 09:31:14.000000 codat-banking-0.8.4/src/codat/models/shared/transactioncategory.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      831 2023-04-05 09:31:14.000000 codat-banking-0.8.4/src/codat/models/shared/transactioncategoryref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      254 2023-04-05 09:31:14.000000 codat-banking-0.8.4/src/codat/models/shared/transactioncategorystatus_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      613 2023-04-05 09:31:14.000000 codat-banking-0.8.4/src/codat/models/shared/transactioncode_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1185 2023-04-05 09:31:14.000000 codat-banking-0.8.4/src/codat/models/shared/transactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4033 2023-04-05 09:31:14.000000 codat-banking-0.8.4/src/codat/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3330 2023-04-05 09:31:14.000000 codat-banking-0.8.4/src/codat/transaction_categories.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4184 2023-04-05 09:31:14.000000 codat-banking-0.8.4/src/codat/transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:31:22.630432 codat-banking-0.8.4/src/codat/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-04-05 09:31:14.000000 codat-banking-0.8.4/src/codat/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-04-05 09:31:14.000000 codat-banking-0.8.4/src/codat/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24799 2023-04-05 09:31:14.000000 codat-banking-0.8.4/src/codat/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:31:22.630432 codat-banking-0.8.4/src/codat_banking.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-05 09:31:22.000000 codat-banking-0.8.4/src/codat_banking.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-05 09:31:22.000000 codat-banking-0.8.4/src/codat_banking.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 09:31:22.000000 codat-banking-0.8.4/src/codat_banking.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-05 09:31:22.000000 codat-banking-0.8.4/src/codat_banking.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-05 09:31:22.000000 codat-banking-0.8.4/src/codat_banking.egg-info/top_level.txt
```

### Comparing `codat-banking-0.5.1/PKG-INFO` & `codat-banking-0.8.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: codat-banking
-Version: 0.5.1
-Summary: Python Client SDK Generated by Speakeasy
-Home-page: UNKNOWN
-Author: Speakeasy
-License: UNKNOWN
-Platform: UNKNOWN
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-
 # codat-banking
 
 <!-- Start SDK Installation -->
 ## SDK Installation
 
 ```bash
 pip install codat-banking
@@ -28,51 +17,49 @@
 s = codat.Codat(
     security=shared.Security(
         auth_header="YOUR_API_KEY_HERE",
     ),
 )
 
 
-req = operations.ListBankingAccountBalancesRequest(
-    company_id="unde",
-    connection_id="deserunt",
-    order_by="porro",
-    page=844266,
-    page_size=602763,
-    query="vero",
+req = operations.ListAccountBalancesRequest(
+    company_id="8a210b68-6988-11ed-a1eb-0242ac120002",
+    connection_id="2e9d2c44-f675-40ba-8049-353bfcb5e171",
+    order_by="-modifiedDate",
+    page=1,
+    page_size=100,
+    query="corrupti",
 )
     
-res = s.account_balances.list_banking_account_balances(req)
+res = s.account_balances.list_account_balances(req)
 
-if res.links is not None:
+if res.account_balances is not None:
     # handle response
 ```
 <!-- End SDK Example Usage -->
 
 <!-- Start SDK Available Operations -->
-## SDK Available Operations
+## Available Resources and Operations
 
 
 ### account_balances
 
-* `list_banking_account_balances` - List account balances
+* `list_account_balances` - List account balances
 
 ### accounts
 
-* `get_banking_account` - Get account
-* `list_banking_accounts` - List accounts
+* `get_account` - Get account
+* `list_accounts` - List accounts
 
 ### transaction_categories
 
-* `get_bank_transaction_category` - Get transaction category
-* `list_bank_transaction_categories` - List all transaction categories
+* `get_transaction_category` - Get transaction category
+* `list_transaction_categories` - List all transaction categories
 
 ### transactions
 
-* `get_banking_transaction` - Get bank transaction
-* `list_all_banking_transactions` - List banking transactions
-* `list_banking_transactions` - List bank account transactions
+* `get_transaction` - Get bank transaction
+* `list_bank_transactions` - List banking transactions
+* `list_transactions` - List transactions
 <!-- End SDK Available Operations -->
 
 ### SDK Generated by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)
-
-
```

### Comparing `codat-banking-0.5.1/src/codat/account_balances.py` & `codat-banking-0.8.4/src/codat/account_balances.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
-from codat.models import operations
+from codat.models import operations, shared
 from typing import Optional
 
 class AccountBalances:
+    r"""Balances for a bank account including end-of-day batch balance or running balances per transaction."""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -15,33 +18,32 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    def list_banking_account_balances(self, request: operations.ListBankingAccountBalancesRequest) -> operations.ListBankingAccountBalancesResponse:
+    def list_account_balances(self, request: operations.ListAccountBalancesRequest) -> operations.ListAccountBalancesResponse:
         r"""List account balances
         Gets a list of balances for a bank account including end-of-day batch balance or running balances per transaction.
         """
-        
         base_url = self._server_url
         
-        url = utils.generate_url(operations.ListBankingAccountBalancesRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/banking-accountBalances', request)
+        url = utils.generate_url(operations.ListAccountBalancesRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/banking-accountBalances', request)
         
-        query_params = utils.get_query_params(operations.ListBankingAccountBalancesRequest, request)
+        query_params = utils.get_query_params(operations.ListAccountBalancesRequest, request)
         
         client = self._security_client
         
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.ListBankingAccountBalancesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.ListAccountBalancesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.ListBankingAccountBalancesLinks])
-                res.links = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.AccountBalances])
+                res.account_balances = out
 
         return res
```

### Comparing `codat-banking-0.5.1/src/codat/models/operations/get_bank_transaction_category.py` & `codat-banking-0.8.4/src/codat/models/operations/list_transactions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,33 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
-import dateutil.parser
 import requests as requests_http
-from codat import utils
-from dataclasses_json import Undefined, dataclass_json
-from datetime import datetime
-from enum import Enum
-from marshmallow import fields
+from ..shared import transactions as shared_transactions
 from typing import Optional
 
 
 @dataclasses.dataclass
-class GetBankTransactionCategoryRequest:
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})
-    transaction_category_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'transactionCategoryId', 'style': 'simple', 'explode': False }})
-    
-class GetBankTransactionCategorySourceModifiedDateStatusEnum(str, Enum):
-    UNKNOWN = "Unknown"
-    ACTIVE = "Active"
-    ARCHIVED = "Archived"
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetBankTransactionCategorySourceModifiedDate:
-    r"""GetBankTransactionCategorySourceModifiedDate
-    The Banking Transaction Categories data type provides a list of hierarchical categories associated with a transaction for greater contextual meaning to transaction activity.
-    """
+class ListTransactionsRequest:
     
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
-    has_children: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('hasChildren'), 'exclude': lambda f: f is None }})
-    modified_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    parent_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('parentId'), 'exclude': lambda f: f is None }})
-    source_modified_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceModifiedDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    status: Optional[GetBankTransactionCategorySourceModifiedDateStatusEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
+    connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})  
+    page: int = dataclasses.field(metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
+    r"""Page number. [Read more](https://docs.codat.io/using-the-api/paging)."""  
+    order_by: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'orderBy', 'style': 'form', 'explode': True }})
+    r"""Field to order results by. [Read more](https://docs.codat.io/using-the-api/ordering-results)."""  
+    page_size: Optional[int] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'pageSize', 'style': 'form', 'explode': True }})
+    r"""Number of records to return in a page. [Read more](https://docs.codat.io/using-the-api/paging)."""  
+    query: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'query', 'style': 'form', 'explode': True }})
+    r"""Codat query string. [Read more](https://docs.codat.io/using-the-api/querying)."""  
     
 
 @dataclasses.dataclass
-class GetBankTransactionCategoryResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    source_modified_date: Optional[GetBankTransactionCategorySourceModifiedDate] = dataclasses.field(default=None)
+class ListTransactionsResponse:
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
+    transactions: Optional[shared_transactions.Transactions] = dataclasses.field(default=None)
+    r"""Success"""
```

### Comparing `codat-banking-0.5.1/src/codat/transaction_categories.py` & `codat-banking-0.8.4/src/codat/transaction_categories.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
-from codat.models import operations
+from codat.models import operations, shared
 from typing import Optional
 
 class TransactionCategories:
+    r"""Hierarchical categories associated with a transaction for greater contextual meaning to transaction activity."""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -15,57 +18,55 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    def get_bank_transaction_category(self, request: operations.GetBankTransactionCategoryRequest) -> operations.GetBankTransactionCategoryResponse:
+    def get_transaction_category(self, request: operations.GetTransactionCategoryRequest) -> operations.GetTransactionCategoryResponse:
         r"""Get transaction category
         Gets a specified bank transaction category for a given company
         """
-        
         base_url = self._server_url
         
-        url = utils.generate_url(operations.GetBankTransactionCategoryRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/banking-transactionCategories/{transactionCategoryId}', request)
+        url = utils.generate_url(operations.GetTransactionCategoryRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/banking-transactionCategories/{transactionCategoryId}', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetBankTransactionCategoryResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetTransactionCategoryResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetBankTransactionCategorySourceModifiedDate])
-                res.source_modified_date = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.TransactionCategory])
+                res.transaction_category = out
 
         return res
 
-    def list_bank_transaction_categories(self, request: operations.ListBankTransactionCategoriesRequest) -> operations.ListBankTransactionCategoriesResponse:
+    def list_transaction_categories(self, request: operations.ListTransactionCategoriesRequest) -> operations.ListTransactionCategoriesResponse:
         r"""List all transaction categories
         Gets a list of hierarchical categories associated with a transaction for greater contextual meaning to transactionactivity.
         """
-        
         base_url = self._server_url
         
-        url = utils.generate_url(operations.ListBankTransactionCategoriesRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/banking-transactionCategories', request)
+        url = utils.generate_url(operations.ListTransactionCategoriesRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/banking-transactionCategories', request)
         
-        query_params = utils.get_query_params(operations.ListBankTransactionCategoriesRequest, request)
+        query_params = utils.get_query_params(operations.ListTransactionCategoriesRequest, request)
         
         client = self._security_client
         
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.ListBankTransactionCategoriesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.ListTransactionCategoriesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.ListBankTransactionCategoriesLinks])
-                res.links = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.TransactionCategories])
+                res.transaction_categories = out
 
         return res
```

### Comparing `codat-banking-0.5.1/src/codat/transactions.py` & `codat-banking-0.8.4/src/codat/transactions.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
-from codat.models import operations
+from codat.models import operations, shared
 from typing import Optional
 
 class Transactions:
+    r"""An immutable source of up-to-date information on income and expenditure."""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -15,82 +18,79 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    def get_banking_transaction(self, request: operations.GetBankingTransactionRequest) -> operations.GetBankingTransactionResponse:
+    def get_transaction(self, request: operations.GetTransactionRequest) -> operations.GetTransactionResponse:
         r"""Get bank transaction
         Gets a specified bank transaction for a given company
         """
-        
         base_url = self._server_url
         
-        url = utils.generate_url(operations.GetBankingTransactionRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/banking-transactions/{transactionId}', request)
+        url = utils.generate_url(operations.GetTransactionRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/banking-transactions/{transactionId}', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetBankingTransactionResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetTransactionResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetBankingTransactionSourceModifiedDate])
-                res.source_modified_date = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Transaction])
+                res.transaction = out
 
         return res
 
-    def list_all_banking_transactions(self, request: operations.ListAllBankingTransactionsRequest) -> operations.ListAllBankingTransactionsResponse:
+    def list_bank_transactions(self, request: operations.ListBankTransactionsRequest) -> operations.ListBankTransactionsResponse:
         r"""List banking transactions
         Gets a list of transactions incurred by a company across all bank accounts.
         """
-        
         base_url = self._server_url
         
-        url = utils.generate_url(operations.ListAllBankingTransactionsRequest, base_url, '/companies/{companyId}/data/banking-transactions', request)
+        url = utils.generate_url(operations.ListBankTransactionsRequest, base_url, '/companies/{companyId}/data/banking-transactions', request)
         
-        query_params = utils.get_query_params(operations.ListAllBankingTransactionsRequest, request)
+        query_params = utils.get_query_params(operations.ListBankTransactionsRequest, request)
         
         client = self._security_client
         
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.ListAllBankingTransactionsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.ListBankTransactionsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.ListAllBankingTransactions200ApplicationJSON])
-                res.list_all_banking_transactions_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Transactions])
+                res.transactions = out
 
         return res
 
-    def list_banking_transactions(self, request: operations.ListBankingTransactionsRequest) -> operations.ListBankingTransactionsResponse:
-        r"""List bank account transactions
+    def list_transactions(self, request: operations.ListTransactionsRequest) -> operations.ListTransactionsResponse:
+        r"""List transactions
         Gets a list of transactions incurred by a bank account.
         """
-        
         base_url = self._server_url
         
-        url = utils.generate_url(operations.ListBankingTransactionsRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/banking-transactions', request)
+        url = utils.generate_url(operations.ListTransactionsRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/banking-transactions', request)
         
-        query_params = utils.get_query_params(operations.ListBankingTransactionsRequest, request)
+        query_params = utils.get_query_params(operations.ListTransactionsRequest, request)
         
         client = self._security_client
         
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.ListBankingTransactionsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.ListTransactionsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.ListBankingTransactions200ApplicationJSON])
-                res.list_banking_transactions_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Transactions])
+                res.transactions = out
 
         return res
```

### Comparing `codat-banking-0.5.1/src/codat/utils/retries.py` & `codat-banking-0.8.4/src/codat/utils/retries.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import random
 import time
 
 import requests
 
 
 class BackoffStrategy:
```

### Comparing `codat-banking-0.5.1/src/codat/utils/utils.py` & `codat-banking-0.8.4/src/codat/utils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import base64
 import json
 import re
 from dataclasses import Field, dataclass, fields, is_dataclass, make_dataclass
 from datetime import date, datetime
 from email.message import Message
 from enum import Enum
```

