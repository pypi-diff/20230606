# Comparing `tmp/codat-commerce-0.7.0.tar.gz` & `tmp/codat-commerce-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codat-commerce-0.7.0.tar", last modified: Wed Mar 22 13:46:56 2023, max compression
+gzip compressed data, was "codat-commerce-0.9.6.tar", last modified: Wed Apr  5 09:29:20 2023, max compression
```

## Comparing `codat-commerce-0.7.0.tar` & `codat-commerce-0.9.6.tar`

### file list

```diff
@@ -1,46 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:46:56.091451 codat-commerce-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-03-22 13:46:56.091451 codat-commerce-0.7.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     1597 2023-03-22 13:46:47.000000 codat-commerce-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 13:46:56.091451 codat-commerce-0.7.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1107 2023-03-22 13:46:47.000000 codat-commerce-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:46:56.087450 codat-commerce-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:46:56.087450 codat-commerce-0.7.0/src/codat/
--rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-03-22 13:46:47.000000 codat-commerce-0.7.0/src/codat/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2043 2023-03-22 13:46:47.000000 codat-commerce-0.7.0/src/codat/company_info.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2037 2023-03-22 13:46:47.000000 codat-commerce-0.7.0/src/codat/customers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1980 2023-03-22 13:46:47.000000 codat-commerce-0.7.0/src/codat/disputes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2040 2023-03-22 13:46:47.000000 codat-commerce-0.7.0/src/codat/locations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:46:56.087450 codat-commerce-0.7.0/src/codat/models/
--rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-03-22 13:46:47.000000 codat-commerce-0.7.0/src/codat/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:46:56.087450 codat-commerce-0.7.0/src/codat/models/operations/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5849 2023-03-22 13:46:47.000000 codat-commerce-0.7.0/src/codat/models/operations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9150 2023-03-22 13:46:47.000000 codat-commerce-0.7.0/src/codat/models/operations/get_commerce_info.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3702 2023-03-22 13:46:47.000000 codat-commerce-0.7.0/src/codat/models/operations/get_companies_companyid_connections_connectionid_data_commerce_taxcomponents.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9569 2023-03-22 13:46:47.000000 codat-commerce-0.7.0/src/codat/models/operations/list_commerce_customers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9076 2023-03-22 13:46:47.000000 codat-commerce-0.7.0/src/codat/models/operations/list_commerce_disputes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8008 2023-03-22 13:46:47.000000 codat-commerce-0.7.0/src/codat/models/operations/list_commerce_locations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21236 2023-03-22 13:46:47.000000 codat-commerce-0.7.0/src/codat/models/operations/list_commerce_orders.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6706 2023-03-22 13:46:47.000000 codat-commerce-0.7.0/src/codat/models/operations/list_commerce_paymentmethods.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8798 2023-03-22 13:46:47.000000 codat-commerce-0.7.0/src/codat/models/operations/list_commerce_payments.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7134 2023-03-22 13:46:47.000000 codat-commerce-0.7.0/src/codat/models/operations/list_commerce_productcategories.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10492 2023-03-22 13:46:47.000000 codat-commerce-0.7.0/src/codat/models/operations/list_commerce_products.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9585 2023-03-22 13:46:47.000000 codat-commerce-0.7.0/src/codat/models/operations/list_commerce_transactions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:46:56.087450 codat-commerce-0.7.0/src/codat/models/shared/
--rwxr-xr-x   0 runner    (1001) docker     (123)      124 2023-03-22 13:46:47.000000 codat-commerce-0.7.0/src/codat/models/shared/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      337 2023-03-22 13:46:47.000000 codat-commerce-0.7.0/src/codat/models/shared/security.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2005 2023-03-22 13:46:47.000000 codat-commerce-0.7.0/src/codat/orders.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3305 2023-03-22 13:46:47.000000 codat-commerce-0.7.0/src/codat/payments.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3433 2023-03-22 13:46:47.000000 codat-commerce-0.7.0/src/codat/products.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5638 2023-03-22 13:46:47.000000 codat-commerce-0.7.0/src/codat/sdk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2475 2023-03-22 13:46:47.000000 codat-commerce-0.7.0/src/codat/tax_components.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2175 2023-03-22 13:46:47.000000 codat-commerce-0.7.0/src/codat/transactions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:46:56.087450 codat-commerce-0.7.0/src/codat/utils/
--rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-03-22 13:46:47.000000 codat-commerce-0.7.0/src/codat/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-03-22 13:46:47.000000 codat-commerce-0.7.0/src/codat/utils/retries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24799 2023-03-22 13:46:47.000000 codat-commerce-0.7.0/src/codat/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:46:56.091451 codat-commerce-0.7.0/src/codat_commerce.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-03-22 13:46:56.000000 codat-commerce-0.7.0/src/codat_commerce.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-03-22 13:46:56.000000 codat-commerce-0.7.0/src/codat_commerce.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 13:46:56.000000 codat-commerce-0.7.0/src/codat_commerce.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-03-22 13:46:56.000000 codat-commerce-0.7.0/src/codat_commerce.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-22 13:46:56.000000 codat-commerce-0.7.0/src/codat_commerce.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:29:20.737477 codat-commerce-0.9.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-05 09:29:20.737477 codat-commerce-0.9.6/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1454 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 09:29:20.737477 codat-commerce-0.9.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1107 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:29:20.729477 codat-commerce-0.9.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:29:20.729477 codat-commerce-0.9.6/src/codat/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       95 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2012 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/company_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1979 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/customers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1921 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/disputes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2007 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/locations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:29:20.729477 codat-commerce-0.9.6/src/codat/models/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       76 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:29:20.729477 codat-commerce-0.9.6/src/codat/models/operations/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      982 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/operations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      936 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/operations/get_company_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      950 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/operations/get_tax_components.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1884 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/operations/list_customers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1877 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/operations/list_disputes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      964 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/operations/list_locations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1863 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/operations/list_orders.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1920 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/operations/list_payment_methods.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1877 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/operations/list_payments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1941 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/operations/list_product_categories.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1877 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/operations/list_products.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1905 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/operations/list_transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:29:20.737477 codat-commerce-0.9.6/src/codat/models/shared/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2609 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1241 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/accountbalance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1975 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/address.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      325 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/addresstype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7928 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/companyinfo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5555 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/customer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      712 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/customerref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1165 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/customers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7172 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/dispute.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1160 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/disputes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      593 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/disputestatus_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      500 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/href.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1013 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/links.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      729 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/locationref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3609 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/locations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1177 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/locationsresponse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9475 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/order.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      828 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/orderdiscountallocation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3283 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/orderlineitem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1150 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/orders.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7413 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/payment.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3526 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/paymentmethod.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      739 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/paymentmethodref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1190 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/paymentmethods.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      288 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/paymentmethodstatus_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6583 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/paymentref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1160 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/payments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      349 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/paymentstatus_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      479 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/paymenttype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      723 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/phonenumber.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      320 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/phonenumbertype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2196 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/product.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1201 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/productcategories.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3987 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/productcategory.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      855 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/productinventory.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      875 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/productinventorylocation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1122 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/productprice.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      728 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/productref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1160 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/products.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6823 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/productvariant.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      777 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/productvariantref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      261 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/productvariantstatus_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      646 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/recordref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      337 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/security.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2259 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/servicecharge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      323 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/servicechargetype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3911 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/taxcomponent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1006 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/taxcomponentallocation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      774 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/taxcomponentref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      634 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/taxcomponents.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7888 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/transaction.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1180 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/transactions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      750 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/transactionsourceref.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      299 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/transactionsourcetype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1038 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/models/shared/transactiontype_enum.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1944 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/orders.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3186 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/payments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3317 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/products.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5636 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/sdk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2039 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/tax_components.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2120 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:29:20.737477 codat-commerce-0.9.6/src/codat/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      120 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3705 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/utils/retries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24799 2023-04-05 09:29:09.000000 codat-commerce-0.9.6/src/codat/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 09:29:20.737477 codat-commerce-0.9.6/src/codat_commerce.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-04-05 09:29:20.000000 codat-commerce-0.9.6/src/codat_commerce.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-04-05 09:29:20.000000 codat-commerce-0.9.6/src/codat_commerce.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 09:29:20.000000 codat-commerce-0.9.6/src/codat_commerce.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-05 09:29:20.000000 codat-commerce-0.9.6/src/codat_commerce.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-05 09:29:20.000000 codat-commerce-0.9.6/src/codat_commerce.egg-info/top_level.txt
```

### Comparing `codat-commerce-0.7.0/PKG-INFO` & `codat-commerce-0.9.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codat-commerce
-Version: 0.7.0
+Version: 0.9.6
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -28,65 +28,65 @@
 s = codat.Codat(
     security=shared.Security(
         auth_header="YOUR_API_KEY_HERE",
     ),
 )
 
 
