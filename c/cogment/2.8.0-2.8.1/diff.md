# Comparing `tmp/cogment-2.8.0.tar.gz` & `tmp/cogment-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/builds/ai-r/cogment/cogment-py-sdk/dist/.tmp-hbg83nvd/cogment-2.8.0.tar", last modified: Fri Apr 21 20:04:19 2023, max compression
+gzip compressed data, was "/builds/ai-r/cogment/cogment-py-sdk/dist/.tmp-4cmcyn6_/cogment-2.8.1.tar", last modified: Tue Jun  6 20:18:15 2023, max compression
```

## Comparing `cogment-2.8.0.tar` & `cogment-2.8.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:04:19.000000 cogment-2.8.0/
--rw-rw-rw-   0 root         (0) root         (0)     9511 2023-04-21 20:03:55.000000 cogment-2.8.0/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)    10255 2023-04-21 20:03:55.000000 cogment-2.8.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    14657 2023-04-21 20:04:19.000000 cogment-2.8.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4476 2023-04-21 20:03:55.000000 cogment-2.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/
--rw-rw-rw-   0 root         (0) root         (0)     1720 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3922 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/actor.py
--rw-rw-rw-   0 root         (0) root         (0)    19336 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/agent_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/api/
--rw-r--r--   0 root         (0) root         (0)     1021 2023-03-23 15:54:42.000000 cogment-2.8.0/cogment/api/agent.proto
--rw-r--r--   0 root         (0) root         (0)     1379 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/api/agent_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4231 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/api/agent_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     7025 2023-03-23 15:54:42.000000 cogment-2.8.0/cogment/api/common.proto
--rw-r--r--   0 root         (0) root         (0)    16049 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/api/common_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/api/common_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     4537 2023-03-23 15:54:42.000000 cogment-2.8.0/cogment/api/datalog.proto
--rw-r--r--   0 root         (0) root         (0)    13215 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/api/datalog_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4320 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/api/datalog_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3726 2023-03-23 15:54:42.000000 cogment-2.8.0/cogment/api/directory.proto
--rw-r--r--   0 root         (0) root         (0)     9698 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/api/directory_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8131 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/api/directory_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3627 2023-03-23 15:54:42.000000 cogment-2.8.0/cogment/api/environment.proto
--rw-r--r--   0 root         (0) root         (0)     5639 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/api/environment_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4933 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/api/environment_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3687 2023-03-23 15:54:42.000000 cogment-2.8.0/cogment/api/health.proto
--rw-r--r--   0 root         (0) root         (0)     3339 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/api/health_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5065 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/api/health_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     1044 2023-03-23 15:54:42.000000 cogment-2.8.0/cogment/api/hooks.proto
--rw-r--r--   0 root         (0) root         (0)     1875 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/api/hooks_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4224 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/api/hooks_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     5398 2023-03-23 15:54:42.000000 cogment-2.8.0/cogment/api/model_registry.proto
--rw-r--r--   0 root         (0) root         (0)    15133 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/api/model_registry_pb2.py
--rw-r--r--   0 root         (0) root         (0)    15143 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/api/model_registry_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     4170 2023-03-23 15:54:42.000000 cogment-2.8.0/cogment/api/orchestrator.proto
--rw-r--r--   0 root         (0) root         (0)     8533 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/api/orchestrator_pb2.py
--rw-r--r--   0 root         (0) root         (0)    13880 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/api/orchestrator_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     7431 2023-03-23 15:54:42.000000 cogment-2.8.0/cogment/api/trial_datastore.proto
--rw-r--r--   0 root         (0) root         (0)    15895 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/api/trial_datastore_pb2.py
--rw-r--r--   0 root         (0) root         (0)    11659 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment/api/trial_datastore_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)    17115 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/client_service.py
--rw-rw-rw-   0 root         (0) root         (0)    23312 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/context.py
--rw-rw-rw-   0 root         (0) root         (0)     7910 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/control.py
--rw-rw-rw-   0 root         (0) root         (0)     7853 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/datalog.py
--rw-rw-rw-   0 root         (0) root         (0)    10078 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/datalog_service.py
--rw-rw-rw-   0 root         (0) root         (0)    14369 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/datastore.py
--rw-rw-rw-   0 root         (0) root         (0)    11837 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/directory.py
--rw-rw-rw-   0 root         (0) root         (0)     4136 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/endpoints.py
--rw-rw-rw-   0 root         (0) root         (0)    18791 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/env_service.py
--rw-rw-rw-   0 root         (0) root         (0)     5591 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/environment.py
--rw-rw-rw-   0 root         (0) root         (0)     1004 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     7321 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/generate.py
--rw-rw-rw-   0 root         (0) root         (0)     7840 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/hooks_service.py
--rw-rw-rw-   0 root         (0) root         (0)    10467 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/model_registry.py
--rw-rw-rw-   0 root         (0) root         (0)    19851 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/model_registry_v2.py
--rw-rw-rw-   0 root         (0) root         (0)    21845 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     3680 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/prehook.py
--rw-rw-rw-   0 root         (0) root         (0)    14373 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/session.py
--rw-rw-rw-   0 root         (0) root         (0)     1940 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/trial.py
--rw-rw-rw-   0 root         (0) root         (0)     2392 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      672 2023-04-21 20:03:55.000000 cogment-2.8.0/cogment/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment.egg-info/
--rw-r--r--   0 root         (0) root         (0)    14657 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1726 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      149 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-21 20:04:19.000000 cogment-2.8.0/cogment.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     2013 2023-04-21 20:03:55.000000 cogment-2.8.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      161 2023-04-21 20:04:19.000000 cogment-2.8.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     6037 2023-04-21 20:03:55.000000 cogment-2.8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 20:04:19.000000 cogment-2.8.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2023 2023-04-21 20:03:55.000000 cogment-2.8.0/tests/test_download_cogment.py
--rw-rw-rw-   0 root         (0) root         (0)    26016 2023-04-21 20:03:55.000000 cogment-2.8.0/tests/test_integration.py
--rw-rw-rw-   0 root         (0) root         (0)     4326 2023-04-21 20:03:55.000000 cogment-2.8.0/tests/test_model_registry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 20:18:15.000000 cogment-2.8.1/
+-rw-rw-rw-   0 root         (0) root         (0)     9676 2023-06-06 20:17:56.000000 cogment-2.8.1/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)    10255 2023-06-06 20:17:56.000000 cogment-2.8.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    14822 2023-06-06 20:18:15.000000 cogment-2.8.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4476 2023-06-06 20:17:56.000000 cogment-2.8.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 20:18:15.000000 cogment-2.8.1/cogment/
+-rw-rw-rw-   0 root         (0) root         (0)     1720 2023-06-06 20:17:56.000000 cogment-2.8.1/cogment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3922 2023-06-06 20:17:56.000000 cogment-2.8.1/cogment/actor.py
+-rw-rw-rw-   0 root         (0) root         (0)    19336 2023-06-06 20:17:56.000000 cogment-2.8.1/cogment/agent_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 20:18:15.000000 cogment-2.8.1/cogment/api/
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-03-23 15:54:42.000000 cogment-2.8.1/cogment/api/agent.proto
+-rw-r--r--   0 root         (0) root         (0)     1379 2023-06-06 20:18:15.000000 cogment-2.8.1/cogment/api/agent_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4231 2023-06-06 20:18:15.000000 cogment-2.8.1/cogment/api/agent_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     7025 2023-03-23 15:54:42.000000 cogment-2.8.1/cogment/api/common.proto
+-rw-r--r--   0 root         (0) root         (0)    16049 2023-06-06 20:18:15.000000 cogment-2.8.1/cogment/api/common_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-06 20:18:15.000000 cogment-2.8.1/cogment/api/common_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     4537 2023-03-23 15:54:42.000000 cogment-2.8.1/cogment/api/datalog.proto
+-rw-r--r--   0 root         (0) root         (0)    13215 2023-06-06 20:18:15.000000 cogment-2.8.1/cogment/api/datalog_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4320 2023-06-06 20:18:15.000000 cogment-2.8.1/cogment/api/datalog_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3726 2023-03-23 15:54:42.000000 cogment-2.8.1/cogment/api/directory.proto
+-rw-r--r--   0 root         (0) root         (0)     9698 2023-06-06 20:18:15.000000 cogment-2.8.1/cogment/api/directory_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8131 2023-06-06 20:18:15.000000 cogment-2.8.1/cogment/api/directory_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3627 2023-03-23 15:54:42.000000 cogment-2.8.1/cogment/api/environment.proto
+-rw-r--r--   0 root         (0) root         (0)     5639 2023-06-06 20:18:15.000000 cogment-2.8.1/cogment/api/environment_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4933 2023-06-06 20:18:15.000000 cogment-2.8.1/cogment/api/environment_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3687 2023-03-23 15:54:42.000000 cogment-2.8.1/cogment/api/health.proto
+-rw-r--r--   0 root         (0) root         (0)     3339 2023-06-06 20:18:15.000000 cogment-2.8.1/cogment/api/health_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5065 2023-06-06 20:18:15.000000 cogment-2.8.1/cogment/api/health_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     1044 2023-03-23 15:54:42.000000 cogment-2.8.1/cogment/api/hooks.proto
+-rw-r--r--   0 root         (0) root         (0)     1875 2023-06-06 20:18:15.000000 cogment-2.8.1/cogment/api/hooks_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4224 2023-06-06 20:18:15.000000 cogment-2.8.1/cogment/api/hooks_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     5398 2023-03-23 15:54:42.000000 cogment-2.8.1/cogment/api/model_registry.proto
+-rw-r--r--   0 root         (0) root         (0)    15133 2023-06-06 20:18:15.000000 cogment-2.8.1/cogment/api/model_registry_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    15143 2023-06-06 20:18:15.000000 cogment-2.8.1/cogment/api/model_registry_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     4170 2023-03-23 15:54:42.000000 cogment-2.8.1/cogment/api/orchestrator.proto
+-rw-r--r--   0 root         (0) root         (0)     8533 2023-06-06 20:18:15.000000 cogment-2.8.1/cogment/api/orchestrator_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    13880 2023-06-06 20:18:15.000000 cogment-2.8.1/cogment/api/orchestrator_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     7431 2023-03-23 15:54:42.000000 cogment-2.8.1/cogment/api/trial_datastore.proto
+-rw-r--r--   0 root         (0) root         (0)    15895 2023-06-06 20:18:15.000000 cogment-2.8.1/cogment/api/trial_datastore_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    11659 2023-06-06 20:18:15.000000 cogment-2.8.1/cogment/api/trial_datastore_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)    17115 2023-06-06 20:17:56.000000 cogment-2.8.1/cogment/client_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    23512 2023-06-06 20:17:56.000000 cogment-2.8.1/cogment/context.py
+-rw-rw-rw-   0 root         (0) root         (0)     7910 2023-06-06 20:17:56.000000 cogment-2.8.1/cogment/control.py
+-rw-rw-rw-   0 root         (0) root         (0)     7853 2023-06-06 20:17:56.000000 cogment-2.8.1/cogment/datalog.py
+-rw-rw-rw-   0 root         (0) root         (0)    10078 2023-06-06 20:17:56.000000 cogment-2.8.1/cogment/datalog_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    14369 2023-06-06 20:17:56.000000 cogment-2.8.1/cogment/datastore.py
+-rw-rw-rw-   0 root         (0) root         (0)    11898 2023-06-06 20:17:56.000000 cogment-2.8.1/cogment/directory.py
+-rw-rw-rw-   0 root         (0) root         (0)     4136 2023-06-06 20:17:56.000000 cogment-2.8.1/cogment/endpoints.py
+-rw-rw-rw-   0 root         (0) root         (0)    18791 2023-06-06 20:17:56.000000 cogment-2.8.1/cogment/env_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     5591 2023-06-06 20:17:56.000000 cogment-2.8.1/cogment/environment.py
+-rw-rw-rw-   0 root         (0) root         (0)     1004 2023-06-06 20:17:56.000000 cogment-2.8.1/cogment/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     7321 2023-06-06 20:17:56.000000 cogment-2.8.1/cogment/generate.py
+-rw-rw-rw-   0 root         (0) root         (0)     7840 2023-06-06 20:17:56.000000 cogment-2.8.1/cogment/hooks_service.py
+-rw-rw-rw-   0 root         (0) root         (0)    10467 2023-06-06 20:17:56.000000 cogment-2.8.1/cogment/model_registry.py
+-rw-rw-rw-   0 root         (0) root         (0)    19851 2023-06-06 20:17:56.000000 cogment-2.8.1/cogment/model_registry_v2.py
+-rw-rw-rw-   0 root         (0) root         (0)    21845 2023-06-06 20:17:56.000000 cogment-2.8.1/cogment/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     3680 2023-06-06 20:17:56.000000 cogment-2.8.1/cogment/prehook.py
+-rw-rw-rw-   0 root         (0) root         (0)    14373 2023-06-06 20:17:56.000000 cogment-2.8.1/cogment/session.py
+-rw-rw-rw-   0 root         (0) root         (0)     1940 2023-06-06 20:17:56.000000 cogment-2.8.1/cogment/trial.py
+-rw-rw-rw-   0 root         (0) root         (0)     2392 2023-06-06 20:17:56.000000 cogment-2.8.1/cogment/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      672 2023-06-06 20:17:56.000000 cogment-2.8.1/cogment/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 20:18:15.000000 cogment-2.8.1/cogment.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14822 2023-06-06 20:18:15.000000 cogment-2.8.1/cogment.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1726 2023-06-06 20:18:15.000000 cogment-2.8.1/cogment.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 20:18:15.000000 cogment-2.8.1/cogment.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      149 2023-06-06 20:18:15.000000 cogment-2.8.1/cogment.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-06 20:18:15.000000 cogment-2.8.1/cogment.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2013 2023-06-06 20:17:56.000000 cogment-2.8.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-06-06 20:18:15.000000 cogment-2.8.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     6037 2023-06-06 20:17:56.000000 cogment-2.8.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 20:18:15.000000 cogment-2.8.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2023 2023-06-06 20:17:56.000000 cogment-2.8.1/tests/test_download_cogment.py
+-rw-rw-rw-   0 root         (0) root         (0)    26016 2023-06-06 20:17:56.000000 cogment-2.8.1/tests/test_integration.py
+-rw-rw-rw-   0 root         (0) root         (0)     4326 2023-06-06 20:17:56.000000 cogment-2.8.1/tests/test_model_registry.py
```

### Comparing `cogment-2.8.0/CHANGELOG.md` & `cogment-2.8.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,21 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## Unreleased
 
