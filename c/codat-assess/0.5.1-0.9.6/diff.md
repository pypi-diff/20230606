# Comparing `tmp/codat-assess-0.5.1.tar.gz` & `tmp/codat-assess-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codat-assess-0.5.1.tar", last modified: Fri Mar 17 05:39:19 2023, max compression
+gzip compressed data, was "codat-assess-0.9.6.tar", last modified: Wed Apr  5 09:30:06 2023, max compression
```

## Comparing `codat-assess-0.5.1.tar` & `codat-assess-0.9.6.tar`

### file list

```diff
@@ -1,58 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 05:39:19.273157 codat-assess-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-03-17 05:39:19.273157 codat-assess-0.5.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2788 2023-03-17 05:39:09.000000 codat-assess-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 05:39:19.273157 codat-assess-0.5.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1029 2023-03-17 05:39:09.000000 codat-assess-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 05:39:19.265157 codat-assess-0.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 05:39:19.265157 codat-assess-0.5.1/src/codat/
--rwxr-xr-x   0 runner    (1001) docker     (123)       19 2023-03-17 05:39:09.000000 codat-assess-0.5.1/src/codat/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7025 2023-03-17 05:39:09.000000 codat-assess-0.5.1/src/codat/categories.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4460 2023-03-17 05:39:09.000000 codat-assess-0.5.1/src/codat/data_integrity.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5678 2023-03-17 05:39:09.000000 codat-assess-0.5.1/src/codat/excel_reports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 05:39:19.265157 codat-assess-0.5.1/src/codat/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 05:39:09.000000 codat-assess-0.5.1/src/codat/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 05:39:19.269157 codat-assess-0.5.1/src/codat/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)    23389 2023-03-17 05:39:09.000000 codat-assess-0.5.1/src/codat/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3434 2023-03-17 05:39:09.000000 codat-assess-0.5.1/src/codat/models/operations/get_account_category.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19323 2023-03-17 05:39:09.000000 codat-assess-0.5.1/src/codat/models/operations/get_accounting_marketing_metrics.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5107 2023-03-17 05:39:09.000000 codat-assess-0.5.1/src/codat/models/operations/get_accounts_for_enhanced_balance_sheet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5119 2023-03-17 05:39:09.000000 codat-assess-0.5.1/src/codat/models/operations/get_accounts_for_enhanced_profit_and_loss.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19383 2023-03-17 05:39:09.000000 codat-assess-0.5.1/src/codat/models/operations/get_commerce_customer_retention_metrics.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19231 2023-03-17 05:39:09.000000 codat-assess-0.5.1/src/codat/models/operations/get_commerce_lifetime_value_metrics.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18964 2023-03-17 05:39:09.000000 codat-assess-0.5.1/src/codat/models/operations/get_commerce_orders_metrics.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19002 2023-03-17 05:39:09.000000 codat-assess-0.5.1/src/codat/models/operations/get_commerce_refunds_metrics.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19002 2023-03-17 05:39:09.000000 codat-assess-0.5.1/src/codat/models/operations/get_commerce_revenue_metrics.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7710 2023-03-17 05:39:09.000000 codat-assess-0.5.1/src/codat/models/operations/get_data_integrity_details.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6950 2023-03-17 05:39:09.000000 codat-assess-0.5.1/src/codat/models/operations/get_data_integrity_status.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4454 2023-03-17 05:39:09.000000 codat-assess-0.5.1/src/codat/models/operations/get_data_integrity_summaries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18608 2023-03-17 05:39:09.000000 codat-assess-0.5.1/src/codat/models/operations/get_enhanced_balance_sheet.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8850 2023-03-17 05:39:09.000000 codat-assess-0.5.1/src/codat/models/operations/get_enhanced_cash_flow_transactions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11938 2023-03-17 05:39:09.000000 codat-assess-0.5.1/src/codat/models/operations/get_enhanced_financial_metrics.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18645 2023-03-17 05:39:09.000000 codat-assess-0.5.1/src/codat/models/operations/get_enhanced_profit_and_loss.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      845 2023-03-17 05:39:09.000000 codat-assess-0.5.1/src/codat/models/operations/get_excel_report.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18125 2023-03-17 05:39:09.000000 codat-assess-0.5.1/src/codat/models/operations/get_recurring_revenue_metrics.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6736 2023-03-17 05:39:09.000000 codat-assess-0.5.1/src/codat/models/operations/list_accounts_categories.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1891 2023-03-17 05:39:09.000000 codat-assess-0.5.1/src/codat/models/operations/list_available_account_categories.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2914 2023-03-17 05:39:09.000000 codat-assess-0.5.1/src/codat/models/operations/make_request_to_download_excel_report.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2892 2023-03-17 05:39:09.000000 codat-assess-0.5.1/src/codat/models/operations/request_excel_report_for_download.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18269 2023-03-17 05:39:09.000000 codat-assess-0.5.1/src/codat/models/operations/request_recurring_revenue_metrics.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4573 2023-03-17 05:39:09.000000 codat-assess-0.5.1/src/codat/models/operations/update_account_category.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4667 2023-03-17 05:39:09.000000 codat-assess-0.5.1/src/codat/models/operations/update_accounts_categories.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 05:39:19.269157 codat-assess-0.5.1/src/codat/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)       48 2023-03-17 05:39:09.000000 codat-assess-0.5.1/src/codat/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      254 2023-03-17 05:39:09.000000 codat-assess-0.5.1/src/codat/models/shared/security.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 05:39:19.269157 codat-assess-0.5.1/src/codat/models/webhooks/
--rwxr-xr-x   0 runner    (1001) docker     (123)      210 2023-03-17 05:39:09.000000 codat-assess-0.5.1/src/codat/models/webhooks/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2917 2023-03-17 05:39:09.000000 codat-assess-0.5.1/src/codat/models/webhooks/account_categories_updated.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17955 2023-03-17 05:39:09.000000 codat-assess-0.5.1/src/codat/reports.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3063 2023-03-17 05:39:09.000000 codat-assess-0.5.1/src/codat/sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 05:39:19.269157 codat-assess-0.5.1/src/codat/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)       44 2023-03-17 05:39:09.000000 codat-assess-0.5.1/src/codat/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3629 2023-03-17 05:39:09.000000 codat-assess-0.5.1/src/codat/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24723 2023-03-17 05:39:09.000000 codat-assess-0.5.1/src/codat/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 05:39:19.269157 codat-assess-0.5.1/src/codat_assess.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-03-17 05:39:19.000000 codat-assess-0.5.1/src/codat_assess.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-03-17 05:39:19.000000 codat-assess-0.5.1/src/codat_assess.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 05:39:19.000000 codat-assess-0.5.1/src/codat_assess.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-17 05:39:19.000000 codat-assess-0.5.1/src/codat_assess.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-17 05:39:19.000000 codat-assess-0.5.1/src/codat_assess.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:30:06.490206 codat-assess-0.9.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-04-05 09:30:06.490206 codat-assess-0.9.6/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2943 2023-04-05 09:29:55.000000 codat-assess-0.9.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 09:30:06.490206 codat-assess-0.9.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1105 2023-04-05 09:29:55.000000 codat-assess-0.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:30:06.478206 codat-assess-0.9.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:30:06.482206 codat-assess-0.9.6/src/codat/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6926 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/categories.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4363 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/data_integrity.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6490 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/excel_reports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:30:06.482206 codat-assess-0.9.6/src/codat/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:30:06.482206 codat-assess-0.9.6/src/codat/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3205 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1020 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/operations/download_excel_report.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1122 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/operations/generate_excel_report.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1144 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/operations/get_account_category.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2585 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/operations/get_accounting_marketing_metrics.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1451 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/operations/get_accounts_for_enhanced_balance_sheet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1453 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/operations/get_accounts_for_enhanced_profit_and_loss.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2336 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/operations/get_commerce_customer_retention_metrics.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2328 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/operations/get_commerce_lifetime_value_metrics.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2314 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/operations/get_commerce_orders_metrics.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2316 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/operations/get_commerce_refunds_metrics.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2316 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/operations/get_commerce_revenue_metrics.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2067 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/operations/get_data_integrity_details.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1099 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/operations/get_data_integrity_status.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1358 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/operations/get_data_integrity_summaries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2035 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/operations/get_enhanced_balance_sheet.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1619 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/operations/get_enhanced_cash_flow_transactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2064 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/operations/get_enhanced_financial_metrics.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1576 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/operations/get_enhanced_invoices_report.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2037 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/operations/get_enhanced_profit_and_loss.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1010 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/operations/get_excel_report.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1144 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/operations/get_excel_report_generation_status.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      934 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/operations/get_recurring_revenue_metrics.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1953 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/operations/list_accounts_categories.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      613 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/operations/list_available_account_categories.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      942 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/operations/request_recurring_revenue_metrics.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1380 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/operations/update_account_category.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1238 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/operations/update_accounts_categories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:30:06.490206 codat-assess-0.9.6/src/codat/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3713 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2858 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/accountcategoriesupdatedwebhook.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      993 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/accountcategory.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2096 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/accountcategorydeprecated.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      927 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/accountcategorylevel.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      822 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/accountref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2527 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/accounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1782 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/categories.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1232 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/categorisedaccount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1277 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/categorisedaccounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1537 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/confirmcategories.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      535 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/confirmcategory.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      733 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/customerref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1462 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/dataintegrityamounts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2079 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/dataintegritybyamount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1405 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/dataintegritybycount.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      881 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/dataintegrityconnectionid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      394 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/dataintegritydatatype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4804 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/dataintegritydates.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3448 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/dataintegritydetails.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2514 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/dataintegritymatch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2175 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/dataintegritystatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2073 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/dataintegritystatusinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1384 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/dataintegritysummary.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      766 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/datasource.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1211 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/details.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      725 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/enhancedcashflowitem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2944 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/enhancedcashflowtransaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1289 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/enhancedcashflowtransactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6787 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/enhancedinvoicereportitem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1559 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/enhancedinvoicesreport.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3138 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/enhancedreport.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      985 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/enhancedreportaccountcategory.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2485 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/enhancedreportinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      304 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/excelreporttype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2738 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/excelstatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6831 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/financialmetric.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      960 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/financialmetricerror.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1938 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/financialmetrics.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      502 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/halref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      353 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/integritystatus_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1236 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/invoicestatus_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1033 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/links.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33446 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/payment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1878 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/paymentline.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3539 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/paymentlinelink.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      901 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/paymentlinktype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      284 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/periodunit_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3056 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/report.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1609 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/reportcomponent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      898 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/reportcomponentmeasure.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1350 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/reportdimension.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      880 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/reporterror.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1865 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/reportinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1044 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/reportmeasure.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      337 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      598 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/sourceref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      644 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/status.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      653 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/summaries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      866 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/shared/transactioncategory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:30:06.490206 codat-assess-0.9.6/src/codat/models/webhooks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      166 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/webhooks/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      443 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/models/webhooks/account_categories_updated.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18791 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/reports.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3577 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:30:06.490206 codat-assess-0.9.6/src/codat/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24799 2023-04-05 09:29:55.000000 codat-assess-0.9.6/src/codat/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:30:06.490206 codat-assess-0.9.6/src/codat_assess.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-04-05 09:30:06.000000 codat-assess-0.9.6/src/codat_assess.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-04-05 09:30:06.000000 codat-assess-0.9.6/src/codat_assess.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 09:30:06.000000 codat-assess-0.9.6/src/codat_assess.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-05 09:30:06.000000 codat-assess-0.9.6/src/codat_assess.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-05 09:30:06.000000 codat-assess-0.9.6/src/codat_assess.egg-info/top_level.txt
```

### Comparing `codat-assess-0.5.1/PKG-INFO` & `codat-assess-0.9.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codat-assess
-Version: 0.5.1
+Version: 0.9.6
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -29,28 +29,28 @@
     security=shared.Security(
         auth_header="YOUR_API_KEY_HERE",
     ),
 )
 
 
 req = operations.GetAccountCategoryRequest(
-    account_id="unde",
-    company_id="deserunt",
-    connection_id="porro",
+    account_id="corrupti",
+    company_id="8a210b68-6988-11ed-a1eb-0242ac120002",
+    connection_id="2e9d2c44-f675-40ba-8049-353bfcb5e171",
 )
     
 res = s.categories.get_account_category(req)
 
 if res.categorised_account is not None:
     # handle response
 ```
 <!-- End SDK Example Usage -->
 
 <!-- Start SDK Available Operations -->
-## SDK Available Operations
+## Available Resources and Operations
 
 
 ### categories
 
 * `get_account_category` - Get suggested and/or confirmed category for a specific account
 * `list_accounts_categories` - List suggested and confirmed account categories
 * `list_available_account_categories` - List account categories
@@ -61,31 +61,33 @@
 
 * `get_data_integrity_details` - Lists data integrity details for date type
 * `get_data_integrity_status` - Get data integrity status
 * `get_data_integrity_summaries` - Get data integrity summary
 
 ### excel_reports
 
+* `download_excel_report` - Download generated excel report
+* `generate_excel_report` - Generate an Excel report
 * `get_accounting_marketing_metrics` - Get the marketing metrics from an accounting source for a given company.
 * `get_excel_report` - Download generated excel report
-* `make_request_to_download_excel_report` - Request an Excel report for download
-* `request_excel_report_for_download` - Request an Excel report for download
+* `get_excel_report_generation_status` - Get status of Excel report
 
 ### reports
 
 * `get_accounts_for_enhanced_balance_sheet` - Enhanced Balance Sheet Accounts
 * `get_accounts_for_enhanced_profit_and_loss` - Enhanced Profit and Loss Accounts
 * `get_commerce_customer_retention_metrics` - Get the customer retention metrics for a specific company.
 * `get_commerce_lifetime_value_metrics` - Get the lifetime value metric for a specific company.
 * `get_commerce_orders_metrics` - Get order information for a specific company
 * `get_commerce_refunds_metrics` - Get the refunds information for a specific company
 * `get_commerce_revenue_metrics` - Commerce Revenue Metrics
 * `get_enhanced_balance_sheet` - Enhanced Balance Sheet
 * `get_enhanced_cash_flow_transactions` - Get enhanced cash flow report
-* `get_enhanced_financial_metrics` - List finanicial metrics
+* `get_enhanced_financial_metrics` - List financial metrics
+* `get_enhanced_invoices_report` - Enhanced Invoices Report
 * `get_enhanced_profit_and_loss` - Enhanced Profit and Loss
 * `get_recurring_revenue_metrics` - Get key metrics for subscription revenue
 * `request_recurring_revenue_metrics` - Request production of key subscription revenue metrics
 <!-- End SDK Available Operations -->
 
 ### SDK Generated by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)
```