-req = operations.GetCommerceInfoRequest(
+req = operations.GetCompanyInfoRequest(
     company_id="8a210b68-6988-11ed-a1eb-0242ac120002",
     connection_id="2e9d2c44-f675-40ba-8049-353bfcb5e171",
 )
     
-res = s.company_info.get_commerce_info(req)
+res = s.company_info.get_company_info(req)
 
-if res.source_modified_date is not None:
+if res.company_info is not None:
     # handle response
 ```
 <!-- End SDK Example Usage -->
 
 <!-- Start SDK Available Operations -->
-## SDK Available Operations
+## Available Resources and Operations
 
 
 ### company_info
 
-* `get_commerce_info` - Get company info
+* `get_company_info` - Get company info
 
 ### customers
 
-* `list_commerce_customers` - List customers
+* `list_customers` - List customers
 
 ### disputes
 
-* `list_commerce_disputes` - List disputes
+* `list_disputes` - List disputes
 
 ### locations
 
-* `list_commerce_locations` - List locations
+* `list_locations` - List locations
 
 ### orders
 
-* `list_commerce_orders` - List orders
+* `list_orders` - List orders
 
 ### payments
 
-* `list_commerce_payment_methods` - List payment methods
-* `list_commerce_payments` - List payments
+* `list_payment_methods` - List payment methods
+* `list_payments` - List payments
 
 ### products
 
-* `list_commerce_product_categories` - List product categories
-* `list_commerce_products` - List products
+* `list_product_categories` - List product categories
+* `list_products` - List products
 
 ### tax_components
 
-* `get_companies_company_id_connections_connection_id_data_commerce_tax_components` - List tax components
+* `get_tax_components` - List tax components
 
 ### transactions
 
-* `list_commerce_transactions` - List transactions
+* `list_transactions` - List transactions
 <!-- End SDK Available Operations -->
 
 ### SDK Generated by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)
```

### Comparing `codat-commerce-0.7.0/README.md` & `codat-commerce-0.9.6/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -17,63 +17,63 @@
 s = codat.Codat(
     security=shared.Security(
         auth_header="YOUR_API_KEY_HERE",
     ),
 )
 
 
-req = operations.GetCommerceInfoRequest(
+req = operations.GetCompanyInfoRequest(
     company_id="8a210b68-6988-11ed-a1eb-0242ac120002",
     connection_id="2e9d2c44-f675-40ba-8049-353bfcb5e171",
 )
     
-res = s.company_info.get_commerce_info(req)
+res = s.company_info.get_company_info(req)
 
-if res.source_modified_date is not None:
+if res.company_info is not None:
     # handle response
 ```
 <!-- End SDK Example Usage -->
 
 <!-- Start SDK Available Operations -->
-## SDK Available Operations
+## Available Resources and Operations
 
 
 ### company_info
 
-* `get_commerce_info` - Get company info
+* `get_company_info` - Get company info
 
 ### customers
 
-* `list_commerce_customers` - List customers
+* `list_customers` - List customers
 
 ### disputes
 
-* `list_commerce_disputes` - List disputes
+* `list_disputes` - List disputes
 
 ### locations
 
-* `list_commerce_locations` - List locations
+* `list_locations` - List locations
 
 ### orders
 
-* `list_commerce_orders` - List orders
+* `list_orders` - List orders
 
 ### payments
 
-* `list_commerce_payment_methods` - List payment methods
-* `list_commerce_payments` - List payments
+* `list_payment_methods` - List payment methods
+* `list_payments` - List payments
 
 ### products
 
-* `list_commerce_product_categories` - List product categories
-* `list_commerce_products` - List products
+* `list_product_categories` - List product categories
+* `list_products` - List products
 
 ### tax_components
 
-* `get_companies_company_id_connections_connection_id_data_commerce_tax_components` - List tax components
+* `get_tax_components` - List tax components
 
 ### transactions
 
-* `list_commerce_transactions` - List transactions
+* `list_transactions` - List transactions
 <!-- End SDK Available Operations -->
 
 ### SDK Generated by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)
```

### Comparing `codat-commerce-0.7.0/setup.py` & `codat-commerce-0.9.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="codat-commerce",
-    version="0.7.0",
+    version="0.9.6",
     author="Speakeasy",
     description="Python Client SDK Generated by Speakeasy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi==2022.12.07",
```

### Comparing `codat-commerce-0.7.0/src/codat/company_info.py` & `codat-commerce-0.9.6/src/codat/orders.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from . import utils
-from codat.models import operations
+from codat.models import operations, shared
 from typing import Optional
 
-class CompanyInfo:
+class Orders:
     r"""Retrieve standardized data from linked commerce platforms."""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
@@ -18,33 +18,32 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    def get_commerce_info(self, request: operations.GetCommerceInfoRequest) -> operations.GetCommerceInfoResponse:
-        r"""Get company info
-        Retrieve information about the company, as seen in the commerce platform.
-        
-        This may include information like addresses, tax registration details and social media or website information.
+    def list_orders(self, request: operations.ListOrdersRequest) -> operations.ListOrdersResponse:
+        r"""List orders
+        Get a list of orders placed or held on the linked commerce platform
         """
         base_url = self._server_url
         
-        url = utils.generate_url(operations.GetCommerceInfoRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/commerce-info', request)
+        url = utils.generate_url(operations.ListOrdersRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/commerce-orders', request)
         
+        query_params = utils.get_query_params(operations.ListOrdersRequest, request)
         
         client = self._security_client
         
-        http_res = client.request('GET', url)
+        http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.GetCommerceInfoResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.ListOrdersResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.GetCommerceInfoSourceModifiedDate])
-                res.source_modified_date = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Orders])
+                res.orders = out
 
         return res
```

### Comparing `codat-commerce-0.7.0/src/codat/customers.py` & `codat-commerce-0.9.6/src/codat/customers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from . import utils
-from codat.models import operations
+from codat.models import operations, shared
 from typing import Optional
 
 class Customers:
     r"""Retrieve standardized data from linked commerce platforms."""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
@@ -18,32 +18,32 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    def list_commerce_customers(self, request: operations.ListCommerceCustomersRequest) -> operations.ListCommerceCustomersResponse:
+    def list_customers(self, request: operations.ListCustomersRequest) -> operations.ListCustomersResponse:
         r"""List customers
         List all commerce customers for the given company and data connection
         """
         base_url = self._server_url
         
-        url = utils.generate_url(operations.ListCommerceCustomersRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/commerce-customers', request)
+        url = utils.generate_url(operations.ListCustomersRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/commerce-customers', request)
         
-        query_params = utils.get_query_params(operations.ListCommerceCustomersRequest, request)
+        query_params = utils.get_query_params(operations.ListCustomersRequest, request)
         
         client = self._security_client
         
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.ListCommerceCustomersResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.ListCustomersResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.ListCommerceCustomersLinks])
-                res.links = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Customers])
+                res.customers = out
 
         return res
```

### Comparing `codat-commerce-0.7.0/src/codat/disputes.py` & `codat-commerce-0.9.6/src/codat/disputes.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from . import utils
-from codat.models import operations
+from codat.models import operations, shared
 from typing import Optional
 
 class Disputes:
     r"""Retrieve standardized data from linked commerce platforms."""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
@@ -18,32 +18,32 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    def list_commerce_disputes(self, request: operations.ListCommerceDisputesRequest) -> operations.ListCommerceDisputesResponse:
+    def list_disputes(self, request: operations.ListDisputesRequest) -> operations.ListDisputesResponse:
         r"""List disputes
         List commerce disputes
         """
         base_url = self._server_url
         
-        url = utils.generate_url(operations.ListCommerceDisputesRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/commerce-disputes', request)
+        url = utils.generate_url(operations.ListDisputesRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/commerce-disputes', request)
         
-        query_params = utils.get_query_params(operations.ListCommerceDisputesRequest, request)
+        query_params = utils.get_query_params(operations.ListDisputesRequest, request)
         
         client = self._security_client
         
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.ListCommerceDisputesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.ListDisputesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.ListCommerceDisputesLinks])
-                res.links = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Disputes])
+                res.disputes = out
 
         return res
```

### Comparing `codat-commerce-0.7.0/src/codat/locations.py` & `codat-commerce-0.9.6/src/codat/locations.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from . import utils
-from codat.models import operations
+from codat.models import operations, shared
 from typing import Optional
 
 class Locations:
     r"""Retrieve standardized data from linked commerce platforms."""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
@@ -18,33 +18,33 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    def list_commerce_locations(self, request: operations.ListCommerceLocationsRequest) -> operations.ListCommerceLocationsResponse:
+    def list_locations(self, request: operations.ListLocationsRequest) -> operations.ListLocationsResponse:
         r"""List locations
         Retrieve a list of locations as seen in the commerce platform.
         
         A `location` is a geographic place at which stocks of products may be held, or from where orders were placed.
         """
         base_url = self._server_url
         
-        url = utils.generate_url(operations.ListCommerceLocationsRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/commerce-locations', request)
+        url = utils.generate_url(operations.ListLocationsRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/commerce-locations', request)
         
         
         client = self._security_client
         
         http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.ListCommerceLocationsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.ListLocationsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.ListCommerceLocationsLinks])
-                res.links = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.LocationsResponse])
+                res.locations_response = out
 
         return res
```

### Comparing `codat-commerce-0.7.0/src/codat/models/operations/get_companies_companyid_connections_connectionid_data_commerce_taxcomponents.py` & `codat-commerce-0.9.6/src/codat/models/shared/product.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,55 +1,32 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-import dateutil.parser
-import requests as requests_http
+from ..shared import productvariant as shared_productvariant
 from codat import utils
 from dataclasses_json import Undefined, dataclass_json
-from datetime import datetime
-from marshmallow import fields
 from typing import Optional
 
 
-@dataclasses.dataclass
-class GetCompaniesCompanyIDConnectionsConnectionIDDataCommerceTaxComponentsRequest:
-    
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
-    connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})  
-    
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class GetCompaniesCompanyIDConnectionsConnectionIDDataCommerceTaxComponents200ApplicationJSONSourceModifiedDate:
+class Product:
+    r"""A Product is an item in the company's inventory, and includes information about the price and quantity of all products, and variants thereof, available for sale.
+    
+    Explore our [data coverage](https://knowledge.codat.io/supported-features/commerce?view=tab-by-data-type&dataType=commerce-products) for this data type.
+    """
     
     id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
     r"""A unique, persistent identifier for this record"""  
-    name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
-    r"""Name of the Tax Rate Component in the source commerce platform."""  
-    is_compound: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isCompound'), 'exclude': lambda f: f is None }})
-    r"""The Boolean flag to indicate when a Tax Rate Component compounds on a sale."""  
-    modified_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    r"""The date on which this record was last modified in Codat."""  
-    rate: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('rate'), 'exclude': lambda f: f is None }})
-    r"""Rate of taxation represented as a fraction of the net price (typically in the range 0.00 - 1.00)."""  
-    source_modified_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceModifiedDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    r"""The date on which this record was last modified in the originating system"""  
-    
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class GetCompaniesCompanyIDConnectionsConnectionIDDataCommerceTaxComponents200ApplicationJSON:
-    r"""OK"""
-    
-    tax_components: Optional[list[GetCompaniesCompanyIDConnectionsConnectionIDDataCommerceTaxComponents200ApplicationJSONSourceModifiedDate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('taxComponents'), 'exclude': lambda f: f is None }})  
-    
-
-@dataclasses.dataclass
-class GetCompaniesCompanyIDConnectionsConnectionIDDataCommerceTaxComponentsResponse:
-    
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
-    get_companies_company_id_connections_connection_id_data_commerce_tax_components_200_application_json_object: Optional[GetCompaniesCompanyIDConnectionsConnectionIDDataCommerceTaxComponents200ApplicationJSON] = dataclasses.field(default=None)
-    r"""OK"""  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
+    categorization: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('categorization'), 'exclude': lambda f: f is None }})
+    r"""Retail category that the product is assigned to"""  
+    description: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('description'), 'exclude': lambda f: f is None }})
+    r"""Description of the product recorded in the commerce or point of sale platform."""  
+    is_gift_card: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isGiftCard'), 'exclude': lambda f: f is None }})
+    r"""Whether the product represents a gift card or voucher that
+    can be redeemed in the commerce or POS platform
+    """  
+    name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
+    r"""Name of the product in the commerce or POS system"""  
+    variants: Optional[list[shared_productvariant.ProductVariant]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('variants'), 'exclude': lambda f: f is None }})
```

### Comparing `codat-commerce-0.7.0/src/codat/models/operations/list_commerce_locations.py` & `codat-commerce-0.9.6/src/codat/models/shared/productvariant.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,131 +1,102 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-import dateutil.parser
-import requests as requests_http
+from ..shared import productinventory as shared_productinventory
+from ..shared import productprice as shared_productprice
+from ..shared import productvariantstatus_enum as shared_productvariantstatus_enum
 from codat import utils
 from dataclasses_json import Undefined, dataclass_json
-from datetime import datetime
-from enum import Enum
-from marshmallow import fields
 from typing import Optional
 
 
-@dataclasses.dataclass
-class ListCommerceLocationsRequest:
-    
-    company_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'companyId', 'style': 'simple', 'explode': False }})  
-    connection_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'connectionId', 'style': 'simple', 'explode': False }})  
-    
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class ListCommerceLocationsLinksLinksCurrent:
-    
-    href: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('href') }})  
-    
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class ListCommerceLocationsLinksLinksNext:
-    
-    href: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('href'), 'exclude': lambda f: f is None }})  
-    
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class ListCommerceLocationsLinksLinksPrevious:
-    
-    href: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('href'), 'exclude': lambda f: f is None }})  
-    
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class ListCommerceLocationsLinksLinksSelf:
-    
-    href: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('href') }})  
-    
-
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class ListCommerceLocationsLinksLinks:
+class ProductVariant:
+    r"""Represents a variation of a product available for sale, for example an item of clothing that may be available for sale in multiple sizes and colors."""
     
-    current: ListCommerceLocationsLinksLinksCurrent = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('current') }})  
-    self_: ListCommerceLocationsLinksLinksSelf = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('self') }})  
-    next: Optional[ListCommerceLocationsLinksLinksNext] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})  
-    previous: Optional[ListCommerceLocationsLinksLinksPrevious] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})  
-    
-class ListCommerceLocationsLinksSourceModifiedDateAddressTypeEnum(str, Enum):
-    BILLING = "Billing"
-    DELIVERY = "Delivery"
-    INVENTORY = "Inventory"
-
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class ListCommerceLocationsLinksSourceModifiedDateAddress:
-    r"""Address associated with the location"""
+    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
+    r"""A unique, persistent identifier for this record"""  
+    barcode: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('barcode'), 'exclude': lambda f: f is None }})
+    r"""Unique product number of the variant. This might be a barcode, UPC, ISBN, etc."""  
+    created_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('createdDate'), 'exclude': lambda f: f is None }})
+    r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
+    
+    ```
+    2020-10-08T22:40:50Z
+    2021-01-01T00:00:00
+    ```
     
-    city: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('city'), 'exclude': lambda f: f is None }})
-    r"""The third line of the address, or city"""  
-    country: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('country'), 'exclude': lambda f: f is None }})
-    r"""The country for the address"""  
-    line1: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('line1'), 'exclude': lambda f: f is None }})
-    r"""The first line of the address"""  
-    line2: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('line2'), 'exclude': lambda f: f is None }})
-    r"""The second line of the address"""  
-    postal_code: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('postalCode'), 'exclude': lambda f: f is None }})
-    r"""The postal (or zip) code for the address"""  
-    region: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('region'), 'exclude': lambda f: f is None }})
-    r"""The fourth line of the address, or region"""  
-    type: Optional[ListCommerceLocationsLinksSourceModifiedDateAddressTypeEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})  
     
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class ListCommerceLocationsLinksSourceModifiedDate:
-    r"""The Locations datatype holds information on geographic locations at which stocks of products may be held, as referenced in the Products data type.
-    
-    Locations also holds information on geographic locations where orders were placed, as referenced in the Orders data type.
     
-    From the Locations endpoints you can retrieve:
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
+    inventory: Optional[list[shared_productinventory.ProductInventory]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('inventory'), 'exclude': lambda f: f is None }})
+    r"""Information about the total inventory as well as the locations inventory is in."""  
+    is_tax_enabled: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('isTaxEnabled'), 'exclude': lambda f: f is None }})
+    r"""Whether sales taxes are enabled for this product variant."""  
+    modified_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedDate'), 'exclude': lambda f: f is None }})
+    r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
+    
+    ```
+    2020-10-08T22:40:50Z
+    2021-01-01T00:00:00
+    ```
     