+## v2.8.1 - 2023-06-06
+
+## Fixed
+
+- Use the most recent directory entry when there are duplicates
+- Self IP address discovery functionality is now working on macOS
+
 ## v2.8.0 - 2023-04-21
 
 ### Added
 
 - Option to request full info (not just id and state) from 'watch_trials'
 - Ability to use the SDK without spec (cog_settings)
 - Automatic port selection for 'Context.serve_all_registered()'
@@ -58,16 +65,16 @@
 - In Datastore reward could be returned as 'None' instead of 0.0
 
 ### Added
 
 - Simplified interface for Model Registry (context.get_model_registry_v2)
 
 ## v2.4.1 - 2022-12-02
-- Support and dependency check for python 3.10
 
+- Support and dependency check for python 3.10
 
 ## v2.4.0 - 2022-11-18
 
 ### Added
 
 - 'COGMENT_LOG_LEVEL' environment variable
 - Model Registry client
```

### Comparing `cogment-2.8.0/LICENSE` & `cogment-2.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/PKG-INFO` & `cogment-2.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cogment
-Version: 2.8.0
+Version: 2.8.1
 Summary: Cogment python SDK
 Author-email: Artificial Intelligence Redefined <dev+cogment@ai-r.com>
 Project-URL: Homepage, https://cogment.ai
 Project-URL: repository, https://github.com/cogment/cogment-py-sdk
 Project-URL: Reference Documentation, https://cogment.ai/docs/reference/python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
