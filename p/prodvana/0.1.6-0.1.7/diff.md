# Comparing `tmp/prodvana-0.1.6.tar.gz` & `tmp/prodvana-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodvana-0.1.6.tar", max compression
+gzip compressed data, was "prodvana-0.1.7.tar", max compression
```

## Comparing `prodvana-0.1.6.tar` & `prodvana-0.1.7.tar`

### file list

```diff
@@ -1,332 +1,332 @@
--rw-r--r--   0        0        0       81 2023-05-30 13:39:12.483857 prodvana-0.1.6/README.md
--rw-r--r--   0        0        0        0 2023-05-30 13:39:12.483857 prodvana-0.1.6/prodvana/__init__.py
--rw-r--r--   0        0        0     3529 2023-05-30 13:39:12.483857 prodvana-0.1.6/prodvana/client.py
--rw-r--r--   0        0        0        0 2023-06-02 21:20:34.029790 prodvana-0.1.6/prodvana/proto/__init__.py
--rw-r--r--   0        0        0        0 2023-06-02 21:20:34.029790 prodvana-0.1.6/prodvana/proto/prodvana/__init__.py
--rw-r--r--   0        0        0        0 2023-06-02 21:20:34.057790 prodvana-0.1.6/prodvana/proto/prodvana/agent/__init__.py
--rw-r--r--   0        0        0    19183 2023-06-02 21:20:33.773790 prodvana-0.1.6/prodvana/proto/prodvana/agent/agent_interaction_pb2.py
--rw-r--r--   0        0        0    18983 2023-06-02 21:20:33.973790 prodvana-0.1.6/prodvana/proto/prodvana/agent/agent_interaction_pb2.pyi
--rw-r--r--   0        0        0    22573 2023-06-02 21:20:33.769790 prodvana-0.1.6/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.py
--rw-r--r--   0        0        0     6760 2023-06-02 21:20:33.977790 prodvana-0.1.6/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-02 21:20:34.033790 prodvana-0.1.6/prodvana/proto/prodvana/application/__init__.py
--rw-r--r--   0        0        0     4200 2023-06-02 21:20:33.665790 prodvana-0.1.6/prodvana/proto/prodvana/application/application_config_pb2.py
--rw-r--r--   0        0        0     4693 2023-06-02 21:20:33.865790 prodvana-0.1.6/prodvana/proto/prodvana/application/application_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.661790 prodvana-0.1.6/prodvana/proto/prodvana/application/application_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.865790 prodvana-0.1.6/prodvana/proto/prodvana/application/application_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    24873 2023-06-02 21:20:33.669790 prodvana-0.1.6/prodvana/proto/prodvana/application/application_manager_pb2.py
--rw-r--r--   0        0        0    16394 2023-06-02 21:20:33.873790 prodvana-0.1.6/prodvana/proto/prodvana/application/application_manager_pb2.pyi
--rw-r--r--   0        0        0    22241 2023-06-02 21:20:33.661790 prodvana-0.1.6/prodvana/proto/prodvana/application/application_manager_pb2_grpc.py
--rw-r--r--   0        0        0     6755 2023-06-02 21:20:33.877790 prodvana-0.1.6/prodvana/proto/prodvana/application/application_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2801 2023-06-02 21:20:33.657790 prodvana-0.1.6/prodvana/proto/prodvana/application/object_pb2.py
--rw-r--r--   0        0        0     2184 2023-06-02 21:20:33.873790 prodvana-0.1.6/prodvana/proto/prodvana/application/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.657790 prodvana-0.1.6/prodvana/proto/prodvana/application/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.869790 prodvana-0.1.6/prodvana/proto/prodvana/application/object_pb2_grpc.pyi
--rw-r--r--   0        0        0     2294 2023-06-02 21:20:33.665790 prodvana-0.1.6/prodvana/proto/prodvana/application/user_metadata_pb2.py
--rw-r--r--   0        0        0     1670 2023-06-02 21:20:33.869790 prodvana-0.1.6/prodvana/proto/prodvana/application/user_metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.661790 prodvana-0.1.6/prodvana/proto/prodvana/application/user_metadata_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.873790 prodvana-0.1.6/prodvana/proto/prodvana/application/user_metadata_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-02 21:20:34.061790 prodvana-0.1.6/prodvana/proto/prodvana/auth/__init__.py
--rw-r--r--   0        0        0    13908 2023-06-02 21:20:33.797790 prodvana-0.1.6/prodvana/proto/prodvana/auth/auth_manager_pb2.py
--rw-r--r--   0        0        0    10206 2023-06-02 21:20:34.001790 prodvana-0.1.6/prodvana/proto/prodvana/auth/auth_manager_pb2.pyi
--rw-r--r--   0        0        0    18631 2023-06-02 21:20:33.801790 prodvana-0.1.6/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.py
--rw-r--r--   0        0        0     6767 2023-06-02 21:20:34.005790 prodvana-0.1.6/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     5071 2023-06-02 21:20:33.797790 prodvana-0.1.6/prodvana/proto/prodvana/auth/auth_pb2.py
--rw-r--r--   0        0        0     5515 2023-06-02 21:20:34.005790 prodvana-0.1.6/prodvana/proto/prodvana/auth/auth_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.801790 prodvana-0.1.6/prodvana/proto/prodvana/auth/auth_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:34.001790 prodvana-0.1.6/prodvana/proto/prodvana/auth/auth_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-02 21:20:34.053790 prodvana-0.1.6/prodvana/proto/prodvana/blobs/__init__.py
--rw-r--r--   0        0        0     2876 2023-06-02 21:20:33.761790 prodvana-0.1.6/prodvana/proto/prodvana/blobs/blobs_manager_pb2.py
--rw-r--r--   0        0        0     1129 2023-06-02 21:20:33.965790 prodvana-0.1.6/prodvana/proto/prodvana/blobs/blobs_manager_pb2.pyi
--rw-r--r--   0        0        0     2704 2023-06-02 21:20:33.757790 prodvana-0.1.6/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.py
--rw-r--r--   0        0        0      895 2023-06-02 21:20:33.965790 prodvana-0.1.6/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-02 21:20:34.045790 prodvana-0.1.6/prodvana/proto/prodvana/capability/__init__.py
--rw-r--r--   0        0        0     6823 2023-06-02 21:20:33.713790 prodvana-0.1.6/prodvana/proto/prodvana/capability/capability_pb2.py
--rw-r--r--   0        0        0     5455 2023-06-02 21:20:33.921790 prodvana-0.1.6/prodvana/proto/prodvana/capability/capability_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.713790 prodvana-0.1.6/prodvana/proto/prodvana/capability/capability_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.921790 prodvana-0.1.6/prodvana/proto/prodvana/capability/capability_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-02 21:20:34.033790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/__init__.py
--rw-r--r--   0        0        0     1595 2023-06-02 21:20:33.629790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/dangerous_action_pb2.py
--rw-r--r--   0        0        0      869 2023-06-02 21:20:33.833790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/dangerous_action_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.649790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/dangerous_action_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.845790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/dangerous_action_pb2_grpc.pyi
--rw-r--r--   0        0        0     2659 2023-06-02 21:20:33.637790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/env_pb2.py
--rw-r--r--   0        0        0     2017 2023-06-02 21:20:33.853790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/env_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.625790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/env_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.837790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/env_pb2_grpc.pyi
--rw-r--r--   0        0        0     5636 2023-06-02 21:20:33.649790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/helm_pb2.py
--rw-r--r--   0        0        0     5454 2023-06-02 21:20:33.829790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/helm_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.641790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/helm_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.853790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/helm_pb2_grpc.pyi
--rw-r--r--   0        0        0     3658 2023-06-02 21:20:33.641790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.py
--rw-r--r--   0        0        0     4110 2023-06-02 21:20:33.857790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.653790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/kubernetes_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.841790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/kubernetes_config_pb2_grpc.pyi
--rw-r--r--   0        0        0     1890 2023-06-02 21:20:33.633790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/links_pb2.py
--rw-r--r--   0        0        0      846 2023-06-02 21:20:33.841790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/links_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.657790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/links_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.837790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/links_pb2_grpc.pyi
--rw-r--r--   0        0        0     1384 2023-06-02 21:20:33.633790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/maturity_pb2.py
--rw-r--r--   0        0        0     1103 2023-06-02 21:20:33.837790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/maturity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.629790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/maturity_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.857790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/maturity_pb2_grpc.pyi
--rw-r--r--   0        0        0     2541 2023-06-02 21:20:33.625790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/meta_pb2.py
--rw-r--r--   0        0        0     2531 2023-06-02 21:20:33.849790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/meta_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.645790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/meta_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.849790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/meta_pb2_grpc.pyi
--rw-r--r--   0        0        0     2516 2023-06-02 21:20:33.625790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/notification_pb2.py
--rw-r--r--   0        0        0     1337 2023-06-02 21:20:33.861790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.653790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/notification_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.845790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/notification_pb2_grpc.pyi
--rw-r--r--   0        0        0    12624 2023-06-02 21:20:33.621790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/parameters_pb2.py
--rw-r--r--   0        0        0    10735 2023-06-02 21:20:33.861790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/parameters_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.645790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/parameters_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.853790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/parameters_pb2_grpc.pyi
--rw-r--r--   0        0        0    13928 2023-06-02 21:20:33.633790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/program_pb2.py
--rw-r--r--   0        0        0    15915 2023-06-02 21:20:33.833790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/program_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.621790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/program_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.861790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/program_pb2_grpc.pyi
--rw-r--r--   0        0        0     1837 2023-06-02 21:20:33.653790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/ref_pb2.py
--rw-r--r--   0        0        0      743 2023-06-02 21:20:33.845790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/ref_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.637790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/ref_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.841790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/ref_pb2_grpc.pyi
--rw-r--r--   0        0        0     3229 2023-06-02 21:20:33.641790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/retry_pb2.py
--rw-r--r--   0        0        0     2757 2023-06-02 21:20:33.849790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/retry_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.649790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/retry_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.865790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/retry_pb2_grpc.pyi
--rw-r--r--   0        0        0     2192 2023-06-02 21:20:33.637790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/task_pb2.py
--rw-r--r--   0        0        0     1490 2023-06-02 21:20:33.857790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/task_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.629790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/task_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.829790 prodvana-0.1.6/prodvana/proto/prodvana/common_config/task_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-02 21:20:34.041790 prodvana-0.1.6/prodvana/proto/prodvana/config_file/__init__.py
--rw-r--r--   0        0        0     3597 2023-06-02 21:20:33.701790 prodvana-0.1.6/prodvana/proto/prodvana/config_file/config_pb2.py
--rw-r--r--   0        0        0     4171 2023-06-02 21:20:33.909790 prodvana-0.1.6/prodvana/proto/prodvana/config_file/config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.701790 prodvana-0.1.6/prodvana/proto/prodvana/config_file/config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.909790 prodvana-0.1.6/prodvana/proto/prodvana/config_file/config_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-02 21:20:34.053790 prodvana-0.1.6/prodvana/proto/prodvana/config_writeback/__init__.py
--rw-r--r--   0        0        0     1648 2023-06-02 21:20:33.749790 prodvana-0.1.6/prodvana/proto/prodvana/config_writeback/writeback_pb2.py
--rw-r--r--   0        0        0     1131 2023-06-02 21:20:33.957790 prodvana-0.1.6/prodvana/proto/prodvana/config_writeback/writeback_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.749790 prodvana-0.1.6/prodvana/proto/prodvana/config_writeback/writeback_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.957790 prodvana-0.1.6/prodvana/proto/prodvana/config_writeback/writeback_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-02 21:20:34.053790 prodvana-0.1.6/prodvana/proto/prodvana/delivery/__init__.py
--rw-r--r--   0        0        0     2652 2023-06-02 21:20:33.757790 prodvana-0.1.6/prodvana/proto/prodvana/delivery/delivery_config_pb2.py
--rw-r--r--   0        0        0     2294 2023-06-02 21:20:33.961790 prodvana-0.1.6/prodvana/proto/prodvana/delivery/delivery_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.757790 prodvana-0.1.6/prodvana/proto/prodvana/delivery/delivery_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.961790 prodvana-0.1.6/prodvana/proto/prodvana/delivery/delivery_config_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-02 21:20:34.053790 prodvana-0.1.6/prodvana/proto/prodvana/delivery_extension/__init__.py
--rw-r--r--   0        0        0     7053 2023-06-02 21:20:33.761790 prodvana-0.1.6/prodvana/proto/prodvana/delivery_extension/config_pb2.py
--rw-r--r--   0        0        0     6102 2023-06-02 21:20:33.969790 prodvana-0.1.6/prodvana/proto/prodvana/delivery_extension/config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.765790 prodvana-0.1.6/prodvana/proto/prodvana/delivery_extension/config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.965790 prodvana-0.1.6/prodvana/proto/prodvana/delivery_extension/config_pb2_grpc.pyi
--rw-r--r--   0        0        0    11893 2023-06-02 21:20:33.769790 prodvana-0.1.6/prodvana/proto/prodvana/delivery_extension/manager_pb2.py
--rw-r--r--   0        0        0     7309 2023-06-02 21:20:33.969790 prodvana-0.1.6/prodvana/proto/prodvana/delivery_extension/manager_pb2.pyi
--rw-r--r--   0        0        0    11002 2023-06-02 21:20:33.765790 prodvana-0.1.6/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.py
--rw-r--r--   0        0        0     3288 2023-06-02 21:20:33.973790 prodvana-0.1.6/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2686 2023-06-02 21:20:33.761790 prodvana-0.1.6/prodvana/proto/prodvana/delivery_extension/object_pb2.py
--rw-r--r--   0        0        0     1862 2023-06-02 21:20:33.973790 prodvana-0.1.6/prodvana/proto/prodvana/delivery_extension/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.765790 prodvana-0.1.6/prodvana/proto/prodvana/delivery_extension/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.969790 prodvana-0.1.6/prodvana/proto/prodvana/delivery_extension/object_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-02 21:20:34.045790 prodvana-0.1.6/prodvana/proto/prodvana/desired_state/__init__.py
--rw-r--r--   0        0        0    35437 2023-06-02 21:20:33.717790 prodvana-0.1.6/prodvana/proto/prodvana/desired_state/manager_pb2.py
--rw-r--r--   0        0        0    28895 2023-06-02 21:20:33.921790 prodvana-0.1.6/prodvana/proto/prodvana/desired_state/manager_pb2.pyi
--rw-r--r--   0        0        0    20037 2023-06-02 21:20:33.717790 prodvana-0.1.6/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.py
--rw-r--r--   0        0        0     5752 2023-06-02 21:20:33.925790 prodvana-0.1.6/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-02 21:20:34.045790 prodvana-0.1.6/prodvana/proto/prodvana/desired_state/model/__init__.py
--rw-r--r--   0        0        0    41784 2023-06-02 21:20:33.721790 prodvana-0.1.6/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.py
--rw-r--r--   0        0        0    68647 2023-06-02 21:20:33.929790 prodvana-0.1.6/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.721790 prodvana-0.1.6/prodvana/proto/prodvana/desired_state/model/desired_state_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.929790 prodvana-0.1.6/prodvana/proto/prodvana/desired_state/model/desired_state_pb2_grpc.pyi
--rw-r--r--   0        0        0     3895 2023-06-02 21:20:33.717790 prodvana-0.1.6/prodvana/proto/prodvana/desired_state/model/entity_pb2.py
--rw-r--r--   0        0        0     7903 2023-06-02 21:20:33.929790 prodvana-0.1.6/prodvana/proto/prodvana/desired_state/model/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.721790 prodvana-0.1.6/prodvana/proto/prodvana/desired_state/model/entity_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.925790 prodvana-0.1.6/prodvana/proto/prodvana/desired_state/model/entity_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-02 21:20:34.049790 prodvana-0.1.6/prodvana/proto/prodvana/environment/__init__.py
--rw-r--r--   0        0        0    20651 2023-06-02 22:04:33.405790 prodvana-0.1.6/prodvana/proto/prodvana/environment/clusters_pb2.py
--rw-r--r--   0        0        0    27158 2023-06-02 22:04:33.405790 prodvana-0.1.6/prodvana/proto/prodvana/environment/clusters_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.745790 prodvana-0.1.6/prodvana/proto/prodvana/environment/clusters_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.953790 prodvana-0.1.6/prodvana/proto/prodvana/environment/clusters_pb2_grpc.pyi
--rw-r--r--   0        0        0    18211 2023-06-02 21:20:33.745790 prodvana-0.1.6/prodvana/proto/prodvana/environment/environment_manager_pb2.py
--rw-r--r--   0        0        0    14932 2023-06-02 21:20:33.953790 prodvana-0.1.6/prodvana/proto/prodvana/environment/environment_manager_pb2.pyi
--rw-r--r--   0        0        0    17792 2023-06-02 21:20:33.745790 prodvana-0.1.6/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.py
--rw-r--r--   0        0        0     5195 2023-06-02 21:20:33.949790 prodvana-0.1.6/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-02 21:20:34.061790 prodvana-0.1.6/prodvana/proto/prodvana/events/__init__.py
--rw-r--r--   0        0        0     6416 2023-06-02 21:20:33.817790 prodvana-0.1.6/prodvana/proto/prodvana/events/events_manager_pb2.py
--rw-r--r--   0        0        0     5547 2023-06-02 21:20:34.017790 prodvana-0.1.6/prodvana/proto/prodvana/events/events_manager_pb2.pyi
--rw-r--r--   0        0        0     2714 2023-06-02 21:20:33.809790 prodvana-0.1.6/prodvana/proto/prodvana/events/events_manager_pb2_grpc.py
--rw-r--r--   0        0        0      853 2023-06-02 21:20:34.025790 prodvana-0.1.6/prodvana/proto/prodvana/events/events_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     3627 2023-06-02 21:20:33.817790 prodvana-0.1.6/prodvana/proto/prodvana/events/events_pb2.py
--rw-r--r--   0        0        0     4131 2023-06-02 21:20:34.021790 prodvana-0.1.6/prodvana/proto/prodvana/events/events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.817790 prodvana-0.1.6/prodvana/proto/prodvana/events/events_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:34.017790 prodvana-0.1.6/prodvana/proto/prodvana/events/events_pb2_grpc.pyi
--rw-r--r--   0        0        0    15940 2023-06-02 21:20:33.813790 prodvana-0.1.6/prodvana/proto/prodvana/events/types_pb2.py
--rw-r--r--   0        0        0    30800 2023-06-02 21:20:34.017790 prodvana-0.1.6/prodvana/proto/prodvana/events/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.813790 prodvana-0.1.6/prodvana/proto/prodvana/events/types_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:34.021790 prodvana-0.1.6/prodvana/proto/prodvana/events/types_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-02 21:20:34.053790 prodvana-0.1.6/prodvana/proto/prodvana/insights/__init__.py
--rw-r--r--   0        0        0     3041 2023-06-02 21:20:33.753790 prodvana-0.1.6/prodvana/proto/prodvana/insights/insights_pb2.py
--rw-r--r--   0        0        0     3508 2023-06-02 21:20:33.957790 prodvana-0.1.6/prodvana/proto/prodvana/insights/insights_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.753790 prodvana-0.1.6/prodvana/proto/prodvana/insights/insights_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.961790 prodvana-0.1.6/prodvana/proto/prodvana/insights/insights_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-02 21:20:34.041790 prodvana-0.1.6/prodvana/proto/prodvana/managed_resource/__init__.py
--rw-r--r--   0        0        0    14774 2023-06-02 21:20:33.705790 prodvana-0.1.6/prodvana/proto/prodvana/managed_resource/manager_pb2.py
--rw-r--r--   0        0        0    13338 2023-06-02 21:20:33.913790 prodvana-0.1.6/prodvana/proto/prodvana/managed_resource/manager_pb2.pyi
--rw-r--r--   0        0        0    12065 2023-06-02 21:20:33.705790 prodvana-0.1.6/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.py
--rw-r--r--   0        0        0     3657 2023-06-02 21:20:33.913790 prodvana-0.1.6/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-02 21:20:34.061790 prodvana-0.1.6/prodvana/proto/prodvana/metrics/__init__.py
--rw-r--r--   0        0        0     5507 2023-06-02 21:20:33.809790 prodvana-0.1.6/prodvana/proto/prodvana/metrics/metrics_pb2.py
--rw-r--r--   0        0        0     8746 2023-06-02 21:20:34.013790 prodvana-0.1.6/prodvana/proto/prodvana/metrics/metrics_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.809790 prodvana-0.1.6/prodvana/proto/prodvana/metrics/metrics_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:34.013790 prodvana-0.1.6/prodvana/proto/prodvana/metrics/metrics_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-02 21:20:34.057790 prodvana-0.1.6/prodvana/proto/prodvana/object/__init__.py
--rw-r--r--   0        0        0     1844 2023-06-02 21:20:33.777790 prodvana-0.1.6/prodvana/proto/prodvana/object/meta_pb2.py
--rw-r--r--   0        0        0     1957 2023-06-02 21:20:33.981790 prodvana-0.1.6/prodvana/proto/prodvana/object/meta_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.777790 prodvana-0.1.6/prodvana/proto/prodvana/object/meta_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.981790 prodvana-0.1.6/prodvana/proto/prodvana/object/meta_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-02 21:20:34.045790 prodvana-0.1.6/prodvana/proto/prodvana/organization/__init__.py
--rw-r--r--   0        0        0    16162 2023-06-02 21:20:33.729790 prodvana-0.1.6/prodvana/proto/prodvana/organization/organization_manager_pb2.py
--rw-r--r--   0        0        0     9762 2023-06-02 21:20:33.933790 prodvana-0.1.6/prodvana/proto/prodvana/organization/organization_manager_pb2.pyi
--rw-r--r--   0        0        0    14668 2023-06-02 21:20:33.725790 prodvana-0.1.6/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.py
--rw-r--r--   0        0        0     4779 2023-06-02 21:20:33.937790 prodvana-0.1.6/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2859 2023-06-02 21:20:33.729790 prodvana-0.1.6/prodvana/proto/prodvana/organization/user_metadata_pb2.py
--rw-r--r--   0        0        0     1972 2023-06-02 21:20:33.933790 prodvana-0.1.6/prodvana/proto/prodvana/organization/user_metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.725790 prodvana-0.1.6/prodvana/proto/prodvana/organization/user_metadata_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.933790 prodvana-0.1.6/prodvana/proto/prodvana/organization/user_metadata_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-02 21:20:34.037790 prodvana-0.1.6/prodvana/proto/prodvana/pipelines/__init__.py
--rw-r--r--   0        0        0     2598 2023-06-02 21:20:33.693790 prodvana-0.1.6/prodvana/proto/prodvana/pipelines/object_pb2.py
--rw-r--r--   0        0        0     2595 2023-06-02 21:20:33.905790 prodvana-0.1.6/prodvana/proto/prodvana/pipelines/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.693790 prodvana-0.1.6/prodvana/proto/prodvana/pipelines/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.901790 prodvana-0.1.6/prodvana/proto/prodvana/pipelines/object_pb2_grpc.pyi
--rw-r--r--   0        0        0    10003 2023-06-02 21:20:33.697790 prodvana-0.1.6/prodvana/proto/prodvana/pipelines/pipelines_pb2.py
--rw-r--r--   0        0        0    11698 2023-06-02 21:20:33.901790 prodvana-0.1.6/prodvana/proto/prodvana/pipelines/pipelines_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.693790 prodvana-0.1.6/prodvana/proto/prodvana/pipelines/pipelines_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.901790 prodvana-0.1.6/prodvana/proto/prodvana/pipelines/pipelines_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-02 21:20:34.037790 prodvana-0.1.6/prodvana/proto/prodvana/protection/__init__.py
--rw-r--r--   0        0        0     3412 2023-06-02 21:20:33.677790 prodvana-0.1.6/prodvana/proto/prodvana/protection/attachments_pb2.py
--rw-r--r--   0        0        0     2828 2023-06-02 21:20:33.877790 prodvana-0.1.6/prodvana/proto/prodvana/protection/attachments_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.681790 prodvana-0.1.6/prodvana/proto/prodvana/protection/attachments_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.885790 prodvana-0.1.6/prodvana/proto/prodvana/protection/attachments_pb2_grpc.pyi
--rw-r--r--   0        0        0     1907 2023-06-02 21:20:33.669790 prodvana-0.1.6/prodvana/proto/prodvana/protection/object_pb2.py
--rw-r--r--   0        0        0     1545 2023-06-02 21:20:33.889790 prodvana-0.1.6/prodvana/proto/prodvana/protection/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.673790 prodvana-0.1.6/prodvana/proto/prodvana/protection/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.885790 prodvana-0.1.6/prodvana/proto/prodvana/protection/object_pb2_grpc.pyi
--rw-r--r--   0        0        0     8407 2023-06-02 21:20:33.673790 prodvana-0.1.6/prodvana/proto/prodvana/protection/protection_config_pb2.py
--rw-r--r--   0        0        0     8891 2023-06-02 21:20:33.877790 prodvana-0.1.6/prodvana/proto/prodvana/protection/protection_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.677790 prodvana-0.1.6/prodvana/proto/prodvana/protection/protection_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.881790 prodvana-0.1.6/prodvana/proto/prodvana/protection/protection_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    10471 2023-06-02 21:20:33.681790 prodvana-0.1.6/prodvana/proto/prodvana/protection/protection_manager_pb2.py
--rw-r--r--   0        0        0     6767 2023-06-02 21:20:33.881790 prodvana-0.1.6/prodvana/proto/prodvana/protection/protection_manager_pb2.pyi
--rw-r--r--   0        0        0    10450 2023-06-02 21:20:33.669790 prodvana-0.1.6/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.py
--rw-r--r--   0        0        0     3113 2023-06-02 21:20:33.881790 prodvana-0.1.6/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     6409 2023-06-02 21:20:33.677790 prodvana-0.1.6/prodvana/proto/prodvana/protection/protection_reference_pb2.py
--rw-r--r--   0        0        0     4997 2023-06-02 21:20:33.885790 prodvana-0.1.6/prodvana/proto/prodvana/protection/protection_reference_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.673790 prodvana-0.1.6/prodvana/proto/prodvana/protection/protection_reference_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.889790 prodvana-0.1.6/prodvana/proto/prodvana/protection/protection_reference_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-02 21:20:34.037790 prodvana-0.1.6/prodvana/proto/prodvana/release_channel/__init__.py
--rw-r--r--   0        0        0     3574 2023-06-02 21:20:33.685790 prodvana-0.1.6/prodvana/proto/prodvana/release_channel/object_pb2.py
--rw-r--r--   0        0        0     3325 2023-06-02 21:20:33.897790 prodvana-0.1.6/prodvana/proto/prodvana/release_channel/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.685790 prodvana-0.1.6/prodvana/proto/prodvana/release_channel/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.893790 prodvana-0.1.6/prodvana/proto/prodvana/release_channel/object_pb2_grpc.pyi
--rw-r--r--   0        0        0    12100 2023-06-02 22:16:08.617790 prodvana-0.1.6/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.py
--rw-r--r--   0        0        0    12611 2023-06-02 22:16:08.617790 prodvana-0.1.6/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.685790 prodvana-0.1.6/prodvana/proto/prodvana/release_channel/release_channel_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.897790 prodvana-0.1.6/prodvana/proto/prodvana/release_channel/release_channel_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    11989 2023-06-02 21:20:33.689790 prodvana-0.1.6/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.py
--rw-r--r--   0        0        0     7509 2023-06-02 21:20:33.893790 prodvana-0.1.6/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.pyi
--rw-r--r--   0        0        0    13099 2023-06-02 21:20:33.689790 prodvana-0.1.6/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.py
--rw-r--r--   0        0        0     4150 2023-06-02 21:20:33.893790 prodvana-0.1.6/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-02 21:20:34.041790 prodvana-0.1.6/prodvana/proto/prodvana/repo/__init__.py
--rw-r--r--   0        0        0     2441 2023-06-02 21:20:33.709790 prodvana-0.1.6/prodvana/proto/prodvana/repo/repo_pb2.py
--rw-r--r--   0        0        0     2315 2023-06-02 21:20:33.917790 prodvana-0.1.6/prodvana/proto/prodvana/repo/repo_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.705790 prodvana-0.1.6/prodvana/proto/prodvana/repo/repo_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.913790 prodvana-0.1.6/prodvana/proto/prodvana/repo/repo_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-02 21:20:34.061790 prodvana-0.1.6/prodvana/proto/prodvana/runtimes/__init__.py
--rw-r--r--   0        0        0     1551 2023-06-02 21:20:33.801790 prodvana-0.1.6/prodvana/proto/prodvana/runtimes/features_pb2.py
--rw-r--r--   0        0        0     1320 2023-06-02 21:20:34.009790 prodvana-0.1.6/prodvana/proto/prodvana/runtimes/features_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.805790 prodvana-0.1.6/prodvana/proto/prodvana/runtimes/features_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:34.009790 prodvana-0.1.6/prodvana/proto/prodvana/runtimes/features_pb2_grpc.pyi
--rw-r--r--   0        0        0     7542 2023-06-02 21:20:33.805790 prodvana-0.1.6/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.py
--rw-r--r--   0        0        0     6671 2023-06-02 21:20:34.013790 prodvana-0.1.6/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.805790 prodvana-0.1.6/prodvana/proto/prodvana/runtimes/runtimes_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:34.009790 prodvana-0.1.6/prodvana/proto/prodvana/runtimes/runtimes_config_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-02 21:20:34.041790 prodvana-0.1.6/prodvana/proto/prodvana/scm/__init__.py
--rw-r--r--   0        0        0     1265 2023-06-02 21:20:33.709790 prodvana-0.1.6/prodvana/proto/prodvana/scm/types_pb2.py
--rw-r--r--   0        0        0      914 2023-06-02 21:20:33.917790 prodvana-0.1.6/prodvana/proto/prodvana/scm/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.709790 prodvana-0.1.6/prodvana/proto/prodvana/scm/types_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.917790 prodvana-0.1.6/prodvana/proto/prodvana/scm/types_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-02 21:20:34.057790 prodvana-0.1.6/prodvana/proto/prodvana/secrets/__init__.py
--rw-r--r--   0        0        0    10074 2023-06-02 21:20:33.781790 prodvana-0.1.6/prodvana/proto/prodvana/secrets/secrets_manager_pb2.py
--rw-r--r--   0        0        0     4586 2023-06-02 21:20:33.985790 prodvana-0.1.6/prodvana/proto/prodvana/secrets/secrets_manager_pb2.pyi
--rw-r--r--   0        0        0     9936 2023-06-02 21:20:33.777790 prodvana-0.1.6/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.py
--rw-r--r--   0        0        0     2847 2023-06-02 21:20:33.985790 prodvana-0.1.6/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-02 21:20:34.061790 prodvana-0.1.6/prodvana/proto/prodvana/service/__init__.py
--rw-r--r--   0        0        0     5498 2023-06-02 21:20:33.785790 prodvana-0.1.6/prodvana/proto/prodvana/service/object_pb2.py
--rw-r--r--   0        0        0     5760 2023-06-02 21:20:34.001790 prodvana-0.1.6/prodvana/proto/prodvana/service/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.785790 prodvana-0.1.6/prodvana/proto/prodvana/service/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.993790 prodvana-0.1.6/prodvana/proto/prodvana/service/object_pb2_grpc.pyi
--rw-r--r--   0        0        0     2655 2023-06-02 21:20:33.781790 prodvana-0.1.6/prodvana/proto/prodvana/service/parameters_pb2.py
--rw-r--r--   0        0        0     2424 2023-06-02 21:20:33.997790 prodvana-0.1.6/prodvana/proto/prodvana/service/parameters_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.793790 prodvana-0.1.6/prodvana/proto/prodvana/service/parameters_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.997790 prodvana-0.1.6/prodvana/proto/prodvana/service/parameters_pb2_grpc.pyi
--rw-r--r--   0        0        0    31345 2023-06-02 21:20:33.789790 prodvana-0.1.6/prodvana/proto/prodvana/service/service_config_pb2.py
--rw-r--r--   0        0        0    44279 2023-06-02 21:20:33.985790 prodvana-0.1.6/prodvana/proto/prodvana/service/service_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.793790 prodvana-0.1.6/prodvana/proto/prodvana/service/service_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.989790 prodvana-0.1.6/prodvana/proto/prodvana/service/service_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    47994 2023-06-02 21:20:33.781790 prodvana-0.1.6/prodvana/proto/prodvana/service/service_manager_pb2.py
--rw-r--r--   0        0        0    38013 2023-06-02 21:20:33.993790 prodvana-0.1.6/prodvana/proto/prodvana/service/service_manager_pb2.pyi
--rw-r--r--   0        0        0    33828 2023-06-02 21:20:33.789790 prodvana-0.1.6/prodvana/proto/prodvana/service/service_manager_pb2_grpc.py
--rw-r--r--   0        0        0     9674 2023-06-02 21:20:33.989790 prodvana-0.1.6/prodvana/proto/prodvana/service/service_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2934 2023-06-02 21:20:33.793790 prodvana-0.1.6/prodvana/proto/prodvana/service/user_metadata_pb2.py
--rw-r--r--   0        0        0     2106 2023-06-02 21:20:33.989790 prodvana-0.1.6/prodvana/proto/prodvana/service/user_metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.789790 prodvana-0.1.6/prodvana/proto/prodvana/service/user_metadata_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.997790 prodvana-0.1.6/prodvana/proto/prodvana/service/user_metadata_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-02 21:20:34.037790 prodvana-0.1.6/prodvana/proto/prodvana/settings/__init__.py
--rw-r--r--   0        0        0        0 2023-06-02 21:20:34.041790 prodvana-0.1.6/prodvana/proto/prodvana/settings/organization/__init__.py
--rw-r--r--   0        0        0     8509 2023-06-02 21:20:33.701790 prodvana-0.1.6/prodvana/proto/prodvana/settings/organization/users_pb2.py
--rw-r--r--   0        0        0     5677 2023-06-02 21:20:33.905790 prodvana-0.1.6/prodvana/proto/prodvana/settings/organization/users_pb2.pyi
--rw-r--r--   0        0        0     8214 2023-06-02 21:20:33.697790 prodvana-0.1.6/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.py
--rw-r--r--   0        0        0     2318 2023-06-02 21:20:33.905790 prodvana-0.1.6/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-02 21:20:34.033790 prodvana-0.1.6/prodvana/proto/prodvana/stat/__init__.py
--rw-r--r--   0        0        0     1530 2023-06-02 21:20:33.621790 prodvana-0.1.6/prodvana/proto/prodvana/stat/efficiency_pb2.py
--rw-r--r--   0        0        0     1156 2023-06-02 21:20:33.825790 prodvana-0.1.6/prodvana/proto/prodvana/stat/efficiency_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.617790 prodvana-0.1.6/prodvana/proto/prodvana/stat/efficiency_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.829790 prodvana-0.1.6/prodvana/proto/prodvana/stat/efficiency_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-02 21:20:34.049790 prodvana-0.1.6/prodvana/proto/prodvana/template/__init__.py
--rw-r--r--   0        0        0     2429 2023-06-02 21:20:33.741790 prodvana-0.1.6/prodvana/proto/prodvana/template/service_pb2.py
--rw-r--r--   0        0        0     1768 2023-06-02 21:20:33.945790 prodvana-0.1.6/prodvana/proto/prodvana/template/service_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.741790 prodvana-0.1.6/prodvana/proto/prodvana/template/service_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.949790 prodvana-0.1.6/prodvana/proto/prodvana/template/service_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-02 21:20:34.057790 prodvana-0.1.6/prodvana/proto/prodvana/users/__init__.py
--rw-r--r--   0        0        0     1505 2023-06-02 21:20:33.773790 prodvana-0.1.6/prodvana/proto/prodvana/users/users_pb2.py
--rw-r--r--   0        0        0     1451 2023-06-02 21:20:33.981790 prodvana-0.1.6/prodvana/proto/prodvana/users/users_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.773790 prodvana-0.1.6/prodvana/proto/prodvana/users/users_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.977790 prodvana-0.1.6/prodvana/proto/prodvana/users/users_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-02 21:20:34.033790 prodvana-0.1.6/prodvana/proto/prodvana/version/__init__.py
--rw-r--r--   0        0        0     2142 2023-06-02 21:20:33.617790 prodvana-0.1.6/prodvana/proto/prodvana/version/source_metadata_pb2.py
--rw-r--r--   0        0        0     2646 2023-06-02 21:20:33.825790 prodvana-0.1.6/prodvana/proto/prodvana/version/source_metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.613790 prodvana-0.1.6/prodvana/proto/prodvana/version/source_metadata_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.825790 prodvana-0.1.6/prodvana/proto/prodvana/version/source_metadata_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-02 21:20:34.049790 prodvana-0.1.6/prodvana/proto/prodvana/volumes/__init__.py
--rw-r--r--   0        0        0     4805 2023-06-02 21:20:33.737790 prodvana-0.1.6/prodvana/proto/prodvana/volumes/volumes_pb2.py
--rw-r--r--   0        0        0     4793 2023-06-02 21:20:33.945790 prodvana-0.1.6/prodvana/proto/prodvana/volumes/volumes_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.737790 prodvana-0.1.6/prodvana/proto/prodvana/volumes/volumes_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.945790 prodvana-0.1.6/prodvana/proto/prodvana/volumes/volumes_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-02 21:20:34.049790 prodvana-0.1.6/prodvana/proto/prodvana/workflow/__init__.py
--rw-r--r--   0        0        0     5412 2023-06-02 21:20:33.733790 prodvana-0.1.6/prodvana/proto/prodvana/workflow/integration_config_pb2.py
--rw-r--r--   0        0        0     4328 2023-06-02 21:20:33.941790 prodvana-0.1.6/prodvana/proto/prodvana/workflow/integration_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.729790 prodvana-0.1.6/prodvana/proto/prodvana/workflow/integration_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:33.941790 prodvana-0.1.6/prodvana/proto/prodvana/workflow/integration_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    69010 2023-06-02 21:20:33.733790 prodvana-0.1.6/prodvana/proto/prodvana/workflow/workflow_manager_pb2.py
--rw-r--r--   0        0        0    50096 2023-06-02 21:20:33.937790 prodvana-0.1.6/prodvana/proto/prodvana/workflow/workflow_manager_pb2.pyi
--rw-r--r--   0        0        0    55859 2023-06-02 21:20:33.737790 prodvana-0.1.6/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.py
--rw-r--r--   0        0        0    16155 2023-06-02 21:20:33.937790 prodvana-0.1.6/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-02 21:20:34.065790 prodvana-0.1.6/prodvana/proto/validate/__init__.py
--rw-r--r--   0        0        0    21204 2023-06-02 21:20:33.821790 prodvana-0.1.6/prodvana/proto/validate/validate_pb2.py
--rw-r--r--   0        0        0    64630 2023-06-02 21:20:34.025790 prodvana-0.1.6/prodvana/proto/validate/validate_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-02 21:20:33.821790 prodvana-0.1.6/prodvana/proto/validate/validate_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-02 21:20:34.025790 prodvana-0.1.6/prodvana/proto/validate/validate_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-05-30 13:39:12.503857 prodvana-0.1.6/prodvana/py.typed
--rw-r--r--   0        0        0        0 2023-05-30 13:39:12.503857 prodvana-0.1.6/prodvana/utils/__init__.py
--rw-r--r--   0        0        0      538 2023-05-30 13:39:12.503857 prodvana-0.1.6/prodvana/utils/desired_states.py
--rw-r--r--   0        0        0     4079 2023-05-30 13:39:12.503857 prodvana-0.1.6/prodvana/utils/service_config.py
--rw-r--r--   0        0        0     7140 2023-05-30 13:39:12.503857 prodvana-0.1.6/prodvana/utils/tests/test_service_config.py
--rw-r--r--   0        0        0      746 2023-06-02 22:28:07.557790 prodvana-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      817 1970-01-01 00:00:00.000000 prodvana-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       81 2023-05-31 21:06:51.269689 prodvana-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 21:06:51.269689 prodvana-0.1.7/prodvana/__init__.py
+-rw-r--r--   0        0        0     3529 2023-05-31 21:06:51.269689 prodvana-0.1.7/prodvana/client.py
+-rw-r--r--   0        0        0        0 2023-06-06 19:13:21.787926 prodvana-0.1.7/prodvana/proto/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 19:13:21.787926 prodvana-0.1.7/prodvana/proto/prodvana/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 19:13:21.799926 prodvana-0.1.7/prodvana/proto/prodvana/agent/__init__.py
+-rw-r--r--   0        0        0    19183 2023-06-06 19:13:21.419926 prodvana-0.1.7/prodvana/proto/prodvana/agent/agent_interaction_pb2.py
+-rw-r--r--   0        0        0    18983 2023-06-06 19:13:21.631926 prodvana-0.1.7/prodvana/proto/prodvana/agent/agent_interaction_pb2.pyi
+-rw-r--r--   0        0        0    22573 2023-06-06 19:13:21.415926 prodvana-0.1.7/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.py
+-rw-r--r--   0        0        0     6760 2023-06-06 19:13:21.631926 prodvana-0.1.7/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 19:13:21.807926 prodvana-0.1.7/prodvana/proto/prodvana/application/__init__.py
+-rw-r--r--   0        0        0     4200 2023-06-06 19:13:21.503926 prodvana-0.1.7/prodvana/proto/prodvana/application/application_config_pb2.py
+-rw-r--r--   0        0        0     4693 2023-06-06 19:13:21.711926 prodvana-0.1.7/prodvana/proto/prodvana/application/application_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.499926 prodvana-0.1.7/prodvana/proto/prodvana/application/application_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.711926 prodvana-0.1.7/prodvana/proto/prodvana/application/application_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    24873 2023-06-06 19:13:21.499926 prodvana-0.1.7/prodvana/proto/prodvana/application/application_manager_pb2.py
+-rw-r--r--   0        0        0    16394 2023-06-06 19:13:21.715926 prodvana-0.1.7/prodvana/proto/prodvana/application/application_manager_pb2.pyi
+-rw-r--r--   0        0        0    22241 2023-06-06 19:13:21.499926 prodvana-0.1.7/prodvana/proto/prodvana/application/application_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     6755 2023-06-06 19:13:21.707926 prodvana-0.1.7/prodvana/proto/prodvana/application/application_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2801 2023-06-06 19:13:21.495926 prodvana-0.1.7/prodvana/proto/prodvana/application/object_pb2.py
+-rw-r--r--   0        0        0     2184 2023-06-06 19:13:21.715926 prodvana-0.1.7/prodvana/proto/prodvana/application/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.503926 prodvana-0.1.7/prodvana/proto/prodvana/application/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.719926 prodvana-0.1.7/prodvana/proto/prodvana/application/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2294 2023-06-06 19:13:21.495926 prodvana-0.1.7/prodvana/proto/prodvana/application/user_metadata_pb2.py
+-rw-r--r--   0        0        0     1670 2023-06-06 19:13:21.715926 prodvana-0.1.7/prodvana/proto/prodvana/application/user_metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.491926 prodvana-0.1.7/prodvana/proto/prodvana/application/user_metadata_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.711926 prodvana-0.1.7/prodvana/proto/prodvana/application/user_metadata_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 19:13:21.799926 prodvana-0.1.7/prodvana/proto/prodvana/auth/__init__.py
+-rw-r--r--   0        0        0    13908 2023-06-06 19:13:21.423926 prodvana-0.1.7/prodvana/proto/prodvana/auth/auth_manager_pb2.py
+-rw-r--r--   0        0        0    10206 2023-06-06 19:13:21.635926 prodvana-0.1.7/prodvana/proto/prodvana/auth/auth_manager_pb2.pyi
+-rw-r--r--   0        0        0    18631 2023-06-06 19:13:21.423926 prodvana-0.1.7/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     6767 2023-06-06 19:13:21.635926 prodvana-0.1.7/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5071 2023-06-06 19:13:21.419926 prodvana-0.1.7/prodvana/proto/prodvana/auth/auth_pb2.py
+-rw-r--r--   0        0        0     5515 2023-06-06 19:13:21.635926 prodvana-0.1.7/prodvana/proto/prodvana/auth/auth_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.419926 prodvana-0.1.7/prodvana/proto/prodvana/auth/auth_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.639926 prodvana-0.1.7/prodvana/proto/prodvana/auth/auth_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 19:13:21.803926 prodvana-0.1.7/prodvana/proto/prodvana/blobs/__init__.py
+-rw-r--r--   0        0        0     2876 2023-06-06 19:13:21.427926 prodvana-0.1.7/prodvana/proto/prodvana/blobs/blobs_manager_pb2.py
+-rw-r--r--   0        0        0     1129 2023-06-06 19:13:21.643926 prodvana-0.1.7/prodvana/proto/prodvana/blobs/blobs_manager_pb2.pyi
+-rw-r--r--   0        0        0     2704 2023-06-06 19:13:21.431926 prodvana-0.1.7/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.py
+-rw-r--r--   0        0        0      895 2023-06-06 19:13:21.643926 prodvana-0.1.7/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 19:13:21.819926 prodvana-0.1.7/prodvana/proto/prodvana/capability/__init__.py
+-rw-r--r--   0        0        0     6823 2023-06-06 19:13:21.547926 prodvana-0.1.7/prodvana/proto/prodvana/capability/capability_pb2.py
+-rw-r--r--   0        0        0     5455 2023-06-06 19:13:21.759926 prodvana-0.1.7/prodvana/proto/prodvana/capability/capability_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.551926 prodvana-0.1.7/prodvana/proto/prodvana/capability/capability_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.763926 prodvana-0.1.7/prodvana/proto/prodvana/capability/capability_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 19:13:21.803926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/__init__.py
+-rw-r--r--   0        0        0     1595 2023-06-06 19:13:21.443926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/dangerous_action_pb2.py
+-rw-r--r--   0        0        0      869 2023-06-06 19:13:21.667926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/dangerous_action_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.467926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/dangerous_action_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.647926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/dangerous_action_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2659 2023-06-06 19:13:21.451926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/env_pb2.py
+-rw-r--r--   0        0        0     2017 2023-06-06 19:13:21.683926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/env_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.459926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/env_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.663926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/env_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5636 2023-06-06 19:13:21.455926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/helm_pb2.py
+-rw-r--r--   0        0        0     5454 2023-06-06 19:13:21.659926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/helm_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.455926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/helm_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.663926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/helm_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3658 2023-06-06 19:13:21.439926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.py
+-rw-r--r--   0        0        0     4110 2023-06-06 19:13:21.671926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.467926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/kubernetes_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.651926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/kubernetes_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1890 2023-06-06 19:13:21.463926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/links_pb2.py
+-rw-r--r--   0        0        0      846 2023-06-06 19:13:21.679926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/links_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.447926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/links_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.663926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/links_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1384 2023-06-06 19:13:21.439926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/maturity_pb2.py
+-rw-r--r--   0        0        0     1103 2023-06-06 19:13:21.679926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/maturity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.435926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/maturity_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.667926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/maturity_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2541 2023-06-06 19:13:21.431926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/meta_pb2.py
+-rw-r--r--   0        0        0     2531 2023-06-06 19:13:21.671926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/meta_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.431926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/meta_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.647926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/meta_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2516 2023-06-06 19:13:21.443926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/notification_pb2.py
+-rw-r--r--   0        0        0     1337 2023-06-06 19:13:21.651926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.451926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/notification_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.655926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/notification_pb2_grpc.pyi
+-rw-r--r--   0        0        0    12624 2023-06-06 19:13:21.463926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/parameters_pb2.py
+-rw-r--r--   0        0        0    10735 2023-06-06 19:13:21.651926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/parameters_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.455926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/parameters_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.683926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/parameters_pb2_grpc.pyi
+-rw-r--r--   0        0        0    13928 2023-06-06 19:13:21.447926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/program_pb2.py
+-rw-r--r--   0        0        0    15915 2023-06-06 19:13:21.659926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/program_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.439926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/program_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.667926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/program_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1837 2023-06-06 19:13:21.459926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/ref_pb2.py
+-rw-r--r--   0        0        0      743 2023-06-06 19:13:21.655926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/ref_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.447926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/ref_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.675926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/ref_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3229 2023-06-06 19:13:21.451926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/retry_pb2.py
+-rw-r--r--   0        0        0     2757 2023-06-06 19:13:21.675926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/retry_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.435926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/retry_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.647926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/retry_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2867 2023-06-06 19:24:01.799926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/task_pb2.py
+-rw-r--r--   0        0        0     3495 2023-06-06 19:24:01.799926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/task_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.459926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/task_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.675926 prodvana-0.1.7/prodvana/proto/prodvana/common_config/task_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 19:13:21.823926 prodvana-0.1.7/prodvana/proto/prodvana/config_file/__init__.py
+-rw-r--r--   0        0        0     3597 2023-06-06 19:13:21.563926 prodvana-0.1.7/prodvana/proto/prodvana/config_file/config_pb2.py
+-rw-r--r--   0        0        0     4171 2023-06-06 19:13:21.775926 prodvana-0.1.7/prodvana/proto/prodvana/config_file/config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.563926 prodvana-0.1.7/prodvana/proto/prodvana/config_file/config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.775926 prodvana-0.1.7/prodvana/proto/prodvana/config_file/config_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 19:13:21.823926 prodvana-0.1.7/prodvana/proto/prodvana/config_writeback/__init__.py
+-rw-r--r--   0        0        0     1648 2023-06-06 19:13:21.567926 prodvana-0.1.7/prodvana/proto/prodvana/config_writeback/writeback_pb2.py
+-rw-r--r--   0        0        0     1131 2023-06-06 19:13:21.779926 prodvana-0.1.7/prodvana/proto/prodvana/config_writeback/writeback_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.567926 prodvana-0.1.7/prodvana/proto/prodvana/config_writeback/writeback_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.779926 prodvana-0.1.7/prodvana/proto/prodvana/config_writeback/writeback_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 19:13:21.799926 prodvana-0.1.7/prodvana/proto/prodvana/delivery/__init__.py
+-rw-r--r--   0        0        0     2652 2023-06-06 19:13:21.427926 prodvana-0.1.7/prodvana/proto/prodvana/delivery/delivery_config_pb2.py
+-rw-r--r--   0        0        0     2294 2023-06-06 19:13:21.639926 prodvana-0.1.7/prodvana/proto/prodvana/delivery/delivery_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.423926 prodvana-0.1.7/prodvana/proto/prodvana/delivery/delivery_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.639926 prodvana-0.1.7/prodvana/proto/prodvana/delivery/delivery_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 19:13:21.791926 prodvana-0.1.7/prodvana/proto/prodvana/delivery_extension/__init__.py
+-rw-r--r--   0        0        0     7432 2023-06-06 19:13:21.367926 prodvana-0.1.7/prodvana/proto/prodvana/delivery_extension/config_pb2.py
+-rw-r--r--   0        0        0     6911 2023-06-06 19:13:21.583926 prodvana-0.1.7/prodvana/proto/prodvana/delivery_extension/config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.363926 prodvana-0.1.7/prodvana/proto/prodvana/delivery_extension/config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.579926 prodvana-0.1.7/prodvana/proto/prodvana/delivery_extension/config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    11893 2023-06-06 19:13:21.367926 prodvana-0.1.7/prodvana/proto/prodvana/delivery_extension/manager_pb2.py
+-rw-r--r--   0        0        0     7309 2023-06-06 19:13:21.583926 prodvana-0.1.7/prodvana/proto/prodvana/delivery_extension/manager_pb2.pyi
+-rw-r--r--   0        0        0    11002 2023-06-06 19:13:21.363926 prodvana-0.1.7/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.py
+-rw-r--r--   0        0        0     3288 2023-06-06 19:13:21.575926 prodvana-0.1.7/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2686 2023-06-06 19:13:21.359926 prodvana-0.1.7/prodvana/proto/prodvana/delivery_extension/object_pb2.py
+-rw-r--r--   0        0        0     1862 2023-06-06 19:13:21.579926 prodvana-0.1.7/prodvana/proto/prodvana/delivery_extension/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.367926 prodvana-0.1.7/prodvana/proto/prodvana/delivery_extension/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.583926 prodvana-0.1.7/prodvana/proto/prodvana/delivery_extension/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 19:13:21.791926 prodvana-0.1.7/prodvana/proto/prodvana/desired_state/__init__.py
+-rw-r--r--   0        0        0    35437 2023-06-06 19:13:21.383926 prodvana-0.1.7/prodvana/proto/prodvana/desired_state/manager_pb2.py
+-rw-r--r--   0        0        0    28895 2023-06-06 19:13:21.599926 prodvana-0.1.7/prodvana/proto/prodvana/desired_state/manager_pb2.pyi
+-rw-r--r--   0        0        0    20037 2023-06-06 19:13:21.383926 prodvana-0.1.7/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.py
+-rw-r--r--   0        0        0     5752 2023-06-06 19:13:21.599926 prodvana-0.1.7/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 19:13:21.791926 prodvana-0.1.7/prodvana/proto/prodvana/desired_state/model/__init__.py
+-rw-r--r--   0        0        0    42401 2023-06-06 19:24:01.799926 prodvana-0.1.7/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.py
+-rw-r--r--   0        0        0    70107 2023-06-06 19:24:01.799926 prodvana-0.1.7/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.379926 prodvana-0.1.7/prodvana/proto/prodvana/desired_state/model/desired_state_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.591926 prodvana-0.1.7/prodvana/proto/prodvana/desired_state/model/desired_state_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4037 2023-06-06 19:24:01.803926 prodvana-0.1.7/prodvana/proto/prodvana/desired_state/model/entity_pb2.py
+-rw-r--r--   0        0        0     7935 2023-06-06 19:24:01.803926 prodvana-0.1.7/prodvana/proto/prodvana/desired_state/model/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.379926 prodvana-0.1.7/prodvana/proto/prodvana/desired_state/model/entity_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.595926 prodvana-0.1.7/prodvana/proto/prodvana/desired_state/model/entity_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 19:13:21.803926 prodvana-0.1.7/prodvana/proto/prodvana/environment/__init__.py
+-rw-r--r--   0        0        0    20651 2023-06-06 19:13:21.471926 prodvana-0.1.7/prodvana/proto/prodvana/environment/clusters_pb2.py
+-rw-r--r--   0        0        0    27158 2023-06-06 19:13:21.687926 prodvana-0.1.7/prodvana/proto/prodvana/environment/clusters_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.471926 prodvana-0.1.7/prodvana/proto/prodvana/environment/clusters_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.687926 prodvana-0.1.7/prodvana/proto/prodvana/environment/clusters_pb2_grpc.pyi
+-rw-r--r--   0        0        0    18211 2023-06-06 19:13:21.471926 prodvana-0.1.7/prodvana/proto/prodvana/environment/environment_manager_pb2.py
+-rw-r--r--   0        0        0    14932 2023-06-06 19:13:21.683926 prodvana-0.1.7/prodvana/proto/prodvana/environment/environment_manager_pb2.pyi
+-rw-r--r--   0        0        0    17792 2023-06-06 19:13:21.467926 prodvana-0.1.7/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     5195 2023-06-06 19:13:21.687926 prodvana-0.1.7/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 19:13:21.795926 prodvana-0.1.7/prodvana/proto/prodvana/events/__init__.py
+-rw-r--r--   0        0        0     6416 2023-06-06 19:13:21.387926 prodvana-0.1.7/prodvana/proto/prodvana/events/events_manager_pb2.py
+-rw-r--r--   0        0        0     5547 2023-06-06 19:13:21.607926 prodvana-0.1.7/prodvana/proto/prodvana/events/events_manager_pb2.pyi
+-rw-r--r--   0        0        0     2714 2023-06-06 19:13:21.391926 prodvana-0.1.7/prodvana/proto/prodvana/events/events_manager_pb2_grpc.py
+-rw-r--r--   0        0        0      853 2023-06-06 19:13:21.603926 prodvana-0.1.7/prodvana/proto/prodvana/events/events_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3627 2023-06-06 19:13:21.391926 prodvana-0.1.7/prodvana/proto/prodvana/events/events_pb2.py
+-rw-r--r--   0        0        0     4131 2023-06-06 19:13:21.607926 prodvana-0.1.7/prodvana/proto/prodvana/events/events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.387926 prodvana-0.1.7/prodvana/proto/prodvana/events/events_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.599926 prodvana-0.1.7/prodvana/proto/prodvana/events/events_pb2_grpc.pyi
+-rw-r--r--   0        0        0    15940 2023-06-06 19:13:21.387926 prodvana-0.1.7/prodvana/proto/prodvana/events/types_pb2.py
+-rw-r--r--   0        0        0    30800 2023-06-06 19:13:21.603926 prodvana-0.1.7/prodvana/proto/prodvana/events/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.395926 prodvana-0.1.7/prodvana/proto/prodvana/events/types_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.607926 prodvana-0.1.7/prodvana/proto/prodvana/events/types_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 19:13:21.807926 prodvana-0.1.7/prodvana/proto/prodvana/insights/__init__.py
+-rw-r--r--   0        0        0     3041 2023-06-06 19:13:21.491926 prodvana-0.1.7/prodvana/proto/prodvana/insights/insights_pb2.py
+-rw-r--r--   0        0        0     3508 2023-06-06 19:13:21.707926 prodvana-0.1.7/prodvana/proto/prodvana/insights/insights_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.491926 prodvana-0.1.7/prodvana/proto/prodvana/insights/insights_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.707926 prodvana-0.1.7/prodvana/proto/prodvana/insights/insights_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 19:13:21.811926 prodvana-0.1.7/prodvana/proto/prodvana/managed_resource/__init__.py
+-rw-r--r--   0        0        0    14774 2023-06-06 19:13:21.531926 prodvana-0.1.7/prodvana/proto/prodvana/managed_resource/manager_pb2.py
+-rw-r--r--   0        0        0    13338 2023-06-06 19:13:21.743926 prodvana-0.1.7/prodvana/proto/prodvana/managed_resource/manager_pb2.pyi
+-rw-r--r--   0        0        0    12065 2023-06-06 19:13:21.527926 prodvana-0.1.7/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.py
+-rw-r--r--   0        0        0     3657 2023-06-06 19:13:21.739926 prodvana-0.1.7/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 19:13:21.815926 prodvana-0.1.7/prodvana/proto/prodvana/metrics/__init__.py
+-rw-r--r--   0        0        0     5507 2023-06-06 19:13:21.531926 prodvana-0.1.7/prodvana/proto/prodvana/metrics/metrics_pb2.py
+-rw-r--r--   0        0        0     8746 2023-06-06 19:13:21.743926 prodvana-0.1.7/prodvana/proto/prodvana/metrics/metrics_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.531926 prodvana-0.1.7/prodvana/proto/prodvana/metrics/metrics_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.743926 prodvana-0.1.7/prodvana/proto/prodvana/metrics/metrics_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 19:13:21.795926 prodvana-0.1.7/prodvana/proto/prodvana/object/__init__.py
+-rw-r--r--   0        0        0     1844 2023-06-06 19:13:21.415926 prodvana-0.1.7/prodvana/proto/prodvana/object/meta_pb2.py
+-rw-r--r--   0        0        0     1957 2023-06-06 19:13:21.627926 prodvana-0.1.7/prodvana/proto/prodvana/object/meta_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.415926 prodvana-0.1.7/prodvana/proto/prodvana/object/meta_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.627926 prodvana-0.1.7/prodvana/proto/prodvana/object/meta_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 19:13:21.811926 prodvana-0.1.7/prodvana/proto/prodvana/organization/__init__.py
+-rw-r--r--   0        0        0    16162 2023-06-06 19:13:21.519926 prodvana-0.1.7/prodvana/proto/prodvana/organization/organization_manager_pb2.py
+-rw-r--r--   0        0        0     9762 2023-06-06 19:13:21.731926 prodvana-0.1.7/prodvana/proto/prodvana/organization/organization_manager_pb2.pyi
+-rw-r--r--   0        0        0    14668 2023-06-06 19:13:21.523926 prodvana-0.1.7/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     4779 2023-06-06 19:13:21.735926 prodvana-0.1.7/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2859 2023-06-06 19:13:21.519926 prodvana-0.1.7/prodvana/proto/prodvana/organization/user_metadata_pb2.py
+-rw-r--r--   0        0        0     1972 2023-06-06 19:13:21.735926 prodvana-0.1.7/prodvana/proto/prodvana/organization/user_metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.515926 prodvana-0.1.7/prodvana/proto/prodvana/organization/user_metadata_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.731926 prodvana-0.1.7/prodvana/proto/prodvana/organization/user_metadata_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 19:13:21.791926 prodvana-0.1.7/prodvana/proto/prodvana/pipelines/__init__.py
+-rw-r--r--   0        0        0     2598 2023-06-06 19:13:21.371926 prodvana-0.1.7/prodvana/proto/prodvana/pipelines/object_pb2.py
+-rw-r--r--   0        0        0     2595 2023-06-06 19:13:21.587926 prodvana-0.1.7/prodvana/proto/prodvana/pipelines/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.375926 prodvana-0.1.7/prodvana/proto/prodvana/pipelines/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.591926 prodvana-0.1.7/prodvana/proto/prodvana/pipelines/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0    10003 2023-06-06 19:13:21.371926 prodvana-0.1.7/prodvana/proto/prodvana/pipelines/pipelines_pb2.py
+-rw-r--r--   0        0        0    11698 2023-06-06 19:13:21.587926 prodvana-0.1.7/prodvana/proto/prodvana/pipelines/pipelines_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.371926 prodvana-0.1.7/prodvana/proto/prodvana/pipelines/pipelines_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.587926 prodvana-0.1.7/prodvana/proto/prodvana/pipelines/pipelines_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 19:13:21.795926 prodvana-0.1.7/prodvana/proto/prodvana/protection/__init__.py
+-rw-r--r--   0        0        0     3412 2023-06-06 19:13:21.395926 prodvana-0.1.7/prodvana/proto/prodvana/protection/attachments_pb2.py
+-rw-r--r--   0        0        0     2828 2023-06-06 19:13:21.615926 prodvana-0.1.7/prodvana/proto/prodvana/protection/attachments_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.399926 prodvana-0.1.7/prodvana/proto/prodvana/protection/attachments_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.619926 prodvana-0.1.7/prodvana/proto/prodvana/protection/attachments_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1907 2023-06-06 19:13:21.399926 prodvana-0.1.7/prodvana/proto/prodvana/protection/object_pb2.py
+-rw-r--r--   0        0        0     1545 2023-06-06 19:13:21.615926 prodvana-0.1.7/prodvana/proto/prodvana/protection/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.407926 prodvana-0.1.7/prodvana/proto/prodvana/protection/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.623926 prodvana-0.1.7/prodvana/proto/prodvana/protection/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0     8407 2023-06-06 19:13:21.403926 prodvana-0.1.7/prodvana/proto/prodvana/protection/protection_config_pb2.py
+-rw-r--r--   0        0        0     8891 2023-06-06 19:13:21.611926 prodvana-0.1.7/prodvana/proto/prodvana/protection/protection_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.407926 prodvana-0.1.7/prodvana/proto/prodvana/protection/protection_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.611926 prodvana-0.1.7/prodvana/proto/prodvana/protection/protection_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    10471 2023-06-06 19:13:21.403926 prodvana-0.1.7/prodvana/proto/prodvana/protection/protection_manager_pb2.py
+-rw-r--r--   0        0        0     6767 2023-06-06 19:13:21.619926 prodvana-0.1.7/prodvana/proto/prodvana/protection/protection_manager_pb2.pyi
+-rw-r--r--   0        0        0    10450 2023-06-06 19:13:21.395926 prodvana-0.1.7/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     3113 2023-06-06 19:13:21.623926 prodvana-0.1.7/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6409 2023-06-06 19:13:21.407926 prodvana-0.1.7/prodvana/proto/prodvana/protection/protection_reference_pb2.py
+-rw-r--r--   0        0        0     4997 2023-06-06 19:13:21.611926 prodvana-0.1.7/prodvana/proto/prodvana/protection/protection_reference_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.403926 prodvana-0.1.7/prodvana/proto/prodvana/protection/protection_reference_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.619926 prodvana-0.1.7/prodvana/proto/prodvana/protection/protection_reference_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 19:13:21.819926 prodvana-0.1.7/prodvana/proto/prodvana/release_channel/__init__.py
+-rw-r--r--   0        0        0     3574 2023-06-06 19:13:21.559926 prodvana-0.1.7/prodvana/proto/prodvana/release_channel/object_pb2.py
+-rw-r--r--   0        0        0     3325 2023-06-06 19:13:21.771926 prodvana-0.1.7/prodvana/proto/prodvana/release_channel/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.563926 prodvana-0.1.7/prodvana/proto/prodvana/release_channel/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.775926 prodvana-0.1.7/prodvana/proto/prodvana/release_channel/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0    12100 2023-06-06 19:13:21.559926 prodvana-0.1.7/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.py
+-rw-r--r--   0        0        0    12611 2023-06-06 19:13:21.771926 prodvana-0.1.7/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.555926 prodvana-0.1.7/prodvana/proto/prodvana/release_channel/release_channel_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.767926 prodvana-0.1.7/prodvana/proto/prodvana/release_channel/release_channel_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    11989 2023-06-06 19:13:21.559926 prodvana-0.1.7/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.py
+-rw-r--r--   0        0        0     7509 2023-06-06 19:13:21.771926 prodvana-0.1.7/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.pyi
+-rw-r--r--   0        0        0    13099 2023-06-06 19:13:21.555926 prodvana-0.1.7/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     4150 2023-06-06 19:13:21.767926 prodvana-0.1.7/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 19:13:21.811926 prodvana-0.1.7/prodvana/proto/prodvana/repo/__init__.py
+-rw-r--r--   0        0        0     2441 2023-06-06 19:13:21.515926 prodvana-0.1.7/prodvana/proto/prodvana/repo/repo_pb2.py
+-rw-r--r--   0        0        0     2315 2023-06-06 19:13:21.727926 prodvana-0.1.7/prodvana/proto/prodvana/repo/repo_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.515926 prodvana-0.1.7/prodvana/proto/prodvana/repo/repo_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.731926 prodvana-0.1.7/prodvana/proto/prodvana/repo/repo_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 19:13:21.807926 prodvana-0.1.7/prodvana/proto/prodvana/runtimes/__init__.py
+-rw-r--r--   0        0        0     1551 2023-06-06 19:13:21.507926 prodvana-0.1.7/prodvana/proto/prodvana/runtimes/features_pb2.py
+-rw-r--r--   0        0        0     1320 2023-06-06 19:13:21.727926 prodvana-0.1.7/prodvana/proto/prodvana/runtimes/features_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.511926 prodvana-0.1.7/prodvana/proto/prodvana/runtimes/features_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.727926 prodvana-0.1.7/prodvana/proto/prodvana/runtimes/features_pb2_grpc.pyi
+-rw-r--r--   0        0        0     7542 2023-06-06 19:13:21.511926 prodvana-0.1.7/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.py
+-rw-r--r--   0        0        0     6671 2023-06-06 19:13:21.723926 prodvana-0.1.7/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.511926 prodvana-0.1.7/prodvana/proto/prodvana/runtimes/runtimes_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.723926 prodvana-0.1.7/prodvana/proto/prodvana/runtimes/runtimes_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 19:13:21.815926 prodvana-0.1.7/prodvana/proto/prodvana/scm/__init__.py
+-rw-r--r--   0        0        0     1265 2023-06-06 19:13:21.535926 prodvana-0.1.7/prodvana/proto/prodvana/scm/types_pb2.py
+-rw-r--r--   0        0        0      914 2023-06-06 19:13:21.747926 prodvana-0.1.7/prodvana/proto/prodvana/scm/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.539926 prodvana-0.1.7/prodvana/proto/prodvana/scm/types_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.751926 prodvana-0.1.7/prodvana/proto/prodvana/scm/types_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 19:13:21.811926 prodvana-0.1.7/prodvana/proto/prodvana/secrets/__init__.py
+-rw-r--r--   0        0        0    10074 2023-06-06 19:13:21.523926 prodvana-0.1.7/prodvana/proto/prodvana/secrets/secrets_manager_pb2.py
+-rw-r--r--   0        0        0     4586 2023-06-06 19:13:21.739926 prodvana-0.1.7/prodvana/proto/prodvana/secrets/secrets_manager_pb2.pyi
+-rw-r--r--   0        0        0     9936 2023-06-06 19:13:21.527926 prodvana-0.1.7/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     2847 2023-06-06 19:13:21.735926 prodvana-0.1.7/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 19:13:21.803926 prodvana-0.1.7/prodvana/proto/prodvana/service/__init__.py
+-rw-r--r--   0        0        0     5498 2023-06-06 19:13:21.475926 prodvana-0.1.7/prodvana/proto/prodvana/service/object_pb2.py
+-rw-r--r--   0        0        0     5760 2023-06-06 19:13:21.695926 prodvana-0.1.7/prodvana/proto/prodvana/service/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.487926 prodvana-0.1.7/prodvana/proto/prodvana/service/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.703926 prodvana-0.1.7/prodvana/proto/prodvana/service/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2655 2023-06-06 19:13:21.487926 prodvana-0.1.7/prodvana/proto/prodvana/service/parameters_pb2.py
+-rw-r--r--   0        0        0     2424 2023-06-06 19:13:21.695926 prodvana-0.1.7/prodvana/proto/prodvana/service/parameters_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.483926 prodvana-0.1.7/prodvana/proto/prodvana/service/parameters_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.703926 prodvana-0.1.7/prodvana/proto/prodvana/service/parameters_pb2_grpc.pyi
+-rw-r--r--   0        0        0    34047 2023-06-06 19:24:01.803926 prodvana-0.1.7/prodvana/proto/prodvana/service/service_config_pb2.py
+-rw-r--r--   0        0        0    47738 2023-06-06 19:24:01.803926 prodvana-0.1.7/prodvana/proto/prodvana/service/service_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.479926 prodvana-0.1.7/prodvana/proto/prodvana/service/service_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.699926 prodvana-0.1.7/prodvana/proto/prodvana/service/service_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    47994 2023-06-06 19:13:21.483926 prodvana-0.1.7/prodvana/proto/prodvana/service/service_manager_pb2.py
+-rw-r--r--   0        0        0    38013 2023-06-06 19:13:21.695926 prodvana-0.1.7/prodvana/proto/prodvana/service/service_manager_pb2.pyi
+-rw-r--r--   0        0        0    33828 2023-06-06 19:13:21.479926 prodvana-0.1.7/prodvana/proto/prodvana/service/service_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     9674 2023-06-06 19:13:21.691926 prodvana-0.1.7/prodvana/proto/prodvana/service/service_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2934 2023-06-06 19:13:21.479926 prodvana-0.1.7/prodvana/proto/prodvana/service/user_metadata_pb2.py
+-rw-r--r--   0        0        0     2106 2023-06-06 19:13:21.703926 prodvana-0.1.7/prodvana/proto/prodvana/service/user_metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.475926 prodvana-0.1.7/prodvana/proto/prodvana/service/user_metadata_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.691926 prodvana-0.1.7/prodvana/proto/prodvana/service/user_metadata_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 19:13:21.815926 prodvana-0.1.7/prodvana/proto/prodvana/settings/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 19:13:21.819926 prodvana-0.1.7/prodvana/proto/prodvana/settings/organization/__init__.py
+-rw-r--r--   0        0        0     8509 2023-06-06 19:13:21.547926 prodvana-0.1.7/prodvana/proto/prodvana/settings/organization/users_pb2.py
+-rw-r--r--   0        0        0     5677 2023-06-06 19:13:21.759926 prodvana-0.1.7/prodvana/proto/prodvana/settings/organization/users_pb2.pyi
+-rw-r--r--   0        0        0     8214 2023-06-06 19:13:21.547926 prodvana-0.1.7/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.py
+-rw-r--r--   0        0        0     2318 2023-06-06 19:13:21.759926 prodvana-0.1.7/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 19:13:21.787926 prodvana-0.1.7/prodvana/proto/prodvana/stat/__init__.py
+-rw-r--r--   0        0        0     1530 2023-06-06 19:13:21.359926 prodvana-0.1.7/prodvana/proto/prodvana/stat/efficiency_pb2.py
+-rw-r--r--   0        0        0     1156 2023-06-06 19:13:21.575926 prodvana-0.1.7/prodvana/proto/prodvana/stat/efficiency_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.359926 prodvana-0.1.7/prodvana/proto/prodvana/stat/efficiency_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.575926 prodvana-0.1.7/prodvana/proto/prodvana/stat/efficiency_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 19:13:21.795926 prodvana-0.1.7/prodvana/proto/prodvana/template/__init__.py
+-rw-r--r--   0        0        0     2429 2023-06-06 19:13:21.411926 prodvana-0.1.7/prodvana/proto/prodvana/template/service_pb2.py
+-rw-r--r--   0        0        0     1768 2023-06-06 19:13:21.623926 prodvana-0.1.7/prodvana/proto/prodvana/template/service_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.411926 prodvana-0.1.7/prodvana/proto/prodvana/template/service_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.627926 prodvana-0.1.7/prodvana/proto/prodvana/template/service_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 19:13:21.807926 prodvana-0.1.7/prodvana/proto/prodvana/users/__init__.py
+-rw-r--r--   0        0        0     1505 2023-06-06 19:13:21.507926 prodvana-0.1.7/prodvana/proto/prodvana/users/users_pb2.py
+-rw-r--r--   0        0        0     1451 2023-06-06 19:13:21.723926 prodvana-0.1.7/prodvana/proto/prodvana/users/users_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.503926 prodvana-0.1.7/prodvana/proto/prodvana/users/users_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.719926 prodvana-0.1.7/prodvana/proto/prodvana/users/users_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 19:13:21.815926 prodvana-0.1.7/prodvana/proto/prodvana/version/__init__.py
+-rw-r--r--   0        0        0     2142 2023-06-06 19:13:21.535926 prodvana-0.1.7/prodvana/proto/prodvana/version/source_metadata_pb2.py
+-rw-r--r--   0        0        0     2646 2023-06-06 19:13:21.747926 prodvana-0.1.7/prodvana/proto/prodvana/version/source_metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.535926 prodvana-0.1.7/prodvana/proto/prodvana/version/source_metadata_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.747926 prodvana-0.1.7/prodvana/proto/prodvana/version/source_metadata_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 19:13:21.819926 prodvana-0.1.7/prodvana/proto/prodvana/volumes/__init__.py
+-rw-r--r--   0        0        0     4805 2023-06-06 19:13:21.555926 prodvana-0.1.7/prodvana/proto/prodvana/volumes/volumes_pb2.py
+-rw-r--r--   0        0        0     4793 2023-06-06 19:13:21.763926 prodvana-0.1.7/prodvana/proto/prodvana/volumes/volumes_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.551926 prodvana-0.1.7/prodvana/proto/prodvana/volumes/volumes_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.763926 prodvana-0.1.7/prodvana/proto/prodvana/volumes/volumes_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 19:13:21.815926 prodvana-0.1.7/prodvana/proto/prodvana/workflow/__init__.py
+-rw-r--r--   0        0        0     5412 2023-06-06 19:13:21.543926 prodvana-0.1.7/prodvana/proto/prodvana/workflow/integration_config_pb2.py
+-rw-r--r--   0        0        0     4328 2023-06-06 19:13:21.755926 prodvana-0.1.7/prodvana/proto/prodvana/workflow/integration_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.539926 prodvana-0.1.7/prodvana/proto/prodvana/workflow/integration_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.755926 prodvana-0.1.7/prodvana/proto/prodvana/workflow/integration_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    69010 2023-06-06 19:13:21.539926 prodvana-0.1.7/prodvana/proto/prodvana/workflow/workflow_manager_pb2.py
+-rw-r--r--   0        0        0    50096 2023-06-06 19:13:21.751926 prodvana-0.1.7/prodvana/proto/prodvana/workflow/workflow_manager_pb2.pyi
+-rw-r--r--   0        0        0    55859 2023-06-06 19:13:21.543926 prodvana-0.1.7/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.py
+-rw-r--r--   0        0        0    16155 2023-06-06 19:13:21.755926 prodvana-0.1.7/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-06 19:13:21.823926 prodvana-0.1.7/prodvana/proto/validate/__init__.py
+-rw-r--r--   0        0        0    21204 2023-06-06 19:13:21.571926 prodvana-0.1.7/prodvana/proto/validate/validate_pb2.py
+-rw-r--r--   0        0        0    64630 2023-06-06 19:13:21.783926 prodvana-0.1.7/prodvana/proto/validate/validate_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-06 19:13:21.571926 prodvana-0.1.7/prodvana/proto/validate/validate_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-06 19:13:21.779926 prodvana-0.1.7/prodvana/proto/validate/validate_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-05-31 21:06:51.289690 prodvana-0.1.7/prodvana/py.typed
+-rw-r--r--   0        0        0        0 2023-05-31 21:06:51.289690 prodvana-0.1.7/prodvana/utils/__init__.py
+-rw-r--r--   0        0        0      538 2023-05-31 21:06:51.289690 prodvana-0.1.7/prodvana/utils/desired_states.py
+-rw-r--r--   0        0        0     4079 2023-05-31 21:06:51.289690 prodvana-0.1.7/prodvana/utils/service_config.py
+-rw-r--r--   0        0        0     7140 2023-05-31 21:06:51.289690 prodvana-0.1.7/prodvana/utils/tests/test_service_config.py
+-rw-r--r--   0        0        0      746 2023-06-06 20:21:45.831926 prodvana-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      817 1970-01-01 00:00:00.000000 prodvana-0.1.7/PKG-INFO
```

### Comparing `prodvana-0.1.6/prodvana/client.py` & `prodvana-0.1.7/prodvana/client.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/agent/agent_interaction_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/agent/agent_interaction_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/agent/agent_interaction_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/agent/agent_interaction_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.py` & `prodvana-0.1.7/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/application/application_config_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/application/application_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/application/application_config_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/application/application_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/application/application_manager_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/application/application_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/application/application_manager_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/application/application_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/application/application_manager_pb2_grpc.py` & `prodvana-0.1.7/prodvana/proto/prodvana/application/application_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/application/application_manager_pb2_grpc.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/application/application_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/application/object_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/application/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/application/object_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/application/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/application/user_metadata_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/application/user_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/application/user_metadata_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/application/user_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/auth/auth_manager_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/auth/auth_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/auth/auth_manager_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/auth/auth_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.py` & `prodvana-0.1.7/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/auth/auth_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/auth/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/auth/auth_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/auth/auth_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/blobs/blobs_manager_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/blobs/blobs_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/blobs/blobs_manager_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/blobs/blobs_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.py` & `prodvana-0.1.7/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/capability/capability_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/capability/capability_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/capability/capability_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/capability/capability_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/common_config/dangerous_action_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/common_config/dangerous_action_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/common_config/dangerous_action_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/common_config/dangerous_action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/common_config/env_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/common_config/env_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/common_config/env_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/common_config/env_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/common_config/helm_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/common_config/helm_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/common_config/helm_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/common_config/helm_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/common_config/links_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/common_config/links_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/common_config/links_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/common_config/links_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/common_config/maturity_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/common_config/maturity_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/common_config/maturity_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/common_config/maturity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/common_config/meta_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/common_config/meta_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/common_config/meta_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/common_config/meta_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/common_config/notification_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/common_config/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/common_config/notification_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/common_config/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/common_config/parameters_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/common_config/parameters_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/common_config/parameters_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/common_config/parameters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/common_config/program_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/common_config/program_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/common_config/program_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/common_config/program_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/common_config/ref_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/common_config/ref_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/common_config/ref_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/common_config/ref_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/common_config/retry_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/common_config/retry_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/common_config/retry_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/common_config/retry_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/common_config/task_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/config_writeback/writeback_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,35 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: prodvana/common_config/task.proto
+# source: prodvana/config_writeback/writeback.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
-from prodvana.proto.prodvana.common_config import retry_pb2 as prodvana_dot_common__config_dot_retry__pb2
-from prodvana.proto.prodvana.common_config import program_pb2 as prodvana_dot_common__config_dot_program__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!prodvana/common_config/task.proto\x12\x16prodvana.common_config\x1a\x17validate/validate.proto\x1a\"prodvana/common_config/retry.proto\x1a$prodvana/common_config/program.proto\"\x89\x01\n\nTaskConfig\x12@\n\x07program\x18\x01 \x01(\x0b\x32%.prodvana.common_config.ProgramConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x39\n\x0cretry_config\x18\x02 \x01(\x0b\x32#.prodvana.common_config.RetryConfigBRZPgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/common_configb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)prodvana/config_writeback/writeback.proto\x12\x19prodvana.config_writeback\"A\n\x13\x43onfigWritebackPath\x12\x14\n\x0c\x64isplay_name\x18\x01 \x01(\t\x12\x14\n\x0c\x64isplay_path\x18\x02 \x01(\tBUZSgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/config_writebackb\x06proto3')
 
 
 
