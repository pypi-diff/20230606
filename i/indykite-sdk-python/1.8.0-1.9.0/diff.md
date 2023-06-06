# Comparing `tmp/indykite-sdk-python-1.8.0.tar.gz` & `tmp/indykite-sdk-python-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indykite-sdk-python-1.8.0.tar", last modified: Thu Jan  5 16:12:00 2023, max compression
+gzip compressed data, was "indykite-sdk-python-1.9.0.tar", last modified: Thu Jan 12 15:06:55 2023, max compression
```

## Comparing `indykite-sdk-python-1.8.0.tar` & `indykite-sdk-python-1.9.0.tar`

### file list

```diff
@@ -1,181 +1,186 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 16:12:00.874698 indykite-sdk-python-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    61575 2023-01-05 16:12:00.874698 indykite-sdk-python-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    55783 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 16:12:00.858698 indykite-sdk-python-1.8.0/indykite_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    78043 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 16:12:00.858698 indykite-sdk-python-1.8.0/indykite_sdk/config/
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/config/app_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/config/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/config/application_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/config/application_agent_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/config/config_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/config/customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/config/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/config/oauth2_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/config/oauth2_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/config/service_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/config/service_account_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/config/tenant.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 16:12:00.858698 indykite-sdk-python-1.8.0/indykite_sdk/identity/
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/identity/change_password.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/identity/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/identity/enrich_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/identity/get_digital_twin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/identity/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/identity/introspect_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/identity/patch_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/identity/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 16:12:00.858698 indykite-sdk-python-1.8.0/indykite_sdk/indykite/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 16:12:00.858698 indykite-sdk-python-1.8.0/indykite_sdk/indykite/authorization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/authorization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 16:12:00.858698 indykite-sdk-python-1.8.0/indykite_sdk/indykite/authorization/v1beta1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/authorization/v1beta1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/authorization/v1beta1/authorization_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/authorization/v1beta1/authorization_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 16:12:00.858698 indykite-sdk-python-1.8.0/indykite_sdk/indykite/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 16:12:00.862698 indykite-sdk-python-1.8.0/indykite_sdk/indykite/config/v1beta1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/config/v1beta1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   147659 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/config/v1beta1/config_management_api_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    95947 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/config/v1beta1/config_management_api_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)   113711 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/config/v1beta1/model_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/config/v1beta1/model_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 16:12:00.862698 indykite-sdk-python-1.8.0/indykite_sdk/indykite/events/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/events/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 16:12:00.862698 indykite-sdk-python-1.8.0/indykite_sdk/indykite/events/v1beta1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/events/v1beta1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29147 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/events/v1beta1/events_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/events/v1beta1/events_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 16:12:00.862698 indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 16:12:00.862698 indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta1/attributes_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta1/attributes_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta1/authenteq_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta1/authenteq_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta1/document_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta1/document_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    76624 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta1/identity_management_api_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    62603 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta1/identity_management_api_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21517 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta1/import_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta1/import_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    24034 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta1/model_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta1/model_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 16:12:00.866698 indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta2/attributes_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta2/attributes_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta2/authenteq_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta2/authenteq_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta2/consent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta2/consent_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta2/document_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta2/document_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    84560 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta2/identity_management_api_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta2/identity_management_api_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21668 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta2/import_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta2/import_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    24404 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta2/model_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta2/model_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta2/readid_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta2/readid_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 16:12:00.866698 indykite-sdk-python-1.8.0/indykite_sdk/indykite/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/ingest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 16:12:00.866698 indykite-sdk-python-1.8.0/indykite_sdk/indykite/ingest/v1beta1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/ingest/v1beta1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/ingest/v1beta1/ingest_api_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/ingest/v1beta1/ingest_api_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/ingest/v1beta1/model_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/ingest/v1beta1/model_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 16:12:00.866698 indykite-sdk-python-1.8.0/indykite_sdk/indykite/knowledge_graph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/knowledge_graph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 16:12:00.866698 indykite-sdk-python-1.8.0/indykite_sdk/indykite/knowledge_graph/v1beta1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/knowledge_graph/v1beta1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10025 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/knowledge_graph/v1beta1/policy_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/knowledge_graph/v1beta1/policy_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/knowledge_graph/v1beta1/schema_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/knowledge_graph/v1beta1/schema_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 16:12:00.866698 indykite-sdk-python-1.8.0/indykite_sdk/indykite/objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/objects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 16:12:00.866698 indykite-sdk-python-1.8.0/indykite_sdk/indykite/objects/v1beta1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/objects/v1beta1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/objects/v1beta1/id_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/objects/v1beta1/id_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/objects/v1beta1/struct_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/indykite/objects/v1beta1/struct_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 16:12:00.866698 indykite-sdk-python-1.8.0/indykite_sdk/ingest/
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/ingest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 16:12:00.870698 indykite-sdk-python-1.8.0/indykite_sdk/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/app_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/application_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/application_agent_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/auth_flow_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/config_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/create_app_space.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/create_application.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/create_application_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/create_config_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/create_oauth2_application.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/create_oauth2_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/create_service_account.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/create_tenant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/digital_twin.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/email.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/email_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/email_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/email_service_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/email_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/ingest_mapping_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/oauth2_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/oauth2_application_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/oauth2_client_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/oauth2_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/oauth2_provider_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/postal_address.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/property.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/provider_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/register_application_agent_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/register_service_account_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/sendgrid_email_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/service_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/service_account_credential.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/tenant.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/token_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/unique_name_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/update_app_space.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/update_application.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/update_application_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/update_config_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/update_oauth2_application.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/update_oauth2_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/update_service_account.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/model/update_tenant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 16:12:00.870698 indykite-sdk-python-1.8.0/indykite_sdk/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/utils/deserialize_digital_twin_with_token_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/utils/message_to_value.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 16:12:00.870698 indykite-sdk-python-1.8.0/indykite_sdk/validate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23634 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/validate/validate_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/indykite_sdk/validate/validate_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 16:12:00.874698 indykite-sdk-python-1.8.0/indykite_sdk_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    61575 2023-01-05 16:12:00.000000 indykite-sdk-python-1.8.0/indykite_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-01-05 16:12:00.000000 indykite-sdk-python-1.8.0/indykite_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 16:12:00.000000 indykite-sdk-python-1.8.0/indykite_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-01-05 16:12:00.000000 indykite-sdk-python-1.8.0/indykite_sdk_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-05 16:12:00.000000 indykite-sdk-python-1.8.0/indykite_sdk_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-05 16:12:00.874698 indykite-sdk-python-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-05 16:11:47.000000 indykite-sdk-python-1.8.0/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:54.996718 indykite-sdk-python-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    62330 2023-01-12 15:06:54.996718 indykite-sdk-python-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    56140 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:54.976716 indykite-sdk-python-1.9.0/indykite_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82772 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:54.976716 indykite-sdk-python-1.9.0/indykite_sdk/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/config/app_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/config/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/config/application_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/config/application_agent_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7324 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/config/config_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/config/customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/config/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/config/oauth2_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/config/oauth2_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/config/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/config/service_account_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/config/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:54.976716 indykite-sdk-python-1.9.0/indykite_sdk/identity/
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/identity/change_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/identity/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/identity/enrich_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/identity/get_digital_twin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/identity/helper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6031 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/identity/import_digital_twins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/identity/introspect_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/identity/patch_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/identity/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:54.976716 indykite-sdk-python-1.9.0/indykite_sdk/indykite/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:54.980716 indykite-sdk-python-1.9.0/indykite_sdk/indykite/authorization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/authorization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:54.980716 indykite-sdk-python-1.9.0/indykite_sdk/indykite/authorization/v1beta1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/authorization/v1beta1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8655 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/authorization/v1beta1/authorization_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/authorization/v1beta1/authorization_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:54.980716 indykite-sdk-python-1.9.0/indykite_sdk/indykite/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:54.980716 indykite-sdk-python-1.9.0/indykite_sdk/indykite/config/v1beta1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/config/v1beta1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   147659 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/config/v1beta1/config_management_api_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95947 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/config/v1beta1/config_management_api_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113711 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/config/v1beta1/model_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/config/v1beta1/model_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:54.980716 indykite-sdk-python-1.9.0/indykite_sdk/indykite/events/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/events/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:54.980716 indykite-sdk-python-1.9.0/indykite_sdk/indykite/events/v1beta1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/events/v1beta1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29147 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/events/v1beta1/events_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/events/v1beta1/events_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:54.980716 indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:54.984717 indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta1/attributes_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta1/attributes_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta1/authenteq_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta1/authenteq_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta1/document_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta1/document_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76624 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta1/identity_management_api_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62603 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta1/identity_management_api_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21517 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta1/import_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta1/import_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24034 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta1/model_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta1/model_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:54.984717 indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta2/attributes_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta2/attributes_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta2/authenteq_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta2/authenteq_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta2/consent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta2/consent_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta2/document_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta2/document_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84560 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta2/identity_management_api_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta2/identity_management_api_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21668 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta2/import_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta2/import_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24404 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta2/model_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta2/model_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta2/readid_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta2/readid_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:54.984717 indykite-sdk-python-1.9.0/indykite_sdk/indykite/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/ingest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:54.988717 indykite-sdk-python-1.9.0/indykite_sdk/indykite/ingest/v1beta1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/ingest/v1beta1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/ingest/v1beta1/ingest_api_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/ingest/v1beta1/ingest_api_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5470 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/ingest/v1beta1/model_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/ingest/v1beta1/model_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:54.988717 indykite-sdk-python-1.9.0/indykite_sdk/indykite/knowledge_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/knowledge_graph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:54.988717 indykite-sdk-python-1.9.0/indykite_sdk/indykite/knowledge_graph/v1beta1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/knowledge_graph/v1beta1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10025 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/knowledge_graph/v1beta1/policy_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/knowledge_graph/v1beta1/policy_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/knowledge_graph/v1beta1/schema_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/knowledge_graph/v1beta1/schema_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:54.988717 indykite-sdk-python-1.9.0/indykite_sdk/indykite/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/objects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:54.988717 indykite-sdk-python-1.9.0/indykite_sdk/indykite/objects/v1beta1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/objects/v1beta1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/objects/v1beta1/id_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/objects/v1beta1/id_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/objects/v1beta1/struct_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/indykite/objects/v1beta1/struct_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:54.988717 indykite-sdk-python-1.9.0/indykite_sdk/ingest/
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/ingest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:54.996718 indykite-sdk-python-1.9.0/indykite_sdk/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/app_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/application_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/application_agent_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/auth_flow_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/config_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/create_app_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/create_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/create_application_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/create_config_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/create_oauth2_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/create_oauth2_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/create_service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/create_tenant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/digital_twin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/digital_twin_kind.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/digital_twin_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/email_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/email_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/email_service_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/email_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/import_digital_twin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/ingest_mapping_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/oauth2_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/oauth2_application_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/oauth2_client_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/oauth2_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/oauth2_provider_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/postal_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/provider_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/register_application_agent_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/register_service_account_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/sendgrid_email_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/service_account_credential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/token_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/unique_name_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/update_app_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/update_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/update_application_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/update_config_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/update_oauth2_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/update_oauth2_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/update_service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/model/update_tenant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:54.996718 indykite-sdk-python-1.9.0/indykite_sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/utils/deserialize_digital_twin_with_token_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/utils/hash_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/utils/message_to_value.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:54.996718 indykite-sdk-python-1.9.0/indykite_sdk/validate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23634 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/validate/validate_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/indykite_sdk/validate/validate_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:06:54.996718 indykite-sdk-python-1.9.0/indykite_sdk_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    62330 2023-01-12 15:06:54.000000 indykite-sdk-python-1.9.0/indykite_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-01-12 15:06:54.000000 indykite-sdk-python-1.9.0/indykite_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 15:06:54.000000 indykite-sdk-python-1.9.0/indykite_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-01-12 15:06:54.000000 indykite-sdk-python-1.9.0/indykite_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-12 15:06:54.000000 indykite-sdk-python-1.9.0/indykite_sdk_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-12 15:06:54.996718 indykite-sdk-python-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-12 15:06:22.000000 indykite-sdk-python-1.9.0/version.py
```

### Comparing `indykite-sdk-python-1.8.0/CHANGELOG.md` & `indykite-sdk-python-1.9.0/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Changelog
 
