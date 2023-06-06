# Comparing `tmp/google-cloud-billing-budgets-1.9.0.tar.gz` & `tmp/google-cloud-billing-budgets-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-billing-budgets-1.9.0.tar", last modified: Tue Jan 10 20:33:49 2023, max compression
+gzip compressed data, was "google-cloud-billing-budgets-1.9.1.tar", last modified: Mon Jan 23 16:18:49 2023, max compression
```

## Comparing `google-cloud-billing-budgets-1.9.0.tar` & `google-cloud-billing-budgets-1.9.1.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 20:33:49.001419 google-cloud-billing-budgets-1.9.0/
--rw-rw-r--   0 root         (0)     1003    11358 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4869 2023-01-10 20:33:49.001419 google-cloud-billing-budgets-1.9.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3930 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 20:33:48.989420 google-cloud-billing-budgets-1.9.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 20:33:48.989420 google-cloud-billing-budgets-1.9.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 20:33:48.993420 google-cloud-billing-budgets-1.9.0/google/cloud/billing/
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 20:33:48.993420 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets/
--rw-rw-r--   0 root         (0)     1003     1756 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 20:33:48.993420 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1/
--rw-rw-r--   0 root         (0)     1003     1558 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     1742 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 20:33:48.993420 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1/proto/
--rw-rw-r--   0 root         (0)     1003    10889 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1/proto/budget_model.proto
--rw-rw-r--   0 root         (0)     1003     6798 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1/proto/budget_service.proto
--rw-rw-r--   0 root         (0)     1003       89 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 20:33:48.993420 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 20:33:48.997419 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1/services/budget_service/
--rw-rw-r--   0 root         (0)     1003      765 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1/services/budget_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    34405 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1/services/budget_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    42545 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1/services/budget_service/client.py
--rw-rw-r--   0 root         (0)     1003     5811 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1/services/budget_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 20:33:48.997419 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1/services/budget_service/transports/
--rw-rw-r--   0 root         (0)     1003     1184 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1/services/budget_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9470 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1/services/budget_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17161 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1/services/budget_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    17462 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1/services/budget_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 20:33:48.997419 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1/types/
--rw-rw-r--   0 root         (0)     1003     1285 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    17474 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1/types/budget_model.py
--rw-rw-r--   0 root         (0)     1003     5199 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1/types/budget_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 20:33:48.997419 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1beta1/
--rw-rw-r--   0 root         (0)     1003     1552 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     1752 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1beta1/gapic_version.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 20:33:48.997419 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1beta1/proto/
--rw-rw-r--   0 root         (0)     1003    10763 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1beta1/proto/budget_model.proto
--rw-rw-r--   0 root         (0)     1003     6512 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1beta1/proto/budget_service.proto
--rw-rw-r--   0 root         (0)     1003       89 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 20:33:48.997419 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 20:33:48.997419 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1beta1/services/budget_service/
--rw-rw-r--   0 root         (0)     1003      765 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1beta1/services/budget_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    28245 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1beta1/services/budget_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    36357 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1beta1/services/budget_service/client.py
--rw-rw-r--   0 root         (0)     1003     5856 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1beta1/services/budget_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 20:33:49.001419 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1beta1/services/budget_service/transports/
--rw-rw-r--   0 root         (0)     1003     1184 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1beta1/services/budget_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9480 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1beta1/services/budget_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    17191 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1beta1/services/budget_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    17492 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1beta1/services/budget_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 20:33:49.001419 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1beta1/types/
--rw-rw-r--   0 root         (0)     1003     1279 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    18297 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1beta1/types/budget_model.py
--rw-rw-r--   0 root         (0)     1003     5224 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1beta1/types/budget_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 20:33:49.001419 google-cloud-billing-budgets-1.9.0/google_cloud_billing_budgets.egg-info/
--rw-r--r--   0 root         (0)     1003     4869 2023-01-10 20:33:48.000000 google-cloud-billing-budgets-1.9.0/google_cloud_billing_budgets.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     3095 2023-01-10 20:33:48.000000 google-cloud-billing-budgets-1.9.0/google_cloud_billing_budgets.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-10 20:33:48.000000 google-cloud-billing-budgets-1.9.0/google_cloud_billing_budgets.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-01-10 20:33:48.000000 google-cloud-billing-budgets-1.9.0/google_cloud_billing_budgets.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-01-10 20:33:48.000000 google-cloud-billing-budgets-1.9.0/google_cloud_billing_budgets.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-01-10 20:33:48.000000 google-cloud-billing-budgets-1.9.0/google_cloud_billing_budgets.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-01-10 20:33:48.000000 google-cloud-billing-budgets-1.9.0/google_cloud_billing_budgets.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-01-10 20:33:49.005418 google-cloud-billing-budgets-1.9.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3011 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 20:33:49.001419 google-cloud-billing-budgets-1.9.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 20:33:49.001419 google-cloud-billing-budgets-1.9.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 20:33:49.001419 google-cloud-billing-budgets-1.9.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 20:33:49.001419 google-cloud-billing-budgets-1.9.0/tests/unit/gapic/budgets_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/tests/unit/gapic/budgets_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003    99509 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/tests/unit/gapic/budgets_v1/test_budget_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-01-10 20:33:49.001419 google-cloud-billing-budgets-1.9.0/tests/unit/gapic/budgets_v1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/tests/unit/gapic/budgets_v1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003    84587 2023-01-10 20:30:57.000000 google-cloud-billing-budgets-1.9.0/tests/unit/gapic/budgets_v1beta1/test_budget_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:49.517998 google-cloud-billing-budgets-1.9.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4869 2023-01-23 16:18:49.517998 google-cloud-billing-budgets-1.9.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3930 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:49.505998 google-cloud-billing-budgets-1.9.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:49.505998 google-cloud-billing-budgets-1.9.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:49.505998 google-cloud-billing-budgets-1.9.1/google/cloud/billing/
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:49.509998 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets/
+-rw-rw-r--   0 root         (0)     1003     1756 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:49.509998 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1/
+-rw-rw-r--   0 root         (0)     1003     1558 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1742 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:49.509998 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1/proto/
+-rw-rw-r--   0 root         (0)     1003    10889 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1/proto/budget_model.proto
+-rw-rw-r--   0 root         (0)     1003     6798 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1/proto/budget_service.proto
+-rw-rw-r--   0 root         (0)     1003       89 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:49.509998 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:49.509998 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1/services/budget_service/
+-rw-rw-r--   0 root         (0)     1003      765 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1/services/budget_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    34405 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1/services/budget_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    42570 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1/services/budget_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5811 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1/services/budget_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:49.513998 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1/services/budget_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1184 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1/services/budget_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9470 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1/services/budget_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17161 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1/services/budget_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    17462 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1/services/budget_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:49.513998 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1285 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    19393 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1/types/budget_model.py
+-rw-rw-r--   0 root         (0)     1003     5199 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1/types/budget_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:49.513998 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1beta1/
+-rw-rw-r--   0 root         (0)     1003     1552 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1752 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1beta1/gapic_version.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:49.513998 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1beta1/proto/
+-rw-rw-r--   0 root         (0)     1003    10763 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1beta1/proto/budget_model.proto
+-rw-rw-r--   0 root         (0)     1003     6512 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1beta1/proto/budget_service.proto
+-rw-rw-r--   0 root         (0)     1003       89 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:49.513998 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:49.513998 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1beta1/services/budget_service/
+-rw-rw-r--   0 root         (0)     1003      765 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1beta1/services/budget_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    28245 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1beta1/services/budget_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    36382 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1beta1/services/budget_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5856 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1beta1/services/budget_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:49.513998 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1beta1/services/budget_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1184 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1beta1/services/budget_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9480 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1beta1/services/budget_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    17191 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1beta1/services/budget_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    17492 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1beta1/services/budget_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:49.513998 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1beta1/types/
+-rw-rw-r--   0 root         (0)     1003     1279 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    20365 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1beta1/types/budget_model.py
+-rw-rw-r--   0 root         (0)     1003     5224 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1beta1/types/budget_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:49.517998 google-cloud-billing-budgets-1.9.1/google_cloud_billing_budgets.egg-info/
+-rw-r--r--   0 root         (0)     1003     4869 2023-01-23 16:18:49.000000 google-cloud-billing-budgets-1.9.1/google_cloud_billing_budgets.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     3095 2023-01-23 16:18:49.000000 google-cloud-billing-budgets-1.9.1/google_cloud_billing_budgets.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-01-23 16:18:49.000000 google-cloud-billing-budgets-1.9.1/google_cloud_billing_budgets.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-01-23 16:18:49.000000 google-cloud-billing-budgets-1.9.1/google_cloud_billing_budgets.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-01-23 16:18:49.000000 google-cloud-billing-budgets-1.9.1/google_cloud_billing_budgets.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-01-23 16:18:49.000000 google-cloud-billing-budgets-1.9.1/google_cloud_billing_budgets.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-01-23 16:18:49.000000 google-cloud-billing-budgets-1.9.1/google_cloud_billing_budgets.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-01-23 16:18:49.517998 google-cloud-billing-budgets-1.9.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3011 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:49.517998 google-cloud-billing-budgets-1.9.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:49.517998 google-cloud-billing-budgets-1.9.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:49.517998 google-cloud-billing-budgets-1.9.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:49.517998 google-cloud-billing-budgets-1.9.1/tests/unit/gapic/budgets_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/tests/unit/gapic/budgets_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    99509 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/tests/unit/gapic/budgets_v1/test_budget_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-01-23 16:18:49.517998 google-cloud-billing-budgets-1.9.1/tests/unit/gapic/budgets_v1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/tests/unit/gapic/budgets_v1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    84587 2023-01-23 16:16:10.000000 google-cloud-billing-budgets-1.9.1/tests/unit/gapic/budgets_v1beta1/test_budget_service.py
```

### Comparing `google-cloud-billing-budgets-1.9.0/LICENSE` & `google-cloud-billing-budgets-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-budgets-1.9.0/MANIFEST.in` & `google-cloud-billing-budgets-1.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-budgets-1.9.0/PKG-INFO` & `google-cloud-billing-budgets-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-billing-budgets
-Version: 1.9.0
+Version: 1.9.1
 Summary: Google Cloud Billing Budgets API client library
 Home-page: https://github.com/googleapis/python-billingbudgets
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-billing-budgets-1.9.0/README.rst` & `google-cloud-billing-budgets-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets/__init__.py` & `google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets/gapic_version.py` & `google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.9.0"  # {x-release-please-version}
+__version__ = "1.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1/__init__.py` & `google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1/gapic_metadata.json` & `google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1/gapic_version.py` & `google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.9.0"  # {x-release-please-version}
+__version__ = "1.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1/proto/budget_model.proto` & `google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1/proto/budget_model.proto`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1/proto/budget_service.proto` & `google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1/proto/budget_service.proto`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1/services/__init__.py` & `google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1/services/budget_service/__init__.py` & `google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1/services/budget_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1/services/budget_service/async_client.py` & `google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1/services/budget_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1/services/budget_service/client.py` & `google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1/services/budget_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1008,15 +1008,15 @@
         rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
