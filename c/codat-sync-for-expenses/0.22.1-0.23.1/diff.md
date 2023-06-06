# Comparing `tmp/codat-sync-for-expenses-0.22.1.tar.gz` & `tmp/codat-sync-for-expenses-0.23.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codat-sync-for-expenses-0.22.1.tar", last modified: Thu Jun  1 16:45:57 2023, max compression
+gzip compressed data, was "codat-sync-for-expenses-0.23.1.tar", last modified: Tue Jun  6 20:52:35 2023, max compression
```

## Comparing `codat-sync-for-expenses-0.22.1.tar` & `codat-sync-for-expenses-0.23.1.tar`

### file list

```diff
@@ -1,73 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:45:57.767792 codat-sync-for-expenses-0.22.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-06-01 16:45:57.767792 codat-sync-for-expenses-0.22.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2573 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 16:45:57.767792 codat-sync-for-expenses-0.22.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1186 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:45:57.759792 codat-sync-for-expenses-0.22.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:45:57.763792 codat-sync-for-expenses-0.22.1/src/codat_sync_for_expenses.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-06-01 16:45:57.000000 codat-sync-for-expenses-0.22.1/src/codat_sync_for_expenses.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-06-01 16:45:57.000000 codat-sync-for-expenses-0.22.1/src/codat_sync_for_expenses.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 16:45:57.000000 codat-sync-for-expenses-0.22.1/src/codat_sync_for_expenses.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-01 16:45:57.000000 codat-sync-for-expenses-0.22.1/src/codat_sync_for_expenses.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-01 16:45:57.000000 codat-sync-for-expenses-0.22.1/src/codat_sync_for_expenses.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:45:57.763792 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/
--rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5000 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2858 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/connections.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5291 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/expenses.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2782 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/mapping_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:45:57.763792 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:45:57.763792 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1325 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1266 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/create_expense_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1001 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/create_partner_expense_connection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1032 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/get_company_configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/get_last_successful_sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      998 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/get_latest_sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      990 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/get_mapping_options.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1162 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/get_sync_by_id.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1393 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/get_sync_transaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1224 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/intiate_sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1695 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/list_sync_transactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      998 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/list_syncs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1199 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/save_company_configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1768 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/upload_attachment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:45:57.767792 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1817 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2087 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/accountmappinginfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1024 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/attachment.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      576 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/bankaccount.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5695 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/codaterrormessage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      942 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/companyconfiguration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3075 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/companysyncstatus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      644 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/createexpenserequest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      592 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/createexpenseresponse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      595 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/customer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5368 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/dataconnection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2000 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/dataconnectionerror.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      356 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/dataconnectionstatus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4835 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/expensetransaction.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1324 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/expensetransactionline.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      513 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/hallink.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      304 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/integrationtype.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1714 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/mappingoptions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      533 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/postsync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      575 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/recordref.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1505 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/schema.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      335 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      578 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/supplier.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      568 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/syncinitiated.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2134 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/taxratemappinginfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2413 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1569 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/transactionmetadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2018 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/transactionmetadatalist.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      354 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/transactionstatus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4811 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2994 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8409 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/sync_status.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4884 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/transaction_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:45:57.767792 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26032 2023-06-01 16:45:47.000000 codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:52:35.377539 codat-sync-for-expenses-0.23.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-06-06 20:52:35.377539 codat-sync-for-expenses-0.23.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2573 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 20:52:35.377539 codat-sync-for-expenses-0.23.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1186 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:52:35.369539 codat-sync-for-expenses-0.23.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:52:35.373539 codat-sync-for-expenses-0.23.1/src/codat_sync_for_expenses.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-06-06 20:52:35.000000 codat-sync-for-expenses-0.23.1/src/codat_sync_for_expenses.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-06-06 20:52:35.000000 codat-sync-for-expenses-0.23.1/src/codat_sync_for_expenses.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 20:52:35.000000 codat-sync-for-expenses-0.23.1/src/codat_sync_for_expenses.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-06 20:52:35.000000 codat-sync-for-expenses-0.23.1/src/codat_sync_for_expenses.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-06 20:52:35.000000 codat-sync-for-expenses-0.23.1/src/codat_sync_for_expenses.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:52:35.373539 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      127 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4844 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2586 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/connections.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5135 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/expenses.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2510 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/mapping_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:52:35.373539 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:52:35.373539 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1325 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1266 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/create_expense_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1001 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/create_partner_expense_connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1032 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/get_company_configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1014 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/get_last_successful_sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      998 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/get_latest_sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      990 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/get_mapping_options.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1162 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/get_sync_by_id.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1393 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/get_sync_transaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1224 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/intiate_sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1695 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/list_sync_transactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      998 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/list_syncs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1199 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/save_company_configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1768 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/upload_attachment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:52:35.377539 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1817 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2087 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/accountmappinginfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1024 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/attachment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      576 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/bankaccount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5695 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/codaterrormessage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      942 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/companyconfiguration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3075 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/companysyncstatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      644 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/createexpenserequest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      592 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/createexpenseresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      595 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/customer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5368 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/dataconnection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2000 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/dataconnectionerror.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      356 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/dataconnectionstatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4835 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/expensetransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1324 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/expensetransactionline.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      513 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/hallink.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      304 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/integrationtype.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1714 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/mappingoptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      533 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/postsync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      575 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/recordref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1505 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/schema.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      335 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      578 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/supplier.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      568 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/syncinitiated.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2134 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/taxratemappinginfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2413 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1569 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/transactionmetadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2018 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/transactionmetadatalist.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      354 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/transactionstatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3511 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      734 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/sdkconfiguration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2722 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8485 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/sync_status.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4728 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/transaction_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:52:35.377539 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26032 2023-06-06 20:52:24.000000 codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/utils/utils.py
```

### Comparing `codat-sync-for-expenses-0.22.1/PKG-INFO` & `codat-sync-for-expenses-0.23.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codat-sync-for-expenses
-Version: 0.22.1
+Version: 0.23.1
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `codat-sync-for-expenses-0.22.1/README.md` & `codat-sync-for-expenses-0.23.1/README.md`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.22.1/setup.py` & `codat-sync-for-expenses-0.23.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="codat-sync-for-expenses",
-    version="0.22.1",
+    version="0.23.1",
     author="Speakeasy",
     description="Python Client SDK Generated by Speakeasy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi>=2022.12.7",