+## [1.9.0](https://github.com/indykite/indykite-sdk-python/compare/v1.8.0...v1.9.0) (2023-01-12)
+
+
+### Features
+
+* add import DT and update tests ([ca30bd0](https://github.com/indykite/indykite-sdk-python/commit/ca30bd07503290089f599c3c34bee453dc846822))
+* add import DT and update tests ([c1c954f](https://github.com/indykite/indykite-sdk-python/commit/c1c954f553e6cc10d222459dbd2371fb4100c8d8))
+
 ## [1.8.0](https://github.com/indykite/indykite-sdk-python/compare/v1.7.0...v1.8.0) (2023-01-05)
 
 
 ### Features
 
 * add missing init files ([cf0d5dd](https://github.com/indykite/indykite-sdk-python/commit/cf0d5dd0b7fce45e5b64f33e4566a4690764d250))
```

### Comparing `indykite-sdk-python-1.8.0/LICENSE` & `indykite-sdk-python-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/PKG-INFO` & `indykite-sdk-python-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indykite-sdk-python
-Version: 1.8.0
+Version: 1.9.0
 Summary: A python SDK package for Indykite's system (with protobuf)
 Home-page: https://github.com/indykite/indykite-sdk-python
 Author: Indykite
 Author-email: test@indykite.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,19 +13,19 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # IndyKite Python SDK 🐍
 
 This project serves as a Software Development Kit for developers of Indykite applications.
 
-[![codecov](https://codecov.io/gh/indykite/jarvis-sdk-python/branch/master/graph/badge.svg)](https://codecov.io/gh/indykite/indykite-sdk-python)
+[![codecov](https://codecov.io/gh/indykite/indykite-sdk-python/branch/master/graph/badge.svg)](https://codecov.io/gh/indykite/indykite-sdk-python)
 
 ## Requirements
 
-* Python 3.8
+* Python 3.11
 * [Buf](https://github.com/bufbuild/buf)
 
 ## Installation
 
 * Create virtual env and install dependencies
 
         pipenv install
@@ -1283,15 +1283,15 @@
             bookmarks)
 
     print(update_ingest_mapping_config_node_response)
 ```
 
 ### Get OAuth2 provider information
 
-In an Apppace, you can create OAuth2 providers.
+In an Appspace, you can create OAuth2 providers.
 An OAuth2 service provider is a named set of configuration options for OAuth2. 
 
 #### Read OAuth2 provider
 ```python
 from indykite_sdk.config import ConfigClient
 
 def get_oauth2_provider(self, local, oauth2_provider_id, bookmarks):
@@ -1395,17 +1395,36 @@
 
 def delete_oauth2_application(self, local, oauth2_application_id, etag, bookmarks):
     client_config = ConfigClient(local)
     config = client_config.delete_oauth2_application(oauth2_application_id, etag, bookmarks)
     print(config)
 ```
 
+### Import digital twins
+```python
+from indykite_sdk.indykite.identity.v1beta2.import_pb2 import ImportDigitalTwin
+from indykite_sdk.identity import IdentityClient
+
+def import_digital_twins(self, local, entities, hash_algorithm):
+  client = IdentityClient(local)
+  response = client.import_digital_twins(entities, hash_algorithm)
+  print(response)
+```
+
 
 # Changelog
 
+## [1.9.0](https://github.com/indykite/indykite-sdk-python/compare/v1.8.0...v1.9.0) (2023-01-12)
+
+
+### Features
+
+* add import DT and update tests ([ca30bd0](https://github.com/indykite/indykite-sdk-python/commit/ca30bd07503290089f599c3c34bee453dc846822))
+* add import DT and update tests ([c1c954f](https://github.com/indykite/indykite-sdk-python/commit/c1c954f553e6cc10d222459dbd2371fb4100c8d8))
+
 ## [1.8.0](https://github.com/indykite/indykite-sdk-python/compare/v1.7.0...v1.8.0) (2023-01-05)
 
 
 ### Features
 
 * add missing init files ([cf0d5dd](https://github.com/indykite/indykite-sdk-python/commit/cf0d5dd0b7fce45e5b64f33e4566a4690764d250))
```

### Comparing `indykite-sdk-python-1.8.0/README.md` & `indykite-sdk-python-1.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # IndyKite Python SDK 🐍
 
 This project serves as a Software Development Kit for developers of Indykite applications.
 
-[![codecov](https://codecov.io/gh/indykite/jarvis-sdk-python/branch/master/graph/badge.svg)](https://codecov.io/gh/indykite/indykite-sdk-python)
+[![codecov](https://codecov.io/gh/indykite/indykite-sdk-python/branch/master/graph/badge.svg)](https://codecov.io/gh/indykite/indykite-sdk-python)
 
 ## Requirements
 
-* Python 3.8
+* Python 3.11
 * [Buf](https://github.com/bufbuild/buf)
 
 ## Installation
 
 * Create virtual env and install dependencies
 
         pipenv install
@@ -1268,15 +1268,15 @@
             bookmarks)
 
     print(update_ingest_mapping_config_node_response)
 ```
 
 ### Get OAuth2 provider information
 
-In an Apppace, you can create OAuth2 providers.
+In an Appspace, you can create OAuth2 providers.
 An OAuth2 service provider is a named set of configuration options for OAuth2. 
 
 #### Read OAuth2 provider
 ```python
 from indykite_sdk.config import ConfigClient
 
 def get_oauth2_provider(self, local, oauth2_provider_id, bookmarks):
@@ -1379,7 +1379,18 @@
 from indykite_sdk.config import ConfigClient
 
 def delete_oauth2_application(self, local, oauth2_application_id, etag, bookmarks):
     client_config = ConfigClient(local)
     config = client_config.delete_oauth2_application(oauth2_application_id, etag, bookmarks)
     print(config)
 ```
+
+### Import digital twins
+```python
+from indykite_sdk.indykite.identity.v1beta2.import_pb2 import ImportDigitalTwin
+from indykite_sdk.identity import IdentityClient
+
+def import_digital_twins(self, local, entities, hash_algorithm):
+  client = IdentityClient(local)
+  response = client.import_digital_twins(entities, hash_algorithm)
+  print(response)
+```
```

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/api.py` & `indykite-sdk-python-1.9.0/indykite_sdk/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,25 +4,27 @@
 import argparse
 import base64
 import json
 from datetime import datetime
 from uuid import UUID
 from google.protobuf.json_format import MessageToJson
 
+from indykite_sdk.utils.hash_methods import encrypt_bcrypt, encrypt_sha256
 from indykite_sdk.identity import IdentityClient
 from indykite_sdk.config import ConfigClient
 from indykite_sdk.indykite.config.v1beta1.model_pb2 import (SendGridProviderConfig, MailJetProviderConfig, AmazonSESProviderConfig, MailgunProviderConfig)
 from indykite_sdk.indykite.config.v1beta1.model_pb2 import (EmailServiceConfig, AuthFlowConfig, OAuth2ClientConfig, IngestMappingConfig)
 from indykite_sdk.indykite.config.v1beta1.model_pb2 import OAuth2ProviderConfig, OAuth2ApplicationConfig
 from indykite_sdk.indykite.identity.v1beta2.import_pb2 import ImportDigitalTwinsRequest, ImportDigitalTwin
-from indykite_sdk.indykite.identity.v1beta2.import_pb2 import PasswordCredential, PasswordHash, Bcrypt
+from indykite_sdk.indykite.identity.v1beta2.import_pb2 import PasswordCredential, PasswordHash, Bcrypt, SHA256
 from indykite_sdk.indykite.config.v1beta1.model_pb2 import EmailAttachment, Email, EmailMessage, EmailTemplate, EmailDefinition
 from indykite_sdk.indykite.config.v1beta1.model_pb2 import google_dot_protobuf_dot_wrappers__pb2 as wrappers
 from indykite_sdk.indykite.identity.v1beta2.import_pb2 import Email as EmailIdentity
 
+
 class ParseKwargs(argparse.Action):
     def __call__(self, parser, namespace, values, option_string=None):  # pragma: no cover
         setattr(namespace, self.dest, dict())
         for value in values:
             key, value = value.split('=')
             getattr(namespace, self.dest)[key] = value
 
@@ -434,14 +436,28 @@
     # delete_oauth2_application
     delete_oauth2_application_parser = subparsers.add_parser("delete_oauth2_application")
     delete_oauth2_application_parser.add_argument("oauth2_application_id", help="OAuth2 application id (gid)")
     delete_oauth2_application_parser.add_argument("etag", help="Etag")
 
     # import_digital_twins
     import_digital_twins_parser = subparsers.add_parser("import_digital_twins")
+    import_digital_twins_parser.add_argument("tenant_id", help="Tenant id (gid)")
+
+    # import_digital_twins_hash
+    import_digital_twins_hash_parser = subparsers.add_parser("import_digital_twins_hash")
+    import_digital_twins_hash_parser.add_argument("tenant_id", help="Tenant id (gid)")
+
+    # import_digital_twins_hash256
+    import_digital_twins_hash256_parser = subparsers.add_parser("import_digital_twins_hash256")
+    import_digital_twins_hash256_parser.add_argument("tenant_id", help="Tenant id (gid)")
+
+    # import_digital_twins_update
+    import_digital_twins_update_parser = subparsers.add_parser("import_digital_twins_update")
+    import_digital_twins_update_parser.add_argument("id", help="Digital Twin id (gid)")
+    import_digital_twins_update_parser.add_argument("tenant_id", help="Tenant id (gid)")
 
     args = parser.parse_args()
     local = args.local
     client = IdentityClient(local)
     client_config = ConfigClient(local)
 
     command = args.command
@@ -1473,33 +1489,141 @@
             print_response(config)
         else:
             print("Invalid delete oauth2 application response")
 
     elif command == "import_digital_twins":
 
         entities = [ImportDigitalTwin(
-            tenant_id="696e6479-6b69-4465-8000-030f00000001",
+            tenant_id=args.tenant_id,
             kind="DIGITAL_TWIN_KIND_PERSON",
             state="DIGITAL_TWIN_STATE_ACTIVE",
             password=PasswordCredential(
                 email=EmailIdentity(
-                    email="test2000@example.com",
+                    email="test2101@example.com",
                     verified=True
                 ),
-                hash=PasswordHash(
-                    password_hash=bytes("$2y$10$k64jP7oqwYfQpzmoqAN5OuhrtWI2wICn0wXUzYxMp.UA1PopI653G", "utf-8")
+                value="password"
+            )
+        ),
+            ImportDigitalTwin(
+                tenant_id=args.tenant_id,
+                kind="DIGITAL_TWIN_KIND_PERSON",
+                state="DIGITAL_TWIN_STATE_ACTIVE",
+                password=PasswordCredential(
+                    email=EmailIdentity(
+                        email="test2102@example.com",
+                        verified=True
+                    ),
+                    value="password"
+                )
+            ),
+            ImportDigitalTwin(
+                tenant_id=args.tenant_id,
+                kind="DIGITAL_TWIN_KIND_PERSON",
+                state="DIGITAL_TWIN_STATE_ACTIVE",
+                password=PasswordCredential(
+                    email=EmailIdentity(
+                        email="test2104@example.com",
+                        verified=True
+                    ),
+                    value="password"
                 )
             )
+        ]
+        hash_algorithm = None
+
+        import_digital_twins_config_response = client.import_digital_twins(
+            entities, hash_algorithm)
+        if import_digital_twins_config_response:
+            for response in import_digital_twins_config_response:
+                print_response(response)
+        else:
+            print("Invalid import digital twins response")
+        return import_digital_twins_config_response
+
+    elif command == "import_digital_twins_hash":
+
+        password = 'passwordabc'
+        hash_dict = encrypt_bcrypt(password)
+        for key in hash_dict:
+            salt = key
+            hash_password = hash_dict[key]
+
+        entities = [ImportDigitalTwin(
+            tenant_id=args.tenant_id,
+            kind="DIGITAL_TWIN_KIND_PERSON",
+            state="DIGITAL_TWIN_STATE_ACTIVE",
+            password=PasswordCredential(
+                email=EmailIdentity(
+                    email="test2002@example.com",
+                    verified=True
+                ),
+                hash=PasswordHash(password_hash=hash_password,salt=salt)
+            )
+        )]
+        hash_algorithm = {"bcrypt": {}}
+
+        import_digital_twins_config_response = client.import_digital_twins(
+            entities, hash_algorithm)
+        if import_digital_twins_config_response:
+            for response in import_digital_twins_config_response:
+                print_response(response)
+        else:
+            print("Invalid import digital twins response")
+        return import_digital_twins_config_response
+
+    elif command == "import_digital_twins_hash256":
+
+        password = 'passwordabc'
+        hash_password = encrypt_sha256(password)
+
+        entities = [ImportDigitalTwin(
+            tenant_id=args.tenant_id,
+            kind="DIGITAL_TWIN_KIND_PERSON",
+            state="DIGITAL_TWIN_STATE_ACTIVE",
+            password=PasswordCredential(
+                email=EmailIdentity(
+                    email="test2002@example.com",
+                    verified=True
+                ),
+                hash=PasswordHash(password_hash=hash_password)
+            )
+        )]
+        hash_algorithm = {"sha256": SHA256(rounds=14)}
+
+        import_digital_twins_config_response = client.import_digital_twins(
+            entities, hash_algorithm)
+        if import_digital_twins_config_response:
+            for response in import_digital_twins_config_response:
+                print_response(response)
+        else:
+            print("Invalid import digital twins response")
+        return import_digital_twins_config_response
+
+    elif command == "import_digital_twins_update":
+        entities = [ImportDigitalTwin(
+            id=args.id,
+            tenant_id=args.tenant_id,
+            kind="DIGITAL_TWIN_KIND_PERSON",
+            state="DIGITAL_TWIN_STATE_ACTIVE",
+            password=PasswordCredential(
+                email=EmailIdentity(
+                    email="test2003@example.com",
+                    verified=True
+                ),
+                value="password"
+            )
         )]
-        hash_algorithm = Bcrypt()
+        hash_algorithm = None
 
         import_digital_twins_config_response = client.import_digital_twins(
-            entities,hash_algorithm)
+            entities, hash_algorithm)
         if import_digital_twins_config_response:
-            print_response(import_digital_twins_config_response)
+            for response in import_digital_twins_config_response:
+                print_response(response)
         else:
             print("Invalid import digital twins response")
         return import_digital_twins_config_response
 
 
 def print_verify_info(digital_twin_info):  # pragma: no cover
     print("Digital twin info")
```

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/config/__init__.py` & `indykite-sdk-python-1.9.0/indykite_sdk/config/__init__.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/config/app_space.py` & `indykite-sdk-python-1.9.0/indykite_sdk/config/app_space.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/config/application.py` & `indykite-sdk-python-1.9.0/indykite_sdk/config/application.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/config/application_agent.py` & `indykite-sdk-python-1.9.0/indykite_sdk/config/application_agent.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/config/application_agent_credential.py` & `indykite-sdk-python-1.9.0/indykite_sdk/config/application_agent_credential.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/config/config_node.py` & `indykite-sdk-python-1.9.0/indykite_sdk/config/config_node.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/config/customer.py` & `indykite-sdk-python-1.9.0/indykite_sdk/config/customer.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/config/helper.py` & `indykite-sdk-python-1.9.0/indykite_sdk/config/helper.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/config/oauth2_application.py` & `indykite-sdk-python-1.9.0/indykite_sdk/config/oauth2_application.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/config/oauth2_provider.py` & `indykite-sdk-python-1.9.0/indykite_sdk/config/oauth2_provider.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/config/service_account.py` & `indykite-sdk-python-1.9.0/indykite_sdk/config/service_account.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/config/service_account_credential.py` & `indykite-sdk-python-1.9.0/indykite_sdk/config/service_account_credential.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/config/tenant.py` & `indykite-sdk-python-1.9.0/indykite_sdk/config/tenant.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/example.py` & `indykite-sdk-python-1.9.0/indykite_sdk/example.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/identity/__init__.py` & `indykite-sdk-python-1.9.0/indykite_sdk/identity/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,7 +51,8 @@
     from .change_password import change_password_of_user, change_password
     from .get_digital_twin import get_digital_twin_by_token, get_digital_twin
     from .introspect_token import introspect_token
     from .patch_properties import patch_properties_by_token, patch_properties
     from .verification import start_digital_twin_email_verification, verify_digital_twin_email
     from .delete import del_digital_twin, del_digital_twin_by_token
     from .enrich_token import enrich_token
+    from .import_digital_twins import import_digital_twins
```

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/identity/change_password.py` & `indykite-sdk-python-1.9.0/indykite_sdk/identity/change_password.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/identity/delete.py` & `indykite-sdk-python-1.9.0/indykite_sdk/identity/delete.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/identity/enrich_token.py` & `indykite-sdk-python-1.9.0/indykite_sdk/identity/enrich_token.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/identity/get_digital_twin.py` & `indykite-sdk-python-1.9.0/indykite_sdk/identity/get_digital_twin.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/identity/helper.py` & `indykite-sdk-python-1.9.0/indykite_sdk/identity/helper.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/identity/patch_properties.py` & `indykite-sdk-python-1.9.0/indykite_sdk/identity/patch_properties.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/identity/verification.py` & `indykite-sdk-python-1.9.0/indykite_sdk/identity/verification.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/indykite/authorization/v1beta1/authorization_service_pb2.py` & `indykite-sdk-python-1.9.0/indykite_sdk/indykite/authorization/v1beta1/authorization_service_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from indykite_sdk.validate import validate_pb2 as validate_dot_validate__pb2
 from indykite_sdk.indykite.identity.v1beta2 import identity_management_api_pb2 as indykite_dot_identity_dot_v1beta2_dot_identity__management__api__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n:indykite/authorization/v1beta1/authorization_service.proto\x12\x1eindykite.authorization.v1beta1\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17validate/validate.proto\x1a\x37indykite/identity/v1beta2/identity_management_api.proto\"\xf7\x02\n\x13IsAuthorizedRequest\x12T\n\x07subject\x18\x01 \x01(\x0b\x32\x30.indykite.identity.v1beta2.DigitalTwinIdentifierB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01R\x07subject\x12\x66\n\tresources\x18\x02 \x03(\x0b\x32<.indykite.authorization.v1beta1.IsAuthorizedRequest.ResourceB\n\xfa\x42\x07\x92\x01\x04\x08\x01\x10 R\tresources\x12\x46\n\x07\x61\x63tions\x18\x03 \x03(\tB,\xfa\x42)\x92\x01&\x08\x01\x10\x01\" r\x1e\x10\x02\x18\x32\x32\x18^[a-zA-Z0-9.:_\\-\\/]{2,}$R\x07\x61\x63tions\x1aZ\n\x08Resource\x12\x19\n\x02id\x18\x01 \x01(\tB\t\xfa\x42\x06r\x04\x10\x02\x18\x32R\x02id\x12\x33\n\x05label\x18\x02 \x01(\tB\x1d\xfa\x42\x1ar\x18\x10\x02\x18\x32\x32\x12^(?:[A-Z][a-z]+)+$R\x05label\"\xaf\x02\n\x14IsAuthorizedResponse\x12?\n\rdecision_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0c\x64\x65\x63isionTime\x12\x61\n\tdecisions\x18\x02 \x03(\x0b\x32\x43.indykite.authorization.v1beta1.IsAuthorizedResponse.DecisionsEntryR\tdecisions\x1as\n\x0e\x44\x65\x63isionsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12K\n\x05value\x18\x02 \x01(\x0b\x32\x35.indykite.authorization.v1beta1.AuthorizationDecisionR\x05value:\x02\x38\x01\"\xc2\x01\n\x15\x41uthorizationDecision\x12i\n\x0c\x61llow_action\x18\x01 \x03(\x0b\x32\x46.indykite.authorization.v1beta1.AuthorizationDecision.AllowActionEntryR\x0b\x61llowAction\x1a>\n\x10\x41llowActionEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\x08R\x05value:\x02\x38\x01\x32\x8d\x01\n\x10\x41uthorizationAPI\x12y\n\x0cIsAuthorized\x12\x33.indykite.authorization.v1beta1.IsAuthorizedRequest\x1a\x34.indykite.authorization.v1beta1.IsAuthorizedResponseB\xd9\x01\n\"com.indykite.authorization.v1beta1B\x19\x41uthorizationServiceProtoP\x01\xa2\x02\x03IAX\xaa\x02\x1eIndykite.Authorization.V1beta1\xca\x02\x1eIndykite\\Authorization\\V1beta1\xe2\x02*Indykite\\Authorization\\V1beta1\\GPBMetadata\xea\x02 Indykite::Authorization::V1beta1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n:indykite/authorization/v1beta1/authorization_service.proto\x12\x1eindykite.authorization.v1beta1\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17validate/validate.proto\x1a\x37indykite/identity/v1beta2/identity_management_api.proto\"\xa7\x03\n\x13IsAuthorizedRequest\x12t\n\x17\x64igital_twin_identifier\x18\x01 \x01(\x0b\x32\x30.indykite.identity.v1beta2.DigitalTwinIdentifierB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01H\x00R\x15\x64igitalTwinIdentifier\x12\x66\n\tresources\x18\x02 \x03(\x0b\x32<.indykite.authorization.v1beta1.IsAuthorizedRequest.ResourceB\n\xfa\x42\x07\x92\x01\x04\x08\x01\x10 R\tresources\x12\x46\n\x07\x61\x63tions\x18\x03 \x03(\tB,\xfa\x42)\x92\x01&\x08\x01\x10\x01\" r\x1e\x10\x02\x18\x32\x32\x18^[a-zA-Z0-9.:_\\-\\/]{2,}$R\x07\x61\x63tions\x1aZ\n\x08Resource\x12\x19\n\x02id\x18\x01 \x01(\tB\t\xfa\x42\x06r\x04\x10\x02\x18\x32R\x02id\x12\x33\n\x05label\x18\x02 \x01(\tB\x1d\xfa\x42\x1ar\x18\x10\x02\x18\x32\x32\x12^(?:[A-Z][a-z]+)+$R\x05labelB\x0e\n\x07subject\x12\x03\xf8\x42\x01\"\xaf\x02\n\x14IsAuthorizedResponse\x12?\n\rdecision_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0c\x64\x65\x63isionTime\x12\x61\n\tdecisions\x18\x02 \x03(\x0b\x32\x43.indykite.authorization.v1beta1.IsAuthorizedResponse.DecisionsEntryR\tdecisions\x1as\n\x0e\x44\x65\x63isionsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12K\n\x05value\x18\x02 \x01(\x0b\x32\x35.indykite.authorization.v1beta1.AuthorizationDecisionR\x05value:\x02\x38\x01\"\xc2\x01\n\x15\x41uthorizationDecision\x12i\n\x0c\x61llow_action\x18\x01 \x03(\x0b\x32\x46.indykite.authorization.v1beta1.AuthorizationDecision.AllowActionEntryR\x0b\x61llowAction\x1a>\n\x10\x41llowActionEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\x08R\x05value:\x02\x38\x01\x32\x8d\x01\n\x10\x41uthorizationAPI\x12y\n\x0cIsAuthorized\x12\x33.indykite.authorization.v1beta1.IsAuthorizedRequest\x1a\x34.indykite.authorization.v1beta1.IsAuthorizedResponseB\xd9\x01\n\"com.indykite.authorization.v1beta1B\x19\x41uthorizationServiceProtoP\x01\xa2\x02\x03IAX\xaa\x02\x1eIndykite.Authorization.V1beta1\xca\x02\x1eIndykite\\Authorization\\V1beta1\xe2\x02*Indykite\\Authorization\\V1beta1\\GPBMetadata\xea\x02 Indykite::Authorization::V1beta1b\x06proto3')
 
 
 
 _ISAUTHORIZEDREQUEST = DESCRIPTOR.message_types_by_name['IsAuthorizedRequest']
 _ISAUTHORIZEDREQUEST_RESOURCE = _ISAUTHORIZEDREQUEST.nested_types_by_name['Resource']
 _ISAUTHORIZEDRESPONSE = DESCRIPTOR.message_types_by_name['IsAuthorizedResponse']
 _ISAUTHORIZEDRESPONSE_DECISIONSENTRY = _ISAUTHORIZEDRESPONSE.nested_types_by_name['DecisionsEntry']
@@ -77,32 +77,34 @@
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\"com.indykite.authorization.v1beta1B\031AuthorizationServiceProtoP\001\242\002\003IAX\252\002\036Indykite.Authorization.V1beta1\312\002\036Indykite\\Authorization\\V1beta1\342\002*Indykite\\Authorization\\V1beta1\\GPBMetadata\352\002 Indykite::Authorization::V1beta1'
   _ISAUTHORIZEDREQUEST_RESOURCE.fields_by_name['id']._options = None
   _ISAUTHORIZEDREQUEST_RESOURCE.fields_by_name['id']._serialized_options = b'\372B\006r\004\020\002\0302'
   _ISAUTHORIZEDREQUEST_RESOURCE.fields_by_name['label']._options = None
   _ISAUTHORIZEDREQUEST_RESOURCE.fields_by_name['label']._serialized_options = b'\372B\032r\030\020\002\03022\022^(?:[A-Z][a-z]+)+$'
-  _ISAUTHORIZEDREQUEST.fields_by_name['subject']._options = None
-  _ISAUTHORIZEDREQUEST.fields_by_name['subject']._serialized_options = b'\372B\005\212\001\002\020\001'
+  _ISAUTHORIZEDREQUEST.oneofs_by_name['subject']._options = None
+  _ISAUTHORIZEDREQUEST.oneofs_by_name['subject']._serialized_options = b'\370B\001'
+  _ISAUTHORIZEDREQUEST.fields_by_name['digital_twin_identifier']._options = None
+  _ISAUTHORIZEDREQUEST.fields_by_name['digital_twin_identifier']._serialized_options = b'\372B\005\212\001\002\020\001'
   _ISAUTHORIZEDREQUEST.fields_by_name['resources']._options = None
   _ISAUTHORIZEDREQUEST.fields_by_name['resources']._serialized_options = b'\372B\007\222\001\004\010\001\020 '
   _ISAUTHORIZEDREQUEST.fields_by_name['actions']._options = None
   _ISAUTHORIZEDREQUEST.fields_by_name['actions']._serialized_options = b'\372B)\222\001&\010\001\020\001\" r\036\020\002\03022\030^[a-zA-Z0-9.:_\\-\\/]{2,}$'
   _ISAUTHORIZEDRESPONSE_DECISIONSENTRY._options = None
   _ISAUTHORIZEDRESPONSE_DECISIONSENTRY._serialized_options = b'8\001'
   _AUTHORIZATIONDECISION_ALLOWACTIONENTRY._options = None
   _AUTHORIZATIONDECISION_ALLOWACTIONENTRY._serialized_options = b'8\001'
   _ISAUTHORIZEDREQUEST._serialized_start=210
-  _ISAUTHORIZEDREQUEST._serialized_end=585
-  _ISAUTHORIZEDREQUEST_RESOURCE._serialized_start=495
-  _ISAUTHORIZEDREQUEST_RESOURCE._serialized_end=585
-  _ISAUTHORIZEDRESPONSE._serialized_start=588
-  _ISAUTHORIZEDRESPONSE._serialized_end=891
-  _ISAUTHORIZEDRESPONSE_DECISIONSENTRY._serialized_start=776
-  _ISAUTHORIZEDRESPONSE_DECISIONSENTRY._serialized_end=891
-  _AUTHORIZATIONDECISION._serialized_start=894
-  _AUTHORIZATIONDECISION._serialized_end=1088
-  _AUTHORIZATIONDECISION_ALLOWACTIONENTRY._serialized_start=1026
-  _AUTHORIZATIONDECISION_ALLOWACTIONENTRY._serialized_end=1088
-  _AUTHORIZATIONAPI._serialized_start=1091
-  _AUTHORIZATIONAPI._serialized_end=1232
+  _ISAUTHORIZEDREQUEST._serialized_end=633
+  _ISAUTHORIZEDREQUEST_RESOURCE._serialized_start=527
+  _ISAUTHORIZEDREQUEST_RESOURCE._serialized_end=617
+  _ISAUTHORIZEDRESPONSE._serialized_start=636
+  _ISAUTHORIZEDRESPONSE._serialized_end=939
+  _ISAUTHORIZEDRESPONSE_DECISIONSENTRY._serialized_start=824
+  _ISAUTHORIZEDRESPONSE_DECISIONSENTRY._serialized_end=939
+  _AUTHORIZATIONDECISION._serialized_start=942
+  _AUTHORIZATIONDECISION._serialized_end=1136
+  _AUTHORIZATIONDECISION_ALLOWACTIONENTRY._serialized_start=1074
+  _AUTHORIZATIONDECISION_ALLOWACTIONENTRY._serialized_end=1136
+  _AUTHORIZATIONAPI._serialized_start=1139
+  _AUTHORIZATIONAPI._serialized_end=1280
 # @@protoc_insertion_point(module_scope)
```

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/indykite/authorization/v1beta1/authorization_service_pb2_grpc.py` & `indykite-sdk-python-1.9.0/indykite_sdk/indykite/authorization/v1beta1/authorization_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/indykite/config/v1beta1/config_management_api_pb2.py` & `indykite-sdk-python-1.9.0/indykite_sdk/indykite/config/v1beta1/config_management_api_pb2.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/indykite/config/v1beta1/config_management_api_pb2_grpc.py` & `indykite-sdk-python-1.9.0/indykite_sdk/indykite/config/v1beta1/config_management_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/indykite/config/v1beta1/model_pb2.py` & `indykite-sdk-python-1.9.0/indykite_sdk/indykite/config/v1beta1/model_pb2.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/indykite/events/v1beta1/events_pb2.py` & `indykite-sdk-python-1.9.0/indykite_sdk/indykite/events/v1beta1/events_pb2.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta1/attributes_pb2.py` & `indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta1/attributes_pb2.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta1/authenteq_pb2.py` & `indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta1/authenteq_pb2.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta1/document_pb2.py` & `indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta1/document_pb2.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta1/identity_management_api_pb2.py` & `indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta1/identity_management_api_pb2.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta1/identity_management_api_pb2_grpc.py` & `indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta1/identity_management_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta1/import_pb2.py` & `indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta1/import_pb2.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta1/model_pb2.py` & `indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta1/model_pb2.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta2/attributes_pb2.py` & `indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta2/attributes_pb2.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta2/authenteq_pb2.py` & `indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta2/authenteq_pb2.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta2/consent_pb2.py` & `indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta2/consent_pb2.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta2/document_pb2.py` & `indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta2/document_pb2.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta2/identity_management_api_pb2.py` & `indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta2/identity_management_api_pb2.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta2/identity_management_api_pb2_grpc.py` & `indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta2/identity_management_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta2/import_pb2.py` & `indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta2/import_pb2.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta2/model_pb2.py` & `indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta2/model_pb2.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/indykite/identity/v1beta2/readid_pb2.py` & `indykite-sdk-python-1.9.0/indykite_sdk/indykite/identity/v1beta2/readid_pb2.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/indykite/ingest/v1beta1/ingest_api_pb2.py` & `indykite-sdk-python-1.9.0/indykite_sdk/indykite/ingest/v1beta1/ingest_api_pb2.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/indykite/ingest/v1beta1/ingest_api_pb2_grpc.py` & `indykite-sdk-python-1.9.0/indykite_sdk/indykite/ingest/v1beta1/ingest_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/indykite/ingest/v1beta1/model_pb2.py` & `indykite-sdk-python-1.9.0/indykite_sdk/indykite/ingest/v1beta1/model_pb2.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/indykite/knowledge_graph/v1beta1/policy_pb2.py` & `indykite-sdk-python-1.9.0/indykite_sdk/indykite/knowledge_graph/v1beta1/policy_pb2.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/indykite/knowledge_graph/v1beta1/schema_pb2.py` & `indykite-sdk-python-1.9.0/indykite_sdk/indykite/knowledge_graph/v1beta1/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/indykite/objects/v1beta1/id_pb2.py` & `indykite-sdk-python-1.9.0/indykite_sdk/indykite/objects/v1beta1/id_pb2.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/indykite/objects/v1beta1/struct_pb2.py` & `indykite-sdk-python-1.9.0/indykite_sdk/indykite/objects/v1beta1/struct_pb2.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/ingest/__init__.py` & `indykite-sdk-python-1.9.0/indykite_sdk/ingest/__init__.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/model/app_space.py` & `indykite-sdk-python-1.9.0/indykite_sdk/model/app_space.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/model/application.py` & `indykite-sdk-python-1.9.0/indykite_sdk/model/application.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/model/application_agent.py` & `indykite-sdk-python-1.9.0/indykite_sdk/model/application_agent.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/model/application_agent_credential.py` & `indykite-sdk-python-1.9.0/indykite_sdk/model/application_agent_credential.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/model/auth_flow_config.py` & `indykite-sdk-python-1.9.0/indykite_sdk/model/auth_flow_config.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/model/config_node.py` & `indykite-sdk-python-1.9.0/indykite_sdk/model/config_node.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/model/create_app_space.py` & `indykite-sdk-python-1.9.0/indykite_sdk/model/create_app_space.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/model/create_application.py` & `indykite-sdk-python-1.9.0/indykite_sdk/model/create_application.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/model/create_application_agent.py` & `indykite-sdk-python-1.9.0/indykite_sdk/model/create_application_agent.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/model/create_config_node.py` & `indykite-sdk-python-1.9.0/indykite_sdk/model/create_config_node.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/model/create_oauth2_application.py` & `indykite-sdk-python-1.9.0/indykite_sdk/model/create_oauth2_application.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/model/create_oauth2_provider.py` & `indykite-sdk-python-1.9.0/indykite_sdk/model/create_oauth2_provider.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/model/create_service_account.py` & `indykite-sdk-python-1.9.0/indykite_sdk/model/create_service_account.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/model/create_tenant.py` & `indykite-sdk-python-1.9.0/indykite_sdk/model/create_tenant.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/model/customer.py` & `indykite-sdk-python-1.9.0/indykite_sdk/model/customer.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/model/digital_twin.py` & `indykite-sdk-python-1.9.0/indykite_sdk/model/digital_twin.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/model/email_attachment.py` & `indykite-sdk-python-1.9.0/indykite_sdk/model/email_attachment.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/model/email_message.py` & `indykite-sdk-python-1.9.0/indykite_sdk/model/email_message.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/model/email_service_config.py` & `indykite-sdk-python-1.9.0/indykite_sdk/model/email_service_config.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/model/email_template.py` & `indykite-sdk-python-1.9.0/indykite_sdk/model/email_template.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/model/ingest_mapping_config.py` & `indykite-sdk-python-1.9.0/indykite_sdk/model/ingest_mapping_config.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/model/oauth2_application.py` & `indykite-sdk-python-1.9.0/indykite_sdk/model/oauth2_application.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/model/oauth2_application_config.py` & `indykite-sdk-python-1.9.0/indykite_sdk/model/oauth2_application_config.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/model/oauth2_client_config.py` & `indykite-sdk-python-1.9.0/indykite_sdk/model/oauth2_client_config.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/model/oauth2_provider.py` & `indykite-sdk-python-1.9.0/indykite_sdk/model/oauth2_provider.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/model/oauth2_provider_config.py` & `indykite-sdk-python-1.9.0/indykite_sdk/model/oauth2_provider_config.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/model/postal_address.py` & `indykite-sdk-python-1.9.0/indykite_sdk/model/postal_address.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/model/property.py` & `indykite-sdk-python-1.9.0/indykite_sdk/model/property.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/model/register_application_agent_credential.py` & `indykite-sdk-python-1.9.0/indykite_sdk/model/register_application_agent_credential.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/model/register_service_account_credential.py` & `indykite-sdk-python-1.9.0/indykite_sdk/model/register_service_account_credential.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/model/sendgrid_email_provider.py` & `indykite-sdk-python-1.9.0/indykite_sdk/model/sendgrid_email_provider.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/model/service_account.py` & `indykite-sdk-python-1.9.0/indykite_sdk/model/service_account.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/model/service_account_credential.py` & `indykite-sdk-python-1.9.0/indykite_sdk/model/service_account_credential.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/model/tenant.py` & `indykite-sdk-python-1.9.0/indykite_sdk/model/tenant.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/model/token_info.py` & `indykite-sdk-python-1.9.0/indykite_sdk/model/token_info.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/model/update_app_space.py` & `indykite-sdk-python-1.9.0/indykite_sdk/model/update_app_space.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/model/update_application.py` & `indykite-sdk-python-1.9.0/indykite_sdk/model/update_application.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/model/update_application_agent.py` & `indykite-sdk-python-1.9.0/indykite_sdk/model/update_application_agent.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/model/update_config_node.py` & `indykite-sdk-python-1.9.0/indykite_sdk/model/update_config_node.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/model/update_oauth2_application.py` & `indykite-sdk-python-1.9.0/indykite_sdk/model/update_oauth2_application.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/model/update_oauth2_provider.py` & `indykite-sdk-python-1.9.0/indykite_sdk/model/update_oauth2_provider.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/model/update_service_account.py` & `indykite-sdk-python-1.9.0/indykite_sdk/model/update_service_account.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/model/update_tenant.py` & `indykite-sdk-python-1.9.0/indykite_sdk/model/update_tenant.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/utils/message_to_value.py` & `indykite-sdk-python-1.9.0/indykite_sdk/utils/message_to_value.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk/validate/validate_pb2.py` & `indykite-sdk-python-1.9.0/indykite_sdk/validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk_python.egg-info/PKG-INFO` & `indykite-sdk-python-1.9.0/indykite_sdk_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indykite-sdk-python
-Version: 1.8.0
+Version: 1.9.0
 Summary: A python SDK package for Indykite's system (with protobuf)
 Home-page: https://github.com/indykite/indykite-sdk-python
 Author: Indykite
 Author-email: test@indykite.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,19 +13,19 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # IndyKite Python SDK 🐍
 
 This project serves as a Software Development Kit for developers of Indykite applications.
 
-[![codecov](https://codecov.io/gh/indykite/jarvis-sdk-python/branch/master/graph/badge.svg)](https://codecov.io/gh/indykite/indykite-sdk-python)
+[![codecov](https://codecov.io/gh/indykite/indykite-sdk-python/branch/master/graph/badge.svg)](https://codecov.io/gh/indykite/indykite-sdk-python)
 
 ## Requirements
 
-* Python 3.8
+* Python 3.11
 * [Buf](https://github.com/bufbuild/buf)
 
 ## Installation
 
 * Create virtual env and install dependencies
 
         pipenv install
@@ -1283,15 +1283,15 @@
             bookmarks)
 
     print(update_ingest_mapping_config_node_response)
 ```
 
 ### Get OAuth2 provider information
 
-In an Apppace, you can create OAuth2 providers.
+In an Appspace, you can create OAuth2 providers.
 An OAuth2 service provider is a named set of configuration options for OAuth2. 
 
 #### Read OAuth2 provider
 ```python
 from indykite_sdk.config import ConfigClient
 
 def get_oauth2_provider(self, local, oauth2_provider_id, bookmarks):
@@ -1395,17 +1395,36 @@
 
 def delete_oauth2_application(self, local, oauth2_application_id, etag, bookmarks):
     client_config = ConfigClient(local)
     config = client_config.delete_oauth2_application(oauth2_application_id, etag, bookmarks)
     print(config)
 ```
 
+### Import digital twins
+```python
+from indykite_sdk.indykite.identity.v1beta2.import_pb2 import ImportDigitalTwin
+from indykite_sdk.identity import IdentityClient
+
+def import_digital_twins(self, local, entities, hash_algorithm):
+  client = IdentityClient(local)
+  response = client.import_digital_twins(entities, hash_algorithm)
+  print(response)
+```
+
 
 # Changelog
 
+## [1.9.0](https://github.com/indykite/indykite-sdk-python/compare/v1.8.0...v1.9.0) (2023-01-12)
+
+
+### Features
+
+* add import DT and update tests ([ca30bd0](https://github.com/indykite/indykite-sdk-python/commit/ca30bd07503290089f599c3c34bee453dc846822))
+* add import DT and update tests ([c1c954f](https://github.com/indykite/indykite-sdk-python/commit/c1c954f553e6cc10d222459dbd2371fb4100c8d8))
+
 ## [1.8.0](https://github.com/indykite/indykite-sdk-python/compare/v1.7.0...v1.8.0) (2023-01-05)
 
 
 ### Features
 
 * add missing init files ([cf0d5dd](https://github.com/indykite/indykite-sdk-python/commit/cf0d5dd0b7fce45e5b64f33e4566a4690764d250))
```

### Comparing `indykite-sdk-python-1.8.0/indykite_sdk_python.egg-info/SOURCES.txt` & `indykite-sdk-python-1.9.0/indykite_sdk_python.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 indykite_sdk/config/tenant.py
 indykite_sdk/identity/__init__.py
 indykite_sdk/identity/change_password.py
 indykite_sdk/identity/delete.py
 indykite_sdk/identity/enrich_token.py
 indykite_sdk/identity/get_digital_twin.py
 indykite_sdk/identity/helper.py
+indykite_sdk/identity/import_digital_twins.py
 indykite_sdk/identity/introspect_token.py
 indykite_sdk/identity/patch_properties.py
 indykite_sdk/identity/verification.py
 indykite_sdk/indykite/__init__.py
 indykite_sdk/indykite/authorization/__init__.py
 indykite_sdk/indykite/authorization/v1beta1/__init__.py
 indykite_sdk/indykite/authorization/v1beta1/authorization_service_pb2.py
@@ -107,19 +108,22 @@
 indykite_sdk/model/create_config_node.py
 indykite_sdk/model/create_oauth2_application.py
 indykite_sdk/model/create_oauth2_provider.py
 indykite_sdk/model/create_service_account.py
 indykite_sdk/model/create_tenant.py
 indykite_sdk/model/customer.py
 indykite_sdk/model/digital_twin.py
+indykite_sdk/model/digital_twin_kind.py
+indykite_sdk/model/digital_twin_state.py
 indykite_sdk/model/email.py
 indykite_sdk/model/email_attachment.py
 indykite_sdk/model/email_message.py
 indykite_sdk/model/email_service_config.py
 indykite_sdk/model/email_template.py
+indykite_sdk/model/import_digital_twin.py
 indykite_sdk/model/ingest_mapping_config.py
 indykite_sdk/model/oauth2_application.py
 indykite_sdk/model/oauth2_application_config.py
 indykite_sdk/model/oauth2_client_config.py
 indykite_sdk/model/oauth2_provider.py
 indykite_sdk/model/oauth2_provider_config.py
 indykite_sdk/model/postal_address.py
@@ -139,14 +143,15 @@
 indykite_sdk/model/update_config_node.py
 indykite_sdk/model/update_oauth2_application.py
 indykite_sdk/model/update_oauth2_provider.py
 indykite_sdk/model/update_service_account.py
 indykite_sdk/model/update_tenant.py
 indykite_sdk/utils/__init__.py
 indykite_sdk/utils/deserialize_digital_twin_with_token_info.py
+indykite_sdk/utils/hash_methods.py
 indykite_sdk/utils/message_to_value.py
 indykite_sdk/validate/__init__.py
 indykite_sdk/validate/validate_pb2.py
 indykite_sdk/validate/validate_pb2_grpc.py
 indykite_sdk_python.egg-info/PKG-INFO
 indykite_sdk_python.egg-info/SOURCES.txt
 indykite_sdk_python.egg-info/dependency_links.txt
```

### Comparing `indykite-sdk-python-1.8.0/setup.py` & `indykite-sdk-python-1.9.0/setup.py`

 * *Files identical despite different names*