### Comparing `codat-assess-0.5.1/README.md` & `codat-assess-0.9.6/src/codat_assess.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: codat-assess
+Version: 0.9.6
+Summary: Python Client SDK Generated by Speakeasy
+Home-page: UNKNOWN
+Author: Speakeasy
+License: UNKNOWN
+Platform: UNKNOWN
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+
 # codat-assess
 
 <!-- Start SDK Installation -->
 ## SDK Installation
 
 ```bash
 pip install codat-assess
@@ -18,28 +29,28 @@
     security=shared.Security(
         auth_header="YOUR_API_KEY_HERE",
     ),
 )
 
 
 req = operations.GetAccountCategoryRequest(
-    account_id="unde",
-    company_id="deserunt",
-    connection_id="porro",
+    account_id="corrupti",
+    company_id="8a210b68-6988-11ed-a1eb-0242ac120002",
+    connection_id="2e9d2c44-f675-40ba-8049-353bfcb5e171",
 )
     
 res = s.categories.get_account_category(req)
 
 if res.categorised_account is not None:
     # handle response
 ```
 <!-- End SDK Example Usage -->
 
 <!-- Start SDK Available Operations -->
-## SDK Available Operations
+## Available Resources and Operations
 
 
 ### categories
 
 * `get_account_category` - Get suggested and/or confirmed category for a specific account
 * `list_accounts_categories` - List suggested and confirmed account categories
 * `list_available_account_categories` - List account categories
@@ -50,30 +61,34 @@
 
 * `get_data_integrity_details` - Lists data integrity details for date type
 * `get_data_integrity_status` - Get data integrity status
 * `get_data_integrity_summaries` - Get data integrity summary
 
 ### excel_reports
 
+* `download_excel_report` - Download generated excel report
+* `generate_excel_report` - Generate an Excel report
 * `get_accounting_marketing_metrics` - Get the marketing metrics from an accounting source for a given company.
 * `get_excel_report` - Download generated excel report
-* `make_request_to_download_excel_report` - Request an Excel report for download
-* `request_excel_report_for_download` - Request an Excel report for download
+* `get_excel_report_generation_status` - Get status of Excel report
 
 ### reports
 
 * `get_accounts_for_enhanced_balance_sheet` - Enhanced Balance Sheet Accounts
 * `get_accounts_for_enhanced_profit_and_loss` - Enhanced Profit and Loss Accounts
 * `get_commerce_customer_retention_metrics` - Get the customer retention metrics for a specific company.
 * `get_commerce_lifetime_value_metrics` - Get the lifetime value metric for a specific company.
 * `get_commerce_orders_metrics` - Get order information for a specific company
 * `get_commerce_refunds_metrics` - Get the refunds information for a specific company
 * `get_commerce_revenue_metrics` - Commerce Revenue Metrics
 * `get_enhanced_balance_sheet` - Enhanced Balance Sheet
 * `get_enhanced_cash_flow_transactions` - Get enhanced cash flow report
-* `get_enhanced_financial_metrics` - List finanicial metrics
+* `get_enhanced_financial_metrics` - List financial metrics
+* `get_enhanced_invoices_report` - Enhanced Invoices Report
 * `get_enhanced_profit_and_loss` - Enhanced Profit and Loss
 * `get_recurring_revenue_metrics` - Get key metrics for subscription revenue
 * `request_recurring_revenue_metrics` - Request production of key subscription revenue metrics
 <!-- End SDK Available Operations -->
 
 ### SDK Generated by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)