```

### Comparing `codat-sync-for-expenses-0.22.1/src/codat_sync_for_expenses.egg-info/PKG-INFO` & `codat-sync-for-expenses-0.23.1/src/codat_sync_for_expenses.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codat-sync-for-expenses
-Version: 0.22.1
+Version: 0.23.1
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `codat-sync-for-expenses-0.22.1/src/codat_sync_for_expenses.egg-info/SOURCES.txt` & `codat-sync-for-expenses-0.23.1/src/codat_sync_for_expenses.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 src/codat_sync_for_expenses.egg-info/top_level.txt
 src/codatsyncexpenses/__init__.py
 src/codatsyncexpenses/configuration.py
 src/codatsyncexpenses/connections.py
 src/codatsyncexpenses/expenses.py
 src/codatsyncexpenses/mapping_options.py
 src/codatsyncexpenses/sdk.py
+src/codatsyncexpenses/sdkconfiguration.py
 src/codatsyncexpenses/sync.py
 src/codatsyncexpenses/sync_status.py
 src/codatsyncexpenses/transaction_status.py
 src/codatsyncexpenses/models/__init__.py
 src/codatsyncexpenses/models/operations/__init__.py
 src/codatsyncexpenses/models/operations/create_expense_dataset.py
 src/codatsyncexpenses/models/operations/create_partner_expense_connection.py
```

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/configuration.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,34 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
-import requests as requests_http
-from . import utils
+from .sdkconfiguration import SDKConfiguration
+from codatsyncexpenses import utils
 from codatsyncexpenses.models import operations, shared
 from typing import Optional
 
 class Configuration:
     r"""Companies sync configuration."""
-    _client: requests_http.Session
-    _security_client: requests_http.Session
-    _server_url: str
-    _language: str
-    _sdk_version: str
-    _gen_version: str
-
-    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
-        self._client = client
-        self._security_client = security_client
-        self._server_url = server_url
-        self._language = language
-        self._sdk_version = sdk_version
-        self._gen_version = gen_version
+    sdk_configuration: SDKConfiguration
+
+    def __init__(self, sdk_config: SDKConfiguration) -> None:
+        self.sdk_configuration = sdk_config
         
     
     def get_company_configuration(self, request: operations.GetCompanyConfigurationRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetCompanyConfigurationResponse:
         r"""Get company configuration
         Gets a companies expense sync configuration
         """
-        base_url = self._server_url
+        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = utils.generate_url(operations.GetCompanyConfigurationRequest, base_url, '/companies/{companyId}/sync/expenses/config', request)
         headers = {}
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version}'
         
