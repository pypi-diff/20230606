# Comparing `tmp/odoo_addons_oca_account_payment-16.0.20230418.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_account_payment-16.0.20230511.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1438 bytes, number of entries: 4
--rw-r--r--  2.0 unx      539 b- defN 23-Apr-19 03:02 odoo_addons_oca_account_payment-16.0.20230418.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-19 03:02 odoo_addons_oca_account_payment-16.0.20230418.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-19 03:02 odoo_addons_oca_account_payment-16.0.20230418.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      432 b- defN 23-Apr-19 03:02 odoo_addons_oca_account_payment-16.0.20230418.0.dist-info/RECORD
-4 files, 1064 bytes uncompressed, 584 bytes compressed:  45.1%
+Zip file size: 1446 bytes, number of entries: 4
+-rw-r--r--  2.0 unx      616 b- defN 23-May-12 03:14 odoo_addons_oca_account_payment-16.0.20230511.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-12 03:14 odoo_addons_oca_account_payment-16.0.20230511.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-May-12 03:14 odoo_addons_oca_account_payment-16.0.20230511.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      432 b- defN 23-May-12 03:14 odoo_addons_oca_account_payment-16.0.20230511.0.dist-info/RECORD
+4 files, 1141 bytes uncompressed, 592 bytes compressed:  48.1%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_account_payment-16.0.20230418.0.dist-info/METADATA
+Filename: odoo_addons_oca_account_payment-16.0.20230511.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_account_payment-16.0.20230418.0.dist-info/WHEEL
+Filename: odoo_addons_oca_account_payment-16.0.20230511.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_account_payment-16.0.20230418.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_account_payment-16.0.20230511.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_account_payment-16.0.20230418.0.dist-info/RECORD
+Filename: odoo_addons_oca_account_payment-16.0.20230511.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_account_payment-16.0.20230418.0.dist-info/METADATA` & `odoo_addons_oca_account_payment-16.0.20230511.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-account-payment
-Version: 16.0.20230418.0
+Version: 16.0.20230511.0
 Summary: Meta package for oca-account-payment Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
 Requires-Dist: odoo-addon-account-due-list (<16.1dev,>=16.0dev)
+Requires-Dist: odoo-addon-account-due-list-payment-mode (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-account-payment-promissory-note (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-account-payment-term-extension (<16.1dev,>=16.0dev)
 
 UNKNOWN
```

