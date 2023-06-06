# Comparing `tmp/easypost-7.9.0.tar.gz` & `tmp/easypost-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easypost-7.9.0.tar", last modified: Wed Jan 18 18:04:37 2023, max compression
+gzip compressed data, was "easypost-8.0.0.tar", last modified: Tue Jun  6 21:45:20 2023, max compression
```

## Comparing `easypost-7.9.0.tar` & `easypost-8.0.0.tar`

### file list

```diff
@@ -1,56 +1,138 @@
-drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-01-18 18:04:37.058102 easypost-7.9.0/
--rw-r--r--   0 jhammond   (502) staff       (20)     9894 2023-01-18 18:04:12.000000 easypost-7.9.0/CHANGELOG.md
--rw-r--r--   0 jhammond   (502) staff       (20)     1092 2021-11-01 16:53:26.000000 easypost-7.9.0/LICENSE
--rw-r--r--   0 jhammond   (502) staff       (20)       13 2021-11-01 16:53:26.000000 easypost-7.9.0/MANIFEST.in
--rw-r--r--   0 jhammond   (502) staff       (20)     5838 2023-01-18 18:04:37.058228 easypost-7.9.0/PKG-INFO
--rw-r--r--   0 jhammond   (502) staff       (20)     4702 2023-01-11 17:02:39.000000 easypost-7.9.0/README.md
--rw-r--r--   0 jhammond   (502) staff       (20)     2371 2022-07-28 18:15:12.000000 easypost-7.9.0/UPGRADE_GUIDE.md
-drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-01-18 18:04:37.056665 easypost-7.9.0/easypost/
--rw-r--r--   0 jhammond   (502) staff       (20)     1329 2023-01-18 16:33:27.000000 easypost-7.9.0/easypost/__init__.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1939 2022-09-29 21:58:17.000000 easypost-7.9.0/easypost/address.py
--rw-r--r--   0 jhammond   (502) staff       (20)       74 2022-12-01 20:29:16.000000 easypost-7.9.0/easypost/api_key.py
--rw-r--r--   0 jhammond   (502) staff       (20)     2679 2022-07-05 19:20:56.000000 easypost-7.9.0/easypost/batch.py
-drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-01-18 18:04:37.057858 easypost-7.9.0/easypost/beta/
--rw-r--r--   0 jhammond   (502) staff       (20)       59 2022-08-25 19:10:57.000000 easypost-7.9.0/easypost/beta/__init__.py
--rw-r--r--   0 jhammond   (502) staff       (20)     7358 2023-01-11 17:02:39.000000 easypost-7.9.0/easypost/beta/referral.py
--rw-r--r--   0 jhammond   (502) staff       (20)     3177 2022-08-11 20:30:53.000000 easypost-7.9.0/easypost/billing.py
--rw-r--r--   0 jhammond   (502) staff       (20)       73 2022-07-05 19:20:56.000000 easypost-7.9.0/easypost/brand.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1936 2022-12-01 20:29:16.000000 easypost-7.9.0/easypost/carrier_account.py
--rw-r--r--   0 jhammond   (502) staff       (20)      142 2022-12-01 20:29:16.000000 easypost-7.9.0/easypost/constant.py
--rw-r--r--   0 jhammond   (502) staff       (20)       91 2022-07-05 19:20:56.000000 easypost-7.9.0/easypost/customs_info.py
--rw-r--r--   0 jhammond   (502) staff       (20)       91 2022-07-05 19:20:56.000000 easypost-7.9.0/easypost/customs_item.py
--rw-r--r--   0 jhammond   (502) staff       (20)     7203 2023-01-18 16:33:27.000000 easypost-7.9.0/easypost/easypost_object.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1545 2022-09-29 21:58:17.000000 easypost-7.9.0/easypost/endshipper.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1082 2022-12-01 20:29:16.000000 easypost-7.9.0/easypost/error.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1416 2023-01-18 16:33:27.000000 easypost-7.9.0/easypost/event.py
--rw-r--r--   0 jhammond   (502) staff       (20)      128 2022-07-05 19:20:56.000000 easypost-7.9.0/easypost/insurance.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1158 2022-07-05 19:20:56.000000 easypost-7.9.0/easypost/order.py
--rw-r--r--   0 jhammond   (502) staff       (20)       86 2022-07-05 19:20:56.000000 easypost-7.9.0/easypost/parcel.py
--rw-r--r--   0 jhammond   (502) staff       (20)       24 2023-01-18 16:33:27.000000 easypost-7.9.0/easypost/payload.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1234 2023-01-13 21:00:18.000000 easypost-7.9.0/easypost/pickup.py
--rw-r--r--   0 jhammond   (502) staff       (20)       78 2022-07-05 19:20:56.000000 easypost-7.9.0/easypost/pickup_rate.py
--rw-r--r--   0 jhammond   (502) staff       (20)       80 2022-07-05 19:20:56.000000 easypost-7.9.0/easypost/postage_label.py
--rw-r--r--   0 jhammond   (502) staff       (20)        0 2022-07-05 19:20:56.000000 easypost-7.9.0/easypost/py.typed
--rw-r--r--   0 jhammond   (502) staff       (20)       72 2022-07-05 19:20:56.000000 easypost-7.9.0/easypost/rate.py
--rw-r--r--   0 jhammond   (502) staff       (20)     5152 2023-01-11 17:02:39.000000 easypost-7.9.0/easypost/referral.py
--rw-r--r--   0 jhammond   (502) staff       (20)      125 2022-07-05 19:20:56.000000 easypost-7.9.0/easypost/refund.py
--rw-r--r--   0 jhammond   (502) staff       (20)     1017 2022-08-11 20:30:53.000000 easypost-7.9.0/easypost/report.py
--rw-r--r--   0 jhammond   (502) staff       (20)    13122 2022-08-22 20:51:17.000000 easypost-7.9.0/easypost/requestor.py
--rw-r--r--   0 jhammond   (502) staff       (20)     3788 2022-09-29 21:58:17.000000 easypost-7.9.0/easypost/resource.py
--rw-r--r--   0 jhammond   (502) staff       (20)      605 2022-08-11 20:30:53.000000 easypost-7.9.0/easypost/scanform.py
--rw-r--r--   0 jhammond   (502) staff       (20)     5723 2022-09-21 15:30:40.000000 easypost-7.9.0/easypost/shipment.py
--rw-r--r--   0 jhammond   (502) staff       (20)       81 2022-07-05 19:20:56.000000 easypost-7.9.0/easypost/tax_identifier.py
--rw-r--r--   0 jhammond   (502) staff       (20)      670 2022-07-05 19:20:56.000000 easypost-7.9.0/easypost/tracker.py
--rw-r--r--   0 jhammond   (502) staff       (20)     3246 2022-12-01 20:29:16.000000 easypost-7.9.0/easypost/user.py
--rw-r--r--   0 jhammond   (502) staff       (20)      966 2022-07-05 19:20:56.000000 easypost-7.9.0/easypost/util.py
--rw-r--r--   0 jhammond   (502) staff       (20)       99 2023-01-18 18:04:12.000000 easypost-7.9.0/easypost/version.py
--rw-r--r--   0 jhammond   (502) staff       (20)     2115 2022-07-28 18:15:12.000000 easypost-7.9.0/easypost/webhook.py
-drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-01-18 18:04:37.057442 easypost-7.9.0/easypost.egg-info/
--rw-r--r--   0 jhammond   (502) staff       (20)     5838 2023-01-18 18:04:37.000000 easypost-7.9.0/easypost.egg-info/PKG-INFO
--rw-r--r--   0 jhammond   (502) staff       (20)     1055 2023-01-18 18:04:37.000000 easypost-7.9.0/easypost.egg-info/SOURCES.txt
--rw-r--r--   0 jhammond   (502) staff       (20)        1 2023-01-18 18:04:37.000000 easypost-7.9.0/easypost.egg-info/dependency_links.txt
--rw-r--r--   0 jhammond   (502) staff       (20)      270 2023-01-18 18:04:37.000000 easypost-7.9.0/easypost.egg-info/requires.txt
--rw-r--r--   0 jhammond   (502) staff       (20)        9 2023-01-18 18:04:37.000000 easypost-7.9.0/easypost.egg-info/top_level.txt
--rw-r--r--   0 jhammond   (502) staff       (20)       63 2022-06-27 22:05:20.000000 easypost-7.9.0/pyproject.toml
--rw-r--r--   0 jhammond   (502) staff       (20)       70 2023-01-18 18:04:37.058498 easypost-7.9.0/setup.cfg
--rw-r--r--   0 jhammond   (502) staff       (20)     2142 2023-01-18 18:04:12.000000 easypost-7.9.0/setup.py
+drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-06-06 21:45:20.447738 easypost-8.0.0/
+-rw-r--r--   0 jhammond   (502) staff       (20)    11825 2023-06-06 21:44:38.000000 easypost-8.0.0/CHANGELOG.md
+-rw-r--r--   0 jhammond   (502) staff       (20)     1092 2021-11-01 16:53:26.000000 easypost-8.0.0/LICENSE
+-rw-r--r--   0 jhammond   (502) staff       (20)       13 2021-11-01 16:53:26.000000 easypost-8.0.0/MANIFEST.in
+-rw-r--r--   0 jhammond   (502) staff       (20)     7249 2023-06-06 21:45:20.447541 easypost-8.0.0/PKG-INFO
+-rw-r--r--   0 jhammond   (502) staff       (20)     6163 2023-05-31 19:04:35.000000 easypost-8.0.0/README.md
+-rw-r--r--   0 jhammond   (502) staff       (20)     7100 2023-06-06 21:44:38.000000 easypost-8.0.0/UPGRADE_GUIDE.md
+drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-06-06 21:45:20.432503 easypost-8.0.0/easypost/
+-rw-r--r--   0 jhammond   (502) staff       (20)      373 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/__init__.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1947 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/constant.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     3728 2023-06-06 21:44:36.000000 easypost-8.0.0/easypost/easypost_client.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     6705 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/easypost_object.py
+drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-06-06 21:45:20.433339 easypost-8.0.0/easypost/errors/
+-rw-r--r--   0 jhammond   (502) staff       (20)       87 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/__init__.py
+drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-06-06 21:45:20.436463 easypost-8.0.0/easypost/errors/api/
+-rw-r--r--   0 jhammond   (502) staff       (20)     1187 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/api/__init__.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     2327 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/api/api_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       93 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/api/encoding_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       96 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/api/external_api_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       94 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/api/forbidden_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       99 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/api/gateway_timeout_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       89 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/api/http_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       99 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/api/internal_server_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       99 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/api/invalid_request_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       89 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/api/json_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      101 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/api/method_not_allowed_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       93 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/api/not_found_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       92 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/api/payment_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       94 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/api/rate_limit_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       93 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/api/redirect_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      103 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/api/service_unavailable_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       92 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/api/timeout_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       97 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/api/unauthorized_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       95 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/api/unknown_api_error.py
+drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-06-06 21:45:20.437578 easypost-8.0.0/easypost/errors/general/
+-rw-r--r--   0 jhammond   (502) staff       (20)      560 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/general/__init__.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      206 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/general/easypost_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      119 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/general/end_of_pagination_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      113 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/general/filtering_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      117 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/general/invalid_object_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      120 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/general/invalid_parameter_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      120 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/general/missing_parameter_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      125 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/errors/general/signature_verification_error.py
+drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-06-06 21:45:20.440616 easypost-8.0.0/easypost/models/
+-rw-r--r--   0 jhammond   (502) staff       (20)     1145 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/__init__.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       94 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/address.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       93 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/api_key.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       92 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/batch.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       94 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/billing.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       92 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/brand.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      101 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/carrier_account.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       98 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/customs_info.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       98 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/customs_item.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       97 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/end_shipper.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       92 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/event.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       96 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/insurance.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      477 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/order.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       93 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/parcel.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       94 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/payload.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      495 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/pickup.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       97 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/pickup_rate.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       99 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/postage_label.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       91 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/rate.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       93 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/refund.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       93 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/report.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       95 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/scan_form.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      483 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/shipment.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       94 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/tracker.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       91 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/user.py
+-rw-r--r--   0 jhammond   (502) staff       (20)       94 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/models/webhook.py
+-rw-r--r--   0 jhammond   (502) staff       (20)        0 2022-07-05 19:20:56.000000 easypost-8.0.0/easypost/py.typed
+-rw-r--r--   0 jhammond   (502) staff       (20)    11789 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/requestor.py
+drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-06-06 21:45:20.444168 easypost-8.0.0/easypost/services/
+-rw-r--r--   0 jhammond   (502) staff       (20)     1650 2023-06-06 21:44:36.000000 easypost-8.0.0/easypost/services/__init__.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     2469 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/address_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     4159 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/base_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     3266 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/batch_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1244 2023-06-06 21:44:36.000000 easypost-8.0.0/easypost/services/beta_carrier_metadata_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      898 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/beta_rate_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     2339 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/beta_referral_customer_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     2805 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/billing_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     2470 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/carrier_account_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1013 2023-06-06 21:44:36.000000 easypost-8.0.0/easypost/services/carrier_metadata_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      546 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/customs_info_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      546 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/customs_item_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1665 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/end_shipper_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1972 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/event_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1102 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/insurance_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1650 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/order_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      511 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/parcel_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1823 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/pickup_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      361 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/rate_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     5366 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/referral_customer_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1102 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/refund_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     2390 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/report_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1091 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/scan_form_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     5750 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/shipment_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1956 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/tracker_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     3131 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/user_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      996 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/services/webhook_service.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     4560 2023-05-31 19:04:35.000000 easypost-8.0.0/easypost/util.py
+drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-06-06 21:45:20.433205 easypost-8.0.0/easypost.egg-info/
+-rw-r--r--   0 jhammond   (502) staff       (20)     7249 2023-06-06 21:45:20.000000 easypost-8.0.0/easypost.egg-info/PKG-INFO
+-rw-r--r--   0 jhammond   (502) staff       (20)     3994 2023-06-06 21:45:20.000000 easypost-8.0.0/easypost.egg-info/SOURCES.txt
+-rw-r--r--   0 jhammond   (502) staff       (20)        1 2023-06-06 21:45:20.000000 easypost-8.0.0/easypost.egg-info/dependency_links.txt
+-rw-r--r--   0 jhammond   (502) staff       (20)      249 2023-06-06 21:45:20.000000 easypost-8.0.0/easypost.egg-info/requires.txt
+-rw-r--r--   0 jhammond   (502) staff       (20)        9 2023-06-06 21:45:20.000000 easypost-8.0.0/easypost.egg-info/top_level.txt
+-rw-r--r--   0 jhammond   (502) staff       (20)      272 2023-05-10 20:00:27.000000 easypost-8.0.0/pyproject.toml
+-rw-r--r--   0 jhammond   (502) staff       (20)       38 2023-06-06 21:45:20.447799 easypost-8.0.0/setup.cfg
+-rw-r--r--   0 jhammond   (502) staff       (20)     2125 2023-05-31 19:04:35.000000 easypost-8.0.0/setup.py
+drwxr-xr-x   0 jhammond   (502) staff       (20)        0 2023-06-06 21:45:20.447335 easypost-8.0.0/tests/
+-rw-r--r--   0 jhammond   (502) staff       (20)     4221 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_address.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     4436 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_batch.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1162 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_beta_carrier_metadata.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      792 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_beta_rate.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1854 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_beta_referral_customer.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     4084 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_billing.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     3344 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_carrier_account.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1108 2023-06-06 21:44:36.000000 easypost-8.0.0/tests/test_carrier_metadata.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      719 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_customs_info.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      708 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_customs_item.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1818 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_easypost_client.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1739 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_end_shipper.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     2285 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_error.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     3548 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_event.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     2167 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_insurance.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     2323 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_order.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      574 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_parcel.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     4184 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_pickup.py
+-rw-r--r--   0 jhammond   (502) staff       (20)      322 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_rate.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     4655 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_referral_customer.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1887 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_refund.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     2825 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_report.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     1776 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_scan_form.py
+-rw-r--r--   0 jhammond   (502) staff       (20)    13013 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_shipment.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     2128 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_tracker.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     3078 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_user.py
+-rw-r--r--   0 jhammond   (502) staff       (20)     3263 2023-05-31 19:04:35.000000 easypost-8.0.0/tests/test_webhook.py
```

### Comparing `easypost-7.9.0/CHANGELOG.md` & `easypost-8.0.0/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,48 @@
 # CHANGELOG
 