-        client = self._security_client
+        client = self.sdk_configuration.security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
             retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
             
 
@@ -66,25 +56,25 @@
         return res
 
     
     def save_company_configuration(self, request: operations.SaveCompanyConfigurationRequest, retries: Optional[utils.RetryConfig] = None) -> operations.SaveCompanyConfigurationResponse:
         r"""Set company configuration
         Sets a companies expense sync configuration
         """
-        base_url = self._server_url
+        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = utils.generate_url(operations.SaveCompanyConfigurationRequest, base_url, '/companies/{companyId}/sync/expenses/config', request)
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "company_configuration", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version}'
         
-        client = self._security_client
+        client = self.sdk_configuration.security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
             retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
```

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/connections.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/connections.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,34 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
-import requests as requests_http
-from . import utils
+from .sdkconfiguration import SDKConfiguration
+from codatsyncexpenses import utils
 from codatsyncexpenses.models import operations, shared
 from typing import Optional
 
 class Connections:
     r"""Create and manage partner expense connection."""
-    _client: requests_http.Session
-    _security_client: requests_http.Session
-    _server_url: str
-    _language: str
-    _sdk_version: str
-    _gen_version: str
+    sdk_configuration: SDKConfiguration
 
-    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
-        self._client = client
-        self._security_client = security_client
-        self._server_url = server_url
-        self._language = language
-        self._sdk_version = sdk_version
-        self._gen_version = gen_version
+    def __init__(self, sdk_config: SDKConfiguration) -> None:
+        self.sdk_configuration = sdk_config
         
     
     def create_partner_expense_connection(self, request: operations.CreatePartnerExpenseConnectionRequest, retries: Optional[utils.RetryConfig] = None) -> operations.CreatePartnerExpenseConnectionResponse:
         r"""Create Partner Expense connection
         Creates a Partner Expense data connection
         """
-        base_url = self._server_url
+        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = utils.generate_url(operations.CreatePartnerExpenseConnectionRequest, base_url, '/companies/{companyId}/sync/expenses/connections/partnerExpense', request)
         headers = {}
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version}'
         
-        client = self._security_client
+        client = self.sdk_configuration.security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
             retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
```

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/expenses.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/expenses.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,47 +1,37 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
-import requests as requests_http
-from . import utils
+from .sdkconfiguration import SDKConfiguration
+from codatsyncexpenses import utils
 from codatsyncexpenses.models import operations, shared
 from typing import Optional
 
 class Expenses:
     r"""Create expense datasets and upload receipts."""
-    _client: requests_http.Session
-    _security_client: requests_http.Session
-    _server_url: str
-    _language: str
-    _sdk_version: str
-    _gen_version: str
-
-    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
-        self._client = client
-        self._security_client = security_client
-        self._server_url = server_url
-        self._language = language
-        self._sdk_version = sdk_version
-        self._gen_version = gen_version
+    sdk_configuration: SDKConfiguration
+
+    def __init__(self, sdk_config: SDKConfiguration) -> None:
+        self.sdk_configuration = sdk_config
         
     
     def create_expense_dataset(self, request: operations.CreateExpenseDatasetRequest, retries: Optional[utils.RetryConfig] = None) -> operations.CreateExpenseDatasetResponse:
         r"""Create expense-transactions
         Create an expense transaction
         """
-        base_url = self._server_url
+        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = utils.generate_url(operations.CreateExpenseDatasetRequest, base_url, '/companies/{companyId}/sync/expenses/data/expense-transactions', request)
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "create_expense_request", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version}'
         
-        client = self._security_client
+        client = self.sdk_configuration.security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
             retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
             
 
@@ -69,25 +59,25 @@
         return res
 
     
     def upload_attachment(self, request: operations.UploadAttachmentRequest, retries: Optional[utils.RetryConfig] = None) -> operations.UploadAttachmentResponse:
         r"""Upload attachment
         Creates an attachment in the accounting software against the given transactionId
         """
-        base_url = self._server_url
+        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = utils.generate_url(operations.UploadAttachmentRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/{syncId}/transactions/{transactionId}/attachments', request)
         headers = {}
         req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'multipart')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version}'
         