@@ -134,14 +134,21 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## Unreleased
 
+## v2.8.1 - 2023-06-06
+
+## Fixed
+
+- Use the most recent directory entry when there are duplicates
+- Self IP address discovery functionality is now working on macOS
+
 ## v2.8.0 - 2023-04-21
 
 ### Added
 
 - Option to request full info (not just id and state) from 'watch_trials'
 - Ability to use the SDK without spec (cog_settings)
 - Automatic port selection for 'Context.serve_all_registered()'
@@ -189,16 +196,16 @@
 - In Datastore reward could be returned as 'None' instead of 0.0
 
 ### Added
 
 - Simplified interface for Model Registry (context.get_model_registry_v2)
 
 ## v2.4.1 - 2022-12-02
-- Support and dependency check for python 3.10
 
+- Support and dependency check for python 3.10
 
 ## v2.4.0 - 2022-11-18
 
 ### Added
 
 - 'COGMENT_LOG_LEVEL' environment variable
 - Model Registry client
```

### Comparing `cogment-2.8.0/README.md` & `cogment-2.8.1/README.md`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/__init__.py` & `cogment-2.8.1/cogment/__init__.py`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/actor.py` & `cogment-2.8.1/cogment/actor.py`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/agent_service.py` & `cogment-2.8.1/cogment/agent_service.py`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/api/agent.proto` & `cogment-2.8.1/cogment/api/agent.proto`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/api/agent_pb2.py` & `cogment-2.8.1/cogment/api/agent_pb2.py`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/api/agent_pb2_grpc.py` & `cogment-2.8.1/cogment/api/agent_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/api/common.proto` & `cogment-2.8.1/cogment/api/common.proto`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/api/common_pb2.py` & `cogment-2.8.1/cogment/api/common_pb2.py`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/api/datalog.proto` & `cogment-2.8.1/cogment/api/datalog.proto`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/api/datalog_pb2.py` & `cogment-2.8.1/cogment/api/datalog_pb2.py`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/api/datalog_pb2_grpc.py` & `cogment-2.8.1/cogment/api/datalog_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/api/directory.proto` & `cogment-2.8.1/cogment/api/directory.proto`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/api/directory_pb2.py` & `cogment-2.8.1/cogment/api/directory_pb2.py`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/api/directory_pb2_grpc.py` & `cogment-2.8.1/cogment/api/directory_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/api/environment.proto` & `cogment-2.8.1/cogment/api/environment.proto`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/api/environment_pb2.py` & `cogment-2.8.1/cogment/api/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/api/environment_pb2_grpc.py` & `cogment-2.8.1/cogment/api/environment_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/api/health.proto` & `cogment-2.8.1/cogment/api/health.proto`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/api/health_pb2.py` & `cogment-2.8.1/cogment/api/health_pb2.py`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/api/health_pb2_grpc.py` & `cogment-2.8.1/cogment/api/health_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/api/hooks.proto` & `cogment-2.8.1/cogment/api/hooks.proto`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/api/hooks_pb2.py` & `cogment-2.8.1/cogment/api/hooks_pb2.py`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/api/hooks_pb2_grpc.py` & `cogment-2.8.1/cogment/api/hooks_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/api/model_registry.proto` & `cogment-2.8.1/cogment/api/model_registry.proto`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/api/model_registry_pb2.py` & `cogment-2.8.1/cogment/api/model_registry_pb2.py`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/api/model_registry_pb2_grpc.py` & `cogment-2.8.1/cogment/api/model_registry_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/api/orchestrator.proto` & `cogment-2.8.1/cogment/api/orchestrator.proto`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/api/orchestrator_pb2.py` & `cogment-2.8.1/cogment/api/orchestrator_pb2.py`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/api/orchestrator_pb2_grpc.py` & `cogment-2.8.1/cogment/api/orchestrator_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/api/trial_datastore.proto` & `cogment-2.8.1/cogment/api/trial_datastore.proto`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/api/trial_datastore_pb2.py` & `cogment-2.8.1/cogment/api/trial_datastore_pb2.py`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/api/trial_datastore_pb2_grpc.py` & `cogment-2.8.1/cogment/api/trial_datastore_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/client_service.py` & `cogment-2.8.1/cogment/client_service.py`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/context.py` & `cogment-2.8.1/cogment/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,19 @@
 _ADDITIONAL_REGISTRATION_ITEMS = {"__registration_source" : "PythonSDK-Implicit", "__version" : __version__}
 
 # (host, port): This IP address is normally not assigned, it is reserved for local benchmarking by IANA (RFC2544).
 _SPECIAL_CONNECTION_IP = ("192.19.254.254", 65535)
 
 
 def _self_ip_address():