-    def __enter__(self):
+    def __enter__(self) -> "BudgetServiceClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
 
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
```

### Comparing `google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1/services/budget_service/pagers.py` & `google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1/services/budget_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1/services/budget_service/transports/__init__.py` & `google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1/services/budget_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1/services/budget_service/transports/base.py` & `google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1/services/budget_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1/services/budget_service/transports/grpc.py` & `google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1/services/budget_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1/services/budget_service/transports/grpc_asyncio.py` & `google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1/services/budget_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1/types/__init__.py` & `google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1/types/budget_model.py` & `google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1/types/budget_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,14 +36,27 @@
 
 
 class CalendarPeriod(proto.Enum):
     r"""A ``CalendarPeriod`` represents the abstract concept of a time
     period that has a canonical start. Grammatically, "the start of the
     current ``CalendarPeriod``". All calendar times begin at 12 AM US
     and Canadian Pacific Time (UTC-8).
+
+    Values:
+        CALENDAR_PERIOD_UNSPECIFIED (0):
+
+        MONTH (1):
+            A month. Month starts on the first day of
+            each month, such as January 1, February 1, March
+            1, and so on.
+        QUARTER (2):
+            A quarter. Quarters start on dates January 1,
+            April 1, July 1, and October 1 of each year.
+        YEAR (3):
+            A year. Year starts on January 1.
     """
     CALENDAR_PERIOD_UNSPECIFIED = 0
     MONTH = 1
     QUARTER = 2
     YEAR = 3
 
 