-    A list of all the Locations of a commerce company: `GET /companies/{companyId}/connections/{connectionId}/data/commerce-locations`.
-    The details of an individual location: `GET /companies/{companyId}/connections/{connectionId}/data/commerce-locations/{locationId}`.
     
-    """
     
-    id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('id') }})
-    r"""A unique, persistent identifier for this record"""  
-    address: Optional[ListCommerceLocationsLinksSourceModifiedDateAddress] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('address'), 'exclude': lambda f: f is None }})
-    r"""Address associated with the location"""  
-    modified_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modifiedDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    r"""The date on which this record was last modified in Codat."""  
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
     name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
-    r"""Name of this location"""  
-    source_modified_date: Optional[datetime] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceModifiedDate'), 'encoder': utils.datetimeisoformat(True), 'decoder': dateutil.parser.isoparse, 'mm_field': fields.DateTime(format='iso'), 'exclude': lambda f: f is None }})
-    r"""The date on which this record was last modified in the originating system"""  
-    
-
-@dataclass_json(undefined=Undefined.EXCLUDE)
-@dataclasses.dataclass
-class ListCommerceLocationsLinks:
-    r"""Codat's Paging Model"""
+    r"""Name of the product recorded in the commerce or point of sale platform."""  
+    prices: Optional[list[shared_productprice.ProductPrice]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('prices'), 'exclude': lambda f: f is None }})
+    r"""Prices for the product variants in different currencies."""  
+    shipping_required: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('shippingRequired'), 'exclude': lambda f: f is None }})
+    r"""Indicates whether or not the product requires physical delivery."""  
+    sku: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sku'), 'exclude': lambda f: f is None }})
+    r"""SKU (stock keeping unit) of the variant, as defined by the merchant."""  
+    source_modified_date: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sourceModifiedDate'), 'exclude': lambda f: f is None }})
+    r"""In Codat's data model, dates and times are represented using the <a class=\\"external\\" href=\\"https://en.wikipedia.org/wiki/ISO_8601\\" target=\\"_blank\\">ISO 8601 standard</a>. Date and time fields are formatted as strings; for example:
+    
+    ```
+    2020-10-08T22:40:50Z
+    2021-01-01T00:00:00
+    ```
     
-    links: ListCommerceLocationsLinksLinks = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('_links') }})  
-    page_number: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageNumber') }})  
-    page_size: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('pageSize') }})  
-    total_results: int = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('totalResults') }})  
-    results: Optional[list[ListCommerceLocationsLinksSourceModifiedDate]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})  
     
-
-@dataclasses.dataclass
-class ListCommerceLocationsResponse:
     
-    content_type: str = dataclasses.field()  
-    status_code: int = dataclasses.field()  
-    links: Optional[ListCommerceLocationsLinks] = dataclasses.field(default=None)
-    r"""OK"""  
-    raw_response: Optional[requests_http.Response] = dataclasses.field(default=None)  
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
+    status: Optional[shared_productvariantstatus_enum.ProductVariantStatusEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})  
+    unit_of_measure: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unitOfMeasure'), 'exclude': lambda f: f is None }})
+    r"""Unit of measure for the variant, such as `kg` or `meters`."""  
+    vat_percentage: Optional[float] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('vatPercentage'), 'exclude': lambda f: f is None }})
+    r"""VAT rate for the product variant if sales taxes are enabled."""
```

### Comparing `codat-commerce-0.7.0/src/codat/orders.py` & `codat-commerce-0.9.6/src/codat/tax_components.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from . import utils
-from codat.models import operations
+from codat.models import operations, shared
 from typing import Optional
 
-class Orders:
+class TaxComponents:
     r"""Retrieve standardized data from linked commerce platforms."""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
     _language: str
     _sdk_version: str
     _gen_version: str
@@ -18,32 +18,31 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    def list_commerce_orders(self, request: operations.ListCommerceOrdersRequest) -> operations.ListCommerceOrdersResponse:
-        r"""List orders
-        Get a list of orders placed or held on the linked commerce platform
+    def get_tax_components(self, request: operations.GetTaxComponentsRequest) -> operations.GetTaxComponentsResponse:
+        r"""List tax components
+        This endpoint returns a lits of tax rates from the commerce platform, including tax rate names and values. This supports the mapping of tax rates from the commerce platform to the accounting platform.
         """
         base_url = self._server_url
         