+
+
```

### Comparing `codat-assess-0.5.1/setup.py` & `codat-assess-0.9.6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import setuptools
 
 try:
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="codat-assess",
-    version="0.5.1",
+    version="0.9.6",
     author="Speakeasy",
     description="Python Client SDK Generated by Speakeasy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi==2022.12.07",
```

### Comparing `codat-assess-0.5.1/src/codat/categories.py` & `codat-assess-0.9.6/src/codat/categories.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
-from codat.models import operations
+from codat.models import operations, shared
 from typing import Optional
 
 class Categories:
+    r"""Categorisation"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -19,39 +22,37 @@
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
     def get_account_category(self, request: operations.GetAccountCategoryRequest) -> operations.GetAccountCategoryResponse:
         r"""Get suggested and/or confirmed category for a specific account
         Get category for specific nominal account.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetAccountCategoryRequest, base_url, '/data/companies/{companyId}/connections/{connectionId}/assess/accounts/{accountId}/categories', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetAccountCategoryResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetAccountCategoryCategorisedAccount])
+                out = utils.unmarshal_json(http_res.text, Optional[shared.CategorisedAccount])
                 res.categorised_account = out
 
         return res
 
     def list_accounts_categories(self, request: operations.ListAccountsCategoriesRequest) -> operations.ListAccountsCategoriesResponse:
         r"""List suggested and confirmed account categories
         Lists suggested and confirmed chart of account categories for the given company and data connection.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.ListAccountsCategoriesRequest, base_url, '/data/companies/{companyId}/connections/{connectionId}/assess/accounts/categories', request)
         
         query_params = utils.get_query_params(operations.ListAccountsCategoriesRequest, request)
         
         client = self._security_client
@@ -59,93 +60,90 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListAccountsCategoriesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.ListAccountsCategoriesLinks])
-                res.links = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.CategorisedAccounts])
+                res.categorised_accounts = out
 
         return res
 
     def list_available_account_categories(self) -> operations.ListAvailableAccountCategoriesResponse:
         r"""List account categories
-        Lists available account categories Codat's categorisation engine can provide. 
+        Lists available account categories Codat's categorisation engine can provide.
         """
-        
         base_url = self._server_url
         
         url = base_url.removesuffix('/') + '/data/assess/accounts/categories'
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.ListAvailableAccountCategoriesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[list[operations.ListAvailableAccountCategoriesChartOfAccountCategory]])
-                res.list_available_account_categories_chart_of_account_category_anies = out
+                out = utils.unmarshal_json(http_res.text, Optional[list[shared.Categories]])
+                res.categories = out
 
         return res
 
     def update_account_category(self, request: operations.UpdateAccountCategoryRequest) -> operations.UpdateAccountCategoryResponse:
         r"""Patch account categories
         Update category for a specific nominal account
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.UpdateAccountCategoryRequest, base_url, '/data/companies/{companyId}/connections/{connectionId}/assess/accounts/{accountId}/categories', request)
         
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, "confirm_category", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         
         client = self._security_client
         
         http_res = client.request('PATCH', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.UpdateAccountCategoryResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.UpdateAccountCategoryCategorisedAccount])
+                out = utils.unmarshal_json(http_res.text, Optional[shared.CategorisedAccount])
                 res.categorised_account = out
 
         return res
 
     def update_accounts_categories(self, request: operations.UpdateAccountsCategoriesRequest) -> operations.UpdateAccountsCategoriesResponse:
         r"""Confirm categories for accounts
         Comfirms the categories for all or a batch of accounts for a specific connection.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.UpdateAccountsCategoriesRequest, base_url, '/data/companies/{companyId}/connections/{connectionId}/assess/accounts/categories', request)
         
         headers = {}
-        req_content_type, data, form = utils.serialize_request_body(request, "request_body", 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, "confirm_categories", 'json')
         if req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         
         client = self._security_client
         
         http_res = client.request('PATCH', url, data=data, files=form, headers=headers)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.UpdateAccountsCategoriesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[list[operations.UpdateAccountsCategoriesCategorisedAccount]])
+                out = utils.unmarshal_json(http_res.text, Optional[list[shared.CategorisedAccount]])
                 res.categorised_accounts = out
 
         return res
```

### Comparing `codat-assess-0.5.1/src/codat/data_integrity.py` & `codat-assess-0.9.6/src/codat/data_integrity.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
-from codat.models import operations
+from codat.models import operations, shared
 from typing import Optional
 
 class DataIntegrity:
+    r"""Data integrity is important"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -19,15 +22,14 @@
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
     def get_data_integrity_details(self, request: operations.GetDataIntegrityDetailsRequest) -> operations.GetDataIntegrityDetailsResponse:
         r"""Lists data integrity details for date type
         Gets record-by-record match results for a given company and datatype, optionally restricted by a Codat query string.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetDataIntegrityDetailsRequest, base_url, '/data/companies/{companyId}/assess/dataTypes/{dataType}/dataIntegrity/details', request)
         
         query_params = utils.get_query_params(operations.GetDataIntegrityDetailsRequest, request)
         
         client = self._security_client
@@ -35,48 +37,46 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetDataIntegrityDetailsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetDataIntegrityDetailsLinks])
-                res.links = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Details])
+                res.details = out
 
         return res
 
     def get_data_integrity_status(self, request: operations.GetDataIntegrityStatusRequest) -> operations.GetDataIntegrityStatusResponse:
         r"""Get data integrity status
         Gets match status for a given company and datatype.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetDataIntegrityStatusRequest, base_url, '/data/companies/{companyId}/assess/dataTypes/{dataType}/dataIntegrity/status', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetDataIntegrityStatusResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetDataIntegrityStatus200ApplicationJSON])
-                res.get_data_integrity_status_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Status])
+                res.status = out
 
         return res
 
     def get_data_integrity_summaries(self, request: operations.GetDataIntegritySummariesRequest) -> operations.GetDataIntegritySummariesResponse:
         r"""Get data integrity summary
         Gets match summary for a given company and datatype, optionally restricted by a Codat query string.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetDataIntegritySummariesRequest, base_url, '/data/companies/{companyId}/assess/dataTypes/{dataType}/dataIntegrity/summaries', request)
         
         query_params = utils.get_query_params(operations.GetDataIntegritySummariesRequest, request)
         
         client = self._security_client
@@ -84,13 +84,13 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetDataIntegritySummariesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetDataIntegritySummaries200ApplicationJSON])
-                res.get_data_integrity_summaries_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Summaries])
+                res.summaries = out
 
         return res
```

### Comparing `codat-assess-0.5.1/src/codat/excel_reports.py` & `codat-assess-0.9.6/src/codat/excel_reports.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
-from codat.models import operations
+from codat.models import operations, shared
 from typing import Optional
 
 class ExcelReports:
+    r"""Downloadable reports"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -15,107 +18,126 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    def get_accounting_marketing_metrics(self, request: operations.GetAccountingMarketingMetricsRequest) -> operations.GetAccountingMarketingMetricsResponse:
-        r"""Get the marketing metrics from an accounting source for a given company.
-        Request an Excel report for download.
+    def download_excel_report(self, request: operations.DownloadExcelReportRequest) -> operations.DownloadExcelReportResponse:
+        r"""Download generated excel report
+        Download the previously generated Excel report to a local drive.
         """
-        
         base_url = self._server_url
         
-        url = utils.generate_url(operations.GetAccountingMarketingMetricsRequest, base_url, '/data/companies/{companyId}/connections/{connectionId}/assess/accountingMetrics/marketing', request)
+        url = utils.generate_url(operations.DownloadExcelReportRequest, base_url, '/data/companies/{companyId}/assess/excel/download', request)
         
-        query_params = utils.get_query_params(operations.GetAccountingMarketingMetricsRequest, request)
+        query_params = utils.get_query_params(operations.DownloadExcelReportRequest, request)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params)
+        http_res = client.request('POST', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetAccountingMarketingMetricsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.DownloadExcelReportResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetAccountingMarketingMetrics200ApplicationJSON])
-                res.get_accounting_marketing_metrics_200_application_json_object = out
+            if utils.match_content_type(content_type, 'application/octet-stream'):
+                res.body = http_res.content
 
         return res
 
-    def get_excel_report(self, request: operations.GetExcelReportRequest) -> operations.GetExcelReportResponse:
-        r"""Download generated excel report
-        Download the Excel report to a local drive.
+    def generate_excel_report(self, request: operations.GenerateExcelReportRequest) -> operations.GenerateExcelReportResponse:
+        r"""Generate an Excel report
+        Generate an Excel report which can subsequently be downloaded.
         """
-        
         base_url = self._server_url
         
-        url = utils.generate_url(operations.GetExcelReportRequest, base_url, '/data/companies/{companyId}/assess/excel/download', request)
+        url = utils.generate_url(operations.GenerateExcelReportRequest, base_url, '/data/companies/{companyId}/assess/excel', request)
         