@@ -197,14 +210,28 @@
             passed the threshold. Behavior defaults to CURRENT_SPEND if
             not set.
     """
 
     class Basis(proto.Enum):
         r"""The type of basis used to determine if spend has passed the
         threshold.
+
+        Values:
+            BASIS_UNSPECIFIED (0):
+                Unspecified threshold basis.
+            CURRENT_SPEND (1):
+                Use current spend as the basis for comparison
+                against the threshold.
+            FORECASTED_SPEND (2):
+                Use forecasted spend for the period as the basis for
+                comparison against the threshold. FORECASTED_SPEND can only
+                be set when the budget's time period is a
+                [Filter.calendar_period][google.cloud.billing.budgets.v1.Filter.calendar_period].
+                It cannot be set in combination with
+                [Filter.custom_period][google.cloud.billing.budgets.v1.Filter.custom_period].
         """
         BASIS_UNSPECIFIED = 0
         CURRENT_SPEND = 1
         FORECASTED_SPEND = 2
 
     threshold_percent: float = proto.Field(
         proto.DOUBLE,
@@ -359,14 +386,32 @@
 
     class CreditTypesTreatment(proto.Enum):
         r"""Specifies how credits are applied when determining the spend for
         threshold calculations. Budgets track the total cost minus any
         applicable selected credits. `See the documentation for a list of
         credit
         types <https://cloud.google.com/billing/docs/how-to/export-data-bigquery-tables#credits-type>`__.