-    sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM | socket.SOCK_NONBLOCK)
+    try:
+        sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM | socket.SOCK_NONBLOCK)
+    except AttributeError:
+        # socket.SOCK_NONBLOCK is only defined on "modern" linuxes, fallbacking to not using it
+        sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
     try:
         sock.connect(_SPECIAL_CONNECTION_IP)
         addr = sock.getsockname()[0]
     except Exception as exc:
         logger.debug(f"Failed to connect to get host ip address [{exc}]")
         addr = None
     finally:
```

### Comparing `cogment-2.8.0/cogment/control.py` & `cogment-2.8.1/cogment/control.py`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/datalog.py` & `cogment-2.8.1/cogment/datalog.py`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/datalog_service.py` & `cogment-2.8.1/cogment/datalog_service.py`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/datastore.py` & `cogment-2.8.1/cogment/datastore.py`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/directory.py` & `cogment-2.8.1/cogment/directory.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,14 +167,15 @@
             return endpoint
 
         url = None
         ssl_endpoint = endpoint.using_ssl()
         for dir_url, dir_ssl in dir_urls:
             if (ssl_endpoint and dir_ssl) or (not ssl_endpoint and not dir_ssl):
                 url = dir_url
+                break  # We take the first (most recent) one
 
         if url is not None:
             new_endpoint = copy.copy(endpoint)
             new_endpoint.url = url
         else:
             if not ssl_endpoint:
                 raise CogmentError(f"All services found require an SSL connection [{endpoint.url}]")