-        query_params = utils.get_query_params(operations.GetExcelReportRequest, request)
+        query_params = utils.get_query_params(operations.GenerateExcelReportRequest, request)
         
         client = self._security_client
         
         http_res = client.request('POST', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetExcelReportResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GenerateExcelReportResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(content_type, 'application/octet-stream'):
-                res.body = http_res.content
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[shared.ExcelStatus])
+                res.excel_status = out
 
         return res
 
-    def make_request_to_download_excel_report(self, request: operations.MakeRequestToDownloadExcelReportRequest) -> operations.MakeRequestToDownloadExcelReportResponse:
-        r"""Request an Excel report for download
-        Returns the status of the latest report requested.
+    def get_accounting_marketing_metrics(self, request: operations.GetAccountingMarketingMetricsRequest) -> operations.GetAccountingMarketingMetricsResponse:
+        r"""Get the marketing metrics from an accounting source for a given company.
+        Request an Excel report for download.
         """
-        
         base_url = self._server_url
         
-        url = utils.generate_url(operations.MakeRequestToDownloadExcelReportRequest, base_url, '/data/companies/{companyId}/assess/excel', request)
+        url = utils.generate_url(operations.GetAccountingMarketingMetricsRequest, base_url, '/data/companies/{companyId}/connections/{connectionId}/assess/accountingMetrics/marketing', request)
         
-        query_params = utils.get_query_params(operations.MakeRequestToDownloadExcelReportRequest, request)
+        query_params = utils.get_query_params(operations.GetAccountingMarketingMetricsRequest, request)
         
         client = self._security_client
         
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.MakeRequestToDownloadExcelReportResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetAccountingMarketingMetricsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.MakeRequestToDownloadExcelReport200ApplicationJSON])
-                res.make_request_to_download_excel_report_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Report])
+                res.report = out
 
         return res
 
-    def request_excel_report_for_download(self, request: operations.RequestExcelReportForDownloadRequest) -> operations.RequestExcelReportForDownloadResponse:
-        r"""Request an Excel report for download
-        Request an Excel report for download.
+    def get_excel_report(self, request: operations.GetExcelReportRequest) -> operations.GetExcelReportResponse:
+        r"""Download generated excel report
+        Download the previously generated Excel report to a local drive.
         """
+        base_url = self._server_url
+        
+        url = utils.generate_url(operations.GetExcelReportRequest, base_url, '/data/companies/{companyId}/assess/excel/download', request)
+        
+        query_params = utils.get_query_params(operations.GetExcelReportRequest, request)
+        
+        client = self._security_client
+        
+        http_res = client.request('GET', url, params=query_params)
+        content_type = http_res.headers.get('Content-Type')
+
+        res = operations.GetExcelReportResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/octet-stream'):
+                res.body = http_res.content
+
+        return res
+
+    def get_excel_report_generation_status(self, request: operations.GetExcelReportGenerationStatusRequest) -> operations.GetExcelReportGenerationStatusResponse:
+        r"""Get status of Excel report
+        Returns the status of the latest report requested.
+        """
         base_url = self._server_url
         
-        url = utils.generate_url(operations.RequestExcelReportForDownloadRequest, base_url, '/data/companies/{companyId}/assess/excel', request)
+        url = utils.generate_url(operations.GetExcelReportGenerationStatusRequest, base_url, '/data/companies/{companyId}/assess/excel', request)
         
-        query_params = utils.get_query_params(operations.RequestExcelReportForDownloadRequest, request)
+        query_params = utils.get_query_params(operations.GetExcelReportGenerationStatusRequest, request)
         
         client = self._security_client
         
-        http_res = client.request('POST', url, params=query_params)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.RequestExcelReportForDownloadResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetExcelReportGenerationStatusResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.RequestExcelReportForDownload200ApplicationJSON])
-                res.request_excel_report_for_download_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.ExcelStatus])
+                res.excel_status = out
 
         return res
```

### Comparing `codat-assess-0.5.1/src/codat/models/operations/get_account_category.py` & `codat-assess-0.9.6/src/codat/models/shared/accountcategoriesupdatedwebhook.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,53 +1,40 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
-import dateutil.parser
-import requests as requests_http
 from codat import utils
 from dataclasses_json import Undefined, dataclass_json
-from datetime import datetime
-from marshmallow import fields
 from typing import Optional
 
 
-@dataclasses.dataclass
-class GetAccountCategoryRequest:
-    account_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'accountId', 'style': 'simple', 'explode': False }})
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})
-    
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetAccountCategoryCategorisedAccountAccountRef:
-    r"""GetAccountCategoryCategorisedAccountAccountRef
-    An object containing account reference data.
-    """
-    
-    id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id'), 'exclude': lambda f: f is None }})
-    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
+class AccountCategoriesUpdatedWebhookData:
     
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetAccountCategoryCategorisedAccountModifiedDate:
-    detail_type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('detailType'), 'exclude': lambda f: f is None }})
-    modified_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    subtype: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subtype'), 'exclude': lambda f: f is None }})
-    type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})
+    modified_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedDate'), 'exclude': lambda f: f is None }})
+    r"""The date on which this account categories were last modified in Codat."""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetAccountCategoryCategorisedAccount:
-    account_ref: Optional[GetAccountCategoryCategorisedAccountAccountRef] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('accountRef'), 'exclude': lambda f: f is None }})
-    confirmed: Optional[GetAccountCategoryCategorisedAccountModifiedDate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('confirmed'), 'exclude': lambda f: f is None }})
-    suggested: Optional[GetAccountCategoryCategorisedAccountModifiedDate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('suggested'), 'exclude': lambda f: f is None }})
+class AccountCategoriesUpdatedWebhook:
+    r"""Webhook request body for account categories updated."""
     
-
-@dataclasses.dataclass
-class GetAccountCategoryResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    categorised_account: Optional[GetAccountCategoryCategorisedAccount] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    alert_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('alertId'), 'exclude': lambda f: f is None }})
+    r"""Unique identifier of the alert."""  
+    client_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('clientId'), 'exclude': lambda f: f is None }})
+    r"""Unique identifier for your client in Codat."""  
+    client_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('clientName'), 'exclude': lambda f: f is None }})
+    r"""Name of your client in Codat."""  
+    company_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('companyId'), 'exclude': lambda f: f is None }})
+    r"""Unique identifier for your SMB in Codat."""  
+    data: Optional[AccountCategoriesUpdatedWebhookData] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})  
+    data_connection_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataConnectionId'), 'exclude': lambda f: f is None }})
+    r"""Unique identifier for a company's data connection."""  
+    message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('message'), 'exclude': lambda f: f is None }})
+    r"""A human readable message about the webhook."""  
+    rule_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ruleId'), 'exclude': lambda f: f is None }})
+    r"""Unique identifier for the rule."""  
+    rule_type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ruleType'), 'exclude': lambda f: f is None }})
+    r"""The type of rule."""
```

### Comparing `codat-assess-0.5.1/src/codat/models/operations/get_data_integrity_status.py` & `codat-assess-0.9.6/src/codat/models/shared/financialmetric.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,93 +1,112 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
-import dateutil.parser
-import requests as requests_http
 from codat import utils
 from dataclasses_json import Undefined, dataclass_json
-from datetime import datetime
+from datetime import date
 from enum import Enum
 from marshmallow import fields
 from typing import Optional
 
-class GetDataIntegrityStatusDataTypeEnum(str, Enum):
-    BANKING_ACCOUNTS = "banking-accounts"
-    BANKING_TRANSACTIONS = "banking-transactions"
-    BANK_ACCOUNTS = "bankAccounts"
-    ACCOUNT_TRANSACTIONS = "accountTransactions"
-
+class FinancialMetricErrorsTypeEnum(str, Enum):
+    r"""Metric level error."""
+    UNCATEGORIZED_ACCOUNTS = 'UncategorizedAccounts'
+    MISSING_INPUT_DATA = 'MissingInputData'
+    INPUT_DATA_ERROR = 'InputDataError'
 
-@dataclasses.dataclass
-class GetDataIntegrityStatusRequest:
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    data_type: GetDataIntegrityStatusDataTypeEnum = dataclasses.field(metadata={'path_param': { 'field_name': 'dataType', 'style': 'simple', 'explode': False }})
-    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetDataIntegrityStatus200ApplicationJSONDataIntegrityTypeAmounts:
-    r"""GetDataIntegrityStatus200ApplicationJSONDataIntegrityTypeAmounts
-    Only returned for transactions. For accounts, there is nothing returned.
-    """
-    
-    currency: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currency'), 'exclude': lambda f: f is None }})
-    max: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('max'), 'exclude': lambda f: f is None }})
-    min: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('min'), 'exclude': lambda f: f is None }})
+class FinancialMetricErrors:
     
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetDataIntegrityStatus200ApplicationJSONDataIntegrityTypeConnectionIds:
-    source: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('source'), 'exclude': lambda f: f is None }})
-    target: Optional[list[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('target'), 'exclude': lambda f: f is None }})
+    details: Optional[dict[str, list[str]]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('details'), 'exclude': lambda f: f is None }})
+    r"""Dictionary list outlining the missing properties or allowed values."""  
+    message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('message'), 'exclude': lambda f: f is None }})
+    r"""Description of the error."""  
+    type: Optional[FinancialMetricErrorsTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})
+    r"""Metric level error."""  
     