-        client = self._security_client
+        client = self.sdk_configuration.security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
             retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
```

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/mapping_options.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/sync.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,68 +1,61 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
-import requests as requests_http
-from . import utils
+from .sdkconfiguration import SDKConfiguration
+from codatsyncexpenses import utils
 from codatsyncexpenses.models import operations, shared
 from typing import Optional
 
-class MappingOptions:
-    r"""Mapping options for a companies expenses."""
-    _client: requests_http.Session
-    _security_client: requests_http.Session
-    _server_url: str
-    _language: str
-    _sdk_version: str
-    _gen_version: str
-
-    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
-        self._client = client
-        self._security_client = security_client
-        self._server_url = server_url
-        self._language = language
-        self._sdk_version = sdk_version
-        self._gen_version = gen_version
+class Sync:
+    r"""Triggering a new sync of expenses to accounting software."""
+    sdk_configuration: SDKConfiguration
+
+    def __init__(self, sdk_config: SDKConfiguration) -> None:
+        self.sdk_configuration = sdk_config
         
     
-    def get_mapping_options(self, request: operations.GetMappingOptionsRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetMappingOptionsResponse:
-        r"""Mapping options
-        Gets the expense mapping options for a companies accounting software
+    def intiate_sync(self, request: operations.IntiateSyncRequest, retries: Optional[utils.RetryConfig] = None) -> operations.IntiateSyncResponse:
+        r"""Initiate sync
+        Initiate sync of pending transactions.
         """
-        base_url = self._server_url
+        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetMappingOptionsRequest, base_url, '/companies/{companyId}/sync/expenses/mappingOptions', request)
+        url = utils.generate_url(operations.IntiateSyncRequest, base_url, '/companies/{companyId}/sync/expenses/syncs', request)
         headers = {}
+        req_content_type, data, form = utils.serialize_request_body(request, "post_sync", 'json')
+        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version}'
         
-        client = self._security_client
+        client = self.sdk_configuration.security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
             retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
             
 
         def do_request():
-            return client.request('GET', url, headers=headers)
+            return client.request('POST', url, data=data, files=form, headers=headers)
         
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetMappingOptionsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.IntiateSyncResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if http_res.status_code == 200:
+        if http_res.status_code == 202:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.MappingOptions])
-                res.mapping_options = out
-        elif http_res.status_code in [401, 404, 429]:
+                out = utils.unmarshal_json(http_res.text, Optional[shared.SyncInitiated])
+                res.sync_initiated = out
+        elif http_res.status_code in [400, 404, 422]:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.Schema])
-                res.schema = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.CodatErrorMessage])
+                res.codat_error_message = out
 
         return res
```

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/__init__.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/create_expense_dataset.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/create_expense_dataset.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/create_partner_expense_connection.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/create_partner_expense_connection.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/get_company_configuration.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/get_company_configuration.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/get_last_successful_sync.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/get_last_successful_sync.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/get_latest_sync.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/get_latest_sync.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/get_mapping_options.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/get_mapping_options.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/get_sync_by_id.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/get_sync_by_id.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/get_sync_transaction.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/get_sync_transaction.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/intiate_sync.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/intiate_sync.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/list_sync_transactions.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/list_sync_transactions.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/list_syncs.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/list_syncs.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/save_company_configuration.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/save_company_configuration.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/operations/upload_attachment.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/operations/upload_attachment.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/__init__.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/accountmappinginfo.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/accountmappinginfo.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/attachment.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/attachment.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/bankaccount.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/bankaccount.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/codaterrormessage.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/codaterrormessage.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/companyconfiguration.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/companyconfiguration.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/companysyncstatus.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/companysyncstatus.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/createexpenserequest.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/createexpenserequest.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/createexpenseresponse.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/createexpenseresponse.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/customer.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/customer.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/dataconnection.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/dataconnection.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/dataconnectionerror.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/dataconnectionerror.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/expensetransaction.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/expensetransaction.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/expensetransactionline.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/expensetransactionline.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/hallink.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/hallink.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/mappingoptions.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/mappingoptions.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/postsync.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/postsync.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/recordref.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/recordref.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/schema.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/schema.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/supplier.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/supplier.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/syncinitiated.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/syncinitiated.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/taxratemappinginfo.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/taxratemappinginfo.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/trackingcategorymappinginfo.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/transactionmetadata.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/transactionmetadata.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/models/shared/transactionmetadatalist.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/models/shared/transactionmetadatalist.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/sync.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/mapping_options.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,71 +1,58 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
-import requests as requests_http
-from . import utils
+from .sdkconfiguration import SDKConfiguration
+from codatsyncexpenses import utils
 from codatsyncexpenses.models import operations, shared
 from typing import Optional
 