-_TASKCONFIG = DESCRIPTOR.message_types_by_name['TaskConfig']
-TaskConfig = _reflection.GeneratedProtocolMessageType('TaskConfig', (_message.Message,), {
-  'DESCRIPTOR' : _TASKCONFIG,
-  '__module__' : 'prodvana.common_config.task_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.common_config.TaskConfig)
+_CONFIGWRITEBACKPATH = DESCRIPTOR.message_types_by_name['ConfigWritebackPath']
+ConfigWritebackPath = _reflection.GeneratedProtocolMessageType('ConfigWritebackPath', (_message.Message,), {
+  'DESCRIPTOR' : _CONFIGWRITEBACKPATH,
+  '__module__' : 'prodvana.config_writeback.writeback_pb2'
+  # @@protoc_insertion_point(class_scope:prodvana.config_writeback.ConfigWritebackPath)
   })
-_sym_db.RegisterMessage(TaskConfig)
+_sym_db.RegisterMessage(ConfigWritebackPath)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'ZPgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/common_config'
-  _TASKCONFIG.fields_by_name['program']._options = None
-  _TASKCONFIG.fields_by_name['program']._serialized_options = b'\372B\005\212\001\002\020\001'
-  _TASKCONFIG._serialized_start=161
-  _TASKCONFIG._serialized_end=298
+  DESCRIPTOR._serialized_options = b'ZSgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/config_writeback'
+  _CONFIGWRITEBACKPATH._serialized_start=72
+  _CONFIGWRITEBACKPATH._serialized_end=137
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/common_config/task_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/delivery_extension/object_pb2.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,52 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import builtins
 import google.protobuf.descriptor
 import google.protobuf.message
-import prodvana.proto.prodvana.common_config.program_pb2
-import prodvana.proto.prodvana.common_config.retry_pb2
+import prodvana.proto.prodvana.delivery_extension.config_pb2
+import prodvana.proto.prodvana.object.meta_pb2
 import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-class TaskConfig(google.protobuf.message.Message):
+class DeliveryExtension(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    PROGRAM_FIELD_NUMBER: builtins.int
-    RETRY_CONFIG_FIELD_NUMBER: builtins.int
+    META_FIELD_NUMBER: builtins.int
+    CONFIG_FIELD_NUMBER: builtins.int
+    STATE_FIELD_NUMBER: builtins.int
     @property
-    def program(self) -> prodvana.proto.prodvana.common_config.program_pb2.ProgramConfig: ...
+    def meta(self) -> prodvana.proto.prodvana.object.meta_pb2.ObjectMeta: ...
     @property
-    def retry_config(self) -> prodvana.proto.prodvana.common_config.retry_pb2.RetryConfig:
-        """If not set, the task will not be retried once it starts executing once."""
+    def config(self) -> prodvana.proto.prodvana.delivery_extension.config_pb2.DeliveryExtensionConfig: ...
+    @property
+    def state(self) -> global___DeliveryExtensionState: ...
     def __init__(
         self,
         *,
-        program: prodvana.proto.prodvana.common_config.program_pb2.ProgramConfig | None = ...,
-        retry_config: prodvana.proto.prodvana.common_config.retry_pb2.RetryConfig | None = ...,
+        meta: prodvana.proto.prodvana.object.meta_pb2.ObjectMeta | None = ...,
+        config: prodvana.proto.prodvana.delivery_extension.config_pb2.DeliveryExtensionConfig | None = ...,
+        state: global___DeliveryExtensionState | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["config", b"config", "meta", b"meta", "state", b"state"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["config", b"config", "meta", b"meta", "state", b"state"]) -> None: ...
+
+global___DeliveryExtension = DeliveryExtension
+
+class DeliveryExtensionState(google.protobuf.message.Message):
+    """TODO(naphat) list custom task instances?"""
+
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    def __init__(
+        self,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["program", b"program", "retry_config", b"retry_config"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["program", b"program", "retry_config", b"retry_config"]) -> None: ...
 
-global___TaskConfig = TaskConfig
+global___DeliveryExtensionState = DeliveryExtensionState
```

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/config_file/config_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/config_file/config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/config_file/config_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/config_file/config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/config_writeback/writeback_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/object/meta_pb2.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: prodvana/config_writeback/writeback.proto
+# source: prodvana/object/meta.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from prodvana.proto.prodvana.version import source_metadata_pb2 as prodvana_dot_version_dot_source__metadata__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)prodvana/config_writeback/writeback.proto\x12\x19prodvana.config_writeback\"A\n\x13\x43onfigWritebackPath\x12\x14\n\x0c\x64isplay_name\x18\x01 \x01(\t\x12\x14\n\x0c\x64isplay_path\x18\x02 \x01(\tBUZSgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/config_writebackb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1aprodvana/object/meta.proto\x12\x0fprodvana.object\x1a&prodvana/version/source_metadata.proto\"\xb4\x01\n\nObjectMeta\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x16\n\x0e\x63onfig_version\x18\x04 \x01(\t\x12(\n\x06source\x18\x05 \x01(\x0e\x32\x18.prodvana.version.Source\x12\x39\n\x0fsource_metadata\x18\x06 \x01(\x0b\x32 .prodvana.version.SourceMetadataBKZIgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/objectb\x06proto3')
 
 
 
-_CONFIGWRITEBACKPATH = DESCRIPTOR.message_types_by_name['ConfigWritebackPath']
-ConfigWritebackPath = _reflection.GeneratedProtocolMessageType('ConfigWritebackPath', (_message.Message,), {
-  'DESCRIPTOR' : _CONFIGWRITEBACKPATH,
-  '__module__' : 'prodvana.config_writeback.writeback_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.config_writeback.ConfigWritebackPath)
+_OBJECTMETA = DESCRIPTOR.message_types_by_name['ObjectMeta']
+ObjectMeta = _reflection.GeneratedProtocolMessageType('ObjectMeta', (_message.Message,), {
+  'DESCRIPTOR' : _OBJECTMETA,
+  '__module__' : 'prodvana.object.meta_pb2'
+  # @@protoc_insertion_point(class_scope:prodvana.object.ObjectMeta)
   })
-_sym_db.RegisterMessage(ConfigWritebackPath)
+_sym_db.RegisterMessage(ObjectMeta)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'ZSgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/config_writeback'
-  _CONFIGWRITEBACKPATH._serialized_start=72
-  _CONFIGWRITEBACKPATH._serialized_end=137
+  DESCRIPTOR._serialized_options = b'ZIgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/object'
+  _OBJECTMETA._serialized_start=88
+  _OBJECTMETA._serialized_end=268
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/config_writeback/writeback_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/config_writeback/writeback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/delivery/delivery_config_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/delivery/delivery_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/delivery/delivery_config_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/delivery/delivery_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/delivery_extension/config_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/delivery_extension/config_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: prodvana/delivery_extension/config.proto
 """Generated protocol buffer code."""
+from google.protobuf.internal import enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
@@ -16,16 +17,21 @@
 from prodvana.proto.prodvana.common_config import task_pb2 as prodvana_dot_common__config_dot_task__pb2
 from prodvana.proto.prodvana.common_config import env_pb2 as prodvana_dot_common__config_dot_env__pb2
 from prodvana.proto.prodvana.common_config import kubernetes_config_pb2 as prodvana_dot_common__config_dot_kubernetes__config__pb2
 from prodvana.proto.prodvana.common_config import parameters_pb2 as prodvana_dot_common__config_dot_parameters__pb2
 from prodvana.proto.prodvana.runtimes import runtimes_config_pb2 as prodvana_dot_runtimes_dot_runtimes__config__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(prodvana/delivery_extension/config.proto\x12\x1bprodvana.delivery_extension\x1a\x17validate/validate.proto\x1a!prodvana/common_config/task.proto\x1a prodvana/common_config/env.proto\x1a.prodvana/common_config/kubernetes_config.proto\x1a\'prodvana/common_config/parameters.proto\x1a\'prodvana/runtimes/runtimes_config.proto\"\xba\x02\n\x17\x44\x65liveryExtensionConfig\x12\x39\n\x04name\x18\x01 \x01(\tB+\xfa\x42(r&\x10\x01\x18?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$\x12\x39\n\x0btask_config\x18\x02 \x01(\x0b\x32\".prodvana.common_config.TaskConfigH\x00\x12\x45\n\x11kubernetes_config\x18\x03 \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12N\n\nparameters\x18\x04 \x03(\x0b\x32+.prodvana.common_config.ParameterDefinitionB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x42\x12\n\x0b\x65xec_config\x12\x03\xf8\x42\x01\"\x98\x01\n\x1f\x44\x65liveryExtensionInstanceConfig\x12\x39\n\x04name\x18\x01 \x01(\tB+\xfa\x42(r&\x10\x01\x18?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$\x12:\n\nparameters\x18\x03 \x03(\x0b\x32&.prodvana.common_config.ParameterValue\"\xcf\x03\n\'CompiledDeliveryExtensionInstanceConfig\x12H\n\ndefinition\x18\x01 \x01(\x0b\x32\x34.prodvana.delivery_extension.DeliveryExtensionConfig\x12\x44\n\x11runtime_execution\x18\x02 \x01(\x0b\x32).prodvana.runtimes.RuntimeExecutionConfig\x12\x83\x01\n\x03\x65nv\x18\x03 \x03(\x0b\x32M.prodvana.delivery_extension.CompiledDeliveryExtensionInstanceConfig.EnvEntryB\'\xfa\x42$\x9a\x01!\x18\x01\"\x1dr\x1b\x32\x19^[a-zA-Z_]+[a-zA-Z0-9_]*$\x12@\n\x10parameter_values\x18\x04 \x03(\x0b\x32&.prodvana.common_config.ParameterValue\x1aL\n\x08\x45nvEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .prodvana.common_config.EnvValue:\x02\x38\x01\x42WZUgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/delivery_extensionb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(prodvana/delivery_extension/config.proto\x12\x1bprodvana.delivery_extension\x1a\x17validate/validate.proto\x1a!prodvana/common_config/task.proto\x1a prodvana/common_config/env.proto\x1a.prodvana/common_config/kubernetes_config.proto\x1a\'prodvana/common_config/parameters.proto\x1a\'prodvana/runtimes/runtimes_config.proto\"\xbb\x02\n\x17\x44\x65liveryExtensionConfig\x12:\n\x04name\x18\x01 \x01(\tB,\xfa\x42)r\'\x10\x00\x18?2!^[a-z]?([a-z0-9-]*[a-z0-9]){0,1}$\x12\x39\n\x0btask_config\x18\x02 \x01(\x0b\x32\".prodvana.common_config.TaskConfigH\x00\x12\x45\n\x11kubernetes_config\x18\x03 \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12N\n\nparameters\x18\x04 \x03(\x0b\x32+.prodvana.common_config.ParameterDefinitionB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x42\x12\n\x0b\x65xec_config\x12\x03\xf8\x42\x01\"\x98\x01\n\x1f\x44\x65liveryExtensionInstanceConfig\x12\x39\n\x04name\x18\x01 \x01(\tB+\xfa\x42(r&\x10\x01\x18?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$\x12:\n\nparameters\x18\x03 \x03(\x0b\x32&.prodvana.common_config.ParameterValue\"\xcf\x03\n\'CompiledDeliveryExtensionInstanceConfig\x12H\n\ndefinition\x18\x01 \x01(\x0b\x32\x34.prodvana.delivery_extension.DeliveryExtensionConfig\x12\x44\n\x11runtime_execution\x18\x02 \x01(\x0b\x32).prodvana.runtimes.RuntimeExecutionConfig\x12\x83\x01\n\x03\x65nv\x18\x03 \x03(\x0b\x32M.prodvana.delivery_extension.CompiledDeliveryExtensionInstanceConfig.EnvEntryB\'\xfa\x42$\x9a\x01!\x18\x01\"\x1dr\x1b\x32\x19^[a-zA-Z_]+[a-zA-Z0-9_]*$\x12@\n\x10parameter_values\x18\x04 \x03(\x0b\x32&.prodvana.common_config.ParameterValue\x1aL\n\x08\x45nvEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .prodvana.common_config.EnvValue:\x02\x38\x01*@\n\x04Type\x12\x10\n\x0cUNKNOWN_TYPE\x10\x00\x12\x17\n\x13GLOBAL_USER_CREATED\x10\x01\x12\r\n\tEPHEMERAL\x10\x02\x42WZUgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/delivery_extensionb\x06proto3')
 
+_TYPE = DESCRIPTOR.enum_types_by_name['Type']
+Type = enum_type_wrapper.EnumTypeWrapper(_TYPE)
+UNKNOWN_TYPE = 0
+GLOBAL_USER_CREATED = 1
+EPHEMERAL = 2
 
 
 _DELIVERYEXTENSIONCONFIG = DESCRIPTOR.message_types_by_name['DeliveryExtensionConfig']
 _DELIVERYEXTENSIONINSTANCECONFIG = DESCRIPTOR.message_types_by_name['DeliveryExtensionInstanceConfig']
 _COMPILEDDELIVERYEXTENSIONINSTANCECONFIG = DESCRIPTOR.message_types_by_name['CompiledDeliveryExtensionInstanceConfig']
 _COMPILEDDELIVERYEXTENSIONINSTANCECONFIG_ENVENTRY = _COMPILEDDELIVERYEXTENSIONINSTANCECONFIG.nested_types_by_name['EnvEntry']
 DeliveryExtensionConfig = _reflection.GeneratedProtocolMessageType('DeliveryExtensionConfig', (_message.Message,), {
@@ -60,25 +66,27 @@
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZUgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/delivery_extension'
   _DELIVERYEXTENSIONCONFIG.oneofs_by_name['exec_config']._options = None
   _DELIVERYEXTENSIONCONFIG.oneofs_by_name['exec_config']._serialized_options = b'\370B\001'
   _DELIVERYEXTENSIONCONFIG.fields_by_name['name']._options = None
-  _DELIVERYEXTENSIONCONFIG.fields_by_name['name']._serialized_options = b'\372B(r&\020\001\030?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$'
+  _DELIVERYEXTENSIONCONFIG.fields_by_name['name']._serialized_options = b'\372B)r\'\020\000\030?2!^[a-z]?([a-z0-9-]*[a-z0-9]){0,1}$'
   _DELIVERYEXTENSIONCONFIG.fields_by_name['parameters']._options = None
   _DELIVERYEXTENSIONCONFIG.fields_by_name['parameters']._serialized_options = b'\372B\n\222\001\007\"\005\212\001\002\020\001'
   _DELIVERYEXTENSIONINSTANCECONFIG.fields_by_name['name']._options = None
   _DELIVERYEXTENSIONINSTANCECONFIG.fields_by_name['name']._serialized_options = b'\372B(r&\020\001\030?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$'
   _COMPILEDDELIVERYEXTENSIONINSTANCECONFIG_ENVENTRY._options = None
   _COMPILEDDELIVERYEXTENSIONINSTANCECONFIG_ENVENTRY._serialized_options = b'8\001'
   _COMPILEDDELIVERYEXTENSIONINSTANCECONFIG.fields_by_name['env']._options = None
   _COMPILEDDELIVERYEXTENSIONINSTANCECONFIG.fields_by_name['env']._serialized_options = b'\372B$\232\001!\030\001\"\035r\0332\031^[a-zA-Z_]+[a-zA-Z0-9_]*$'
+  _TYPE._serialized_start=1236
+  _TYPE._serialized_end=1300
   _DELIVERYEXTENSIONCONFIG._serialized_start=298
-  _DELIVERYEXTENSIONCONFIG._serialized_end=612
-  _DELIVERYEXTENSIONINSTANCECONFIG._serialized_start=615
-  _DELIVERYEXTENSIONINSTANCECONFIG._serialized_end=767
-  _COMPILEDDELIVERYEXTENSIONINSTANCECONFIG._serialized_start=770
-  _COMPILEDDELIVERYEXTENSIONINSTANCECONFIG._serialized_end=1233
-  _COMPILEDDELIVERYEXTENSIONINSTANCECONFIG_ENVENTRY._serialized_start=1157
-  _COMPILEDDELIVERYEXTENSIONINSTANCECONFIG_ENVENTRY._serialized_end=1233
+  _DELIVERYEXTENSIONCONFIG._serialized_end=613
+  _DELIVERYEXTENSIONINSTANCECONFIG._serialized_start=616
+  _DELIVERYEXTENSIONINSTANCECONFIG._serialized_end=768
+  _COMPILEDDELIVERYEXTENSIONINSTANCECONFIG._serialized_start=771
+  _COMPILEDDELIVERYEXTENSIONINSTANCECONFIG._serialized_end=1234
+  _COMPILEDDELIVERYEXTENSIONINSTANCECONFIG_ENVENTRY._serialized_start=1158
+  _COMPILEDDELIVERYEXTENSIONINSTANCECONFIG_ENVENTRY._serialized_end=1234
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/delivery_extension/config_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/delivery_extension/config_pb2.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -2,29 +2,50 @@
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
+import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
 import prodvana.proto.prodvana.common_config.env_pb2
 import prodvana.proto.prodvana.common_config.kubernetes_config_pb2
 import prodvana.proto.prodvana.common_config.parameters_pb2
 import prodvana.proto.prodvana.common_config.task_pb2
 import prodvana.proto.prodvana.runtimes.runtimes_config_pb2
 import sys
+import typing
 
-if sys.version_info >= (3, 8):
+if sys.version_info >= (3, 10):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
+class _Type:
+    ValueType = typing.NewType("ValueType", builtins.int)
+    V: typing_extensions.TypeAlias = ValueType
+
+class _TypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_Type.ValueType], builtins.type):  # noqa: F821
+    DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
+    UNKNOWN_TYPE: _Type.ValueType  # 0
+    GLOBAL_USER_CREATED: _Type.ValueType  # 1
+    EPHEMERAL: _Type.ValueType  # 2
+    """one-off delivery extensions inlined into other configs"""
+
+class Type(_Type, metaclass=_TypeEnumTypeWrapper): ...
+
+UNKNOWN_TYPE: Type.ValueType  # 0
+GLOBAL_USER_CREATED: Type.ValueType  # 1
+EPHEMERAL: Type.ValueType  # 2
+"""one-off delivery extensions inlined into other configs"""
+global___Type = Type
+
 class DeliveryExtensionConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     NAME_FIELD_NUMBER: builtins.int
     TASK_CONFIG_FIELD_NUMBER: builtins.int
     KUBERNETES_CONFIG_FIELD_NUMBER: builtins.int
     PARAMETERS_FIELD_NUMBER: builtins.int
```

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/delivery_extension/manager_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/delivery_extension/manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/delivery_extension/manager_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/delivery_extension/manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.py` & `prodvana-0.1.7/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/delivery_extension/object_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/delivery_extension/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/delivery_extension/object_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/template/service_pb2.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,42 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import builtins
 import google.protobuf.descriptor
 import google.protobuf.message
-import prodvana.proto.prodvana.delivery_extension.config_pb2
+import google.protobuf.timestamp_pb2
 import prodvana.proto.prodvana.object.meta_pb2
+import prodvana.proto.prodvana.service.service_config_pb2
 import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
-class DeliveryExtension(google.protobuf.message.Message):
+class ServiceTemplate(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     META_FIELD_NUMBER: builtins.int
-    CONFIG_FIELD_NUMBER: builtins.int
-    STATE_FIELD_NUMBER: builtins.int
+    LAST_UPDATE_TIMESTAMP_FIELD_NUMBER: builtins.int
+    SERVICE_CONFIG_FIELD_NUMBER: builtins.int
     @property
     def meta(self) -> prodvana.proto.prodvana.object.meta_pb2.ObjectMeta: ...
     @property
-    def config(self) -> prodvana.proto.prodvana.delivery_extension.config_pb2.DeliveryExtensionConfig: ...
+    def last_update_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
     @property
-    def state(self) -> global___DeliveryExtensionState: ...
+    def service_config(self) -> prodvana.proto.prodvana.service.service_config_pb2.ServiceConfig: ...
     def __init__(
         self,
         *,
         meta: prodvana.proto.prodvana.object.meta_pb2.ObjectMeta | None = ...,
-        config: prodvana.proto.prodvana.delivery_extension.config_pb2.DeliveryExtensionConfig | None = ...,
-        state: global___DeliveryExtensionState | None = ...,
+        last_update_timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
+        service_config: prodvana.proto.prodvana.service.service_config_pb2.ServiceConfig | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["config", b"config", "meta", b"meta", "state", b"state"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["config", b"config", "meta", b"meta", "state", b"state"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["last_update_timestamp", b"last_update_timestamp", "meta", b"meta", "service_config", b"service_config"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["last_update_timestamp", b"last_update_timestamp", "meta", b"meta", "service_config", b"service_config"]) -> None: ...
 
-global___DeliveryExtension = DeliveryExtension
-
-class DeliveryExtensionState(google.protobuf.message.Message):
-    """TODO(naphat) list custom task instances?"""
-
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-    def __init__(
-        self,
-    ) -> None: ...
-
-global___DeliveryExtensionState = DeliveryExtensionState
+global___ServiceTemplate = ServiceTemplate
```

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/desired_state/manager_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/desired_state/manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/desired_state/manager_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/desired_state/manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.py` & `prodvana-0.1.7/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,24 +14,23 @@
 
 
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
 from prodvana.proto.prodvana.common_config import program_pb2 as prodvana_dot_common__config_dot_program__pb2
 from prodvana.proto.prodvana.common_config import retry_pb2 as prodvana_dot_common__config_dot_retry__pb2
+from prodvana.proto.prodvana.common_config import task_pb2 as prodvana_dot_common__config_dot_task__pb2
 from prodvana.proto.prodvana.environment import clusters_pb2 as prodvana_dot_environment_dot_clusters__pb2
 from prodvana.proto.prodvana.protection import protection_reference_pb2 as prodvana_dot_protection_dot_protection__reference__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n0prodvana/desired_state/model/desired_state.proto\x12\x1cprodvana.desired_state.model\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17validate/validate.proto\x1a$prodvana/common_config/program.proto\x1a\"prodvana/common_config/retry.proto\x1a#prodvana/environment/clusters.proto\x1a.prodvana/protection/protection_reference.proto\"p\n\x0eProtectionLink\x12;\n\tlifecycle\x18\x03 \x01(\x0b\x32(.prodvana.protection.ProtectionLifecycle\x12\x15\n\rattachment_id\x18\x04 \x01(\tJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03\"\x93\x06\n\tCondition\x12X\n\x07rc_cond\x18\x01 \x01(\x0b\x32\x45.prodvana.desired_state.model.Condition.ReleaseChannelStableConditionH\x00\x12Q\n\x0fmanual_approval\x18\x02 \x01(\x0b\x32\x36.prodvana.desired_state.model.Condition.ManualApprovalH\x00\x12\\\n\x0b\x63ustom_task\x18\x03 \x01(\x0b\x32\x45.prodvana.desired_state.model.Condition.CustomTaskSuccessfulConditionH\x00\x12\x18\n\x10\x64\x65sired_state_id\x18\x04 \x01(\t\x1a\xa7\x01\n\x1dReleaseChannelStableCondition\x12\x13\n\x0b\x61pplication\x18\x01 \x01(\t\x12\x0f\n\x07service\x18\x02 \x01(\t\x12\x12\n\nservice_id\x18\x03 \x01(\t\x12\x17\n\x0frelease_channel\x18\x04 \x01(\t\x12\x1a\n\x12release_channel_id\x18\x05 \x01(\t\x12\x17\n\x0fservice_version\x18\x06 \x01(\t\x1a\x1f\n\x0eManualApproval\x12\r\n\x05topic\x18\x01 \x01(\t\x1a\x88\x02\n\x1d\x43ustomTaskSuccessfulCondition\x12\x18\n\x10\x63ustom_task_name\x18\x01 \x01(\t\x12\x66\n\nprotection\x18\x02 \x01(\x0b\x32P.prodvana.desired_state.model.Condition.CustomTaskSuccessfulCondition.ProtectionH\x00\x1a[\n\nProtection\x12\x0c\n\x04name\x18\x01 \x01(\t\x12?\n\ttask_type\x18\x03 \x01(\x0e\x32,.prodvana.desired_state.model.CustomTaskTypeB\x08\n\x06sourceB\x0b\n\tcondition\"L\n\nIdentifier\x12\x30\n\x04type\x18\x01 \x01(\x0e\x32\".prodvana.desired_state.model.Type\x12\x0c\n\x04name\x18\x02 \x01(\t\"\xd3\x02\n\x08Metadata\x12>\n\rpreconditions\x18\x01 \x03(\x0b\x32\'.prodvana.desired_state.model.Condition\x12;\n\ninvariants\x18\x02 \x03(\x0b\x32\'.prodvana.desired_state.model.Condition\x12\x36\n\x04self\x18\x03 \x01(\x0b\x32(.prodvana.desired_state.model.Identifier\x12\x18\n\x10\x64\x65sired_state_id\x18\x04 \x01(\t\x12\x1d\n\x15root_desired_state_id\x18\x05 \x01(\t\x12\x46\n\x10protection_links\x18\x06 \x03(\x0b\x32,.prodvana.desired_state.model.ProtectionLinkJ\x04\x08\x07\x10\x08R\x0bprotections\"\xad\x01\n\x11StatusExplanation\x12\x39\n\x07subject\x18\x01 \x01(\x0b\x32(.prodvana.desired_state.model.Identifier\x12:\n\x06reason\x18\x02 \x01(\x0e\x32*.prodvana.desired_state.model.StatusReason\x12\x0f\n\x07message\x18\x03 \x01(\t\x12\x10\n\x08messages\x18\x04 \x03(\t\"\x8b\x01\n\x11\x41\x63tionExplanation\x12&\n\x02ts\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12=\n\x0b\x61\x63tion_type\x18\x02 \x01(\x0e\x32(.prodvana.desired_state.model.ActionType\x12\x0f\n\x07message\x18\x03 \x01(\t\"\xcf\x01\n\x07Version\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x10\n\x08replicas\x18\x02 \x01(\x05\x12\x1a\n\x12\x61vailable_replicas\x18\x08 \x01(\x05\x12\x32\n\x0epush_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06\x61\x63tive\x18\x05 \x01(\x08\x12\x17\n\x0ftarget_replicas\x18\x06 \x01(\x05J\x04\x08\x03\x10\x04J\x04\x08\x07\x10\x08R\tunhealthyR\x11unhealthy_reasons\"\x86\x03\n\x14ServiceInstanceState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x13\n\x0b\x61pplication\x18\x02 \x01(\t\x12\x0f\n\x07service\x18\x03 \x01(\t\x12\x17\n\x0frelease_channel\x18\x04 \x01(\t\x12\x12\n\nservice_id\x18\x08 \x01(\t\x12\x1a\n\x12release_channel_id\x18\t \x01(\t\x12\x37\n\x08versions\x18\x05 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12?\n\x10rollback_version\x18\x06 \x01(\x0b\x32%.prodvana.desired_state.model.Version\x12\x10\n\x08rollback\x18\x07 \x01(\x08\x12=\n\x08\x64\x65livery\x18\n \x01(\x0b\x32+.prodvana.desired_state.model.DeliveryState\"\x9d\x02\n\x0cServiceState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x13\n\x0b\x61pplication\x18\x02 \x01(\t\x12\x0f\n\x07service\x18\x03 \x01(\t\x12\x12\n\nservice_id\x18\x05 \x01(\t\x12L\n\x10release_channels\x18\x06 \x03(\x0b\x32\x32.prodvana.desired_state.model.ServiceInstanceState\x12\x43\n\x0c\x63ustom_tasks\x18\x07 \x03(\x0b\x32-.prodvana.desired_state.model.CustomTaskStateJ\x04\x08\x04\x10\x05J\x04\x08\x08\x10\t\"\xd2\x01\n\x11ServiceGroupState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12<\n\x08services\x18\x02 \x03(\x0b\x32*.prodvana.desired_state.model.ServiceState\x12\x43\n\x0c\x63ustom_tasks\x18\x03 \x03(\x0b\x32-.prodvana.desired_state.model.CustomTaskStateJ\x04\x08\x04\x10\x05\"\xa8\x02\n\x13\x43\x61naryProgressState\x12H\n\x06status\x18\x01 \x01(\x0e\x32\x38.prodvana.desired_state.model.CanaryProgressState.Status\x12 \n\rcanary_weight\x18\x02 \x01(\x05\x42\t\xfa\x42\x06\x1a\x04\x18\x64(\x00\x12+\n\x08\x64uration\x18\x03 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x39\n\x15pause_start_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"=\n\x06Status\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07PENDING\x10\x01\x12\n\n\x06PAUSED\x10\x02\x12\r\n\tCOMPLETED\x10\x03\"\x94\x03\n\rDeliveryState\x12\x18\n\x10\x64\x65sired_state_id\x18\x0c \x01(\t\x12\x42\n\x06status\x18\x08 \x01(\x0e\x32\x32.prodvana.desired_state.model.DeliveryState.Status\x12\x0f\n\x07message\x18\x06 \x01(\t\x12J\n\x0f\x63\x61nary_progress\x18\x0b \x03(\x0b\x32\x31.prodvana.desired_state.model.CanaryProgressState\x12\x11\n\tfirst_run\x18\r \x01(\x08\x12\x12\n\ngeneration\x18\x0e \x01(\t\"q\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x16\n\x12STATUS_PROGRESSING\x10\x01\x12\x11\n\rSTATUS_PAUSED\x10\x02\x12\x12\n\x0eSTATUS_HEALTHY\x10\x03\x12\x14\n\x10STATUS_UNHEALTHY\x10\x04J\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x07\x10\x08J\x04\x08\t\x10\nJ\x04\x08\n\x10\x0b\"V\n\x1bRuntimeExtensionFetchOutput\x12\x37\n\x08versions\x18\x01 \x03(\x0b\x32%.prodvana.desired_state.model.Version\"\xa5\x07\n\rRuntimeObject\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x13\n\x0bobject_type\x18\x02 \x01(\t\x12\x11\n\tnamespace\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x37\n\x08versions\x18\x05 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12\x42\n\x06status\x18\x06 \x01(\x0e\x32\x32.prodvana.desired_state.model.RuntimeObject.Status\x12?\n\x10rollback_version\x18\x07 \x01(\x0b\x32%.prodvana.desired_state.model.Version\x12=\n\x08\x64\x65livery\x18\x08 \x01(\x0b\x32+.prodvana.desired_state.model.DeliveryState\x12\x18\n\x10version_agnostic\x18\n \x01(\x08\x12\x0f\n\x07message\x18\x0c \x01(\t\x12W\n\x11runtime_extension\x18\r \x01(\x0b\x32<.prodvana.desired_state.model.RuntimeObject.RuntimeExtension\x12W\n\x0foutput_blob_ids\x18\x0e \x03(\x0b\x32>.prodvana.desired_state.model.RuntimeObject.OutputBlobIdsEntry\x12+\n\x08interval\x18\x0f \x01(\x0b\x32\x19.google.protobuf.Duration\x12*\n\x07timeout\x18\x10 \x01(\x0b\x32\x19.google.protobuf.Duration\x1a\x65\n\x10RuntimeExtension\x12=\n\x05\x66\x65tch\x18\x01 \x01(\x0b\x32..prodvana.environment.CompiledExtensionCommand\x12\x12\n\nservice_id\x18\x02 \x01(\t\x1a\x34\n\x12OutputBlobIdsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"0\n\x06Status\x12\x0b\n\x07PENDING\x10\x00\x12\r\n\tSUCCEEDED\x10\x01\x12\n\n\x06\x46\x41ILED\x10\x02J\x04\x08\t\x10\nJ\x04\x08\x0b\x10\x0cR\x0eunhealthy_podsR\nstate_hash\"O\n\x0e\x43onditionState\x12=\n\x06status\x18\x01 \x01(\x0e\x32-.prodvana.desired_state.model.ConditionStatus\"\xde\x02\n\x0c\x43ontrolState\x12\x10\n\x08rollback\x18\x01 \x01(\x08\x12I\n\x13precondition_states\x18\x02 \x03(\x0b\x32,.prodvana.desired_state.model.ConditionState\x12\x46\n\x10invariant_states\x18\x03 \x03(\x0b\x32,.prodvana.desired_state.model.ConditionState\x12\x0e\n\x06paused\x18\x04 \x01(\x08\x12L\n\x13status_explanations\x18\x05 \x03(\x0b\x32/.prodvana.desired_state.model.StatusExplanation\x12K\n\x12\x61\x63tion_explanation\x18\x06 \x01(\x0b\x32/.prodvana.desired_state.model.ActionExplanation\"\x9e\x01\n\x13ManualApprovalState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x42\n\x06status\x18\x02 \x01(\x0e\x32\x32.prodvana.desired_state.model.ManualApprovalStatus\x12\r\n\x05topic\x18\x03 \x01(\t\"\xc1\x05\n\x05State\x12=\n\x07service\x18\x01 \x01(\x0b\x32*.prodvana.desired_state.model.ServiceStateH\x00\x12N\n\x10service_instance\x18\x02 \x01(\x0b\x32\x32.prodvana.desired_state.model.ServiceInstanceStateH\x00\x12H\n\rservice_group\x18\x03 \x01(\x0b\x32/.prodvana.desired_state.model.ServiceGroupStateH\x00\x12\x45\n\x0eruntime_object\x18\x04 \x01(\x0b\x32+.prodvana.desired_state.model.RuntimeObjectH\x00\x12L\n\x0fmanual_approval\x18\x05 \x01(\x0b\x32\x31.prodvana.desired_state.model.ManualApprovalStateH\x00\x12\x44\n\x0b\x63ustom_task\x18\x06 \x01(\x0b\x32-.prodvana.desired_state.model.CustomTaskStateH\x00\x12S\n\x15protection_attachment\x18\x07 \x01(\x0b\x32\x32.prodvana.desired_state.model.ProtectionAttachmentH\x00\x12L\n\x0fprotection_link\x18\x08 \x01(\x0b\x32\x31.prodvana.desired_state.model.ProtectionLinkStateH\x00\x12R\n\x12\x64\x65livery_extension\x18\t \x01(\x0b\x32\x34.prodvana.desired_state.model.DeliveryExtensionStateH\x00\x42\r\n\x0bstate_oneof\"\x82\x01\n\x0b\x41nnotations\x12I\n\x0b\x61nnotations\x18\x01 \x03(\x0b\x32\x34.prodvana.desired_state.model.Annotations.Annotation\x1a(\n\nAnnotation\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"\xae\x01\n\x18\x43ustomTaskExecutionState\x12>\n\x06status\x18\x01 \x01(\x0e\x32..prodvana.desired_state.model.CustomTaskStatus\x12\x10\n\x08\x61ttempts\x18\x02 \x01(\x03\x12@\n\x1clatest_attempt_end_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xce\x03\n\x0f\x43ustomTaskState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x15\n\x04name\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x1c\n\x0b\x64\x65scription\x18\x03 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x13\n\x0b\x61pplication\x18\x04 \x01(\t\x12\x16\n\x0e\x61pplication_id\x18\x05 \x01(\t\x12\x17\n\x0frelease_channel\x18\x06 \x01(\t\x12\x1a\n\x12release_channel_id\x18\x07 \x01(\t\x12@\n\x07program\x18\t \x01(\x0b\x32%.prodvana.common_config.ProgramConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12J\n\ntask_state\x18\x0c \x01(\x0b\x32\x36.prodvana.desired_state.model.CustomTaskExecutionState\x12\x39\n\x0cretry_config\x18\r \x01(\x0b\x32#.prodvana.common_config.RetryConfig\x12\x13\n\x0bservice_ids\x18\x0e \x03(\tJ\x04\x08\x08\x10\tJ\x04\x08\n\x10\x0bJ\x04\x08\x0b\x10\x0c\"\xeb\x04\n\x13ProtectionLinkState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12=\n\x06status\x18\x02 \x01(\x0e\x32-.prodvana.desired_state.model.ConditionStatus\x12:\n\x04link\x18\x03 \x01(\x0b\x32,.prodvana.desired_state.model.ProtectionLink\x12\x35\n\x11started_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x35\n\x11stopped_timestamp\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12T\n\x0estopped_reason\x18\x06 \x01(\x0e\x32<.prodvana.desired_state.model.ProtectionLinkState.StopReason\x12;\n\x17\x66irst_success_timestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xa1\x01\n\nStopReason\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x17\n\x13LIFECYCLE_COMPLETED\x10\x01\x12\x12\n\x0eSUCCEEDED_ONCE\x10\x02\x12\x1a\n\x16SUCCEEDED_FOR_DURATION\x10\x03\x12\r\n\tTIMED_OUT\x10\x04\x12\n\n\x06\x46\x41ILED\x10\x05\x12\x0b\n\x07\x44\x45LETED\x10\x06\x12\x15\n\x11MANUALLY_BYPASSED\x10\x07\"\x89\x04\n\x14ProtectionAttachment\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x37\n\x08versions\x18\x02 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12\x46\n\x17last_completed_versions\x18\x05 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12<\n\x18last_completed_timestamp\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12I\n\x15last_completed_status\x18\x07 \x01(\x0e\x32*.prodvana.desired_state.model.SimpleStatus\x12[\n\"last_completed_status_explanations\x18\x08 \x03(\x0b\x32/.prodvana.desired_state.model.StatusExplanation\x12&\n\x1elast_completed_applied_version\x18\t \x01(\t\x12\x15\n\rprotection_id\x18\x03 \x01(\t\x12\x15\n\rattachment_id\x18\x04 \x01(\t\"\xa8\x04\n\x16\x44\x65liveryExtensionState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x37\n\x08versions\x18\x02 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12\x14\n\x0c\x65xtension_id\x18\x03 \x01(\t\x12@\n\x07program\x18\x04 \x01(\x0b\x32%.prodvana.common_config.ProgramConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x39\n\x0cretry_config\x18\x05 \x01(\x0b\x32#.prodvana.common_config.RetryConfig\x12<\n\x18last_completed_timestamp\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12I\n\x15last_completed_status\x18\x07 \x01(\x0e\x32*.prodvana.desired_state.model.SimpleStatus\x12[\n\"last_completed_status_explanations\x18\x08 \x03(\x0b\x32/.prodvana.desired_state.model.StatusExplanation\x12&\n\x1elast_completed_applied_version\x18\t \x01(\t\"\xc6\x02\n\x06Signal\x12\x36\n\x04type\x18\x01 \x01(\x0e\x32(.prodvana.desired_state.model.SignalType\x12Z\n\x12\x64\x65livery_promotion\x18\x02 \x01(\x0b\x32<.prodvana.desired_state.model.Signal.DeliveryPromotionConfigH\x00\x12R\n\x11protection_bypass\x18\x03 \x01(\x0b\x32\x35.prodvana.desired_state.model.Signal.ProtectionBypassH\x00\x1a\x36\n\x17\x44\x65liveryPromotionConfig\x12\r\n\x05stage\x18\x01 \x01(\x03\x12\x0c\n\x04\x66ull\x18\x02 \x01(\x08\x1a\x12\n\x10ProtectionBypassB\x08\n\x06\x63onfig\"?\n\x08\x44\x65\x62ugLog\x12&\n\x02ts\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0b\n\x03log\x18\x02 \x01(\t*\xcb\x01\n\x04Type\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07SERVICE\x10\x01\x12\x14\n\x10SERVICE_INSTANCE\x10\x02\x12\x11\n\rSERVICE_GROUP\x10\x03\x12\x12\n\x0eRUNTIME_OBJECT\x10\x04\x12\x13\n\x0fMANUAL_APPROVAL\x10\x05\x12\x0f\n\x0b\x43USTOM_TASK\x10\x06\x12\x19\n\x15PROTECTION_ATTACHMENT\x10\x07\x12\x13\n\x0fPROTECTION_LINK\x10\x08\x12\x16\n\x12\x44\x45LIVERY_EXTENSION\x10\t*\x83\x01\n\tLifecycle\x12\x15\n\x11UNKNOWN_LIFECYCLE\x10\x00\x12\x15\n\x11\x43ONVERGENCE_START\x10\x01\x12\x10\n\x0cPRE_APPROVAL\x10\x02\x12\x11\n\rPOST_APPROVAL\x10\x03\x12\x0e\n\nDEPLOYMENT\x10\x04\x12\x13\n\x0fPOST_DEPLOYMENT\x10\x05*\x9a\x01\n\x0e\x43ustomTaskType\x12\x1c\n\x18\x43USTOM_TASK_TYPE_UNKNOWN\x10\x00\x12\x15\n\x11PRE_APPROVAL_TASK\x10\x01\x12\x0c\n\x08\x41PPROVAL\x10\x02\x12\x16\n\x12POST_APPROVAL_TASK\x10\x03\x12\x13\n\x0f\x44\x45PLOYMENT_TASK\x10\x04\x12\x18\n\x14POST_DEPLOYMENT_TASK\x10\x05*\xf0\x01\n\x06Status\x12\x12\n\x0eUNKNOWN_STATUS\x10\x00\x12\x0e\n\nCONVERGING\x10\x01\x12\r\n\tCONVERGED\x10\x02\x12\n\n\x06\x46\x41ILED\x10\x03\x12\x10\n\x0cROLLING_BACK\x10\x04\x12\x0f\n\x0bROLLED_BACK\x10\x05\x12\x13\n\x0f\x46\x41ILED_ROLLBACK\x10\x0c\x12\n\n\x06PAUSED\x10\x06\x12\x10\n\x0c\x43HILD_PAUSED\x10\x07\x12\x19\n\x15WAITING_PRECONDITIONS\x10\x08\x12\x0c\n\x08REPLACED\x10\t\x12\x1b\n\x17WAITING_MANUAL_APPROVAL\x10\n\x12\x0b\n\x07\x44\x45LETED\x10\x0b*R\n\x0cSimpleStatus\x12\x0e\n\nSS_UNKNOWN\x10\x00\x12\x11\n\rSS_CONVERGING\x10\x01\x12\x10\n\x0cSS_CONVERGED\x10\x02\x12\r\n\tSS_FAILED\x10\x03*\xec\x01\n\x0cStatusReason\x12\x12\n\x0eREASON_UNKNOWN\x10\x00\x12\x14\n\x10NO_CURRENT_STATE\x10\x01\x12\x10\n\x0c\x41PPLY_FAILED\x10\x02\x12\x12\n\x0eUNHEALTHY_PODS\x10\x03\x12\x11\n\rUPDATING_PODS\x10\x04\x12\x14\n\x10VERSION_MISMATCH\x10\x05\x12\x19\n\x15RUNTIME_OBJECT_FAILED\x10\x06\x12\x18\n\x14PRECONDITIONS_FAILED\x10\x07\x12\x1c\n\x18MANUAL_APPROVAL_REJECTED\x10\x08\x12\x10\n\x0cSTUCK_ENTITY\x10\t*r\n\nActionType\x12\x17\n\x13\x41\x43TION_TYPE_UNKNOWN\x10\x00\x12\x18\n\x14\x41\x43TION_TYPE_APPLYING\x10\x01\x12\x17\n\x13\x41\x43TION_TYPE_APPLIED\x10\x02\x12\x18\n\x14\x41\x43TION_TYPE_COMPLETE\x10\x03*\x96\x01\n\x0f\x43onditionStatus\x12\x1c\n\x18\x43ONDITION_UNKNOWN_STATUS\x10\x00\x12\x15\n\x11\x43ONDITION_PENDING\x10\x01\x12\x17\n\x13\x43ONDITION_SATISFIED\x10\x02\x12\x1f\n\x1b\x43ONDITION_MANUALLY_BYPASSED\x10\x03\x12\x14\n\x10\x43ONDITION_FAILED\x10\x04*?\n\x14ManualApprovalStatus\x12\x0b\n\x07PENDING\x10\x00\x12\x0c\n\x08\x41PPROVED\x10\x01\x12\x0c\n\x08REJECTED\x10\x02*\x85\x01\n\x10\x43ustomTaskStatus\x12\x17\n\x13\x43USTOM_TASK_PENDING\x10\x00\x12\x1a\n\x16\x43USTOM_TASK_SUCCESSFUL\x10\x01\x12!\n\x1d\x43USTOM_TASK_RETRIES_EXHAUSTED\x10\x02\x12\x19\n\x15\x43USTOM_TASK_TIMED_OUT\x10\x03*O\n\nSignalType\x12\x12\n\x0eSIGNAL_UNKNOWN\x10\x00\x12\x16\n\x12\x44\x45LIVERY_PROMOTION\x10\x01\x12\x15\n\x11PROTECTION_BYPASS\x10\x02\x42XZVgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/desired_state/modelb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n0prodvana/desired_state/model/desired_state.proto\x12\x1cprodvana.desired_state.model\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17validate/validate.proto\x1a$prodvana/common_config/program.proto\x1a\"prodvana/common_config/retry.proto\x1a!prodvana/common_config/task.proto\x1a#prodvana/environment/clusters.proto\x1a.prodvana/protection/protection_reference.proto\"p\n\x0eProtectionLink\x12;\n\tlifecycle\x18\x03 \x01(\x0b\x32(.prodvana.protection.ProtectionLifecycle\x12\x15\n\rattachment_id\x18\x04 \x01(\tJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03\"\x93\x06\n\tCondition\x12X\n\x07rc_cond\x18\x01 \x01(\x0b\x32\x45.prodvana.desired_state.model.Condition.ReleaseChannelStableConditionH\x00\x12Q\n\x0fmanual_approval\x18\x02 \x01(\x0b\x32\x36.prodvana.desired_state.model.Condition.ManualApprovalH\x00\x12\\\n\x0b\x63ustom_task\x18\x03 \x01(\x0b\x32\x45.prodvana.desired_state.model.Condition.CustomTaskSuccessfulConditionH\x00\x12\x18\n\x10\x64\x65sired_state_id\x18\x04 \x01(\t\x1a\xa7\x01\n\x1dReleaseChannelStableCondition\x12\x13\n\x0b\x61pplication\x18\x01 \x01(\t\x12\x0f\n\x07service\x18\x02 \x01(\t\x12\x12\n\nservice_id\x18\x03 \x01(\t\x12\x17\n\x0frelease_channel\x18\x04 \x01(\t\x12\x1a\n\x12release_channel_id\x18\x05 \x01(\t\x12\x17\n\x0fservice_version\x18\x06 \x01(\t\x1a\x1f\n\x0eManualApproval\x12\r\n\x05topic\x18\x01 \x01(\t\x1a\x88\x02\n\x1d\x43ustomTaskSuccessfulCondition\x12\x18\n\x10\x63ustom_task_name\x18\x01 \x01(\t\x12\x66\n\nprotection\x18\x02 \x01(\x0b\x32P.prodvana.desired_state.model.Condition.CustomTaskSuccessfulCondition.ProtectionH\x00\x1a[\n\nProtection\x12\x0c\n\x04name\x18\x01 \x01(\t\x12?\n\ttask_type\x18\x03 \x01(\x0e\x32,.prodvana.desired_state.model.CustomTaskTypeB\x08\n\x06sourceB\x0b\n\tcondition\"\xa0\x01\n\x11\x44\x65liveryExtension\x12\x13\n\x0binstance_id\x18\x01 \x01(\t\x12\x38\n\tlifecycle\x18\x02 \x01(\x0e\x32%.prodvana.common_config.TaskLifecycle\x12<\n\nreferences\x18\x03 \x03(\x0b\x32(.prodvana.desired_state.model.Identifier\"L\n\nIdentifier\x12\x30\n\x04type\x18\x01 \x01(\x0e\x32\".prodvana.desired_state.model.Type\x12\x0c\n\x04name\x18\x02 \x01(\t\"\xa1\x03\n\x08Metadata\x12>\n\rpreconditions\x18\x01 \x03(\x0b\x32\'.prodvana.desired_state.model.Condition\x12;\n\ninvariants\x18\x02 \x03(\x0b\x32\'.prodvana.desired_state.model.Condition\x12\x36\n\x04self\x18\x03 \x01(\x0b\x32(.prodvana.desired_state.model.Identifier\x12\x18\n\x10\x64\x65sired_state_id\x18\x04 \x01(\t\x12\x1d\n\x15root_desired_state_id\x18\x05 \x01(\t\x12\x46\n\x10protection_links\x18\x06 \x03(\x0b\x32,.prodvana.desired_state.model.ProtectionLink\x12L\n\x13\x64\x65livery_extensions\x18\x08 \x03(\x0b\x32/.prodvana.desired_state.model.DeliveryExtensionJ\x04\x08\x07\x10\x08R\x0bprotections\"\xad\x01\n\x11StatusExplanation\x12\x39\n\x07subject\x18\x01 \x01(\x0b\x32(.prodvana.desired_state.model.Identifier\x12:\n\x06reason\x18\x02 \x01(\x0e\x32*.prodvana.desired_state.model.StatusReason\x12\x0f\n\x07message\x18\x03 \x01(\t\x12\x10\n\x08messages\x18\x04 \x03(\t\"\x8b\x01\n\x11\x41\x63tionExplanation\x12&\n\x02ts\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12=\n\x0b\x61\x63tion_type\x18\x02 \x01(\x0e\x32(.prodvana.desired_state.model.ActionType\x12\x0f\n\x07message\x18\x03 \x01(\t\"\xcf\x01\n\x07Version\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x10\n\x08replicas\x18\x02 \x01(\x05\x12\x1a\n\x12\x61vailable_replicas\x18\x08 \x01(\x05\x12\x32\n\x0epush_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06\x61\x63tive\x18\x05 \x01(\x08\x12\x17\n\x0ftarget_replicas\x18\x06 \x01(\x05J\x04\x08\x03\x10\x04J\x04\x08\x07\x10\x08R\tunhealthyR\x11unhealthy_reasons\"\x86\x03\n\x14ServiceInstanceState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x13\n\x0b\x61pplication\x18\x02 \x01(\t\x12\x0f\n\x07service\x18\x03 \x01(\t\x12\x17\n\x0frelease_channel\x18\x04 \x01(\t\x12\x12\n\nservice_id\x18\x08 \x01(\t\x12\x1a\n\x12release_channel_id\x18\t \x01(\t\x12\x37\n\x08versions\x18\x05 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12?\n\x10rollback_version\x18\x06 \x01(\x0b\x32%.prodvana.desired_state.model.Version\x12\x10\n\x08rollback\x18\x07 \x01(\x08\x12=\n\x08\x64\x65livery\x18\n \x01(\x0b\x32+.prodvana.desired_state.model.DeliveryState\"\xf0\x02\n\x0cServiceState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x13\n\x0b\x61pplication\x18\x02 \x01(\t\x12\x0f\n\x07service\x18\x03 \x01(\t\x12\x12\n\nservice_id\x18\x05 \x01(\t\x12L\n\x10release_channels\x18\x06 \x03(\x0b\x32\x32.prodvana.desired_state.model.ServiceInstanceState\x12\x43\n\x0c\x63ustom_tasks\x18\x07 \x03(\x0b\x32-.prodvana.desired_state.model.CustomTaskState\x12Q\n\x13\x64\x65livery_extensions\x18\t \x03(\x0b\x32\x34.prodvana.desired_state.model.DeliveryExtensionStateJ\x04\x08\x04\x10\x05J\x04\x08\x08\x10\t\"\xa5\x02\n\x11ServiceGroupState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12<\n\x08services\x18\x02 \x03(\x0b\x32*.prodvana.desired_state.model.ServiceState\x12\x43\n\x0c\x63ustom_tasks\x18\x03 \x03(\x0b\x32-.prodvana.desired_state.model.CustomTaskState\x12Q\n\x13\x64\x65livery_extensions\x18\x05 \x03(\x0b\x32\x34.prodvana.desired_state.model.DeliveryExtensionStateJ\x04\x08\x04\x10\x05\"\xa8\x02\n\x13\x43\x61naryProgressState\x12H\n\x06status\x18\x01 \x01(\x0e\x32\x38.prodvana.desired_state.model.CanaryProgressState.Status\x12 \n\rcanary_weight\x18\x02 \x01(\x05\x42\t\xfa\x42\x06\x1a\x04\x18\x64(\x00\x12+\n\x08\x64uration\x18\x03 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x39\n\x15pause_start_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"=\n\x06Status\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07PENDING\x10\x01\x12\n\n\x06PAUSED\x10\x02\x12\r\n\tCOMPLETED\x10\x03\"\x94\x03\n\rDeliveryState\x12\x18\n\x10\x64\x65sired_state_id\x18\x0c \x01(\t\x12\x42\n\x06status\x18\x08 \x01(\x0e\x32\x32.prodvana.desired_state.model.DeliveryState.Status\x12\x0f\n\x07message\x18\x06 \x01(\t\x12J\n\x0f\x63\x61nary_progress\x18\x0b \x03(\x0b\x32\x31.prodvana.desired_state.model.CanaryProgressState\x12\x11\n\tfirst_run\x18\r \x01(\x08\x12\x12\n\ngeneration\x18\x0e \x01(\t\"q\n\x06Status\x12\x12\n\x0eSTATUS_UNKNOWN\x10\x00\x12\x16\n\x12STATUS_PROGRESSING\x10\x01\x12\x11\n\rSTATUS_PAUSED\x10\x02\x12\x12\n\x0eSTATUS_HEALTHY\x10\x03\x12\x14\n\x10STATUS_UNHEALTHY\x10\x04J\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03J\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x07\x10\x08J\x04\x08\t\x10\nJ\x04\x08\n\x10\x0b\"V\n\x1bRuntimeExtensionFetchOutput\x12\x37\n\x08versions\x18\x01 \x03(\x0b\x32%.prodvana.desired_state.model.Version\"\xa5\x07\n\rRuntimeObject\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x13\n\x0bobject_type\x18\x02 \x01(\t\x12\x11\n\tnamespace\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x37\n\x08versions\x18\x05 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12\x42\n\x06status\x18\x06 \x01(\x0e\x32\x32.prodvana.desired_state.model.RuntimeObject.Status\x12?\n\x10rollback_version\x18\x07 \x01(\x0b\x32%.prodvana.desired_state.model.Version\x12=\n\x08\x64\x65livery\x18\x08 \x01(\x0b\x32+.prodvana.desired_state.model.DeliveryState\x12\x18\n\x10version_agnostic\x18\n \x01(\x08\x12\x0f\n\x07message\x18\x0c \x01(\t\x12W\n\x11runtime_extension\x18\r \x01(\x0b\x32<.prodvana.desired_state.model.RuntimeObject.RuntimeExtension\x12W\n\x0foutput_blob_ids\x18\x0e \x03(\x0b\x32>.prodvana.desired_state.model.RuntimeObject.OutputBlobIdsEntry\x12+\n\x08interval\x18\x0f \x01(\x0b\x32\x19.google.protobuf.Duration\x12*\n\x07timeout\x18\x10 \x01(\x0b\x32\x19.google.protobuf.Duration\x1a\x65\n\x10RuntimeExtension\x12=\n\x05\x66\x65tch\x18\x01 \x01(\x0b\x32..prodvana.environment.CompiledExtensionCommand\x12\x12\n\nservice_id\x18\x02 \x01(\t\x1a\x34\n\x12OutputBlobIdsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"0\n\x06Status\x12\x0b\n\x07PENDING\x10\x00\x12\r\n\tSUCCEEDED\x10\x01\x12\n\n\x06\x46\x41ILED\x10\x02J\x04\x08\t\x10\nJ\x04\x08\x0b\x10\x0cR\x0eunhealthy_podsR\nstate_hash\"O\n\x0e\x43onditionState\x12=\n\x06status\x18\x01 \x01(\x0e\x32-.prodvana.desired_state.model.ConditionStatus\"\xde\x02\n\x0c\x43ontrolState\x12\x10\n\x08rollback\x18\x01 \x01(\x08\x12I\n\x13precondition_states\x18\x02 \x03(\x0b\x32,.prodvana.desired_state.model.ConditionState\x12\x46\n\x10invariant_states\x18\x03 \x03(\x0b\x32,.prodvana.desired_state.model.ConditionState\x12\x0e\n\x06paused\x18\x04 \x01(\x08\x12L\n\x13status_explanations\x18\x05 \x03(\x0b\x32/.prodvana.desired_state.model.StatusExplanation\x12K\n\x12\x61\x63tion_explanation\x18\x06 \x01(\x0b\x32/.prodvana.desired_state.model.ActionExplanation\"\x9e\x01\n\x13ManualApprovalState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x42\n\x06status\x18\x02 \x01(\x0e\x32\x32.prodvana.desired_state.model.ManualApprovalStatus\x12\r\n\x05topic\x18\x03 \x01(\t\"\xc1\x05\n\x05State\x12=\n\x07service\x18\x01 \x01(\x0b\x32*.prodvana.desired_state.model.ServiceStateH\x00\x12N\n\x10service_instance\x18\x02 \x01(\x0b\x32\x32.prodvana.desired_state.model.ServiceInstanceStateH\x00\x12H\n\rservice_group\x18\x03 \x01(\x0b\x32/.prodvana.desired_state.model.ServiceGroupStateH\x00\x12\x45\n\x0eruntime_object\x18\x04 \x01(\x0b\x32+.prodvana.desired_state.model.RuntimeObjectH\x00\x12L\n\x0fmanual_approval\x18\x05 \x01(\x0b\x32\x31.prodvana.desired_state.model.ManualApprovalStateH\x00\x12\x44\n\x0b\x63ustom_task\x18\x06 \x01(\x0b\x32-.prodvana.desired_state.model.CustomTaskStateH\x00\x12S\n\x15protection_attachment\x18\x07 \x01(\x0b\x32\x32.prodvana.desired_state.model.ProtectionAttachmentH\x00\x12L\n\x0fprotection_link\x18\x08 \x01(\x0b\x32\x31.prodvana.desired_state.model.ProtectionLinkStateH\x00\x12R\n\x12\x64\x65livery_extension\x18\t \x01(\x0b\x32\x34.prodvana.desired_state.model.DeliveryExtensionStateH\x00\x42\r\n\x0bstate_oneof\"\x82\x01\n\x0b\x41nnotations\x12I\n\x0b\x61nnotations\x18\x01 \x03(\x0b\x32\x34.prodvana.desired_state.model.Annotations.Annotation\x1a(\n\nAnnotation\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"\xae\x01\n\x18\x43ustomTaskExecutionState\x12>\n\x06status\x18\x01 \x01(\x0e\x32..prodvana.desired_state.model.CustomTaskStatus\x12\x10\n\x08\x61ttempts\x18\x02 \x01(\x03\x12@\n\x1clatest_attempt_end_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xce\x03\n\x0f\x43ustomTaskState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x15\n\x04name\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x1c\n\x0b\x64\x65scription\x18\x03 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x13\n\x0b\x61pplication\x18\x04 \x01(\t\x12\x16\n\x0e\x61pplication_id\x18\x05 \x01(\t\x12\x17\n\x0frelease_channel\x18\x06 \x01(\t\x12\x1a\n\x12release_channel_id\x18\x07 \x01(\t\x12@\n\x07program\x18\t \x01(\x0b\x32%.prodvana.common_config.ProgramConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12J\n\ntask_state\x18\x0c \x01(\x0b\x32\x36.prodvana.desired_state.model.CustomTaskExecutionState\x12\x39\n\x0cretry_config\x18\r \x01(\x0b\x32#.prodvana.common_config.RetryConfig\x12\x13\n\x0bservice_ids\x18\x0e \x03(\tJ\x04\x08\x08\x10\tJ\x04\x08\n\x10\x0bJ\x04\x08\x0b\x10\x0c\"\xeb\x04\n\x13ProtectionLinkState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12=\n\x06status\x18\x02 \x01(\x0e\x32-.prodvana.desired_state.model.ConditionStatus\x12:\n\x04link\x18\x03 \x01(\x0b\x32,.prodvana.desired_state.model.ProtectionLink\x12\x35\n\x11started_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x35\n\x11stopped_timestamp\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12T\n\x0estopped_reason\x18\x06 \x01(\x0e\x32<.prodvana.desired_state.model.ProtectionLinkState.StopReason\x12;\n\x17\x66irst_success_timestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xa1\x01\n\nStopReason\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x17\n\x13LIFECYCLE_COMPLETED\x10\x01\x12\x12\n\x0eSUCCEEDED_ONCE\x10\x02\x12\x1a\n\x16SUCCEEDED_FOR_DURATION\x10\x03\x12\r\n\tTIMED_OUT\x10\x04\x12\n\n\x06\x46\x41ILED\x10\x05\x12\x0b\n\x07\x44\x45LETED\x10\x06\x12\x15\n\x11MANUALLY_BYPASSED\x10\x07\"\x89\x04\n\x14ProtectionAttachment\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x37\n\x08versions\x18\x02 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12\x46\n\x17last_completed_versions\x18\x05 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12<\n\x18last_completed_timestamp\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12I\n\x15last_completed_status\x18\x07 \x01(\x0e\x32*.prodvana.desired_state.model.SimpleStatus\x12[\n\"last_completed_status_explanations\x18\x08 \x03(\x0b\x32/.prodvana.desired_state.model.StatusExplanation\x12&\n\x1elast_completed_applied_version\x18\t \x01(\t\x12\x15\n\rprotection_id\x18\x03 \x01(\t\x12\x15\n\rattachment_id\x18\x04 \x01(\t\"\x81\x05\n\x16\x44\x65liveryExtensionState\x12\x34\n\x04meta\x18\x01 \x01(\x0b\x32&.prodvana.desired_state.model.Metadata\x12\x37\n\x08versions\x18\x02 \x03(\x0b\x32%.prodvana.desired_state.model.Version\x12\x14\n\x0c\x65xtension_id\x18\x03 \x01(\t\x12\x1d\n\x15\x65xtension_instance_id\x18\n \x01(\t\x12\x38\n\tlifecycle\x18\x0b \x01(\x0e\x32%.prodvana.common_config.TaskLifecycle\x12<\n\x18last_completed_timestamp\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12I\n\x15last_completed_status\x18\x07 \x01(\x0e\x32*.prodvana.desired_state.model.SimpleStatus\x12[\n\"last_completed_status_explanations\x18\x08 \x03(\x0b\x32/.prodvana.desired_state.model.StatusExplanation\x12&\n\x1elast_completed_applied_version\x18\t \x01(\t\x12<\n\nreferences\x18\x0c \x03(\x0b\x32(.prodvana.desired_state.model.Identifier\x12=\n\x06status\x18\r \x01(\x0e\x32-.prodvana.desired_state.model.ConditionStatus\"\xc6\x02\n\x06Signal\x12\x36\n\x04type\x18\x01 \x01(\x0e\x32(.prodvana.desired_state.model.SignalType\x12Z\n\x12\x64\x65livery_promotion\x18\x02 \x01(\x0b\x32<.prodvana.desired_state.model.Signal.DeliveryPromotionConfigH\x00\x12R\n\x11protection_bypass\x18\x03 \x01(\x0b\x32\x35.prodvana.desired_state.model.Signal.ProtectionBypassH\x00\x1a\x36\n\x17\x44\x65liveryPromotionConfig\x12\r\n\x05stage\x18\x01 \x01(\x03\x12\x0c\n\x04\x66ull\x18\x02 \x01(\x08\x1a\x12\n\x10ProtectionBypassB\x08\n\x06\x63onfig\"?\n\x08\x44\x65\x62ugLog\x12&\n\x02ts\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0b\n\x03log\x18\x02 \x01(\t*\xcb\x01\n\x04Type\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0b\n\x07SERVICE\x10\x01\x12\x14\n\x10SERVICE_INSTANCE\x10\x02\x12\x11\n\rSERVICE_GROUP\x10\x03\x12\x12\n\x0eRUNTIME_OBJECT\x10\x04\x12\x13\n\x0fMANUAL_APPROVAL\x10\x05\x12\x0f\n\x0b\x43USTOM_TASK\x10\x06\x12\x19\n\x15PROTECTION_ATTACHMENT\x10\x07\x12\x13\n\x0fPROTECTION_LINK\x10\x08\x12\x16\n\x12\x44\x45LIVERY_EXTENSION\x10\t*\x9a\x01\n\x0e\x43ustomTaskType\x12\x1c\n\x18\x43USTOM_TASK_TYPE_UNKNOWN\x10\x00\x12\x15\n\x11PRE_APPROVAL_TASK\x10\x01\x12\x0c\n\x08\x41PPROVAL\x10\x02\x12\x16\n\x12POST_APPROVAL_TASK\x10\x03\x12\x13\n\x0f\x44\x45PLOYMENT_TASK\x10\x04\x12\x18\n\x14POST_DEPLOYMENT_TASK\x10\x05*\xf0\x01\n\x06Status\x12\x12\n\x0eUNKNOWN_STATUS\x10\x00\x12\x0e\n\nCONVERGING\x10\x01\x12\r\n\tCONVERGED\x10\x02\x12\n\n\x06\x46\x41ILED\x10\x03\x12\x10\n\x0cROLLING_BACK\x10\x04\x12\x0f\n\x0bROLLED_BACK\x10\x05\x12\x13\n\x0f\x46\x41ILED_ROLLBACK\x10\x0c\x12\n\n\x06PAUSED\x10\x06\x12\x10\n\x0c\x43HILD_PAUSED\x10\x07\x12\x19\n\x15WAITING_PRECONDITIONS\x10\x08\x12\x0c\n\x08REPLACED\x10\t\x12\x1b\n\x17WAITING_MANUAL_APPROVAL\x10\n\x12\x0b\n\x07\x44\x45LETED\x10\x0b*R\n\x0cSimpleStatus\x12\x0e\n\nSS_UNKNOWN\x10\x00\x12\x11\n\rSS_CONVERGING\x10\x01\x12\x10\n\x0cSS_CONVERGED\x10\x02\x12\r\n\tSS_FAILED\x10\x03*\xec\x01\n\x0cStatusReason\x12\x12\n\x0eREASON_UNKNOWN\x10\x00\x12\x14\n\x10NO_CURRENT_STATE\x10\x01\x12\x10\n\x0c\x41PPLY_FAILED\x10\x02\x12\x12\n\x0eUNHEALTHY_PODS\x10\x03\x12\x11\n\rUPDATING_PODS\x10\x04\x12\x14\n\x10VERSION_MISMATCH\x10\x05\x12\x19\n\x15RUNTIME_OBJECT_FAILED\x10\x06\x12\x18\n\x14PRECONDITIONS_FAILED\x10\x07\x12\x1c\n\x18MANUAL_APPROVAL_REJECTED\x10\x08\x12\x10\n\x0cSTUCK_ENTITY\x10\t*r\n\nActionType\x12\x17\n\x13\x41\x43TION_TYPE_UNKNOWN\x10\x00\x12\x18\n\x14\x41\x43TION_TYPE_APPLYING\x10\x01\x12\x17\n\x13\x41\x43TION_TYPE_APPLIED\x10\x02\x12\x18\n\x14\x41\x43TION_TYPE_COMPLETE\x10\x03*\x96\x01\n\x0f\x43onditionStatus\x12\x1c\n\x18\x43ONDITION_UNKNOWN_STATUS\x10\x00\x12\x15\n\x11\x43ONDITION_PENDING\x10\x01\x12\x17\n\x13\x43ONDITION_SATISFIED\x10\x02\x12\x1f\n\x1b\x43ONDITION_MANUALLY_BYPASSED\x10\x03\x12\x14\n\x10\x43ONDITION_FAILED\x10\x04*?\n\x14ManualApprovalStatus\x12\x0b\n\x07PENDING\x10\x00\x12\x0c\n\x08\x41PPROVED\x10\x01\x12\x0c\n\x08REJECTED\x10\x02*\x85\x01\n\x10\x43ustomTaskStatus\x12\x17\n\x13\x43USTOM_TASK_PENDING\x10\x00\x12\x1a\n\x16\x43USTOM_TASK_SUCCESSFUL\x10\x01\x12!\n\x1d\x43USTOM_TASK_RETRIES_EXHAUSTED\x10\x02\x12\x19\n\x15\x43USTOM_TASK_TIMED_OUT\x10\x03*O\n\nSignalType\x12\x12\n\x0eSIGNAL_UNKNOWN\x10\x00\x12\x16\n\x12\x44\x45LIVERY_PROMOTION\x10\x01\x12\x15\n\x11PROTECTION_BYPASS\x10\x02\x42XZVgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/desired_state/modelb\x06proto3')
 
 _TYPE = DESCRIPTOR.enum_types_by_name['Type']
 Type = enum_type_wrapper.EnumTypeWrapper(_TYPE)
-_LIFECYCLE = DESCRIPTOR.enum_types_by_name['Lifecycle']
-Lifecycle = enum_type_wrapper.EnumTypeWrapper(_LIFECYCLE)
 _CUSTOMTASKTYPE = DESCRIPTOR.enum_types_by_name['CustomTaskType']
 CustomTaskType = enum_type_wrapper.EnumTypeWrapper(_CUSTOMTASKTYPE)
 _STATUS = DESCRIPTOR.enum_types_by_name['Status']
 Status = enum_type_wrapper.EnumTypeWrapper(_STATUS)
 _SIMPLESTATUS = DESCRIPTOR.enum_types_by_name['SimpleStatus']
 SimpleStatus = enum_type_wrapper.EnumTypeWrapper(_SIMPLESTATUS)
 _STATUSREASON = DESCRIPTOR.enum_types_by_name['StatusReason']
@@ -52,20 +51,14 @@
 SERVICE_GROUP = 3
 RUNTIME_OBJECT = 4
 MANUAL_APPROVAL = 5
 CUSTOM_TASK = 6
 PROTECTION_ATTACHMENT = 7
 PROTECTION_LINK = 8
 DELIVERY_EXTENSION = 9
-UNKNOWN_LIFECYCLE = 0
-CONVERGENCE_START = 1
-PRE_APPROVAL = 2
-POST_APPROVAL = 3
-DEPLOYMENT = 4
-POST_DEPLOYMENT = 5
 CUSTOM_TASK_TYPE_UNKNOWN = 0
 PRE_APPROVAL_TASK = 1
 APPROVAL = 2
 POST_APPROVAL_TASK = 3
 DEPLOYMENT_TASK = 4
 POST_DEPLOYMENT_TASK = 5
 UNKNOWN_STATUS = 0
@@ -118,14 +111,15 @@
 
 _PROTECTIONLINK = DESCRIPTOR.message_types_by_name['ProtectionLink']
 _CONDITION = DESCRIPTOR.message_types_by_name['Condition']
 _CONDITION_RELEASECHANNELSTABLECONDITION = _CONDITION.nested_types_by_name['ReleaseChannelStableCondition']
 _CONDITION_MANUALAPPROVAL = _CONDITION.nested_types_by_name['ManualApproval']
 _CONDITION_CUSTOMTASKSUCCESSFULCONDITION = _CONDITION.nested_types_by_name['CustomTaskSuccessfulCondition']
 _CONDITION_CUSTOMTASKSUCCESSFULCONDITION_PROTECTION = _CONDITION_CUSTOMTASKSUCCESSFULCONDITION.nested_types_by_name['Protection']
+_DELIVERYEXTENSION = DESCRIPTOR.message_types_by_name['DeliveryExtension']
 _IDENTIFIER = DESCRIPTOR.message_types_by_name['Identifier']
 _METADATA = DESCRIPTOR.message_types_by_name['Metadata']
 _STATUSEXPLANATION = DESCRIPTOR.message_types_by_name['StatusExplanation']
 _ACTIONEXPLANATION = DESCRIPTOR.message_types_by_name['ActionExplanation']
 _VERSION = DESCRIPTOR.message_types_by_name['Version']
 _SERVICEINSTANCESTATE = DESCRIPTOR.message_types_by_name['ServiceInstanceState']
 _SERVICESTATE = DESCRIPTOR.message_types_by_name['ServiceState']
@@ -197,14 +191,21 @@
   })
 _sym_db.RegisterMessage(Condition)
 _sym_db.RegisterMessage(Condition.ReleaseChannelStableCondition)
 _sym_db.RegisterMessage(Condition.ManualApproval)
 _sym_db.RegisterMessage(Condition.CustomTaskSuccessfulCondition)
 _sym_db.RegisterMessage(Condition.CustomTaskSuccessfulCondition.Protection)
 
+DeliveryExtension = _reflection.GeneratedProtocolMessageType('DeliveryExtension', (_message.Message,), {
+  'DESCRIPTOR' : _DELIVERYEXTENSION,
+  '__module__' : 'prodvana.desired_state.model.desired_state_pb2'
+  # @@protoc_insertion_point(class_scope:prodvana.desired_state.model.DeliveryExtension)
+  })
+_sym_db.RegisterMessage(DeliveryExtension)
+
 Identifier = _reflection.GeneratedProtocolMessageType('Identifier', (_message.Message,), {
   'DESCRIPTOR' : _IDENTIFIER,
   '__module__' : 'prodvana.desired_state.model.desired_state_pb2'
   # @@protoc_insertion_point(class_scope:prodvana.desired_state.model.Identifier)
   })
 _sym_db.RegisterMessage(Identifier)
 
@@ -419,110 +420,108 @@
   _RUNTIMEOBJECT_OUTPUTBLOBIDSENTRY._serialized_options = b'8\001'
   _CUSTOMTASKSTATE.fields_by_name['name']._options = None
   _CUSTOMTASKSTATE.fields_by_name['name']._serialized_options = b'\372B\004r\002\020\001'
   _CUSTOMTASKSTATE.fields_by_name['description']._options = None
   _CUSTOMTASKSTATE.fields_by_name['description']._serialized_options = b'\372B\004r\002\020\001'
   _CUSTOMTASKSTATE.fields_by_name['program']._options = None
   _CUSTOMTASKSTATE.fields_by_name['program']._serialized_options = b'\372B\005\212\001\002\020\001'
-  _DELIVERYEXTENSIONSTATE.fields_by_name['program']._options = None
-  _DELIVERYEXTENSIONSTATE.fields_by_name['program']._serialized_options = b'\372B\005\212\001\002\020\001'
-  _TYPE._serialized_start=8981
-  _TYPE._serialized_end=9184
-  _LIFECYCLE._serialized_start=9187
-  _LIFECYCLE._serialized_end=9318
-  _CUSTOMTASKTYPE._serialized_start=9321
-  _CUSTOMTASKTYPE._serialized_end=9475
-  _STATUS._serialized_start=9478
-  _STATUS._serialized_end=9718
-  _SIMPLESTATUS._serialized_start=9720
-  _SIMPLESTATUS._serialized_end=9802
-  _STATUSREASON._serialized_start=9805
-  _STATUSREASON._serialized_end=10041
-  _ACTIONTYPE._serialized_start=10043
-  _ACTIONTYPE._serialized_end=10157
-  _CONDITIONSTATUS._serialized_start=10160
-  _CONDITIONSTATUS._serialized_end=10310
-  _MANUALAPPROVALSTATUS._serialized_start=10312
-  _MANUALAPPROVALSTATUS._serialized_end=10375
-  _CUSTOMTASKSTATUS._serialized_start=10378
-  _CUSTOMTASKSTATUS._serialized_end=10511
-  _SIGNALTYPE._serialized_start=10513
-  _SIGNALTYPE._serialized_end=10592
-  _PROTECTIONLINK._serialized_start=331
-  _PROTECTIONLINK._serialized_end=443
-  _CONDITION._serialized_start=446
-  _CONDITION._serialized_end=1233
-  _CONDITION_RELEASECHANNELSTABLECONDITION._serialized_start=753
-  _CONDITION_RELEASECHANNELSTABLECONDITION._serialized_end=920
-  _CONDITION_MANUALAPPROVAL._serialized_start=922
-  _CONDITION_MANUALAPPROVAL._serialized_end=953
-  _CONDITION_CUSTOMTASKSUCCESSFULCONDITION._serialized_start=956
-  _CONDITION_CUSTOMTASKSUCCESSFULCONDITION._serialized_end=1220
-  _CONDITION_CUSTOMTASKSUCCESSFULCONDITION_PROTECTION._serialized_start=1119
-  _CONDITION_CUSTOMTASKSUCCESSFULCONDITION_PROTECTION._serialized_end=1210
-  _IDENTIFIER._serialized_start=1235
-  _IDENTIFIER._serialized_end=1311
-  _METADATA._serialized_start=1314
-  _METADATA._serialized_end=1653
-  _STATUSEXPLANATION._serialized_start=1656
-  _STATUSEXPLANATION._serialized_end=1829
-  _ACTIONEXPLANATION._serialized_start=1832
-  _ACTIONEXPLANATION._serialized_end=1971
-  _VERSION._serialized_start=1974
-  _VERSION._serialized_end=2181
-  _SERVICEINSTANCESTATE._serialized_start=2184
-  _SERVICEINSTANCESTATE._serialized_end=2574
-  _SERVICESTATE._serialized_start=2577
-  _SERVICESTATE._serialized_end=2862
-  _SERVICEGROUPSTATE._serialized_start=2865
-  _SERVICEGROUPSTATE._serialized_end=3075
-  _CANARYPROGRESSSTATE._serialized_start=3078
-  _CANARYPROGRESSSTATE._serialized_end=3374
-  _CANARYPROGRESSSTATE_STATUS._serialized_start=3313
-  _CANARYPROGRESSSTATE_STATUS._serialized_end=3374
-  _DELIVERYSTATE._serialized_start=3377
-  _DELIVERYSTATE._serialized_end=3781
-  _DELIVERYSTATE_STATUS._serialized_start=3620
-  _DELIVERYSTATE_STATUS._serialized_end=3733
-  _RUNTIMEEXTENSIONFETCHOUTPUT._serialized_start=3783
-  _RUNTIMEEXTENSIONFETCHOUTPUT._serialized_end=3869
-  _RUNTIMEOBJECT._serialized_start=3872
-  _RUNTIMEOBJECT._serialized_end=4805
-  _RUNTIMEOBJECT_RUNTIMEEXTENSION._serialized_start=4560
-  _RUNTIMEOBJECT_RUNTIMEEXTENSION._serialized_end=4661
-  _RUNTIMEOBJECT_OUTPUTBLOBIDSENTRY._serialized_start=4663
-  _RUNTIMEOBJECT_OUTPUTBLOBIDSENTRY._serialized_end=4715
-  _RUNTIMEOBJECT_STATUS._serialized_start=4717
-  _RUNTIMEOBJECT_STATUS._serialized_end=4765
-  _CONDITIONSTATE._serialized_start=4807
-  _CONDITIONSTATE._serialized_end=4886
-  _CONTROLSTATE._serialized_start=4889
-  _CONTROLSTATE._serialized_end=5239
-  _MANUALAPPROVALSTATE._serialized_start=5242
-  _MANUALAPPROVALSTATE._serialized_end=5400
-  _STATE._serialized_start=5403
-  _STATE._serialized_end=6108
-  _ANNOTATIONS._serialized_start=6111
-  _ANNOTATIONS._serialized_end=6241
-  _ANNOTATIONS_ANNOTATION._serialized_start=6201
-  _ANNOTATIONS_ANNOTATION._serialized_end=6241
-  _CUSTOMTASKEXECUTIONSTATE._serialized_start=6244
-  _CUSTOMTASKEXECUTIONSTATE._serialized_end=6418
-  _CUSTOMTASKSTATE._serialized_start=6421
-  _CUSTOMTASKSTATE._serialized_end=6883
-  _PROTECTIONLINKSTATE._serialized_start=6886
-  _PROTECTIONLINKSTATE._serialized_end=7505
-  _PROTECTIONLINKSTATE_STOPREASON._serialized_start=7344
-  _PROTECTIONLINKSTATE_STOPREASON._serialized_end=7505
-  _PROTECTIONATTACHMENT._serialized_start=7508
-  _PROTECTIONATTACHMENT._serialized_end=8029
-  _DELIVERYEXTENSIONSTATE._serialized_start=8032
-  _DELIVERYEXTENSIONSTATE._serialized_end=8584
-  _SIGNAL._serialized_start=8587
-  _SIGNAL._serialized_end=8913
-  _SIGNAL_DELIVERYPROMOTIONCONFIG._serialized_start=8829
-  _SIGNAL_DELIVERYPROMOTIONCONFIG._serialized_end=8883
-  _SIGNAL_PROTECTIONBYPASS._serialized_start=8885
-  _SIGNAL_PROTECTIONBYPASS._serialized_end=8903
-  _DEBUGLOG._serialized_start=8915
-  _DEBUGLOG._serialized_end=8978
+  _TYPE._serialized_start=9512
+  _TYPE._serialized_end=9715
+  _CUSTOMTASKTYPE._serialized_start=9718
+  _CUSTOMTASKTYPE._serialized_end=9872
+  _STATUS._serialized_start=9875
+  _STATUS._serialized_end=10115
+  _SIMPLESTATUS._serialized_start=10117
+  _SIMPLESTATUS._serialized_end=10199
+  _STATUSREASON._serialized_start=10202
+  _STATUSREASON._serialized_end=10438
+  _ACTIONTYPE._serialized_start=10440
+  _ACTIONTYPE._serialized_end=10554
+  _CONDITIONSTATUS._serialized_start=10557
+  _CONDITIONSTATUS._serialized_end=10707
+  _MANUALAPPROVALSTATUS._serialized_start=10709
+  _MANUALAPPROVALSTATUS._serialized_end=10772
+  _CUSTOMTASKSTATUS._serialized_start=10775
+  _CUSTOMTASKSTATUS._serialized_end=10908
+  _SIGNALTYPE._serialized_start=10910
+  _SIGNALTYPE._serialized_end=10989
+  _PROTECTIONLINK._serialized_start=366
+  _PROTECTIONLINK._serialized_end=478
+  _CONDITION._serialized_start=481
+  _CONDITION._serialized_end=1268
+  _CONDITION_RELEASECHANNELSTABLECONDITION._serialized_start=788
+  _CONDITION_RELEASECHANNELSTABLECONDITION._serialized_end=955
+  _CONDITION_MANUALAPPROVAL._serialized_start=957
+  _CONDITION_MANUALAPPROVAL._serialized_end=988
+  _CONDITION_CUSTOMTASKSUCCESSFULCONDITION._serialized_start=991
+  _CONDITION_CUSTOMTASKSUCCESSFULCONDITION._serialized_end=1255
+  _CONDITION_CUSTOMTASKSUCCESSFULCONDITION_PROTECTION._serialized_start=1154
+  _CONDITION_CUSTOMTASKSUCCESSFULCONDITION_PROTECTION._serialized_end=1245
+  _DELIVERYEXTENSION._serialized_start=1271
+  _DELIVERYEXTENSION._serialized_end=1431
+  _IDENTIFIER._serialized_start=1433
+  _IDENTIFIER._serialized_end=1509
+  _METADATA._serialized_start=1512
+  _METADATA._serialized_end=1929
+  _STATUSEXPLANATION._serialized_start=1932
+  _STATUSEXPLANATION._serialized_end=2105
+  _ACTIONEXPLANATION._serialized_start=2108
+  _ACTIONEXPLANATION._serialized_end=2247
+  _VERSION._serialized_start=2250
+  _VERSION._serialized_end=2457
+  _SERVICEINSTANCESTATE._serialized_start=2460
+  _SERVICEINSTANCESTATE._serialized_end=2850
+  _SERVICESTATE._serialized_start=2853
+  _SERVICESTATE._serialized_end=3221
+  _SERVICEGROUPSTATE._serialized_start=3224
+  _SERVICEGROUPSTATE._serialized_end=3517
+  _CANARYPROGRESSSTATE._serialized_start=3520
+  _CANARYPROGRESSSTATE._serialized_end=3816
+  _CANARYPROGRESSSTATE_STATUS._serialized_start=3755
+  _CANARYPROGRESSSTATE_STATUS._serialized_end=3816
+  _DELIVERYSTATE._serialized_start=3819
+  _DELIVERYSTATE._serialized_end=4223
+  _DELIVERYSTATE_STATUS._serialized_start=4062
+  _DELIVERYSTATE_STATUS._serialized_end=4175
+  _RUNTIMEEXTENSIONFETCHOUTPUT._serialized_start=4225
+  _RUNTIMEEXTENSIONFETCHOUTPUT._serialized_end=4311
+  _RUNTIMEOBJECT._serialized_start=4314
+  _RUNTIMEOBJECT._serialized_end=5247
+  _RUNTIMEOBJECT_RUNTIMEEXTENSION._serialized_start=5002
+  _RUNTIMEOBJECT_RUNTIMEEXTENSION._serialized_end=5103
+  _RUNTIMEOBJECT_OUTPUTBLOBIDSENTRY._serialized_start=5105
+  _RUNTIMEOBJECT_OUTPUTBLOBIDSENTRY._serialized_end=5157
+  _RUNTIMEOBJECT_STATUS._serialized_start=5159
+  _RUNTIMEOBJECT_STATUS._serialized_end=5207
+  _CONDITIONSTATE._serialized_start=5249
+  _CONDITIONSTATE._serialized_end=5328
+  _CONTROLSTATE._serialized_start=5331
+  _CONTROLSTATE._serialized_end=5681
+  _MANUALAPPROVALSTATE._serialized_start=5684
+  _MANUALAPPROVALSTATE._serialized_end=5842
+  _STATE._serialized_start=5845
+  _STATE._serialized_end=6550
+  _ANNOTATIONS._serialized_start=6553
+  _ANNOTATIONS._serialized_end=6683
+  _ANNOTATIONS_ANNOTATION._serialized_start=6643
+  _ANNOTATIONS_ANNOTATION._serialized_end=6683
+  _CUSTOMTASKEXECUTIONSTATE._serialized_start=6686
+  _CUSTOMTASKEXECUTIONSTATE._serialized_end=6860
+  _CUSTOMTASKSTATE._serialized_start=6863
+  _CUSTOMTASKSTATE._serialized_end=7325
+  _PROTECTIONLINKSTATE._serialized_start=7328
+  _PROTECTIONLINKSTATE._serialized_end=7947
+  _PROTECTIONLINKSTATE_STOPREASON._serialized_start=7786
+  _PROTECTIONLINKSTATE_STOPREASON._serialized_end=7947
+  _PROTECTIONATTACHMENT._serialized_start=7950
+  _PROTECTIONATTACHMENT._serialized_end=8471
+  _DELIVERYEXTENSIONSTATE._serialized_start=8474
+  _DELIVERYEXTENSIONSTATE._serialized_end=9115
+  _SIGNAL._serialized_start=9118
+  _SIGNAL._serialized_end=9444
+  _SIGNAL_DELIVERYPROMOTIONCONFIG._serialized_start=9360
+  _SIGNAL_DELIVERYPROMOTIONCONFIG._serialized_end=9414
+  _SIGNAL_PROTECTIONBYPASS._serialized_start=9416
+  _SIGNAL_PROTECTIONBYPASS._serialized_end=9434
+  _DEBUGLOG._serialized_start=9446
+  _DEBUGLOG._serialized_end=9509
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import google.protobuf.duration_pb2
 import google.protobuf.internal.containers
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
 import google.protobuf.timestamp_pb2
 import prodvana.proto.prodvana.common_config.program_pb2
 import prodvana.proto.prodvana.common_config.retry_pb2
+import prodvana.proto.prodvana.common_config.task_pb2
 import prodvana.proto.prodvana.environment.clusters_pb2
 import prodvana.proto.prodvana.protection.protection_reference_pb2
 import sys
 import typing
 
 if sys.version_info >= (3, 10):
     import typing as typing_extensions
@@ -51,37 +52,14 @@
 MANUAL_APPROVAL: Type.ValueType  # 5
 CUSTOM_TASK: Type.ValueType  # 6
 PROTECTION_ATTACHMENT: Type.ValueType  # 7
 PROTECTION_LINK: Type.ValueType  # 8
 DELIVERY_EXTENSION: Type.ValueType  # 9
 global___Type = Type
 
-class _Lifecycle:
-    ValueType = typing.NewType("ValueType", builtins.int)
-    V: typing_extensions.TypeAlias = ValueType
-
-class _LifecycleEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_Lifecycle.ValueType], builtins.type):  # noqa: F821
-    DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
-    UNKNOWN_LIFECYCLE: _Lifecycle.ValueType  # 0
-    CONVERGENCE_START: _Lifecycle.ValueType  # 1
-    PRE_APPROVAL: _Lifecycle.ValueType  # 2
-    POST_APPROVAL: _Lifecycle.ValueType  # 3
-    DEPLOYMENT: _Lifecycle.ValueType  # 4
-    POST_DEPLOYMENT: _Lifecycle.ValueType  # 5
-
-class Lifecycle(_Lifecycle, metaclass=_LifecycleEnumTypeWrapper): ...
-
-UNKNOWN_LIFECYCLE: Lifecycle.ValueType  # 0
-CONVERGENCE_START: Lifecycle.ValueType  # 1
-PRE_APPROVAL: Lifecycle.ValueType  # 2
-POST_APPROVAL: Lifecycle.ValueType  # 3
-DEPLOYMENT: Lifecycle.ValueType  # 4
-POST_DEPLOYMENT: Lifecycle.ValueType  # 5
-global___Lifecycle = Lifecycle
-
 class _CustomTaskType:
     ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
 
 class _CustomTaskTypeEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_CustomTaskType.ValueType], builtins.type):  # noqa: F821
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     CUSTOM_TASK_TYPE_UNKNOWN: _CustomTaskType.ValueType  # 0
@@ -445,14 +423,35 @@
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["condition", b"condition", "custom_task", b"custom_task", "manual_approval", b"manual_approval", "rc_cond", b"rc_cond"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["condition", b"condition", "custom_task", b"custom_task", "desired_state_id", b"desired_state_id", "manual_approval", b"manual_approval", "rc_cond", b"rc_cond"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["condition", b"condition"]) -> typing_extensions.Literal["rc_cond", "manual_approval", "custom_task"] | None: ...
 
 global___Condition = Condition
 
+class DeliveryExtension(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    INSTANCE_ID_FIELD_NUMBER: builtins.int
+    LIFECYCLE_FIELD_NUMBER: builtins.int
+    REFERENCES_FIELD_NUMBER: builtins.int
+    instance_id: builtins.str
+    lifecycle: prodvana.proto.prodvana.common_config.task_pb2.TaskLifecycle.ValueType
+    @property
+    def references(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Identifier]: ...
+    def __init__(
+        self,
+        *,
+        instance_id: builtins.str = ...,
+        lifecycle: prodvana.proto.prodvana.common_config.task_pb2.TaskLifecycle.ValueType = ...,
+        references: collections.abc.Iterable[global___Identifier] | None = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["instance_id", b"instance_id", "lifecycle", b"lifecycle", "references", b"references"]) -> None: ...
+
+global___DeliveryExtension = DeliveryExtension
+
 class Identifier(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     TYPE_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
     type: global___Type.ValueType
     name: builtins.str
@@ -472,37 +471,41 @@
 
     PRECONDITIONS_FIELD_NUMBER: builtins.int
     INVARIANTS_FIELD_NUMBER: builtins.int
     SELF_FIELD_NUMBER: builtins.int
     DESIRED_STATE_ID_FIELD_NUMBER: builtins.int
     ROOT_DESIRED_STATE_ID_FIELD_NUMBER: builtins.int
     PROTECTION_LINKS_FIELD_NUMBER: builtins.int
+    DELIVERY_EXTENSIONS_FIELD_NUMBER: builtins.int
     @property
     def preconditions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Condition]: ...
     @property
     def invariants(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Condition]: ...
     @property
     def self(self) -> global___Identifier: ...
     desired_state_id: builtins.str
     root_desired_state_id: builtins.str
     @property
     def protection_links(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ProtectionLink]: ...
+    @property
+    def delivery_extensions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___DeliveryExtension]: ...
     def __init__(
         # pyright: reportSelfClsParameterName=false
         self_,
         *,
         preconditions: collections.abc.Iterable[global___Condition] | None = ...,
         invariants: collections.abc.Iterable[global___Condition] | None = ...,
         self: global___Identifier | None = ...,
         desired_state_id: builtins.str = ...,
         root_desired_state_id: builtins.str = ...,
         protection_links: collections.abc.Iterable[global___ProtectionLink] | None = ...,
+        delivery_extensions: collections.abc.Iterable[global___DeliveryExtension] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["self", b"self"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["desired_state_id", b"desired_state_id", "invariants", b"invariants", "preconditions", b"preconditions", "protection_links", b"protection_links", "root_desired_state_id", b"root_desired_state_id", "self", b"self"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["delivery_extensions", b"delivery_extensions", "desired_state_id", b"desired_state_id", "invariants", b"invariants", "preconditions", b"preconditions", "protection_links", b"protection_links", "root_desired_state_id", b"root_desired_state_id", "self", b"self"]) -> None: ...
 
 global___Metadata = Metadata
 
 class StatusExplanation(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     SUBJECT_FIELD_NUMBER: builtins.int
@@ -646,62 +649,70 @@
 
     META_FIELD_NUMBER: builtins.int
     APPLICATION_FIELD_NUMBER: builtins.int
     SERVICE_FIELD_NUMBER: builtins.int
     SERVICE_ID_FIELD_NUMBER: builtins.int
     RELEASE_CHANNELS_FIELD_NUMBER: builtins.int
     CUSTOM_TASKS_FIELD_NUMBER: builtins.int
+    DELIVERY_EXTENSIONS_FIELD_NUMBER: builtins.int
     @property
     def meta(self) -> global___Metadata: ...
     application: builtins.str
     service: builtins.str
     service_id: builtins.str
     """set internally by prodvana"""
     @property
     def release_channels(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ServiceInstanceState]: ...
     @property
     def custom_tasks(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___CustomTaskState]:
         """Definitions for custom tasks used by this service. Must be empty if part of service group."""
+    @property
+    def delivery_extensions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___DeliveryExtensionState]: ...
     def __init__(
         self,
         *,
         meta: global___Metadata | None = ...,
         application: builtins.str = ...,
         service: builtins.str = ...,
         service_id: builtins.str = ...,
         release_channels: collections.abc.Iterable[global___ServiceInstanceState] | None = ...,
         custom_tasks: collections.abc.Iterable[global___CustomTaskState] | None = ...,
+        delivery_extensions: collections.abc.Iterable[global___DeliveryExtensionState] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["meta", b"meta"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["application", b"application", "custom_tasks", b"custom_tasks", "meta", b"meta", "release_channels", b"release_channels", "service", b"service", "service_id", b"service_id"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["application", b"application", "custom_tasks", b"custom_tasks", "delivery_extensions", b"delivery_extensions", "meta", b"meta", "release_channels", b"release_channels", "service", b"service", "service_id", b"service_id"]) -> None: ...
 
 global___ServiceState = ServiceState
 
 class ServiceGroupState(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     META_FIELD_NUMBER: builtins.int
     SERVICES_FIELD_NUMBER: builtins.int
     CUSTOM_TASKS_FIELD_NUMBER: builtins.int
+    DELIVERY_EXTENSIONS_FIELD_NUMBER: builtins.int
     @property
     def meta(self) -> global___Metadata: ...
     @property
     def services(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ServiceState]: ...
     @property
     def custom_tasks(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___CustomTaskState]:
         """Definitions for custom tasks used by this service group."""
+    @property
+    def delivery_extensions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___DeliveryExtensionState]: ...
     def __init__(
         self,
         *,
         meta: global___Metadata | None = ...,
         services: collections.abc.Iterable[global___ServiceState] | None = ...,
         custom_tasks: collections.abc.Iterable[global___CustomTaskState] | None = ...,
+        delivery_extensions: collections.abc.Iterable[global___DeliveryExtensionState] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["meta", b"meta"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["custom_tasks", b"custom_tasks", "meta", b"meta", "services", b"services"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["custom_tasks", b"custom_tasks", "delivery_extensions", b"delivery_extensions", "meta", b"meta", "services", b"services"]) -> None: ...
 
 global___ServiceGroupState = ServiceGroupState
 
 class CanaryProgressState(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class _Status:
@@ -1277,50 +1288,56 @@
 
 class DeliveryExtensionState(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     META_FIELD_NUMBER: builtins.int
     VERSIONS_FIELD_NUMBER: builtins.int
     EXTENSION_ID_FIELD_NUMBER: builtins.int
-    PROGRAM_FIELD_NUMBER: builtins.int
-    RETRY_CONFIG_FIELD_NUMBER: builtins.int
+    EXTENSION_INSTANCE_ID_FIELD_NUMBER: builtins.int
+    LIFECYCLE_FIELD_NUMBER: builtins.int
     LAST_COMPLETED_TIMESTAMP_FIELD_NUMBER: builtins.int
     LAST_COMPLETED_STATUS_FIELD_NUMBER: builtins.int
     LAST_COMPLETED_STATUS_EXPLANATIONS_FIELD_NUMBER: builtins.int
     LAST_COMPLETED_APPLIED_VERSION_FIELD_NUMBER: builtins.int
+    REFERENCES_FIELD_NUMBER: builtins.int
+    STATUS_FIELD_NUMBER: builtins.int
     @property
     def meta(self) -> global___Metadata: ...
     @property
     def versions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Version]: ...
     extension_id: builtins.str
-    @property
-    def program(self) -> prodvana.proto.prodvana.common_config.program_pb2.ProgramConfig: ...
-    @property
-    def retry_config(self) -> prodvana.proto.prodvana.common_config.retry_pb2.RetryConfig: ...
+    extension_instance_id: builtins.str
+    lifecycle: prodvana.proto.prodvana.common_config.task_pb2.TaskLifecycle.ValueType
     @property
     def last_completed_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
     last_completed_status: global___SimpleStatus.ValueType
     @property
     def last_completed_status_explanations(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___StatusExplanation]: ...
     last_completed_applied_version: builtins.str
+    @property
+    def references(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Identifier]: ...
+    status: global___ConditionStatus.ValueType
+    """next tag: 14"""
     def __init__(
         self,
         *,
         meta: global___Metadata | None = ...,
         versions: collections.abc.Iterable[global___Version] | None = ...,
         extension_id: builtins.str = ...,
-        program: prodvana.proto.prodvana.common_config.program_pb2.ProgramConfig | None = ...,
-        retry_config: prodvana.proto.prodvana.common_config.retry_pb2.RetryConfig | None = ...,
+        extension_instance_id: builtins.str = ...,
+        lifecycle: prodvana.proto.prodvana.common_config.task_pb2.TaskLifecycle.ValueType = ...,
         last_completed_timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         last_completed_status: global___SimpleStatus.ValueType = ...,
         last_completed_status_explanations: collections.abc.Iterable[global___StatusExplanation] | None = ...,
         last_completed_applied_version: builtins.str = ...,
+        references: collections.abc.Iterable[global___Identifier] | None = ...,
+        status: global___ConditionStatus.ValueType = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["last_completed_timestamp", b"last_completed_timestamp", "meta", b"meta", "program", b"program", "retry_config", b"retry_config"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["extension_id", b"extension_id", "last_completed_applied_version", b"last_completed_applied_version", "last_completed_status", b"last_completed_status", "last_completed_status_explanations", b"last_completed_status_explanations", "last_completed_timestamp", b"last_completed_timestamp", "meta", b"meta", "program", b"program", "retry_config", b"retry_config", "versions", b"versions"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["last_completed_timestamp", b"last_completed_timestamp", "meta", b"meta"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["extension_id", b"extension_id", "extension_instance_id", b"extension_instance_id", "last_completed_applied_version", b"last_completed_applied_version", "last_completed_status", b"last_completed_status", "last_completed_status_explanations", b"last_completed_status_explanations", "last_completed_timestamp", b"last_completed_timestamp", "lifecycle", b"lifecycle", "meta", b"meta", "references", b"references", "status", b"status", "versions", b"versions"]) -> None: ...
 
 global___DeliveryExtensionState = DeliveryExtensionState
 
 class Signal(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class DeliveryPromotionConfig(google.protobuf.message.Message):
```

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/desired_state/model/entity_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/desired_state/model/entity_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,19 +8,20 @@
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from prodvana.proto.prodvana.common_config import task_pb2 as prodvana_dot_common__config_dot_task__pb2
 from prodvana.proto.prodvana.desired_state.model import desired_state_pb2 as prodvana_dot_desired__state_dot_model_dot_desired__state__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)prodvana/desired_state/model/entity.proto\x12\x1cprodvana.desired_state.model\x1a\x30prodvana/desired_state/model/desired_state.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xb4\x08\n\x06\x45ntity\x12\x34\n\x02id\x18\x01 \x01(\x0b\x32(.prodvana.desired_state.model.Identifier\x12\x18\n\x10\x64\x65sired_state_id\x18\x02 \x01(\t\x12\x1d\n\x15root_desired_state_id\x18\x03 \x01(\t\x12>\n\x0b\x61nnotations\x18\x04 \x01(\x0b\x32).prodvana.desired_state.model.Annotations\x12\x34\n\x06status\x18\x05 \x01(\x0e\x32$.prodvana.desired_state.model.Status\x12\x41\n\rsimple_status\x18\x11 \x01(\x0e\x32*.prodvana.desired_state.model.SimpleStatus\x12;\n\x0estarting_state\x18\x06 \x01(\x0b\x32#.prodvana.desired_state.model.State\x12<\n\x0flast_seen_state\x18\x07 \x01(\x0b\x32#.prodvana.desired_state.model.State\x12:\n\rdesired_state\x18\x08 \x01(\x0b\x32#.prodvana.desired_state.model.State\x12K\n\x15precondition_statuses\x18\t \x03(\x0b\x32,.prodvana.desired_state.model.ConditionState\x12L\n\x13status_explanations\x18\n \x03(\x0b\x32/.prodvana.desired_state.model.StatusExplanation\x12\x34\n\x04logs\x18\x0b \x03(\x0b\x32&.prodvana.desired_state.model.DebugLog\x12K\n\x12\x61\x63tion_explanation\x18\x0c \x01(\x0b\x32/.prodvana.desired_state.model.ActionExplanation\x12\x39\n\x15last_update_timestamp\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x16last_fetched_timestamp\x18\x0e \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x16last_applied_timestamp\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12>\n\x0c\x64\x65pendencies\x18\x10 \x03(\x0b\x32(.prodvana.desired_state.model.Identifier\x12:\n\tlifecycle\x18\x12 \x01(\x0e\x32\'.prodvana.desired_state.model.Lifecycle\"}\n\x0b\x45ntityGraph\x12\x36\n\x04root\x18\x01 \x01(\x0b\x32(.prodvana.desired_state.model.Identifier\x12\x36\n\x08\x65ntities\x18\x02 \x03(\x0b\x32$.prodvana.desired_state.model.EntityBXZVgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/desired_state/modelb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)prodvana/desired_state/model/entity.proto\x12\x1cprodvana.desired_state.model\x1a!prodvana/common_config/task.proto\x1a\x30prodvana/desired_state/model/desired_state.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xb2\x08\n\x06\x45ntity\x12\x34\n\x02id\x18\x01 \x01(\x0b\x32(.prodvana.desired_state.model.Identifier\x12\x18\n\x10\x64\x65sired_state_id\x18\x02 \x01(\t\x12\x1d\n\x15root_desired_state_id\x18\x03 \x01(\t\x12>\n\x0b\x61nnotations\x18\x04 \x01(\x0b\x32).prodvana.desired_state.model.Annotations\x12\x34\n\x06status\x18\x05 \x01(\x0e\x32$.prodvana.desired_state.model.Status\x12\x41\n\rsimple_status\x18\x11 \x01(\x0e\x32*.prodvana.desired_state.model.SimpleStatus\x12;\n\x0estarting_state\x18\x06 \x01(\x0b\x32#.prodvana.desired_state.model.State\x12<\n\x0flast_seen_state\x18\x07 \x01(\x0b\x32#.prodvana.desired_state.model.State\x12:\n\rdesired_state\x18\x08 \x01(\x0b\x32#.prodvana.desired_state.model.State\x12K\n\x15precondition_statuses\x18\t \x03(\x0b\x32,.prodvana.desired_state.model.ConditionState\x12L\n\x13status_explanations\x18\n \x03(\x0b\x32/.prodvana.desired_state.model.StatusExplanation\x12\x34\n\x04logs\x18\x0b \x03(\x0b\x32&.prodvana.desired_state.model.DebugLog\x12K\n\x12\x61\x63tion_explanation\x18\x0c \x01(\x0b\x32/.prodvana.desired_state.model.ActionExplanation\x12\x39\n\x15last_update_timestamp\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x16last_fetched_timestamp\x18\x0e \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12:\n\x16last_applied_timestamp\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12>\n\x0c\x64\x65pendencies\x18\x10 \x03(\x0b\x32(.prodvana.desired_state.model.Identifier\x12\x38\n\tlifecycle\x18\x12 \x01(\x0e\x32%.prodvana.common_config.TaskLifecycle\"}\n\x0b\x45ntityGraph\x12\x36\n\x04root\x18\x01 \x01(\x0b\x32(.prodvana.desired_state.model.Identifier\x12\x36\n\x08\x65ntities\x18\x02 \x03(\x0b\x32$.prodvana.desired_state.model.EntityBXZVgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/desired_state/modelb\x06proto3')
 
 
 
 _ENTITY = DESCRIPTOR.message_types_by_name['Entity']
 _ENTITYGRAPH = DESCRIPTOR.message_types_by_name['EntityGraph']
 Entity = _reflection.GeneratedProtocolMessageType('Entity', (_message.Message,), {
   'DESCRIPTOR' : _ENTITY,
@@ -36,12 +37,12 @@
   })
 _sym_db.RegisterMessage(EntityGraph)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'ZVgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/desired_state/model'
-  _ENTITY._serialized_start=159
-  _ENTITY._serialized_end=1235
-  _ENTITYGRAPH._serialized_start=1237
-  _ENTITYGRAPH._serialized_end=1362
+  _ENTITY._serialized_start=194
+  _ENTITY._serialized_end=1268
+  _ENTITYGRAPH._serialized_start=1270
+  _ENTITYGRAPH._serialized_end=1395
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/desired_state/model/entity_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/desired_state/model/entity_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 """
 import builtins
 import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import google.protobuf.timestamp_pb2
+import prodvana.proto.prodvana.common_config.task_pb2
 import prodvana.proto.prodvana.desired_state.model.desired_state_pb2
 import sys
 
 if sys.version_info >= (3, 8):
     import typing as typing_extensions
 else:
     import typing_extensions
@@ -68,15 +69,15 @@
     def last_fetched_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp:
         """when prodvana last fetched entity state, best effort"""
     @property
     def last_applied_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp:
         """when prodvana last applied state for this entity, best effort"""
     @property
     def dependencies(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.desired_state.model.desired_state_pb2.Identifier]: ...
-    lifecycle: prodvana.proto.prodvana.desired_state.model.desired_state_pb2.Lifecycle.ValueType
+    lifecycle: prodvana.proto.prodvana.common_config.task_pb2.TaskLifecycle.ValueType
     """next tag: 19"""
     def __init__(
         self,
         *,
         id: prodvana.proto.prodvana.desired_state.model.desired_state_pb2.Identifier | None = ...,
         desired_state_id: builtins.str = ...,
         root_desired_state_id: builtins.str = ...,
@@ -90,15 +91,15 @@
         status_explanations: collections.abc.Iterable[prodvana.proto.prodvana.desired_state.model.desired_state_pb2.StatusExplanation] | None = ...,
         logs: collections.abc.Iterable[prodvana.proto.prodvana.desired_state.model.desired_state_pb2.DebugLog] | None = ...,
         action_explanation: prodvana.proto.prodvana.desired_state.model.desired_state_pb2.ActionExplanation | None = ...,
         last_update_timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         last_fetched_timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         last_applied_timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         dependencies: collections.abc.Iterable[prodvana.proto.prodvana.desired_state.model.desired_state_pb2.Identifier] | None = ...,
-        lifecycle: prodvana.proto.prodvana.desired_state.model.desired_state_pb2.Lifecycle.ValueType = ...,
+        lifecycle: prodvana.proto.prodvana.common_config.task_pb2.TaskLifecycle.ValueType = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["action_explanation", b"action_explanation", "annotations", b"annotations", "desired_state", b"desired_state", "id", b"id", "last_applied_timestamp", b"last_applied_timestamp", "last_fetched_timestamp", b"last_fetched_timestamp", "last_seen_state", b"last_seen_state", "last_update_timestamp", b"last_update_timestamp", "starting_state", b"starting_state"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["action_explanation", b"action_explanation", "annotations", b"annotations", "dependencies", b"dependencies", "desired_state", b"desired_state", "desired_state_id", b"desired_state_id", "id", b"id", "last_applied_timestamp", b"last_applied_timestamp", "last_fetched_timestamp", b"last_fetched_timestamp", "last_seen_state", b"last_seen_state", "last_update_timestamp", b"last_update_timestamp", "lifecycle", b"lifecycle", "logs", b"logs", "precondition_statuses", b"precondition_statuses", "root_desired_state_id", b"root_desired_state_id", "simple_status", b"simple_status", "starting_state", b"starting_state", "status", b"status", "status_explanations", b"status_explanations"]) -> None: ...
 
 global___Entity = Entity
 
 class EntityGraph(google.protobuf.message.Message):
```

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/environment/clusters_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/environment/clusters_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/environment/clusters_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/environment/clusters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/environment/environment_manager_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/environment/environment_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/environment/environment_manager_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/environment/environment_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.py` & `prodvana-0.1.7/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/events/events_manager_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/events/events_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/events/events_manager_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/events/events_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/events/events_manager_pb2_grpc.py` & `prodvana-0.1.7/prodvana/proto/prodvana/events/events_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/events/events_manager_pb2_grpc.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/events/events_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/events/events_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/events/events_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/events/events_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/events/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/events/types_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/events/types_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/events/types_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/events/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/insights/insights_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/insights/insights_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/insights/insights_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/insights/insights_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/managed_resource/manager_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/managed_resource/manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/managed_resource/manager_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/managed_resource/manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.py` & `prodvana-0.1.7/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/metrics/metrics_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/metrics/metrics_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/metrics/metrics_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/metrics/metrics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/object/meta_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/version/source_metadata_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,46 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: prodvana/object/meta.proto
+# source: prodvana/version/source_metadata.proto
 """Generated protocol buffer code."""
+from google.protobuf.internal import enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from prodvana.proto.prodvana.version import source_metadata_pb2 as prodvana_dot_version_dot_source__metadata__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1aprodvana/object/meta.proto\x12\x0fprodvana.object\x1a&prodvana/version/source_metadata.proto\"\xb4\x01\n\nObjectMeta\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x16\n\x0e\x63onfig_version\x18\x04 \x01(\t\x12(\n\x06source\x18\x05 \x01(\x0e\x32\x18.prodvana.version.Source\x12\x39\n\x0fsource_metadata\x18\x06 \x01(\x0b\x32 .prodvana.version.SourceMetadataBKZIgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/objectb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&prodvana/version/source_metadata.proto\x12\x10prodvana.version\"V\n\x0eSourceMetadata\x12\x10\n\x08repo_url\x18\x01 \x01(\t\x12\x11\n\tfile_path\x18\x02 \x01(\t\x12\x0e\n\x06\x63ommit\x18\x03 \x01(\t\x12\x0f\n\x07user_id\x18\x04 \x01(\t*m\n\x06Source\x12\x12\n\x0eUNKNOWN_SOURCE\x10\x00\x12\x07\n\x03WEB\x10\x01\x12\x16\n\x12INTERACTIVE_PVNCTL\x10\x02\x12\x0f\n\x0b\x43ONFIG_FILE\x10\x03\x12\x0f\n\x0bREPO_FOLLOW\x10\x04\x12\x0c\n\x08PRODVANA\x10\x05\x42LZJgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/versionb\x06proto3')
 
-
-
-_OBJECTMETA = DESCRIPTOR.message_types_by_name['ObjectMeta']
-ObjectMeta = _reflection.GeneratedProtocolMessageType('ObjectMeta', (_message.Message,), {
-  'DESCRIPTOR' : _OBJECTMETA,
-  '__module__' : 'prodvana.object.meta_pb2'
-  # @@protoc_insertion_point(class_scope:prodvana.object.ObjectMeta)
+_SOURCE = DESCRIPTOR.enum_types_by_name['Source']
+Source = enum_type_wrapper.EnumTypeWrapper(_SOURCE)
+UNKNOWN_SOURCE = 0
+WEB = 1
+INTERACTIVE_PVNCTL = 2
+CONFIG_FILE = 3
+REPO_FOLLOW = 4
+PRODVANA = 5
+
+
+_SOURCEMETADATA = DESCRIPTOR.message_types_by_name['SourceMetadata']
+SourceMetadata = _reflection.GeneratedProtocolMessageType('SourceMetadata', (_message.Message,), {
+  'DESCRIPTOR' : _SOURCEMETADATA,
+  '__module__' : 'prodvana.version.source_metadata_pb2'
+  # @@protoc_insertion_point(class_scope:prodvana.version.SourceMetadata)
   })
-_sym_db.RegisterMessage(ObjectMeta)
+_sym_db.RegisterMessage(SourceMetadata)
 
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'ZIgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/object'
-  _OBJECTMETA._serialized_start=88
-  _OBJECTMETA._serialized_end=268
+  DESCRIPTOR._serialized_options = b'ZJgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/version'
+  _SOURCE._serialized_start=148
+  _SOURCE._serialized_end=257
+  _SOURCEMETADATA._serialized_start=60
+  _SOURCEMETADATA._serialized_end=146
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/object/meta_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/object/meta_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/organization/organization_manager_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/organization/organization_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/organization/organization_manager_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/organization/organization_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.py` & `prodvana-0.1.7/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/organization/user_metadata_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/organization/user_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/organization/user_metadata_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/organization/user_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/pipelines/object_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/pipelines/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/pipelines/object_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/pipelines/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/pipelines/pipelines_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/pipelines/pipelines_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/pipelines/pipelines_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/pipelines/pipelines_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/protection/attachments_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/protection/attachments_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/protection/attachments_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/protection/attachments_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/protection/object_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/protection/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/protection/object_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/protection/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/protection/protection_config_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/protection/protection_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/protection/protection_config_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/protection/protection_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/protection/protection_manager_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/protection/protection_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/protection/protection_manager_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/protection/protection_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.py` & `prodvana-0.1.7/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/protection/protection_reference_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/protection/protection_reference_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/protection/protection_reference_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/protection/protection_reference_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/release_channel/object_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/release_channel/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/release_channel/object_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/release_channel/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.py` & `prodvana-0.1.7/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/repo/repo_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/repo/repo_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/repo/repo_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/repo/repo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/runtimes/features_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/runtimes/features_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/runtimes/features_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/runtimes/features_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/scm/types_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/scm/types_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/scm/types_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/scm/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/secrets/secrets_manager_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/secrets/secrets_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/secrets/secrets_manager_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/secrets/secrets_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.py` & `prodvana-0.1.7/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/service/object_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/service/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/service/object_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/service/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/service/parameters_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/service/parameters_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/service/parameters_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/service/parameters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/service/service_config_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/service/service_config_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,25 +18,27 @@
 from prodvana.proto.prodvana.common_config import kubernetes_config_pb2 as prodvana_dot_common__config_dot_kubernetes__config__pb2
 from prodvana.proto.prodvana.common_config import helm_pb2 as prodvana_dot_common__config_dot_helm__pb2
 from prodvana.proto.prodvana.common_config import maturity_pb2 as prodvana_dot_common__config_dot_maturity__pb2
 from prodvana.proto.prodvana.common_config import parameters_pb2 as prodvana_dot_common__config_dot_parameters__pb2
 from prodvana.proto.prodvana.common_config import program_pb2 as prodvana_dot_common__config_dot_program__pb2
 from prodvana.proto.prodvana.common_config import ref_pb2 as prodvana_dot_common__config_dot_ref__pb2
 from prodvana.proto.prodvana.common_config import retry_pb2 as prodvana_dot_common__config_dot_retry__pb2
+from prodvana.proto.prodvana.common_config import task_pb2 as prodvana_dot_common__config_dot_task__pb2
 from prodvana.proto.prodvana.delivery import delivery_config_pb2 as prodvana_dot_delivery_dot_delivery__config__pb2
+from prodvana.proto.prodvana.delivery_extension import config_pb2 as prodvana_dot_delivery__extension_dot_config__pb2
 from prodvana.proto.prodvana.protection import protection_reference_pb2 as prodvana_dot_protection_dot_protection__reference__pb2
 from prodvana.proto.prodvana.release_channel import release_channel_config_pb2 as prodvana_dot_release__channel_dot_release__channel__config__pb2
 from prodvana.proto.prodvana.runtimes import runtimes_config_pb2 as prodvana_dot_runtimes_dot_runtimes__config__pb2
 from prodvana.proto.prodvana.workflow import integration_config_pb2 as prodvana_dot_workflow_dot_integration__config__pb2
 from prodvana.proto.prodvana.service import parameters_pb2 as prodvana_dot_service_dot_parameters__pb2
 from prodvana.proto.prodvana.volumes import volumes_pb2 as prodvana_dot_volumes_dot_volumes__pb2
 from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%prodvana/service/service_config.proto\x12\x10prodvana.service\x1a\x1egoogle/protobuf/duration.proto\x1a$prodvana/capability/capability.proto\x1a prodvana/common_config/env.proto\x1a.prodvana/common_config/kubernetes_config.proto\x1a!prodvana/common_config/helm.proto\x1a%prodvana/common_config/maturity.proto\x1a\'prodvana/common_config/parameters.proto\x1a$prodvana/common_config/program.proto\x1a prodvana/common_config/ref.proto\x1a\"prodvana/common_config/retry.proto\x1a\'prodvana/delivery/delivery_config.proto\x1a.prodvana/protection/protection_reference.proto\x1a\x35prodvana/release_channel/release_channel_config.proto\x1a\'prodvana/runtimes/runtimes_config.proto\x1a*prodvana/workflow/integration_config.proto\x1a!prodvana/service/parameters.proto\x1a\x1eprodvana/volumes/volumes.proto\x1a\x17validate/validate.proto\"1\n\x0eReplicasConfig\x12\x0f\n\x05\x66ixed\x18\x01 \x01(\x05H\x00\x42\x0e\n\x0c\x63onfig_oneof\"\xaa\x02\n\x0eMetricAnalysis\x12J\n\x0csuccess_rate\x18\x02 \x01(\x0b\x32\x32.prodvana.service.MetricAnalysis.SuccessRateConfigH\x00\x12\x45\n\x0blatency_p95\x18\x03 \x01(\x0b\x32..prodvana.service.MetricAnalysis.LatencyConfigH\x00\x1a\x32\n\x11SuccessRateConfig\x12\x1d\n\x15min_threshold_percent\x18\x01 \x01(\x01\x1a?\n\rLatencyConfig\x12.\n\x0bmax_latency\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationB\x10\n\x0e\x61nalysis_oneof\"\xb7\x02\n\x15ReleaseStrategyConfig\x12<\n\x19individual_stage_deadline\x18\x01 \x01(\x0b\x32\x19.google.protobuf.Duration\x12=\n\x1a\x61utomated_testing_duration\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\x12:\n\x10metrics_analysis\x18\x03 \x03(\x0b\x32 .prodvana.service.MetricAnalysis\x12\x17\n\x0fmanual_approval\x18\x04 \x01(\x08\x12\x31\n\x0e\x63heck_interval\x18\x05 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x19\n\x11\x66\x61ilure_threshold\x18\x06 \x01(\x05\"f\n\tTLSSecret\x12\x14\n\nraw_secret\x18\x03 \x01(\tH\x00\x12\x30\n\x06secret\x18\x04 \x01(\x0b\x32\x1e.prodvana.common_config.SecretH\x00\x42\x11\n\ntls_secret\x12\x03\xf8\x42\x01\"\x81\x01\n\x0eTLSCertificate\x12\x37\n\x08tls_cert\x18\x01 \x01(\x0b\x32\x1b.prodvana.service.TLSSecretB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x36\n\x07tls_key\x18\x02 \x01(\x0b\x32\x1b.prodvana.service.TLSSecretB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\"j\n\x0b\x43\x65rtificate\x12/\n\x03tls\x18\x01 \x01(\x0b\x32 .prodvana.service.TLSCertificateH\x00\x12\x16\n\x0c\x61ws_acm_cert\x18\x02 \x01(\tH\x00\x42\x12\n\x0b\x63\x65rtificate\x12\x03\xf8\x42\x01\"\xed\x06\n\x17PerReleaseChannelConfig\x12 \n\x0frelease_channel\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12&\n\x10\x63ustom_hostnames\x18\x02 \x03(\tB\x0c\xfa\x42\t\x92\x01\x06\"\x04r\x02h\x01\x12W\n\x08programs\x18\x05 \x03(\x0b\x32\x36.prodvana.common_config.PerReleaseChannelProgramConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12+\n\x04\x63\x65rt\x18\x06 \x01(\x0b\x32\x1d.prodvana.service.Certificate\x12:\n\x0f\x64\x65livery_config\x18\x07 \x01(\x0b\x32!.prodvana.delivery.DeliveryConfig\x12\x38\n\x07volumes\x18\x08 \x03(\x0b\x32\x18.prodvana.volumes.VolumeB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x32\n\x08replicas\x18\t \x01(\x0b\x32 .prodvana.service.ReplicasConfig\x12\x43\n\x0epre_push_tasks\x18\n \x03(\x0b\x32\x1c.prodvana.service.TaskConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x41\n\x10runtime_specific\x18\x0b \x01(\x0b\x32\'.prodvana.service.RuntimeSpecificConfig\x12\x1a\n\x12runtime_connection\x18\x11 \x01(\t\x12\x45\n\x11runtime_extension\x18\r \x01(\x0b\x32(.prodvana.service.RuntimeExtensionConfigH\x00\x12\x45\n\x11kubernetes_config\x18\x0e \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x43\n\x0f\x65xternal_config\x18\x10 \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x32\n\x04helm\x18\x0f \x01(\x0b\x32\".prodvana.common_config.HelmConfigH\x00\x42\x0e\n\x0c\x63onfig_oneofJ\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x0c\x10\rR\x0bprotections\",\n\x13\x43\x61pabilityReference\x12\x15\n\x04name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"U\n\x18\x43ompiledCapabilityConfig\x12\x39\n\ncapability\x18\x01 \x01(\x0b\x32%.prodvana.capability.CapabilityConfig\".\n\x10ProgramReference\x12\x0e\n\x04name\x18\x01 \x01(\tH\x00\x42\n\n\x03ref\x12\x03\xf8\x42\x01\"6\n\rTaskReference\x12\x19\n\x0frelease_channel\x18\x01 \x01(\tH\x00\x42\n\n\x03ref\x12\x03\xf8\x42\x01\"\xf1\x01\n\nTaskConfig\x12@\n\x07program\x18\x01 \x01(\x0b\x32%.prodvana.common_config.ProgramConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x38\n\x0c\x62\x61se_program\x18\x02 \x01(\x0b\x32\".prodvana.service.ProgramReference\x12\x39\n\x0cretry_config\x18\x03 \x01(\x0b\x32#.prodvana.common_config.RetryConfig\x12,\n\x03ref\x18\x04 \x01(\x0b\x32\x1f.prodvana.service.TaskReference\"\x9c\x02\n\x15RuntimeSpecificConfig\x12@\n\x03k8s\x18\x01 \x01(\x0b\x32\x31.prodvana.service.RuntimeSpecificConfig.K8SConfigH\x00\x1a\xae\x01\n\tK8SConfig\x12\x66\n\x13service_annotations\x18\x01 \x03(\x0b\x32I.prodvana.service.RuntimeSpecificConfig.K8SConfig.ServiceAnnotationsEntry\x1a\x39\n\x17ServiceAnnotationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\x10\n\x0eruntime_config\"Z\n\x16RuntimeExtensionConfig\x12@\n\x10parameter_values\x18\x01 \x03(\x0b\x32&.prodvana.common_config.ParameterValue\"&\n\x12\x41utoRollbackConfig\x12\x10\n\x08\x64isabled\x18\x01 \x01(\x08\"\xec\x01\n\x1fProtectionConvergenceAttachment\x12:\n\x04name\x18\x01 \x01(\tB,\xfa\x42)r\'\x10\x00\x18?2!^[a-z]?([a-z0-9-]*[a-z0-9]){0,1}$\x12?\n\x03ref\x18\x02 \x01(\x0b\x32(.prodvana.protection.ProtectionReferenceB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12L\n\tlifecycle\x18\x03 \x03(\x0b\x32(.prodvana.protection.ProtectionLifecycleB\x0f\xfa\x42\x0c\x92\x01\t\x08\x01\"\x05\x8a\x01\x02\x10\x01\"\xe5\x0c\n\rServiceConfig\x12\x39\n\x04name\x18\x01 \x01(\tB+\xfa\x42(r&\x10\x01\x18?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$\x12\x13\n\x0b\x61pplication\x18\x14 \x01(\t\x12\x46\n\x08programs\x18\x02 \x03(\x0b\x32%.prodvana.common_config.ProgramConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x32\n\x08replicas\x18\x04 \x01(\x0b\x32 .prodvana.service.ReplicasConfig\x12\x41\n\x10release_strategy\x18\x05 \x01(\x0b\x32\'.prodvana.service.ReleaseStrategyConfig\x12U\n\x13per_release_channel\x18\t \x03(\x0b\x32).prodvana.service.PerReleaseChannelConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12J\n\x0c\x63\x61pabilities\x18\n \x03(\x0b\x32%.prodvana.service.CapabilityReferenceB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12:\n\x0f\x64\x65livery_config\x18\x0b \x01(\x0b\x32!.prodvana.delivery.DeliveryConfig\x12\x38\n\x07volumes\x18\x0c \x03(\x0b\x32\x18.prodvana.volumes.VolumeB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12@\n\x12\x64\x65ploy_annotations\x18\r \x01(\x0b\x32$.prodvana.workflow.AnnotationsConfig\x12\x41\n\rbase_template\x18\x0e \x01(\x0b\x32*.prodvana.common_config.ServiceTemplateRef\x12\x34\n\x0epre_push_tasks\x18\x0f \x03(\x0b\x32\x1c.prodvana.service.TaskConfig\x12\x41\n\x10runtime_specific\x18\x10 \x01(\x0b\x32\'.prodvana.service.RuntimeSpecificConfig\x12\x1a\n\x12runtime_connection\x18\x1c \x01(\t\x12N\n\nparameters\x18\x15 \x03(\x0b\x32+.prodvana.common_config.ParameterDefinitionB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x42\n\x10parameter_values\x18\x16 \x01(\x0b\x32(.prodvana.service.ServiceParameterValues\x12\x34\n\x11progress_deadline\x18\x18 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x45\n\x11runtime_extension\x18\x12 \x01(\x0b\x32(.prodvana.service.RuntimeExtensionConfigH\x00\x12\x45\n\x11kubernetes_config\x18\x13 \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x43\n\x0f\x65xternal_config\x18\x1b \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x32\n\x04helm\x18\x1a \x01(\x0b\x32\".prodvana.common_config.HelmConfigH\x00\x12M\n\x12parameters_autogen\x18\x17 \x01(\x0e\x32\x31.prodvana.service.ServiceConfig.ParametersAutogen\x12;\n\rauto_rollback\x18\x19 \x01(\x0b\x32$.prodvana.service.AutoRollbackConfig\"M\n\x11ParametersAutogen\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04NONE\x10\x01\x12\t\n\x05IMAGE\x10\x02\x12\x16\n\x12IMAGE_AND_REPLICAS\x10\x03\x42\x0e\n\x0c\x63onfig_oneofJ\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08J\x04\x08\x08\x10\tJ\x04\x08\x11\x10\x12R\x08\x65xternalR\x10image_repositoryR\x15\x63ontainer_registry_idR\x0bprotections\"\xc9\x0c\n\x1d\x43ompiledServiceInstanceConfig\x12\x0f\n\x07service\x18\x01 \x01(\t\x12\x13\n\x0b\x61pplication\x18\x12 \x01(\t\x12\x17\n\x0frelease_channel\x18\x02 \x01(\t\x12\x37\n\x08programs\x18\x03 \x03(\x0b\x32%.prodvana.common_config.ProgramConfig\x12\x32\n\x08replicas\x18\x04 \x01(\x0b\x32 .prodvana.service.ReplicasConfig\x12\x32\n\x08maturity\x18\x05 \x01(\x0e\x32 .prodvana.common_config.Maturity\x12\x41\n\x10release_strategy\x18\x06 \x01(\x0b\x32\'.prodvana.service.ReleaseStrategyConfig\x12\x18\n\x10\x63ustom_hostnames\x18\x07 \x03(\t\x12+\n\x04\x63\x65rt\x18\n \x01(\x0b\x32\x1d.prodvana.service.Certificate\x12\x46\n\x07runtime\x18\x0b \x01(\x0b\x32\x35.prodvana.release_channel.ReleaseChannelRuntimeConfig\x12\x44\n\x11runtime_execution\x18\x1b \x01(\x0b\x32).prodvana.runtimes.RuntimeExecutionConfig\x12@\n\x0c\x63\x61pabilities\x18\x0c \x03(\x0b\x32*.prodvana.service.CompiledCapabilityConfig\x12:\n\x0f\x64\x65livery_config\x18\r \x01(\x0b\x32!.prodvana.delivery.DeliveryConfig\x12\x38\n\x07volumes\x18\x0e \x03(\x0b\x32\x18.prodvana.volumes.VolumeB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12@\n\x12\x64\x65ploy_annotations\x18\x0f \x01(\x0b\x32$.prodvana.workflow.AnnotationsConfig\x12\x41\n\rbase_template\x18\x10 \x01(\x0b\x32*.prodvana.common_config.ServiceTemplateRef\x12\x34\n\x0epre_push_tasks\x18\x11 \x03(\x0b\x32\x1c.prodvana.service.TaskConfig\x12\x41\n\x10runtime_specific\x18\x13 \x01(\x0b\x32\'.prodvana.service.RuntimeSpecificConfig\x12?\n\nparameters\x18\x18 \x03(\x0b\x32+.prodvana.common_config.ParameterDefinition\x12@\n\x10parameter_values\x18\x19 \x03(\x0b\x32&.prodvana.common_config.ParameterValue\x12\x34\n\x11progress_deadline\x18\x1a \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x45\n\x11runtime_extension\x18\x16 \x01(\x0b\x32(.prodvana.service.RuntimeExtensionConfigH\x00\x12\x45\n\x11kubernetes_config\x18\x17 \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x32\n\x04helm\x18\x1d \x01(\x0b\x32\".prodvana.common_config.HelmConfigH\x00\x12n\n\x03\x65nv\x18\x1c \x03(\x0b\x32\x38.prodvana.service.CompiledServiceInstanceConfig.EnvEntryB\'\xfa\x42$\x9a\x01!\x18\x01\"\x1dr\x1b\x32\x19^[a-zA-Z_]+[a-zA-Z0-9_]*$\x1aL\n\x08\x45nvEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .prodvana.common_config.EnvValue:\x02\x38\x01\x42\x0e\n\x0c\x63onfig_oneofJ\x04\x08\x08\x10\tJ\x04\x08\t\x10\nJ\x04\x08\x14\x10\x15J\x04\x08\x15\x10\x16R\x0bprotectionsR\x0cruntime_type\"\x88\x02\n\x11\x43ompiledJobConfig\x12\x13\n\x0bname_prefix\x18\x01 \x01(\t\x12\x17\n\x0frelease_channel\x18\x02 \x01(\t\x12\x37\n\x08programs\x18\x03 \x03(\x0b\x32%.prodvana.common_config.ProgramConfig\x12\x46\n\x07runtime\x18\x04 \x01(\x0b\x32\x35.prodvana.release_channel.ReleaseChannelRuntimeConfig\x12\x44\n\x11runtime_execution\x18\x05 \x01(\x0b\x32).prodvana.runtimes.RuntimeExecutionConfigBLZJgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/serviceb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%prodvana/service/service_config.proto\x12\x10prodvana.service\x1a\x1egoogle/protobuf/duration.proto\x1a$prodvana/capability/capability.proto\x1a prodvana/common_config/env.proto\x1a.prodvana/common_config/kubernetes_config.proto\x1a!prodvana/common_config/helm.proto\x1a%prodvana/common_config/maturity.proto\x1a\'prodvana/common_config/parameters.proto\x1a$prodvana/common_config/program.proto\x1a prodvana/common_config/ref.proto\x1a\"prodvana/common_config/retry.proto\x1a!prodvana/common_config/task.proto\x1a\'prodvana/delivery/delivery_config.proto\x1a(prodvana/delivery_extension/config.proto\x1a.prodvana/protection/protection_reference.proto\x1a\x35prodvana/release_channel/release_channel_config.proto\x1a\'prodvana/runtimes/runtimes_config.proto\x1a*prodvana/workflow/integration_config.proto\x1a!prodvana/service/parameters.proto\x1a\x1eprodvana/volumes/volumes.proto\x1a\x17validate/validate.proto\"1\n\x0eReplicasConfig\x12\x0f\n\x05\x66ixed\x18\x01 \x01(\x05H\x00\x42\x0e\n\x0c\x63onfig_oneof\"\xaa\x02\n\x0eMetricAnalysis\x12J\n\x0csuccess_rate\x18\x02 \x01(\x0b\x32\x32.prodvana.service.MetricAnalysis.SuccessRateConfigH\x00\x12\x45\n\x0blatency_p95\x18\x03 \x01(\x0b\x32..prodvana.service.MetricAnalysis.LatencyConfigH\x00\x1a\x32\n\x11SuccessRateConfig\x12\x1d\n\x15min_threshold_percent\x18\x01 \x01(\x01\x1a?\n\rLatencyConfig\x12.\n\x0bmax_latency\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationB\x10\n\x0e\x61nalysis_oneof\"\xb7\x02\n\x15ReleaseStrategyConfig\x12<\n\x19individual_stage_deadline\x18\x01 \x01(\x0b\x32\x19.google.protobuf.Duration\x12=\n\x1a\x61utomated_testing_duration\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\x12:\n\x10metrics_analysis\x18\x03 \x03(\x0b\x32 .prodvana.service.MetricAnalysis\x12\x17\n\x0fmanual_approval\x18\x04 \x01(\x08\x12\x31\n\x0e\x63heck_interval\x18\x05 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x19\n\x11\x66\x61ilure_threshold\x18\x06 \x01(\x05\"f\n\tTLSSecret\x12\x14\n\nraw_secret\x18\x03 \x01(\tH\x00\x12\x30\n\x06secret\x18\x04 \x01(\x0b\x32\x1e.prodvana.common_config.SecretH\x00\x42\x11\n\ntls_secret\x12\x03\xf8\x42\x01\"\x81\x01\n\x0eTLSCertificate\x12\x37\n\x08tls_cert\x18\x01 \x01(\x0b\x32\x1b.prodvana.service.TLSSecretB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x36\n\x07tls_key\x18\x02 \x01(\x0b\x32\x1b.prodvana.service.TLSSecretB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\"j\n\x0b\x43\x65rtificate\x12/\n\x03tls\x18\x01 \x01(\x0b\x32 .prodvana.service.TLSCertificateH\x00\x12\x16\n\x0c\x61ws_acm_cert\x18\x02 \x01(\tH\x00\x42\x12\n\x0b\x63\x65rtificate\x12\x03\xf8\x42\x01\"\xc4\x07\n\x17PerReleaseChannelConfig\x12 \n\x0frelease_channel\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12&\n\x10\x63ustom_hostnames\x18\x02 \x03(\tB\x0c\xfa\x42\t\x92\x01\x06\"\x04r\x02h\x01\x12W\n\x08programs\x18\x05 \x03(\x0b\x32\x36.prodvana.common_config.PerReleaseChannelProgramConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12+\n\x04\x63\x65rt\x18\x06 \x01(\x0b\x32\x1d.prodvana.service.Certificate\x12:\n\x0f\x64\x65livery_config\x18\x07 \x01(\x0b\x32!.prodvana.delivery.DeliveryConfig\x12\x38\n\x07volumes\x18\x08 \x03(\x0b\x32\x18.prodvana.volumes.VolumeB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x32\n\x08replicas\x18\t \x01(\x0b\x32 .prodvana.service.ReplicasConfig\x12\x43\n\x0epre_push_tasks\x18\n \x03(\x0b\x32\x1c.prodvana.service.TaskConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12U\n\x13\x64\x65livery_extensions\x18\x12 \x03(\x0b\x32).prodvana.service.DeliveryExtensionConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x41\n\x10runtime_specific\x18\x0b \x01(\x0b\x32\'.prodvana.service.RuntimeSpecificConfig\x12\x1a\n\x12runtime_connection\x18\x11 \x01(\t\x12\x45\n\x11runtime_extension\x18\r \x01(\x0b\x32(.prodvana.service.RuntimeExtensionConfigH\x00\x12\x45\n\x11kubernetes_config\x18\x0e \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x43\n\x0f\x65xternal_config\x18\x10 \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x32\n\x04helm\x18\x0f \x01(\x0b\x32\".prodvana.common_config.HelmConfigH\x00\x42\x0e\n\x0c\x63onfig_oneofJ\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x0c\x10\rR\x0bprotections\",\n\x13\x43\x61pabilityReference\x12\x15\n\x04name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"U\n\x18\x43ompiledCapabilityConfig\x12\x39\n\ncapability\x18\x01 \x01(\x0b\x32%.prodvana.capability.CapabilityConfig\".\n\x10ProgramReference\x12\x0e\n\x04name\x18\x01 \x01(\tH\x00\x42\n\n\x03ref\x12\x03\xf8\x42\x01\"6\n\rTaskReference\x12\x19\n\x0frelease_channel\x18\x01 \x01(\tH\x00\x42\n\n\x03ref\x12\x03\xf8\x42\x01\"\xf1\x01\n\nTaskConfig\x12@\n\x07program\x18\x01 \x01(\x0b\x32%.prodvana.common_config.ProgramConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x38\n\x0c\x62\x61se_program\x18\x02 \x01(\x0b\x32\".prodvana.service.ProgramReference\x12\x39\n\x0cretry_config\x18\x03 \x01(\x0b\x32#.prodvana.common_config.RetryConfig\x12,\n\x03ref\x18\x04 \x01(\x0b\x32\x1f.prodvana.service.TaskReference\"p\n\x0eProtectionLink\x12;\n\tlifecycle\x18\x03 \x01(\x0b\x32(.prodvana.protection.ProtectionLifecycle\x12\x15\n\rattachment_id\x18\x04 \x01(\tJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03\"\xb9\x01\n\x17\x44\x65liveryExtensionConfig\x12G\n\x07inlined\x18\x01 \x01(\x0b\x32\x34.prodvana.delivery_extension.DeliveryExtensionConfigH\x00\x12\x42\n\tlifecycle\x18\x02 \x01(\x0e\x32%.prodvana.common_config.TaskLifecycleB\x08\xfa\x42\x05\x82\x01\x02 \x00\x42\x11\n\ndefinition\x12\x03\xf8\x42\x01\"\x9c\x02\n\x15RuntimeSpecificConfig\x12@\n\x03k8s\x18\x01 \x01(\x0b\x32\x31.prodvana.service.RuntimeSpecificConfig.K8SConfigH\x00\x1a\xae\x01\n\tK8SConfig\x12\x66\n\x13service_annotations\x18\x01 \x03(\x0b\x32I.prodvana.service.RuntimeSpecificConfig.K8SConfig.ServiceAnnotationsEntry\x1a\x39\n\x17ServiceAnnotationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\x10\n\x0eruntime_config\"Z\n\x16RuntimeExtensionConfig\x12@\n\x10parameter_values\x18\x01 \x03(\x0b\x32&.prodvana.common_config.ParameterValue\"&\n\x12\x41utoRollbackConfig\x12\x10\n\x08\x64isabled\x18\x01 \x01(\x08\"\xec\x01\n\x1fProtectionConvergenceAttachment\x12:\n\x04name\x18\x01 \x01(\tB,\xfa\x42)r\'\x10\x00\x18?2!^[a-z]?([a-z0-9-]*[a-z0-9]){0,1}$\x12?\n\x03ref\x18\x02 \x01(\x0b\x32(.prodvana.protection.ProtectionReferenceB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12L\n\tlifecycle\x18\x03 \x03(\x0b\x32(.prodvana.protection.ProtectionLifecycleB\x0f\xfa\x42\x0c\x92\x01\t\x08\x01\"\x05\x8a\x01\x02\x10\x01\"\xad\r\n\rServiceConfig\x12\x39\n\x04name\x18\x01 \x01(\tB+\xfa\x42(r&\x10\x01\x18?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$\x12\x13\n\x0b\x61pplication\x18\x14 \x01(\t\x12\x46\n\x08programs\x18\x02 \x03(\x0b\x32%.prodvana.common_config.ProgramConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x32\n\x08replicas\x18\x04 \x01(\x0b\x32 .prodvana.service.ReplicasConfig\x12\x41\n\x10release_strategy\x18\x05 \x01(\x0b\x32\'.prodvana.service.ReleaseStrategyConfig\x12U\n\x13per_release_channel\x18\t \x03(\x0b\x32).prodvana.service.PerReleaseChannelConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12J\n\x0c\x63\x61pabilities\x18\n \x03(\x0b\x32%.prodvana.service.CapabilityReferenceB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12:\n\x0f\x64\x65livery_config\x18\x0b \x01(\x0b\x32!.prodvana.delivery.DeliveryConfig\x12\x38\n\x07volumes\x18\x0c \x03(\x0b\x32\x18.prodvana.volumes.VolumeB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12@\n\x12\x64\x65ploy_annotations\x18\r \x01(\x0b\x32$.prodvana.workflow.AnnotationsConfig\x12\x41\n\rbase_template\x18\x0e \x01(\x0b\x32*.prodvana.common_config.ServiceTemplateRef\x12\x34\n\x0epre_push_tasks\x18\x0f \x03(\x0b\x32\x1c.prodvana.service.TaskConfig\x12\x46\n\x13\x64\x65livery_extensions\x18\x1d \x03(\x0b\x32).prodvana.service.DeliveryExtensionConfig\x12\x41\n\x10runtime_specific\x18\x10 \x01(\x0b\x32\'.prodvana.service.RuntimeSpecificConfig\x12\x1a\n\x12runtime_connection\x18\x1c \x01(\t\x12N\n\nparameters\x18\x15 \x03(\x0b\x32+.prodvana.common_config.ParameterDefinitionB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x42\n\x10parameter_values\x18\x16 \x01(\x0b\x32(.prodvana.service.ServiceParameterValues\x12\x34\n\x11progress_deadline\x18\x18 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x45\n\x11runtime_extension\x18\x12 \x01(\x0b\x32(.prodvana.service.RuntimeExtensionConfigH\x00\x12\x45\n\x11kubernetes_config\x18\x13 \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x43\n\x0f\x65xternal_config\x18\x1b \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x32\n\x04helm\x18\x1a \x01(\x0b\x32\".prodvana.common_config.HelmConfigH\x00\x12M\n\x12parameters_autogen\x18\x17 \x01(\x0e\x32\x31.prodvana.service.ServiceConfig.ParametersAutogen\x12;\n\rauto_rollback\x18\x19 \x01(\x0b\x32$.prodvana.service.AutoRollbackConfig\"M\n\x11ParametersAutogen\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04NONE\x10\x01\x12\t\n\x05IMAGE\x10\x02\x12\x16\n\x12IMAGE_AND_REPLICAS\x10\x03\x42\x0e\n\x0c\x63onfig_oneofJ\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08J\x04\x08\x08\x10\tJ\x04\x08\x11\x10\x12R\x08\x65xternalR\x10image_repositoryR\x15\x63ontainer_registry_idR\x0bprotections\"\x91\r\n\x1d\x43ompiledServiceInstanceConfig\x12\x0f\n\x07service\x18\x01 \x01(\t\x12\x13\n\x0b\x61pplication\x18\x12 \x01(\t\x12\x17\n\x0frelease_channel\x18\x02 \x01(\t\x12\x37\n\x08programs\x18\x03 \x03(\x0b\x32%.prodvana.common_config.ProgramConfig\x12\x32\n\x08replicas\x18\x04 \x01(\x0b\x32 .prodvana.service.ReplicasConfig\x12\x32\n\x08maturity\x18\x05 \x01(\x0e\x32 .prodvana.common_config.Maturity\x12\x41\n\x10release_strategy\x18\x06 \x01(\x0b\x32\'.prodvana.service.ReleaseStrategyConfig\x12\x18\n\x10\x63ustom_hostnames\x18\x07 \x03(\t\x12+\n\x04\x63\x65rt\x18\n \x01(\x0b\x32\x1d.prodvana.service.Certificate\x12\x46\n\x07runtime\x18\x0b \x01(\x0b\x32\x35.prodvana.release_channel.ReleaseChannelRuntimeConfig\x12\x44\n\x11runtime_execution\x18\x1b \x01(\x0b\x32).prodvana.runtimes.RuntimeExecutionConfig\x12@\n\x0c\x63\x61pabilities\x18\x0c \x03(\x0b\x32*.prodvana.service.CompiledCapabilityConfig\x12:\n\x0f\x64\x65livery_config\x18\r \x01(\x0b\x32!.prodvana.delivery.DeliveryConfig\x12\x38\n\x07volumes\x18\x0e \x03(\x0b\x32\x18.prodvana.volumes.VolumeB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12@\n\x12\x64\x65ploy_annotations\x18\x0f \x01(\x0b\x32$.prodvana.workflow.AnnotationsConfig\x12\x41\n\rbase_template\x18\x10 \x01(\x0b\x32*.prodvana.common_config.ServiceTemplateRef\x12\x34\n\x0epre_push_tasks\x18\x11 \x03(\x0b\x32\x1c.prodvana.service.TaskConfig\x12\x46\n\x13\x64\x65livery_extensions\x18\x1e \x03(\x0b\x32).prodvana.service.DeliveryExtensionConfig\x12\x41\n\x10runtime_specific\x18\x13 \x01(\x0b\x32\'.prodvana.service.RuntimeSpecificConfig\x12?\n\nparameters\x18\x18 \x03(\x0b\x32+.prodvana.common_config.ParameterDefinition\x12@\n\x10parameter_values\x18\x19 \x03(\x0b\x32&.prodvana.common_config.ParameterValue\x12\x34\n\x11progress_deadline\x18\x1a \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x45\n\x11runtime_extension\x18\x16 \x01(\x0b\x32(.prodvana.service.RuntimeExtensionConfigH\x00\x12\x45\n\x11kubernetes_config\x18\x17 \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x32\n\x04helm\x18\x1d \x01(\x0b\x32\".prodvana.common_config.HelmConfigH\x00\x12n\n\x03\x65nv\x18\x1c \x03(\x0b\x32\x38.prodvana.service.CompiledServiceInstanceConfig.EnvEntryB\'\xfa\x42$\x9a\x01!\x18\x01\"\x1dr\x1b\x32\x19^[a-zA-Z_]+[a-zA-Z0-9_]*$\x1aL\n\x08\x45nvEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .prodvana.common_config.EnvValue:\x02\x38\x01\x42\x0e\n\x0c\x63onfig_oneofJ\x04\x08\x08\x10\tJ\x04\x08\t\x10\nJ\x04\x08\x14\x10\x15J\x04\x08\x15\x10\x16R\x0bprotectionsR\x0cruntime_type\"\x88\x02\n\x11\x43ompiledJobConfig\x12\x13\n\x0bname_prefix\x18\x01 \x01(\t\x12\x17\n\x0frelease_channel\x18\x02 \x01(\t\x12\x37\n\x08programs\x18\x03 \x03(\x0b\x32%.prodvana.common_config.ProgramConfig\x12\x46\n\x07runtime\x18\x04 \x01(\x0b\x32\x35.prodvana.release_channel.ReleaseChannelRuntimeConfig\x12\x44\n\x11runtime_execution\x18\x05 \x01(\x0b\x32).prodvana.runtimes.RuntimeExecutionConfigBLZJgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/serviceb\x06proto3')
 
 
 
 _REPLICASCONFIG = DESCRIPTOR.message_types_by_name['ReplicasConfig']
 _METRICANALYSIS = DESCRIPTOR.message_types_by_name['MetricAnalysis']
 _METRICANALYSIS_SUCCESSRATECONFIG = _METRICANALYSIS.nested_types_by_name['SuccessRateConfig']
 _METRICANALYSIS_LATENCYCONFIG = _METRICANALYSIS.nested_types_by_name['LatencyConfig']
@@ -46,14 +48,16 @@
 _CERTIFICATE = DESCRIPTOR.message_types_by_name['Certificate']
 _PERRELEASECHANNELCONFIG = DESCRIPTOR.message_types_by_name['PerReleaseChannelConfig']
 _CAPABILITYREFERENCE = DESCRIPTOR.message_types_by_name['CapabilityReference']
 _COMPILEDCAPABILITYCONFIG = DESCRIPTOR.message_types_by_name['CompiledCapabilityConfig']
 _PROGRAMREFERENCE = DESCRIPTOR.message_types_by_name['ProgramReference']
 _TASKREFERENCE = DESCRIPTOR.message_types_by_name['TaskReference']
 _TASKCONFIG = DESCRIPTOR.message_types_by_name['TaskConfig']
+_PROTECTIONLINK = DESCRIPTOR.message_types_by_name['ProtectionLink']
+_DELIVERYEXTENSIONCONFIG = DESCRIPTOR.message_types_by_name['DeliveryExtensionConfig']
 _RUNTIMESPECIFICCONFIG = DESCRIPTOR.message_types_by_name['RuntimeSpecificConfig']
 _RUNTIMESPECIFICCONFIG_K8SCONFIG = _RUNTIMESPECIFICCONFIG.nested_types_by_name['K8SConfig']
 _RUNTIMESPECIFICCONFIG_K8SCONFIG_SERVICEANNOTATIONSENTRY = _RUNTIMESPECIFICCONFIG_K8SCONFIG.nested_types_by_name['ServiceAnnotationsEntry']
 _RUNTIMEEXTENSIONCONFIG = DESCRIPTOR.message_types_by_name['RuntimeExtensionConfig']
 _AUTOROLLBACKCONFIG = DESCRIPTOR.message_types_by_name['AutoRollbackConfig']
 _PROTECTIONCONVERGENCEATTACHMENT = DESCRIPTOR.message_types_by_name['ProtectionConvergenceAttachment']
 _SERVICECONFIG = DESCRIPTOR.message_types_by_name['ServiceConfig']
@@ -157,14 +161,28 @@
 TaskConfig = _reflection.GeneratedProtocolMessageType('TaskConfig', (_message.Message,), {
   'DESCRIPTOR' : _TASKCONFIG,
   '__module__' : 'prodvana.service.service_config_pb2'
   # @@protoc_insertion_point(class_scope:prodvana.service.TaskConfig)
   })
 _sym_db.RegisterMessage(TaskConfig)
 
+ProtectionLink = _reflection.GeneratedProtocolMessageType('ProtectionLink', (_message.Message,), {
+  'DESCRIPTOR' : _PROTECTIONLINK,
+  '__module__' : 'prodvana.service.service_config_pb2'
+  # @@protoc_insertion_point(class_scope:prodvana.service.ProtectionLink)
+  })
+_sym_db.RegisterMessage(ProtectionLink)
+
+DeliveryExtensionConfig = _reflection.GeneratedProtocolMessageType('DeliveryExtensionConfig', (_message.Message,), {
+  'DESCRIPTOR' : _DELIVERYEXTENSIONCONFIG,
+  '__module__' : 'prodvana.service.service_config_pb2'
+  # @@protoc_insertion_point(class_scope:prodvana.service.DeliveryExtensionConfig)
+  })
+_sym_db.RegisterMessage(DeliveryExtensionConfig)
+
 RuntimeSpecificConfig = _reflection.GeneratedProtocolMessageType('RuntimeSpecificConfig', (_message.Message,), {
 
   'K8SConfig' : _reflection.GeneratedProtocolMessageType('K8SConfig', (_message.Message,), {
 
     'ServiceAnnotationsEntry' : _reflection.GeneratedProtocolMessageType('ServiceAnnotationsEntry', (_message.Message,), {
       'DESCRIPTOR' : _RUNTIMESPECIFICCONFIG_K8SCONFIG_SERVICEANNOTATIONSENTRY,
       '__module__' : 'prodvana.service.service_config_pb2'
@@ -252,22 +270,28 @@
   _PERRELEASECHANNELCONFIG.fields_by_name['custom_hostnames']._serialized_options = b'\372B\t\222\001\006\"\004r\002h\001'
   _PERRELEASECHANNELCONFIG.fields_by_name['programs']._options = None
   _PERRELEASECHANNELCONFIG.fields_by_name['programs']._serialized_options = b'\372B\n\222\001\007\"\005\212\001\002\020\001'
   _PERRELEASECHANNELCONFIG.fields_by_name['volumes']._options = None
   _PERRELEASECHANNELCONFIG.fields_by_name['volumes']._serialized_options = b'\372B\n\222\001\007\"\005\212\001\002\020\001'
   _PERRELEASECHANNELCONFIG.fields_by_name['pre_push_tasks']._options = None
   _PERRELEASECHANNELCONFIG.fields_by_name['pre_push_tasks']._serialized_options = b'\372B\n\222\001\007\"\005\212\001\002\020\001'
+  _PERRELEASECHANNELCONFIG.fields_by_name['delivery_extensions']._options = None
+  _PERRELEASECHANNELCONFIG.fields_by_name['delivery_extensions']._serialized_options = b'\372B\n\222\001\007\"\005\212\001\002\020\001'
   _CAPABILITYREFERENCE.fields_by_name['name']._options = None
   _CAPABILITYREFERENCE.fields_by_name['name']._serialized_options = b'\372B\004r\002\020\001'
   _PROGRAMREFERENCE.oneofs_by_name['ref']._options = None
   _PROGRAMREFERENCE.oneofs_by_name['ref']._serialized_options = b'\370B\001'
   _TASKREFERENCE.oneofs_by_name['ref']._options = None
   _TASKREFERENCE.oneofs_by_name['ref']._serialized_options = b'\370B\001'
   _TASKCONFIG.fields_by_name['program']._options = None
   _TASKCONFIG.fields_by_name['program']._serialized_options = b'\372B\005\212\001\002\020\001'
+  _DELIVERYEXTENSIONCONFIG.oneofs_by_name['definition']._options = None
+  _DELIVERYEXTENSIONCONFIG.oneofs_by_name['definition']._serialized_options = b'\370B\001'
+  _DELIVERYEXTENSIONCONFIG.fields_by_name['lifecycle']._options = None
+  _DELIVERYEXTENSIONCONFIG.fields_by_name['lifecycle']._serialized_options = b'\372B\005\202\001\002 \000'
   _RUNTIMESPECIFICCONFIG_K8SCONFIG_SERVICEANNOTATIONSENTRY._options = None
   _RUNTIMESPECIFICCONFIG_K8SCONFIG_SERVICEANNOTATIONSENTRY._serialized_options = b'8\001'
   _PROTECTIONCONVERGENCEATTACHMENT.fields_by_name['name']._options = None
   _PROTECTIONCONVERGENCEATTACHMENT.fields_by_name['name']._serialized_options = b'\372B)r\'\020\000\030?2!^[a-z]?([a-z0-9-]*[a-z0-9]){0,1}$'
   _PROTECTIONCONVERGENCEATTACHMENT.fields_by_name['ref']._options = None
   _PROTECTIONCONVERGENCEATTACHMENT.fields_by_name['ref']._serialized_options = b'\372B\005\212\001\002\020\001'
   _PROTECTIONCONVERGENCEATTACHMENT.fields_by_name['lifecycle']._options = None
@@ -286,58 +310,62 @@
   _SERVICECONFIG.fields_by_name['parameters']._serialized_options = b'\372B\n\222\001\007\"\005\212\001\002\020\001'
   _COMPILEDSERVICEINSTANCECONFIG_ENVENTRY._options = None
   _COMPILEDSERVICEINSTANCECONFIG_ENVENTRY._serialized_options = b'8\001'
   _COMPILEDSERVICEINSTANCECONFIG.fields_by_name['volumes']._options = None
   _COMPILEDSERVICEINSTANCECONFIG.fields_by_name['volumes']._serialized_options = b'\372B\n\222\001\007\"\005\212\001\002\020\001'
   _COMPILEDSERVICEINSTANCECONFIG.fields_by_name['env']._options = None
   _COMPILEDSERVICEINSTANCECONFIG.fields_by_name['env']._serialized_options = b'\372B$\232\001!\030\001\"\035r\0332\031^[a-zA-Z_]+[a-zA-Z0-9_]*$'
-  _REPLICASCONFIG._serialized_start=755
-  _REPLICASCONFIG._serialized_end=804
-  _METRICANALYSIS._serialized_start=807
-  _METRICANALYSIS._serialized_end=1105
-  _METRICANALYSIS_SUCCESSRATECONFIG._serialized_start=972
-  _METRICANALYSIS_SUCCESSRATECONFIG._serialized_end=1022
-  _METRICANALYSIS_LATENCYCONFIG._serialized_start=1024
-  _METRICANALYSIS_LATENCYCONFIG._serialized_end=1087
-  _RELEASESTRATEGYCONFIG._serialized_start=1108
-  _RELEASESTRATEGYCONFIG._serialized_end=1419
-  _TLSSECRET._serialized_start=1421
-  _TLSSECRET._serialized_end=1523
-  _TLSCERTIFICATE._serialized_start=1526
-  _TLSCERTIFICATE._serialized_end=1655
-  _CERTIFICATE._serialized_start=1657
-  _CERTIFICATE._serialized_end=1763
-  _PERRELEASECHANNELCONFIG._serialized_start=1766
-  _PERRELEASECHANNELCONFIG._serialized_end=2643
-  _CAPABILITYREFERENCE._serialized_start=2645
-  _CAPABILITYREFERENCE._serialized_end=2689
-  _COMPILEDCAPABILITYCONFIG._serialized_start=2691
-  _COMPILEDCAPABILITYCONFIG._serialized_end=2776
-  _PROGRAMREFERENCE._serialized_start=2778
-  _PROGRAMREFERENCE._serialized_end=2824
-  _TASKREFERENCE._serialized_start=2826
-  _TASKREFERENCE._serialized_end=2880
-  _TASKCONFIG._serialized_start=2883
-  _TASKCONFIG._serialized_end=3124
-  _RUNTIMESPECIFICCONFIG._serialized_start=3127
-  _RUNTIMESPECIFICCONFIG._serialized_end=3411
-  _RUNTIMESPECIFICCONFIG_K8SCONFIG._serialized_start=3219
-  _RUNTIMESPECIFICCONFIG_K8SCONFIG._serialized_end=3393
-  _RUNTIMESPECIFICCONFIG_K8SCONFIG_SERVICEANNOTATIONSENTRY._serialized_start=3336
-  _RUNTIMESPECIFICCONFIG_K8SCONFIG_SERVICEANNOTATIONSENTRY._serialized_end=3393
-  _RUNTIMEEXTENSIONCONFIG._serialized_start=3413
-  _RUNTIMEEXTENSIONCONFIG._serialized_end=3503
-  _AUTOROLLBACKCONFIG._serialized_start=3505
-  _AUTOROLLBACKCONFIG._serialized_end=3543
-  _PROTECTIONCONVERGENCEATTACHMENT._serialized_start=3546
-  _PROTECTIONCONVERGENCEATTACHMENT._serialized_end=3782
-  _SERVICECONFIG._serialized_start=3785
-  _SERVICECONFIG._serialized_end=5422
-  _SERVICECONFIG_PARAMETERSAUTOGEN._serialized_start=5241
-  _SERVICECONFIG_PARAMETERSAUTOGEN._serialized_end=5318
-  _COMPILEDSERVICEINSTANCECONFIG._serialized_start=5425
-  _COMPILEDSERVICEINSTANCECONFIG._serialized_end=7034
-  _COMPILEDSERVICEINSTANCECONFIG_ENVENTRY._serialized_start=6891
-  _COMPILEDSERVICEINSTANCECONFIG_ENVENTRY._serialized_end=6967
-  _COMPILEDJOBCONFIG._serialized_start=7037
-  _COMPILEDJOBCONFIG._serialized_end=7301
+  _REPLICASCONFIG._serialized_start=832
+  _REPLICASCONFIG._serialized_end=881
+  _METRICANALYSIS._serialized_start=884
+  _METRICANALYSIS._serialized_end=1182
+  _METRICANALYSIS_SUCCESSRATECONFIG._serialized_start=1049
+  _METRICANALYSIS_SUCCESSRATECONFIG._serialized_end=1099
+  _METRICANALYSIS_LATENCYCONFIG._serialized_start=1101
+  _METRICANALYSIS_LATENCYCONFIG._serialized_end=1164
+  _RELEASESTRATEGYCONFIG._serialized_start=1185
+  _RELEASESTRATEGYCONFIG._serialized_end=1496
+  _TLSSECRET._serialized_start=1498
+  _TLSSECRET._serialized_end=1600
+  _TLSCERTIFICATE._serialized_start=1603
+  _TLSCERTIFICATE._serialized_end=1732
+  _CERTIFICATE._serialized_start=1734
+  _CERTIFICATE._serialized_end=1840
+  _PERRELEASECHANNELCONFIG._serialized_start=1843
+  _PERRELEASECHANNELCONFIG._serialized_end=2807
+  _CAPABILITYREFERENCE._serialized_start=2809
+  _CAPABILITYREFERENCE._serialized_end=2853
+  _COMPILEDCAPABILITYCONFIG._serialized_start=2855
+  _COMPILEDCAPABILITYCONFIG._serialized_end=2940
+  _PROGRAMREFERENCE._serialized_start=2942
+  _PROGRAMREFERENCE._serialized_end=2988
+  _TASKREFERENCE._serialized_start=2990
+  _TASKREFERENCE._serialized_end=3044
+  _TASKCONFIG._serialized_start=3047
+  _TASKCONFIG._serialized_end=3288
+  _PROTECTIONLINK._serialized_start=3290
+  _PROTECTIONLINK._serialized_end=3402
+  _DELIVERYEXTENSIONCONFIG._serialized_start=3405
+  _DELIVERYEXTENSIONCONFIG._serialized_end=3590
+  _RUNTIMESPECIFICCONFIG._serialized_start=3593
+  _RUNTIMESPECIFICCONFIG._serialized_end=3877
+  _RUNTIMESPECIFICCONFIG_K8SCONFIG._serialized_start=3685
+  _RUNTIMESPECIFICCONFIG_K8SCONFIG._serialized_end=3859
+  _RUNTIMESPECIFICCONFIG_K8SCONFIG_SERVICEANNOTATIONSENTRY._serialized_start=3802
+  _RUNTIMESPECIFICCONFIG_K8SCONFIG_SERVICEANNOTATIONSENTRY._serialized_end=3859
+  _RUNTIMEEXTENSIONCONFIG._serialized_start=3879
+  _RUNTIMEEXTENSIONCONFIG._serialized_end=3969
+  _AUTOROLLBACKCONFIG._serialized_start=3971
+  _AUTOROLLBACKCONFIG._serialized_end=4009
+  _PROTECTIONCONVERGENCEATTACHMENT._serialized_start=4012
+  _PROTECTIONCONVERGENCEATTACHMENT._serialized_end=4248
+  _SERVICECONFIG._serialized_start=4251
+  _SERVICECONFIG._serialized_end=5960
+  _SERVICECONFIG_PARAMETERSAUTOGEN._serialized_start=5779
+  _SERVICECONFIG_PARAMETERSAUTOGEN._serialized_end=5856
+  _COMPILEDSERVICEINSTANCECONFIG._serialized_start=5963
+  _COMPILEDSERVICEINSTANCECONFIG._serialized_end=7644
+  _COMPILEDSERVICEINSTANCECONFIG_ENVENTRY._serialized_start=7501
+  _COMPILEDSERVICEINSTANCECONFIG_ENVENTRY._serialized_end=7577
+  _COMPILEDJOBCONFIG._serialized_start=7647
+  _COMPILEDJOBCONFIG._serialized_end=7911
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/service/service_config_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/service/service_config_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 import prodvana.proto.prodvana.common_config.helm_pb2
 import prodvana.proto.prodvana.common_config.kubernetes_config_pb2
 import prodvana.proto.prodvana.common_config.maturity_pb2
 import prodvana.proto.prodvana.common_config.parameters_pb2
 import prodvana.proto.prodvana.common_config.program_pb2
 import prodvana.proto.prodvana.common_config.ref_pb2
 import prodvana.proto.prodvana.common_config.retry_pb2
+import prodvana.proto.prodvana.common_config.task_pb2
 import prodvana.proto.prodvana.delivery.delivery_config_pb2
+import prodvana.proto.prodvana.delivery_extension.config_pb2
 import prodvana.proto.prodvana.protection.protection_reference_pb2
 import prodvana.proto.prodvana.release_channel.release_channel_config_pb2
 import prodvana.proto.prodvana.runtimes.runtimes_config_pb2
 import prodvana.proto.prodvana.service.parameters_pb2
 import prodvana.proto.prodvana.volumes.volumes_pb2
 import prodvana.proto.prodvana.workflow.integration_config_pb2
 import sys
@@ -208,14 +210,15 @@
     CUSTOM_HOSTNAMES_FIELD_NUMBER: builtins.int
     PROGRAMS_FIELD_NUMBER: builtins.int
     CERT_FIELD_NUMBER: builtins.int
     DELIVERY_CONFIG_FIELD_NUMBER: builtins.int
     VOLUMES_FIELD_NUMBER: builtins.int
     REPLICAS_FIELD_NUMBER: builtins.int
     PRE_PUSH_TASKS_FIELD_NUMBER: builtins.int
+    DELIVERY_EXTENSIONS_FIELD_NUMBER: builtins.int
     RUNTIME_SPECIFIC_FIELD_NUMBER: builtins.int
     RUNTIME_CONNECTION_FIELD_NUMBER: builtins.int
     RUNTIME_EXTENSION_FIELD_NUMBER: builtins.int
     KUBERNETES_CONFIG_FIELD_NUMBER: builtins.int
     EXTERNAL_CONFIG_FIELD_NUMBER: builtins.int
     HELM_FIELD_NUMBER: builtins.int
     release_channel: builtins.str
@@ -228,15 +231,18 @@
     @property
     def delivery_config(self) -> prodvana.proto.prodvana.delivery.delivery_config_pb2.DeliveryConfig: ...
     @property
     def volumes(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.volumes.volumes_pb2.Volume]: ...
     @property
     def replicas(self) -> global___ReplicasConfig: ...
     @property
-    def pre_push_tasks(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___TaskConfig]: ...
+    def pre_push_tasks(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___TaskConfig]:
+        """DEPRECATED: Replace with delivery_extensions once its implemented."""
+    @property
+    def delivery_extensions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___DeliveryExtensionConfig]: ...
     @property
     def runtime_specific(self) -> global___RuntimeSpecificConfig: ...
     runtime_connection: builtins.str
     """which runtime connection to use in each release channel.
     optional if only one runtime makes sense for the service config.
     """
     @property
@@ -255,23 +261,24 @@
         custom_hostnames: collections.abc.Iterable[builtins.str] | None = ...,
         programs: collections.abc.Iterable[prodvana.proto.prodvana.common_config.program_pb2.PerReleaseChannelProgramConfig] | None = ...,
         cert: global___Certificate | None = ...,
         delivery_config: prodvana.proto.prodvana.delivery.delivery_config_pb2.DeliveryConfig | None = ...,
         volumes: collections.abc.Iterable[prodvana.proto.prodvana.volumes.volumes_pb2.Volume] | None = ...,
         replicas: global___ReplicasConfig | None = ...,
         pre_push_tasks: collections.abc.Iterable[global___TaskConfig] | None = ...,
+        delivery_extensions: collections.abc.Iterable[global___DeliveryExtensionConfig] | None = ...,
         runtime_specific: global___RuntimeSpecificConfig | None = ...,
         runtime_connection: builtins.str = ...,
         runtime_extension: global___RuntimeExtensionConfig | None = ...,
         kubernetes_config: prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig | None = ...,
         external_config: prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig | None = ...,
         helm: prodvana.proto.prodvana.common_config.helm_pb2.HelmConfig | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["cert", b"cert", "config_oneof", b"config_oneof", "delivery_config", b"delivery_config", "external_config", b"external_config", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "replicas", b"replicas", "runtime_extension", b"runtime_extension", "runtime_specific", b"runtime_specific"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["cert", b"cert", "config_oneof", b"config_oneof", "custom_hostnames", b"custom_hostnames", "delivery_config", b"delivery_config", "external_config", b"external_config", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "pre_push_tasks", b"pre_push_tasks", "programs", b"programs", "release_channel", b"release_channel", "replicas", b"replicas", "runtime_connection", b"runtime_connection", "runtime_extension", b"runtime_extension", "runtime_specific", b"runtime_specific", "volumes", b"volumes"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["cert", b"cert", "config_oneof", b"config_oneof", "custom_hostnames", b"custom_hostnames", "delivery_config", b"delivery_config", "delivery_extensions", b"delivery_extensions", "external_config", b"external_config", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "pre_push_tasks", b"pre_push_tasks", "programs", b"programs", "release_channel", b"release_channel", "replicas", b"replicas", "runtime_connection", b"runtime_connection", "runtime_extension", b"runtime_extension", "runtime_specific", b"runtime_specific", "volumes", b"volumes"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["config_oneof", b"config_oneof"]) -> typing_extensions.Literal["runtime_extension", "kubernetes_config", "external_config", "helm"] | None: ...
 
 global___PerReleaseChannelConfig = PerReleaseChannelConfig
 
 class CapabilityReference(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
@@ -366,14 +373,53 @@
         ref: global___TaskReference | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["base_program", b"base_program", "program", b"program", "ref", b"ref", "retry_config", b"retry_config"]) -> builtins.bool: ...
     def ClearField(self, field_name: typing_extensions.Literal["base_program", b"base_program", "program", b"program", "ref", b"ref", "retry_config", b"retry_config"]) -> None: ...
 
 global___TaskConfig = TaskConfig
 
+class ProtectionLink(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    LIFECYCLE_FIELD_NUMBER: builtins.int
+    ATTACHMENT_ID_FIELD_NUMBER: builtins.int
+    @property
+    def lifecycle(self) -> prodvana.proto.prodvana.protection.protection_reference_pb2.ProtectionLifecycle: ...
+    attachment_id: builtins.str
+    def __init__(
+        self,
+        *,
+        lifecycle: prodvana.proto.prodvana.protection.protection_reference_pb2.ProtectionLifecycle | None = ...,
+        attachment_id: builtins.str = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["lifecycle", b"lifecycle"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["attachment_id", b"attachment_id", "lifecycle", b"lifecycle"]) -> None: ...
+
+global___ProtectionLink = ProtectionLink
+
+class DeliveryExtensionConfig(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    INLINED_FIELD_NUMBER: builtins.int
+    LIFECYCLE_FIELD_NUMBER: builtins.int
+    @property
+    def inlined(self) -> prodvana.proto.prodvana.delivery_extension.config_pb2.DeliveryExtensionConfig: ...
+    lifecycle: prodvana.proto.prodvana.common_config.task_pb2.TaskLifecycle.ValueType
+    def __init__(
+        self,
+        *,
+        inlined: prodvana.proto.prodvana.delivery_extension.config_pb2.DeliveryExtensionConfig | None = ...,
+        lifecycle: prodvana.proto.prodvana.common_config.task_pb2.TaskLifecycle.ValueType = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["definition", b"definition", "inlined", b"inlined"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["definition", b"definition", "inlined", b"inlined", "lifecycle", b"lifecycle"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["definition", b"definition"]) -> typing_extensions.Literal["inlined"] | None: ...
+
+global___DeliveryExtensionConfig = DeliveryExtensionConfig
+
 class RuntimeSpecificConfig(google.protobuf.message.Message):
     """RuntimeSpecificConfig contains Service level configuration options that only make sense for a
     specific Runtime type. Configuration added here should only apply to a single Service; if the
     Runtime specific configuration relates to all services, it should be configured as at the
     Runtime cluster level (or as a runtime extension).
     """
 
@@ -509,14 +555,15 @@
     PER_RELEASE_CHANNEL_FIELD_NUMBER: builtins.int
     CAPABILITIES_FIELD_NUMBER: builtins.int
     DELIVERY_CONFIG_FIELD_NUMBER: builtins.int
     VOLUMES_FIELD_NUMBER: builtins.int
     DEPLOY_ANNOTATIONS_FIELD_NUMBER: builtins.int
     BASE_TEMPLATE_FIELD_NUMBER: builtins.int
     PRE_PUSH_TASKS_FIELD_NUMBER: builtins.int
+    DELIVERY_EXTENSIONS_FIELD_NUMBER: builtins.int
     RUNTIME_SPECIFIC_FIELD_NUMBER: builtins.int
     RUNTIME_CONNECTION_FIELD_NUMBER: builtins.int
     PARAMETERS_FIELD_NUMBER: builtins.int
     PARAMETER_VALUES_FIELD_NUMBER: builtins.int
     PROGRESS_DEADLINE_FIELD_NUMBER: builtins.int
     RUNTIME_EXTENSION_FIELD_NUMBER: builtins.int
     KUBERNETES_CONFIG_FIELD_NUMBER: builtins.int
@@ -541,15 +588,18 @@
     @property
     def volumes(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.volumes.volumes_pb2.Volume]: ...
     @property
     def deploy_annotations(self) -> prodvana.proto.prodvana.workflow.integration_config_pb2.AnnotationsConfig: ...
     @property
     def base_template(self) -> prodvana.proto.prodvana.common_config.ref_pb2.ServiceTemplateRef: ...
     @property
-    def pre_push_tasks(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___TaskConfig]: ...
+    def pre_push_tasks(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___TaskConfig]:
+        """DEPRECATED: Replace with delivery_extensions once its implemented."""
+    @property
+    def delivery_extensions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___DeliveryExtensionConfig]: ...
     @property
     def runtime_specific(self) -> global___RuntimeSpecificConfig: ...
     runtime_connection: builtins.str
     """which runtime connection to use in each release channel.
     optional if only one runtime makes sense for the service config.
     """
     @property
@@ -584,28 +634,29 @@
         per_release_channel: collections.abc.Iterable[global___PerReleaseChannelConfig] | None = ...,
         capabilities: collections.abc.Iterable[global___CapabilityReference] | None = ...,
         delivery_config: prodvana.proto.prodvana.delivery.delivery_config_pb2.DeliveryConfig | None = ...,
         volumes: collections.abc.Iterable[prodvana.proto.prodvana.volumes.volumes_pb2.Volume] | None = ...,
         deploy_annotations: prodvana.proto.prodvana.workflow.integration_config_pb2.AnnotationsConfig | None = ...,
         base_template: prodvana.proto.prodvana.common_config.ref_pb2.ServiceTemplateRef | None = ...,
         pre_push_tasks: collections.abc.Iterable[global___TaskConfig] | None = ...,
+        delivery_extensions: collections.abc.Iterable[global___DeliveryExtensionConfig] | None = ...,
         runtime_specific: global___RuntimeSpecificConfig | None = ...,
         runtime_connection: builtins.str = ...,
         parameters: collections.abc.Iterable[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterDefinition] | None = ...,
         parameter_values: prodvana.proto.prodvana.service.parameters_pb2.ServiceParameterValues | None = ...,
         progress_deadline: google.protobuf.duration_pb2.Duration | None = ...,
         runtime_extension: global___RuntimeExtensionConfig | None = ...,
         kubernetes_config: prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig | None = ...,
         external_config: prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig | None = ...,
         helm: prodvana.proto.prodvana.common_config.helm_pb2.HelmConfig | None = ...,
         parameters_autogen: global___ServiceConfig.ParametersAutogen.ValueType = ...,
         auto_rollback: global___AutoRollbackConfig | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["auto_rollback", b"auto_rollback", "base_template", b"base_template", "config_oneof", b"config_oneof", "delivery_config", b"delivery_config", "deploy_annotations", b"deploy_annotations", "external_config", b"external_config", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "parameter_values", b"parameter_values", "progress_deadline", b"progress_deadline", "release_strategy", b"release_strategy", "replicas", b"replicas", "runtime_extension", b"runtime_extension", "runtime_specific", b"runtime_specific"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["application", b"application", "auto_rollback", b"auto_rollback", "base_template", b"base_template", "capabilities", b"capabilities", "config_oneof", b"config_oneof", "delivery_config", b"delivery_config", "deploy_annotations", b"deploy_annotations", "external_config", b"external_config", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "name", b"name", "parameter_values", b"parameter_values", "parameters", b"parameters", "parameters_autogen", b"parameters_autogen", "per_release_channel", b"per_release_channel", "pre_push_tasks", b"pre_push_tasks", "programs", b"programs", "progress_deadline", b"progress_deadline", "release_strategy", b"release_strategy", "replicas", b"replicas", "runtime_connection", b"runtime_connection", "runtime_extension", b"runtime_extension", "runtime_specific", b"runtime_specific", "volumes", b"volumes"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["application", b"application", "auto_rollback", b"auto_rollback", "base_template", b"base_template", "capabilities", b"capabilities", "config_oneof", b"config_oneof", "delivery_config", b"delivery_config", "delivery_extensions", b"delivery_extensions", "deploy_annotations", b"deploy_annotations", "external_config", b"external_config", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "name", b"name", "parameter_values", b"parameter_values", "parameters", b"parameters", "parameters_autogen", b"parameters_autogen", "per_release_channel", b"per_release_channel", "pre_push_tasks", b"pre_push_tasks", "programs", b"programs", "progress_deadline", b"progress_deadline", "release_strategy", b"release_strategy", "replicas", b"replicas", "runtime_connection", b"runtime_connection", "runtime_extension", b"runtime_extension", "runtime_specific", b"runtime_specific", "volumes", b"volumes"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["config_oneof", b"config_oneof"]) -> typing_extensions.Literal["runtime_extension", "kubernetes_config", "external_config", "helm"] | None: ...
 
 global___ServiceConfig = ServiceConfig
 
 class CompiledServiceInstanceConfig(google.protobuf.message.Message):
     """a compiled version of ServiceConfig specific to a service instance, with release-channel configs applied"""
 
@@ -641,14 +692,15 @@
     RUNTIME_EXECUTION_FIELD_NUMBER: builtins.int
     CAPABILITIES_FIELD_NUMBER: builtins.int
     DELIVERY_CONFIG_FIELD_NUMBER: builtins.int
     VOLUMES_FIELD_NUMBER: builtins.int
     DEPLOY_ANNOTATIONS_FIELD_NUMBER: builtins.int
     BASE_TEMPLATE_FIELD_NUMBER: builtins.int
     PRE_PUSH_TASKS_FIELD_NUMBER: builtins.int
+    DELIVERY_EXTENSIONS_FIELD_NUMBER: builtins.int
     RUNTIME_SPECIFIC_FIELD_NUMBER: builtins.int
     PARAMETERS_FIELD_NUMBER: builtins.int
     PARAMETER_VALUES_FIELD_NUMBER: builtins.int
     PROGRESS_DEADLINE_FIELD_NUMBER: builtins.int
     RUNTIME_EXTENSION_FIELD_NUMBER: builtins.int
     KUBERNETES_CONFIG_FIELD_NUMBER: builtins.int
     HELM_FIELD_NUMBER: builtins.int
@@ -678,15 +730,18 @@
     @property
     def volumes(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.volumes.volumes_pb2.Volume]: ...
     @property
     def deploy_annotations(self) -> prodvana.proto.prodvana.workflow.integration_config_pb2.AnnotationsConfig: ...
     @property
     def base_template(self) -> prodvana.proto.prodvana.common_config.ref_pb2.ServiceTemplateRef: ...
     @property
-    def pre_push_tasks(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___TaskConfig]: ...
+    def pre_push_tasks(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___TaskConfig]:
+        """DEPRECATED: Replace with delivery_extensions once its implemented."""
+    @property
+    def delivery_extensions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___DeliveryExtensionConfig]: ...
     @property
     def runtime_specific(self) -> global___RuntimeSpecificConfig: ...
     @property
     def parameters(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterDefinition]: ...
     @property
     def parameter_values(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterValue]: ...
     @property
@@ -719,25 +774,26 @@
         runtime_execution: prodvana.proto.prodvana.runtimes.runtimes_config_pb2.RuntimeExecutionConfig | None = ...,
         capabilities: collections.abc.Iterable[global___CompiledCapabilityConfig] | None = ...,
         delivery_config: prodvana.proto.prodvana.delivery.delivery_config_pb2.DeliveryConfig | None = ...,
         volumes: collections.abc.Iterable[prodvana.proto.prodvana.volumes.volumes_pb2.Volume] | None = ...,
         deploy_annotations: prodvana.proto.prodvana.workflow.integration_config_pb2.AnnotationsConfig | None = ...,
         base_template: prodvana.proto.prodvana.common_config.ref_pb2.ServiceTemplateRef | None = ...,
         pre_push_tasks: collections.abc.Iterable[global___TaskConfig] | None = ...,
+        delivery_extensions: collections.abc.Iterable[global___DeliveryExtensionConfig] | None = ...,
         runtime_specific: global___RuntimeSpecificConfig | None = ...,
         parameters: collections.abc.Iterable[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterDefinition] | None = ...,
         parameter_values: collections.abc.Iterable[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterValue] | None = ...,
         progress_deadline: google.protobuf.duration_pb2.Duration | None = ...,
         runtime_extension: global___RuntimeExtensionConfig | None = ...,
         kubernetes_config: prodvana.proto.prodvana.common_config.kubernetes_config_pb2.KubernetesConfig | None = ...,
         helm: prodvana.proto.prodvana.common_config.helm_pb2.HelmConfig | None = ...,
         env: collections.abc.Mapping[builtins.str, prodvana.proto.prodvana.common_config.env_pb2.EnvValue] | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["base_template", b"base_template", "cert", b"cert", "config_oneof", b"config_oneof", "delivery_config", b"delivery_config", "deploy_annotations", b"deploy_annotations", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "progress_deadline", b"progress_deadline", "release_strategy", b"release_strategy", "replicas", b"replicas", "runtime", b"runtime", "runtime_execution", b"runtime_execution", "runtime_extension", b"runtime_extension", "runtime_specific", b"runtime_specific"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["application", b"application", "base_template", b"base_template", "capabilities", b"capabilities", "cert", b"cert", "config_oneof", b"config_oneof", "custom_hostnames", b"custom_hostnames", "delivery_config", b"delivery_config", "deploy_annotations", b"deploy_annotations", "env", b"env", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "maturity", b"maturity", "parameter_values", b"parameter_values", "parameters", b"parameters", "pre_push_tasks", b"pre_push_tasks", "programs", b"programs", "progress_deadline", b"progress_deadline", "release_channel", b"release_channel", "release_strategy", b"release_strategy", "replicas", b"replicas", "runtime", b"runtime", "runtime_execution", b"runtime_execution", "runtime_extension", b"runtime_extension", "runtime_specific", b"runtime_specific", "service", b"service", "volumes", b"volumes"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["application", b"application", "base_template", b"base_template", "capabilities", b"capabilities", "cert", b"cert", "config_oneof", b"config_oneof", "custom_hostnames", b"custom_hostnames", "delivery_config", b"delivery_config", "delivery_extensions", b"delivery_extensions", "deploy_annotations", b"deploy_annotations", "env", b"env", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "maturity", b"maturity", "parameter_values", b"parameter_values", "parameters", b"parameters", "pre_push_tasks", b"pre_push_tasks", "programs", b"programs", "progress_deadline", b"progress_deadline", "release_channel", b"release_channel", "release_strategy", b"release_strategy", "replicas", b"replicas", "runtime", b"runtime", "runtime_execution", b"runtime_execution", "runtime_extension", b"runtime_extension", "runtime_specific", b"runtime_specific", "service", b"service", "volumes", b"volumes"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["config_oneof", b"config_oneof"]) -> typing_extensions.Literal["runtime_extension", "kubernetes_config", "helm"] | None: ...
 
 global___CompiledServiceInstanceConfig = CompiledServiceInstanceConfig
 
 class CompiledJobConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/service/service_manager_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/service/service_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/service/service_manager_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/service/service_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/service/service_manager_pb2_grpc.py` & `prodvana-0.1.7/prodvana/proto/prodvana/service/service_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/service/service_manager_pb2_grpc.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/service/service_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/service/user_metadata_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/service/user_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/service/user_metadata_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/service/user_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/settings/organization/users_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/settings/organization/users_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/settings/organization/users_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/settings/organization/users_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.py` & `prodvana-0.1.7/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/stat/efficiency_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/stat/efficiency_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/stat/efficiency_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/stat/efficiency_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/template/service_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/template/service_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/users/users_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/users/users_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/users/users_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/users/users_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/version/source_metadata_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/version/source_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/volumes/volumes_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/volumes/volumes_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/volumes/volumes_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/volumes/volumes_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/workflow/integration_config_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/workflow/integration_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/workflow/integration_config_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/workflow/integration_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/workflow/workflow_manager_pb2.py` & `prodvana-0.1.7/prodvana/proto/prodvana/workflow/workflow_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/workflow/workflow_manager_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/workflow/workflow_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.py` & `prodvana-0.1.7/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.pyi` & `prodvana-0.1.7/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/validate/validate_pb2.py` & `prodvana-0.1.7/prodvana/proto/validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/proto/validate/validate_pb2.pyi` & `prodvana-0.1.7/prodvana/proto/validate/validate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/utils/desired_states.py` & `prodvana-0.1.7/prodvana/utils/desired_states.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/utils/service_config.py` & `prodvana-0.1.7/prodvana/utils/service_config.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/prodvana/utils/tests/test_service_config.py` & `prodvana-0.1.7/prodvana/utils/tests/test_service_config.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.1.6/pyproject.toml` & `prodvana-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prodvana"
-version = "0.1.6"
+version = "0.1.7"
 description = "Prodvana's client libraries"
 readme = "README.md"
 authors = []
 homepage = "https://prodvana.io"
 documentation = "https://docs.prodvana.io"
 repository = "https://github.com/prodvana/prodvana-public"
 exclude = ["examples"]
```

### Comparing `prodvana-0.1.6/PKG-INFO` & `prodvana-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prodvana
-Version: 0.1.6
+Version: 0.1.7
 Summary: Prodvana's client libraries
 Home-page: https://prodvana.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: google-api-python-client (>=2.58.0,<3.0)
```