+class FinancialMetricKeyEnum(str, Enum):
+    UNKNOWN = 'Unknown'
+    EBITDA = 'EBITDA'
+    DEBT_SERVICE_COVERAGE_RATIO = 'DebtServiceCoverageRatio'
+    CURRENT_RATIO_QUICK_RATIO = 'CurrentRatio QuickRatio'
+    GROSS_PROFIT_MARGIN = 'GrossProfitMargin'
+    FIXED_CHARGE_COVERAGE_RATIO = 'FixedChargeCoverageRatio'
+    WORKING_CAPITAL = 'WorkingCapital'
+    FREE_CASH_FLOW = 'FreeCashFlow'
+    NET_PROFIT_MARGIN = 'NetProfitMargin'
+    RETURN_ON_ASSETS_RATIO = 'ReturnOnAssetsRatio'
+    RETURN_ON_EQUITY_RATIO = 'ReturnOnEquityRatio'
+    OPERATING_PROFIT_MARGIN = 'OperatingProfitMargin'
+    DEPT_TO_EQUITY = 'DeptToEquity'
+    DEBT_TO_ASSETS = 'DebtToAssets'
+    INTEREST_COVERAGE_RATIO = 'InterestCoverageRatio'
+    CASH_RATIO = 'CashRatio'
+    INVENTORY_TURNOVER_RATIO = 'InventoryTurnoverRatio'
+    ASSET_TURNOVER_RATIO = 'AssetTurnoverRatio'
+    WORKING_CAPITAL_TURNOVER_RATIO = 'WorkingCapitalTurnoverRatio'
+    DAYS_SALES_OUTSTANDING = 'DaysSalesOutstanding'
+    DAYS_PAYABLES_OUTSTANDING = 'DaysPayablesOutstanding'
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetDataIntegrityStatus200ApplicationJSONDataIntegrityTypeDates:
-    r"""GetDataIntegrityStatus200ApplicationJSONDataIntegrityTypeDates
-    Only returned for transactions. For accounts, there is nothing returned.
-    """
-    
-    max_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('maxDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    max_overlapping_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('maxOverlappingDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    min_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    min_overlapping_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('minOverlappingDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    
-class GetDataIntegrityStatus200ApplicationJSONDataIntegrityTypeStatusInfoCurrentStatusEnum(str, Enum):
-    UNKNOWN = "Unknown"
-    DOES_NOT_EXIST = "DoesNotExist"
-    ERROR = "Error"
-    COMPLETE = "Complete"
+class FinancialMetricMetricUnitEnum(str, Enum):
+    RATIO = 'Ratio'
+    MONEY = 'Money'
+
+class FinancialMetricPeriodsErrorsTypeEnum(str, Enum):
+    r"""Period error type."""
+    MISSING_ACCOUNT_DATA = 'MissingAccountData'
+    DATES_OUT_OF_RANGE = 'DatesOutOfRange'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetDataIntegrityStatus200ApplicationJSONDataIntegrityTypeStatusInfo:
-    current_status: Optional[GetDataIntegrityStatus200ApplicationJSONDataIntegrityTypeStatusInfoCurrentStatusEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('currentStatus'), 'exclude': lambda f: f is None }})
-    last_matched: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastMatched'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    status_message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('statusMessage'), 'exclude': lambda f: f is None }})
+class FinancialMetricPeriodsErrors:
+    
+    details: Optional[dict[str, list[str]]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('details'), 'exclude': lambda f: f is None }})
+    r"""Dictionary list outlining the missing properties or allowed values."""  
+    massage: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('massage'), 'exclude': lambda f: f is None }})
+    r"""Description of the error."""  
+    type: Optional[FinancialMetricPeriodsErrorsTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})
+    r"""Period error type."""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetDataIntegrityStatus200ApplicationJSONDataIntegrityType:
-    amounts: Optional[GetDataIntegrityStatus200ApplicationJSONDataIntegrityTypeAmounts] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('amounts'), 'exclude': lambda f: f is None }})
-    connection_ids: Optional[GetDataIntegrityStatus200ApplicationJSONDataIntegrityTypeConnectionIds] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('connectionIds'), 'exclude': lambda f: f is None }})
-    dates: Optional[GetDataIntegrityStatus200ApplicationJSONDataIntegrityTypeDates] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dates'), 'exclude': lambda f: f is None }})
-    status_info: Optional[GetDataIntegrityStatus200ApplicationJSONDataIntegrityTypeStatusInfo] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('statusInfo'), 'exclude': lambda f: f is None }})
-    type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})
+class FinancialMetricPeriodsInputs:
+    
+    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
+    r"""The name of the metric input e.g. “Current Assets”, “Capital Expenditure”."""  
+    value: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('value'), 'exclude': lambda f: f is None }})
+    r"""The positive or negative number of the input value."""  
     
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetDataIntegrityStatus200ApplicationJSON:
-    metadata: Optional[list[GetDataIntegrityStatus200ApplicationJSONDataIntegrityType]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
+class FinancialMetricPeriods:
+    
+    errors: Optional[list[FinancialMetricPeriodsErrors]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errors'), 'exclude': lambda f: f is None }})  
+    from_date: Optional[date] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fromDate'), 'encoder': utils.dateisoformat(True), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
+    r"""The date from which the report starts."""  
+    inputs: Optional[list[FinancialMetricPeriodsInputs]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('inputs'), 'exclude': lambda f: f is None }})  
+    to_date: Optional[date] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('toDate'), 'encoder': utils.dateisoformat(True), 'decoder': utils.datefromisoformat, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
+    r"""The date on which the report ends (inclusive of day)."""  
+    value: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('value'), 'exclude': lambda f: f is None }})
+    r"""The top level metric value that is calculated for the specified period.
+    
+    If the system cannot calculate for that period, the value will be null. The system will still show the metric inputs.
+    """  
     
 
+@dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetDataIntegrityStatusResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    get_data_integrity_status_200_application_json_object: Optional[GetDataIntegrityStatus200ApplicationJSON] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+class FinancialMetric:
+    
+    errors: Optional[list[FinancialMetricErrors]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errors'), 'exclude': lambda f: f is None }})  
+    key: Optional[FinancialMetricKeyEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('key'), 'exclude': lambda f: f is None }})  
+    metric_unit: Optional[FinancialMetricMetricUnitEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metricUnit'), 'exclude': lambda f: f is None }})  
+    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
+    r"""Metric name."""  
+    periods: Optional[list[FinancialMetricPeriods]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('periods'), 'exclude': lambda f: f is None }})
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `codat-assess-0.5.1/src/codat/models/operations/get_excel_report.py` & `codat-assess-0.9.6/src/codat/models/operations/request_recurring_revenue_metrics.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,25 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
-from enum import Enum
+from ..shared import report as shared_report
 from typing import Optional
 
-class GetExcelReportReportTypeEnum(str, Enum):
-    AUDIT = "audit"
-
 
 @dataclasses.dataclass
-class GetExcelReportRequest:
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    report_type: GetExcelReportReportTypeEnum = dataclasses.field(metadata={'query_param': { 'field_name': 'reportType', 'style': 'form', 'explode': True }})
+class RequestRecurringRevenueMetricsRequest:
+    
+    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
+    connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})  
     
 
 @dataclasses.dataclass
-class GetExcelReportResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    body: Optional[bytes] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+class RequestRecurringRevenueMetricsResponse:
+    
+    content_type: str = dataclasses.field()  
+    status_code: int = dataclasses.field()  
+    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
+    report: Optional[shared_report.Report] = dataclasses.field(default=None)
+    r"""OK"""
```

### Comparing `codat-assess-0.5.1/src/codat/models/operations/list_available_account_categories.py` & `codat-assess-0.9.6/src/codat/models/shared/reportcomponent.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,21 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
-import requests as requests_http
+from ..shared import reportcomponentmeasure as shared_reportcomponentmeasure
 from codat import utils
 from dataclasses_json import Undefined, dataclass_json
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class ListAvailableAccountCategoriesChartOfAccountCategory:
-    detail_type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('detailType'), 'exclude': lambda f: f is None }})
-    detail_type_description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('detailTypeDescription'), 'exclude': lambda f: f is None }})
-    detail_type_display_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('detailTypeDisplayName'), 'exclude': lambda f: f is None }})
-    subtype: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subtype'), 'exclude': lambda f: f is None }})
-    subtype_display_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subtypeDisplayName'), 'exclude': lambda f: f is None }})
-    type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})
+class ReportComponent:
     