-        url = utils.generate_url(operations.ListCommerceOrdersRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/commerce-orders', request)
+        url = utils.generate_url(operations.GetTaxComponentsRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/commerce-taxComponents', request)
         
-        query_params = utils.get_query_params(operations.ListCommerceOrdersRequest, request)
         
         client = self._security_client
         
-        http_res = client.request('GET', url, params=query_params)
+        http_res = client.request('GET', url)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.ListCommerceOrdersResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.GetTaxComponentsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.ListCommerceOrdersLinks])
-                res.links = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.TaxComponents])
+                res.tax_components = out
 
         return res
```

### Comparing `codat-commerce-0.7.0/src/codat/payments.py` & `codat-commerce-0.9.6/src/codat/payments.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from . import utils
-from codat.models import operations
+from codat.models import operations, shared
 from typing import Optional
 
 class Payments:
     r"""Retrieve standardized data from linked commerce platforms."""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
@@ -18,56 +18,56 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    def list_commerce_payment_methods(self, request: operations.ListCommercePaymentMethodsRequest) -> operations.ListCommercePaymentMethodsResponse:
+    def list_payment_methods(self, request: operations.ListPaymentMethodsRequest) -> operations.ListPaymentMethodsResponse:
         r"""List payment methods
         Retrieve a list of payment methods, such as card, cash or other online payment methods, as held in the linked commerce platform.
         """
         base_url = self._server_url
         
