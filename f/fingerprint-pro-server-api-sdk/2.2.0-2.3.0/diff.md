# Comparing `tmp/fingerprint-pro-server-api-sdk-2.2.0.tar.gz` & `tmp/fingerprint-pro-server-api-sdk-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fingerprint-pro-server-api-sdk-2.2.0.tar", last modified: Tue May 16 13:49:15 2023, max compression
+gzip compressed data, was "fingerprint-pro-server-api-sdk-2.3.0.tar", last modified: Tue Jun  6 11:30:33 2023, max compression
```

## Comparing `fingerprint-pro-server-api-sdk-2.2.0.tar` & `fingerprint-pro-server-api-sdk-2.3.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:49:15.753661 fingerprint-pro-server-api-sdk-2.2.0/
--rw-r--r--   0 root         (0) root         (0)     1069 2023-05-16 13:48:47.000000 fingerprint-pro-server-api-sdk-2.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    14727 2023-05-16 13:49:15.753661 fingerprint-pro-server-api-sdk-2.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9145 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:49:15.737661 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/
--rw-r--r--   0 root         (0) root         (0)     5486 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:49:15.741661 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/api/
--rw-r--r--   0 root         (0) root         (0)      165 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11598 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/api/fingerprint_api.py
--rw-r--r--   0 root         (0) root         (0)    25588 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/api_client.py
--rw-r--r--   0 root         (0) root         (0)     8894 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/configuration.py
--rw-r--r--   0 root         (0) root         (0)      362 2023-05-16 13:48:47.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/extend_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:49:15.753661 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/
--rw-r--r--   0 root         (0) root         (0)     5224 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4885 2023-05-16 13:49:10.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/botd_detection_result.py
--rw-r--r--   0 root         (0) root         (0)     7320 2023-05-16 13:49:10.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/botd_result.py
--rw-r--r--   0 root         (0) root         (0)     9277 2023-05-16 13:49:10.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/browser_details.py
--rw-r--r--   0 root         (0) root         (0)     3642 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/confidence.py
--rw-r--r--   0 root         (0) root         (0)     3428 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/error_event403_response.py
--rw-r--r--   0 root         (0) root         (0)     5134 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/error_event403_response_error.py
--rw-r--r--   0 root         (0) root         (0)     3428 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/error_event404_response.py
--rw-r--r--   0 root         (0) root         (0)     4705 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/error_event404_response_error.py
--rw-r--r--   0 root         (0) root         (0)     3448 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/error_visits403.py
--rw-r--r--   0 root         (0) root         (0)     3386 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/event_response.py
--rw-r--r--   0 root         (0) root         (0)     4776 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/identification_error.py
--rw-r--r--   0 root         (0) root         (0)     4356 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/ip_block_list_result.py
--rw-r--r--   0 root         (0) root         (0)     4615 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/ip_block_list_result_details.py
--rw-r--r--   0 root         (0) root         (0)     3821 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/ip_info_result.py
--rw-r--r--   0 root         (0) root         (0)     4082 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/ip_info_result_v4.py
--rw-r--r--   0 root         (0) root         (0)     4082 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/ip_info_result_v6.py
--rw-r--r--   0 root         (0) root         (0)     9377 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/ip_location.py
--rw-r--r--   0 root         (0) root         (0)     3276 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/ip_location_city.py
--rw-r--r--   0 root         (0) root         (0)     3949 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/location.py
--rw-r--r--   0 root         (0) root         (0)     3781 2023-05-16 13:48:47.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/many_requests_response.py
--rw-r--r--   0 root         (0) root         (0)     4667 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/product_error.py
--rw-r--r--   0 root         (0) root         (0)    10616 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/products_response.py
--rw-r--r--   0 root         (0) root         (0)     4007 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/products_response_botd.py
--rw-r--r--   0 root         (0) root         (0)     4230 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/products_response_identification.py
--rw-r--r--   0 root         (0) root         (0)    16816 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/products_response_identification_data.py
--rw-r--r--   0 root         (0) root         (0)     6501 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/response.py
--rw-r--r--   0 root         (0) root         (0)    14805 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/response_visits.py
--rw-r--r--   0 root         (0) root         (0)     3929 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/seen_at.py
--rw-r--r--   0 root         (0) root         (0)     4081 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/signal_response_emulator.py
--rw-r--r--   0 root         (0) root         (0)     4051 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/signal_response_emulator_data.py
--rw-r--r--   0 root         (0) root         (0)     4097 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/signal_response_incognito.py
--rw-r--r--   0 root         (0) root         (0)     3636 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/signal_response_incognito_data.py
--rw-r--r--   0 root         (0) root         (0)     4093 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/signal_response_ip_blocklist.py
--rw-r--r--   0 root         (0) root         (0)     4013 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/signal_response_ip_info.py
--rw-r--r--   0 root         (0) root         (0)     4033 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/signal_response_proxy.py
--rw-r--r--   0 root         (0) root         (0)     3622 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/signal_response_proxy_data.py
--rw-r--r--   0 root         (0) root         (0)     4081 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/signal_response_root_apps.py
--rw-r--r--   0 root         (0) root         (0)     4029 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/signal_response_root_apps_data.py
--rw-r--r--   0 root         (0) root         (0)     4061 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/signal_response_tampering.py
--rw-r--r--   0 root         (0) root         (0)     4001 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/signal_response_tor.py
--rw-r--r--   0 root         (0) root         (0)     3584 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/signal_response_tor_data.py
--rw-r--r--   0 root         (0) root         (0)     3965 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/signal_response_vpn.py
--rw-r--r--   0 root         (0) root         (0)     3901 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/subdivision.py
--rw-r--r--   0 root         (0) root         (0)     4748 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/tampering_result.py
--rw-r--r--   0 root         (0) root         (0)    14174 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/visit.py
--rw-r--r--   0 root         (0) root         (0)     4128 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/vpn_result.py
--rw-r--r--   0 root         (0) root         (0)     4691 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/vpn_result_methods.py
--rw-r--r--   0 root         (0) root         (0)     4078 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/webhook_signal_response_emulator.py
--rw-r--r--   0 root         (0) root         (0)     3649 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/webhook_signal_response_proxy.py
--rw-r--r--   0 root         (0) root         (0)     4056 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/webhook_signal_response_root_apps.py
--rw-r--r--   0 root         (0) root         (0)     3611 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/webhook_signal_response_tor.py
--rw-r--r--   0 root         (0) root         (0)    22987 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/webhook_visit.py
--rw-r--r--   0 root         (0) root         (0)    13535 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:49:15.741661 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)    14727 2023-05-16 13:49:15.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3968 2023-05-16 13:49:15.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 13:49:15.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2023-05-16 13:49:15.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       36 2023-05-16 13:49:15.000000 fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      473 2023-05-16 13:49:15.753661 fingerprint-pro-server-api-sdk-2.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3054 2023-05-16 13:49:11.000000 fingerprint-pro-server-api-sdk-2.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 13:49:15.753661 fingerprint-pro-server-api-sdk-2.2.0/test/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 13:48:47.000000 fingerprint-pro-server-api-sdk-2.2.0/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16976 2023-05-16 13:49:13.000000 fingerprint-pro-server-api-sdk-2.2.0/test/test_fingerprint_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 11:30:33.291185 fingerprint-pro-server-api-sdk-2.3.0/
+-rw-r--r--   0 root         (0) root         (0)     1069 2023-06-06 11:30:09.000000 fingerprint-pro-server-api-sdk-2.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    15007 2023-06-06 11:30:33.291185 fingerprint-pro-server-api-sdk-2.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9280 2023-06-06 11:30:30.000000 fingerprint-pro-server-api-sdk-2.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 11:30:33.279185 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/
+-rw-r--r--   0 root         (0) root         (0)     5621 2023-06-06 11:30:30.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 11:30:33.283185 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/api/
+-rw-r--r--   0 root         (0) root         (0)      165 2023-06-06 11:30:30.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16939 2023-06-06 11:30:30.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/api/fingerprint_api.py
+-rw-r--r--   0 root         (0) root         (0)    25723 2023-06-06 11:30:30.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/api_client.py
+-rw-r--r--   0 root         (0) root         (0)     9029 2023-06-06 11:30:30.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/configuration.py
+-rw-r--r--   0 root         (0) root         (0)      362 2023-06-06 11:30:09.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/extend_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 11:30:33.291185 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/
+-rw-r--r--   0 root         (0) root         (0)     5359 2023-06-06 11:30:30.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5020 2023-06-06 11:30:29.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/botd_detection_result.py
+-rw-r--r--   0 root         (0) root         (0)     7455 2023-06-06 11:30:29.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/botd_result.py
+-rw-r--r--   0 root         (0) root         (0)     9412 2023-06-06 11:30:29.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/browser_details.py
+-rw-r--r--   0 root         (0) root         (0)     3777 2023-06-06 11:30:29.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/confidence.py
+-rw-r--r--   0 root         (0) root         (0)     3563 2023-06-06 11:30:29.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/error_event403_response.py
+-rw-r--r--   0 root         (0) root         (0)     5269 2023-06-06 11:30:29.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/error_event403_response_error.py
+-rw-r--r--   0 root         (0) root         (0)     3563 2023-06-06 11:30:29.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/error_event404_response.py
+-rw-r--r--   0 root         (0) root         (0)     4840 2023-06-06 11:30:29.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/error_event404_response_error.py
+-rw-r--r--   0 root         (0) root         (0)     3583 2023-06-06 11:30:29.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/error_visits403.py
+-rw-r--r--   0 root         (0) root         (0)     3521 2023-06-06 11:30:29.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/event_response.py
+-rw-r--r--   0 root         (0) root         (0)     4911 2023-06-06 11:30:29.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/identification_error.py
+-rw-r--r--   0 root         (0) root         (0)     4491 2023-06-06 11:30:29.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/ip_block_list_result.py
+-rw-r--r--   0 root         (0) root         (0)     4750 2023-06-06 11:30:29.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/ip_block_list_result_details.py
+-rw-r--r--   0 root         (0) root         (0)     3956 2023-06-06 11:30:29.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/ip_info_result.py
+-rw-r--r--   0 root         (0) root         (0)     4217 2023-06-06 11:30:29.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/ip_info_result_v4.py
+-rw-r--r--   0 root         (0) root         (0)     4217 2023-06-06 11:30:29.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/ip_info_result_v6.py
+-rw-r--r--   0 root         (0) root         (0)     8982 2023-06-06 11:30:29.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/ip_location.py
+-rw-r--r--   0 root         (0) root         (0)     3411 2023-06-06 11:30:29.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/ip_location_city.py
+-rw-r--r--   0 root         (0) root         (0)     4084 2023-06-06 11:30:29.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/location.py
+-rw-r--r--   0 root         (0) root         (0)     3781 2023-06-06 11:30:09.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/many_requests_response.py
+-rw-r--r--   0 root         (0) root         (0)     4802 2023-06-06 11:30:29.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/product_error.py
+-rw-r--r--   0 root         (0) root         (0)    10751 2023-06-06 11:30:29.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/products_response.py
+-rw-r--r--   0 root         (0) root         (0)     4142 2023-06-06 11:30:29.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/products_response_botd.py
+-rw-r--r--   0 root         (0) root         (0)     4365 2023-06-06 11:30:29.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/products_response_identification.py
+-rw-r--r--   0 root         (0) root         (0)    16861 2023-06-06 11:30:29.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/products_response_identification_data.py
+-rw-r--r--   0 root         (0) root         (0)     6510 2023-06-06 11:30:29.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/response.py
+-rw-r--r--   0 root         (0) root         (0)    14850 2023-06-06 11:30:29.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/response_visits.py
+-rw-r--r--   0 root         (0) root         (0)     4064 2023-06-06 11:30:29.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/seen_at.py
+-rw-r--r--   0 root         (0) root         (0)     4216 2023-06-06 11:30:29.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/signal_response_emulator.py
+-rw-r--r--   0 root         (0) root         (0)     4186 2023-06-06 11:30:29.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/signal_response_emulator_data.py
+-rw-r--r--   0 root         (0) root         (0)     4232 2023-06-06 11:30:30.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/signal_response_incognito.py
+-rw-r--r--   0 root         (0) root         (0)     3771 2023-06-06 11:30:30.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/signal_response_incognito_data.py
+-rw-r--r--   0 root         (0) root         (0)     4228 2023-06-06 11:30:30.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/signal_response_ip_blocklist.py
+-rw-r--r--   0 root         (0) root         (0)     4148 2023-06-06 11:30:30.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/signal_response_ip_info.py
+-rw-r--r--   0 root         (0) root         (0)     4168 2023-06-06 11:30:30.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/signal_response_proxy.py
+-rw-r--r--   0 root         (0) root         (0)     3757 2023-06-06 11:30:30.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/signal_response_proxy_data.py
+-rw-r--r--   0 root         (0) root         (0)     4216 2023-06-06 11:30:30.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/signal_response_root_apps.py
+-rw-r--r--   0 root         (0) root         (0)     4164 2023-06-06 11:30:30.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/signal_response_root_apps_data.py
+-rw-r--r--   0 root         (0) root         (0)     4196 2023-06-06 11:30:30.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/signal_response_tampering.py
+-rw-r--r--   0 root         (0) root         (0)     4136 2023-06-06 11:30:30.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/signal_response_tor.py
+-rw-r--r--   0 root         (0) root         (0)     3719 2023-06-06 11:30:30.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/signal_response_tor_data.py
+-rw-r--r--   0 root         (0) root         (0)     4100 2023-06-06 11:30:30.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/signal_response_vpn.py
+-rw-r--r--   0 root         (0) root         (0)     4036 2023-06-06 11:30:30.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/subdivision.py
+-rw-r--r--   0 root         (0) root         (0)     4883 2023-06-06 11:30:30.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/tampering_result.py
+-rw-r--r--   0 root         (0) root         (0)    14219 2023-06-06 11:30:30.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/visit.py
+-rw-r--r--   0 root         (0) root         (0)     4263 2023-06-06 11:30:30.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/vpn_result.py
+-rw-r--r--   0 root         (0) root         (0)     4826 2023-06-06 11:30:30.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/vpn_result_methods.py
+-rw-r--r--   0 root         (0) root         (0)     4213 2023-06-06 11:30:30.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/webhook_signal_response_emulator.py
+-rw-r--r--   0 root         (0) root         (0)     3784 2023-06-06 11:30:30.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/webhook_signal_response_proxy.py
+-rw-r--r--   0 root         (0) root         (0)     4191 2023-06-06 11:30:30.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/webhook_signal_response_root_apps.py
+-rw-r--r--   0 root         (0) root         (0)     3746 2023-06-06 11:30:30.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/webhook_signal_response_tor.py
+-rw-r--r--   0 root         (0) root         (0)    23032 2023-06-06 11:30:30.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/webhook_visit.py
+-rw-r--r--   0 root         (0) root         (0)    13670 2023-06-06 11:30:30.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 11:30:33.283185 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15007 2023-06-06 11:30:33.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3968 2023-06-06 11:30:33.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 11:30:33.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2023-06-06 11:30:33.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2023-06-06 11:30:33.000000 fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      473 2023-06-06 11:30:33.291185 fingerprint-pro-server-api-sdk-2.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3334 2023-06-06 11:30:30.000000 fingerprint-pro-server-api-sdk-2.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 11:30:33.291185 fingerprint-pro-server-api-sdk-2.3.0/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 11:30:09.000000 fingerprint-pro-server-api-sdk-2.3.0/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16976 2023-06-06 11:30:31.000000 fingerprint-pro-server-api-sdk-2.3.0/test/test_fingerprint_api.py
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/LICENSE` & `fingerprint-pro-server-api-sdk-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/PKG-INFO` & `fingerprint-pro-server-api-sdk-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: fingerprint-pro-server-api-sdk
-Version: 2.2.0
-Summary: Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.
+Version: 2.3.0
+Summary: Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it&#x27;s not intended to be used from the client side, whether it&#x27;s a browser or a mobile device. 
 Home-page: https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk
 Author: Fingerprint
 Author-email: support@fingerprint.com
 License: MIT
 Keywords: Swagger,Fingerprint Pro Server API,browser,detection,fingerprint,identification,fingerprinting,browser-fingerprinting,browser-fingerprint,fraud-detection,fraud,audio-fingerprinting,fingerprintjs,fingerprintjs-pro,visitor-identifier
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -52,20 +52,20 @@
   </a>
   <a href="https://discord.gg/39EpE2neBg">
     <img src="https://img.shields.io/discord/852099967190433792?style=logo&label=Discord&logo=Discord&logoColor=white" alt="Discord server">
   </a>
 </p>
 
 # Fingerprint Pro Server Python SDK
-Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.
+Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device. 
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
 - API version: 3
-- Package version: 2.2.0
+- Package version: 2.3.0
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
```

#### html2text {}

```diff
@@ -1,12 +1,14 @@
-Metadata-Version: 2.1 Name: fingerprint-pro-server-api-sdk Version: 2.2.0
+Metadata-Version: 2.1 Name: fingerprint-pro-server-api-sdk Version: 2.3.0
 Summary: Fingerprint Pro Server API allows you to get information about
-visitors and about individual events in a server environment. This API can be
-used for data exports, decision-making, and data analysis scenarios. Home-page:
-https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk Author:
+visitors and about individual events in a server environment. It can be used
+for data exports, decision-making, and data analysis scenarios. Server API is
+intended for server-side usage, it&#x27;s not intended to be used from the
+client side, whether it&#x27;s a browser or a mobile device. Home-page: https:/
+/github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk Author:
 Fingerprint Author-email: support@fingerprint.com License: MIT Keywords:
 Swagger,Fingerprint Pro Server
 API,browser,detection,fingerprint,identification,fingerprinting,browser-
 fingerprinting,browser-fingerprint,fraud-detection,fraud,audio-
 fingerprinting,fingerprintjs,fingerprintjs-pro,visitor-identifier Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
@@ -21,18 +23,20 @@
 :: Python Modules Classifier: Topic :: Security Description-Content-Type: text/
 markdown License-File: LICENSE
                               [Fingerprint_logo]
  [PyPI] [coverage] [CI_badge] [CI_badge] [CI_badge] [https://img.shields.io/:
                license-mit-blue.svg?style=flat] [Discord_server]
 # Fingerprint Pro Server Python SDK Fingerprint Pro Server API allows you to
 get information about visitors and about individual events in a server