+
+        Values:
+            CREDIT_TYPES_TREATMENT_UNSPECIFIED (0):
+
+            INCLUDE_ALL_CREDITS (1):
+                All types of credit are subtracted from the
+                gross cost to determine the spend for threshold
+                calculations.
+            EXCLUDE_ALL_CREDITS (2):
+                All types of credit are added to the net cost
+                to determine the spend for threshold
+                calculations.
+            INCLUDE_SPECIFIED_CREDITS (3):
+                `Credit
+                types <https://cloud.google.com/billing/docs/how-to/export-data-bigquery-tables#credits-type>`__
+                specified in the credit_types field are subtracted from the
+                gross cost to determine the spend for threshold
+                calculations.
         """
         CREDIT_TYPES_TREATMENT_UNSPECIFIED = 0
         INCLUDE_ALL_CREDITS = 1
         EXCLUDE_ALL_CREDITS = 2
         INCLUDE_SPECIFIED_CREDITS = 3
 
     projects: MutableSequence[str] = proto.RepeatedField(
```

### Comparing `google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1/types/budget_service.py` & `google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1/types/budget_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1beta1/__init__.py` & `google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1beta1/gapic_metadata.json` & `google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1beta1/gapic_version.py` & `google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1beta1/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.9.0"  # {x-release-please-version}
+__version__ = "1.9.1"  # {x-release-please-version}
```

### Comparing `google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1beta1/proto/budget_model.proto` & `google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1beta1/proto/budget_model.proto`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1beta1/proto/budget_service.proto` & `google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1beta1/proto/budget_service.proto`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1beta1/services/__init__.py` & `google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1beta1/services/budget_service/__init__.py` & `google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1beta1/services/budget_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1beta1/services/budget_service/async_client.py` & `google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1beta1/services/budget_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1beta1/services/budget_service/client.py` & `google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1beta1/services/budget_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -875,15 +875,15 @@
         rpc(
             request,
             retry=retry,
             timeout=timeout,
             metadata=metadata,
         )
 
-    def __enter__(self):
+    def __enter__(self) -> "BudgetServiceClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
 
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
```

### Comparing `google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1beta1/services/budget_service/pagers.py` & `google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1beta1/services/budget_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1beta1/services/budget_service/transports/__init__.py` & `google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1beta1/services/budget_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1beta1/services/budget_service/transports/base.py` & `google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1beta1/services/budget_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1beta1/services/budget_service/transports/grpc.py` & `google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1beta1/services/budget_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1beta1/services/budget_service/transports/grpc_asyncio.py` & `google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1beta1/services/budget_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1beta1/types/__init__.py` & `google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1beta1/types/budget_model.py` & `google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1beta1/types/budget_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,29 @@
 
 
 class CalendarPeriod(proto.Enum):
     r"""A ``CalendarPeriod`` represents the abstract concept of a time
     period that has a canonical start. Grammatically, "the start of the
     current ``CalendarPeriod``". All calendar times begin at 12 AM US
     and Canadian Pacific Time (UTC-8).
