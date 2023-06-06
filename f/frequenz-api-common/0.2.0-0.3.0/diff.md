# Comparing `tmp/frequenz-api-common-0.2.0.tar.gz` & `tmp/frequenz-api-common-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frequenz-api-common-0.2.0.tar", last modified: Tue May 23 11:39:02 2023, max compression
+gzip compressed data, was "frequenz-api-common-0.3.0.tar", last modified: Tue Jun  6 09:33:28 2023, max compression
```

## Comparing `frequenz-api-common-0.2.0.tar` & `frequenz-api-common-0.3.0.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.249514 frequenz-api-common-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)      281 2023-05-23 11:38:44.000000 frequenz-api-common-0.2.0/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (122)     2263 2023-05-23 11:38:44.000000 frequenz-api-common-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)     1090 2023-05-23 11:38:44.000000 frequenz-api-common-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      203 2023-05-23 11:38:44.000000 frequenz-api-common-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-05-23 11:39:02.249514 frequenz-api-common-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-05-23 11:38:44.000000 frequenz-api-common-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      130 2023-05-23 11:38:44.000000 frequenz-api-common-0.2.0/RELEASE_NOTES.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.233512 frequenz-api-common-0.2.0/proto/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.233512 frequenz-api-common-0.2.0/proto/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.233512 frequenz-api-common-0.2.0/proto/frequenz/api/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.237513 frequenz-api-common-0.2.0/proto/frequenz/api/common/
--rw-r--r--   0 runner    (1001) docker     (122)     2860 2023-05-23 11:38:44.000000 frequenz-api-common-0.2.0/proto/frequenz/api/common/components.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.237513 frequenz-api-common-0.2.0/proto/frequenz/api/common/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)     6145 2023-05-23 11:38:44.000000 frequenz-api-common-0.2.0/proto/frequenz/api/common/metrics/electrical.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3552 2023-05-23 11:38:44.000000 frequenz-api-common-0.2.0/proto/frequenz/api/common/metrics.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.233512 frequenz-api-common-0.2.0/py/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.233512 frequenz-api-common-0.2.0/py/frequenz/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.233512 frequenz-api-common-0.2.0/py/frequenz/api/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.237513 frequenz-api-common-0.2.0/py/frequenz/api/common/
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-05-23 11:38:44.000000 frequenz-api-common-0.2.0/py/frequenz/api/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.237513 frequenz-api-common-0.2.0/py/frequenz/api/common/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)      121 2023-05-23 11:38:44.000000 frequenz-api-common-0.2.0/py/frequenz/api/common/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-23 11:38:44.000000 frequenz-api-common-0.2.0/py/frequenz/api/common/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.237513 frequenz-api-common-0.2.0/py/frequenz_api_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-05-23 11:39:02.000000 frequenz-api-common-0.2.0/py/frequenz_api_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3704 2023-05-23 11:39:02.000000 frequenz-api-common-0.2.0/py/frequenz_api_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 11:39:02.000000 frequenz-api-common-0.2.0/py/frequenz_api_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      485 2023-05-23 11:39:02.000000 frequenz-api-common-0.2.0/py/frequenz_api_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-23 11:39:02.000000 frequenz-api-common-0.2.0/py/frequenz_api_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2030 2023-05-23 11:38:44.000000 frequenz-api-common-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-23 11:39:02.249514 frequenz-api-common-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.233512 frequenz-api-common-0.2.0/submodules/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.233512 frequenz-api-common-0.2.0/submodules/api-common-protos/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.237513 frequenz-api-common-0.2.0/submodules/api-common-protos/google/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.241513 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/annotations.proto
--rw-r--r--   0 runner    (1001) docker     (122)     7374 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/auth.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/backend.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2504 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/billing.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3392 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/client.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3169 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/config_change.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2719 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/consumer.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2008 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/context.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1225 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/control.proto
--rw-r--r--   0 runner    (1001) docker     (122)     8657 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/distribution.proto
--rw-r--r--   0 runner    (1001) docker     (122)     6132 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/documentation.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2824 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/endpoint.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3318 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/field_behavior.proto
--rw-r--r--   0 runner    (1001) docker     (122)    12099 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/http.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2605 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/httpbody.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1391 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/label.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2910 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/launch_stage.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2045 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/log.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3209 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/logging.proto
--rw-r--r--   0 runner    (1001) docker     (122)     6628 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/metric.proto
--rw-r--r--   0 runner    (1001) docker     (122)     5512 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/monitored_resource.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3524 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/monitoring.proto
--rw-r--r--   0 runner    (1001) docker     (122)    10854 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/quota.proto
--rw-r--r--   0 runner    (1001) docker     (122)    11347 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/resource.proto
--rw-r--r--   0 runner    (1001) docker     (122)    14929 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/routing.proto
--rw-r--r--   0 runner    (1001) docker     (122)     6099 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/service.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1093 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/source_info.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3472 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/system_parameter.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3513 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/usage.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.241513 frequenz-api-common-0.2.0/submodules/api-common-protos/google/cloud/
--rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/cloud/extended_operations.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.233512 frequenz-api-common-0.2.0/submodules/api-common-protos/google/iam/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.233512 frequenz-api-common-0.2.0/submodules/api-common-protos/google/iam/admin/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.245513 frequenz-api-common-0.2.0/submodules/api-common-protos/google/iam/admin/v1/
--rw-r--r--   0 runner    (1001) docker     (122)    41483 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/iam/admin/v1/iam.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.245513 frequenz-api-common-0.2.0/submodules/api-common-protos/google/iam/v1/
--rw-r--r--   0 runner    (1001) docker     (122)     5482 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/iam/v1/iam_policy.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.245513 frequenz-api-common-0.2.0/submodules/api-common-protos/google/iam/v1/logging/
--rw-r--r--   0 runner    (1001) docker     (122)     1287 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/iam/v1/options.proto
--rw-r--r--   0 runner    (1001) docker     (122)     8659 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/iam/v1/policy.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.237513 frequenz-api-common-0.2.0/submodules/api-common-protos/google/logging/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.245513 frequenz-api-common-0.2.0/submodules/api-common-protos/google/logging/type/
--rw-r--r--   0 runner    (1001) docker     (122)     3389 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/logging/type/http_request.proto
--rw-r--r--   0 runner    (1001) docker     (122)     2508 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/logging/type/log_severity.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.245513 frequenz-api-common-0.2.0/submodules/api-common-protos/google/longrunning/
--rw-r--r--   0 runner    (1001) docker     (122)    10515 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/longrunning/operations.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.245513 frequenz-api-common-0.2.0/submodules/api-common-protos/google/rpc/
--rw-r--r--   0 runner    (1001) docker     (122)     7125 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/rpc/code.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.245513 frequenz-api-common-0.2.0/submodules/api-common-protos/google/rpc/context/
--rw-r--r--   0 runner    (1001) docker     (122)    12015 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/rpc/context/attribute_context.proto
--rw-r--r--   0 runner    (1001) docker     (122)     9504 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/rpc/error_details.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1924 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/rpc/status.proto
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 11:39:02.245513 frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/
--rw-r--r--   0 runner    (1001) docker     (122)     1766 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/calendar_period.proto
--rw-r--r--   0 runner    (1001) docker     (122)     6193 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/color.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/date.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3508 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/datetime.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/dayofweek.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1834 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/expr.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1176 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/fraction.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1447 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/latlng.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1603 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/money.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1482 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/month.proto
--rw-r--r--   0 runner    (1001) docker     (122)     6239 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/postal_address.proto
--rw-r--r--   0 runner    (1001) docker     (122)     3795 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/quaternion.proto
--rw-r--r--   0 runner    (1001) docker     (122)     1668 2023-05-23 11:38:45.000000 frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/timeofday.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.612018 frequenz-api-common-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      281 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (122)     2263 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1090 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      203 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-06-06 09:33:28.608018 frequenz-api-common-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2415 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/RELEASE_NOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.600018 frequenz-api-common-0.3.0/proto/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.600018 frequenz-api-common-0.3.0/proto/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.600018 frequenz-api-common-0.3.0/proto/frequenz/api/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.604018 frequenz-api-common-0.3.0/proto/frequenz/api/common/
+-rw-r--r--   0 runner    (1001) docker     (122)     2864 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/proto/frequenz/api/common/components.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.604018 frequenz-api-common-0.3.0/proto/frequenz/api/common/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)     6145 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/proto/frequenz/api/common/metrics/electrical.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     7405 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/proto/frequenz/api/common/metrics.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.600018 frequenz-api-common-0.3.0/py/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.600018 frequenz-api-common-0.3.0/py/frequenz/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.600018 frequenz-api-common-0.3.0/py/frequenz/api/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.604018 frequenz-api-common-0.3.0/py/frequenz/api/common/
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/py/frequenz/api/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.604018 frequenz-api-common-0.3.0/py/frequenz/api/common/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)      121 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/py/frequenz/api/common/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/py/frequenz/api/common/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.604018 frequenz-api-common-0.3.0/py/frequenz_api_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-06-06 09:33:28.000000 frequenz-api-common-0.3.0/py/frequenz_api_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3704 2023-06-06 09:33:28.000000 frequenz-api-common-0.3.0/py/frequenz_api_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-06 09:33:28.000000 frequenz-api-common-0.3.0/py/frequenz_api_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      485 2023-06-06 09:33:28.000000 frequenz-api-common-0.3.0/py/frequenz_api_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-06 09:33:28.000000 frequenz-api-common-0.3.0/py/frequenz_api_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2030 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-06 09:33:28.612018 frequenz-api-common-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.600018 frequenz-api-common-0.3.0/submodules/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.600018 frequenz-api-common-0.3.0/submodules/api-common-protos/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.600018 frequenz-api-common-0.3.0/submodules/api-common-protos/google/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.608018 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/annotations.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     7374 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/auth.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/backend.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2504 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/billing.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3392 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/client.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3169 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/config_change.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2719 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/consumer.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2008 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/context.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1225 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/control.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     8657 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/distribution.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     6132 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/documentation.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2824 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/endpoint.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3318 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/field_behavior.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    12099 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/http.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2605 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/httpbody.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1391 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/label.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2910 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/launch_stage.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2045 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/log.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3209 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/logging.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     6628 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/metric.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     5512 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/monitored_resource.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3524 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/monitoring.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    10854 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/quota.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    11347 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/resource.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    14929 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/routing.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     6099 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/service.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1093 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/source_info.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3472 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/system_parameter.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3513 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/usage.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.608018 frequenz-api-common-0.3.0/submodules/api-common-protos/google/cloud/
+-rw-r--r--   0 runner    (1001) docker     (122)     6308 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/cloud/extended_operations.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.600018 frequenz-api-common-0.3.0/submodules/api-common-protos/google/iam/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.600018 frequenz-api-common-0.3.0/submodules/api-common-protos/google/iam/admin/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.608018 frequenz-api-common-0.3.0/submodules/api-common-protos/google/iam/admin/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)    41483 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/iam/admin/v1/iam.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.608018 frequenz-api-common-0.3.0/submodules/api-common-protos/google/iam/v1/
+-rw-r--r--   0 runner    (1001) docker     (122)     5482 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/iam/v1/iam_policy.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.608018 frequenz-api-common-0.3.0/submodules/api-common-protos/google/iam/v1/logging/
+-rw-r--r--   0 runner    (1001) docker     (122)     1287 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1470 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/iam/v1/options.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     8659 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/iam/v1/policy.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.600018 frequenz-api-common-0.3.0/submodules/api-common-protos/google/logging/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.608018 frequenz-api-common-0.3.0/submodules/api-common-protos/google/logging/type/
+-rw-r--r--   0 runner    (1001) docker     (122)     3389 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/logging/type/http_request.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     2508 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/logging/type/log_severity.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.608018 frequenz-api-common-0.3.0/submodules/api-common-protos/google/longrunning/
+-rw-r--r--   0 runner    (1001) docker     (122)    10515 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/longrunning/operations.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.608018 frequenz-api-common-0.3.0/submodules/api-common-protos/google/rpc/
+-rw-r--r--   0 runner    (1001) docker     (122)     7125 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/rpc/code.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.608018 frequenz-api-common-0.3.0/submodules/api-common-protos/google/rpc/context/
+-rw-r--r--   0 runner    (1001) docker     (122)    12015 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/rpc/context/attribute_context.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     9504 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/rpc/error_details.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1924 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/rpc/status.proto
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-06 09:33:28.608018 frequenz-api-common-0.3.0/submodules/api-common-protos/google/type/
+-rw-r--r--   0 runner    (1001) docker     (122)     1766 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/type/calendar_period.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     6193 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/type/color.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1933 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/type/date.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3508 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/type/datetime.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1337 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/type/dayofweek.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1834 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/type/expr.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1176 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/type/fraction.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1447 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/type/latlng.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1603 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/type/money.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1482 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/type/month.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     6239 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/type/postal_address.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     3795 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/type/quaternion.proto
+-rw-r--r--   0 runner    (1001) docker     (122)     1668 2023-06-06 09:33:11.000000 frequenz-api-common-0.3.0/submodules/api-common-protos/google/type/timeofday.proto
```

### Comparing `frequenz-api-common-0.2.0/CONTRIBUTING.md` & `frequenz-api-common-0.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/LICENSE` & `frequenz-api-common-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/PKG-INFO` & `frequenz-api-common-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-api-common
-Version: 0.2.0
+Version: 0.3.0
 Summary: Frequenz common gRPC API and bindings
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-api-common/releases
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-api-common
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-api-common/issues
 Project-URL: Support, https://github.com/frequenz-floss/frequenz-api-common/discussions/categories/support