-
-@dataclasses.dataclass
-class ListAvailableAccountCategoriesResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    list_available_account_categories_chart_of_account_category_anies: Optional[list[ListAvailableAccountCategoriesChartOfAccountCategory]] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    components: Optional[list[ReportComponent]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('components'), 'exclude': lambda f: f is None }})  
+    dimension: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dimension'), 'exclude': lambda f: f is None }})  
+    dimension_display_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dimensionDisplayName'), 'exclude': lambda f: f is None }})  
+    item: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('item'), 'exclude': lambda f: f is None }})  
+    item_display_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('itemDisplayName'), 'exclude': lambda f: f is None }})  
+    measures: Optional[list[shared_reportcomponentmeasure.ReportComponentMeasure]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('measures'), 'exclude': lambda f: f is None }})
```

### Comparing `codat-assess-0.5.1/src/codat/models/operations/make_request_to_download_excel_report.py` & `codat-assess-0.9.6/src/codat/models/shared/categories.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,26 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
-import dateutil.parser
-import requests as requests_http
 from codat import utils
 from dataclasses_json import Undefined, dataclass_json
-from datetime import datetime
-from enum import Enum
-from marshmallow import fields
 from typing import Optional
 
-class MakeRequestToDownloadExcelReportReportTypeEnum(str, Enum):
-    AUDIT = "audit"
-
-
-@dataclasses.dataclass
-class MakeRequestToDownloadExcelReportRequest:
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    report_type: MakeRequestToDownloadExcelReportReportTypeEnum = dataclasses.field(metadata={'query_param': { 'field_name': 'reportType', 'style': 'form', 'explode': True }})
-    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class MakeRequestToDownloadExcelReport200ApplicationJSON:
-    error_message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorMessage'), 'exclude': lambda f: f is None }})
-    file_size: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fileSize'), 'exclude': lambda f: f is None }})
-    in_progress: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('inProgress'), 'exclude': lambda f: f is None }})
-    last_generated: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastGenerated'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    last_invocation_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastInvocationId'), 'exclude': lambda f: f is None }})
-    queued: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('queued'), 'exclude': lambda f: f is None }})
-    report_type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reportType'), 'exclude': lambda f: f is None }})
-    success: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('success'), 'exclude': lambda f: f is None }})
+class Categories:
     
-
-@dataclasses.dataclass
-class MakeRequestToDownloadExcelReportResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    make_request_to_download_excel_report_200_application_json_object: Optional[MakeRequestToDownloadExcelReport200ApplicationJSON] = dataclasses.field(default=None)
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
+    detail_type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('detailType'), 'exclude': lambda f: f is None }})
+    r"""Most granular chart of account type."""  
+    detail_type_description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('detailTypeDescription'), 'exclude': lambda f: f is None }})
+    r"""A description of the fully categorized (to detail type) account."""  
+    detail_type_display_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('detailTypeDisplayName'), 'exclude': lambda f: f is None }})
+    r"""Human readable detailType display name."""  
+    subtype: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subtype'), 'exclude': lambda f: f is None }})
+    r"""The account subtype."""  
+    subtype_display_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('subtypeDisplayName'), 'exclude': lambda f: f is None }})
+    r"""Human readable subtype display name."""  
+    type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})
+    r"""The top level account type."""
```

### Comparing `codat-assess-0.5.1/src/codat/models/operations/request_excel_report_for_download.py` & `codat-assess-0.9.6/src/codat/models/shared/excelstatus.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,43 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
-import dateutil.parser
-import requests as requests_http
 from codat import utils
 from dataclasses_json import Undefined, dataclass_json
-from datetime import datetime
-from enum import Enum
-from marshmallow import fields
 from typing import Optional
 
-class RequestExcelReportForDownloadReportTypeEnum(str, Enum):
-    AUDIT = "audit"
-
-
-@dataclasses.dataclass
-class RequestExcelReportForDownloadRequest:
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})
-    report_type: RequestExcelReportForDownloadReportTypeEnum = dataclasses.field(metadata={'query_param': { 'field_name': 'reportType', 'style': 'form', 'explode': True }})
-    
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class RequestExcelReportForDownload200ApplicationJSON:
-    error_message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorMessage'), 'exclude': lambda f: f is None }})
-    file_size: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fileSize'), 'exclude': lambda f: f is None }})
-    in_progress: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('inProgress'), 'exclude': lambda f: f is None }})
-    last_generated: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastGenerated'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    last_invocation_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastInvocationId'), 'exclude': lambda f: f is None }})
-    queued: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('queued'), 'exclude': lambda f: f is None }})
-    report_type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reportType'), 'exclude': lambda f: f is None }})
-    success: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('success'), 'exclude': lambda f: f is None }})
+class ExcelStatus:
+    r"""OK"""
     
-
-@dataclasses.dataclass
-class RequestExcelReportForDownloadResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    request_excel_report_for_download_200_application_json_object: Optional[RequestExcelReportForDownload200ApplicationJSON] = dataclasses.field(default=None)
+    error_message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('errorMessage'), 'exclude': lambda f: f is None }})  
+    file_size: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fileSize'), 'exclude': lambda f: f is None }})  
+    in_progress: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('inProgress'), 'exclude': lambda f: f is None }})  
+    last_generated: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastGenerated'), 'exclude': lambda f: f is None }})
+    r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
+    
+    ```
+    2020-10-08T22:40:50Z
+    2021-01-01T00:00:00
+    ```
+    
+    
+    
+    When syncing data that contains `DateTime` fields from Codat, make sure you support the following cases when reading time information:
+    
+    - Coordinated Universal Time (UTC): `2021-11-15T06:00:00Z`
+    - Unqualified local time: `2021-11-15T01:00:00`
+    - UTC time offsets: `2021-11-15T01:00:00-05:00`
+    
+    > Time zones
+    > 
+    > Not all dates from Codat will contain information about time zones.  
+    > Where it is not available from the underlying platform, Codat will return these as times local to the business whose data has been synced.
+    """  
+    last_invocation_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('lastInvocationId'), 'exclude': lambda f: f is None }})  
+    queued: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('queued'), 'exclude': lambda f: f is None }})  
+    report_type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('reportType'), 'exclude': lambda f: f is None }})  
+    success: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('success'), 'exclude': lambda f: f is None }})
```

### Comparing `codat-assess-0.5.1/src/codat/models/webhooks/account_categories_updated.py` & `codat-assess-0.9.6/src/codat/models/shared/reportmeasure.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,18 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 from __future__ import annotations
 import dataclasses
-import dateutil.parser
-import requests as requests_http
 from codat import utils
 from dataclasses_json import Undefined, dataclass_json
-from datetime import datetime
-from marshmallow import fields
 from typing import Optional
 
 
-@dataclasses.dataclass
-class AccountCategoriesUpdatedResponse:
-    content_type: str = dataclasses.field()
-    status_code: int = dataclasses.field()
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)
-    
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class AccountCategoriesUpdatedAccountCategoriesUpdatedWebhookData:
-    modified_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class AccountCategoriesUpdatedAccountCategoriesUpdatedWebhook:
-    r"""AccountCategoriesUpdatedAccountCategoriesUpdatedWebhook
-    Webhook request body for account categories updated.
-    """
+class ReportMeasure:
     
-    alert_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('alertId'), 'exclude': lambda f: f is None }})
-    client_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('clientId'), 'exclude': lambda f: f is None }})
-    client_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('clientName'), 'exclude': lambda f: f is None }})
-    company_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('companyId'), 'exclude': lambda f: f is None }})
-    data: Optional[AccountCategoriesUpdatedAccountCategoriesUpdatedWebhookData] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('data'), 'exclude': lambda f: f is None }})
-    data_connection_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('dataConnectionId'), 'exclude': lambda f: f is None }})
-    message: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('message'), 'exclude': lambda f: f is None }})
-    rule_id: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ruleId'), 'exclude': lambda f: f is None }})
-    rule_type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ruleType'), 'exclude': lambda f: f is None }})
+    display_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('displayName'), 'exclude': lambda f: f is None }})  
+    index: Optional[int] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('index'), 'exclude': lambda f: f is None }})  
+    type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})  
+    units: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('units'), 'exclude': lambda f: f is None }})
```

### Comparing `codat-assess-0.5.1/src/codat/reports.py` & `codat-assess-0.9.6/src/codat/reports.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
+
 import requests as requests_http
 from . import utils
-from codat.models import operations
+from codat.models import operations, shared
 from typing import Optional
 
 class Reports:
+    r"""Data integrity is important"""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
 
@@ -17,17 +20,18 @@
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
     def get_accounts_for_enhanced_balance_sheet(self, request: operations.GetAccountsForEnhancedBalanceSheetRequest) -> operations.GetAccountsForEnhancedBalanceSheetResponse:
         r"""Enhanced Balance Sheet Accounts
-        Gets a list of accounts with account categories per statement period, specific to balance sheet
-        """
+        The Enhanced Balance Sheet Accounts endpoint returns a list of categorized accounts that appear on a company’s Balance Sheet along with a balance per financial statement date.
         
+        Codat suggests a category for each account automatically, but you can [change it](/docs/assess-categorizing-accounts-ecommerce-lending) to a more suitable one.
+        """
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetAccountsForEnhancedBalanceSheetRequest, base_url, '/companies/{companyId}/reports/enhancedBalanceSheet/accounts', request)
         
         query_params = utils.get_query_params(operations.GetAccountsForEnhancedBalanceSheetRequest, request)
         
         client = self._security_client
