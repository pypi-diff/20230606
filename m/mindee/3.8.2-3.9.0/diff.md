# Comparing `tmp/mindee-3.8.2.tar.gz` & `tmp/mindee-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mindee-3.8.2.tar", last modified: Tue May 23 13:54:57 2023, max compression
+gzip compressed data, was "mindee-3.9.0.tar", last modified: Tue Jun  6 14:06:05 2023, max compression
```

## Comparing `mindee-3.8.2.tar` & `mindee-3.9.0.tar`

### file list

```diff
@@ -1,148 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.980667 mindee-3.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-23 13:54:29.000000 mindee-3.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-23 13:54:57.980667 mindee-3.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-23 13:54:29.000000 mindee-3.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.956667 mindee-3.8.2/mindee/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11467 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    21238 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.960667 mindee-3.8.2/mindee/documents/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.960667 mindee-3.8.2/mindee/documents/cropper/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/cropper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/cropper/cropper_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.960667 mindee-3.8.2/mindee/documents/custom/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/custom/custom_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/custom/custom_v1_fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.960667 mindee-3.8.2/mindee/documents/eu/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/eu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.960667 mindee-3.8.2/mindee/documents/eu/license_plate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/eu/license_plate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/eu/license_plate/license_plate_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.960667 mindee-3.8.2/mindee/documents/financial/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/financial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8099 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/financial/financial_document_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/financial/financial_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.960667 mindee-3.8.2/mindee/documents/fr/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/fr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.960667 mindee-3.8.2/mindee/documents/fr/bank_account_details/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/fr/bank_account_details/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/fr/bank_account_details/bank_account_details_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.960667 mindee-3.8.2/mindee/documents/fr/carte_grise/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/fr/carte_grise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/fr/carte_grise/carte_grise_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.964667 mindee-3.8.2/mindee/documents/fr/carte_vitale/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/fr/carte_vitale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/fr/carte_vitale/carte_vitale_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.964667 mindee-3.8.2/mindee/documents/fr/id_card/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/fr/id_card/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/fr/id_card/id_card_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.964667 mindee-3.8.2/mindee/documents/invoice/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/invoice/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7160 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/invoice/invoice_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/invoice/invoice_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/invoice/line_item_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/invoice/reconstruct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.964667 mindee-3.8.2/mindee/documents/invoice_splitter/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/invoice_splitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/invoice_splitter/invoice_splitter_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.964667 mindee-3.8.2/mindee/documents/passport/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/passport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/passport/passport_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.964667 mindee-3.8.2/mindee/documents/proof_of_address/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/proof_of_address/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/proof_of_address/proof_of_address_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.968667 mindee-3.8.2/mindee/documents/receipt/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/receipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/receipt/line_item_v5.py
--rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/receipt/receipt_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/receipt/receipt_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/receipt/receipt_v5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.968667 mindee-3.8.2/mindee/documents/shipping_container/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/shipping_container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/shipping_container/shipping_container_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.968667 mindee-3.8.2/mindee/documents/us/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/us/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.968667 mindee-3.8.2/mindee/documents/us/bank_check/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/us/bank_check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/documents/us/bank_check/bank_check_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    11161 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.972667 mindee-3.8.2/mindee/fields/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/fields/amount.py
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/fields/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/fields/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/fields/company_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/fields/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/fields/locale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/fields/orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/fields/payment_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/fields/position.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/fields/tax.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/fields/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.972667 mindee-3.8.2/mindee/input/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/input/page_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/input/sources.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/response.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/version
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-23 13:54:29.000000 mindee-3.8.2/mindee/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.960667 mindee-3.8.2/mindee.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-23 13:54:57.000000 mindee-3.8.2/mindee.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-05-23 13:54:57.000000 mindee-3.8.2/mindee.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:54:57.000000 mindee-3.8.2/mindee.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-23 13:54:57.000000 mindee-3.8.2/mindee.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:54:35.000000 mindee-3.8.2/mindee.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-23 13:54:57.000000 mindee-3.8.2/mindee.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-23 13:54:57.000000 mindee-3.8.2/mindee.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-23 13:54:29.000000 mindee-3.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-23 13:54:57.980667 mindee-3.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-23 13:54:29.000000 mindee-3.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.972667 mindee-3.8.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.976667 mindee-3.8.2/tests/documents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/documents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.976667 mindee-3.8.2/tests/documents/fr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/documents/fr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/documents/fr/test_bank_account_details_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/documents/fr/test_carte_grise_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/documents/fr/test_carte_vitale_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/documents/fr/test_id_card_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/documents/test_cropper_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/documents/test_custom_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/documents/test_financial_document_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/documents/test_financial_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/documents/test_invoice_splitter_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/documents/test_invoice_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    13481 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/documents/test_invoice_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/documents/test_passport_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/documents/test_proof_of_address_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/documents/test_receipt_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/documents/test_receipt_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/documents/test_receipt_v5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/documents/test_shipping_container_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.976667 mindee-3.8.2/tests/documents/us/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/documents/us/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/documents/us/test_bank_check_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:57.980667 mindee-3.8.2/tests/fields/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/fields/test_amount.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/fields/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/fields/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/fields/test_locale.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/fields/test_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/fields/test_payment_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/fields/test_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/fields/test_tax.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/test_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-23 13:54:29.000000 mindee-3.8.2/tests/test_pkg_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.666709 mindee-3.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-06 14:05:44.000000 mindee-3.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-06-06 14:06:05.666709 mindee-3.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-06-06 14:05:44.000000 mindee-3.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.650709 mindee-3.9.0/mindee/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11467 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21238 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.654708 mindee-3.9.0/mindee/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.654708 mindee-3.9.0/mindee/documents/cropper/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/cropper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/cropper/cropper_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.654708 mindee-3.9.0/mindee/documents/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/custom/custom_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/custom/custom_v1_fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.654708 mindee-3.9.0/mindee/documents/eu/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/eu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.654708 mindee-3.9.0/mindee/documents/eu/license_plate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/eu/license_plate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/eu/license_plate/license_plate_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.654708 mindee-3.9.0/mindee/documents/financial_document/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/financial_document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9995 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/financial_document/financial_document_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/financial_document/financial_document_v1_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/financial_document/financial_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.654708 mindee-3.9.0/mindee/documents/fr/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/fr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.654708 mindee-3.9.0/mindee/documents/fr/bank_account_details/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/fr/bank_account_details/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/fr/bank_account_details/bank_account_details_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.654708 mindee-3.9.0/mindee/documents/fr/carte_grise/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/fr/carte_grise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8496 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/fr/carte_grise/carte_grise_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.654708 mindee-3.9.0/mindee/documents/fr/carte_vitale/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/fr/carte_vitale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/fr/carte_vitale/carte_vitale_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.654708 mindee-3.9.0/mindee/documents/fr/id_card/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/fr/id_card/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/fr/id_card/id_card_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.658709 mindee-3.9.0/mindee/documents/invoice/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/invoice/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/invoice/invoice_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/invoice/invoice_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/invoice/invoice_v4_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/invoice/reconstruct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.658709 mindee-3.9.0/mindee/documents/invoice_splitter/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/invoice_splitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/invoice_splitter/invoice_splitter_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.658709 mindee-3.9.0/mindee/documents/passport/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/passport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9595 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/passport/passport_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.658709 mindee-3.9.0/mindee/documents/proof_of_address/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/proof_of_address/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/proof_of_address/proof_of_address_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.658709 mindee-3.9.0/mindee/documents/receipt/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/receipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6414 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/receipt/receipt_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/receipt/receipt_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7306 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/receipt/receipt_v5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/receipt/receipt_v5_line_item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.658709 mindee-3.9.0/mindee/documents/shipping_container/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/shipping_container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/shipping_container/shipping_container_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.658709 mindee-3.9.0/mindee/documents/us/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/us/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.658709 mindee-3.9.0/mindee/documents/us/bank_check/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/us/bank_check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/documents/us/bank_check/bank_check_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11161 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.658709 mindee-3.9.0/mindee/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/fields/amount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/fields/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/fields/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/fields/company_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/fields/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/fields/locale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/fields/ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/fields/orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/fields/payment_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/fields/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/fields/tax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/fields/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.662709 mindee-3.9.0/mindee/input/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/input/page_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/input/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7498 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/version
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-06 14:05:44.000000 mindee-3.9.0/mindee/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.654708 mindee-3.9.0/mindee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-06-06 14:06:05.000000 mindee-3.9.0/mindee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-06-06 14:06:05.000000 mindee-3.9.0/mindee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 14:06:05.000000 mindee-3.9.0/mindee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-06 14:06:05.000000 mindee-3.9.0/mindee.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 14:05:48.000000 mindee-3.9.0/mindee.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-06 14:06:05.000000 mindee-3.9.0/mindee.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-06 14:06:05.000000 mindee-3.9.0/mindee.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-06 14:05:44.000000 mindee-3.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-06 14:06:05.666709 mindee-3.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-06 14:05:44.000000 mindee-3.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.662709 mindee-3.9.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.662709 mindee-3.9.0/tests/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/documents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.662709 mindee-3.9.0/tests/documents/fr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/documents/fr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/documents/fr/test_bank_account_details_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/documents/fr/test_carte_grise_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/documents/fr/test_carte_vitale_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/documents/fr/test_id_card_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/documents/test_cropper_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/documents/test_custom_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/documents/test_financial_document_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/documents/test_financial_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/documents/test_invoice_splitter_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/documents/test_invoice_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13481 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/documents/test_invoice_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/documents/test_passport_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/documents/test_proof_of_address_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/documents/test_receipt_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/documents/test_receipt_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/documents/test_receipt_v5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/documents/test_shipping_container_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.662709 mindee-3.9.0/tests/documents/us/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/documents/us/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/documents/us/test_bank_check_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:06:05.666709 mindee-3.9.0/tests/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/fields/test_amount.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/fields/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/fields/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/fields/test_locale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/fields/test_ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/fields/test_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/fields/test_payment_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/fields/test_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/fields/test_tax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/test_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-06 14:05:44.000000 mindee-3.9.0/tests/test_pkg_versions.py
```

### Comparing `mindee-3.8.2/LICENSE` & `mindee-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/PKG-INFO` & `mindee-3.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindee
-Version: 3.8.2
+Version: 3.9.0
 Summary: Mindee API helper library for Python
 Home-page: https://mindee.com/
 Author: Mindee
 Author-email: devrel@mindee.com
 License: MIT
 Project-URL: Documentation, https://developers.mindee.com/docs/python-sdk
 Project-URL: Source, https://github.com/publicMindee/mindee-api-python
```

### Comparing `mindee-3.8.2/README.md` & `mindee-3.9.0/README.md`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/mindee/cli.py` & `mindee-3.9.0/mindee/cli.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/mindee/client.py` & `mindee-3.9.0/mindee/client.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/mindee/documents/__init__.py` & `mindee-3.9.0/mindee/documents/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from mindee.documents import eu, fr, us
 from mindee.documents.cropper import CropperV1, TypeCropperV1
 from mindee.documents.custom import CustomV1, TypeCustomV1
-from mindee.documents.financial import (
+from mindee.documents.financial_document import (
     FinancialDocumentV1,
     FinancialV1,
     TypeFinancialDocumentV1,
     TypeFinancialV1,
 )
 from mindee.documents.invoice import InvoiceV3, InvoiceV4, TypeInvoiceV3, TypeInvoiceV4
 from mindee.documents.invoice_splitter import InvoiceSplitterV1, TypeInvoiceSplitterV1
```