```

### Comparing `frequenz-api-common-0.2.0/proto/frequenz/api/common/components.proto` & `frequenz-api-common-0.3.0/proto/frequenz/api/common/components.proto`

 * *Files 1% similar despite different names*

```diff
@@ -71,26 +71,26 @@
   INVERTER_TYPE_SOLAR = 2;
 
   // Hybrid inverter.
   INVERTER_TYPE_HYBRID = 3;
 }
 
 // Enumerated EV charger types.
-enum EVChargerType {
+enum EvChargerType {
   // Default type.
-  EVCHARGER_TYPE_UNSPECIFIED = 0;
+  EV_CHARGER_TYPE_UNSPECIFIED = 0;
 
   // The EV charging station supports AC charging only.
-  EVCHARGER_TYPE_AC = 1;
+  EV_CHARGER_TYPE_AC = 1;
 
   // The EV charging station supports DC charging only.
-  EVCHARGER_TYPE_DC = 2;
+  EV_CHARGER_TYPE_DC = 2;
 
   // The EV charging station supports both AC and DC.
-  EVCHARGER_TYPE_HYBRID = 3;
+  EV_CHARGER_TYPE_HYBRID = 3;
 }
 
 // Enumerated sensor types.
 enum SensorType {
   // Unspecified
   SENSOR_TYPE_UNSPECIFIED = 0;
```

### Comparing `frequenz-api-common-0.2.0/proto/frequenz/api/common/metrics/electrical.proto` & `frequenz-api-common-0.3.0/proto/frequenz/api/common/metrics/electrical.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/proto/frequenz/api/common/metrics.proto` & `frequenz-api-common-0.3.0/proto/frequenz/api/common/metrics.proto`

 * *Files 25% similar despite different names*

```diff
@@ -86,7 +86,93 @@
   // <-------|============|------------------|============|--------->
   //                exclusion.lower    exclusion.upper
   // ```
   // ---- values here are disallowed and wil be rejected
   // ==== vales here are allowed and will be accepted
   Bounds system_inclusion_bounds = 5;
 }
+
+// Metrics depicted as a collection of statistical summaries.
+//
+// Useful when a component has to report multiple values for the same metric.
+// E.g., a battery is a collection of several blocks, and each block has a
+// temperature sensor. The battery can report a summary of the values provided
+// by all these sensors, like, min, max, avg, etc., and if possible, the entire
+// array of temperature values.
+message MetricAggregation {
+  // The average value of the metric.
+  float avg = 1;
+
+  // The minimum value of the metric.
+  optional float min = 2;
+
+  // The maximum value of the metric.
+  optional float max = 3;
+
+  // The array of all the metric values.
+  repeated float raw_values = 12;
+
+  // The manufacturer's rated bounds of the metric. This may differ from
+  // `system_bounds` as it does not take into account the current state of the
+  // overall system.
+  frequenz.api.common.metrics.Bounds rated_bounds = 13;
+
+  // The current bounds of the metric, as imposed by the component this metric
+  // originates from.
+  frequenz.api.common.metrics.Bounds component_bounds = 14;
+
+  // These bounds indicate the range of values that are disallowed for the
+  // metric.
+  // If these bounds for a metric are [`lower`, `upper`], then this metric's
+  // `value` needs to comply with the constraints
+  // `value <= lower` OR `upper <= value`.
+  //
+  // It is important to note that these bounds work together with
+  // `system_inclusion_bounds`.
+  //
+  // E.g., for the system to accept a charge command,
+  // clients need to request power values within the bounds
+  // `[system_inclusion_bounds.lower, system_exclusion_bounds.lower]`.
+  // This means that clients can only request charge commands with power values
+  // that are within the `system_inclusion_bounds`, but not within
+  // `system_exclusion_bounds`.
+  // Similarly, for the system to accept a discharge command,
+  // clients need to request power values within the bounds
+  // `[system_exclusion_bounds.upper, system_inclusion_bounds.upper]`.
+  //
+  // The following diagram illustrates the relationship between the bounds.
+  // ```
+  //   inclusion.lower                              inclusion.upper
+  // <-------|============|------------------|============|--------->
+  //                exclusion.lower    exclusion.upper
+  // ```
+  // ---- values here are disallowed and wil be rejected
+  // ==== vales here are allowed and will be accepted
+  frequenz.api.common.metrics.Bounds system_exclusion_bounds = 4;
+
+  // These bounds indicate the range of values that are allowed for the metric.
+  // If these bounds for a metric are [`lower`, `upper`], then this metric's
+  // `value` needs to comply with the constraint `lower <= value <= upper`
+  //
+  // It is important to note that these bounds work together with
+  // `system_exclusion_bounds`.
+  //
+  // E.g., for the system to accept a charge command,
+  // clients need to request power values within the bounds
+  // `[system_inclusion_bounds.lower, system_exclusion_bounds.lower]`.
+  // This means that clients can only request charge commands with power values
+  // that are within the `system_inclusion_bounds`, but not within
+  // `system_exclusion_bounds`.
+  // Similarly, for the system to accept a discharge command,
+  // clients need to request power values within the bounds
+  // `[system_exclusion_bounds.upper, system_inclusion_bounds.upper]`.
+  //
+  // The following diagram illustrates the relationship between the bounds.
+  // ```
+  //   inclusion.lower                              inclusion.upper
+  // <-------|============|------------------|============|--------->
+  //                exclusion.lower    exclusion.upper
+  // ```
+  // ---- values here are disallowed and wil be rejected
+  // ==== vales here are allowed and will be accepted
+  frequenz.api.common.metrics.Bounds system_inclusion_bounds = 5;
+}
```

### Comparing `frequenz-api-common-0.2.0/py/frequenz_api_common.egg-info/PKG-INFO` & `frequenz-api-common-0.3.0/py/frequenz_api_common.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frequenz-api-common
-Version: 0.2.0
+Version: 0.3.0
 Summary: Frequenz common gRPC API and bindings
 Author-email: Frequenz Energy-as-a-Service GmbH <floss@frequenz.com>
 License: MIT
 Project-URL: Changelog, https://github.com/frequenz-floss/frequenz-api-common/releases
 Project-URL: Repository, https://github.com/frequenz-floss/frequenz-api-common
 Project-URL: Issues, https://github.com/frequenz-floss/frequenz-api-common/issues
 Project-URL: Support, https://github.com/frequenz-floss/frequenz-api-common/discussions/categories/support
```

### Comparing `frequenz-api-common-0.2.0/py/frequenz_api_common.egg-info/SOURCES.txt` & `frequenz-api-common-0.3.0/py/frequenz_api_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/pyproject.toml` & `frequenz-api-common-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [build-system]
 requires = [
   "setuptools == 67.7.2",
   "setuptools_scm[toml] == 7.1.0",
-  "frequenz-repo-config[api] == 0.1.0",
+  "frequenz-repo-config[api] == 0.2.0",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "frequenz-api-common"
 description = "Frequenz common gRPC API and bindings"
 readme = "README.md"
@@ -35,15 +35,15 @@
 dev-docstrings = ["pydocstyle == 6.3.0", "darglint == 1.8.1"]
 dev-formatting = ["black == 23.3.0", "isort == 5.12.0"]
 dev-mypy = [
   "mypy == 1.3.0",
   # For checking the noxfile and tests
   "frequenz-api-common[dev-noxfile,dev-pytest]",
 ]
-dev-noxfile = ["nox == 2023.4.22", "frequenz-repo-config[api] == 0.1.0"]
+dev-noxfile = ["nox == 2023.4.22", "frequenz-repo-config[api] == 0.2.0"]
 dev-pylint = [
   "pylint == 2.17.4",
   # For checking the noxfile and tests
   "frequenz-api-common[dev-noxfile,dev-pytest]",
 ]
 dev-pytest = ["pytest == 7.3.1"]
 dev = [
```

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/annotations.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/annotations.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/auth.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/auth.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/backend.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/backend.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/billing.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/billing.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/client.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/client.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/config_change.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/config_change.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/consumer.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/consumer.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/context.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/context.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/control.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/control.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/distribution.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/distribution.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/documentation.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/documentation.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/endpoint.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/endpoint.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/field_behavior.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/field_behavior.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/http.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/http.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/httpbody.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/httpbody.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/label.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/label.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/launch_stage.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/launch_stage.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/log.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/log.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/logging.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/logging.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/metric.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/metric.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/monitored_resource.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/monitored_resource.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/monitoring.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/monitoring.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/quota.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/quota.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/resource.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/resource.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/routing.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/routing.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/service.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/service.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/source_info.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/source_info.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/system_parameter.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/system_parameter.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/api/usage.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/api/usage.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/cloud/extended_operations.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/cloud/extended_operations.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/iam/admin/v1/iam.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/iam/admin/v1/iam.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/iam/v1/iam_policy.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/iam/v1/iam_policy.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/iam/v1/logging/audit_data.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/iam/v1/options.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/iam/v1/options.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/iam/v1/policy.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/iam/v1/policy.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/logging/type/http_request.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/logging/type/http_request.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/logging/type/log_severity.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/logging/type/log_severity.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/longrunning/operations.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/longrunning/operations.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/rpc/code.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/rpc/code.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/rpc/context/attribute_context.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/rpc/context/attribute_context.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/rpc/error_details.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/rpc/error_details.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/rpc/status.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/rpc/status.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/calendar_period.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/type/calendar_period.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/color.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/type/color.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/date.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/type/date.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/datetime.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/type/datetime.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/dayofweek.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/type/dayofweek.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/expr.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/type/expr.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/fraction.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/type/fraction.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/latlng.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/type/latlng.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/money.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/type/money.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/month.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/type/month.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/postal_address.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/type/postal_address.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/quaternion.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/type/quaternion.proto`

 * *Files identical despite different names*

### Comparing `frequenz-api-common-0.2.0/submodules/api-common-protos/google/type/timeofday.proto` & `frequenz-api-common-0.3.0/submodules/api-common-protos/google/type/timeofday.proto`

 * *Files identical despite different names*