-        url = utils.generate_url(operations.ListCommercePaymentMethodsRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/commerce-paymentMethods', request)
+        url = utils.generate_url(operations.ListPaymentMethodsRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/commerce-paymentMethods', request)
         
-        query_params = utils.get_query_params(operations.ListCommercePaymentMethodsRequest, request)
+        query_params = utils.get_query_params(operations.ListPaymentMethodsRequest, request)
         
         client = self._security_client
         
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.ListCommercePaymentMethodsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.ListPaymentMethodsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.ListCommercePaymentMethodsLinks])
-                res.links = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.PaymentMethods])
+                res.payment_methods = out
 
         return res
 
-    def list_commerce_payments(self, request: operations.ListCommercePaymentsRequest) -> operations.ListCommercePaymentsResponse:
+    def list_payments(self, request: operations.ListPaymentsRequest) -> operations.ListPaymentsResponse:
         r"""List payments
         List commerce payments for the given company & data connection.
         """
         base_url = self._server_url
         
-        url = utils.generate_url(operations.ListCommercePaymentsRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/commerce-payments', request)
+        url = utils.generate_url(operations.ListPaymentsRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/commerce-payments', request)
         
-        query_params = utils.get_query_params(operations.ListCommercePaymentsRequest, request)
+        query_params = utils.get_query_params(operations.ListPaymentsRequest, request)
         
         client = self._security_client
         
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.ListCommercePaymentsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.ListPaymentsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.ListCommercePaymentsLinks])
-                res.links = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Payments])
+                res.payments = out
 
         return res