### Comparing `mindee-3.8.2/mindee/documents/base.py` & `mindee-3.9.0/mindee/documents/base.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/mindee/documents/config.py` & `mindee-3.9.0/mindee/documents/config.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/mindee/documents/cropper/cropper_v1.py` & `mindee-3.9.0/mindee/documents/cropper/cropper_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/mindee/documents/custom/custom_v1.py` & `mindee-3.9.0/mindee/documents/custom/custom_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/mindee/documents/custom/custom_v1_fields.py` & `mindee-3.9.0/mindee/documents/custom/custom_v1_fields.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/mindee/documents/eu/license_plate/license_plate_v1.py` & `mindee-3.9.0/mindee/documents/eu/license_plate/license_plate_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         """
         Build the object from the prediction API JSON.
 
         :param api_prediction: Raw prediction from HTTP response
         :param page_n: Page number
         """
         self.license_plates = [
-            TextField(prediction, page_n=page_n)
+            TextField(prediction, page_id=page_n)
             for prediction in api_prediction["license_plates"]
         ]
 
     def __str__(self) -> str:
         license_plates = f"\n { ' ' * 15 }".join(
             [str(item) for item in self.license_plates]
         )
```

### Comparing `mindee-3.8.2/mindee/documents/financial/financial_document_v1.py` & `mindee-3.9.0/mindee/documents/invoice/invoice_v4.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 from typing import List, Optional, TypeVar
 
 from mindee.documents.base import Document, TypeApiPrediction, clean_out_string
-from mindee.documents.invoice.line_item_v4 import InvoiceLineItemV4
+from mindee.documents.invoice import checks, reconstruct
+from mindee.documents.invoice.invoice_v4_line_item import InvoiceV4LineItem
 from mindee.fields.amount import AmountField
 from mindee.fields.classification import ClassificationField
 from mindee.fields.company_registration import CompanyRegistrationField
 from mindee.fields.date import DateField
 from mindee.fields.locale import LocaleField
 from mindee.fields.payment_details import PaymentDetails
-from mindee.fields.tax import TaxField
+from mindee.fields.tax import Taxes
 from mindee.fields.text import TextField
 
 
-class FinancialDocumentV1(Document):
+class InvoiceV4(Document):
     locale: LocaleField
     """locale information"""
+    document_type: ClassificationField
+    """Whether the document is an INVOICE or a CREDIT NOTE."""
     total_amount: AmountField
     """Total including taxes"""
     total_net: AmountField
     """Total excluding taxes"""
-    date: DateField
+    invoice_date: DateField
     """Date the invoice was issued"""
     invoice_number: TextField
     """Invoice number"""
     reference_numbers: List[TextField]
     """List of Reference numbers including PO number."""
     due_date: DateField
     """Date the invoice is due"""
-    taxes: List[TaxField] = []
+    taxes: Taxes
     """List of all taxes"""
     total_tax: AmountField
     """Sum total of all taxes"""
     supplier_name: TextField
     """Supplier 's name"""
     supplier_address: TextField
     """Supplier's address"""
@@ -41,155 +44,144 @@
     """Customer's name"""
     customer_address: TextField
     """Customer's address"""
     customer_company_registrations: List[CompanyRegistrationField]
     """Customer company registration numbers"""
     supplier_payment_details: List[PaymentDetails]
     """Payment details"""
-    line_items: List[InvoiceLineItemV4]
+    line_items: List[InvoiceV4LineItem]
     """Details of line items"""
-    tip: AmountField
-    """Total amount of tip and gratuity."""
-    time: TextField
-    """Time as seen on the receipt in HH:MM format."""
-    document_type: ClassificationField
-    """A classification field, among predefined classes."""
-    category: ClassificationField
-    """The invoice or receipt category among predefined classes."""
-    subcategory: ClassificationField
-    """The invoice or receipt sub-category among predefined classes."""
 
     def __init__(
         self,
         api_prediction=None,
         input_source=None,
         page_n: Optional[int] = None,
     ):
         """
-        Union of `Invoice` and `Receipt`.
+        Invoice document.
 
         :param api_prediction: Raw prediction from HTTP response
         :param input_source: Input object
-        :param page_n: Page number for multi-page PDF input
+        :param page_n: Page number for multi pages pdf input
         """
-        # need this for building from prediction
-        self.input_file = input_source
-
         super().__init__(
             input_source=input_source,
-            document_type="financial_doc",
+            document_type="invoice",
             api_prediction=api_prediction,
             page_n=page_n,
         )
         self._build_from_api_prediction(api_prediction["prediction"], page_n=page_n)
+        self._checklist()
+        self._reconstruct()
 
     def _build_from_api_prediction(
         self, api_prediction: TypeApiPrediction, page_n: Optional[int] = None
     ) -> None:
         """
-        Build the document from an API response JSON.
+        Build the object from the prediction API JSON.
 
         :param api_prediction: Raw prediction from HTTP response
         :param page_n: Page number for multi pages pdf input
         """
+        self.document_type = ClassificationField(
+            api_prediction["document_type"], page_id=page_n
+        )
         self.supplier_company_registrations = [
-            CompanyRegistrationField(field_dict, page_n=page_n)
+            CompanyRegistrationField(field_dict, page_id=page_n)
             for field_dict in api_prediction["supplier_company_registrations"]
         ]
-        self.date = DateField(api_prediction["date"], page_n=page_n)
-        self.due_date = DateField(api_prediction["due_date"], page_n=page_n)
-        self.invoice_number = TextField(api_prediction["invoice_number"], page_n=page_n)
+        self.invoice_date = DateField(api_prediction["date"], page_id=page_n)
+        self.due_date = DateField(api_prediction["due_date"], page_id=page_n)
+        self.invoice_number = TextField(
+            api_prediction["invoice_number"], page_id=page_n
+        )
         self.reference_numbers = [
-            TextField(reference_number, page_n=page_n)
+            TextField(reference_number, page_id=page_n)
             for reference_number in api_prediction["reference_numbers"]
         ]
-        self.locale = LocaleField(
-            api_prediction["locale"], value_key="language", page_n=page_n
-        )
-        self.supplier_name = TextField(api_prediction["supplier_name"], page_n=page_n)
+        self.locale = LocaleField(api_prediction["locale"], page_id=page_n)
+        self.supplier_name = TextField(api_prediction["supplier_name"], page_id=page_n)
         self.supplier_address = TextField(
-            api_prediction["supplier_address"], page_n=page_n
+            api_prediction["supplier_address"], page_id=page_n
         )
-        self.customer_name = TextField(api_prediction["customer_name"], page_n=page_n)
+        self.customer_name = TextField(api_prediction["customer_name"], page_id=page_n)
         self.customer_company_registrations = [
-            CompanyRegistrationField(field_dict, page_n=page_n)
+            CompanyRegistrationField(field_dict, page_id=page_n)
             for field_dict in api_prediction["customer_company_registrations"]
         ]
         self.customer_address = TextField(
-            api_prediction["customer_address"], page_n=page_n
+            api_prediction["customer_address"], page_id=page_n
         )
 
-        self.taxes = [
-            TaxField(tax_prediction, page_n=page_n, value_key="value")
-            for tax_prediction in api_prediction["taxes"]
-        ]
+        self.taxes = Taxes(api_prediction["taxes"], page_id=page_n)
         self.supplier_payment_details = [
-            PaymentDetails(payment_detail, page_n=page_n)
+            PaymentDetails(payment_detail, page_id=page_n)
             for payment_detail in api_prediction["supplier_payment_details"]
         ]
         self.line_items = [
-            InvoiceLineItemV4(prediction=line_item, page_n=page_n)
+            InvoiceV4LineItem(prediction=line_item, page_id=page_n)
             for line_item in api_prediction["line_items"]
         ]
-        self.total_amount = AmountField(api_prediction["total_amount"], page_n=page_n)
-        self.total_net = AmountField(api_prediction["total_net"], page_n=page_n)
-        self.total_tax = AmountField(api_prediction["total_tax"], page_n=page_n)
-        self.tip = AmountField(api_prediction["tip"], page_n=page_n)
-        self.time = TextField(api_prediction["time"], page_n=page_n)
-        self.document_type = ClassificationField(
-            api_prediction["document_type"], page_n=page_n
-        )
-        self.category = ClassificationField(api_prediction["category"], page_n=page_n)
-        self.subcategory = ClassificationField(
-            api_prediction["subcategory"], page_n=page_n
-        )
+        self.total_amount = AmountField(api_prediction["total_amount"], page_id=page_n)
+        self.total_net = AmountField(api_prediction["total_net"], page_id=page_n)
+        self.total_tax = AmountField({"value": None, "confidence": 0.0}, page_id=page_n)
 
     def __str__(self) -> str:
         supplier_company_registrations = "; ".join(
             [str(n.value) for n in self.supplier_company_registrations]
         )
         customer_company_registrations = "; ".join(
             [str(n.value) for n in self.customer_company_registrations]
         )
         reference_numbers = ", ".join([str(n.value) for n in self.reference_numbers])
         payment_details = "\n                          ".join(
             [str(p) for p in self.supplier_payment_details]
         )
-        taxes = "\n       ".join(f"{t}" for t in self.taxes)
         line_items = "\n"
         if self.line_items:
             line_items = "\n  Code           | QTY    | Price   | Amount   | Tax (Rate)       | Description\n"
             for item in self.line_items:
                 line_items += f"  {item}\n"
+
         return clean_out_string(
-            "----- Financial Document V1 -----\n"
-            f"Filename: {self.filename or ''}\n"
-            f"Document type: {self.document_type}\n"
-            f"Category: {self.category}\n"
-            f"Subcategory: {self.subcategory}\n"
-            f"Locale: {self.locale}\n"
-            f"Invoice number: {self.invoice_number}\n"
-            f"Reference numbers: {reference_numbers}\n"
-            f"Date: {self.date}\n"
-            f"Due date: {self.due_date}\n"
-            f"Time: {self.time}\n"
-            f"Supplier name: {self.supplier_name}\n"
-            f"Supplier address: {self.supplier_address}\n"
-            f"Supplier company registrations: {supplier_company_registrations}\n"
-            f"Supplier payment details: {payment_details}\n"
-            f"Customer name: {self.customer_name}\n"
-            f"Customer address: {self.customer_address}\n"
-            f"Customer company registrations: {customer_company_registrations}\n"
-            f"Tip: {self.tip}\n"
-            f"Taxes: {taxes}\n"
-            f"Total tax: {self.total_tax}\n"
-            f"Total net: {self.total_net}\n"
-            f"Total amount: {self.total_amount}\n"
-            f"Line Items: {line_items}"
-            "----------------------"
-        )
+            "Invoice V4 Prediction\n"
+            "=====================\n"
+            f":Filename: {self.filename or ''}\n"
+            f":Locale: {self.locale}\n"
+            f":Invoice number: {self.invoice_number}\n"
+            f":Reference numbers: {reference_numbers}\n"
+            f":Invoice date: {self.invoice_date}\n"
+            f":Invoice due date: {self.due_date}\n"
+            f":Supplier name: {self.supplier_name}\n"
+            f":Supplier address: {self.supplier_address}\n"
+            f":Supplier company registrations: {supplier_company_registrations}\n"
+            f":Supplier payment details: {payment_details}\n"
+            f":Customer name: {self.customer_name}\n"
+            f":Customer company registrations: {customer_company_registrations}\n"
+            f":Customer address: {self.customer_address}\n"
+            f":Line Items: {line_items}"
+            f":Taxes: {self.taxes}\n"
+            f":Total tax: {self.total_tax}\n"
+            f":Total net: {self.total_net}\n"
+            f":Total amount: {self.total_amount}"
+        )
+
+    def _reconstruct(self) -> None:
+        """Call fields reconstruction methods."""
+        reconstruct.total_tax_from_tax_lines(self)
+        reconstruct.total_excl_from_tcc_and_taxes(self)
+        reconstruct.total_incl_from_taxes_plus_excl(self)
+        reconstruct.total_tax_from_incl_and_excl(self)
 
     def _checklist(self) -> None:
-        pass
+        """Call check methods."""
+        self.checklist = {
+            "taxes_match_total_incl": checks.taxes_match_total_incl(self),
+            "taxes_match_total_excl": checks.taxes_match_total_excl(self),
+            "taxes_plus_total_excl_match_total_incl": checks.taxes_plus_total_excl_match_total_incl(
+                self
+            ),
+        }
 
 
-TypeFinancialDocumentV1 = TypeVar("TypeFinancialDocumentV1", bound=FinancialDocumentV1)
+TypeInvoiceV4 = TypeVar("TypeInvoiceV4", bound=InvoiceV4)
```

### Comparing `mindee-3.8.2/mindee/documents/financial/financial_v1.py` & `mindee-3.9.0/mindee/documents/financial_document/financial_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/mindee/documents/fr/bank_account_details/bank_account_details_v1.py` & `mindee-3.9.0/mindee/documents/fr/bank_account_details/bank_account_details_v1.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,23 +42,23 @@
         Build the object from the prediction API JSON.
 
         :param api_prediction: Raw prediction from HTTP response
         :param page_n: Page number
         """
         self.iban = TextField(
             api_prediction["iban"],
-            page_n=page_n,
+            page_id=page_n,
         )
         self.account_holder_name = TextField(
             api_prediction["account_holder_name"],
-            page_n=page_n,
+            page_id=page_n,
         )
         self.swift = TextField(
             api_prediction["swift"],
-            page_n=page_n,
+            page_id=page_n,
         )
 
     def __str__(self) -> str:
         return clean_out_string(
             "----- FR Bank Account Details V1 -----\n"
             f"Filename: {self.filename or ''}\n"
             f"IBAN: { self.iban }\n"
```

### Comparing `mindee-3.8.2/mindee/documents/fr/carte_grise/carte_grise_v1.py` & `mindee-3.9.0/mindee/documents/fr/carte_grise/carte_grise_v1.py`

 * *Files 5% similar despite different names*

```diff
@@ -116,57 +116,59 @@
         """
         Build the document from an API response JSON.
 
         :param api_prediction: Raw prediction from HTTP response
         :param page_n: Page number for multi pages pdf input
         """
         # pylint: disable=invalid-name
-        self.formula_number = TextField(api_prediction["formula_number"], page_n=page_n)
-        self.mrz1 = TextField(api_prediction["mrz1"], page_n=page_n)
-        self.mrz2 = TextField(api_prediction["mrz2"], page_n=page_n)
+        self.formula_number = TextField(
+            api_prediction["formula_number"], page_id=page_n
+        )
+        self.mrz1 = TextField(api_prediction["mrz1"], page_id=page_n)
+        self.mrz2 = TextField(api_prediction["mrz2"], page_id=page_n)
         self.owner_first_name = TextField(
-            api_prediction["owner_first_name"], page_n=page_n
+            api_prediction["owner_first_name"], page_id=page_n
         )
-        self.owner_surname = TextField(api_prediction["owner_surname"], page_n=page_n)
-        self.a = TextField(api_prediction["a"], page_n=page_n)
-        self.b = DateField(api_prediction["b"], page_n=page_n)
-        self.c1 = TextField(api_prediction["c1"], page_n=page_n)
-        self.c3 = TextField(api_prediction["c3"], page_n=page_n)
-        self.c41 = TextField(api_prediction["c41"], page_n=page_n)
-        self.c4a = TextField(api_prediction["c4a"], page_n=page_n)
-        self.d1 = TextField(api_prediction["d1"], page_n=page_n)
-        self.d3 = TextField(api_prediction["d3"], page_n=page_n)
-        self.e = TextField(api_prediction["e"], page_n=page_n)
-        self.f1 = TextField(api_prediction["f1"], page_n=page_n)
-        self.f2 = TextField(api_prediction["f2"], page_n=page_n)
-        self.f3 = TextField(api_prediction["f3"], page_n=page_n)
-        self.g = TextField(api_prediction["g"], page_n=page_n)
-        self.g1 = TextField(api_prediction["g1"], page_n=page_n)
-        self.i = DateField(api_prediction["i"], page_n=page_n)
-        self.j = TextField(api_prediction["j"], page_n=page_n)
-        self.j1 = TextField(api_prediction["j1"], page_n=page_n)
-        self.j2 = TextField(api_prediction["j2"], page_n=page_n)
-        self.j3 = TextField(api_prediction["j3"], page_n=page_n)
-        self.p1 = TextField(api_prediction["p1"], page_n=page_n)
-        self.p2 = TextField(api_prediction["p2"], page_n=page_n)
-        self.p3 = TextField(api_prediction["p3"], page_n=page_n)
-        self.p6 = TextField(api_prediction["p6"], page_n=page_n)
-        self.q = TextField(api_prediction["q"], page_n=page_n)
-        self.s1 = TextField(api_prediction["s1"], page_n=page_n)
-        self.s2 = TextField(api_prediction["s2"], page_n=page_n)
-        self.u1 = TextField(api_prediction["u1"], page_n=page_n)
-        self.u2 = TextField(api_prediction["u2"], page_n=page_n)
-        self.v7 = TextField(api_prediction["v7"], page_n=page_n)
-        self.x1 = DateField(api_prediction["x1"], page_n=page_n)
-        self.y1 = TextField(api_prediction["y1"], page_n=page_n)
-        self.y2 = TextField(api_prediction["y2"], page_n=page_n)
-        self.y3 = TextField(api_prediction["y3"], page_n=page_n)
-        self.y4 = TextField(api_prediction["y4"], page_n=page_n)
-        self.y5 = TextField(api_prediction["y5"], page_n=page_n)
-        self.y6 = TextField(api_prediction["y6"], page_n=page_n)
+        self.owner_surname = TextField(api_prediction["owner_surname"], page_id=page_n)
+        self.a = TextField(api_prediction["a"], page_id=page_n)
+        self.b = DateField(api_prediction["b"], page_id=page_n)
+        self.c1 = TextField(api_prediction["c1"], page_id=page_n)
+        self.c3 = TextField(api_prediction["c3"], page_id=page_n)
+        self.c41 = TextField(api_prediction["c41"], page_id=page_n)
+        self.c4a = TextField(api_prediction["c4a"], page_id=page_n)
+        self.d1 = TextField(api_prediction["d1"], page_id=page_n)
+        self.d3 = TextField(api_prediction["d3"], page_id=page_n)
+        self.e = TextField(api_prediction["e"], page_id=page_n)
+        self.f1 = TextField(api_prediction["f1"], page_id=page_n)
+        self.f2 = TextField(api_prediction["f2"], page_id=page_n)
+        self.f3 = TextField(api_prediction["f3"], page_id=page_n)
+        self.g = TextField(api_prediction["g"], page_id=page_n)
+        self.g1 = TextField(api_prediction["g1"], page_id=page_n)
+        self.i = DateField(api_prediction["i"], page_id=page_n)
+        self.j = TextField(api_prediction["j"], page_id=page_n)
+        self.j1 = TextField(api_prediction["j1"], page_id=page_n)
+        self.j2 = TextField(api_prediction["j2"], page_id=page_n)
+        self.j3 = TextField(api_prediction["j3"], page_id=page_n)
+        self.p1 = TextField(api_prediction["p1"], page_id=page_n)
+        self.p2 = TextField(api_prediction["p2"], page_id=page_n)
+        self.p3 = TextField(api_prediction["p3"], page_id=page_n)
+        self.p6 = TextField(api_prediction["p6"], page_id=page_n)
+        self.q = TextField(api_prediction["q"], page_id=page_n)
+        self.s1 = TextField(api_prediction["s1"], page_id=page_n)
+        self.s2 = TextField(api_prediction["s2"], page_id=page_n)
+        self.u1 = TextField(api_prediction["u1"], page_id=page_n)
+        self.u2 = TextField(api_prediction["u2"], page_id=page_n)
+        self.v7 = TextField(api_prediction["v7"], page_id=page_n)
+        self.x1 = DateField(api_prediction["x1"], page_id=page_n)
+        self.y1 = TextField(api_prediction["y1"], page_id=page_n)
+        self.y2 = TextField(api_prediction["y2"], page_id=page_n)
+        self.y3 = TextField(api_prediction["y3"], page_id=page_n)
+        self.y4 = TextField(api_prediction["y4"], page_id=page_n)
+        self.y5 = TextField(api_prediction["y5"], page_id=page_n)
+        self.y6 = TextField(api_prediction["y6"], page_id=page_n)
 
     def __str__(self) -> str:
         return clean_out_string(
             "----- FR Carte Grise V1 -----\n"
             f"Filename: {self.filename or ''}\n"
             f"formula_number: {self.formula_number}\n"
             f"mrz1: {self.mrz1}\n"
```

### Comparing `mindee-3.8.2/mindee/documents/fr/carte_vitale/carte_vitale_v1.py` & `mindee-3.9.0/mindee/documents/fr/carte_vitale/carte_vitale_v1.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,28 +44,28 @@
         """
         Build the object from the prediction API JSON.
 
         :param api_prediction: Raw prediction from HTTP response
         :param page_n: Page number
         """
         self.given_names = [
-            TextField(prediction, page_n=page_n)
+            TextField(prediction, page_id=page_n)
             for prediction in api_prediction["given_names"]
         ]
         self.surname = TextField(
             api_prediction["surname"],
-            page_n=page_n,
+            page_id=page_n,
         )
         self.social_security = TextField(
             api_prediction["social_security"],
-            page_n=page_n,
+            page_id=page_n,
         )
         self.issuance_date = DateField(
             api_prediction["issuance_date"],
-            page_n=page_n,
+            page_id=page_n,
         )
 
     def __str__(self) -> str:
         given_names = "\n".join([str(item) for item in self.given_names])
         return clean_out_string(
             "----- FR Carte Vitale V1 -----\n"
             f"Filename: {self.filename or ''}\n"
```

### Comparing `mindee-3.8.2/mindee/documents/fr/id_card/id_card_v1.py` & `mindee-3.9.0/mindee/documents/fr/id_card/id_card_v1.py`

 * *Files 12% similar despite different names*

```diff
@@ -59,55 +59,55 @@
         Build the object from the prediction API JSON.
 
         :param api_prediction: Raw prediction from HTTP response
         :param page_n: Page number
         """
         self.document_side = TextField(
             api_prediction.get("document_side", {}),
-            page_n=page_n,
+            page_id=page_n,
         )
         self.id_number = TextField(
             api_prediction["id_number"],
-            page_n=page_n,
+            page_id=page_n,
         )
         self.given_names = [
-            TextField(prediction, page_n=page_n)
+            TextField(prediction, page_id=page_n)
             for prediction in api_prediction["given_names"]
         ]
         self.surname = TextField(
             api_prediction["surname"],
-            page_n=page_n,
+            page_id=page_n,
         )
         self.birth_date = DateField(
             api_prediction["birth_date"],
-            page_n=page_n,
+            page_id=page_n,
         )
         self.birth_place = TextField(
             api_prediction["birth_place"],
-            page_n=page_n,
+            page_id=page_n,
         )
         self.expiry_date = DateField(
             api_prediction["expiry_date"],
-            page_n=page_n,
+            page_id=page_n,
         )
         self.authority = TextField(
             api_prediction["authority"],
-            page_n=page_n,
+            page_id=page_n,
         )
         self.gender = TextField(
             api_prediction["gender"],
-            page_n=page_n,
+            page_id=page_n,
         )
         self.mrz1 = TextField(
             api_prediction["mrz1"],
-            page_n=page_n,
+            page_id=page_n,
         )
         self.mrz2 = TextField(
             api_prediction["mrz2"],
-            page_n=page_n,
+            page_id=page_n,
         )
 
     def __str__(self) -> str:
         given_names = "\n".join([str(item) for item in self.given_names])
         return clean_out_string(
             "----- FR Carte Nationale d'Identité V1 -----\n"
             f"Filename: {self.filename or ''}\n"
```

### Comparing `mindee-3.8.2/mindee/documents/invoice/checks.py` & `mindee-3.9.0/mindee/documents/invoice/checks.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/mindee/documents/invoice/invoice_v3.py` & `mindee-3.9.0/mindee/documents/invoice/invoice_v3.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from mindee.documents.invoice import checks, reconstruct
 from mindee.fields.amount import AmountField
 from mindee.fields.classification import ClassificationField
 from mindee.fields.company_registration import CompanyRegistrationField
 from mindee.fields.date import DateField
 from mindee.fields.locale import LocaleField
 from mindee.fields.payment_details import PaymentDetails
-from mindee.fields.tax import TaxField
+from mindee.fields.tax import Taxes
 from mindee.fields.text import TextField
 
 
 class InvoiceV3(Document):
     locale: LocaleField
     """locale information"""
     document_type: ClassificationField
@@ -23,15 +23,15 @@
     """Total excluding taxes. Same as ``total_excl``."""
     invoice_date: DateField
     """Date the invoice was issued"""
     invoice_number: TextField
     """Invoice number"""
     due_date: DateField
     """Date the invoice is due"""
-    taxes: List[TaxField] = []
+    taxes: Taxes
     """List of all taxes"""
     total_tax: AmountField
     """Sum total of all taxes"""
     supplier: TextField
     """Supplier 's name"""
     supplier_address: TextField
     """Supplier's address"""
@@ -75,50 +75,46 @@
         """
         Build the object from the prediction API JSON.
 
         :param api_prediction: Raw prediction from HTTP response
         :param page_n: Page number for multi pages pdf input
         """
         self.document_type = ClassificationField(
-            api_prediction["document_type"], page_n=page_n
+            api_prediction["document_type"], page_id=page_n
         )
         self.company_number = [
-            CompanyRegistrationField(field_dict, page_n=page_n)
+            CompanyRegistrationField(field_dict, page_id=page_n)
             for field_dict in api_prediction["company_registration"]
         ]
-        self.invoice_date = DateField(api_prediction["date"], page_n=page_n)
-        self.due_date = DateField(api_prediction["due_date"], page_n=page_n)
-        self.invoice_number = TextField(api_prediction["invoice_number"], page_n=page_n)
-        self.locale = LocaleField(
-            api_prediction["locale"], value_key="language", page_n=page_n
+        self.invoice_date = DateField(api_prediction["date"], page_id=page_n)
+        self.due_date = DateField(api_prediction["due_date"], page_id=page_n)
+        self.invoice_number = TextField(
+            api_prediction["invoice_number"], page_id=page_n
         )
-        self.supplier = TextField(api_prediction["supplier"], page_n=page_n)
+        self.locale = LocaleField(api_prediction["locale"], page_id=page_n)
+        self.supplier = TextField(api_prediction["supplier"], page_id=page_n)
         self.supplier_address = TextField(
-            api_prediction["supplier_address"], page_n=page_n
+            api_prediction["supplier_address"], page_id=page_n
         )
-        self.customer_name = TextField(api_prediction["customer"], page_n=page_n)
+        self.customer_name = TextField(api_prediction["customer"], page_id=page_n)
         self.customer_company_registration = [
-            CompanyRegistrationField(field_dict, page_n=page_n)
+            CompanyRegistrationField(field_dict, page_id=page_n)
             for field_dict in api_prediction["customer_company_registration"]
         ]
         self.customer_address = TextField(
-            api_prediction["customer_address"], page_n=page_n
+            api_prediction["customer_address"], page_id=page_n
         )
-
-        self.taxes = [
-            TaxField(tax_prediction, page_n=page_n, value_key="value")
-            for tax_prediction in api_prediction["taxes"]
-        ]
+        self.taxes = Taxes(api_prediction["taxes"], page_id=page_n)
         self.payment_details = [
-            PaymentDetails(payment_detail, page_n=page_n)
+            PaymentDetails(payment_detail, page_id=page_n)
             for payment_detail in api_prediction["payment_details"]
         ]
-        self.total_amount = AmountField(api_prediction["total_incl"], page_n=page_n)
-        self.total_net = AmountField(api_prediction["total_excl"], page_n=page_n)
-        self.total_tax = AmountField({"value": None, "confidence": 0.0}, page_n=page_n)
+        self.total_amount = AmountField(api_prediction["total_incl"], page_id=page_n)
+        self.total_net = AmountField(api_prediction["total_excl"], page_id=page_n)
+        self.total_tax = AmountField({"value": None, "confidence": 0.0}, page_id=page_n)
 
     @property
     def total_incl(self) -> AmountField:
         """Total including taxes."""
         return self.total_amount
 
     @total_incl.setter
@@ -138,35 +134,34 @@
         company_numbers = "; ".join([str(n.value) for n in self.company_number])
         customer_company_registration = "; ".join(
             [str(n.value) for n in self.customer_company_registration]
         )
         payment_details = "\n                 ".join(
             [str(p) for p in self.payment_details]
         )
-        taxes = "\n       ".join(f"{t}" for t in self.taxes)
 
         return clean_out_string(
-            "----- Invoice V3 -----\n"
-            f"Filename: {self.filename or ''}\n"
-            f"Invoice number: {self.invoice_number}\n"
-            f"Total amount including taxes: {self.total_amount}\n"
-            f"Total amount excluding taxes: {self.total_net}\n"
-            f"Invoice date: {self.invoice_date}\n"
-            f"Invoice due date: {self.due_date}\n"
-            f"Supplier name: {self.supplier}\n"
-            f"Supplier address: {self.supplier_address}\n"
-            f"Customer name: {self.customer_name}\n"
-            f"Customer company registration: {customer_company_registration}\n"
-            f"Customer address: {self.customer_address}\n"
-            f"Payment details: {payment_details}\n"
-            f"Company numbers: {company_numbers}\n"
-            f"Taxes: {taxes}\n"
-            f"Total taxes: {self.total_tax}\n"
-            f"Locale: {self.locale}\n"
-            "----------------------"
+            "Invoice V3 Prediction\n"
+            "=====================\n"
+            f":Filename: {self.filename or ''}\n"
+            f":Invoice number: {self.invoice_number}\n"
+            f":Total amount: {self.total_amount}\n"
+            f":Total net: {self.total_net}\n"
+            f":Invoice date: {self.invoice_date}\n"
+            f":Invoice due date: {self.due_date}\n"
+            f":Supplier name: {self.supplier}\n"
+            f":Supplier address: {self.supplier_address}\n"
+            f":Customer name: {self.customer_name}\n"
+            f":Customer company registration: {customer_company_registration}\n"
+            f":Customer address: {self.customer_address}\n"
+            f":Payment details: {payment_details}\n"
+            f":Company numbers: {company_numbers}\n"
+            f":Taxes: {self.taxes}\n"
+            f":Total tax: {self.total_tax}\n"
+            f":Locale: {self.locale}"
         )
 
     def _reconstruct(self) -> None:
         """Call fields reconstruction methods."""
         reconstruct.total_tax_from_tax_lines(self)
         reconstruct.total_excl_from_tcc_and_taxes(self)
         reconstruct.total_incl_from_taxes_plus_excl(self)
```

### Comparing `mindee-3.8.2/mindee/documents/invoice/line_item_v4.py` & `mindee-3.9.0/mindee/documents/invoice/invoice_v4_line_item.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 from typing import Optional
 
-from mindee.fields.base import FieldPositionMixin, TypePrediction, float_to_string
+from mindee.fields.base import (
+    FieldConfidenceMixin,
+    FieldPositionMixin,
+    TypePrediction,
+    float_to_string,
+    to_opt_float,
+)
 
 
-class InvoiceLineItemV4(FieldPositionMixin):
+class InvoiceV4LineItem(FieldPositionMixin, FieldConfidenceMixin):
     product_code: Optional[str]
     """The product code referring to the item."""
     description: Optional[str]
     """The item description."""
     quantity: Optional[float]
     """The item quantity"""
     unit_price: Optional[float]
@@ -22,41 +28,31 @@
     """Confidence score"""
     page_n: int
     """The document page on which the information was found."""
 
     def __init__(
         self,
         prediction: TypePrediction,
-        page_n: Optional[int] = None,
+        page_id: Optional[int] = None,
     ):
+        self._set_confidence(prediction)
         self._set_position(prediction)
 
-        if page_n is None:
+        if page_id is None:
             self.page_n = prediction["page_id"]
         else:
-            self.page_n = page_n
-
-        try:
-            self.confidence = float(prediction["confidence"])
-        except (KeyError, TypeError):
-            pass
-
-        def to_opt_float(key: str) -> Optional[float]:
-            try:
-                return float(prediction[key])
-            except TypeError:
-                return None
+            self.page_n = page_id
 
         self.product_code = prediction["product_code"]
         self.description = prediction["description"]
-        self.quantity = to_opt_float("quantity")
-        self.unit_price = to_opt_float("unit_price")
-        self.total_amount = to_opt_float("total_amount")
-        self.tax_rate = to_opt_float("tax_rate")
-        self.tax_amount = to_opt_float("tax_amount")
+        self.quantity = to_opt_float(prediction, "quantity")
+        self.unit_price = to_opt_float(prediction, "unit_price")
+        self.total_amount = to_opt_float(prediction, "total_amount")
+        self.tax_rate = to_opt_float(prediction, "tax_rate")
+        self.tax_amount = to_opt_float(prediction, "tax_amount")
 
     def __str__(self) -> str:
         tax = float_to_string(self.tax_amount)
         if self.tax_rate is not None:
             tax += f" ({float_to_string(self.tax_rate)}%)"
 
         description = self.description or ""
```

### Comparing `mindee-3.8.2/mindee/documents/invoice/reconstruct.py` & `mindee-3.9.0/mindee/documents/invoice/reconstruct.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/mindee/documents/invoice_splitter/invoice_splitter_v1.py` & `mindee-3.9.0/mindee/documents/invoice_splitter/invoice_splitter_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/mindee/documents/passport/passport_v1.py` & `mindee-3.9.0/mindee/documents/passport/passport_v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,30 +66,30 @@
     ) -> None:
         """
         Build the document from an API response JSON.
 
         :param api_prediction: Raw prediction from HTTP response
         :param page_n: Page number for multi pages pdf input
         """
-        self.country = TextField(api_prediction["country"], page_n=page_n)
-        self.id_number = TextField(api_prediction["id_number"], page_n=page_n)
-        self.birth_date = DateField(api_prediction["birth_date"], page_n=page_n)
-        self.expiry_date = DateField(api_prediction["expiry_date"], page_n=page_n)
-        self.issuance_date = DateField(api_prediction["issuance_date"], page_n=page_n)
-        self.birth_place = TextField(api_prediction["birth_place"], page_n=page_n)
-        self.gender = TextField(api_prediction["gender"], page_n=page_n)
-        self.surname = TextField(api_prediction["surname"], page_n=page_n)
-        self.mrz1 = TextField(api_prediction["mrz1"], page_n=page_n)
-        self.mrz2 = TextField(api_prediction["mrz2"], page_n=page_n)
+        self.country = TextField(api_prediction["country"], page_id=page_n)
+        self.id_number = TextField(api_prediction["id_number"], page_id=page_n)
+        self.birth_date = DateField(api_prediction["birth_date"], page_id=page_n)
+        self.expiry_date = DateField(api_prediction["expiry_date"], page_id=page_n)
+        self.issuance_date = DateField(api_prediction["issuance_date"], page_id=page_n)
+        self.birth_place = TextField(api_prediction["birth_place"], page_id=page_n)
+        self.gender = TextField(api_prediction["gender"], page_id=page_n)
+        self.surname = TextField(api_prediction["surname"], page_id=page_n)
+        self.mrz1 = TextField(api_prediction["mrz1"], page_id=page_n)
+        self.mrz2 = TextField(api_prediction["mrz2"], page_id=page_n)
         self.given_names = [
-            TextField(given_name, page_n=page_n)
+            TextField(given_name, page_id=page_n)
             for given_name in api_prediction["given_names"]
         ]
-        self.mrz = TextField({"value": None, "confidence": 0.0}, page_n=page_n)
-        self.full_name = TextField({"value": None, "confidence": 0.0}, page_n=page_n)
+        self.mrz = TextField({"value": None, "confidence": 0.0}, page_id=page_n)
+        self.full_name = TextField({"value": None, "confidence": 0.0}, page_id=page_n)
 
     def __str__(self) -> str:
         given_names = " ".join(
             [
                 given_name.value if given_name.value is not None else ""
                 for given_name in self.given_names
             ]
```

### Comparing `mindee-3.8.2/mindee/documents/proof_of_address/proof_of_address_v1.py` & `mindee-3.9.0/mindee/documents/proof_of_address/proof_of_address_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,47 +57,47 @@
         Build the object from the prediction API JSON.
 
         :param api_prediction: Raw prediction from HTTP response
         :param page_n: Page number
         """
         self.locale = LocaleField(
             api_prediction["locale"],
-            page_n=page_n,
+            page_id=page_n,
         )
         self.issuer_name = TextField(
             api_prediction["issuer_name"],
-            page_n=page_n,
+            page_id=page_n,
         )
         self.issuer_company_registration = [
-            CompanyRegistrationField(prediction, page_n=page_n)
+            CompanyRegistrationField(prediction, page_id=page_n)
             for prediction in api_prediction["issuer_company_registration"]
         ]
         self.issuer_address = TextField(
             api_prediction["issuer_address"],
-            page_n=page_n,
+            page_id=page_n,
         )
         self.recipient_name = TextField(
             api_prediction["recipient_name"],
-            page_n=page_n,
+            page_id=page_n,
         )
         self.recipient_company_registration = [
-            CompanyRegistrationField(prediction, page_n=page_n)
+            CompanyRegistrationField(prediction, page_id=page_n)
             for prediction in api_prediction["recipient_company_registration"]
         ]
         self.recipient_address = TextField(
             api_prediction["recipient_address"],
-            page_n=page_n,
+            page_id=page_n,
         )
         self.dates = [
-            DateField(prediction, page_n=page_n)
+            DateField(prediction, page_id=page_n)
             for prediction in api_prediction["dates"]
         ]
         self.date = DateField(
             api_prediction["date"],
-            page_n=page_n,
+            page_id=page_n,
         )
 
     def __str__(self) -> str:
         issuer_company_registration = f"\n { ' ' * 28 }".join(
             [str(item) for item in self.issuer_company_registration],
         )
         recipient_company_registration = f"\n { ' ' * 31 }".join(
```

### Comparing `mindee-3.8.2/mindee/documents/receipt/line_item_v5.py` & `mindee-3.9.0/mindee/fields/amount.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,58 +1,42 @@
 from typing import Optional
 
-from mindee.fields.base import FieldPositionMixin, TypePrediction, float_to_string
+from mindee.fields.base import (
+    BaseField,
+    FieldPositionMixin,
+    TypePrediction,
+    float_to_string,
+)
 
 
-class ReceiptV5LineItem(FieldPositionMixin):
-    description: Optional[str]
-    """The item description."""
-    quantity: Optional[float]
-    """The item quantity"""
-    unit_price: Optional[float]
-    """The item unit price."""
-    total_amount: Optional[float]
-    """The item total amount."""
-    confidence: float = 0.0
-    """Confidence score"""
-    page_n: int
-    """The document page on which the information was found."""
+class AmountField(FieldPositionMixin, BaseField):
+    value: Optional[float] = None
 
     def __init__(
         self,
         prediction: TypePrediction,
-        page_n: Optional[int] = None,
+        reconstructed: bool = False,
+        page_id: Optional[int] = None,
     ):
-        self._set_position(prediction)
-
-        if page_n is None:
-            self.page_n = prediction["page_id"]
-        else:
-            self.page_n = page_n
+        """
+        Amount field object.
 
+        :param prediction: Amount prediction object from HTTP response
+        :param reconstructed: Bool for reconstructed object (not extracted in the API)
+        :param page_id: Page number for multi-page document
+        """
+        super().__init__(
+            prediction,
+            value_key="value",
+            reconstructed=reconstructed,
+            page_n=page_id,
+        )
         try:
-            self.confidence = float(prediction["confidence"])
-        except (KeyError, TypeError):
-            pass
-
-        def to_opt_float(key: str) -> Optional[float]:
-            try:
-                return float(prediction[key])
-            except TypeError:
-                return None
-
-        self.description = prediction["description"]
-        self.quantity = to_opt_float("quantity")
-        self.unit_price = to_opt_float("unit_price")
-        self.total_amount = to_opt_float("total_amount")
+            self.value = round(float(prediction["value"]), 3)
+        except (ValueError, TypeError, KeyError):
+            self.value = None
+            self.confidence = 0.0
+
+        self._set_position(prediction)
 
     def __str__(self) -> str:
-        description = self.description or ""
-        if len(description) > 32:
-            description = description[:32] + "..."
-        row = [
-            float_to_string(self.quantity),
-            float_to_string(self.unit_price),
-            float_to_string(self.total_amount),
-            description,
-        ]
-        return "| {:<8} | {:<8} | {:<9} | {:<34} |".format(*row)
+        return float_to_string(self.value)
```

### Comparing `mindee-3.8.2/mindee/documents/receipt/receipt_v3.py` & `mindee-3.9.0/mindee/documents/receipt/receipt_v3.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from typing import List, Optional, TypeVar
+from typing import Optional, TypeVar
 
 from mindee.documents.base import Document, TypeApiPrediction, clean_out_string
 from mindee.fields.amount import AmountField
 from mindee.fields.base import field_array_confidence, field_array_sum
 from mindee.fields.classification import ClassificationField
 from mindee.fields.date import DateField
 from mindee.fields.locale import LocaleField
-from mindee.fields.tax import TaxField
+from mindee.fields.tax import Taxes
 from mindee.fields.text import TextField
 
 
 class ReceiptV3(Document):
     locale: LocaleField
     """locale information"""
     total_incl: AmountField
@@ -19,15 +19,15 @@
     """Date the receipt was issued"""
     time: TextField
     """Time the receipt was issued"""
     category: ClassificationField
     """Service category"""
     merchant_name: TextField
     """Merchant's name"""
-    taxes: List[TaxField]
+    taxes: Taxes
     """List of all taxes"""
     total_tax: AmountField
     """Sum total of all taxes"""
     total_excl: AmountField
     """Total excluding taxes"""
 
     def __init__(
@@ -50,59 +50,51 @@
             page_n=page_n,
         )
         self._build_from_api_prediction(api_prediction["prediction"], page_n=page_n)
         self._checklist()
         self._reconstruct()
 
     def __str__(self) -> str:
-        taxes = "\n       ".join(f"{t}" for t in self.taxes)
         return clean_out_string(
-            "-----Receipt data-----\n"
-            f"Filename: {self.filename or ''}\n"
-            f"Total amount including taxes: {self.total_incl}\n"
-            f"Total amount excluding taxes: {self.total_excl}\n"
-            f"Date: {self.date}\n"
-            f"Category: {self.category}\n"
-            f"Time: {self.time}\n"
-            f"Merchant name: {self.merchant_name}\n"
-            f"Taxes: {taxes}\n"
-            f"Total taxes: {self.total_tax}\n"
-            f"Locale: {self.locale}\n"
-            "----------------------"
+            "Receipt V3 Prediction\n"
+            "=====================\n"
+            f":Filename: {self.filename or ''}\n"
+            f":Total amount: {self.total_incl}\n"
+            f":Total net: {self.total_excl}\n"
+            f":Date: {self.date}\n"
+            f":Category: {self.category}\n"
+            f":Time: {self.time}\n"
+            f":Merchant name: {self.merchant_name}\n"
+            f":Taxes: {self.taxes}\n"
+            f":Total tax: {self.total_tax}\n"
+            f":Locale: {self.locale}"
         )
 
     def _build_from_api_prediction(
         self, api_prediction: TypeApiPrediction, page_n: Optional[int] = None
     ) -> None:
         """
         Build the document from an API response JSON.
 
         :param api_prediction: Raw prediction from HTTP response
         :param page_n: Page number for multi pages pdf input
         """
-        self.locale = LocaleField(api_prediction["locale"], page_n=page_n)
-        self.total_incl = AmountField(api_prediction["total_incl"], page_n=page_n)
-        self.date = DateField(api_prediction["date"], page_n=page_n)
-        self.category = ClassificationField(api_prediction["category"], page_n=page_n)
+        self.locale = LocaleField(api_prediction["locale"], page_id=page_n)
+        self.total_incl = AmountField(api_prediction["total_incl"], page_id=page_n)
+        self.date = DateField(api_prediction["date"], page_id=page_n)
+        self.category = ClassificationField(api_prediction["category"], page_id=page_n)
         self.merchant_name = TextField(
-            api_prediction["supplier"], value_key="value", page_n=page_n
+            api_prediction["supplier"], value_key="value", page_id=page_n
+        )
+        self.time = TextField(api_prediction["time"], value_key="value", page_id=page_n)
+        self.taxes = Taxes(api_prediction["taxes"], page_id=page_n)
+        self.total_tax = AmountField({"value": None, "confidence": 0.0}, page_id=page_n)
+        self.total_excl = AmountField(
+            {"value": None, "confidence": 0.0}, page_id=page_n
         )
-        self.time = TextField(api_prediction["time"], value_key="value", page_n=page_n)
-        self.taxes = [
-            TaxField(
-                tax_prediction,
-                page_n=page_n,
-                value_key="value",
-                rate_key="rate",
-                code_key="code",
-            )
-            for tax_prediction in api_prediction["taxes"]
-        ]
-        self.total_tax = AmountField({"value": None, "confidence": 0.0}, page_n=page_n)
-        self.total_excl = AmountField({"value": None, "confidence": 0.0}, page_n=page_n)
 
     def _checklist(self) -> None:
         """Call check methods."""
         self.checklist = {"taxes_match_total_incl": self.__taxes_match_total()}
 
     def _reconstruct(self) -> None:
         """Call fields reconstruction methods."""
```

### Comparing `mindee-3.8.2/mindee/documents/receipt/receipt_v4.py` & `mindee-3.9.0/mindee/documents/receipt/receipt_v4.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from typing import List, Optional, TypeVar
+from typing import Optional, TypeVar
 
 from mindee.documents.base import Document, TypeApiPrediction, clean_out_string
 from mindee.fields.amount import AmountField
 from mindee.fields.classification import ClassificationField
 from mindee.fields.date import DateField
 from mindee.fields.locale import LocaleField
-from mindee.fields.tax import TaxField
+from mindee.fields.tax import Taxes
 from mindee.fields.text import TextField
 
 
 class ReceiptV4(Document):
     locale: LocaleField
     """locale information"""
     total_amount: AmountField
@@ -22,15 +22,15 @@
     """The type, or service category, of the purchase."""
     subcategory: ClassificationField
     """The receipt sub category among predefined classes."""
     document_type: ClassificationField
     """Whether the document is an expense receipt or a credit card receipt."""
     supplier: TextField
     """The merchant, or supplier, as found on the receipt."""
-    taxes: List[TaxField]
+    taxes: Taxes
     """List of all taxes."""
     total_tax: AmountField
     """Total tax amount of the purchase."""
     total_net: AmountField
     "Total amount of the purchase excluding taxes."
     tip: AmountField
     """Total amount of tip and gratuity."""
@@ -61,60 +61,50 @@
     ) -> None:
         """
         Build the document from an API response JSON.
 
         :param api_prediction: Raw prediction from HTTP response
         :param page_n: Page number for multi pages pdf input
         """
-        self.locale = LocaleField(api_prediction["locale"], page_n=page_n)
-        self.total_amount = AmountField(api_prediction["total_amount"], page_n=page_n)
-        self.total_net = AmountField(api_prediction["total_net"], page_n=page_n)
-        self.total_tax = AmountField(api_prediction["total_tax"], page_n=page_n)
-        self.tip = AmountField(api_prediction["tip"], page_n=page_n)
-        self.date = DateField(api_prediction["date"], page_n=page_n)
-        self.category = ClassificationField(api_prediction["category"], page_n=page_n)
+        self.locale = LocaleField(api_prediction["locale"], page_id=page_n)
+        self.total_amount = AmountField(api_prediction["total_amount"], page_id=page_n)
+        self.total_net = AmountField(api_prediction["total_net"], page_id=page_n)
+        self.total_tax = AmountField(api_prediction["total_tax"], page_id=page_n)
+        self.tip = AmountField(api_prediction["tip"], page_id=page_n)
+        self.date = DateField(api_prediction["date"], page_id=page_n)
+        self.category = ClassificationField(api_prediction["category"], page_id=page_n)
         self.subcategory = ClassificationField(
-            api_prediction["subcategory"], page_n=page_n
+            api_prediction["subcategory"], page_id=page_n
         )
         self.document_type = ClassificationField(
-            api_prediction["document_type"], page_n=page_n
+            api_prediction["document_type"], page_id=page_n
         )
         self.supplier = TextField(
-            api_prediction["supplier"], value_key="value", page_n=page_n
+            api_prediction["supplier"], value_key="value", page_id=page_n
         )
-        self.time = TextField(api_prediction["time"], value_key="value", page_n=page_n)
-        self.taxes = [
-            TaxField(
-                tax_prediction,
-                page_n=page_n,
-                value_key="value",
-                rate_key="rate",
-                code_key="code",
-            )
-            for tax_prediction in api_prediction["taxes"]
-        ]
+        self.time = TextField(api_prediction["time"], value_key="value", page_id=page_n)
+        self.taxes = Taxes(api_prediction["taxes"], page_id=page_n)
 
     def __str__(self) -> str:
-        taxes = "\n       ".join(f"{t}" for t in self.taxes)
         return clean_out_string(
-            "----- Receipt V4 -----\n"
-            f"Filename: {self.filename or ''}\n"
-            f"Total amount: {self.total_amount}\n"
-            f"Total net: {self.total_net}\n"
-            f"Tip: {self.tip}\n"
-            f"Date: {self.date}\n"
-            f"Category: {self.category}\n"
-            f"Subcategory: {self.subcategory}\n"
-            f"Document type: {self.document_type}\n"
-            f"Time: {self.time}\n"
-            f"Supplier name: {self.supplier}\n"
-            f"Taxes: {taxes}\n"
-            f"Total taxes: {self.total_tax}\n"
-            f"Locale: {self.locale}\n"
-            "----------------------"
+            "Receipt V4 Prediction\n"
+            "=====================\n"
+            f":Filename: {self.filename or ''}\n"
+            f":Total amount: {self.total_amount}\n"
+            f":Total net: {self.total_net}\n"
+            f":Tip: {self.tip}\n"
+            f":Date: {self.date}\n"
+            f":Category: {self.category}\n"
+            f":Subcategory: {self.subcategory}\n"
+            f":Document type: {self.document_type}\n"
+            f":Time: {self.time}\n"
+            f":Supplier name: {self.supplier}\n"
+            f":Taxes: {self.taxes}\n"
+            f":Total tax: {self.total_tax}\n"
+            f":Locale: {self.locale}"
         )
 
     def _checklist(self) -> None:
         pass
 
 
 TypeReceiptV4 = TypeVar("TypeReceiptV4", bound=ReceiptV4)
```

### Comparing `mindee-3.8.2/mindee/documents/receipt/receipt_v5.py` & `mindee-3.9.0/mindee/documents/receipt/receipt_v5.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,65 @@
 from typing import List, Optional, TypeVar
 
 from mindee.documents.base import Document, TypeApiPrediction, clean_out_string
-from mindee.documents.receipt.line_item_v5 import ReceiptV5LineItem
 from mindee.fields.amount import AmountField
 from mindee.fields.classification import ClassificationField
 from mindee.fields.company_registration import CompanyRegistrationField
 from mindee.fields.date import DateField
 from mindee.fields.locale import LocaleField
-from mindee.fields.tax import TaxField
+from mindee.fields.tax import Taxes
 from mindee.fields.text import TextField
 
+from .receipt_v5_line_item import ReceiptV5LineItem
+
 
 class ReceiptV5(Document):
-    locale: LocaleField
-    """locale information"""
-    total_amount: AmountField
-    """The total amount paid including taxes, discounts, fees, tips, and gratuity."""
-    date: DateField
-    """The date the purchase was made."""
-    time: TextField
-    """Time of purchase with 24 hours formatting (HH:MM)."""
+    """Receipt v5 prediction results."""
+
     category: ClassificationField
     """The receipt category among predefined classes."""
-    subcategory: ClassificationField
-    """The receipt sub category among predefined classes for transport and food."""
+    date: DateField
+    """The date the purchase was made."""
     document_type: ClassificationField
     """Whether the document is an expense receipt or a credit card receipt."""
-    supplier_name: TextField
-    """The name of the supplier or merchant."""
-    supplier_phone_number: TextField
-    """The Phone number of the supplier or merchant."""
+    line_items: List[ReceiptV5LineItem]
+    """Full extraction of lines, including: description, quantity, unit price and total."""
+    locale: LocaleField
+    """The locale identifier in BCP 47 (RFC 5646) format: ISO language code, '-', ISO country code."""
+    subcategory: ClassificationField
+    """The receipt sub category among predefined classes for transport and food."""
     supplier_address: TextField
-    """The address of the supplier or merchant."""
+    """The address of the supplier or merchant returned as a single string."""
     supplier_company_registrations: List[CompanyRegistrationField]
     """List of supplier company registrations or identifiers."""
-    taxes: List[TaxField]
+    supplier_name: TextField
+    """The name of the supplier or merchant."""
+    supplier_phone_number: TextField
+    """The Phone number of the supplier or merchant returned as a single string."""
+    taxes: Taxes
     """List of tax lines information including: Amount, tax rate, tax base amount and tax code."""
-    total_tax: AmountField
-    """The total amount of taxes."""
-    total_net: AmountField
-    """The total amount excluding taxes."""
+    time: TextField
+    """Time of purchase with 24 hours formatting (HH:MM)."""
     tip: AmountField
     """The total amount of tip and gratuity."""
-    line_items: List[ReceiptV5LineItem]
-    """Full extraction of lines, including: description, quantity, unit price and total."""
+    total_amount: AmountField
+    """The total amount paid including taxes, discounts, fees, tips, and gratuity."""
+    total_net: AmountField
+    """The total amount excluding taxes."""
+    total_tax: AmountField
+    """The total amount of taxes."""
 
     def __init__(
         self,
         api_prediction=None,
         input_source=None,
         page_n: Optional[int] = None,
     ):
         """
-        Receipt document.
+        Receipt v5 prediction results.
 
         :param api_prediction: Raw prediction from HTTP response
         :param input_source: Input object
         :param page_n: Page number for multi pages pdf input
         """
         super().__init__(
             input_source=input_source,
@@ -66,98 +69,129 @@
         )
         self._build_from_api_prediction(api_prediction["prediction"], page_n=page_n)
 
     def _build_from_api_prediction(
         self, api_prediction: TypeApiPrediction, page_n: Optional[int] = None
     ) -> None:
         """
-        Build the document from an API response JSON.
+        Build the object from the prediction API JSON.
 
         :param api_prediction: Raw prediction from HTTP response
-        :param page_n: Page number for multi pages pdf input
+        :param page_n: Page number
         """
-        self.locale = LocaleField(api_prediction["locale"], page_n=page_n)
-        self.total_amount = AmountField(api_prediction["total_amount"], page_n=page_n)
-        self.total_net = AmountField(api_prediction["total_net"], page_n=page_n)
-        self.total_tax = AmountField(api_prediction["total_tax"], page_n=page_n)
-        self.tip = AmountField(api_prediction["tip"], page_n=page_n)
-        self.date = DateField(api_prediction["date"], page_n=page_n)
-        self.category = ClassificationField(api_prediction["category"], page_n=page_n)
-        self.subcategory = ClassificationField(
-            api_prediction["subcategory"], page_n=page_n
+        self.category = ClassificationField(
+            api_prediction["category"],
+            page_id=page_n,
+        )
+        self.date = DateField(
+            api_prediction["date"],
+            page_id=page_n,
         )
         self.document_type = ClassificationField(
-            api_prediction["document_type"], page_n=page_n
+            api_prediction["document_type"],
+            page_id=page_n,
         )
-        self.supplier_name = TextField(
-            api_prediction["supplier_name"], value_key="value", page_n=page_n
+        self.line_items = [
+            ReceiptV5LineItem(prediction, page_id=page_n)
+            for prediction in api_prediction["line_items"]
+        ]
+        self.locale = LocaleField(
+            api_prediction["locale"],
+            page_id=page_n,
         )
-        self.supplier_phone_number = TextField(
-            api_prediction["supplier_phone_number"], value_key="value", page_n=page_n
+        self.subcategory = ClassificationField(
+            api_prediction["subcategory"],
+            page_id=page_n,
         )
         self.supplier_address = TextField(
-            api_prediction["supplier_address"], value_key="value", page_n=page_n
+            api_prediction["supplier_address"],
+            page_id=page_n,
         )
         self.supplier_company_registrations = [
-            CompanyRegistrationField(field_dict, page_n=page_n)
-            for field_dict in api_prediction["supplier_company_registrations"]
-        ]
-        self.time = TextField(api_prediction["time"], value_key="value", page_n=page_n)
-        self.taxes = [
-            TaxField(
-                tax_prediction,
-                page_n=page_n,
-                value_key="value",
-                rate_key="rate",
-                code_key="code",
-            )
-            for tax_prediction in api_prediction["taxes"]
-        ]
-        self.line_items = [
-            ReceiptV5LineItem(prediction=line_item, page_n=page_n)
-            for line_item in api_prediction["line_items"]
+            CompanyRegistrationField(prediction, page_id=page_n)
+            for prediction in api_prediction["supplier_company_registrations"]
         ]
+        self.supplier_name = TextField(
+            api_prediction["supplier_name"],
+            page_id=page_n,
+        )
+        self.supplier_phone_number = TextField(
+            api_prediction["supplier_phone_number"],
+            page_id=page_n,
+        )
+        self.taxes = Taxes(api_prediction["taxes"], page_id=page_n)
+        self.time = TextField(
+            api_prediction["time"],
+            page_id=page_n,
+        )
+        self.tip = AmountField(
+            api_prediction["tip"],
+            page_id=page_n,
+        )
+        self.total_amount = AmountField(
+            api_prediction["total_amount"],
+            page_id=page_n,
+        )
+        self.total_net = AmountField(
+            api_prediction["total_net"],
+            page_id=page_n,
+        )
+        self.total_tax = AmountField(
+            api_prediction["total_tax"],
+            page_id=page_n,
+        )
+
+    @staticmethod
+    def _line_items_separator(char: str) -> str:
+        out_str = "  "
+        out_str += f"+{char * 38}"
+        out_str += f"+{char * 10}"
+        out_str += f"+{char * 14}"
+        out_str += f"+{char * 12}"
+        return out_str + "+"
+
+    def _line_items_to_str(self) -> str:
+        if not self.line_items:
+            return ""
+
+        lines = f"\n{self._line_items_separator('-')}\n  ".join(
+            [item.to_table_line() for item in self.line_items]
+        )
+        out_str = ""
+        out_str += f"\n{self._line_items_separator('-')}\n "
+        out_str += " | Description                         "
+        out_str += " | Quantity"
+        out_str += " | Total Amount"
+        out_str += " | Unit Price"
+        out_str += f" |\n{self._line_items_separator('=')}"
+        out_str += f"\n  {lines}"
+        out_str += f"\n{self._line_items_separator('-')}"
+        return out_str
 
     def __str__(self) -> str:
-        taxes = "\n       ".join(f"{t}" for t in self.taxes)
         supplier_company_registrations = "; ".join(
             [str(n.value) for n in self.supplier_company_registrations]
         )
-        line_items = "\n"
-        if self.line_items:
-            line_items = (
-                "\n  +----------+----------+-----------+------------------------------------+"
-                "\n  | Quantity | Price    | Amount    | Description                        |"
-                "\n  +==========+==========+===========+====================================+"
-            )
-            for item in self.line_items:
-                line_items += (
-                    f"\n  {item}"
-                    "\n  +----------+----------+-----------+------------------------------------+"
-                )
-
         return clean_out_string(
-            "Receipt V5 Prediction\n=====================\n"
+            "Receipt V5 Prediction\n"
+            "=====================\n"
             f":Filename: {self.filename or ''}\n"
             f":Expense Locale: {self.locale}\n"
-            f":Total Amount: {self.total_amount}\n"
-            f":Total Excluding Taxes: {self.total_net}\n"
-            f":Tip and Gratuity: {self.tip}\n"
-            f":Purchase Date: {self.date}\n"
-            f":Purchase Time: {self.time}\n"
             f":Expense Category: {self.category}\n"
             f":Expense Sub Category: {self.subcategory}\n"
             f":Document Type: {self.document_type}\n"
+            f":Purchase Date: {self.date}\n"
+            f":Purchase Time: {self.time}\n"
+            f":Total Amount: {self.total_amount}\n"
+            f":Total Excluding Taxes: {self.total_net}\n"
+            f":Total Tax: {self.total_tax}\n"
+            f":Tip and Gratuity: {self.tip}\n"
+            f":Taxes: {self.taxes}\n"
             f":Supplier Name: {self.supplier_name}\n"
-            f":Supplier Phone Number: {self.supplier_phone_number}\n"
-            f":Supplier Address: {self.supplier_address}\n"
             f":Supplier Company Registrations: {supplier_company_registrations}\n"
-            f":Line Items: {line_items}\n"
-            f":Taxes: {taxes}\n"
-            f":Total Taxes: {self.total_tax}\n"
+            f":Supplier Address: {self.supplier_address}\n"
+            f":Supplier Phone Number: {self.supplier_phone_number}\n"
+            f":Line Items: {self._line_items_to_str()}\n"
         )
 
-    def _checklist(self) -> None:
-        pass
-
 
 TypeReceiptV5 = TypeVar("TypeReceiptV5", bound=ReceiptV5)
```

### Comparing `mindee-3.8.2/mindee/documents/shipping_container/shipping_container_v1.py` & `mindee-3.9.0/mindee/documents/shipping_container/shipping_container_v1.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,23 +42,23 @@
         Build the object from the prediction API JSON.
 
         :param api_prediction: Raw prediction from HTTP response
         :param page_n: Page number
         """
         self.owner = TextField(
             api_prediction["owner"],
-            page_n=page_n,
+            page_id=page_n,
         )
         self.serial_number = TextField(
             api_prediction["serial_number"],
-            page_n=page_n,
+            page_id=page_n,
         )
         self.size_type = TextField(
             api_prediction["size_type"],
-            page_n=page_n,
+            page_id=page_n,
         )
 
     def __str__(self) -> str:
         return clean_out_string(
             "----- Shipping Container V1 -----\n"
             f"Filename: {self.filename or ''}\n"
             f"Owner: { self.owner }\n"
```

### Comparing `mindee-3.8.2/mindee/documents/us/bank_check/bank_check_v1.py` & `mindee-3.9.0/mindee/documents/us/bank_check/bank_check_v1.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,21 +51,25 @@
     ) -> None:
         """
         Build the document from an API response JSON.
 
         :param api_prediction: Raw prediction from HTTP response
         :param page_n: Page number for multi pages pdf input
         """
-        self.routing_number = TextField(api_prediction["routing_number"], page_n=page_n)
-        self.account_number = TextField(api_prediction["account_number"], page_n=page_n)
-        self.check_number = TextField(api_prediction["check_number"], page_n=page_n)
-        self.date = DateField(api_prediction["date"], page_n=page_n)
-        self.amount = AmountField(api_prediction["amount"], page_n=page_n)
+        self.routing_number = TextField(
+            api_prediction["routing_number"], page_id=page_n
+        )
+        self.account_number = TextField(
+            api_prediction["account_number"], page_id=page_n
+        )
+        self.check_number = TextField(api_prediction["check_number"], page_id=page_n)
+        self.date = DateField(api_prediction["date"], page_id=page_n)
+        self.amount = AmountField(api_prediction["amount"], page_id=page_n)
         self.payees = [
-            TextField(payee, page_n=page_n) for payee in api_prediction["payees"]
+            TextField(payee, page_id=page_n) for payee in api_prediction["payees"]
         ]
         self.check_position = PositionField(
             api_prediction["check_position"], page_n=page_n
         )
         self.signatures_positions = [
             PositionField(signature_position, page_n=page_n)
             for signature_position in api_prediction["signatures_positions"]
```

### Comparing `mindee-3.8.2/mindee/endpoints.py` & `mindee-3.9.0/mindee/endpoints.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/mindee/fields/amount.py` & `mindee-3.9.0/mindee/fields/text.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,30 @@
 from typing import Optional
 
-from mindee.fields.base import (
-    BaseField,
-    FieldPositionMixin,
-    TypePrediction,
-    float_to_string,
-)
+from mindee.fields.base import BaseField, FieldPositionMixin, TypePrediction
 
 
-class AmountField(FieldPositionMixin, BaseField):
-    value: Optional[float] = None
+class TextField(FieldPositionMixin, BaseField):
+    value: Optional[str] = None
 
     def __init__(
         self,
         prediction: TypePrediction,
+        value_key: str = "value",
         reconstructed: bool = False,
-        page_n: Optional[int] = None,
+        page_id: Optional[int] = None,
     ):
         """
-        Amount field object.
+        Text field object.
 
         :param prediction: Amount prediction object from HTTP response
+        :param value_key: Key to use in the amount_prediction dict
         :param reconstructed: Bool for reconstructed object (not extracted in the API)
-        :param page_n: Page number for multi-page document
+        :param page_id: Page number for multi-page document
         """
         super().__init__(
             prediction,
-            value_key="value",
+            value_key=value_key,
             reconstructed=reconstructed,
-            page_n=page_n,
+            page_n=page_id,
         )
-        try:
-            self.value = round(float(prediction["value"]), 3)
-        except (ValueError, TypeError, KeyError):
-            self.value = None
-            self.confidence = 0.0
-
         self._set_position(prediction)
-
-    def __str__(self) -> str:
-        return float_to_string(self.value)
```

### Comparing `mindee-3.8.2/mindee/fields/base.py` & `mindee-3.9.0/mindee/fields/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 from mindee.geometry import Point, Polygon, Quadrilateral, get_bounding_box
 
 TypePrediction = Dict[str, Any]
 
 
 class FieldPositionMixin:
+    """Mixin class to add position information."""
+
     bounding_box: Optional[Quadrilateral]
     """A right rectangle containing the word in the document."""
     polygon: Polygon
     """A polygon containing the word in the document."""
 
     def _set_position(self, prediction: TypePrediction):
         self.bounding_box = None
@@ -20,19 +22,30 @@
             )
         except KeyError:
             pass
         if self.polygon:
             self.bounding_box = get_bounding_box(self.polygon)
 
 
-class BaseField:
+class FieldConfidenceMixin:
+    """Mixin class to add a confidence score."""
+
+    confidence: float = 0.0
+    """The confidence score."""
+
+    def _set_confidence(self, prediction: TypePrediction):
+        try:
+            self.confidence = float(prediction["confidence"])
+        except (KeyError, TypeError):
+            pass
+
+
+class BaseField(FieldConfidenceMixin):
     value: Optional[Any] = None
     """Raw field value"""
-    confidence: float = 0.0
-    """Confidence score"""
     reconstructed: bool
     """Whether the field was reconstructed from other fields."""
     page_n: Optional[int] = None
     """The document page on which the information was found."""
 
     def __init__(
         self,
@@ -59,18 +72,15 @@
 
         self.reconstructed = reconstructed
 
         if value_key not in prediction or prediction[value_key] == "N/A":
             return
 
         self.value = prediction[value_key]
-        try:
-            self.confidence = float(prediction["confidence"])
-        except (KeyError, TypeError):
-            pass
+        self._set_confidence(prediction)
 
     def __eq__(self, other: Any) -> bool:
         if not isinstance(other, BaseField):
             return NotImplemented
         if self.value is None and other.value is None:
             return True
         if self.value is None or other.value is None:
@@ -135,12 +145,21 @@
         except (AttributeError, TypeError):
             return 0.0
     return float(arr_sum)
 
 
 def float_to_string(value: Optional[float], min_precision=2) -> str:
     """Print a float with a specified minimum precision, but allowing greater precision."""
-    if value is not None:
-        precision = len(str(value).split(".")[1])
-        precision = max(precision, min_precision)
-        return f"{value:.{precision}f}"
-    return ""
+    if value is None:
+        return ""
+
+    precision = len(str(value).split(".")[1])
+    precision = max(precision, min_precision)
+    return f"{value:.{precision}f}"
+
+
+def to_opt_float(prediction: TypePrediction, key: str) -> Optional[float]:
+    """Make sure a prediction value is either a ``float`` or ``None``."""
+    try:
+        return float(prediction[key])
+    except TypeError:
+        return None
```

### Comparing `mindee-3.8.2/mindee/fields/classification.py` & `mindee-3.9.0/mindee/fields/classification.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,23 +10,23 @@
     """The value as a string."""
 
     def __init__(
         self,
         prediction: TypePrediction,
         value_key: str = "value",
         reconstructed: bool = False,
-        page_n: Optional[int] = None,
+        page_id: Optional[int] = None,
     ):
         """
         Text field object.
 
         :param prediction: Amount prediction object from HTTP response
         :param value_key: Key to use in the amount_prediction dict
         :param reconstructed: Bool for reconstructed object (not extracted in the API)
-        :param page_n: Page number for multi-page document
+        :param page_id: Page number for multi-page document
         """
         super().__init__(
             prediction,
             value_key=value_key,
             reconstructed=reconstructed,
-            page_n=page_n,
+            page_n=page_id,
         )
```

### Comparing `mindee-3.8.2/mindee/fields/company_registration.py` & `mindee-3.9.0/mindee/fields/company_registration.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
     """The type of registration."""
 
     def __init__(
         self,
         prediction: TypePrediction,
         value_key: str = "value",
         reconstructed: bool = False,
-        page_n: Optional[int] = None,
+        page_id: Optional[int] = None,
     ):
-        super().__init__(prediction, value_key, reconstructed, page_n)
+        super().__init__(prediction, value_key, reconstructed, page_id)
         self.type = prediction["type"]
         self._set_position(prediction)
 
     def __str__(self) -> str:
         if self.value:
             return f"{self.type}: {self.value}"
         return ""
```

### Comparing `mindee-3.8.2/mindee/fields/date.py` & `mindee-3.9.0/mindee/fields/date.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,28 +15,28 @@
     value: Optional[str] = None
     """The raw field value."""
 
     def __init__(
         self,
         prediction: TypePrediction,
         reconstructed: bool = False,
-        page_n: Optional[int] = None,
+        page_id: Optional[int] = None,
     ):
         """
         Date field object.
 
         :param prediction: Date prediction object from HTTP response
         :param reconstructed: Bool for reconstructed object (not extracted in the API)
-        :param page_n: Page number for multi-page document
+        :param page_id: Page number for multi-page document
         """
         super().__init__(
             prediction,
             value_key="value",
             reconstructed=reconstructed,
-            page_n=page_n,
+            page_n=page_id,
         )
         self._set_position(prediction)
 
         if self.value:
             try:
                 self.date_object = (
                     datetime.strptime(self.value, ISO8601_DATE_FORMAT)
```

### Comparing `mindee-3.8.2/mindee/fields/locale.py` & `mindee-3.9.0/mindee/fields/locale.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,31 +10,31 @@
     """ISO 3166-1 alpha-2 country code"""
     currency: Optional[str] = None
     """ISO 4217 currency code"""
 
     def __init__(
         self,
         prediction: TypePrediction,
-        value_key: str = "value",
         reconstructed: bool = False,
-        page_n: Optional[int] = None,
+        page_id: Optional[int] = None,
     ):
         """
         Locale field object.
 
         :param prediction: Locale prediction object from HTTP response
-        :param value_key: Key to use in the locale_prediction dict
         :param reconstructed: Bool for reconstructed object (not extracted in the API)
-        :param page_n: Page number for multi-page document
+        :param page_id: Page number for multi-page document
         """
+        value_key = "value" if "value" in prediction else "language"
+
         super().__init__(
             prediction,
             value_key=value_key,
             reconstructed=reconstructed,
-            page_n=page_n,
+            page_n=page_id,
         )
         self.language = self._get_value(prediction, "language")
         self.country = self._get_value(prediction, "country")
         self.currency = self._get_value(prediction, "currency")
 
     @staticmethod
     def _get_value(locale_prediction: dict, key: str) -> Optional[str]:
```

### Comparing `mindee-3.8.2/mindee/fields/orientation.py` & `mindee-3.9.0/mindee/fields/orientation.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/mindee/fields/payment_details.py` & `mindee-3.9.0/mindee/fields/payment_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,35 +18,35 @@
         prediction: TypePrediction,
         value_key: str = "iban",
         account_number_key: str = "account_number",
         iban_key: str = "iban",
         routing_number_key: str = "routing_number",
         swift_key: str = "swift",
         reconstructed: bool = False,
-        page_n: Optional[int] = None,
+        page_id: Optional[int] = None,
     ):
         """
         Payment details field object.
 
         :param prediction: Payment detail prediction object from HTTP response
         :param value_key: Corresponds to iban
         :param account_number_key: Key to use for getting the account number in the
             payment_details_prediction dict
         :param iban_key: Key to use for getting the IBAN in the payment_details_prediction dict
         :param routing_number_key: Key to use for getting the Routing number in the
             payment_details_prediction dict
         :param swift_key: Key to use for getting the SWIFT  in the payment_details_prediction dict
         :param reconstructed: Bool for reconstructed object (not extracted in the API)
-        :param page_n: Page number for multi-page document
+        :param page_id: Page number for multi-page document
         """
         super().__init__(
             prediction,
             value_key=value_key,
             reconstructed=reconstructed,
-            page_n=page_n,
+            page_n=page_id,
         )
 
         self._set_position(prediction)
 
         try:
             assert isinstance(prediction[account_number_key], str)
             self.account_number = str(prediction[account_number_key])
```

### Comparing `mindee-3.8.2/mindee/fields/position.py` & `mindee-3.9.0/mindee/fields/position.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/mindee/geometry.py` & `mindee-3.9.0/mindee/geometry.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/mindee/input/page_options.py` & `mindee-3.9.0/mindee/input/page_options.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/mindee/input/sources.py` & `mindee-3.9.0/mindee/input/sources.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/mindee/response.py` & `mindee-3.9.0/mindee/response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, Generic, List, Optional, Union
 
-from mindee.documents.base import TypeDocument
+from mindee.documents.base import TypeApiPrediction, TypeDocument
 from mindee.documents.config import DocumentConfig
+from mindee.fields.ocr import Ocr
 from mindee.input.sources import LocalInputSource, UrlInputSource
 from mindee.logger import logger
 
 
 class RequestStatus(Enum):
     FAILURE = "failure"
     SUCCESS = "success"
@@ -71,28 +72,30 @@
 class PredictResponse(Generic[TypeDocument]):
     """
     Response of a prediction request.
 
     This is a generic class, so certain class properties depend on the document type.
     """
 
-    http_response: Dict[str, Any]
+    http_response: TypeApiPrediction
     """Raw HTTP response JSON"""
     document_type: Optional[str] = None
     """Document type"""
     input_path: Optional[str] = None
     """Path of the input file"""
     input_filename: Optional[str] = None
     """Name of the input file"""
     input_mimetype: Optional[str] = None
     """MIME type of the input file"""
     document: Optional[TypeDocument]
     """An instance of the ``Document`` class, according to the type given."""
     pages: List[TypeDocument]
     """A list of instances of the ``Document`` class, according to the type given."""
+    ocr: Optional[Ocr]
+    """Full OCR operation results."""
 
     def __init__(
         self,
         doc_config: DocumentConfig,
         http_response: Dict[str, Any],
         input_source: Optional[Union[LocalInputSource, UrlInputSource]],
         response_ok: bool,
@@ -112,16 +115,25 @@
         if isinstance(input_source, LocalInputSource):
             self.input_path = input_source.filepath
             self.input_filename = input_source.filename
             self.input_mimetype = input_source.file_mimetype
 
         if not response_ok:
             self.document = None
+            self.ocr = None
         else:
             self._load_response(doc_config, input_source)
+            self.ocr = self._load_ocr(http_response)
+
+    @staticmethod
+    def _load_ocr(http_response: TypeApiPrediction):
+        ocr_prediction = http_response["document"].get("ocr", None)
+        if not ocr_prediction or not ocr_prediction.get("mvision-v1", None):
+            return None
+        return Ocr(ocr_prediction)
 
     def _load_response(
         self,
         doc_config: DocumentConfig,
         input_source: Optional[Union[LocalInputSource, UrlInputSource]],
     ) -> None:
         # This is some seriously ugly stuff.
```

### Comparing `mindee-3.8.2/mindee/versions.py` & `mindee-3.9.0/mindee/versions.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/mindee.egg-info/PKG-INFO` & `mindee-3.9.0/mindee.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindee
-Version: 3.8.2
+Version: 3.9.0
 Summary: Mindee API helper library for Python
 Home-page: https://mindee.com/
 Author: Mindee
 Author-email: devrel@mindee.com
 License: MIT
 Project-URL: Documentation, https://developers.mindee.com/docs/python-sdk
 Project-URL: Source, https://github.com/publicMindee/mindee-api-python
```

### Comparing `mindee-3.8.2/mindee.egg-info/SOURCES.txt` & `mindee-3.9.0/mindee.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -28,55 +28,57 @@
 mindee/documents/cropper/cropper_v1.py
 mindee/documents/custom/__init__.py
 mindee/documents/custom/custom_v1.py
 mindee/documents/custom/custom_v1_fields.py
 mindee/documents/eu/__init__.py
 mindee/documents/eu/license_plate/__init__.py
 mindee/documents/eu/license_plate/license_plate_v1.py
-mindee/documents/financial/__init__.py
-mindee/documents/financial/financial_document_v1.py
-mindee/documents/financial/financial_v1.py
+mindee/documents/financial_document/__init__.py
+mindee/documents/financial_document/financial_document_v1.py
+mindee/documents/financial_document/financial_document_v1_line_item.py
+mindee/documents/financial_document/financial_v1.py
 mindee/documents/fr/__init__.py
 mindee/documents/fr/bank_account_details/__init__.py
 mindee/documents/fr/bank_account_details/bank_account_details_v1.py
 mindee/documents/fr/carte_grise/__init__.py
 mindee/documents/fr/carte_grise/carte_grise_v1.py
 mindee/documents/fr/carte_vitale/__init__.py
 mindee/documents/fr/carte_vitale/carte_vitale_v1.py
 mindee/documents/fr/id_card/__init__.py
 mindee/documents/fr/id_card/id_card_v1.py
 mindee/documents/invoice/__init__.py
 mindee/documents/invoice/checks.py
 mindee/documents/invoice/invoice_v3.py
 mindee/documents/invoice/invoice_v4.py
-mindee/documents/invoice/line_item_v4.py
+mindee/documents/invoice/invoice_v4_line_item.py
 mindee/documents/invoice/reconstruct.py
 mindee/documents/invoice_splitter/__init__.py
 mindee/documents/invoice_splitter/invoice_splitter_v1.py
 mindee/documents/passport/__init__.py
 mindee/documents/passport/passport_v1.py
 mindee/documents/proof_of_address/__init__.py
 mindee/documents/proof_of_address/proof_of_address_v1.py
 mindee/documents/receipt/__init__.py
-mindee/documents/receipt/line_item_v5.py
 mindee/documents/receipt/receipt_v3.py
 mindee/documents/receipt/receipt_v4.py
 mindee/documents/receipt/receipt_v5.py
+mindee/documents/receipt/receipt_v5_line_item.py
 mindee/documents/shipping_container/__init__.py
 mindee/documents/shipping_container/shipping_container_v1.py
 mindee/documents/us/__init__.py
 mindee/documents/us/bank_check/__init__.py
 mindee/documents/us/bank_check/bank_check_v1.py
 mindee/fields/__init__.py
 mindee/fields/amount.py
 mindee/fields/base.py
 mindee/fields/classification.py
 mindee/fields/company_registration.py
 mindee/fields/date.py
 mindee/fields/locale.py
+mindee/fields/ocr.py
 mindee/fields/orientation.py
 mindee/fields/payment_details.py
 mindee/fields/position.py
 mindee/fields/tax.py
 mindee/fields/text.py
 mindee/input/__init__.py
 mindee/input/page_options.py
@@ -108,11 +110,12 @@
 tests/documents/us/__init__.py
 tests/documents/us/test_bank_check_v1.py
 tests/fields/__init__.py
 tests/fields/test_amount.py
 tests/fields/test_date.py
 tests/fields/test_field.py
 tests/fields/test_locale.py
+tests/fields/test_ocr.py
 tests/fields/test_orientation.py
 tests/fields/test_payment_details.py
 tests/fields/test_position.py
 tests/fields/test_tax.py
```

### Comparing `mindee-3.8.2/pyproject.toml` & `mindee-3.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/setup.cfg` & `mindee-3.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/tests/documents/fr/test_bank_account_details_v1.py` & `mindee-3.9.0/tests/documents/fr/test_bank_account_details_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/tests/documents/fr/test_carte_grise_v1.py` & `mindee-3.9.0/tests/documents/fr/test_carte_grise_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/tests/documents/fr/test_carte_vitale_v1.py` & `mindee-3.9.0/tests/documents/fr/test_carte_vitale_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/tests/documents/fr/test_id_card_v1.py` & `mindee-3.9.0/tests/documents/fr/test_id_card_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/tests/documents/test_cropper_v1.py` & `mindee-3.9.0/tests/documents/test_cropper_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/tests/documents/test_custom_v1.py` & `mindee-3.9.0/tests/documents/test_custom_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/tests/documents/test_financial_document_v1.py` & `mindee-3.9.0/tests/documents/test_financial_document_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,30 +40,22 @@
 
 def test_doc_constructor_invoice(financial_doc_from_invoice_object):
     assert financial_doc_from_invoice_object.date.value == "2019-02-11"
     assert (
         financial_doc_from_invoice_object.supplier_address.value
         == "4490 Oak Drive Albany, NY 12210"
     )
-    doc_str = (
-        open(f"{FINANCIAL_DOC_DATA_DIR}/response_v1/invoice_to_string.txt")
-        .read()
-        .strip()
-    )
+    doc_str = open(f"{FINANCIAL_DOC_DATA_DIR}/response_v1/invoice_to_string.rst").read()
     assert str(financial_doc_from_invoice_object) == doc_str
 
 
 def test_doc_constructor_receipt(financial_doc_from_receipt_object):
     assert financial_doc_from_receipt_object.date.value == "2014-07-07"
     assert financial_doc_from_receipt_object.supplier_address.value is None
-    doc_str = (
-        open(f"{FINANCIAL_DOC_DATA_DIR}/response_v1/receipt_to_string.txt")
-        .read()
-        .strip()
-    )
+    doc_str = open(f"{FINANCIAL_DOC_DATA_DIR}/response_v1/receipt_to_string.rst").read()
     assert str(financial_doc_from_receipt_object) == doc_str
 
 
 def test_all_na(financial_doc_object_all_na):
     assert financial_doc_object_all_na.orientation is None
     assert financial_doc_object_all_na.locale.value is None
     assert financial_doc_object_all_na.total_amount.value is None
```

### Comparing `mindee-3.8.2/tests/documents/test_financial_v1.py` & `mindee-3.9.0/tests/documents/test_financial_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/tests/documents/test_invoice_splitter_v1.py` & `mindee-3.9.0/tests/documents/test_invoice_splitter_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/tests/documents/test_invoice_v3.py` & `mindee-3.9.0/tests/documents/test_invoice_v3.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,20 +43,20 @@
         is True
     )
     assert invoice_v3_doc_object.total_tax.value == 97.98
     assert invoice_v3_doc_object.invoice_date.value == "2020-02-17"
     assert invoice_v3_doc_object.invoice_date.confidence == 0.99
     assert invoice_v3_doc_object.invoice_number.value == "0042004801351"
     assert invoice_v3_doc_object.invoice_number.confidence == 0.95
-    doc_str = open(f"{INVOICE_DATA_DIR}/response_v3/doc_to_string.txt").read().strip()
+    doc_str = open(f"{INVOICE_DATA_DIR}/response_v3/doc_to_string.rst").read().strip()
     assert str(invoice_v3_doc_object) == doc_str
 
 
 def test_page_constructor(invoice_v3_page_object):
-    doc_str = open(f"{INVOICE_DATA_DIR}/response_v3/page0_to_string.txt").read().strip()
+    doc_str = open(f"{INVOICE_DATA_DIR}/response_v3/page0_to_string.rst").read().strip()
     assert invoice_v3_page_object.orientation.value == 0
     assert invoice_v3_page_object.invoice_number.page_n == 0
     assert str(invoice_v3_page_object) == doc_str
     assert len(invoice_v3_page_object.cropper) == 0
 
 
 def test_all_na(invoice_v3_doc_object_empty):
```

### Comparing `mindee-3.8.2/tests/documents/test_invoice_v4.py` & `mindee-3.9.0/tests/documents/test_invoice_v4.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,20 +48,20 @@
     assert invoice_v4_doc_object.invoice_date.value == "2020-02-17"
     assert invoice_v4_doc_object.invoice_date.confidence == 0.99
     assert invoice_v4_doc_object.invoice_number.value == "0042004801351"
     assert invoice_v4_doc_object.invoice_number.confidence == 0.95
     for line_item in invoice_v4_doc_object.line_items:
         assert line_item.page_n == 0 or line_item.page_n == 1
         assert len(line_item.polygon) == 4
-    doc_str = open(f"{INVOICE_DATA_DIR}/response_v4/doc_to_string.txt").read().strip()
+    doc_str = open(f"{INVOICE_DATA_DIR}/response_v4/doc_to_string.rst").read().strip()
     assert str(invoice_v4_doc_object) == doc_str
 
 
 def test_page_constructor(invoice_v4_page_object):
-    doc_str = open(f"{INVOICE_DATA_DIR}/response_v4/page0_to_string.txt").read().strip()
+    doc_str = open(f"{INVOICE_DATA_DIR}/response_v4/page0_to_string.rst").read().strip()
     assert invoice_v4_page_object.orientation.value == 0
     assert invoice_v4_page_object.invoice_number.page_n == 0
     assert str(invoice_v4_page_object) == doc_str
     assert len(invoice_v4_page_object.cropper) == 0
     for line_item in invoice_v4_page_object.line_items:
         assert line_item.page_n == 0
         assert len(line_item.polygon) == 4
```

### Comparing `mindee-3.8.2/tests/documents/test_passport_v1.py` & `mindee-3.9.0/tests/documents/test_passport_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/tests/documents/test_proof_of_address_v1.py` & `mindee-3.9.0/tests/documents/test_proof_of_address_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/tests/documents/test_receipt_v3.py` & `mindee-3.9.0/tests/documents/test_receipt_v3.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     return json_data["document"]["inference"]["pages"][0]
 
 
 def test_doc_constructor(receipt_v3_doc_object):
     assert receipt_v3_doc_object.date.value == "2016-02-26"
     assert receipt_v3_doc_object.total_tax.value == 1.7
     assert receipt_v3_doc_object.checklist["taxes_match_total_incl"] is True
-    doc_str = open(f"{RECEIPT_DATA_DIR}/response_v3/doc_to_string.txt").read().strip()
+    doc_str = open(f"{RECEIPT_DATA_DIR}/response_v3/doc_to_string.rst").read().strip()
     assert receipt_v3_doc_object.date.page_n == 0
     assert str(receipt_v3_doc_object) == doc_str
 
 
 def test_all_na(receipt_v3_doc_object_empty):
     assert receipt_v3_doc_object_empty.locale.value is None
     assert receipt_v3_doc_object_empty.total_incl.value is None
```

### Comparing `mindee-3.8.2/tests/documents/test_receipt_v4.py` & `mindee-3.9.0/tests/documents/test_receipt_v4.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,24 +28,24 @@
         api_prediction=json_data["document"]["inference"]["pages"][0], page_n=0
     )
 
 
 def test_doc_constructor(receipt_v4_doc_object):
     assert receipt_v4_doc_object.date.value == "2014-07-07"
     assert receipt_v4_doc_object.total_tax.value == 3.34
-    doc_str = open(f"{RECEIPT_DATA_DIR}/response_v4/doc_to_string.txt").read().strip()
+    doc_str = open(f"{RECEIPT_DATA_DIR}/response_v4/doc_to_string.rst").read().strip()
     assert receipt_v4_doc_object.orientation is None
     assert receipt_v4_doc_object.date.page_n == 0
     assert str(receipt_v4_doc_object) == doc_str
 
 
 def test_page_constructor(receipt_v4_page_object):
     assert receipt_v4_page_object.date.value == "2014-07-07"
     assert receipt_v4_page_object.total_tax.value == 3.34
-    doc_str = open(f"{RECEIPT_DATA_DIR}/response_v4/page0_to_string.txt").read().strip()
+    doc_str = open(f"{RECEIPT_DATA_DIR}/response_v4/page0_to_string.rst").read().strip()
     assert receipt_v4_page_object.orientation.value == 0
     assert receipt_v4_page_object.date.page_n == 0
     assert str(receipt_v4_page_object) == doc_str
     assert len(receipt_v4_page_object.cropper) == 0
 
 
 def test_cropper():
```

### Comparing `mindee-3.8.2/tests/documents/test_receipt_v5.py` & `mindee-3.9.0/tests/documents/test_receipt_v5.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/tests/documents/test_shipping_container_v1.py` & `mindee-3.9.0/tests/documents/test_shipping_container_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/tests/documents/us/test_bank_check_v1.py` & `mindee-3.9.0/tests/documents/us/test_bank_check_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/tests/fields/test_amount.py` & `mindee-3.9.0/tests/fields/test_amount.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/tests/fields/test_date.py` & `mindee-3.9.0/tests/fields/test_date.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/tests/fields/test_field.py` & `mindee-3.9.0/tests/fields/test_field.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/tests/fields/test_locale.py` & `mindee-3.9.0/tests/fields/test_locale.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/tests/fields/test_orientation.py` & `mindee-3.9.0/tests/fields/test_orientation.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/tests/fields/test_payment_details.py` & `mindee-3.9.0/tests/fields/test_payment_details.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/tests/fields/test_position.py` & `mindee-3.9.0/tests/fields/test_position.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/tests/test_cli.py` & `mindee-3.9.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/tests/test_client.py` & `mindee-3.9.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/tests/test_geometry.py` & `mindee-3.9.0/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/tests/test_inputs.py` & `mindee-3.9.0/tests/test_inputs.py`

 * *Files identical despite different names*

### Comparing `mindee-3.8.2/tests/test_pkg_versions.py` & `mindee-3.9.0/tests/test_pkg_versions.py`

 * *Files identical despite different names*