```

### Comparing `cogment-2.8.0/cogment/endpoints.py` & `cogment-2.8.1/cogment/endpoints.py`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/env_service.py` & `cogment-2.8.1/cogment/env_service.py`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/environment.py` & `cogment-2.8.1/cogment/environment.py`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/errors.py` & `cogment-2.8.1/cogment/errors.py`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/generate.py` & `cogment-2.8.1/cogment/generate.py`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/hooks_service.py` & `cogment-2.8.1/cogment/hooks_service.py`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/model_registry.py` & `cogment-2.8.1/cogment/model_registry.py`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/model_registry_v2.py` & `cogment-2.8.1/cogment/model_registry_v2.py`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/parameters.py` & `cogment-2.8.1/cogment/parameters.py`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/prehook.py` & `cogment-2.8.1/cogment/prehook.py`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/session.py` & `cogment-2.8.1/cogment/session.py`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/trial.py` & `cogment-2.8.1/cogment/trial.py`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/utils.py` & `cogment-2.8.1/cogment/utils.py`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/cogment/version.py` & `cogment-2.8.1/cogment/version.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # no import: add a comment to please linters
 
-__version__ = "2.8.0"
+__version__ = "2.8.1"
```

### Comparing `cogment-2.8.0/cogment.egg-info/PKG-INFO` & `cogment-2.8.1/cogment.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cogment
-Version: 2.8.0
+Version: 2.8.1
 Summary: Cogment python SDK
 Author-email: Artificial Intelligence Redefined <dev+cogment@ai-r.com>
 Project-URL: Homepage, https://cogment.ai
 Project-URL: repository, https://github.com/cogment/cogment-py-sdk
 Project-URL: Reference Documentation, https://cogment.ai/docs/reference/python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