```

### Comparing `codat-commerce-0.7.0/src/codat/products.py` & `codat-commerce-0.9.6/src/codat/products.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from . import utils
-from codat.models import operations
+from codat.models import operations, shared
 from typing import Optional
 
 class Products:
     r"""Retrieve standardized data from linked commerce platforms."""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
@@ -18,56 +18,56 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    def list_commerce_product_categories(self, request: operations.ListCommerceProductCategoriesRequest) -> operations.ListCommerceProductCategoriesResponse:
+    def list_product_categories(self, request: operations.ListProductCategoriesRequest) -> operations.ListProductCategoriesResponse:
         r"""List product categories
         Product categories are used to classify a group of products together, either by type (eg \"Furniture\"), or sometimes by tax profile.
         """
         base_url = self._server_url
         
-        url = utils.generate_url(operations.ListCommerceProductCategoriesRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/commerce-productCategories', request)
+        url = utils.generate_url(operations.ListProductCategoriesRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/commerce-productCategories', request)
         
-        query_params = utils.get_query_params(operations.ListCommerceProductCategoriesRequest, request)
+        query_params = utils.get_query_params(operations.ListProductCategoriesRequest, request)
         
         client = self._security_client
         
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.ListCommerceProductCategoriesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.ListProductCategoriesResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.ListCommerceProductCategoriesLinks])
-                res.links = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.ProductCategories])
+                res.product_categories = out
 
         return res
 