@@ -35,24 +39,25 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetAccountsForEnhancedBalanceSheetResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetAccountsForEnhancedBalanceSheetEnhancedReport])
+                out = utils.unmarshal_json(http_res.text, Optional[shared.EnhancedReport])
                 res.enhanced_report = out
 
         return res
 
     def get_accounts_for_enhanced_profit_and_loss(self, request: operations.GetAccountsForEnhancedProfitAndLossRequest) -> operations.GetAccountsForEnhancedProfitAndLossResponse:
         r"""Enhanced Profit and Loss Accounts
-        Gets a list of accounts with account categories per statement period, specific to profit and loss
-        """
+        The Enhanced Profit and Loss Accounts endpoint returns a list of categorized accounts that appear on a company’s Profit and Loss. It also includes a balance per the financial statement date.
         
+        Codat suggests a category for each account automatically, but you can [change it](/docs/assess-categorizing-accounts-ecommerce-lending) to a more suitable one.
+        """
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetAccountsForEnhancedProfitAndLossRequest, base_url, '/companies/{companyId}/reports/enhancedProfitAndLoss/accounts', request)
         
         query_params = utils.get_query_params(operations.GetAccountsForEnhancedProfitAndLossRequest, request)
         
         client = self._security_client
@@ -60,24 +65,23 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetAccountsForEnhancedProfitAndLossResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetAccountsForEnhancedProfitAndLossEnhancedReport])
+                out = utils.unmarshal_json(http_res.text, Optional[shared.EnhancedReport])
                 res.enhanced_report = out
 
         return res
 
     def get_commerce_customer_retention_metrics(self, request: operations.GetCommerceCustomerRetentionMetricsRequest) -> operations.GetCommerceCustomerRetentionMetricsResponse:
         r"""Get the customer retention metrics for a specific company.
         Gets the customer retention metrics for a specific company connection, over one or more periods of time.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetCommerceCustomerRetentionMetricsRequest, base_url, '/data/companies/{companyId}/connections/{connectionId}/assess/commerceMetrics/customerRetention', request)
         
         query_params = utils.get_query_params(operations.GetCommerceCustomerRetentionMetricsRequest, request)
         
         client = self._security_client
@@ -85,24 +89,23 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetCommerceCustomerRetentionMetricsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetCommerceCustomerRetentionMetrics200ApplicationJSON])
-                res.get_commerce_customer_retention_metrics_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Report])
+                res.report = out
 
         return res
 
     def get_commerce_lifetime_value_metrics(self, request: operations.GetCommerceLifetimeValueMetricsRequest) -> operations.GetCommerceLifetimeValueMetricsResponse:
         r"""Get the lifetime value metric for a specific company.
         Gets the lifetime value metric for a specific company connection, over one or more periods of time.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetCommerceLifetimeValueMetricsRequest, base_url, '/data/companies/{companyId}/connections/{connectionId}/assess/commerceMetrics/lifetimeValue', request)
         
         query_params = utils.get_query_params(operations.GetCommerceLifetimeValueMetricsRequest, request)
         
         client = self._security_client
@@ -110,24 +113,23 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetCommerceLifetimeValueMetricsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetCommerceLifetimeValueMetrics200ApplicationJSON])
-                res.get_commerce_lifetime_value_metrics_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Report])
+                res.report = out
 
         return res
 
     def get_commerce_orders_metrics(self, request: operations.GetCommerceOrdersMetricsRequest) -> operations.GetCommerceOrdersMetricsResponse:
         r"""Get order information for a specific company
         Gets the order information for a specific company connection, over one or more periods of time.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetCommerceOrdersMetricsRequest, base_url, '/data/companies/{companyId}/connections/{connectionId}/assess/commerceMetrics/orders', request)
         
         query_params = utils.get_query_params(operations.GetCommerceOrdersMetricsRequest, request)
         
         client = self._security_client
@@ -135,24 +137,23 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetCommerceOrdersMetricsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetCommerceOrdersMetrics200ApplicationJSON])
-                res.get_commerce_orders_metrics_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Report])
+                res.report = out
 
         return res
 
     def get_commerce_refunds_metrics(self, request: operations.GetCommerceRefundsMetricsRequest) -> operations.GetCommerceRefundsMetricsResponse:
         r"""Get the refunds information for a specific company
         Gets the refunds information for a specific company connection, over one or more periods of time.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetCommerceRefundsMetricsRequest, base_url, '/data/companies/{companyId}/connections/{connectionId}/assess/commerceMetrics/refunds', request)
         
         query_params = utils.get_query_params(operations.GetCommerceRefundsMetricsRequest, request)
         
         client = self._security_client
@@ -160,24 +161,23 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetCommerceRefundsMetricsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetCommerceRefundsMetrics200ApplicationJSON])
-                res.get_commerce_refunds_metrics_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Report])
+                res.report = out
 
         return res
 
     def get_commerce_revenue_metrics(self, request: operations.GetCommerceRevenueMetricsRequest) -> operations.GetCommerceRevenueMetricsResponse:
         r"""Commerce Revenue Metrics
         Get the revenue and revenue growth for a specific company connection, over one or more periods of time.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetCommerceRevenueMetricsRequest, base_url, '/data/companies/{companyId}/connections/{connectionId}/assess/commerceMetrics/revenue', request)
         
         query_params = utils.get_query_params(operations.GetCommerceRevenueMetricsRequest, request)
         
         client = self._security_client
@@ -185,24 +185,23 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetCommerceRevenueMetricsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetCommerceRevenueMetrics200ApplicationJSON])
-                res.get_commerce_revenue_metrics_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Report])
+                res.report = out
 
         return res
 
     def get_enhanced_balance_sheet(self, request: operations.GetEnhancedBalanceSheetRequest) -> operations.GetEnhancedBalanceSheetResponse:
         r"""Enhanced Balance Sheet
         Gets a fully categorized balance sheet statement for a given company, over one or more period(s).
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetEnhancedBalanceSheetRequest, base_url, '/data/companies/{companyId}/connections/{connectionId}/assess/enhancedBalanceSheet', request)
         
         query_params = utils.get_query_params(operations.GetEnhancedBalanceSheetRequest, request)
         
         client = self._security_client
@@ -210,24 +209,23 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetEnhancedBalanceSheetResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetEnhancedBalanceSheet200ApplicationJSON])
-                res.get_enhanced_balance_sheet_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Report])
+                res.report = out
 
         return res
 
     def get_enhanced_cash_flow_transactions(self, request: operations.GetEnhancedCashFlowTransactionsRequest) -> operations.GetEnhancedCashFlowTransactionsResponse:
         r"""Get enhanced cash flow report
-        Gets a list of banking transactions and their categories.
+        The Enhanced Cash Flow Transactions endpoint provides a fully categorized list of banking transactions for a company. Accounts and transaction data are obtained from the company's banking data sources.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetEnhancedCashFlowTransactionsRequest, base_url, '/companies/{companyId}/reports/enhancedCashFlow/transactions', request)
         
         query_params = utils.get_query_params(operations.GetEnhancedCashFlowTransactionsRequest, request)
         
         client = self._security_client
@@ -235,24 +233,23 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetEnhancedCashFlowTransactionsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetEnhancedCashFlowTransactionsEnhancedCashFlowTransactions])
+                out = utils.unmarshal_json(http_res.text, Optional[shared.EnhancedCashFlowTransactions])
                 res.enhanced_cash_flow_transactions = out
 
         return res
 
     def get_enhanced_financial_metrics(self, request: operations.GetEnhancedFinancialMetricsRequest) -> operations.GetEnhancedFinancialMetricsResponse:
-        r"""List finanicial metrics
+        r"""List financial metrics
         Gets all the available financial metrics for a given company, over one or more periods.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetEnhancedFinancialMetricsRequest, base_url, '/data/companies/{companyId}/connections/{connectionId}/assess/financialMetrics', request)
         
         query_params = utils.get_query_params(operations.GetEnhancedFinancialMetricsRequest, request)
         
         client = self._security_client