@@ -134,14 +134,21 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## Unreleased
 
+## v2.8.1 - 2023-06-06
+
+## Fixed
+
+- Use the most recent directory entry when there are duplicates
+- Self IP address discovery functionality is now working on macOS
+
 ## v2.8.0 - 2023-04-21
 
 ### Added
 
 - Option to request full info (not just id and state) from 'watch_trials'
 - Ability to use the SDK without spec (cog_settings)
 - Automatic port selection for 'Context.serve_all_registered()'
@@ -189,16 +196,16 @@
 - In Datastore reward could be returned as 'None' instead of 0.0
 
 ### Added
 
 - Simplified interface for Model Registry (context.get_model_registry_v2)
 
 ## v2.4.1 - 2022-12-02
-- Support and dependency check for python 3.10
 
+- Support and dependency check for python 3.10
 
 ## v2.4.0 - 2022-11-18
 
 ### Added
 
 - 'COGMENT_LOG_LEVEL' environment variable
 - Model Registry client
```

### Comparing `cogment-2.8.0/cogment.egg-info/SOURCES.txt` & `cogment-2.8.1/cogment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/pyproject.toml` & `cogment-2.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/setup.py` & `cogment-2.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/tests/test_download_cogment.py` & `cogment-2.8.1/tests/test_download_cogment.py`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/tests/test_integration.py` & `cogment-2.8.1/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `cogment-2.8.0/tests/test_model_registry.py` & `cogment-2.8.1/tests/test_model_registry.py`

 * *Files identical despite different names*