+
+    Values:
+        CALENDAR_PERIOD_UNSPECIFIED (0):
+            Calendar period is unset. This is the default
+            if the budget is for a custom time period
+            (CustomPeriod).
+        MONTH (1):
+            A month. Month starts on the first day of
+            each month, such as January 1, February 1, March
+            1, and so on.
+        QUARTER (2):
+            A quarter. Quarters start on dates January 1,
+            April 1, July 1, and October 1 of each year.
+        YEAR (3):
+            A year. Year starts on January 1.
     """
     CALENDAR_PERIOD_UNSPECIFIED = 0
     MONTH = 1
     QUARTER = 2
     YEAR = 3
 
 
@@ -212,14 +227,28 @@
             passed the threshold. Behavior defaults to CURRENT_SPEND if
             not set.
     """
 
     class Basis(proto.Enum):
         r"""The type of basis used to determine if spend has passed the
         threshold.
+
+        Values:
+            BASIS_UNSPECIFIED (0):
+                Unspecified threshold basis.
+            CURRENT_SPEND (1):
+                Use current spend as the basis for comparison
+                against the threshold.
+            FORECASTED_SPEND (2):
+                Use forecasted spend for the period as the basis for
+                comparison against the threshold. FORECASTED_SPEND can only
+                be set when the budget's time period is a
+                [Filter.calendar_period][google.cloud.billing.budgets.v1beta1.Filter.calendar_period].
+                It cannot be set in combination with
+                [Filter.custom_period][google.cloud.billing.budgets.v1beta1.Filter.custom_period].
         """
         BASIS_UNSPECIFIED = 0
         CURRENT_SPEND = 1
         FORECASTED_SPEND = 2
 
     threshold_percent: float = proto.Field(
         proto.DOUBLE,
@@ -377,14 +406,32 @@
 
     class CreditTypesTreatment(proto.Enum):
         r"""Specifies how credits are applied when determining the spend for
         threshold calculations. Budgets track the total cost minus any
         applicable selected credits. `See the documentation for a list of
         credit
         types <https://cloud.google.com/billing/docs/how-to/export-data-bigquery-tables#credits-type>`__.
+
+        Values:
+            CREDIT_TYPES_TREATMENT_UNSPECIFIED (0):
+
+            INCLUDE_ALL_CREDITS (1):
+                All types of credit are subtracted from the
+                gross cost to determine the spend for threshold
+                calculations.
+            EXCLUDE_ALL_CREDITS (2):
+                All types of credit are added to the net cost
+                to determine the spend for threshold
+                calculations.
+            INCLUDE_SPECIFIED_CREDITS (3):
+                `Credit
+                types <https://cloud.google.com/billing/docs/how-to/export-data-bigquery-tables#credits-type>`__
+                specified in the credit_types field are subtracted from the
+                gross cost to determine the spend for threshold
+                calculations.
         """
         CREDIT_TYPES_TREATMENT_UNSPECIFIED = 0
         INCLUDE_ALL_CREDITS = 1
         EXCLUDE_ALL_CREDITS = 2
         INCLUDE_SPECIFIED_CREDITS = 3
 
     projects: MutableSequence[str] = proto.RepeatedField(
```

### Comparing `google-cloud-billing-budgets-1.9.0/google/cloud/billing/budgets_v1beta1/types/budget_service.py` & `google-cloud-billing-budgets-1.9.1/google/cloud/billing/budgets_v1beta1/types/budget_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-budgets-1.9.0/google_cloud_billing_budgets.egg-info/PKG-INFO` & `google-cloud-billing-budgets-1.9.1/google_cloud_billing_budgets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-billing-budgets
-Version: 1.9.0
+Version: 1.9.1
 Summary: Google Cloud Billing Budgets API client library
 Home-page: https://github.com/googleapis/python-billingbudgets
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-billing-budgets-1.9.0/google_cloud_billing_budgets.egg-info/SOURCES.txt` & `google-cloud-billing-budgets-1.9.1/google_cloud_billing_budgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-budgets-1.9.0/setup.py` & `google-cloud-billing-budgets-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-budgets-1.9.0/tests/__init__.py` & `google-cloud-billing-budgets-1.9.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-budgets-1.9.0/tests/unit/__init__.py` & `google-cloud-billing-budgets-1.9.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-budgets-1.9.0/tests/unit/gapic/__init__.py` & `google-cloud-billing-budgets-1.9.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-budgets-1.9.0/tests/unit/gapic/budgets_v1/__init__.py` & `google-cloud-billing-budgets-1.9.1/tests/unit/gapic/budgets_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-budgets-1.9.0/tests/unit/gapic/budgets_v1/test_budget_service.py` & `google-cloud-billing-budgets-1.9.1/tests/unit/gapic/budgets_v1/test_budget_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-budgets-1.9.0/tests/unit/gapic/budgets_v1beta1/__init__.py` & `google-cloud-billing-budgets-1.9.1/tests/unit/gapic/budgets_v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-billing-budgets-1.9.0/tests/unit/gapic/budgets_v1beta1/test_budget_service.py` & `google-cloud-billing-budgets-1.9.1/tests/unit/gapic/budgets_v1beta1/test_budget_service.py`

 * *Files identical despite different names*