-environment. This API can be used for data exports, decision-making, and data
-analysis scenarios. This Python package is automatically generated by the
-[Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project: -
-API version: 3 - Package version: 2.2.0 - Build package:
+environment. It can be used for data exports, decision-making, and data
+analysis scenarios. Server API is intended for server-side usage, it's not
+intended to be used from the client side, whether it's a browser or a mobile
+device. This Python package is automatically generated by the [Swagger Codegen]
+(https://github.com/swagger-api/swagger-codegen) project: - API version: 3 -
+Package version: 2.3.0 - Build package:
 io.swagger.codegen.v3.generators.python.PythonClientCodegen ## Requirements.
 Python 2.7 and 3.4+ ## Installation & Usage ### pip install You can install the
 package directly from the Github ```sh pip install git+https://github.com/
 fingerprintjs/fingerprint-pro-server-api-python-sdk.git ``` Or from the PyPI
 ```sh pip install fingerprint_pro_server_api_sdk ``` Then import the package:
 ```python import fingerprint_pro_server_api_sdk ``` ### Setuptools Install via
 [Setuptools](http://pypi.python.org/pypi/setuptools). ```sh python setup.py
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/README.md` & `fingerprint-pro-server-api-sdk-2.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -28,20 +28,20 @@
   </a>
   <a href="https://discord.gg/39EpE2neBg">
     <img src="https://img.shields.io/discord/852099967190433792?style=logo&label=Discord&logo=Discord&logoColor=white" alt="Discord server">
   </a>
 </p>
 
 # Fingerprint Pro Server Python SDK
-Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.
+Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device. 
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
 - API version: 3
-- Package version: 2.2.0
+- Package version: 2.3.0
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
```

#### html2text {}

```diff
@@ -1,16 +1,18 @@
                             ___[Fingerprint_logo]_
  [PyPI] [coverage] [CI_badge] [CI_badge] [CI_badge] [https://img.shields.io/:
                license-mit-blue.svg?style=flat] [Discord_server]
 # Fingerprint Pro Server Python SDK Fingerprint Pro Server API allows you to
 get information about visitors and about individual events in a server
-environment. This API can be used for data exports, decision-making, and data
-analysis scenarios. This Python package is automatically generated by the
-[Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project: -
-API version: 3 - Package version: 2.2.0 - Build package:
+environment. It can be used for data exports, decision-making, and data
+analysis scenarios. Server API is intended for server-side usage, it's not
+intended to be used from the client side, whether it's a browser or a mobile
+device. This Python package is automatically generated by the [Swagger Codegen]
+(https://github.com/swagger-api/swagger-codegen) project: - API version: 3 -
+Package version: 2.3.0 - Build package:
 io.swagger.codegen.v3.generators.python.PythonClientCodegen ## Requirements.
 Python 2.7 and 3.4+ ## Installation & Usage ### pip install You can install the
 package directly from the Github ```sh pip install git+https://github.com/
 fingerprintjs/fingerprint-pro-server-api-python-sdk.git ``` Or from the PyPI
 ```sh pip install fingerprint_pro_server_api_sdk ``` Then import the package:
 ```python import fingerprint_pro_server_api_sdk ``` ### Setuptools Install via
 [Setuptools](http://pypi.python.org/pypi/setuptools). ```sh python setup.py
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/__init__.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 # flake8: noqa
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/api_client.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 from __future__ import absolute_import
 
@@ -68,15 +68,15 @@
         self.pool = ThreadPool()
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Swagger-Codegen/2.2.0/python'
+        self.user_agent = 'Swagger-Codegen/2.3.0/python'
 
     def __del__(self):
         self.pool.close()
         self.pool.join()
 
     @property
     def user_agent(self):
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/configuration.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
@@ -259,9 +259,9 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 3\n"\
-               "SDK Package Version: 2.2.0".\
+               "SDK Package Version: 2.3.0".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/__init__.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 
 # flake8: noqa
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/botd_detection_result.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/botd_detection_result.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/botd_result.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/botd_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/browser_details.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/browser_details.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/confidence.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/confidence.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/error_event403_response.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/error_event403_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/error_event403_response_error.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/error_event404_response_error.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class ErrorEvent403ResponseError(object):
+class ErrorEvent404ResponseError(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -34,68 +34,68 @@
 
     attribute_map = {
         'code': 'code',
         'message': 'message'
     }
 
     def __init__(self, code=None, message=None):  # noqa: E501
-        """ErrorEvent403ResponseError - a model defined in Swagger"""  # noqa: E501
+        """ErrorEvent404ResponseError - a model defined in Swagger"""  # noqa: E501
         self._code = None
         self._message = None
         self.discriminator = None
         self.code = code
         self.message = message
 
     @property
     def code(self):
-        """Gets the code of this ErrorEvent403ResponseError.  # noqa: E501
+        """Gets the code of this ErrorEvent404ResponseError.  # noqa: E501
 
-        Error code:  * `TokenRequired` - `Auth-API-Key` header is missing or empty  * `TokenNotFound` - subscription not found for specified secret key  * `SubscriptionNotActive` - subscription is not active  * `WrongRegion` - server and subscription region differ   # noqa: E501
+        Error code:  * `RequestNotFound` - request not found for specified id   # noqa: E501
 
-        :return: The code of this ErrorEvent403ResponseError.  # noqa: E501
+        :return: The code of this ErrorEvent404ResponseError.  # noqa: E501
         :rtype: str
         """
         return self._code
 
     @code.setter
     def code(self, code):
-        """Sets the code of this ErrorEvent403ResponseError.
+        """Sets the code of this ErrorEvent404ResponseError.
 
-        Error code:  * `TokenRequired` - `Auth-API-Key` header is missing or empty  * `TokenNotFound` - subscription not found for specified secret key  * `SubscriptionNotActive` - subscription is not active  * `WrongRegion` - server and subscription region differ   # noqa: E501
+        Error code:  * `RequestNotFound` - request not found for specified id   # noqa: E501
 
-        :param code: The code of this ErrorEvent403ResponseError.  # noqa: E501
+        :param code: The code of this ErrorEvent404ResponseError.  # noqa: E501
         :type: str
         """
         if code is None:
             raise ValueError("Invalid value for `code`, must not be `None`")  # noqa: E501
-        allowed_values = ["TokenRequired", "TokenNotFound", "SubscriptionNotActive", "WrongRegion"]  # noqa: E501
+        allowed_values = ["RequestNotFound"]  # noqa: E501
         if (code not in allowed_values):
             raise ValueError(
                 "Invalid value for `code` ({0}), must be one of {1}"  # noqa: E501
                 .format(code, allowed_values)
             )
 
         self._code = code
 
     @property
     def message(self):
-        """Gets the message of this ErrorEvent403ResponseError.  # noqa: E501
+        """Gets the message of this ErrorEvent404ResponseError.  # noqa: E501
 
 
-        :return: The message of this ErrorEvent403ResponseError.  # noqa: E501
+        :return: The message of this ErrorEvent404ResponseError.  # noqa: E501
         :rtype: str
         """
         return self._message
 
     @message.setter
     def message(self, message):
-        """Sets the message of this ErrorEvent403ResponseError.
+        """Sets the message of this ErrorEvent404ResponseError.
 
 
-        :param message: The message of this ErrorEvent403ResponseError.  # noqa: E501
+        :param message: The message of this ErrorEvent404ResponseError.  # noqa: E501
         :type: str
         """
         if message is None:
             raise ValueError("Invalid value for `message`, must not be `None`")  # noqa: E501
 
         self._message = message
 
@@ -116,15 +116,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ErrorEvent403ResponseError, dict):
+        if issubclass(ErrorEvent404ResponseError, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -132,18 +132,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ErrorEvent403ResponseError):
+        if not isinstance(other, ErrorEvent404ResponseError):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, ErrorEvent403ResponseError):
+        if not isinstance(other, ErrorEvent404ResponseError):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/error_event404_response.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/error_event404_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/error_event404_response_error.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/identification_error.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class ErrorEvent404ResponseError(object):
+class IdentificationError(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -34,68 +34,68 @@
 
     attribute_map = {
         'code': 'code',
         'message': 'message'
     }
 
     def __init__(self, code=None, message=None):  # noqa: E501
-        """ErrorEvent404ResponseError - a model defined in Swagger"""  # noqa: E501
+        """IdentificationError - a model defined in Swagger"""  # noqa: E501
         self._code = None
         self._message = None
         self.discriminator = None
         self.code = code
         self.message = message
 
     @property
     def code(self):
-        """Gets the code of this ErrorEvent404ResponseError.  # noqa: E501
+        """Gets the code of this IdentificationError.  # noqa: E501
 
-        Error code:  * `RequestNotFound` - request not found for specified id   # noqa: E501
+        Error code:  * `429 Too Many Requests` - the limit on secret API key requests per second has been exceeded  * `Failed` - internal server error   # noqa: E501
 
-        :return: The code of this ErrorEvent404ResponseError.  # noqa: E501
+        :return: The code of this IdentificationError.  # noqa: E501
         :rtype: str
         """
         return self._code
 
     @code.setter
     def code(self, code):
-        """Sets the code of this ErrorEvent404ResponseError.
+        """Sets the code of this IdentificationError.
 
-        Error code:  * `RequestNotFound` - request not found for specified id   # noqa: E501
+        Error code:  * `429 Too Many Requests` - the limit on secret API key requests per second has been exceeded  * `Failed` - internal server error   # noqa: E501
 
-        :param code: The code of this ErrorEvent404ResponseError.  # noqa: E501
+        :param code: The code of this IdentificationError.  # noqa: E501
         :type: str
         """
         if code is None:
             raise ValueError("Invalid value for `code`, must not be `None`")  # noqa: E501
-        allowed_values = ["RequestNotFound"]  # noqa: E501
+        allowed_values = ["429 Too Many Requests", "Failed"]  # noqa: E501
         if (code not in allowed_values):
             raise ValueError(
                 "Invalid value for `code` ({0}), must be one of {1}"  # noqa: E501
                 .format(code, allowed_values)
             )
 
         self._code = code
 
     @property
     def message(self):
-        """Gets the message of this ErrorEvent404ResponseError.  # noqa: E501
+        """Gets the message of this IdentificationError.  # noqa: E501
 
 
-        :return: The message of this ErrorEvent404ResponseError.  # noqa: E501
+        :return: The message of this IdentificationError.  # noqa: E501
         :rtype: str
         """
         return self._message
 
     @message.setter
     def message(self, message):
-        """Sets the message of this ErrorEvent404ResponseError.
+        """Sets the message of this IdentificationError.
 
 
-        :param message: The message of this ErrorEvent404ResponseError.  # noqa: E501
+        :param message: The message of this IdentificationError.  # noqa: E501
         :type: str
         """
         if message is None:
             raise ValueError("Invalid value for `message`, must not be `None`")  # noqa: E501
 
         self._message = message
 
@@ -116,15 +116,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ErrorEvent404ResponseError, dict):
+        if issubclass(IdentificationError, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -132,18 +132,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ErrorEvent404ResponseError):
+        if not isinstance(other, IdentificationError):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, ErrorEvent404ResponseError):
+        if not isinstance(other, IdentificationError):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/error_visits403.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/error_visits403.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/event_response.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/event_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/identification_error.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/product_error.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class IdentificationError(object):
+class ProductError(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -34,68 +34,68 @@
 
     attribute_map = {
         'code': 'code',
         'message': 'message'
     }
 
     def __init__(self, code=None, message=None):  # noqa: E501
-        """IdentificationError - a model defined in Swagger"""  # noqa: E501
+        """ProductError - a model defined in Swagger"""  # noqa: E501
         self._code = None
         self._message = None
         self.discriminator = None
         self.code = code
         self.message = message
 
     @property
     def code(self):
-        """Gets the code of this IdentificationError.  # noqa: E501
+        """Gets the code of this ProductError.  # noqa: E501
 
-        Error code:  * `429 Too Many Requests` - the limit on secret API key requests per second has been exceeded  * `Failed` - internal server error   # noqa: E501
+        Error code:  * `TooManyRequests` - the limit on secret API key requests per second has been exceeded  * `Failed` - internal server error   # noqa: E501
 
-        :return: The code of this IdentificationError.  # noqa: E501
+        :return: The code of this ProductError.  # noqa: E501
         :rtype: str
         """
         return self._code
 
     @code.setter
     def code(self, code):
-        """Sets the code of this IdentificationError.
+        """Sets the code of this ProductError.
 
-        Error code:  * `429 Too Many Requests` - the limit on secret API key requests per second has been exceeded  * `Failed` - internal server error   # noqa: E501
+        Error code:  * `TooManyRequests` - the limit on secret API key requests per second has been exceeded  * `Failed` - internal server error   # noqa: E501
 
-        :param code: The code of this IdentificationError.  # noqa: E501
+        :param code: The code of this ProductError.  # noqa: E501
         :type: str
         """
         if code is None:
             raise ValueError("Invalid value for `code`, must not be `None`")  # noqa: E501
-        allowed_values = ["429 Too Many Requests", "Failed"]  # noqa: E501
+        allowed_values = ["TooManyRequests", "Failed"]  # noqa: E501
         if (code not in allowed_values):
             raise ValueError(
                 "Invalid value for `code` ({0}), must be one of {1}"  # noqa: E501
                 .format(code, allowed_values)
             )
 
         self._code = code
 
     @property
     def message(self):
-        """Gets the message of this IdentificationError.  # noqa: E501
+        """Gets the message of this ProductError.  # noqa: E501
 
 
-        :return: The message of this IdentificationError.  # noqa: E501
+        :return: The message of this ProductError.  # noqa: E501
         :rtype: str
         """
         return self._message
 
     @message.setter
     def message(self, message):
-        """Sets the message of this IdentificationError.
+        """Sets the message of this ProductError.
 
 
-        :param message: The message of this IdentificationError.  # noqa: E501
+        :param message: The message of this ProductError.  # noqa: E501
         :type: str
         """
         if message is None:
             raise ValueError("Invalid value for `message`, must not be `None`")  # noqa: E501
 
         self._message = message
 
@@ -116,15 +116,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(IdentificationError, dict):
+        if issubclass(ProductError, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -132,18 +132,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, IdentificationError):
+        if not isinstance(other, ProductError):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, IdentificationError):
+        if not isinstance(other, ProductError):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/ip_block_list_result.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/ip_block_list_result.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/ip_block_list_result_details.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/ip_block_list_result_details.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/ip_info_result.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/ip_info_result.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/ip_info_result_v4.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/ip_info_result_v4.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/ip_info_result_v6.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/ip_info_result_v6.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/ip_location.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/ip_location.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
@@ -59,24 +59,30 @@
         self._postal_code = None
         self._timezone = None
         self._city = None
         self._country = None
         self._continent = None
         self._subdivisions = None
         self.discriminator = None
-        self.accuracy_radius = accuracy_radius
-        self.latitude = latitude
-        self.longitude = longitude
+        if accuracy_radius is not None:
+            self.accuracy_radius = accuracy_radius
+        if latitude is not None:
+            self.latitude = latitude
+        if longitude is not None:
+            self.longitude = longitude
         if postal_code is not None:
             self.postal_code = postal_code
-        self.timezone = timezone
+        if timezone is not None:
+            self.timezone = timezone
         if city is not None:
             self.city = city
-        self.country = country
-        self.continent = continent
+        if country is not None:
+            self.country = country
+        if continent is not None:
+            self.continent = continent
         if subdivisions is not None:
             self.subdivisions = subdivisions
 
     @property
     def accuracy_radius(self):
         """Gets the accuracy_radius of this IPLocation.  # noqa: E501
 
@@ -90,16 +96,14 @@
     def accuracy_radius(self, accuracy_radius):
         """Sets the accuracy_radius of this IPLocation.
 
 
         :param accuracy_radius: The accuracy_radius of this IPLocation.  # noqa: E501
         :type: int
         """
-        if accuracy_radius is None:
-            raise ValueError("Invalid value for `accuracy_radius`, must not be `None`")  # noqa: E501
 
         self._accuracy_radius = accuracy_radius
 
     @property
     def latitude(self):
         """Gets the latitude of this IPLocation.  # noqa: E501
 
@@ -113,16 +117,14 @@
     def latitude(self, latitude):
         """Sets the latitude of this IPLocation.
 
 
         :param latitude: The latitude of this IPLocation.  # noqa: E501
         :type: float
         """
-        if latitude is None:
-            raise ValueError("Invalid value for `latitude`, must not be `None`")  # noqa: E501
 
         self._latitude = latitude
 
     @property
     def longitude(self):
         """Gets the longitude of this IPLocation.  # noqa: E501
 
@@ -136,16 +138,14 @@
     def longitude(self, longitude):
         """Sets the longitude of this IPLocation.
 
 
         :param longitude: The longitude of this IPLocation.  # noqa: E501
         :type: float
         """
-        if longitude is None:
-            raise ValueError("Invalid value for `longitude`, must not be `None`")  # noqa: E501
 
         self._longitude = longitude
 
     @property
     def postal_code(self):
         """Gets the postal_code of this IPLocation.  # noqa: E501
 
@@ -180,16 +180,14 @@
     def timezone(self, timezone):
         """Sets the timezone of this IPLocation.
 
 
         :param timezone: The timezone of this IPLocation.  # noqa: E501
         :type: str
         """
-        if timezone is None:
-            raise ValueError("Invalid value for `timezone`, must not be `None`")  # noqa: E501
 
         self._timezone = timezone
 
     @property
     def city(self):
         """Gets the city of this IPLocation.  # noqa: E501
 
@@ -224,16 +222,14 @@
     def country(self, country):
         """Sets the country of this IPLocation.
 
 
         :param country: The country of this IPLocation.  # noqa: E501
         :type: Location
         """
-        if country is None:
-            raise ValueError("Invalid value for `country`, must not be `None`")  # noqa: E501
 
         self._country = country
 
     @property
     def continent(self):
         """Gets the continent of this IPLocation.  # noqa: E501
 
@@ -247,16 +243,14 @@
     def continent(self, continent):
         """Sets the continent of this IPLocation.
 
 
         :param continent: The continent of this IPLocation.  # noqa: E501
         :type: Location
         """
-        if continent is None:
-            raise ValueError("Invalid value for `continent`, must not be `None`")  # noqa: E501
 
         self._continent = continent
 
     @property
     def subdivisions(self):
         """Gets the subdivisions of this IPLocation.  # noqa: E501
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/ip_location_city.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/ip_location_city.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/location.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/location.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/many_requests_response.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/many_requests_response.py`

 * *Files identical despite different names*

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/product_error.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/error_event403_response_error.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class ProductError(object):
+class ErrorEvent403ResponseError(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -34,68 +34,68 @@
 
     attribute_map = {
         'code': 'code',
         'message': 'message'
     }
 
     def __init__(self, code=None, message=None):  # noqa: E501
-        """ProductError - a model defined in Swagger"""  # noqa: E501
+        """ErrorEvent403ResponseError - a model defined in Swagger"""  # noqa: E501
         self._code = None
         self._message = None
         self.discriminator = None
         self.code = code
         self.message = message
 
     @property
     def code(self):
-        """Gets the code of this ProductError.  # noqa: E501
+        """Gets the code of this ErrorEvent403ResponseError.  # noqa: E501
 
-        Error code:  * `TooManyRequests` - the limit on secret API key requests per second has been exceeded  * `Failed` - internal server error   # noqa: E501
+        Error code:  * `TokenRequired` - `Auth-API-Key` header is missing or empty  * `TokenNotFound` - subscription not found for specified secret key  * `SubscriptionNotActive` - subscription is not active  * `WrongRegion` - server and subscription region differ   # noqa: E501
 
-        :return: The code of this ProductError.  # noqa: E501
+        :return: The code of this ErrorEvent403ResponseError.  # noqa: E501
         :rtype: str
         """
         return self._code
 
     @code.setter
     def code(self, code):
-        """Sets the code of this ProductError.
+        """Sets the code of this ErrorEvent403ResponseError.
 
-        Error code:  * `TooManyRequests` - the limit on secret API key requests per second has been exceeded  * `Failed` - internal server error   # noqa: E501
+        Error code:  * `TokenRequired` - `Auth-API-Key` header is missing or empty  * `TokenNotFound` - subscription not found for specified secret key  * `SubscriptionNotActive` - subscription is not active  * `WrongRegion` - server and subscription region differ   # noqa: E501
 
-        :param code: The code of this ProductError.  # noqa: E501
+        :param code: The code of this ErrorEvent403ResponseError.  # noqa: E501
         :type: str
         """
         if code is None:
             raise ValueError("Invalid value for `code`, must not be `None`")  # noqa: E501
-        allowed_values = ["TooManyRequests", "Failed"]  # noqa: E501
+        allowed_values = ["TokenRequired", "TokenNotFound", "SubscriptionNotActive", "WrongRegion"]  # noqa: E501
         if (code not in allowed_values):
             raise ValueError(
                 "Invalid value for `code` ({0}), must be one of {1}"  # noqa: E501
                 .format(code, allowed_values)
             )
 
         self._code = code
 
     @property
     def message(self):
-        """Gets the message of this ProductError.  # noqa: E501
+        """Gets the message of this ErrorEvent403ResponseError.  # noqa: E501
 
 
-        :return: The message of this ProductError.  # noqa: E501
+        :return: The message of this ErrorEvent403ResponseError.  # noqa: E501
         :rtype: str
         """
         return self._message
 
     @message.setter
     def message(self, message):
-        """Sets the message of this ProductError.
+        """Sets the message of this ErrorEvent403ResponseError.
 
 
-        :param message: The message of this ProductError.  # noqa: E501
+        :param message: The message of this ErrorEvent403ResponseError.  # noqa: E501
         :type: str
         """
         if message is None:
             raise ValueError("Invalid value for `message`, must not be `None`")  # noqa: E501
 
         self._message = message
 
@@ -116,15 +116,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ProductError, dict):
+        if issubclass(ErrorEvent403ResponseError, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -132,18 +132,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ProductError):
+        if not isinstance(other, ErrorEvent403ResponseError):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, ProductError):
+        if not isinstance(other, ErrorEvent403ResponseError):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/products_response.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/products_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/products_response_botd.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/products_response_botd.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/products_response_identification.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/products_response_identification.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/products_response_identification_data.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/products_response_identification_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
@@ -81,15 +81,16 @@
         self._last_seen_at = None
         self._visitor_id = None
         self.discriminator = None
         self.request_id = request_id
         self.browser_details = browser_details
         self.incognito = incognito
         self.ip = ip
-        self.ip_location = ip_location
+        if ip_location is not None:
+            self.ip_location = ip_location
         self.timestamp = timestamp
         self.time = time
         self.url = url
         if tag is not None:
             self.tag = tag
         if linked_id is not None:
             self.linked_id = linked_id
@@ -209,16 +210,14 @@
     def ip_location(self, ip_location):
         """Sets the ip_location of this ProductsResponseIdentificationData.
 
 
         :param ip_location: The ip_location of this ProductsResponseIdentificationData.  # noqa: E501
         :type: IPLocation
         """
-        if ip_location is None:
-            raise ValueError("Invalid value for `ip_location`, must not be `None`")  # noqa: E501
 
         self._ip_location = ip_location
 
     @property
     def timestamp(self):
         """Gets the timestamp of this ProductsResponseIdentificationData.  # noqa: E501
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/response.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/response.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
@@ -101,49 +101,49 @@
 
         self._visits = visits
 
     @property
     def last_timestamp(self):
         """Gets the last_timestamp of this Response.  # noqa: E501
 
-        When more results are available (e.g., you scanned 200 results using `limit` parameter, but a total of 600 results are available), a special `lastTimestamp` top-level attribute is added to the response. If you want to paginate the results further in the past, you should use the value of this attribute.  # noqa: E501
+        ⚠️ Deprecated paging attribute, please use `paginationKey` instead. Timestamp of the last visit in the current page of results.   # noqa: E501
 
         :return: The last_timestamp of this Response.  # noqa: E501
         :rtype: int
         """
         return self._last_timestamp
 
     @last_timestamp.setter
     def last_timestamp(self, last_timestamp):
         """Sets the last_timestamp of this Response.
 
-        When more results are available (e.g., you scanned 200 results using `limit` parameter, but a total of 600 results are available), a special `lastTimestamp` top-level attribute is added to the response. If you want to paginate the results further in the past, you should use the value of this attribute.  # noqa: E501
+        ⚠️ Deprecated paging attribute, please use `paginationKey` instead. Timestamp of the last visit in the current page of results.   # noqa: E501
 
         :param last_timestamp: The last_timestamp of this Response.  # noqa: E501
         :type: int
         """
 
         self._last_timestamp = last_timestamp
 
     @property
     def pagination_key(self):
         """Gets the pagination_key of this Response.  # noqa: E501
 
-        Visit's `requestId` of the last visit in the current page.  # noqa: E501
+        Request ID of the last visit in the current page of results. Use this value in the following request as the `paginationKey` parameter to get the next page of results.  # noqa: E501
 
         :return: The pagination_key of this Response.  # noqa: E501
         :rtype: str
         """
         return self._pagination_key
 
     @pagination_key.setter
     def pagination_key(self, pagination_key):
         """Sets the pagination_key of this Response.
 
-        Visit's `requestId` of the last visit in the current page.  # noqa: E501
+        Request ID of the last visit in the current page of results. Use this value in the following request as the `paginationKey` parameter to get the next page of results.  # noqa: E501
 
         :param pagination_key: The pagination_key of this Response.  # noqa: E501
         :type: str
         """
 
         self._pagination_key = pagination_key
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/response_visits.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/response_visits.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
@@ -78,15 +78,16 @@
         self._first_seen_at = None
         self._last_seen_at = None
         self.discriminator = None
         self.request_id = request_id
         self.browser_details = browser_details
         self.incognito = incognito
         self.ip = ip
-        self.ip_location = ip_location
+        if ip_location is not None:
+            self.ip_location = ip_location
         self.timestamp = timestamp
         self.time = time
         self.url = url
         self.tag = tag
         if linked_id is not None:
             self.linked_id = linked_id
         self.confidence = confidence
@@ -204,16 +205,14 @@
     def ip_location(self, ip_location):
         """Sets the ip_location of this ResponseVisits.
 
 
         :param ip_location: The ip_location of this ResponseVisits.  # noqa: E501
         :type: IPLocation
         """
-        if ip_location is None:
-            raise ValueError("Invalid value for `ip_location`, must not be `None`")  # noqa: E501
 
         self._ip_location = ip_location
 
     @property
     def timestamp(self):
         """Gets the timestamp of this ResponseVisits.  # noqa: E501
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/seen_at.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/seen_at.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/signal_response_emulator.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/signal_response_tor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,93 +1,93 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class SignalResponseEmulator(object):
+class SignalResponseTor(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'data': 'SignalResponseEmulatorData',
+        'data': 'SignalResponseTorData',
         'error': 'ProductError'
     }
 
     attribute_map = {
         'data': 'data',
         'error': 'error'
     }
 
     def __init__(self, data=None, error=None):  # noqa: E501
-        """SignalResponseEmulator - a model defined in Swagger"""  # noqa: E501
+        """SignalResponseTor - a model defined in Swagger"""  # noqa: E501
         self._data = None
         self._error = None
         self.discriminator = None
         if data is not None:
             self.data = data
         if error is not None:
             self.error = error
 
     @property
     def data(self):
-        """Gets the data of this SignalResponseEmulator.  # noqa: E501
+        """Gets the data of this SignalResponseTor.  # noqa: E501
 
 
-        :return: The data of this SignalResponseEmulator.  # noqa: E501
-        :rtype: SignalResponseEmulatorData
+        :return: The data of this SignalResponseTor.  # noqa: E501
+        :rtype: SignalResponseTorData
         """
         return self._data
 
     @data.setter
     def data(self, data):
-        """Sets the data of this SignalResponseEmulator.
+        """Sets the data of this SignalResponseTor.
 
 
-        :param data: The data of this SignalResponseEmulator.  # noqa: E501
-        :type: SignalResponseEmulatorData
+        :param data: The data of this SignalResponseTor.  # noqa: E501
+        :type: SignalResponseTorData
         """
 
         self._data = data
 
     @property
     def error(self):
-        """Gets the error of this SignalResponseEmulator.  # noqa: E501
+        """Gets the error of this SignalResponseTor.  # noqa: E501
 
 
-        :return: The error of this SignalResponseEmulator.  # noqa: E501
+        :return: The error of this SignalResponseTor.  # noqa: E501
         :rtype: ProductError
         """
         return self._error
 
     @error.setter
     def error(self, error):
-        """Sets the error of this SignalResponseEmulator.
+        """Sets the error of this SignalResponseTor.
 
 
-        :param error: The error of this SignalResponseEmulator.  # noqa: E501
+        :param error: The error of this SignalResponseTor.  # noqa: E501
         :type: ProductError
         """
 
         self._error = error
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -106,15 +106,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(SignalResponseEmulator, dict):
+        if issubclass(SignalResponseTor, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -122,18 +122,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, SignalResponseEmulator):
+        if not isinstance(other, SignalResponseTor):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, SignalResponseEmulator):
+        if not isinstance(other, SignalResponseTor):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/signal_response_emulator_data.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/signal_response_emulator_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/signal_response_incognito.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/signal_response_incognito.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/signal_response_incognito_data.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/signal_response_incognito_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/signal_response_ip_blocklist.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/signal_response_ip_blocklist.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/signal_response_ip_info.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/signal_response_ip_info.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/signal_response_proxy.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/signal_response_proxy.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/signal_response_proxy_data.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/signal_response_proxy_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/signal_response_root_apps.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/signal_response_root_apps.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/signal_response_root_apps_data.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/signal_response_root_apps_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/signal_response_tampering.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/signal_response_tampering.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/signal_response_tor.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/subdivision.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,97 +1,97 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class SignalResponseTor(object):
+class Subdivision(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'data': 'SignalResponseTorData',
-        'error': 'ProductError'
+        'iso_code': 'str',
+        'name': 'str'
     }
 
     attribute_map = {
-        'data': 'data',
-        'error': 'error'
+        'iso_code': 'isoCode',
+        'name': 'name'
     }
 
-    def __init__(self, data=None, error=None):  # noqa: E501
-        """SignalResponseTor - a model defined in Swagger"""  # noqa: E501
-        self._data = None
-        self._error = None
+    def __init__(self, iso_code=None, name=None):  # noqa: E501
+        """Subdivision - a model defined in Swagger"""  # noqa: E501
+        self._iso_code = None
+        self._name = None
         self.discriminator = None
-        if data is not None:
-            self.data = data
-        if error is not None:
-            self.error = error
+        if iso_code is not None:
+            self.iso_code = iso_code
+        if name is not None:
+            self.name = name
 
     @property
-    def data(self):
-        """Gets the data of this SignalResponseTor.  # noqa: E501
+    def iso_code(self):
+        """Gets the iso_code of this Subdivision.  # noqa: E501
 
 
-        :return: The data of this SignalResponseTor.  # noqa: E501
-        :rtype: SignalResponseTorData
+        :return: The iso_code of this Subdivision.  # noqa: E501
+        :rtype: str
         """
-        return self._data
+        return self._iso_code
 
-    @data.setter
-    def data(self, data):
-        """Sets the data of this SignalResponseTor.
+    @iso_code.setter
+    def iso_code(self, iso_code):
+        """Sets the iso_code of this Subdivision.
 
 
-        :param data: The data of this SignalResponseTor.  # noqa: E501
-        :type: SignalResponseTorData
+        :param iso_code: The iso_code of this Subdivision.  # noqa: E501
+        :type: str
         """
 
-        self._data = data
+        self._iso_code = iso_code
 
     @property
-    def error(self):
-        """Gets the error of this SignalResponseTor.  # noqa: E501
+    def name(self):
+        """Gets the name of this Subdivision.  # noqa: E501
 
 
-        :return: The error of this SignalResponseTor.  # noqa: E501
-        :rtype: ProductError
+        :return: The name of this Subdivision.  # noqa: E501
+        :rtype: str
         """
-        return self._error
+        return self._name
 
-    @error.setter
-    def error(self, error):
-        """Sets the error of this SignalResponseTor.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this Subdivision.
 
 
-        :param error: The error of this SignalResponseTor.  # noqa: E501
-        :type: ProductError
+        :param name: The name of this Subdivision.  # noqa: E501
+        :type: str
         """
 
-        self._error = error
+        self._name = name
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -106,15 +106,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(SignalResponseTor, dict):
+        if issubclass(Subdivision, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -122,18 +122,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, SignalResponseTor):
+        if not isinstance(other, Subdivision):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, SignalResponseTor):
+        if not isinstance(other, Subdivision):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/signal_response_tor_data.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/signal_response_tor_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/signal_response_vpn.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/signal_response_vpn.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/subdivision.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/vpn_result.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,97 +1,99 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class Subdivision(object):
+class VpnResult(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'iso_code': 'str',
-        'name': 'str'
+        'result': 'bool',
+        'methods': 'VpnResultMethods'
     }
 
     attribute_map = {
-        'iso_code': 'isoCode',
-        'name': 'name'
+        'result': 'result',
+        'methods': 'methods'
     }
 
-    def __init__(self, iso_code=None, name=None):  # noqa: E501
-        """Subdivision - a model defined in Swagger"""  # noqa: E501
-        self._iso_code = None
-        self._name = None
+    def __init__(self, result=None, methods=None):  # noqa: E501
+        """VpnResult - a model defined in Swagger"""  # noqa: E501
+        self._result = None
+        self._methods = None
         self.discriminator = None
-        if iso_code is not None:
-            self.iso_code = iso_code
-        if name is not None:
-            self.name = name
+        if result is not None:
+            self.result = result
+        if methods is not None:
+            self.methods = methods
 
     @property
-    def iso_code(self):
-        """Gets the iso_code of this Subdivision.  # noqa: E501
+    def result(self):
+        """Gets the result of this VpnResult.  # noqa: E501
 
+        VPN or other anonymising service has been used when sending the request.  # noqa: E501
 
-        :return: The iso_code of this Subdivision.  # noqa: E501
-        :rtype: str
+        :return: The result of this VpnResult.  # noqa: E501
+        :rtype: bool
         """
-        return self._iso_code
+        return self._result
 
-    @iso_code.setter
-    def iso_code(self, iso_code):
-        """Sets the iso_code of this Subdivision.
+    @result.setter
+    def result(self, result):
+        """Sets the result of this VpnResult.
 
+        VPN or other anonymising service has been used when sending the request.  # noqa: E501
 
-        :param iso_code: The iso_code of this Subdivision.  # noqa: E501
-        :type: str
+        :param result: The result of this VpnResult.  # noqa: E501
+        :type: bool
         """
 
-        self._iso_code = iso_code
+        self._result = result
 
     @property
-    def name(self):
-        """Gets the name of this Subdivision.  # noqa: E501
+    def methods(self):
+        """Gets the methods of this VpnResult.  # noqa: E501
 
 
-        :return: The name of this Subdivision.  # noqa: E501
-        :rtype: str
+        :return: The methods of this VpnResult.  # noqa: E501
+        :rtype: VpnResultMethods
         """
-        return self._name
+        return self._methods
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this Subdivision.
+    @methods.setter
+    def methods(self, methods):
+        """Sets the methods of this VpnResult.
 
 
-        :param name: The name of this Subdivision.  # noqa: E501
-        :type: str
+        :param methods: The methods of this VpnResult.  # noqa: E501
+        :type: VpnResultMethods
         """
 
-        self._name = name
+        self._methods = methods
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -106,15 +108,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(Subdivision, dict):
+        if issubclass(VpnResult, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -122,18 +124,18 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Subdivision):
+        if not isinstance(other, VpnResult):
             return False
 
         return self.to_dict() == other.to_dict()
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
-        if not isinstance(other, Subdivision):
+        if not isinstance(other, VpnResult):
             return True
 
         return self.to_dict() != other.to_dict()
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/tampering_result.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/tampering_result.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/visit.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/visit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
@@ -78,15 +78,16 @@
         self._first_seen_at = None
         self._last_seen_at = None
         self.discriminator = None
         self.request_id = request_id
         self.browser_details = browser_details
         self.incognito = incognito
         self.ip = ip
-        self.ip_location = ip_location
+        if ip_location is not None:
+            self.ip_location = ip_location
         self.timestamp = timestamp
         self.time = time
         self.url = url
         if tag is not None:
             self.tag = tag
         if linked_id is not None:
             self.linked_id = linked_id
@@ -205,16 +206,14 @@
     def ip_location(self, ip_location):
         """Sets the ip_location of this Visit.
 
 
         :param ip_location: The ip_location of this Visit.  # noqa: E501
         :type: IPLocation
         """
-        if ip_location is None:
-            raise ValueError("Invalid value for `ip_location`, must not be `None`")  # noqa: E501
 
         self._ip_location = ip_location
 
     @property
     def timestamp(self):
         """Gets the timestamp of this Visit.  # noqa: E501
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/vpn_result_methods.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/vpn_result_methods.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/webhook_signal_response_emulator.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/webhook_signal_response_emulator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/webhook_signal_response_proxy.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/webhook_signal_response_proxy.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/webhook_signal_response_root_apps.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/webhook_signal_response_root_apps.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/webhook_signal_response_tor.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/webhook_signal_response_tor.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/models/webhook_visit.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/models/webhook_visit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
@@ -137,15 +137,16 @@
         if proxy is not None:
             self.proxy = proxy
         if tampering is not None:
             self.tampering = tampering
         self.request_id = request_id
         self.browser_details = browser_details
         self.ip = ip
-        self.ip_location = ip_location
+        if ip_location is not None:
+            self.ip_location = ip_location
         self.timestamp = timestamp
         self.time = time
         self.url = url
         if tag is not None:
             self.tag = tag
         if linked_id is not None:
             self.linked_id = linked_id
@@ -518,16 +519,14 @@
     def ip_location(self, ip_location):
         """Sets the ip_location of this WebhookVisit.
 
 
         :param ip_location: The ip_location of this WebhookVisit.  # noqa: E501
         :type: IPLocation
         """
-        if ip_location is None:
-            raise ValueError("Invalid value for `ip_location`, must not be `None`")  # noqa: E501
 
         self._ip_location = ip_location
 
     @property
     def timestamp(self):
         """Gets the timestamp of this WebhookVisit.  # noqa: E501
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk/rest.py` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk.egg-info/PKG-INFO` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: fingerprint-pro-server-api-sdk
-Version: 2.2.0
-Summary: Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.
+Version: 2.3.0
+Summary: Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it&#x27;s not intended to be used from the client side, whether it&#x27;s a browser or a mobile device. 
 Home-page: https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk
 Author: Fingerprint
 Author-email: support@fingerprint.com
 License: MIT
 Keywords: Swagger,Fingerprint Pro Server API,browser,detection,fingerprint,identification,fingerprinting,browser-fingerprinting,browser-fingerprint,fraud-detection,fraud,audio-fingerprinting,fingerprintjs,fingerprintjs-pro,visitor-identifier
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -52,20 +52,20 @@
   </a>
   <a href="https://discord.gg/39EpE2neBg">
     <img src="https://img.shields.io/discord/852099967190433792?style=logo&label=Discord&logo=Discord&logoColor=white" alt="Discord server">
   </a>
 </p>
 
 # Fingerprint Pro Server Python SDK
-Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.
+Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device. 
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
 - API version: 3
-- Package version: 2.2.0
+- Package version: 2.3.0
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
```

#### html2text {}

```diff
@@ -1,12 +1,14 @@
-Metadata-Version: 2.1 Name: fingerprint-pro-server-api-sdk Version: 2.2.0
+Metadata-Version: 2.1 Name: fingerprint-pro-server-api-sdk Version: 2.3.0
 Summary: Fingerprint Pro Server API allows you to get information about
-visitors and about individual events in a server environment. This API can be
-used for data exports, decision-making, and data analysis scenarios. Home-page:
-https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk Author:
+visitors and about individual events in a server environment. It can be used
+for data exports, decision-making, and data analysis scenarios. Server API is
+intended for server-side usage, it&#x27;s not intended to be used from the
+client side, whether it&#x27;s a browser or a mobile device. Home-page: https:/
+/github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk Author:
 Fingerprint Author-email: support@fingerprint.com License: MIT Keywords:
 Swagger,Fingerprint Pro Server
 API,browser,detection,fingerprint,identification,fingerprinting,browser-
 fingerprinting,browser-fingerprint,fraud-detection,fraud,audio-
 fingerprinting,fingerprintjs,fingerprintjs-pro,visitor-identifier Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
@@ -21,18 +23,20 @@
 :: Python Modules Classifier: Topic :: Security Description-Content-Type: text/
 markdown License-File: LICENSE
                               [Fingerprint_logo]
  [PyPI] [coverage] [CI_badge] [CI_badge] [CI_badge] [https://img.shields.io/:
                license-mit-blue.svg?style=flat] [Discord_server]
 # Fingerprint Pro Server Python SDK Fingerprint Pro Server API allows you to
 get information about visitors and about individual events in a server
-environment. This API can be used for data exports, decision-making, and data
-analysis scenarios. This Python package is automatically generated by the
-[Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project: -
-API version: 3 - Package version: 2.2.0 - Build package:
+environment. It can be used for data exports, decision-making, and data
+analysis scenarios. Server API is intended for server-side usage, it's not
+intended to be used from the client side, whether it's a browser or a mobile
+device. This Python package is automatically generated by the [Swagger Codegen]
+(https://github.com/swagger-api/swagger-codegen) project: - API version: 3 -
+Package version: 2.3.0 - Build package:
 io.swagger.codegen.v3.generators.python.PythonClientCodegen ## Requirements.
 Python 2.7 and 3.4+ ## Installation & Usage ### pip install You can install the
 package directly from the Github ```sh pip install git+https://github.com/
 fingerprintjs/fingerprint-pro-server-api-python-sdk.git ``` Or from the PyPI
 ```sh pip install fingerprint_pro_server_api_sdk ``` Then import the package:
 ```python import fingerprint_pro_server_api_sdk ``` ### Setuptools Install via
 [Setuptools](http://pypi.python.org/pypi/setuptools). ```sh python setup.py
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/fingerprint_pro_server_api_sdk.egg-info/SOURCES.txt` & `fingerprint-pro-server-api-sdk-2.3.0/fingerprint_pro_server_api_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/setup.py` & `fingerprint-pro-server-api-sdk-2.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # coding: utf-8
 
 """
     Fingerprint Pro Server API
 
-    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.  # noqa: E501
+    Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it's not intended to be used from the client side, whether it's a browser or a mobile device.   # noqa: E501
 
     OpenAPI spec version: 3
     Contact: support@fingerprint.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pathlib
 import re
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "fingerprint-pro-server-api-sdk"
-VERSION = "2.2.0"
+VERSION = "2.3.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 
@@ -36,15 +36,15 @@
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 long_description = re.sub("<source[^>]*>\n", '', long_description.replace("<picture>\n", "").replace("</picture>\n", ""))
 long_description = re.sub(r"(?P<prefix>\[[^]]*]\()(?P<postfix>docs/[^)]*\))", '\g<prefix>https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk/blob/main/\g<postfix>', long_description)
 
 setup(
     name=NAME,
     version=VERSION,
-    description="Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. This API can be used for data exports, decision-making, and data analysis scenarios.",
+    description="Fingerprint Pro Server API allows you to get information about visitors and about individual events in a server environment. It can be used for data exports, decision-making, and data analysis scenarios. Server API is intended for server-side usage, it&#x27;s not intended to be used from the client side, whether it&#x27;s a browser or a mobile device. ",
     long_description=long_description,
     long_description_content_type='text/markdown',
     license="MIT",
     license_files=["LICENSE"],
     author="Fingerprint",
     author_email="support@fingerprint.com",
     url="https://github.com/fingerprintjs/fingerprint-pro-server-api-python-sdk",
```

### Comparing `fingerprint-pro-server-api-sdk-2.2.0/test/test_fingerprint_api.py` & `fingerprint-pro-server-api-sdk-2.3.0/test/test_fingerprint_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from fingerprint_pro_server_api_sdk import Configuration, ManyRequestsResponse, ErrorVisits403, ErrorEvent403Response, \
     ErrorEvent404Response
 from fingerprint_pro_server_api_sdk.api.fingerprint_api import FingerprintApi  # noqa: E501
 from fingerprint_pro_server_api_sdk.rest import KnownApiException
 
 API_KEY = 'private_key'
 
-VERSION = '2.2.0'
+VERSION = '2.3.0'
 
 
 class MockPoolManager(object):
     def __init__(self, tc):
         self._tc = tc
         self._reqs = []
```