@@ -260,24 +257,47 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetEnhancedFinancialMetricsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetEnhancedFinancialMetrics200ApplicationJSON])
-                res.get_enhanced_financial_metrics_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.FinancialMetrics])
+                res.financial_metrics = out
+
+        return res
+
+    def get_enhanced_invoices_report(self, request: operations.GetEnhancedInvoicesReportRequest) -> operations.GetEnhancedInvoicesReportResponse:
+        r"""Enhanced Invoices Report
+        Gets a list of invoices linked to the corresponding banking transaction
+        """
+        base_url = self._server_url
+        
+        url = utils.generate_url(operations.GetEnhancedInvoicesReportRequest, base_url, '/companies/{companyId}/reports/enhancedInvoices', request)
+        
+        query_params = utils.get_query_params(operations.GetEnhancedInvoicesReportRequest, request)
+        
+        client = self._security_client
+        
+        http_res = client.request('GET', url, params=query_params)
+        content_type = http_res.headers.get('Content-Type')
+
+        res = operations.GetEnhancedInvoicesReportResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        
+        if http_res.status_code == 200:
+            if utils.match_content_type(content_type, 'application/json'):
+                out = utils.unmarshal_json(http_res.text, Optional[shared.EnhancedInvoicesReport])
+                res.enhanced_invoices_report = out
 
         return res
 
     def get_enhanced_profit_and_loss(self, request: operations.GetEnhancedProfitAndLossRequest) -> operations.GetEnhancedProfitAndLossResponse:
         r"""Enhanced Profit and Loss
         Gets a fully categorized profit and loss statement for a given company, over one or more period(s).
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetEnhancedProfitAndLossRequest, base_url, '/data/companies/{companyId}/connections/{connectionId}/assess/enhancedProfitAndLoss', request)
         
         query_params = utils.get_query_params(operations.GetEnhancedProfitAndLossRequest, request)
         
         client = self._security_client
@@ -285,61 +305,59 @@
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetEnhancedProfitAndLossResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetEnhancedProfitAndLoss200ApplicationJSON])
-                res.get_enhanced_profit_and_loss_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Report])
+                res.report = out
 
         return res
 
     def get_recurring_revenue_metrics(self, request: operations.GetRecurringRevenueMetricsRequest) -> operations.GetRecurringRevenueMetricsResponse:
         r"""Get key metrics for subscription revenue
         Gets key metrics for subscription revenue.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.GetRecurringRevenueMetricsRequest, base_url, '/data/companies/{companyId}/connections/{connectionId}/assess/subscriptions/mrr', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.GetRecurringRevenueMetricsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetRecurringRevenueMetrics200ApplicationJSON])
-                res.get_recurring_revenue_metrics_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Report])
+                res.report = out
 
         return res
 
     def request_recurring_revenue_metrics(self, request: operations.RequestRecurringRevenueMetricsRequest) -> operations.RequestRecurringRevenueMetricsResponse:
         r"""Request production of key subscription revenue metrics
         Request production of key subscription revenue metrics.
         """
-        
         base_url = self._server_url
         
         url = utils.generate_url(operations.RequestRecurringRevenueMetricsRequest, base_url, '/data/companies/{companyId}/connections/{connectionId}/assess/subscriptions/process', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
         res = operations.RequestRecurringRevenueMetricsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.RequestRecurringRevenueMetrics200ApplicationJSON])
-                res.request_recurring_revenue_metrics_200_application_json_object = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Report])
+                res.report = out
 
         return res
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `codat-assess-0.5.1/src/codat/sdk.py` & `codat-assess-0.9.6/src/codat/sdk.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,64 @@
-__doc__ = """ SDK Documentation: Codat's Assess API enable you to make smarter credit decisions on your small business customers. Assess enriches your customer's accounting, commerce and banking data to surface actionable insights you didn't have before.
+"""Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
-[Read more...](https://www.codat.io/assess/)
-
-[See our OpenAPI spec](https://github.com/codatio/oas) """
 import requests as requests_http
 from . import utils
 from .categories import Categories
 from .data_integrity import DataIntegrity
 from .excel_reports import ExcelReports
 from .reports import Reports
 from codat.models import shared
 
 SERVERS = [
-	"https://api.codat.io",
+    "https://api.codat.io",
+    r"""Production"""
 ]
+"""Contains the list of servers available to the SDK"""
 
 class Codat:
-    r"""SDK Documentation: Codat's Assess API enable you to make smarter credit decisions on your small business customers. Assess enriches your customer's accounting, commerce and banking data to surface actionable insights you didn't have before.
+    r"""Codat's financial insights API
+    Codat's Assess API enable you to make smarter credit decisions on your small business customers. Assess enriches your customer's accounting, commerce and banking data to surface actionable insights you didn't have before.
     
     [Read more...](https://www.codat.io/assess/)
     
-    [See our OpenAPI spec](https://github.com/codatio/oas) """
+    [See our OpenAPI spec](https://github.com/codatio/oas)
+    """
     categories: Categories
+    r"""Categorisation"""
     data_integrity: DataIntegrity
+    r"""Data integrity is important"""
     excel_reports: ExcelReports
+    r"""Downloadable reports"""
     reports: Reports
-    
+    r"""Data integrity is important"""
+
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str = SERVERS[0]
     _language: str = "python"
-    _sdk_version: str = "0.5.1"
-    _gen_version: str = "1.12.1"
+    _sdk_version: str = "0.9.6"
+    _gen_version: str = "2.16.7"
 
     def __init__(self,
                  security: shared.Security = None,
                  server_url: str = None,
                  url_params: dict[str, str] = None,
                  client: requests_http.Session = None
                  ) -> None:
+        """Instantiates the SDK configuring it with the provided parameters.
+        
+        :param security: The security details required for authentication
+        :type security: shared.Security
+        :param server_url: The server URL to use for all operations
+        :type server_url: str
+        :param url_params: Parameters to optionally template the server URL with
+        :type url_params: dict[str, str]
+        :param client: The requests.Session HTTP client to use for all operations
+        :type client: requests_http.Session        
+        """
         self._client = requests_http.Session()
         
         
         if server_url is not None:
             if url_params is not None:
                 self._server_url = utils.template_url(server_url, url_params)
             else:
```

### Comparing `codat-assess-0.5.1/src/codat/utils/retries.py` & `codat-assess-0.9.6/src/codat/utils/retries.py`

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

### Comparing `codat-assess-0.5.1/src/codat/utils/utils.py` & `codat-assess-0.9.6/src/codat/utils/utils.py`

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

### Comparing `codat-assess-0.5.1/src/codat_assess.egg-info/PKG-INFO` & `codat-assess-0.9.6/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: codat-assess
-Version: 0.5.1
-Summary: Python Client SDK Generated by Speakeasy
-Home-page: UNKNOWN
-Author: Speakeasy
-License: UNKNOWN
-Platform: UNKNOWN
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-
 # codat-assess
 
 <!-- Start SDK Installation -->
 ## SDK Installation
 
 ```bash
 pip install codat-assess
@@ -29,28 +18,28 @@
     security=shared.Security(
         auth_header="YOUR_API_KEY_HERE",
     ),
 )
 
 
 req = operations.GetAccountCategoryRequest(
-    account_id="unde",
-    company_id="deserunt",
-    connection_id="porro",
+    account_id="corrupti",
+    company_id="8a210b68-6988-11ed-a1eb-0242ac120002",
+    connection_id="2e9d2c44-f675-40ba-8049-353bfcb5e171",
 )
     
 res = s.categories.get_account_category(req)
 
 if res.categorised_account is not None:
     # handle response
 ```
 <!-- End SDK Example Usage -->
 
 <!-- Start SDK Available Operations -->
-## SDK Available Operations
+## Available Resources and Operations
 
 
 ### categories
 
 * `get_account_category` - Get suggested and/or confirmed category for a specific account
 * `list_accounts_categories` - List suggested and confirmed account categories
 * `list_available_account_categories` - List account categories
@@ -61,32 +50,32 @@
 
 * `get_data_integrity_details` - Lists data integrity details for date type
 * `get_data_integrity_status` - Get data integrity status
 * `get_data_integrity_summaries` - Get data integrity summary
 
 ### excel_reports
 
+* `download_excel_report` - Download generated excel report
+* `generate_excel_report` - Generate an Excel report
 * `get_accounting_marketing_metrics` - Get the marketing metrics from an accounting source for a given company.
 * `get_excel_report` - Download generated excel report
-* `make_request_to_download_excel_report` - Request an Excel report for download
-* `request_excel_report_for_download` - Request an Excel report for download
+* `get_excel_report_generation_status` - Get status of Excel report
 
 ### reports
 
 * `get_accounts_for_enhanced_balance_sheet` - Enhanced Balance Sheet Accounts
 * `get_accounts_for_enhanced_profit_and_loss` - Enhanced Profit and Loss Accounts
 * `get_commerce_customer_retention_metrics` - Get the customer retention metrics for a specific company.
 * `get_commerce_lifetime_value_metrics` - Get the lifetime value metric for a specific company.
 * `get_commerce_orders_metrics` - Get order information for a specific company
 * `get_commerce_refunds_metrics` - Get the refunds information for a specific company
 * `get_commerce_revenue_metrics` - Commerce Revenue Metrics
 * `get_enhanced_balance_sheet` - Enhanced Balance Sheet
 * `get_enhanced_cash_flow_transactions` - Get enhanced cash flow report
-* `get_enhanced_financial_metrics` - List finanicial metrics
+* `get_enhanced_financial_metrics` - List financial metrics
+* `get_enhanced_invoices_report` - Enhanced Invoices Report
 * `get_enhanced_profit_and_loss` - Enhanced Profit and Loss
 * `get_recurring_revenue_metrics` - Get key metrics for subscription revenue
 * `request_recurring_revenue_metrics` - Request production of key subscription revenue metrics
 <!-- End SDK Available Operations -->
 
 ### SDK Generated by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)
-
-
```