-    def list_commerce_products(self, request: operations.ListCommerceProductsRequest) -> operations.ListCommerceProductsResponse:
+    def list_products(self, request: operations.ListProductsRequest) -> operations.ListProductsResponse:
         r"""List products
         The Products data type provides the company's product inventory, and includes the price and quantity of all products, and product variants, available for sale.
         """
         base_url = self._server_url
         
-        url = utils.generate_url(operations.ListCommerceProductsRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/commerce-products', request)
+        url = utils.generate_url(operations.ListProductsRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/commerce-products', request)
         
-        query_params = utils.get_query_params(operations.ListCommerceProductsRequest, request)
+        query_params = utils.get_query_params(operations.ListProductsRequest, request)
         
         client = self._security_client
         
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.ListCommerceProductsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.ListProductsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.ListCommerceProductsLinks])
-                res.links = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Products])
+                res.products = out
 
         return res
```

### Comparing `codat-commerce-0.7.0/src/codat/sdk.py` & `codat-commerce-0.9.6/src/codat/sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 SERVERS = [
     "https://api.codat.io",
     r"""Production"""
 ]
 """Contains the list of servers available to the SDK"""
 
 class Codat:
-    r"""Codat's standardized API for accessing commerce data 
+    r"""Codat's standardized API for accessing commerce data
     Codat's Commerce API allows you to access standardised data from over 11 commerce and POS systems.
     
     Standardize how you connect to your customers’ payment, PoS, and eCommerce systems. Retrieve orders, payouts, payments, and product data in the same way for all the leading commerce platforms.
     
     [Read more...](https://docs.codat.io/commerce-api/overview)
     
-    [See our OpenAPI spec](https://github.com/codatio/oas) 
+    [See our OpenAPI spec](https://github.com/codatio/oas)
     """
     company_info: CompanyInfo
     r"""Retrieve standardized data from linked commerce platforms."""
     customers: Customers
     r"""Retrieve standardized data from linked commerce platforms."""
     disputes: Disputes
     r"""Retrieve standardized data from linked commerce platforms."""
@@ -48,16 +48,16 @@
     transactions: Transactions
     r"""Retrieve standardized data from linked commerce platforms."""
 
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str = SERVERS[0]
     _language: str = "python"
-    _sdk_version: str = "0.7.0"
-    _gen_version: str = "2.13.0"
+    _sdk_version: str = "0.9.6"
+    _gen_version: str = "2.16.7"
 
     def __init__(self,
                  security: shared.Security = None,
                  server_url: str = None,
                  url_params: dict[str, str] = None,
                  client: requests_http.Session = None
                  ) -> None:
```

### Comparing `codat-commerce-0.7.0/src/codat/transactions.py` & `codat-commerce-0.9.6/src/codat/transactions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from . import utils
-from codat.models import operations
+from codat.models import operations, shared
 from typing import Optional
 
 class Transactions:
     r"""Retrieve standardized data from linked commerce platforms."""
     _client: requests_http.Session
     _security_client: requests_http.Session
     _server_url: str
@@ -18,32 +18,32 @@
         self._client = client
         self._security_client = security_client
         self._server_url = server_url
         self._language = language
         self._sdk_version = sdk_version
         self._gen_version = gen_version
         
-    def list_commerce_transactions(self, request: operations.ListCommerceTransactionsRequest) -> operations.ListCommerceTransactionsResponse:
+    def list_transactions(self, request: operations.ListTransactionsRequest) -> operations.ListTransactionsResponse:
         r"""List transactions
         Details of all financial transactions recorded in the commerce or point of sale system are added to the Transactions data type. For example, payments, service charges, and fees.
         """
         base_url = self._server_url
         
-        url = utils.generate_url(operations.ListCommerceTransactionsRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/commerce-transactions', request)
+        url = utils.generate_url(operations.ListTransactionsRequest, base_url, '/companies/{companyId}/connections/{connectionId}/data/commerce-transactions', request)
         
-        query_params = utils.get_query_params(operations.ListCommerceTransactionsRequest, request)
+        query_params = utils.get_query_params(operations.ListTransactionsRequest, request)
         
         client = self._security_client
         
         http_res = client.request('GET', url, params=query_params)
         content_type = http_res.headers.get('Content-Type')
 
-        res = operations.ListCommerceTransactionsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
+        res = operations.ListTransactionsResponse(status_code=http_res.status_code, content_type=content_type, raw_response=http_res)
         
         if http_res.status_code == 200:
             if utils.match_content_type(content_type, 'application/json'):
-                out = utils.unmarshal_json(http_res.text, Optional[operations.ListCommerceTransactionsLinks])
-                res.links = out
+                out = utils.unmarshal_json(http_res.text, Optional[shared.Transactions])
+                res.transactions = out
 
         return res
```

### Comparing `codat-commerce-0.7.0/src/codat/utils/retries.py` & `codat-commerce-0.9.6/src/codat/utils/retries.py`

 * *Files identical despite different names*

### Comparing `codat-commerce-0.7.0/src/codat/utils/utils.py` & `codat-commerce-0.9.6/src/codat/utils/utils.py`

 * *Files identical despite different names*

### Comparing `codat-commerce-0.7.0/src/codat_commerce.egg-info/PKG-INFO` & `codat-commerce-0.9.6/src/codat_commerce.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codat-commerce
-Version: 0.7.0
+Version: 0.9.6
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: UNKNOWN
 Author: Speakeasy
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -28,65 +28,65 @@
 s = codat.Codat(
     security=shared.Security(
         auth_header="YOUR_API_KEY_HERE",
     ),
 )
 
 
-req = operations.GetCommerceInfoRequest(
+req = operations.GetCompanyInfoRequest(
     company_id="8a210b68-6988-11ed-a1eb-0242ac120002",
     connection_id="2e9d2c44-f675-40ba-8049-353bfcb5e171",
 )
     
-res = s.company_info.get_commerce_info(req)
+res = s.company_info.get_company_info(req)
 
-if res.source_modified_date is not None:
+if res.company_info is not None:
     # handle response
 ```
 <!-- End SDK Example Usage -->
 
 <!-- Start SDK Available Operations -->
-## SDK Available Operations
+## Available Resources and Operations
 
 
 ### company_info
 
-* `get_commerce_info` - Get company info
+* `get_company_info` - Get company info
 
 ### customers
 
-* `list_commerce_customers` - List customers
+* `list_customers` - List customers
 
 ### disputes
 
-* `list_commerce_disputes` - List disputes
+* `list_disputes` - List disputes
 
 ### locations
 
-* `list_commerce_locations` - List locations
+* `list_locations` - List locations
 
 ### orders
 
-* `list_commerce_orders` - List orders
+* `list_orders` - List orders
 
 ### payments
 
-* `list_commerce_payment_methods` - List payment methods
-* `list_commerce_payments` - List payments
+* `list_payment_methods` - List payment methods
+* `list_payments` - List payments
 
 ### products
 
-* `list_commerce_product_categories` - List product categories
-* `list_commerce_products` - List products
+* `list_product_categories` - List product categories
+* `list_products` - List products
 
 ### tax_components
 
-* `get_companies_company_id_connections_connection_id_data_commerce_tax_components` - List tax components
+* `get_tax_components` - List tax components
 
 ### transactions
 
-* `list_commerce_transactions` - List transactions
+* `list_transactions` - List transactions
 <!-- End SDK Available Operations -->
 
 ### SDK Generated by [Speakeasy](https://docs.speakeasyapi.dev/docs/using-speakeasy/client-sdks)
```