+## v8.0.0 (2023-06-06)
+
+See our [Upgrade Guide](UPGRADE_GUIDE.md#upgrading-from-7x-to-80) for more details.
+
+- New `EasyPostClient` object
+  - Logic is grouped together in Services and each EasyPost object has a new model (eg: `client.shipment.create()`)
+- Error handling overhaul
+  - Introduces ~2 dozen new error types that extend from either `ApiError` or `EasyPostError`
+  - ApiErrors behave like the previous `Error` class did. They will include a `message`, `http_status`, and `http_body`. Additionally, a new `code` and `errors` keys are present and populate when available
+- Beta namespace changed from `easypost.beta.x` to `client.beta_x`
+- Empty API response functions return `None` instead of `True`
+- Corrected naming conventions
+  - References to `Referral` are now `ReferralCustomer` and `referral_customer` to match the API and docs
+  - References to `Smartrate` are now `SmartRate` and `smart_rate` to match the API and docs
+  - References to `Scanform` are now `ScanForm` and `scan_form`
+  - `primary_or_secondary` paramater name for billing functions is now called `priority` to match the API and docs
+- The `update_email` function of the `referral_customer` service had the parameter order switched so `id` (previously called `user_id`) is first which matches the rest of the library
+- Retrieving carrier metadata is now in GA
+- Dropped Python 3.6 support
+- Bumps all dependencies
+
+## v7.13.0 (2023-05-02)
+
+- Adds `retrieve_estimated_delivery_date` function to the Shipment class
+
+## v7.12.0 (2023-04-18)
+
+- Adds beta `retrieve_carrier_metadata` function
+- Improves error deserialization to handle bad format returned from the JSON
+
+## v7.11.0 (2023-04-04)
+
+- Adds `get_next_page` function that retrieves the next page of results for a paginated collection
+
+## v7.10.0 (2023-02-17)
+
+- Adds beta `retrieve_stateless_rates` function
+- Adds `get_lowest_stateless_rate` function to filter the lowest stateless rate
+
 ## v7.9.0 (2023-01-18)
 
 - Adds `all` function to `Pickup` to retrieve all pickups
 - Adds `retrieve_payload` and `retrieve_all_payloads` functions to `Event`
 
 ## v7.8.0 (2023-01-11)
```

### Comparing `easypost-7.9.0/LICENSE` & `easypost-8.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easypost-7.9.0/PKG-INFO` & `easypost-8.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: easypost
-Version: 7.9.0
+Version: 8.0.0
 Summary: EasyPost Shipping API Client Library for Python
 Home-page: https://easypost.com/
 Author: EasyPost
 Author-email: support@easypost.com
 Project-URL: Docs, https://www.easypost.com/docs/api
 Project-URL: Tracker, https://github.com/EasyPost/easypost-python/issues
 Project-URL: Source, https://github.com/EasyPost/easypost-python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.6, <4
+Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # EasyPost Python Client Library
 
 [![CI](https://github.com/EasyPost/easypost-python/workflows/CI/badge.svg)](https://github.com/EasyPost/easypost-python/actions?query=workflow%3ACI)
@@ -51,17 +50,17 @@
 
 A simple create & buy shipment example:
 
 ```python
 import os
 import easypost
 
-easypost.api_key = os.getenv('EASYPOST_API_KEY')
+client = easypost.EasyPostClient(os.getenv('EASYPOST_API_KEY'))
 
-shipment = easypost.Shipment.create(
+shipment = client.shipment.create(
     from_address = {
         "name": "EasyPost",
         "street1": "118 2nd Street",
         "street2": "4th Floor",
         "city": "San Francisco",
         "state": "CA",
         "zip": "94105",
@@ -81,25 +80,33 @@
         "length": 10.2,
         "width": 7.8,
         "height": 4.3,
         "weight": 21.2,
     },
 )
 
-shipment.buy(rate=shipment.lowest_rate())
+bought_shipment = client.shipment.buy(shipment.id, rate=shipment.lowest_rate())
 
-print(shipment)
+print(bought_shipment)
 ```
 
 ## Documentation
 
-API Documentation can be found at: <https://easypost.com/docs/api>.
+API documentation can be found at: <https://easypost.com/docs/api>.
+
+Library documentation can be found on the web at: <https://easypost.github.io/easypost-python/> or by building them locally via the `make docs` command.
 
 Upgrading major versions of this project? Refer to the [Upgrade Guide](UPGRADE_GUIDE.md).
 
+## Support
+
+New features and bug fixes are released on the latest major release of this library. If you are on an older major release of this library, we recommend upgrading to the most recent release to take advantage of new features, bug fixes, and security patches. Older versions of this library will continue to work and be available as long as the API version they are tied to remains active; however, they will not receive updates and are considered EOL.
+
+For additional support, see our [org-wide support policy](https://github.com/EasyPost/.github/blob/main/SUPPORT.md).
+
 ## Development
 
 ```bash
 # Install dependencies
 make install
 
 # Lint project
@@ -143,7 +150,18 @@
 - `EASYPOST_PROD_API_KEY`
 
 Some tests may require an EasyPost user with a particular set of enabled features such as a `Partner` user when creating referrals. We have attempted to call out these functions in their respective docstrings. The following are required when you need to re-record cassettes for applicable tests:
 
 - `USPS_CARRIER_ACCOUNT_ID` (eg: one-call buying a shipment for non-EasyPost employees)
 - `PARTNER_USER_PROD_API_KEY` (eg: creating a referral user)
 - `REFERRAL_CUSTOMER_PROD_API_KEY` (eg: adding a credit card to a referral user)
+
+#### Google Cloud SDK
+
+To run the test suite with the Google Cloud SDK (`urlfetch` instead of the `requests` library), you'll need the following:
+
+1. Install the appengine Python package to this virtual environment: `venv/bin/pip install appengine-python-standard`
+1. Install the Google Cloud SDK
+   - [Direct Download](https://cloud.google.com/sdk/docs/install)
+   - [Homebrew](https://formulae.brew.sh/cask/google-cloud-sdk)
+1. Point the `PYTHONPATH` environment variable to the path of the newly installed `google-cloud-sdk` directory. For Homebrew, this is `"$(brew --prefix)/share/google-cloud-sdk"`
+1. Run the test suite with the commands listed in this README
```

### Comparing `easypost-7.9.0/easypost/batch.py` & `easypost-8.0.0/easypost/services/address_service.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,62 +1,72 @@
-from typing import Optional
+from typing import (
+    Any,
+    Dict,
+    Optional,
+)
 
 from easypost.easypost_object import convert_to_easypost_object
+from easypost.models import Address
 from easypost.requestor import (
     RequestMethod,
     Requestor,
 )
-from easypost.resource import (
-    AllResource,
-    CreateResource,
-)
+from easypost.services.base_service import BaseService
 
 
-class Batch(AllResource, CreateResource):
-    @classmethod
-    def create_and_buy(cls, api_key: Optional[str] = None, **params) -> "Batch":
-        """Create and buy a Batch."""
-        requestor = Requestor(local_api_key=api_key)
-        url = "%s/%s" % (cls.class_url(), "create_and_buy")
-        wrapped_params = {cls.snakecase_name(): params}
-        response, api_key = requestor.request(method=RequestMethod.POST, url=url, params=wrapped_params)
-        return convert_to_easypost_object(response=response, api_key=api_key)
-
-    def buy(self, **params) -> "Batch":
-        """Buy a batch."""
-        requestor = Requestor(local_api_key=self._api_key)
-        url = "%s/%s" % (self.instance_url(), "buy")
-        response, api_key = requestor.request(method=RequestMethod.POST, url=url, params=params)
-        self.refresh_from(values=response, api_key=api_key)
-        return self
-
-    def label(self, **params) -> "Batch":
-        """Create a batch label."""
-        requestor = Requestor(local_api_key=self._api_key)
-        url = "%s/%s" % (self.instance_url(), "label")
-        response, api_key = requestor.request(method=RequestMethod.POST, url=url, params=params)
-        self.refresh_from(values=response, api_key=api_key)
-        return self
-
-    def remove_shipments(self, **params) -> "Batch":
-        """Remove shipments from a batch."""
-        requestor = Requestor(local_api_key=self._api_key)
-        url = "%s/%s" % (self.instance_url(), "remove_shipments")
-        response, api_key = requestor.request(method=RequestMethod.POST, url=url, params=params)
-        self.refresh_from(values=response, api_key=api_key)
-        return self
-
-    def add_shipments(self, **params) -> "Batch":
-        """Add shipments from a batch."""
-        requestor = Requestor(local_api_key=self._api_key)
-        url = "%s/%s" % (self.instance_url(), "add_shipments")
-        response, api_key = requestor.request(method=RequestMethod.POST, url=url, params=params)
-        self.refresh_from(values=response, api_key=api_key)
-        return self
-
-    def create_scan_form(self, **params) -> "Batch":
-        """Create a scanform for a batch."""
-        requestor = Requestor(local_api_key=self._api_key)
-        url = "%s/%s" % (self.instance_url(), "scan_form")
-        response, api_key = requestor.request(method=RequestMethod.POST, url=url, params=params)
-        self.refresh_from(values=response, api_key=api_key)
-        return self
+class AddressService(BaseService):
+    def __init__(self, client):
+        self._client = client
+        self._model_class = Address.__name__
+
+    def create(
+        self,
+        verify: Optional[bool] = None,
+        verify_strict: Optional[bool] = None,
+        **params,
+    ) -> Address:
+        """Create an Address."""
+        url = self._class_url(self._model_class)
+        wrapped_params = {self._snakecase_name(self._model_class): params}  # type: Dict[str, Any]
+
+        if verify:
+            wrapped_params["verify"] = verify
+        if verify_strict:
+            wrapped_params["verify_strict"] = verify_strict
+
+        response = Requestor(self._client).request(method=RequestMethod.POST, url=url, params=wrapped_params)
+
+        return convert_to_easypost_object(response=response)
+
+    def all(self, **params) -> Dict[str, Any]:
+        """Retrieve a list of Addresses."""
+        return self._all_resources(self._model_class, **params)
+
+    def retrieve(self, id) -> Address:
+        """Retrieve an Address."""
+        return self._retrieve_resource(self._model_class, id)
+
+    def create_and_verify(self, **params) -> Address:
+        """Create and verify an Address in one call."""
+        url = f"{self._class_url('address')}/create_and_verify"
+        wrapped_params = {self._snakecase_name(self._model_class): params}
+
+        response = Requestor(self._client).request(method=RequestMethod.POST, url=url, params=wrapped_params)
+
+        return convert_to_easypost_object(response=response["address"])
+
+    def verify(self, id) -> Address:
+        """Verify an already created Address."""
+        url = f"{self._instance_url('address', id)}/verify"
+
+        response = Requestor(self._client).request(method=RequestMethod.GET, url=url)
+
+        return convert_to_easypost_object(response=response["address"])
+
+    def get_next_page(
+        self,
+        addresses: Dict[str, Any],
+        page_size: int,
+        optional_params: Optional[Dict[str, Any]] = None,
+    ) -> Dict[str, Any]:
+        """Retrieve the next page of the list Addresses response."""
+        return self._get_next_page_resources(self._model_class, addresses, page_size, optional_params)
```

### Comparing `easypost-7.9.0/easypost/beta/referral.py` & `easypost-8.0.0/easypost/services/referral_customer_service.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,192 +1,135 @@
+from copy import deepcopy
 from typing import (
     Any,
     Dict,
-    List,
     Optional,
 )
 
 import requests
 
+from easypost.constant import (
+    SEND_STRIPE_DETAILS_ERROR,
+    TIMEOUT,
+)
 from easypost.easypost_object import convert_to_easypost_object
-from easypost.error import Error
+from easypost.errors import ExternalApiError
+from easypost.models import User
 from easypost.requestor import (
     RequestMethod,
     Requestor,
 )
+from easypost.services.base_service import BaseService
 
 
-class Referral:
-    @staticmethod
-    def create(
-        api_key: Optional[str] = None,
-        **params,
-    ) -> Dict[str, Any]:
-        """Create a referral user.
+class ReferralCustomerService(BaseService):
+    def __init__(self, client):
+        self._client = client
+        self._model_class = User.__name__
+
+    def create(self, **params) -> User:
+        """Create a referral customer.
 
         This function requires the Partner User's API key.
         """
-        requestor = Requestor(local_api_key=api_key)
-        new_params = {"user": params}
-        response, api_key = requestor.request(
+        wrapped_params = {"user": params}
+
+        response = Requestor(self._client).request(
             method=RequestMethod.POST,
             url="/referral_customers",
-            params=new_params,
-            beta=True,
+            params=wrapped_params,
         )
-        return convert_to_easypost_object(response=response, api_key=api_key)
 
-    @staticmethod
-    def update_email(
-        email,
-        user_id,
-        api_key: Optional[str] = None,
-    ) -> bool:
-        """Update a referral user.
+        return convert_to_easypost_object(response=response)
+
+    def update_email(self, id: str, email: str) -> None:
+        """Update a referral customer.
 
         This function requires the Partner User's API key.
         """
-        requestor = Requestor(local_api_key=api_key)
-        url = f"/referral_customers/{user_id}"
+        url = f"/referral_customers/{id}"
         wrapped_params = {
             "user": {
                 "email": email,
             }
         }
-        _, _ = requestor.request(
+
+        Requestor(self._client).request(
             method=RequestMethod.PUT,
             url=url,
             params=wrapped_params,
-            beta=True,
         )
 
-        # Return true if succeeds, an error will be thrown if it fails
-        return True
-
-    @staticmethod
-    def all(
-        api_key: Optional[str] = None,
-        **params,
-    ) -> List:
-        """Retrieve a list of referral users.
+    def all(self, **params) -> Dict[str, Any]:
+        """Retrieve a list of referral customers.
 
         This function requires the Partner User's API key.
         """
-        requestor = Requestor(local_api_key=api_key)
-        response, api_key = requestor.request(
+        response = Requestor(self._client).request(
             method=RequestMethod.GET,
             url="/referral_customers",
             params=params,
-            beta=True,
         )
-        return convert_to_easypost_object(response=response, api_key=api_key)
 
-    @staticmethod
+        return convert_to_easypost_object(response=response)
+
+    def get_next_page(
+        self,
+        referral_customers: Dict[str, Any],
+        page_size: int,
+        optional_params: Optional[Dict[str, Any]] = None,
+    ) -> Dict[str, Any]:
+        """Retrieve next page of referral customers."""
+        return self._get_next_page_resources("referral_customers", referral_customers, page_size, optional_params)
+
     def add_credit_card(
+        self,
         referral_api_key: str,
         number: str,
         expiration_month: int,
         expiration_year: int,
         cvc: str,
-        primary_or_secondary: str = "primary",
+        priority: str = "primary",
     ) -> Dict[str, Any]:
-        """Add credit card to a referral user.
+        """Add credit card to a referral customer.
 
-        This function requires the Referral User's API key.
+        This function requires the ReferralCustomer User's API key.
         """
-        easypost_stripe_api_key = Referral._retrieve_easypost_stripe_api_key()
+        easypost_stripe_api_key = self._retrieve_easypost_stripe_api_key()
 
         try:
-            stripe_token = Referral._create_stripe_token(
-                number, expiration_month, expiration_year, cvc, easypost_stripe_api_key
+            stripe_token = self._create_stripe_token(
+                number,
+                expiration_month,
+                expiration_year,
+                cvc,
+                easypost_stripe_api_key,
             )
         except Exception:
-            raise Error(message="Could not send card details to Stripe, please try again later")
+            raise ExternalApiError(message=SEND_STRIPE_DETAILS_ERROR)
 
-        response = Referral._create_easypost_credit_card(
+        response = self._create_easypost_credit_card(
             referral_api_key,
             stripe_token.get("id", ""),
-            priority=primary_or_secondary,
-        )
-        return convert_to_easypost_object(response)
-
-    @staticmethod
-    def add_payment_method(
-        stripe_customer_id: str,
-        payment_method_reference: str,
-        primary_or_secondary: str = "primary",
-    ) -> Dict[str, Any]:
-        """Add a Stripe payment method to your EasyPost account.
-
-        This endpoint uses a user's personal Stripe account. The `stripe_customer_id`
-        and `payment_method_reference` IDs both come from Stripe. By adding these to
-        EasyPost, we will associate your Stripe payment method with either your primary
-        or secondary EasyPost payment method.
-        """
-        requestor = Requestor()
-        wrapped_params = {
-            "payment_method": {
-                "stripe_customer_id": stripe_customer_id,
-                "payment_method_reference": payment_method_reference,
-                "priority": primary_or_secondary,
-            }
-        }
-
-        response, api_key = requestor.request(
-            method=RequestMethod.POST,
-            url="/referral_customers/payment_method",
-            params=wrapped_params,
-            beta=True,
+            priority=priority,
         )
 
-        return convert_to_easypost_object(response=response, api_key=api_key)
-
-    @staticmethod
-    def refund_by_amount(refund_amount: int) -> Dict[str, Any]:
-        """Refund a ReferralCustomer wallet by specifying an amount."""
-        requestor = Requestor()
-        wrapped_params = {"refund_amount": refund_amount}
-
-        response, api_key = requestor.request(
-            method=RequestMethod.POST,
-            url="/referral_customers/refunds",
-            params=wrapped_params,
-            beta=True,
-        )
-
-        return convert_to_easypost_object(response=response, api_key=api_key)
-
-    @staticmethod
-    def refund_by_payment_log(payment_log_id: str) -> Dict[str, Any]:
-        """Refund a ReferralCustomer wallet by specifying a payment log ID to completely refund."""
-        requestor = Requestor()
-        wrapped_params = {"payment_log_id": payment_log_id}
-
-        response, api_key = requestor.request(
-            method=RequestMethod.POST,
-            url="/referral_customers/refunds",
-            params=wrapped_params,
-            beta=True,
-        )
-
-        return convert_to_easypost_object(response=response, api_key=api_key)
+        return convert_to_easypost_object(response)
 
-    @staticmethod
-    def _retrieve_easypost_stripe_api_key() -> str:
+    def _retrieve_easypost_stripe_api_key(self) -> str:
         """Retrieve EasyPost's Stripe public API key."""
-        requestor = Requestor()
-        public_key, _ = requestor.request(
+        public_key = Requestor(self._client).request(
             method=RequestMethod.GET,
             url="/partners/stripe_public_key",
-            beta=True,
         )
+
         return public_key.get("public_key", "")
 
-    @staticmethod
     def _create_stripe_token(
+        self,
         number: str,
         expiration_month: int,
         expiration_year: int,
         cvc: str,
         easypost_stripe_key: str,
     ) -> Dict[str, Any]:
         """Get credit card token from Stripe."""
@@ -208,33 +151,37 @@
         url = "https://api.stripe.com/v1/tokens"
 
         stripe_response = requests.post(
             url,
             params=form_encoded_params,
             headers=headers,
             auth=requests.auth.HTTPBasicAuth(easypost_stripe_key, ""),
+            timeout=TIMEOUT,
         )
+
         return stripe_response.json()
 
-    @staticmethod
     def _create_easypost_credit_card(
+        self,
         referral_api_key: str,
         stripe_object_id: str,
         priority: str = "primary",
     ) -> Dict[str, Any]:
         """Submit Stripe credit card token to EasyPost."""
-        requestor = Requestor(local_api_key=referral_api_key)
-
         params = {
             "credit_card": {
                 "stripe_object_id": stripe_object_id,
                 "priority": priority,
             }
         }
 
-        response, _ = requestor.request(
+        # Override the API key to use the referral's for this single request
+        referral_client = deepcopy(self._client)
+        referral_client.api_key = referral_api_key
+
+        response = Requestor(referral_client).request(
             method=RequestMethod.POST,
             params=params,
             url="/credit_cards",
-            beta=True,
         )
+
         return response
```

### Comparing `easypost-7.9.0/easypost/billing.py` & `easypost-8.0.0/easypost/services/billing_service.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,78 +1,78 @@
 from typing import (
     Any,
     Dict,
     List,
-    Optional,
 )
 
+from easypost.constant import (
+    INVALID_PAYMENT_METHOD_ERROR,
+    NO_BILLING_ERROR,
+)
 from easypost.easypost_object import convert_to_easypost_object
-from easypost.error import Error
+from easypost.errors import InvalidObjectError
+from easypost.models import Billing
 from easypost.requestor import (
     RequestMethod,
     Requestor,
 )
-from easypost.resource import Resource
+from easypost.services.base_service import BaseService
+
 
+class BillingService(BaseService):
+    def __init__(self, client):
+        self._client = client
+        self._model_class = Billing.__name__
 
-class Billing(Resource):
-    @classmethod
-    def fund_wallet(cls, amount: str, primary_or_secondary: str = "primary", api_key: Optional[str] = None) -> bool:
+    def fund_wallet(self, amount: str, priority: str = "primary") -> None:
         """Fund your EasyPost wallet by charging your primary or secondary payment method on file."""
-        endpoint, payment_method_id = Billing._get_payment_method_info(primary_or_secondary=primary_or_secondary)
+        endpoint, payment_method_id = self._get_payment_method_info(priority=priority)
 
-        requestor = Requestor(local_api_key=api_key)
         url = f"{endpoint}/{payment_method_id}/charges"
         wrapped_params = {"amount": amount}
-        requestor.request(method=RequestMethod.POST, url=url, params=wrapped_params)
 
-        # Return true if the request succeeds, an error will be thrown if it fails
-        return True
+        Requestor(self._client).request(method=RequestMethod.POST, url=url, params=wrapped_params)
 
-    @classmethod
-    def delete_payment_method(cls, primary_or_secondary: str, api_key: Optional[str] = None) -> bool:
+    def delete_payment_method(self, priority: str) -> None:
         """Delete a payment method."""
-        endpoint, payment_method_id = Billing._get_payment_method_info(primary_or_secondary=primary_or_secondary)
+        endpoint, payment_method_id = self._get_payment_method_info(priority=priority)
 
-        requestor = Requestor(local_api_key=api_key)
         url = f"{endpoint}/{payment_method_id}"
-        requestor.request(method=RequestMethod.DELETE, url=url)
 
-        # Return true if the request succeeds, an error will be thrown if it fails
-        return True
+        Requestor(self._client).request(method=RequestMethod.DELETE, url=url)
 
-    @classmethod
-    def retrieve_payment_methods(cls, api_key: Optional[str] = None, **params) -> Dict[str, Any]:
+    def retrieve_payment_methods(self, **params) -> Dict[str, Any]:
         """Retrieve payment methods."""
-        requestor = Requestor(local_api_key=api_key)
-        response, api_key = requestor.request(method=RequestMethod.GET, url="/payment_methods", params=params)
+        response = Requestor(self._client).request(
+            method=RequestMethod.GET,
+            url="/payment_methods",
+            params=params,
+        )
 
         if response.get("id") is None:
-            raise Error(message="Billing has not been setup for this user. Please add a payment method.")
+            raise InvalidObjectError(message=NO_BILLING_ERROR)
 
-        return convert_to_easypost_object(response=response, api_key=api_key)
+        return convert_to_easypost_object(response=response)
 
-    @classmethod
-    def _get_payment_method_info(cls, primary_or_secondary: str = "primary") -> List[str]:
+    def _get_payment_method_info(self, priority: str = "primary") -> List[str]:
         """Get payment method info (type of the payment method and ID of the payment method)"""
-        payment_methods = Billing.retrieve_payment_methods()
+        payment_methods = self.retrieve_payment_methods()
 
         payment_method_map = {
             "primary": "primary_payment_method",
             "secondary": "secondary_payment_method",
         }
 
-        payment_method_to_use = payment_method_map.get(primary_or_secondary)
-        error_string = "The chosen payment method is not valid. Please try again."
+        payment_method_to_use = payment_method_map.get(priority)
 
         if payment_method_to_use and payment_methods[payment_method_to_use]:
             payment_method_id = payment_methods[payment_method_to_use]["id"]
             if payment_method_id.startswith("card_"):
                 endpoint = "/credit_cards"
             elif payment_method_id.startswith("bank_"):
                 endpoint = "/bank_accounts"
             else:
-                raise Error(message=error_string)
+                raise InvalidObjectError(message=INVALID_PAYMENT_METHOD_ERROR)
         else:
-            raise Error(message=error_string)
+            raise InvalidObjectError(message=INVALID_PAYMENT_METHOD_ERROR)
 
         return [endpoint, payment_method_id]
```

### Comparing `easypost-7.9.0/easypost/endshipper.py` & `easypost-8.0.0/easypost/services/report_service.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,73 @@
-from typing import Optional
-
-from easypost.easypost_object import (
-    EasyPostObject,
-    convert_to_easypost_object,
+from typing import (
+    Any,
+    Dict,
+    Optional,
 )
+
+from easypost.constant import MISSING_PARAMETER_ERROR
+from easypost.easypost_object import convert_to_easypost_object
+from easypost.errors import MissingParameterError
+from easypost.models import Report
 from easypost.requestor import (
     RequestMethod,
     Requestor,
 )
-from easypost.resource import AllResource
+from easypost.services.base_service import BaseService
+
+
+class ReportService(BaseService):
+    def __init__(self, client):
+        self._client = client
+        self._model_class = Report.__name__
+
+    def create(self, **params) -> Report:
+        """Create a Report."""
+        refund_type = params.pop("type")
+
+        if refund_type is None:
+            raise MissingParameterError(MISSING_PARAMETER_ERROR.format("type"))
+
+        url = f"{self._class_url(self._model_class)}/{refund_type}"
+
+        response = Requestor(self._client).request(method=RequestMethod.POST, url=url, params=params)
+
+        return convert_to_easypost_object(response=response)
+
+    def all(self, **params) -> Dict[str, Any]:
+        """Retrieve a list of Reports."""
+        refund_type = params.pop("type")
+
+        if refund_type is None:
+            raise MissingParameterError(MISSING_PARAMETER_ERROR.format("type"))
+
+        url = f"{self._class_url(self._model_class)}/{refund_type}"
+
+        response = Requestor(self._client).request(method=RequestMethod.GET, url=url, params=params)
+        response["type"] = refund_type  # Needed for retrieving the next page
+
+        return convert_to_easypost_object(response=response)
+
+    def retrieve(self, id: str) -> Report:
+        """Retrieve a Report."""
+        return self._retrieve_resource(self._model_class, id)
+
+    def get_next_page(
+        self,
+        reports: Dict[str, Any],
+        page_size: Optional[int] = None,
+    ) -> Dict[str, Any]:
+        """Retrieve the next page of the list Report response."""
+        refund_type = reports.get("type")
+
+        if refund_type is None:
+            raise MissingParameterError(MISSING_PARAMETER_ERROR.format("type"))
 
+        url = f"{self._class_url(self._model_class)}/{refund_type}"
+        params = {
+            "before_id": reports["reports"][-1].id,
+            "page_size": page_size,
+        }
 
-class EndShipper(AllResource):
-    @classmethod
-    def create(cls, api_key: Optional[str] = None, **params) -> "EndShipper":
-        """Create an EndShipper."""
-        requestor = Requestor(local_api_key=api_key)
-        url = cls.class_url()
-        wrapped_params = {"address": params}
-        response, api_key = requestor.request(method=RequestMethod.POST, url=url, params=wrapped_params)
-        return convert_to_easypost_object(response=response, api_key=api_key)
-
-    def save(self) -> "EndShipper":
-        """Update an EndShipper object.
-
-        This function requires all parameters to be present for an EndShipper.
-        """
-        if self._unsaved_values:
-            requestor = Requestor(local_api_key=self._api_key)
-            params = {}
-            for k in self._unsaved_values:
-                params[k] = getattr(self, k)
-                if type(params[k]) is EasyPostObject:
-                    params[k] = params[k].flatten_unsaved()
-            wrapped_params = {"address": params}  # This function is overridden due to the key has to be `address`
-            url = self.instance_url()
-            response, api_key = requestor.request(method=RequestMethod.PUT, url=url, params=wrapped_params)
-            self.refresh_from(values=response, api_key=api_key)
+        response = Requestor(self._client).request(method=RequestMethod.GET, url=url, params=params)
 
-        return self
+        return convert_to_easypost_object(response=response)
```

### Comparing `easypost-7.9.0/easypost/event.py` & `easypost-8.0.0/easypost/services/beta_rate_service.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,32 @@
-import json
 from typing import (
-    List,
-    Optional,
+    Any,
+    Dict,
 )
 
-import easypost
 from easypost.easypost_object import convert_to_easypost_object
+from easypost.models import Rate
 from easypost.requestor import (
     RequestMethod,
     Requestor,
 )
-from easypost.resource import AllResource
+from easypost.services.base_service import BaseService
 
 
-class Event(AllResource):
-    @classmethod
-    def receive(cls, values: str) -> "Event":
-        return convert_to_easypost_object(response=json.loads(s=values), api_key=easypost.api_key)
-
-    @classmethod
-    def retrieve_all_payloads(cls, event_id: str, api_key: Optional[str] = None, **params) -> List["easypost.Payload"]:
-        """Retrieve a list of Payloads for an Event."""
-        requestor = Requestor(local_api_key=api_key)
-        url = f"{cls.class_url()}/{event_id}/payloads"
-        response, api_key = requestor.request(method=RequestMethod.GET, url=url, params=params)
-        return convert_to_easypost_object(response=response, api_key=api_key)
-
-    @classmethod
-    def retrieve_payload(
-        cls, event_id: str, payload_id: str, api_key: Optional[str] = None, **params
-    ) -> "easypost.Payload":
-        """Retrieve a Payload of an Event."""
-        requestor = Requestor(local_api_key=api_key)
-        url = f"{cls.class_url()}/{event_id}/payloads/{payload_id}"
-        response, api_key = requestor.request(method=RequestMethod.GET, url=url, params=params)
-        return convert_to_easypost_object(response=response, api_key=api_key)
+class BetaRateService(BaseService):
+    def __init__(self, client):
+        self._client = client
+        self._model_class = Rate.__name__
+
+    def retrieve_stateless_rates(self, **params) -> Dict[str, Any]:
+        """Retrieves stateless rates by passing shipment data."""
+        url = self._class_url(self._model_class)
+        wrapped_params = {"shipment": params}
+
+        response = Requestor(self._client).request(
+            method=RequestMethod.POST,
+            url=url,
+            params=wrapped_params,
+            beta=True,
+        )
+
+        return convert_to_easypost_object(response=response.get("rates", None))
```

### Comparing `easypost-7.9.0/easypost/pickup.py` & `easypost-8.0.0/easypost/services/pickup_service.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,56 @@
-from typing import List
+from typing import (
+    Any,
+    Dict,
+    Optional,
+)
 
+from easypost.easypost_object import convert_to_easypost_object
+from easypost.models import Pickup
 from easypost.requestor import (
     RequestMethod,
     Requestor,
 )
-from easypost.resource import (
-    AllResource,
-    CreateResource,
-)
-from easypost.util import get_lowest_object_rate
+from easypost.services.base_service import BaseService
+
+
+class PickupService(BaseService):
+    def __init__(self, client):
+        self._client = client
+        self._model_class = Pickup.__name__
+
+    def create(self, **params) -> Pickup:
+        """Create a Pickup."""
+        return self._create_resource(self._model_class, **params)
+
+    def all(self, **params) -> Dict[str, Any]:
+        """Retrieve a list of Pickups."""
+        return self._all_resources(self._model_class, **params)
+
+    def retrieve(self, id: str) -> Pickup:
+        """Retrieve a Pickup."""
+        return self._retrieve_resource(self._model_class, id)
+
+    def get_next_page(
+        self,
+        pickups: Dict[str, Any],
+        page_size: int,
+        optional_params: Optional[Dict[str, Any]] = None,
+    ) -> Dict[str, Any]:
+        """Retrieve the next page of the list Pickup response."""
+        return self._get_next_page_resources(self._model_class, pickups, page_size, optional_params)
+
+    def buy(self, id: str, **params) -> Pickup:
+        """Buy a Pickup."""
+        url = f"{self._instance_url(self._model_class, id)}/buy"
+
+        response = Requestor(self._client).request(method=RequestMethod.POST, url=url, params=params)
+
+        return convert_to_easypost_object(response=response)
 
+    def cancel(self, id: str, **params) -> Pickup:
+        """Cancel a Pickup."""
+        url = f"{self._instance_url(self._model_class, id)}/cancel"
 
-class Pickup(CreateResource, AllResource):
-    def buy(self, **params) -> "Pickup":
-        """Buy a pickup."""
-        requestor = Requestor(local_api_key=self._api_key)
-        url = "%s/%s" % (self.instance_url(), "buy")
-        response, api_key = requestor.request(method=RequestMethod.POST, url=url, params=params)
-        self.refresh_from(values=response, api_key=api_key)
-        return self
-
-    def cancel(self, **params) -> "Pickup":
-        """Cancel a pickup."""
-        requestor = Requestor(local_api_key=self._api_key)
-        url = "%s/%s" % (self.instance_url(), "cancel")
-        response, api_key = requestor.request(method=RequestMethod.POST, url=url, params=params)
-        self.refresh_from(values=response, api_key=api_key)
-        return self
-
-    def lowest_rate(self, carriers: List[str] = None, services: List[str] = None):
-        """Get the lowest rate of this pickup."""
-        lowest_rate = get_lowest_object_rate(self, carriers, services, "pickup_rates")
+        response = Requestor(self._client).request(method=RequestMethod.POST, url=url, params=params)
 
-        return lowest_rate
+        return convert_to_easypost_object(response=response)
```

### Comparing `easypost-7.9.0/easypost/referral.py` & `easypost-8.0.0/easypost/services/shipment_service.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,179 +1,147 @@
 from typing import (
     Any,
     Dict,
     List,
     Optional,
 )
 
-import requests
-
 from easypost.easypost_object import convert_to_easypost_object
-from easypost.error import Error
+from easypost.models import (
+    Rate,
+    Shipment,
+)
 from easypost.requestor import (
     RequestMethod,
     Requestor,
 )
+from easypost.services.base_service import BaseService
+from easypost.util import get_lowest_smart_rate
 
 
-# TODO: Rename `Referral` to `ReferralCustomer` and have the module name match as well
-class Referral:
-    @staticmethod
-    def create(
-        api_key: Optional[str] = None,
-        **params,
-    ) -> Dict[str, Any]:
-        """Create a referral user.
-
-        This function requires the Partner User's API key.
-        """
-        requestor = Requestor(local_api_key=api_key)
-        new_params = {"user": params}
-        response, api_key = requestor.request(
-            method=RequestMethod.POST,
-            url="/referral_customers",
-            params=new_params,
-        )
-        return convert_to_easypost_object(response=response, api_key=api_key)
-
-    @staticmethod
-    def update_email(
-        email,
-        user_id,
-        api_key: Optional[str] = None,
-    ) -> bool:
-        """Update a referral user.
-
-        This function requires the Partner User's API key.
-        """
-        requestor = Requestor(local_api_key=api_key)
-        url = f"/referral_customers/{user_id}"
+class ShipmentService(BaseService):
+    def __init__(self, client):
+        self._client = client
+        self._model_class = Shipment.__name__
+
+    def create(self, with_carbon_offset: Optional[bool] = False, **params) -> Shipment:
+        """Create a Shipment."""
+        url = self._class_url(self._model_class)
         wrapped_params = {
-            "user": {
-                "email": email,
-            }
+            self._snakecase_name(self._model_class): params,
+            "carbon_offset": with_carbon_offset,
         }
-        _, _ = requestor.request(
-            method=RequestMethod.PUT,
-            url=url,
-            params=wrapped_params,
-        )
-
-        # Return true if succeeds, an error will be thrown if it fails
-        return True
-
-    @staticmethod
-    def all(
-        api_key: Optional[str] = None,
-        **params,
-    ) -> List:
-        """Retrieve a list of referral users.
 
-        This function requires the Partner User's API key.
-        """
-        requestor = Requestor(local_api_key=api_key)
-        response, api_key = requestor.request(
-            method=RequestMethod.GET,
-            url="/referral_customers",
-            params=params,
-        )
-        return convert_to_easypost_object(response=response, api_key=api_key)
-
-    @staticmethod
-    def add_credit_card(
-        referral_api_key: str,
-        number: str,
-        expiration_month: int,
-        expiration_year: int,
-        cvc: str,
-        primary_or_secondary: str = "primary",
-    ) -> Dict[str, Any]:
-        """Add credit card to a referral user.
+        response = Requestor(self._client).request(method=RequestMethod.POST, url=url, params=wrapped_params)
 
-        This function requires the Referral User's API key.
-        """
-        easypost_stripe_api_key = Referral._retrieve_easypost_stripe_api_key()
-
-        try:
-            stripe_token = Referral._create_stripe_token(
-                number,
-                expiration_month,
-                expiration_year,
-                cvc,
-                easypost_stripe_api_key,
-            )
-        except Exception:
-            raise Error(message="Could not send card details to Stripe, please try again later")
-
-        response = Referral._create_easypost_credit_card(
-            referral_api_key,
-            stripe_token.get("id", ""),
-            priority=primary_or_secondary,
-        )
-        return convert_to_easypost_object(response)
-
-    @staticmethod
-    def _retrieve_easypost_stripe_api_key() -> str:
-        """Retrieve EasyPost's Stripe public API key."""
-        requestor = Requestor()
-        public_key, _ = requestor.request(
-            method=RequestMethod.GET,
-            url="/partners/stripe_public_key",
-        )
-        return public_key.get("public_key", "")
-
-    @staticmethod
-    def _create_stripe_token(
-        number: str,
-        expiration_month: int,
-        expiration_year: int,
-        cvc: str,
-        easypost_stripe_key: str,
+        return convert_to_easypost_object(response=response)
+
+    def all(self, **params) -> Dict[str, Any]:
+        """Retrieve a list of Shipments."""
+        response = Requestor(self._client).request(method=RequestMethod.GET, url="/shipments", params=params)
+        response["include_children"] = params.get("include_children")
+        response["purchased"] = params.get("purchased")
+
+        return convert_to_easypost_object(response=response)
+
+    def retrieve(self, id: str) -> Shipment:
+        """Retrieve a Shipment."""
+        return self._retrieve_resource(self._model_class, id)
+
+    def get_next_page(
+        self,
+        shipments: Dict[str, Any],
+        page_size: int,
+        optional_params: Optional[Dict[str, Any]] = None,
     ) -> Dict[str, Any]:
-        """Get credit card token from Stripe."""
-        headers = {
-            # This Stripe endpoint only accepts URL form encoded bodies
-            "Content-type": "application/x-www-form-urlencoded",
+        """Get next page of shipment collection."""
+        optional_params = {
+            "include_children": shipments.get("include_children"),
+            "purchased": shipments.get("purchased"),
         }
 
-        credit_card_dict = {
-            "card": {
-                "number": number,
-                "exp_month": expiration_month,
-                "exp_year": expiration_year,
-                "cvc": cvc,
-            }
-        }
+        return self._get_next_page_resources(self._model_class, shipments, page_size, optional_params)
 
-        form_encoded_params = Requestor.form_encode_params(credit_card_dict)
-        url = "https://api.stripe.com/v1/tokens"
+    def regenerate_rates(self, id: str, with_carbon_offset: Optional[bool] = False) -> Shipment:
+        """Regenerate Rates for a Shipment."""
+        url = f"{self._instance_url(self._model_class, id)}/rerate"
+        wrapped_params = {"carbon_offset": with_carbon_offset}
 
-        stripe_response = requests.post(
-            url,
-            params=form_encoded_params,
-            headers=headers,
-            auth=requests.auth.HTTPBasicAuth(easypost_stripe_key, ""),
-        )
-        return stripe_response.json()
-
-    @staticmethod
-    def _create_easypost_credit_card(
-        referral_api_key: str,
-        stripe_object_id: str,
-        priority: str = "primary",
-    ) -> Dict[str, Any]:
-        """Submit Stripe credit card token to EasyPost."""
-        requestor = Requestor(local_api_key=referral_api_key)
+        response = Requestor(self._client).request(method=RequestMethod.POST, url=url, params=wrapped_params)
 
-        params = {
-            "credit_card": {
-                "stripe_object_id": stripe_object_id,
-                "priority": priority,
-            }
-        }
+        return convert_to_easypost_object(response=response)
+
+    def get_smart_rates(self, id: str) -> List[Rate]:
+        """Get SmartRates for a Shipment."""
+        url = f"{self._instance_url(self._model_class, id)}/smartrate"
+
+        response = Requestor(self._client).request(method=RequestMethod.GET, url=url)
+
+        return convert_to_easypost_object(response=response.get("result", []))
+
+    def buy(
+        self,
+        id: str,
+        with_carbon_offset: Optional[bool] = False,
+        end_shipper_id: Optional[str] = None,
+        **params,
+    ) -> Shipment:
+        """Buy a Shipment."""
+        url = f"{self._instance_url(self._model_class, id)}/buy"
+        params["carbon_offset"] = with_carbon_offset
+        if end_shipper_id:
+            params["end_shipper_id"] = end_shipper_id
+
+        response = Requestor(self._client).request(method=RequestMethod.POST, url=url, params=params)
+
+        return convert_to_easypost_object(response=response)
+
+    def refund(self, id: str, **params) -> Shipment:
+        """Refund a Shipment."""
+        url = f"{self._instance_url(self._model_class, id)}/refund"
+
+        response = Requestor(self._client).request(method=RequestMethod.POST, url=url, params=params)
+
+        return convert_to_easypost_object(response=response)
+
+    def insure(self, id: str, **params) -> Shipment:
+        """Insure a Shipment."""
+        url = f"{self._instance_url(self._model_class, id)}/insure"
+
+        response = Requestor(self._client).request(method=RequestMethod.POST, url=url, params=params)
+
+        return convert_to_easypost_object(response=response)
+
+    def label(self, id: str, **params) -> Shipment:
+        """Convert the label format of a Shipment."""
+        url = f"{self._instance_url(self._model_class, id)}/label"
+
+        response = Requestor(self._client).request(method=RequestMethod.GET, url=url, params=params)
+
+        return convert_to_easypost_object(response=response)
+
+    def lowest_smart_rate(self, id: str, delivery_days: int, delivery_accuracy: str) -> Rate:
+        """Get the lowest SmartRate of a Shipment."""
+        smartrates = self.get_smart_rates(id)
+        lowest_smart_rate = get_lowest_smart_rate(smartrates, delivery_days, delivery_accuracy.lower())
+
+        return lowest_smart_rate
+
+    def generate_form(self, id: str, form_type: str, form_options: Optional[Dict[str, Any]] = {}) -> Shipment:
+        """Generate a form for a Shipment."""
+        params = {"type": form_type}
+        params.update(form_options)  # type: ignore
+        wrapped_params = {"form": params}
+        url = f"{self._instance_url(self._model_class, id)}/forms"
+
+        response = Requestor(self._client).request(method=RequestMethod.POST, url=url, params=wrapped_params)
+
+        return convert_to_easypost_object(response=response)
+
+    def retrieve_estimated_delivery_date(self, id: str, planned_ship_date: str) -> List[Dict[str, Any]]:
+        """Retrieves the estimated delivery date of each Rate via SmartRate."""
+        url = f"{self._instance_url(self._model_class, id)}/smartrate/delivery_date"
+        wrapped_params = {"planned_ship_date": planned_ship_date}
+
+        response = Requestor(self._client).request(method=RequestMethod.GET, url=url, params=wrapped_params)
 
-        response, _ = requestor.request(
-            method=RequestMethod.POST,
-            params=params,
-            url="/credit_cards",
-        )
-        return response
+        return convert_to_easypost_object(response=response.get("rates", []))
```

### Comparing `easypost-7.9.0/easypost/requestor.py` & `easypost-8.0.0/easypost/requestor.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,127 +10,159 @@
     List,
     Optional,
     Tuple,
     Union,
 )
 from urllib.parse import urlencode
 
+import requests
+
 from easypost.constant import (
+    API_VERSION,
+    COMMUNICATION_ERROR,
+    INVALID_REQUEST_LIB_ERROR,
+    INVALID_REQUEST_METHOD_ERROR,
+    INVALID_REQUEST_PARAMETERS_ERROR,
+    INVALID_RESPONSE_BODY_ERROR,
     SUPPORT_EMAIL,
-    TIMEOUT,
+    TIMEOUT_ERROR,
+    VERSION,
 )
 from easypost.easypost_object import EasyPostObject
-from easypost.error import Error
+from easypost.errors import (
+    EasyPostError,
+    ForbiddenError,
+    GatewayTimeoutError,
+    HttpError,
+    InternalServerError,
+    InvalidRequestError,
+    JsonError,
+    MethodNotAllowedError,
+    NotFoundError,
+    PaymentError,
+    RateLimitError,
+    RedirectError,
+    ServiceUnavailableError,
+    TimeoutError,
+    UnauthorizedError,
+    UnknownApiError,
+)
+
+
+STATUS_CODE_TO_ERROR_MAPPING: Dict[int, Any] = {
+    401: UnauthorizedError,
+    402: PaymentError,
+    403: ForbiddenError,
+    404: NotFoundError,
+    405: MethodNotAllowedError,
+    408: TimeoutError,
+    422: InvalidRequestError,
+    429: RateLimitError,
+    500: InternalServerError,
+    503: ServiceUnavailableError,
+    504: GatewayTimeoutError,
+}
 
 
 class RequestMethod(Enum):
     GET = "get"
     POST = "post"
     PUT = "put"
     PATCH = "patch"
     DELETE = "delete"
 
 
 class Requestor:
-    def __init__(self, local_api_key: Optional[str] = None):
-        self._api_key = local_api_key
+    def __init__(self, client):
+        self._client = client
 
     @classmethod
     def _objects_to_ids(cls, param: Dict[str, Any]) -> Dict[str, Any]:
         """If providing an object as a parameter to another object,
-        only pass along the ID so the API will use the object reference correctly."""
+        only pass along the ID so the API will use the object reference correctly.
+        """
         if isinstance(param, EasyPostObject):
             return {"id": param.id}
         elif isinstance(param, dict):
             data = {}
-            for (k, v) in param.items():
+            for k, v in param.items():
                 if isinstance(v, list):
                     data[k] = [cls._objects_to_ids(item) for item in v]  # type: ignore
                 else:
                     data[k] = cls._objects_to_ids(v)  # type: ignore
             return data
         else:
             return param
 
     @staticmethod
-    def form_encode_params(data: Dict, parent_keys: List[str] = None, parent_dict: Dict = None) -> Dict:
+    def form_encode_params(
+        data: Dict[str, Any],
+        parent_keys: Optional[List[str]] = None,
+        parent_dict: Optional[Dict[str, Any]] = None,
+    ) -> Dict:
         """Form-encode a multi-layer dictionary to a one-layer dictionary."""
         result = parent_dict or {}
         keys = parent_keys or []
 
         for key, value in data.items():
             if isinstance(value, dict):
                 keys.append(key)
                 result = Requestor.form_encode_params(data=value, parent_keys=keys, parent_dict=result)
             else:
                 dict_key = Requestor._build_dict_key(keys + [key])
                 result[dict_key] = value
+
         return result
 
     @staticmethod
     def _build_dict_key(keys: List[str]) -> str:
         """Build a dict key from a list of keys.
         Example: [code, number] -> code[number]
         """
         result = keys[0]
 
         for key in keys[1:]:
             result += f"[{key}]"
+
         return result
 
     def request(
         self,
         method: RequestMethod,
         url: str,
         params: Optional[Dict[str, Any]] = None,
-        api_key_required: bool = True,
         beta: bool = False,
-    ) -> Tuple[dict, Optional[str]]:
+    ) -> Dict[str, Any]:
         """Make a request to the EasyPost API."""
         if params is None:
             params = {}
-        http_body, http_status, my_api_key = self.request_raw(
+
+        http_body, http_status = self.request_raw(
             method=method,
             url=url,
             params=params,
-            api_key_required=api_key_required,
             beta=beta,
         )
+
         response = self.interpret_response(http_body=http_body, http_status=http_status)
-        return response, my_api_key
+
+        return response
 
     def request_raw(
         self,
         method: RequestMethod,
         url: str,
         params: Optional[Dict[str, Any]] = None,
-        api_key_required: bool = True,
         beta: bool = False,
-    ) -> Tuple[str, int, Optional[str]]:
+    ) -> Tuple[str, int]:
         """Internal logic required to make a request to the EasyPost API."""
-        # Importing here to avoid circular imports
-        from easypost import (
-            VERSION,
-            api_base,
-            api_key,
-        )
-
-        my_api_key = self._api_key or api_key
-
-        if api_key_required and my_api_key is None:
-            raise Error(
-                "No API key provided. Set an API key via \"easypost.api_key = 'APIKEY'. "
-                "Your API keys can be found in your EasyPost dashboard, or you can email us "
-                f"at {SUPPORT_EMAIL} for assistance."
-            )
+        abs_url = f"{self._client.api_base}{url}"
 
         if beta:
-            abs_url = f"https://api.easypost.com/beta{url}"
-        else:
-            abs_url = f"{api_base}{url}"
+            abs_url = abs_url.replace(API_VERSION, "beta")
 
         params = self._objects_to_ids(param=params or {})
 
         # Fallback values for the user-agent header
         user_agent = {
             "client_version": VERSION,
             "implementation": "NA",
@@ -155,50 +187,51 @@
                 else:
                     user_agent[attr] = val  # type: ignore
             except Exception:  # nosec
                 # If we fail to get OS info, do nothing as we already set fallbacks for these values
                 pass
 
         user_agent = (
-            f"EasyPost/v2 PythonClient/{VERSION} Python/{user_agent['python_version']}"  # type: ignore
+            f"EasyPost/{API_VERSION} PythonClient/{VERSION} Python/{user_agent['python_version']}"  # type: ignore
             f" OS/{user_agent['os']} OSVersion/{user_agent['os_version']} OSArch/{user_agent['os_arch']}"
             f" Implementation/{user_agent['implementation']}"
         )
 
         headers = {
-            "Authorization": "Bearer %s" % my_api_key,
+            "Authorization": "Bearer %s" % self._client.api_key,
             "User-Agent": user_agent,
         }
 
-        if request_lib == "urlfetch":
+        if self._client._request_lib == "urlfetch":
             http_body, http_status = self.urlfetch_request(
                 method=method, abs_url=abs_url, headers=headers, params=params
             )
-        elif request_lib == "requests":
+        elif self._client._request_lib == "requests":
             http_body, http_status = self.requests_request(
                 method=method, abs_url=abs_url, headers=headers, params=params
             )
         else:
-            raise Error(f"Bug discovered: invalid request_lib: {request_lib}. Please report to {SUPPORT_EMAIL}.")
+            raise EasyPostError(INVALID_REQUEST_LIB_ERROR.format(self._client._request_lib, SUPPORT_EMAIL))
 
-        return http_body, http_status, my_api_key
+        return http_body, http_status
 
     def interpret_response(self, http_body: str, http_status: int) -> Dict[str, Any]:
         """Interpret the response body we receive from the API."""
         if http_status == 204:
             # HTTP 204 does not have any response body and we can just return here
             return {}
+
         try:
             response = json.loads(http_body)
         except JSONDecodeError:
-            raise Exception(
-                f"Unable to parse response body from API: {http_body}\nHTTP response code was: {http_status}"
-            )
-        if not (200 <= http_status < 300):
+            raise JsonError(INVALID_RESPONSE_BODY_ERROR.format(http_body, http_status))
+
+        if http_status < 200 or http_status >= 300:
             self.handle_api_error(http_status=http_status, http_body=http_body, response=response)
+
         return response
 
     def requests_request(
         self,
         method: RequestMethod,
         abs_url: str,
         headers: Dict[str, Any],
@@ -208,147 +241,116 @@
         if method in [RequestMethod.GET, RequestMethod.DELETE]:
             url_params = params
             body = None
         elif method in [RequestMethod.POST, RequestMethod.PATCH, RequestMethod.PUT]:
             url_params = None
             body = params
         else:
-            # how did you reach here with an enum?
-            raise Error(f"Bug discovered: invalid request method: {method}. Please report to {SUPPORT_EMAIL}.")
+            raise EasyPostError(INVALID_REQUEST_METHOD_ERROR.format(method, SUPPORT_EMAIL))
 
         if url_params and method not in [RequestMethod.GET, RequestMethod.DELETE]:
-            raise Error("Only GET and DELETE requests support parameters.")
+            raise EasyPostError(INVALID_REQUEST_PARAMETERS_ERROR)
 
         try:
-            result = requests_session.request(
+            result = self._client._requests_session.request(
                 method=method.value,
                 url=abs_url,
                 params=url_params,
                 headers=headers,
                 json=body,
-                timeout=timeout,
+                timeout=self._client.timeout,
                 verify=True,
             )
             http_body = result.text
             http_status = result.status_code
+        except requests.exceptions.Timeout:
+            raise TimeoutError(TIMEOUT_ERROR)
         except Exception as e:
-            raise Error(
-                "Unexpected error communicating with EasyPost. If this "
-                f"problem persists please let us know at {SUPPORT_EMAIL}.",
-                original_exception=e,
-            )
+            raise HttpError(COMMUNICATION_ERROR.format(SUPPORT_EMAIL, e))
+
         return http_body, http_status
 
     def urlfetch_request(
         self,
         method: RequestMethod,
         abs_url: str,
         headers: Dict[str, Any],
         params: Dict[str, Any],
     ) -> Tuple[str, int]:
         """Make a request by using the `urlfetch` library."""
-        fetch_args = {"method": method.value, "headers": headers, "validate_certificate": False, "deadline": timeout}
+        fetch_args = {
+            "method": method.value,
+            "headers": headers,
+            "validate_certificate": False,
+            "deadline": self._client.timeout,
+        }
+
         if method in [RequestMethod.GET, RequestMethod.DELETE]:
             # GET/DELETE requests use query params
             fetch_args["url"] = self.add_params_to_url(url=abs_url, params=params, method=method)
         elif method in [RequestMethod.POST, RequestMethod.PUT]:
             fetch_args["url"] = abs_url
             # POST/PUT requests use body params
             fetch_args["payload"] = json.dumps(params, default=self._utf8)
         else:
-            # how did you reach here with an enum?
-            raise Error(f"Bug discovered: invalid request method: {method}. Please report to {SUPPORT_EMAIL}.")
+            raise EasyPostError(INVALID_REQUEST_METHOD_ERROR.format(method, SUPPORT_EMAIL))
 
         try:
             from google.appengine.api import urlfetch  # type: ignore
 
             result = urlfetch.fetch(**fetch_args)  # type: ignore
         except Exception as e:
-            raise Error(
-                "Unexpected error communicating with EasyPost. "
-                f"If this problem persists, let us know at {SUPPORT_EMAIL}.",
-                original_exception=e,
-            )
+            raise HttpError(COMMUNICATION_ERROR.format(SUPPORT_EMAIL, e))
 
         return result.content, result.status_code
 
     def handle_api_error(self, http_status: int, http_body: str, response: Dict[str, Any]) -> None:
-        """Handles API errors returned from EasyPost."""
+        """Handles API errors returned from the EasyPost API."""
         try:
             error = response["error"]
         except (KeyError, TypeError):
-            raise Error("Invalid response from API: (%d) %r " % (http_status, http_body), http_status, http_body)
+            raise JsonError(
+                message=INVALID_RESPONSE_BODY_ERROR.format(http_status, http_body),
+                http_status=http_status,
+                http_body=http_body,
+            )
 
-        try:
-            raise Error(message=error.get("message", ""), http_status=http_status, http_body=http_body)
-        except AttributeError:
-            raise Error(message=error, http_status=http_status, http_body=http_body)
+        if http_status >= 300 and http_status < 400:
+            raise RedirectError(message=error, http_status=http_status, http_body=http_body)
+
+        error_type = STATUS_CODE_TO_ERROR_MAPPING.get(http_status, UnknownApiError)
+
+        raise error_type(message=error.get("message", ""), http_status=http_status, http_body=http_body)
 
     def _utf8(self, value: Union[str, bytes]) -> str:
         # Python3's str(bytestring) returns "b'bytestring'" so we use .decode instead
         if isinstance(value, bytes):
             return value.decode(encoding="utf-8")
         return value
 
     def encode_url_params(self, params: Dict[str, Any], method: RequestMethod) -> Union[str, None]:
         """Encode params for a URL."""
         if method not in [RequestMethod.GET, RequestMethod.DELETE]:
-            raise Error("Only GET and DELETE requests support parameters.")
+            raise EasyPostError(INVALID_REQUEST_PARAMETERS_ERROR)
+
         converted_params = []
+
         for key, value in sorted(params.items()):
             if value is None:
                 continue  # Don't add Nones to the query
             elif isinstance(value, datetime.datetime):
                 value = int(time.mktime(value.timetuple()))  # to UTC timestamp
             converted_params.append((key, value))
+
         return urlencode(query=converted_params)
 
     def add_params_to_url(self, url: str, params: Dict[str, Any], method: RequestMethod) -> str:
         """Add params to the URL."""
         if method not in [RequestMethod.GET, RequestMethod.DELETE]:
-            raise Error("Only GET and DELETE requests support parameters.")
+            raise EasyPostError(INVALID_REQUEST_PARAMETERS_ERROR)
+
         encoded_params = self.encode_url_params(params=params, method=method)
+
         if encoded_params:
             return "%s?%s" % (url, encoded_params)
-        return url
-
 
-# use urlfetch as request_lib on google app engine, otherwise use requests
-request_lib = None
-try:
-    from google.appengine.api import urlfetch
-
-    request_lib = "urlfetch"
-    # use the GAE application-wide "deadline" (or its default)
-    timeout = urlfetch.get_default_fetch_deadline() or TIMEOUT
-except ImportError:
-    timeout = TIMEOUT
-    try:
-        import requests
-
-        request_lib = "requests"
-        requests_session = requests.Session()
-        requests_http_adapter = requests.adapters.HTTPAdapter(max_retries=3)
-        requests_session.mount(prefix="https://api.easypost.com", adapter=requests_http_adapter)
-    except Exception:
-        raise ImportError(
-            "EasyPost requires an up to date requests library. "
-            'Update requests via "pip install -U requests" or '
-            f"contact us at {SUPPORT_EMAIL}."
-        )
-
-    try:
-        version = requests.__version__
-        major, minor, patch = [int(i) for i in version.split(".")]
-    except Exception:
-        raise ImportError(
-            "EasyPost requires an up to date requests library. "
-            'Update requests via "pip install -U requests" or contact '
-            f"us at {SUPPORT_EMAIL}."
-        )
-    else:
-        if major < 1:
-            raise ImportError(
-                "EasyPost requires an up to date requests library. Update "
-                'requests via "pip install -U requests" or contact us '
-                f"at {SUPPORT_EMAIL}."
-            )
+        return url
```

### Comparing `easypost-7.9.0/easypost/resource.py` & `easypost-8.0.0/easypost/services/base_service.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,104 +1,110 @@
 import re
 from typing import (
     Any,
+    Dict,
     List,
     Optional,
 )
 
-from easypost.easypost_object import (
-    EasyPostObject,
-    convert_to_easypost_object,
-)
-from easypost.error import Error
+from easypost.constant import NO_MORE_PAGES_ERROR
+from easypost.easypost_object import convert_to_easypost_object
+from easypost.errors import EndOfPaginationError
 from easypost.requestor import (
     RequestMethod,
     Requestor,
 )
 
 
-class Resource(EasyPostObject):
-    @classmethod
-    def retrieve(cls, easypost_id: str, api_key: Optional[str] = None, **params) -> object:
-        """Retrieve an object from the EasyPost API."""
-        instance = cls(easypost_id=easypost_id, api_key=api_key, **params)
-        instance.refresh()
-        return instance
-
-    def refresh(self) -> object:
-        """Refresh the local object from the API response."""
-        requestor = Requestor(local_api_key=self._api_key)
-        url = self.instance_url()
-        response, api_key = requestor.request(method=RequestMethod.GET, url=url, params=self._retrieve_params)
-        self.refresh_from(values=response, api_key=api_key)
-        return self
+class BaseService:
+    """The base service that all other services inherit containing shared logic."""
 
-    @classmethod
-    def snakecase_name(cls) -> str:
+    def __init__(self, client):
+        self._client = client
+
+    def _snakecase_name(self, class_name: str) -> str:
         """Return the class name as snake_case."""
-        snake_name = (cls.__name__[0:1] + re.sub(r"([A-Z])", r"_\1", cls.__name__[1:])).lower()
-        return snake_name
+        return re.sub(r"(?<!^)(?=[A-Z])", "_", class_name).lower()
 
-    @classmethod
-    def class_url(cls) -> str:
+    def _class_url(self, class_name: str) -> str:
         """Generate a URL based on class name."""
-        cls_name = cls.snakecase_name()
-        if cls_name[-1:] in ("s", "h"):
-            return "/%ses" % cls_name
+        transformed_class_name = self._snakecase_name(class_name)
+        if transformed_class_name[-1:] in ("s", "h"):
+            return f"/{transformed_class_name}es"
         else:
-            return "/%ss" % cls_name
+            return f"/{transformed_class_name}s"
+
+    def _instance_url(self, class_name: str, id: str) -> str:
+        """Generate an instance URL based on a class name and ID."""
+        return f"{self._class_url(class_name)}/{id}"
+
+    def _create_resource(self, class_name: str, **params) -> Any:
+        """Create an EasyPost object via the EasyPost API."""
+        url = self._class_url(class_name)
+        wrapped_params = {self._snakecase_name(class_name): params}
+
+        response = Requestor(self._client).request(method=RequestMethod.POST, url=url, params=wrapped_params)
+
+        return convert_to_easypost_object(response=response)
+
+    def _all_resources(self, class_name: str, **params) -> Any:
+        """Retrieve a list of EasyPostObjects from the EasyPost API."""
+        url = self._class_url(class_name)
+
+        response = Requestor(self._client).request(method=RequestMethod.GET, url=url, params=params)
+
+        return convert_to_easypost_object(response=response)
+
+    def _retrieve_resource(self, class_name: str, id: str) -> Any:
+        """Retrieve an object from the EasyPost API."""
+        url = self._instance_url(class_name, id)
+
+        response = Requestor(self._client).request(method=RequestMethod.GET, url=url)
+
+        return convert_to_easypost_object(response=response)
+
+    def _update_resource(self, class_name: str, id: str, method: RequestMethod = RequestMethod.PATCH, **params) -> Any:
+        """Update an EasyPost object via the EasyPost API."""
+        url = self._instance_url(class_name, id)
+        wrapped_params = {self._snakecase_name(class_name): params}
+
+        response = Requestor(self._client).request(method=method, url=url, params=wrapped_params)
+
+        return convert_to_easypost_object(response=response)
+
+    def _delete_resource(self, class_name: str, id: str) -> Any:
+        """Delete an EasyPost object via the EasyPost API."""
+        url = self._instance_url(class_name, id)
+
+        response = Requestor(self._client).request(method=RequestMethod.DELETE, url=url)
+
+        return convert_to_easypost_object(response=response)
+
+    def _get_next_page_resources(
+        self,
+        class_name: str,
+        collection: Dict[str, Any],
+        page_size: int,
+        optional_params: Optional[Dict[str, Any]] = None,
+    ) -> Dict[str, Any]:
+        """Retrieve next page of EasyPostObjects via the EasyPost API."""
+        url = self._class_url(class_name)
+        collection_array = collection.get(url[1:])
+
+        if collection_array is None or len(collection_array) == 0 or not collection.get("has_more"):
+            raise EndOfPaginationError(NO_MORE_PAGES_ERROR)
+
+        params = {
+            "before_id": collection_array[-1].id,
+            "page_size": page_size,
+        }
+
+        if optional_params:
+            params.update(optional_params)
+
+        response = Requestor(self._client).request(method=RequestMethod.GET, url=url, params=params)
+
+        response_array: List[Any] = response.get(url[1:])  # type: ignore
+        if response is None or len(response_array) == 0 or not response.get("has_more"):
+            raise EndOfPaginationError(NO_MORE_PAGES_ERROR)
 
-    def instance_url(self) -> str:
-        """Generate an instance URL based on the ID of the object."""
-        easypost_id = self.get("id")
-        if not easypost_id:
-            raise Error("%s instance has invalid ID: %r" % (type(self).__name__, easypost_id))
-        return "%s/%s" % (self.class_url(), easypost_id)
-
-
-class AllResource(Resource):
-    @classmethod
-    def all(cls, api_key: Optional[str] = None, **params) -> List[Any]:
-        """Retrieve a list of records from the API."""
-        requestor = Requestor(local_api_key=api_key)
-        url = cls.class_url()
-        response, api_key = requestor.request(method=RequestMethod.GET, url=url, params=params)
-        return convert_to_easypost_object(response=response, api_key=api_key)
-
-
-class CreateResource(Resource):
-    @classmethod
-    def create(cls, api_key: Optional[str] = None, **params) -> Any:
-        """Create an EasyPost object."""
-        requestor = Requestor(local_api_key=api_key)
-        url = cls.class_url()
-        wrapped_params = {cls.snakecase_name(): params}
-        response, api_key = requestor.request(method=RequestMethod.POST, url=url, params=wrapped_params)
-        return convert_to_easypost_object(response=response, api_key=api_key)
-
-
-class UpdateResource(Resource):
-    def save(self) -> Any:
-        """Update an EasyPost object."""
-        if self._unsaved_values:
-            requestor = Requestor(local_api_key=self._api_key)
-            params = {}
-            for k in self._unsaved_values:
-                params[k] = getattr(self, k)
-                if type(params[k]) is EasyPostObject:
-                    params[k] = params[k].flatten_unsaved()
-            params = {self.snakecase_name(): params}
-            url = self.instance_url()
-            response, api_key = requestor.request(method=RequestMethod.PATCH, url=url, params=params)
-            self.refresh_from(values=response, api_key=api_key)
-
-        return self
-
-
-class DeleteResource(Resource):
-    def delete(self, **params) -> Any:
-        """Delete an EasyPost object."""
-        requestor = Requestor(local_api_key=self._api_key)
-        url = self.instance_url()
-        response, api_key = requestor.request(method=RequestMethod.DELETE, url=url, params=params)
-        self.refresh_from(values=response, api_key=api_key)
-        return self
+        return convert_to_easypost_object(response=response)
```

### Comparing `easypost-7.9.0/easypost.egg-info/PKG-INFO` & `easypost-8.0.0/easypost.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: easypost
-Version: 7.9.0
+Version: 8.0.0
 Summary: EasyPost Shipping API Client Library for Python
 Home-page: https://easypost.com/
 Author: EasyPost
 Author-email: support@easypost.com
 Project-URL: Docs, https://www.easypost.com/docs/api
 Project-URL: Tracker, https://github.com/EasyPost/easypost-python/issues
 Project-URL: Source, https://github.com/EasyPost/easypost-python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.6, <4
+Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # EasyPost Python Client Library
 
 [![CI](https://github.com/EasyPost/easypost-python/workflows/CI/badge.svg)](https://github.com/EasyPost/easypost-python/actions?query=workflow%3ACI)
@@ -51,17 +50,17 @@
 
 A simple create & buy shipment example:
 
 ```python
 import os
 import easypost
 
-easypost.api_key = os.getenv('EASYPOST_API_KEY')
+client = easypost.EasyPostClient(os.getenv('EASYPOST_API_KEY'))
 
-shipment = easypost.Shipment.create(
+shipment = client.shipment.create(
     from_address = {
         "name": "EasyPost",
         "street1": "118 2nd Street",
         "street2": "4th Floor",
         "city": "San Francisco",
         "state": "CA",
         "zip": "94105",
@@ -81,25 +80,33 @@
         "length": 10.2,
         "width": 7.8,
         "height": 4.3,
         "weight": 21.2,
     },
 )
 
-shipment.buy(rate=shipment.lowest_rate())
+bought_shipment = client.shipment.buy(shipment.id, rate=shipment.lowest_rate())
 
-print(shipment)
+print(bought_shipment)
 ```
 
 ## Documentation
 
-API Documentation can be found at: <https://easypost.com/docs/api>.
+API documentation can be found at: <https://easypost.com/docs/api>.
+
+Library documentation can be found on the web at: <https://easypost.github.io/easypost-python/> or by building them locally via the `make docs` command.
 
 Upgrading major versions of this project? Refer to the [Upgrade Guide](UPGRADE_GUIDE.md).
 
+## Support
+
+New features and bug fixes are released on the latest major release of this library. If you are on an older major release of this library, we recommend upgrading to the most recent release to take advantage of new features, bug fixes, and security patches. Older versions of this library will continue to work and be available as long as the API version they are tied to remains active; however, they will not receive updates and are considered EOL.
+
+For additional support, see our [org-wide support policy](https://github.com/EasyPost/.github/blob/main/SUPPORT.md).
+
 ## Development
 
 ```bash
 # Install dependencies
 make install
 
 # Lint project
@@ -143,7 +150,18 @@
 - `EASYPOST_PROD_API_KEY`
 
 Some tests may require an EasyPost user with a particular set of enabled features such as a `Partner` user when creating referrals. We have attempted to call out these functions in their respective docstrings. The following are required when you need to re-record cassettes for applicable tests:
 
 - `USPS_CARRIER_ACCOUNT_ID` (eg: one-call buying a shipment for non-EasyPost employees)
 - `PARTNER_USER_PROD_API_KEY` (eg: creating a referral user)
 - `REFERRAL_CUSTOMER_PROD_API_KEY` (eg: adding a credit card to a referral user)
+
+#### Google Cloud SDK
+
+To run the test suite with the Google Cloud SDK (`urlfetch` instead of the `requests` library), you'll need the following:
+
+1. Install the appengine Python package to this virtual environment: `venv/bin/pip install appengine-python-standard`
+1. Install the Google Cloud SDK
+   - [Direct Download](https://cloud.google.com/sdk/docs/install)
+   - [Homebrew](https://formulae.brew.sh/cask/google-cloud-sdk)
+1. Point the `PYTHONPATH` environment variable to the path of the newly installed `google-cloud-sdk` directory. For Homebrew, this is `"$(brew --prefix)/share/google-cloud-sdk"`
+1. Run the test suite with the commands listed in this README
```