-class Sync:
-    r"""Triggering a new sync of expenses to accounting software."""
-    _client: requests_http.Session
-    _security_client: requests_http.Session
-    _server_url: str
-    _language: str
-    _sdk_version: str
-    _gen_version: str
-
-    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
-        self._client = client
-        self._security_client = security_client
-        self._server_url = server_url
-        self._language = language
-        self._sdk_version = sdk_version
-        self._gen_version = gen_version
+class MappingOptions:
+    r"""Mapping options for a companies expenses."""
+    sdk_configuration: SDKConfiguration
+
+    def __init__(self, sdk_config: SDKConfiguration) -> None:
+        self.sdk_configuration = sdk_config
         
     
-    def intiate_sync(self, request: operations.IntiateSyncRequest, retries: Optional[utils.RetryConfig] = None) -> operations.IntiateSyncResponse:
-        r"""Initiate sync
-        Initiate sync of pending transactions.
+    def get_mapping_options(self, request: operations.GetMappingOptionsRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetMappingOptionsResponse:
+        r"""Mapping options
+        Gets the expense mapping options for a companies accounting software
         """
-        base_url = self._server_url
+        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.IntiateSyncRequest, base_url, '/companies/{companyId}/sync/expenses/syncs', request)
+        url = utils.generate_url(operations.GetMappingOptionsRequest, base_url, '/companies/{companyId}/sync/expenses/mappingOptions', request)
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "post_sync", 'json')
-        if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version}'
         
-        client = self._security_client
+        client = self.sdk_configuration.security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
             retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
             
 
         def do_request():
-            return client.request('POST', url, data=data, files=form, headers=headers)
+            return client.request('GET', url, headers=headers)
         
         http_res = utils.retry(do_request, utils.Retries(retry_config, [
             '408',
             '429',
             '5XX'
         ]))
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.IntiateSyncResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetMappingOptionsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
-        if http_res.status_code == 202:
+        if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.SyncInitiated])
-                res.sync_initiated = out
-        elif http_res.status_code in [400, 404, 422]:
+                out = utils.unmarshal_json(http_res.text, Optional[shared.MappingOptions])
+                res.mapping_options = out
+        elif http_res.status_code in [401, 404, 429]:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[shared.CodatErrorMessage])
-                res.codat_error_message = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Schema])
+                res.schema = out
 
         return res
```

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/sync_status.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/sync_status.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,34 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
-import requests as requests_http
-from . import utils
+from .sdkconfiguration import SDKConfiguration
+from codatsyncexpenses import utils
 from codatsyncexpenses.models import operations, shared
 from typing import Optional
 
 class SyncStatus:
     r"""Check the status of ongoing or previous expense syncs."""
-    _client: requests_http.Session
-    _security_client: requests_http.Session
-    _server_url: str
-    _language: str
-    _sdk_version: str
-    _gen_version: str
-
-    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
-        self._client = client
-        self._security_client = security_client
-        self._server_url = server_url
-        self._language = language
-        self._sdk_version = sdk_version
-        self._gen_version = gen_version
+    sdk_configuration: SDKConfiguration
+
+    def __init__(self, sdk_config: SDKConfiguration) -> None:
+        self.sdk_configuration = sdk_config
         
     
     def get_last_successful_sync(self, request: operations.GetLastSuccessfulSyncRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetLastSuccessfulSyncResponse:
         r"""Last successful sync
         Gets the status of the last successfull sync
         """
-        base_url = self._server_url
+        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = utils.generate_url(operations.GetLastSuccessfulSyncRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/lastSuccessful/status', request)
         headers = {}
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version}'
         
-        client = self._security_client
+        client = self.sdk_configuration.security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
             retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
             
 
@@ -66,22 +56,22 @@
         return res
 
     
     def get_latest_sync(self, request: operations.GetLatestSyncRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetLatestSyncResponse:
         r"""Latest sync status
         Gets the latest sync status
         """
-        base_url = self._server_url
+        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = utils.generate_url(operations.GetLatestSyncRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/latest/status', request)
         headers = {}
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version}'
         
-        client = self._security_client
+        client = self.sdk_configuration.security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
             retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
             
 
@@ -109,22 +99,22 @@
         return res
 
     
     def get_sync_by_id(self, request: operations.GetSyncByIDRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetSyncByIDResponse:
         r"""Get Sync status
         Get the sync status for a specified sync
         """
-        base_url = self._server_url
+        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = utils.generate_url(operations.GetSyncByIDRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/{syncId}/status', request)
         headers = {}
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version}'
         
-        client = self._security_client
+        client = self.sdk_configuration.security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
             retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
             
 
@@ -152,22 +142,22 @@
         return res
 
     
     def list_syncs(self, request: operations.ListSyncsRequest, retries: Optional[utils.RetryConfig] = None) -> operations.ListSyncsResponse:
         r"""List sync statuses
         Gets a list of sync statuses
         """
-        base_url = self._server_url
+        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = utils.generate_url(operations.ListSyncsRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/list/status', request)
         headers = {}
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version}'
         
-        client = self._security_client
+        client = self.sdk_configuration.security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
             retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
```

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/transaction_status.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/transaction_status.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,34 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
-import requests as requests_http
-from . import utils
+from .sdkconfiguration import SDKConfiguration
+from codatsyncexpenses import utils
 from codatsyncexpenses.models import operations, shared
 from typing import Optional
 
 class TransactionStatus:
     r"""Retrieve the status of transactions within a sync."""
-    _client: requests_http.Session
-    _security_client: requests_http.Session
-    _server_url: str
-    _language: str
-    _sdk_version: str
-    _gen_version: str
-
-    def __init__(self, client: requests_http.Session, security_client: requests_http.Session, server_url: str, language: str, sdk_version: str, gen_version: str) -> None:
-        self._client = client
-        self._security_client = security_client
-        self._server_url = server_url
-        self._language = language
-        self._sdk_version = sdk_version
-        self._gen_version = gen_version
+    sdk_configuration: SDKConfiguration
+
+    def __init__(self, sdk_config: SDKConfiguration) -> None:
+        self.sdk_configuration = sdk_config
         
     
     def get_sync_transaction(self, request: operations.GetSyncTransactionRequest, retries: Optional[utils.RetryConfig] = None) -> operations.GetSyncTransactionResponse:
         r"""Get Sync Transaction
         Gets the status of a transaction for a sync
         """
-        base_url = self._server_url
+        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = utils.generate_url(operations.GetSyncTransactionRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/{syncId}/transactions/{transactionId}', request)
         headers = {}
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version}'
         
-        client = self._security_client
+        client = self.sdk_configuration.security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
             retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
             
 
@@ -66,23 +56,23 @@
         return res
 
     
     def list_sync_transactions(self, request: operations.ListSyncTransactionsRequest, retries: Optional[utils.RetryConfig] = None) -> operations.ListSyncTransactionsResponse:
         r"""Get Sync transactions
         Get's the transactions and status for a sync
         """
-        base_url = self._server_url
+        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = utils.generate_url(operations.ListSyncTransactionsRequest, base_url, '/companies/{companyId}/sync/expenses/syncs/{syncId}/transactions', request)
         headers = {}
         query_params = utils.get_query_params(operations.ListSyncTransactionsRequest, request)
         headers['Accept'] = 'application/json;q=1, application/json;q=0'
-        headers['user-agent'] = f'speakeasy-sdk/{self._language} {self._sdk_version} {self._gen_version}'
+        headers['user-agent'] = f'speakeasy-sdk/{self.sdk_configuration.language} {self.sdk_configuration.sdk_version} {self.sdk_configuration.gen_version}'
         
-        client = self._security_client
+        client = self.sdk_configuration.security_client
         
         retry_config = retries
         if retry_config is None:
             retry_config = utils.RetryConfig('backoff', True)
             retry_config.backoff = utils.BackoffStrategy(500, 60000, 1.5, 3600000)
```

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/utils/retries.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/utils/retries.py`

 * *Files identical despite different names*

### Comparing `codat-sync-for-expenses-0.22.1/src/codatsyncexpenses/utils/utils.py` & `codat-sync-for-expenses-0.23.1/src/codatsyncexpenses/utils/utils.py`

 * *Files identical despite different names*

