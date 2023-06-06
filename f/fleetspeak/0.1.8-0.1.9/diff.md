# Comparing `tmp/fleetspeak-0.1.8.tar.gz` & `tmp/fleetspeak-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fleetspeak-0.1.8.tar", last modified: Tue Nov 24 12:06:31 2020, max compression
+gzip compressed data, was "fleetspeak-0.1.9.tar", last modified: Thu Apr  1 07:11:40 2021, max compression
```

## Comparing `fleetspeak-0.1.8.tar` & `fleetspeak-0.1.9.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)     6135 2020-11-24 11:59:07.000000 fleetspeak-0.1.8/setup.py
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/server_connector/
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/server_connector/testing/
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)     1809 2020-11-24 11:59:07.000000 fleetspeak-0.1.8/fleetspeak/server_connector/testing/loopback.py
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)    12622 2020-11-24 11:59:07.000000 fleetspeak-0.1.8/fleetspeak/server_connector/connector.py
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)     2479 2020-11-24 11:59:07.000000 fleetspeak-0.1.8/fleetspeak/server_connector/connector_test.py
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/client/
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/client/daemonservice/
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/client/daemonservice/proto/
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/client/daemonservice/proto/fleetspeak_daemonservice/
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)       83 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/client/daemonservice/proto/fleetspeak_daemonservice/messages_pb2_grpc.py
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)     3780 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/client/daemonservice/proto/fleetspeak_daemonservice/messages_pb2.py
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)     9728 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/client/daemonservice/proto/fleetspeak_daemonservice/config_pb2.py
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)       83 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/client/daemonservice/proto/fleetspeak_daemonservice/config_pb2_grpc.py
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/client/socketservice/
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/client/socketservice/proto/
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/client/socketservice/proto/fleetspeak_socketservice/
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)     3945 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/client/socketservice/proto/fleetspeak_socketservice/config_pb2.py
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)       83 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/client/socketservice/proto/fleetspeak_socketservice/config_pb2_grpc.py
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/client/generic/
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/client/generic/proto/
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/client/generic/proto/fleetspeak_client_generic/
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)     9095 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/client/generic/proto/fleetspeak_client_generic/config_pb2.py
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)       83 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/client/generic/proto/fleetspeak_client_generic/config_pb2_grpc.py
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/client/stdinservice/
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/client/stdinservice/proto/
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/client/stdinservice/proto/fleetspeak_stdinservice/
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)       83 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/client/stdinservice/proto/fleetspeak_stdinservice/messages_pb2_grpc.py
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)     6337 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/client/stdinservice/proto/fleetspeak_stdinservice/messages_pb2.py
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)     2425 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/client/stdinservice/proto/fleetspeak_stdinservice/config_pb2.py
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)       83 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/client/stdinservice/proto/fleetspeak_stdinservice/config_pb2_grpc.py
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/client/proto/
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/client/proto/fleetspeak_client/
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)       83 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/client/proto/fleetspeak_client/api_pb2_grpc.py
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)     4175 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/client/proto/fleetspeak_client/api_pb2.py
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)     5975 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/client/proto/fleetspeak_client/client_pb2.py
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)       83 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/client/proto/fleetspeak_client/client_pb2_grpc.py
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/client/channel/
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/client/channel/proto/
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/client/channel/proto/fleetspeak_channel/
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)     2802 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/client/channel/proto/fleetspeak_channel/channel_pb2.py
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)       83 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/client/channel/proto/fleetspeak_channel/channel_pb2_grpc.py
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/common/
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/common/proto/
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/common/proto/fleetspeak/
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)       83 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/common/proto/fleetspeak/system_pb2_grpc.py
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)       83 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/common/proto/fleetspeak/common_pb2_grpc.py
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)    19898 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/common/proto/fleetspeak/system_pb2.py
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)    30708 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/common/proto/fleetspeak/common_pb2.py
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/common/proto/fleetspeak_monitoring/
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)    15668 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/common/proto/fleetspeak_monitoring/resource_pb2.py
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)       83 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/common/proto/fleetspeak_monitoring/resource_pb2_grpc.py
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/inttesting/
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/inttesting/frr/
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/inttesting/frr/proto/
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/inttesting/frr/proto/fleetspeak_frr/
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)    24081 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/inttesting/frr/proto/fleetspeak_frr/frr_pb2.py
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)     5495 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/inttesting/frr/proto/fleetspeak_frr/frr_pb2_grpc.py
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/config/
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/config/proto/
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/config/proto/fleetspeak_config/
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)     7587 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/config/proto/fleetspeak_config/config_pb2.py
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)       83 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/config/proto/fleetspeak_config/config_pb2_grpc.py
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/server/
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/server/grpcservice/
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/server/grpcservice/proto/
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/server/grpcservice/proto/fleetspeak_grpcservice/
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)     4394 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/server/grpcservice/proto/fleetspeak_grpcservice/grpcservice_pb2.py
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)     1868 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/server/grpcservice/proto/fleetspeak_grpcservice/grpcservice_pb2_grpc.py
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/server/components/
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/server/components/proto/
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/server/components/proto/fleetspeak_components/
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)    12935 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/server/components/proto/fleetspeak_components/config_pb2.py
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)       83 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/server/components/proto/fleetspeak_components/config_pb2_grpc.py
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/server/proto/
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/server/proto/fleetspeak_server/
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)     9099 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/server/proto/fleetspeak_server/resource_pb2.py
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)       83 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/server/proto/fleetspeak_server/server_pb2_grpc.py
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)     3936 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/server/proto/fleetspeak_server/services_pb2.py
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)       83 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/server/proto/fleetspeak_server/resource_pb2_grpc.py
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)     5663 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/server/proto/fleetspeak_server/broadcasts_pb2.py
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)     3634 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/server/proto/fleetspeak_server/server_pb2.py
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)       83 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/server/proto/fleetspeak_server/broadcasts_pb2_grpc.py
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)    37948 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/server/proto/fleetspeak_server/admin_pb2.py
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)       83 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/server/proto/fleetspeak_server/services_pb2_grpc.py
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)    13004 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/server/proto/fleetspeak_server/admin_pb2_grpc.py
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/osquery/
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/osquery/proto/
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/osquery/proto/fleetspeak_osquery/
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)       83 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/osquery/proto/fleetspeak_osquery/osquery_pb2_grpc.py
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)    17736 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/src/osquery/proto/fleetspeak_osquery/osquery_pb2.py
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/client_connector/
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak/client_connector/testing/
--rwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)     1195 2020-11-24 11:59:07.000000 fleetspeak-0.1.8/fleetspeak/client_connector/testing/testclient_launcher.py
--rwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)     2516 2020-11-24 11:59:07.000000 fleetspeak-0.1.8/fleetspeak/client_connector/testing/testclient.py
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)     7405 2020-11-24 11:59:07.000000 fleetspeak-0.1.8/fleetspeak/client_connector/connector.py
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)       38 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/setup.cfg
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)        6 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/VERSION
-drwxrwxr-x   0 mbushkov  (1001) mbushkov  (1002)        0 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak.egg-info/
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)       30 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak.egg-info/requires.txt
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)        1 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak.egg-info/dependency_links.txt
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)       11 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak.egg-info/top_level.txt
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)     3550 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak.egg-info/SOURCES.txt
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)      823 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/fleetspeak.egg-info/PKG-INFO
--rw-rw-r--   0 mbushkov  (1001) mbushkov  (1002)      823 2020-11-24 12:06:31.000000 fleetspeak-0.1.8/PKG-INFO
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.931455 fleetspeak-0.1.9/
+-rw-r-----   0 molnar   (145895) primarygroup (89939)      823 2021-04-01 07:11:40.931455 fleetspeak-0.1.9/PKG-INFO
+-rw-r-----   0 molnar   (145895) primarygroup (89939)        6 2021-04-01 07:11:40.931455 fleetspeak-0.1.9/VERSION
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.927455 fleetspeak-0.1.9/fleetspeak/
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.927455 fleetspeak-0.1.9/fleetspeak/client_connector/
+-rw-r-----   0 molnar   (145895) primarygroup (89939)     7405 2021-04-01 07:04:04.000000 fleetspeak-0.1.9/fleetspeak/client_connector/connector.py
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.927455 fleetspeak-0.1.9/fleetspeak/client_connector/testing/
+-rwxr-x---   0 molnar   (145895) primarygroup (89939)     2516 2021-04-01 07:04:04.000000 fleetspeak-0.1.9/fleetspeak/client_connector/testing/testclient.py
+-rwxr-x---   0 molnar   (145895) primarygroup (89939)     1195 2021-04-01 07:04:04.000000 fleetspeak-0.1.9/fleetspeak/client_connector/testing/testclient_launcher.py
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.927455 fleetspeak-0.1.9/fleetspeak/server_connector/
+-rw-r-----   0 molnar   (145895) primarygroup (89939)    12622 2021-04-01 07:04:04.000000 fleetspeak-0.1.9/fleetspeak/server_connector/connector.py
+-rw-r-----   0 molnar   (145895) primarygroup (89939)     2479 2021-04-01 07:04:04.000000 fleetspeak-0.1.9/fleetspeak/server_connector/connector_test.py
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.927455 fleetspeak-0.1.9/fleetspeak/server_connector/testing/
+-rw-r-----   0 molnar   (145895) primarygroup (89939)     1809 2021-04-01 07:04:04.000000 fleetspeak-0.1.9/fleetspeak/server_connector/testing/loopback.py
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.927455 fleetspeak-0.1.9/fleetspeak/src/
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.927455 fleetspeak-0.1.9/fleetspeak/src/client/
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.927455 fleetspeak-0.1.9/fleetspeak/src/client/channel/
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.927455 fleetspeak-0.1.9/fleetspeak/src/client/channel/proto/
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.927455 fleetspeak-0.1.9/fleetspeak/src/client/channel/proto/fleetspeak_channel/
+-rw-r-----   0 molnar   (145895) primarygroup (89939)     2802 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/client/channel/proto/fleetspeak_channel/channel_pb2.py
+-rw-r-----   0 molnar   (145895) primarygroup (89939)       83 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/client/channel/proto/fleetspeak_channel/channel_pb2_grpc.py
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.927455 fleetspeak-0.1.9/fleetspeak/src/client/daemonservice/
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.927455 fleetspeak-0.1.9/fleetspeak/src/client/daemonservice/proto/
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.927455 fleetspeak-0.1.9/fleetspeak/src/client/daemonservice/proto/fleetspeak_daemonservice/
+-rw-r-----   0 molnar   (145895) primarygroup (89939)     9728 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/client/daemonservice/proto/fleetspeak_daemonservice/config_pb2.py
+-rw-r-----   0 molnar   (145895) primarygroup (89939)       83 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/client/daemonservice/proto/fleetspeak_daemonservice/config_pb2_grpc.py
+-rw-r-----   0 molnar   (145895) primarygroup (89939)     3780 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/client/daemonservice/proto/fleetspeak_daemonservice/messages_pb2.py
+-rw-r-----   0 molnar   (145895) primarygroup (89939)       83 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/client/daemonservice/proto/fleetspeak_daemonservice/messages_pb2_grpc.py
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.927455 fleetspeak-0.1.9/fleetspeak/src/client/generic/
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.927455 fleetspeak-0.1.9/fleetspeak/src/client/generic/proto/
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.927455 fleetspeak-0.1.9/fleetspeak/src/client/generic/proto/fleetspeak_client_generic/
+-rw-r-----   0 molnar   (145895) primarygroup (89939)     9095 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/client/generic/proto/fleetspeak_client_generic/config_pb2.py
+-rw-r-----   0 molnar   (145895) primarygroup (89939)       83 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/client/generic/proto/fleetspeak_client_generic/config_pb2_grpc.py
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.927455 fleetspeak-0.1.9/fleetspeak/src/client/proto/
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.931455 fleetspeak-0.1.9/fleetspeak/src/client/proto/fleetspeak_client/
+-rw-r-----   0 molnar   (145895) primarygroup (89939)     4175 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/client/proto/fleetspeak_client/api_pb2.py
+-rw-r-----   0 molnar   (145895) primarygroup (89939)       83 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/client/proto/fleetspeak_client/api_pb2_grpc.py
+-rw-r-----   0 molnar   (145895) primarygroup (89939)     5975 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/client/proto/fleetspeak_client/client_pb2.py
+-rw-r-----   0 molnar   (145895) primarygroup (89939)       83 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/client/proto/fleetspeak_client/client_pb2_grpc.py
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.927455 fleetspeak-0.1.9/fleetspeak/src/client/socketservice/
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.927455 fleetspeak-0.1.9/fleetspeak/src/client/socketservice/proto/
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.931455 fleetspeak-0.1.9/fleetspeak/src/client/socketservice/proto/fleetspeak_socketservice/
+-rw-r-----   0 molnar   (145895) primarygroup (89939)     3945 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/client/socketservice/proto/fleetspeak_socketservice/config_pb2.py
+-rw-r-----   0 molnar   (145895) primarygroup (89939)       83 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/client/socketservice/proto/fleetspeak_socketservice/config_pb2_grpc.py
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.927455 fleetspeak-0.1.9/fleetspeak/src/client/stdinservice/
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.927455 fleetspeak-0.1.9/fleetspeak/src/client/stdinservice/proto/
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.931455 fleetspeak-0.1.9/fleetspeak/src/client/stdinservice/proto/fleetspeak_stdinservice/
+-rw-r-----   0 molnar   (145895) primarygroup (89939)     2425 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/client/stdinservice/proto/fleetspeak_stdinservice/config_pb2.py
+-rw-r-----   0 molnar   (145895) primarygroup (89939)       83 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/client/stdinservice/proto/fleetspeak_stdinservice/config_pb2_grpc.py
+-rw-r-----   0 molnar   (145895) primarygroup (89939)     6337 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/client/stdinservice/proto/fleetspeak_stdinservice/messages_pb2.py
+-rw-r-----   0 molnar   (145895) primarygroup (89939)       83 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/client/stdinservice/proto/fleetspeak_stdinservice/messages_pb2_grpc.py
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.927455 fleetspeak-0.1.9/fleetspeak/src/common/
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.927455 fleetspeak-0.1.9/fleetspeak/src/common/proto/
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.931455 fleetspeak-0.1.9/fleetspeak/src/common/proto/fleetspeak/
+-rw-r-----   0 molnar   (145895) primarygroup (89939)    30708 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/common/proto/fleetspeak/common_pb2.py
+-rw-r-----   0 molnar   (145895) primarygroup (89939)       83 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/common/proto/fleetspeak/common_pb2_grpc.py
+-rw-r-----   0 molnar   (145895) primarygroup (89939)    19898 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/common/proto/fleetspeak/system_pb2.py
+-rw-r-----   0 molnar   (145895) primarygroup (89939)       83 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/common/proto/fleetspeak/system_pb2_grpc.py
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.931455 fleetspeak-0.1.9/fleetspeak/src/common/proto/fleetspeak_monitoring/
+-rw-r-----   0 molnar   (145895) primarygroup (89939)    15668 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/common/proto/fleetspeak_monitoring/resource_pb2.py
+-rw-r-----   0 molnar   (145895) primarygroup (89939)       83 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/common/proto/fleetspeak_monitoring/resource_pb2_grpc.py
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.927455 fleetspeak-0.1.9/fleetspeak/src/config/
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.927455 fleetspeak-0.1.9/fleetspeak/src/config/proto/
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.931455 fleetspeak-0.1.9/fleetspeak/src/config/proto/fleetspeak_config/
+-rw-r-----   0 molnar   (145895) primarygroup (89939)     7587 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/config/proto/fleetspeak_config/config_pb2.py
+-rw-r-----   0 molnar   (145895) primarygroup (89939)       83 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/config/proto/fleetspeak_config/config_pb2_grpc.py
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.927455 fleetspeak-0.1.9/fleetspeak/src/inttesting/
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.927455 fleetspeak-0.1.9/fleetspeak/src/inttesting/frr/
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.927455 fleetspeak-0.1.9/fleetspeak/src/inttesting/frr/proto/
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.931455 fleetspeak-0.1.9/fleetspeak/src/inttesting/frr/proto/fleetspeak_frr/
+-rw-r-----   0 molnar   (145895) primarygroup (89939)    24081 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/inttesting/frr/proto/fleetspeak_frr/frr_pb2.py
+-rw-r-----   0 molnar   (145895) primarygroup (89939)     5495 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/inttesting/frr/proto/fleetspeak_frr/frr_pb2_grpc.py
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.927455 fleetspeak-0.1.9/fleetspeak/src/osquery/
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.927455 fleetspeak-0.1.9/fleetspeak/src/osquery/proto/
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.931455 fleetspeak-0.1.9/fleetspeak/src/osquery/proto/fleetspeak_osquery/
+-rw-r-----   0 molnar   (145895) primarygroup (89939)    17736 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/osquery/proto/fleetspeak_osquery/osquery_pb2.py
+-rw-r-----   0 molnar   (145895) primarygroup (89939)       83 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/osquery/proto/fleetspeak_osquery/osquery_pb2_grpc.py
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.927455 fleetspeak-0.1.9/fleetspeak/src/server/
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.927455 fleetspeak-0.1.9/fleetspeak/src/server/components/
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.927455 fleetspeak-0.1.9/fleetspeak/src/server/components/proto/
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.931455 fleetspeak-0.1.9/fleetspeak/src/server/components/proto/fleetspeak_components/
+-rw-r-----   0 molnar   (145895) primarygroup (89939)    13410 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/server/components/proto/fleetspeak_components/config_pb2.py
+-rw-r-----   0 molnar   (145895) primarygroup (89939)       83 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/server/components/proto/fleetspeak_components/config_pb2_grpc.py
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.927455 fleetspeak-0.1.9/fleetspeak/src/server/grpcservice/
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.927455 fleetspeak-0.1.9/fleetspeak/src/server/grpcservice/proto/
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.931455 fleetspeak-0.1.9/fleetspeak/src/server/grpcservice/proto/fleetspeak_grpcservice/
+-rw-r-----   0 molnar   (145895) primarygroup (89939)     4394 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/server/grpcservice/proto/fleetspeak_grpcservice/grpcservice_pb2.py
+-rw-r-----   0 molnar   (145895) primarygroup (89939)     1868 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/server/grpcservice/proto/fleetspeak_grpcservice/grpcservice_pb2_grpc.py
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.927455 fleetspeak-0.1.9/fleetspeak/src/server/proto/
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.931455 fleetspeak-0.1.9/fleetspeak/src/server/proto/fleetspeak_server/
+-rw-r-----   0 molnar   (145895) primarygroup (89939)    45892 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/server/proto/fleetspeak_server/admin_pb2.py
+-rw-r-----   0 molnar   (145895) primarygroup (89939)    15256 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/server/proto/fleetspeak_server/admin_pb2_grpc.py
+-rw-r-----   0 molnar   (145895) primarygroup (89939)     5663 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/server/proto/fleetspeak_server/broadcasts_pb2.py
+-rw-r-----   0 molnar   (145895) primarygroup (89939)       83 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/server/proto/fleetspeak_server/broadcasts_pb2_grpc.py
+-rw-r-----   0 molnar   (145895) primarygroup (89939)     9099 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/server/proto/fleetspeak_server/resource_pb2.py
+-rw-r-----   0 molnar   (145895) primarygroup (89939)       83 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/server/proto/fleetspeak_server/resource_pb2_grpc.py
+-rw-r-----   0 molnar   (145895) primarygroup (89939)     3634 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/server/proto/fleetspeak_server/server_pb2.py
+-rw-r-----   0 molnar   (145895) primarygroup (89939)       83 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/server/proto/fleetspeak_server/server_pb2_grpc.py
+-rw-r-----   0 molnar   (145895) primarygroup (89939)     3936 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/server/proto/fleetspeak_server/services_pb2.py
+-rw-r-----   0 molnar   (145895) primarygroup (89939)       83 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak/src/server/proto/fleetspeak_server/services_pb2_grpc.py
+drwxr-x---   0 molnar   (145895) primarygroup (89939)        0 2021-04-01 07:11:40.927455 fleetspeak-0.1.9/fleetspeak.egg-info/
+-rw-r-----   0 molnar   (145895) primarygroup (89939)      823 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak.egg-info/PKG-INFO
+-rw-r-----   0 molnar   (145895) primarygroup (89939)     3550 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak.egg-info/SOURCES.txt
+-rw-r-----   0 molnar   (145895) primarygroup (89939)        1 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak.egg-info/dependency_links.txt
+-rw-r-----   0 molnar   (145895) primarygroup (89939)       30 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak.egg-info/requires.txt
+-rw-r-----   0 molnar   (145895) primarygroup (89939)       11 2021-04-01 07:11:40.000000 fleetspeak-0.1.9/fleetspeak.egg-info/top_level.txt
+-rw-r-----   0 molnar   (145895) primarygroup (89939)       38 2021-04-01 07:11:40.931455 fleetspeak-0.1.9/setup.cfg
+-rw-r-----   0 molnar   (145895) primarygroup (89939)     6135 2021-04-01 07:04:04.000000 fleetspeak-0.1.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `fleetspeak-0.1.8/setup.py` & `fleetspeak-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `fleetspeak-0.1.8/fleetspeak/server_connector/testing/loopback.py` & `fleetspeak-0.1.9/fleetspeak/server_connector/testing/loopback.py`

 * *Files identical despite different names*

### Comparing `fleetspeak-0.1.8/fleetspeak/server_connector/connector.py` & `fleetspeak-0.1.9/fleetspeak/server_connector/connector.py`

 * *Files identical despite different names*

### Comparing `fleetspeak-0.1.8/fleetspeak/server_connector/connector_test.py` & `fleetspeak-0.1.9/fleetspeak/server_connector/connector_test.py`

 * *Files identical despite different names*

### Comparing `fleetspeak-0.1.8/fleetspeak/src/client/daemonservice/proto/fleetspeak_daemonservice/messages_pb2.py` & `fleetspeak-0.1.9/fleetspeak/src/client/daemonservice/proto/fleetspeak_daemonservice/messages_pb2.py`

 * *Files identical despite different names*

### Comparing `fleetspeak-0.1.8/fleetspeak/src/client/daemonservice/proto/fleetspeak_daemonservice/config_pb2.py` & `fleetspeak-0.1.9/fleetspeak/src/client/daemonservice/proto/fleetspeak_daemonservice/config_pb2.py`

 * *Files identical despite different names*

### Comparing `fleetspeak-0.1.8/fleetspeak/src/client/socketservice/proto/fleetspeak_socketservice/config_pb2.py` & `fleetspeak-0.1.9/fleetspeak/src/client/socketservice/proto/fleetspeak_socketservice/config_pb2.py`

 * *Files identical despite different names*

### Comparing `fleetspeak-0.1.8/fleetspeak/src/client/generic/proto/fleetspeak_client_generic/config_pb2.py` & `fleetspeak-0.1.9/fleetspeak/src/client/generic/proto/fleetspeak_client_generic/config_pb2.py`

 * *Files identical despite different names*

### Comparing `fleetspeak-0.1.8/fleetspeak/src/client/stdinservice/proto/fleetspeak_stdinservice/messages_pb2.py` & `fleetspeak-0.1.9/fleetspeak/src/client/stdinservice/proto/fleetspeak_stdinservice/messages_pb2.py`

 * *Files identical despite different names*

### Comparing `fleetspeak-0.1.8/fleetspeak/src/client/stdinservice/proto/fleetspeak_stdinservice/config_pb2.py` & `fleetspeak-0.1.9/fleetspeak/src/client/stdinservice/proto/fleetspeak_stdinservice/config_pb2.py`

 * *Files identical despite different names*

### Comparing `fleetspeak-0.1.8/fleetspeak/src/client/proto/fleetspeak_client/api_pb2.py` & `fleetspeak-0.1.9/fleetspeak/src/client/proto/fleetspeak_client/api_pb2.py`

 * *Files identical despite different names*

### Comparing `fleetspeak-0.1.8/fleetspeak/src/client/proto/fleetspeak_client/client_pb2.py` & `fleetspeak-0.1.9/fleetspeak/src/client/proto/fleetspeak_client/client_pb2.py`

 * *Files identical despite different names*

### Comparing `fleetspeak-0.1.8/fleetspeak/src/client/channel/proto/fleetspeak_channel/channel_pb2.py` & `fleetspeak-0.1.9/fleetspeak/src/client/channel/proto/fleetspeak_channel/channel_pb2.py`

 * *Files identical despite different names*

### Comparing `fleetspeak-0.1.8/fleetspeak/src/common/proto/fleetspeak/system_pb2.py` & `fleetspeak-0.1.9/fleetspeak/src/common/proto/fleetspeak/system_pb2.py`

 * *Files identical despite different names*

### Comparing `fleetspeak-0.1.8/fleetspeak/src/common/proto/fleetspeak/common_pb2.py` & `fleetspeak-0.1.9/fleetspeak/src/common/proto/fleetspeak/common_pb2.py`

 * *Files identical despite different names*

### Comparing `fleetspeak-0.1.8/fleetspeak/src/common/proto/fleetspeak_monitoring/resource_pb2.py` & `fleetspeak-0.1.9/fleetspeak/src/common/proto/fleetspeak_monitoring/resource_pb2.py`

 * *Files identical despite different names*

### Comparing `fleetspeak-0.1.8/fleetspeak/src/inttesting/frr/proto/fleetspeak_frr/frr_pb2.py` & `fleetspeak-0.1.9/fleetspeak/src/inttesting/frr/proto/fleetspeak_frr/frr_pb2.py`

 * *Files identical despite different names*

### Comparing `fleetspeak-0.1.8/fleetspeak/src/inttesting/frr/proto/fleetspeak_frr/frr_pb2_grpc.py` & `fleetspeak-0.1.9/fleetspeak/src/inttesting/frr/proto/fleetspeak_frr/frr_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fleetspeak-0.1.8/fleetspeak/src/config/proto/fleetspeak_config/config_pb2.py` & `fleetspeak-0.1.9/fleetspeak/src/config/proto/fleetspeak_config/config_pb2.py`

 * *Files identical despite different names*

### Comparing `fleetspeak-0.1.8/fleetspeak/src/server/grpcservice/proto/fleetspeak_grpcservice/grpcservice_pb2.py` & `fleetspeak-0.1.9/fleetspeak/src/server/grpcservice/proto/fleetspeak_grpcservice/grpcservice_pb2.py`

 * *Files identical despite different names*

### Comparing `fleetspeak-0.1.8/fleetspeak/src/server/grpcservice/proto/fleetspeak_grpcservice/grpcservice_pb2_grpc.py` & `fleetspeak-0.1.9/fleetspeak/src/server/grpcservice/proto/fleetspeak_grpcservice/grpcservice_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fleetspeak-0.1.8/fleetspeak/src/server/components/proto/fleetspeak_components/config_pb2.py` & `fleetspeak-0.1.9/fleetspeak/src/server/components/proto/fleetspeak_components/config_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='fleetspeak/src/server/components/proto/fleetspeak_components/config.proto',
   package='fleetspeak.components',
   syntax='proto3',
   serialized_options=_b('ZYgithub.com/google/fleetspeak/fleetspeak/src/server/components/proto/fleetspeak_components'),
-  serialized_pb=_b('\nIfleetspeak/src/server/components/proto/fleetspeak_components/config.proto\x12\x15\x66leetspeak.components\"\x97\x03\n\x06\x43onfig\x12\x1e\n\x16mysql_data_source_name\x18\x01 \x01(\t\x12\x38\n\x0chttps_config\x18\x02 \x01(\x0b\x32\".fleetspeak.components.HttpsConfig\x12\x38\n\x0c\x61\x64min_config\x18\x07 \x01(\x0b\x32\".fleetspeak.components.AdminConfig\x12\x38\n\x0cstats_config\x18\x08 \x01(\x0b\x32\".fleetspeak.components.StatsConfig\x12\x45\n\x13health_check_config\x18\t \x01(\x0b\x32(.fleetspeak.components.HealthCheckConfig\x12\x16\n\x0eproxy_protocol\x18\x03 \x01(\x08\x12\x16\n\x0erequired_label\x18\x04 \x01(\t\x12#\n\x1bnotification_listen_address\x18\x05 \x01(\t\x12#\n\x1bnotification_public_address\x18\x06 \x01(\t\"c\n\x0bHttpsConfig\x12\x16\n\x0elisten_address\x18\x01 \x01(\t\x12\x14\n\x0c\x63\x65rtificates\x18\x02 \x01(\t\x12\x0b\n\x03key\x18\x03 \x01(\t\x12\x19\n\x11\x64isable_streaming\x18\x04 \x01(\x08\"%\n\x0b\x41\x64minConfig\x12\x16\n\x0elisten_address\x18\x01 \x01(\t\"\x1e\n\x0bStatsConfig\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x01(\t\"+\n\x11HealthCheckConfig\x12\x16\n\x0elisten_address\x18\x01 \x01(\tB[ZYgithub.com/google/fleetspeak/fleetspeak/src/server/components/proto/fleetspeak_componentsb\x06proto3')
+  serialized_pb=_b('\nIfleetspeak/src/server/components/proto/fleetspeak_components/config.proto\x12\x15\x66leetspeak.components\"\xbf\x03\n\x06\x43onfig\x12\x1e\n\x16mysql_data_source_name\x18\x01 \x01(\t\x12\x38\n\x0chttps_config\x18\x02 \x01(\x0b\x32\".fleetspeak.components.HttpsConfig\x12\x38\n\x0c\x61\x64min_config\x18\x07 \x01(\x0b\x32\".fleetspeak.components.AdminConfig\x12\x38\n\x0cstats_config\x18\x08 \x01(\x0b\x32\".fleetspeak.components.StatsConfig\x12\x45\n\x13health_check_config\x18\t \x01(\x0b\x32(.fleetspeak.components.HealthCheckConfig\x12\x16\n\x0eproxy_protocol\x18\x03 \x01(\x08\x12\x16\n\x0erequired_label\x18\x04 \x01(\t\x12#\n\x1bnotification_listen_address\x18\x05 \x01(\t\x12#\n\x1bnotification_public_address\x18\x06 \x01(\t\x12&\n\x1enotification_use_http_notifier\x18\n \x01(\x08\"c\n\x0bHttpsConfig\x12\x16\n\x0elisten_address\x18\x01 \x01(\t\x12\x14\n\x0c\x63\x65rtificates\x18\x02 \x01(\t\x12\x0b\n\x03key\x18\x03 \x01(\t\x12\x19\n\x11\x64isable_streaming\x18\x04 \x01(\x08\"%\n\x0b\x41\x64minConfig\x12\x16\n\x0elisten_address\x18\x01 \x01(\t\"\x1e\n\x0bStatsConfig\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x01(\t\"+\n\x11HealthCheckConfig\x12\x16\n\x0elisten_address\x18\x01 \x01(\tB[ZYgithub.com/google/fleetspeak/fleetspeak/src/server/components/proto/fleetspeak_componentsb\x06proto3')
 )
 
 
 
 
 _CONFIG = _descriptor.Descriptor(
   name='Config',
@@ -92,28 +92,35 @@
     _descriptor.FieldDescriptor(
       name='notification_public_address', full_name='fleetspeak.components.Config.notification_public_address', index=8,
       number=6, type=9, cpp_type=9, label=1,
       has_default_value=False, default_value=_b("").decode('utf-8'),
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='notification_use_http_notifier', full_name='fleetspeak.components.Config.notification_use_http_notifier', index=9,
+      number=10, type=8, cpp_type=7, label=1,
+      has_default_value=False, default_value=False,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=101,
-  serialized_end=508,
+  serialized_end=548,
 )
 
 
 _HTTPSCONFIG = _descriptor.Descriptor(
   name='HttpsConfig',
   full_name='fleetspeak.components.HttpsConfig',
   filename=None,
@@ -156,16 +163,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=510,
-  serialized_end=609,
+  serialized_start=550,
+  serialized_end=649,
 )
 
 
 _ADMINCONFIG = _descriptor.Descriptor(
   name='AdminConfig',
   full_name='fleetspeak.components.AdminConfig',
   filename=None,
@@ -187,16 +194,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=611,
-  serialized_end=648,
+  serialized_start=651,
+  serialized_end=688,
 )
 
 
 _STATSCONFIG = _descriptor.Descriptor(
   name='StatsConfig',
   full_name='fleetspeak.components.StatsConfig',
   filename=None,
@@ -218,16 +225,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=650,
-  serialized_end=680,
+  serialized_start=690,
+  serialized_end=720,
 )
 
 
 _HEALTHCHECKCONFIG = _descriptor.Descriptor(
   name='HealthCheckConfig',
   full_name='fleetspeak.components.HealthCheckConfig',
   filename=None,
@@ -249,16 +256,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=682,
-  serialized_end=725,
+  serialized_start=722,
+  serialized_end=765,
 )
 
 _CONFIG.fields_by_name['https_config'].message_type = _HTTPSCONFIG
 _CONFIG.fields_by_name['admin_config'].message_type = _ADMINCONFIG
 _CONFIG.fields_by_name['stats_config'].message_type = _STATSCONFIG
 _CONFIG.fields_by_name['health_check_config'].message_type = _HEALTHCHECKCONFIG
 DESCRIPTOR.message_types_by_name['Config'] = _CONFIG
```

### Comparing `fleetspeak-0.1.8/fleetspeak/src/server/proto/fleetspeak_server/resource_pb2.py` & `fleetspeak-0.1.9/fleetspeak/src/server/proto/fleetspeak_server/resource_pb2.py`

 * *Files identical despite different names*

### Comparing `fleetspeak-0.1.8/fleetspeak/src/server/proto/fleetspeak_server/services_pb2.py` & `fleetspeak-0.1.9/fleetspeak/src/server/proto/fleetspeak_server/services_pb2.py`

 * *Files identical despite different names*

### Comparing `fleetspeak-0.1.8/fleetspeak/src/server/proto/fleetspeak_server/broadcasts_pb2.py` & `fleetspeak-0.1.9/fleetspeak/src/server/proto/fleetspeak_server/broadcasts_pb2.py`

 * *Files identical despite different names*

### Comparing `fleetspeak-0.1.8/fleetspeak/src/server/proto/fleetspeak_server/server_pb2.py` & `fleetspeak-0.1.9/fleetspeak/src/server/proto/fleetspeak_server/server_pb2.py`

 * *Files identical despite different names*

### Comparing `fleetspeak-0.1.8/fleetspeak/src/server/proto/fleetspeak_server/admin_pb2.py` & `fleetspeak-0.1.9/fleetspeak/src/server/proto/fleetspeak_server/admin_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='fleetspeak/src/server/proto/fleetspeak_server/admin.proto',
   package='fleetspeak.server',
   syntax='proto3',
   serialized_options=_b('ZJgithub.com/google/fleetspeak/fleetspeak/src/server/proto/fleetspeak_server'),
-  serialized_pb=_b('\n9fleetspeak/src/server/proto/fleetspeak_server/admin.proto\x12\x11\x66leetspeak.server\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x33\x66leetspeak/src/common/proto/fleetspeak/common.proto\x1a>fleetspeak/src/server/proto/fleetspeak_server/broadcasts.proto\x1a<fleetspeak/src/server/proto/fleetspeak_server/resource.proto\"X\n\x16\x43reateBroadcastRequest\x12/\n\tbroadcast\x18\x01 \x01(\x0b\x32\x1c.fleetspeak.server.Broadcast\x12\r\n\x05limit\x18\x02 \x01(\x04\"3\n\x1bListActiveBroadcastsRequest\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\"P\n\x1cListActiveBroadcastsResponse\x12\x30\n\nbroadcasts\x18\x01 \x03(\x0b\x32\x1c.fleetspeak.server.Broadcast\"(\n\x12ListClientsRequest\x12\x12\n\nclient_ids\x18\x01 \x03(\x0c\"A\n\x13ListClientsResponse\x12*\n\x07\x63lients\x18\x01 \x03(\x0b\x32\x19.fleetspeak.server.Client\"\xfb\x01\n\x06\x43lient\x12\x11\n\tclient_id\x18\x01 \x01(\x0c\x12!\n\x06labels\x18\x02 \x03(\x0b\x32\x11.fleetspeak.Label\x12\x35\n\x11last_contact_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1c\n\x14last_contact_address\x18\x04 \x01(\t\x12!\n\x19last_contact_streaming_to\x18\x07 \x01(\t\x12.\n\nlast_clock\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0b\x62lacklisted\x18\x06 \x01(\x08\"-\n\x17GetMessageStatusRequest\x12\x12\n\nmessage_id\x18\x01 \x01(\x0c\"2\n\x1c\x44\x65letePendingMessagesRequest\x12\x12\n\nclient_ids\x18\x01 \x03(\x0c\"x\n\x18GetMessageStatusResponse\x12\x31\n\rcreation_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12)\n\x06result\x18\x02 \x01(\x0b\x32\x19.fleetspeak.MessageResult\"I\n\x10StoreFileRequest\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x11\n\tfile_name\x18\x02 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x0c\".\n\x19ListClientContactsRequest\x12\x11\n\tclient_id\x18\x01 \x01(\x0c\"P\n\x1aListClientContactsResponse\x12\x32\n\x08\x63ontacts\x18\x01 \x03(\x0b\x32 .fleetspeak.server.ClientContact\"\x84\x01\n\rClientContact\x12\x12\n\nsent_nonce\x18\x01 \x01(\x06\x12\x16\n\x0ereceived_nonce\x18\x02 \x01(\x06\x12\x18\n\x10observed_address\x18\x03 \x01(\t\x12-\n\ttimestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"+\n\x16\x42lacklistClientRequest\x12\x11\n\tclient_id\x18\x01 \x01(\x0c\"\xa3\x01\n&FetchClientResourceUsageRecordsRequest\x12\x11\n\tclient_id\x18\x01 \x01(\x0c\x12\x33\n\x0fstart_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rend_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"h\n\'FetchClientResourceUsageRecordsResponse\x12=\n\x07records\x18\x01 \x03(\x0b\x32,.fleetspeak.server.ClientResourceUsageRecord2\xd0\x08\n\x05\x41\x64min\x12X\n\x0f\x43reateBroadcast\x12).fleetspeak.server.CreateBroadcastRequest\x1a\x18.fleetspeak.EmptyMessage\"\x00\x12y\n\x14ListActiveBroadcasts\x12..fleetspeak.server.ListActiveBroadcastsRequest\x1a/.fleetspeak.server.ListActiveBroadcastsResponse\"\x00\x12^\n\x0bListClients\x12%.fleetspeak.server.ListClientsRequest\x1a&.fleetspeak.server.ListClientsResponse\"\x00\x12s\n\x12ListClientContacts\x12,.fleetspeak.server.ListClientContactsRequest\x1a-.fleetspeak.server.ListClientContactsResponse\"\x00\x12m\n\x10GetMessageStatus\x12*.fleetspeak.server.GetMessageStatusRequest\x1a+.fleetspeak.server.GetMessageStatusResponse\"\x00\x12@\n\rInsertMessage\x12\x13.fleetspeak.Message\x1a\x18.fleetspeak.EmptyMessage\"\x00\x12\x64\n\x15\x44\x65letePendingMessages\x12/.fleetspeak.server.DeletePendingMessagesRequest\x1a\x18.fleetspeak.EmptyMessage\"\x00\x12L\n\tStoreFile\x12#.fleetspeak.server.StoreFileRequest\x1a\x18.fleetspeak.EmptyMessage\"\x00\x12\x41\n\tKeepAlive\x12\x18.fleetspeak.EmptyMessage\x1a\x18.fleetspeak.EmptyMessage\"\x00\x12X\n\x0f\x42lacklistClient\x12).fleetspeak.server.BlacklistClientRequest\x1a\x18.fleetspeak.EmptyMessage\"\x00\x12\x9a\x01\n\x1f\x46\x65tchClientResourceUsageRecords\x12\x39.fleetspeak.server.FetchClientResourceUsageRecordsRequest\x1a:.fleetspeak.server.FetchClientResourceUsageRecordsResponse\"\x00\x42LZJgithub.com/google/fleetspeak/fleetspeak/src/server/proto/fleetspeak_serverb\x06proto3')
+  serialized_pb=_b('\n9fleetspeak/src/server/proto/fleetspeak_server/admin.proto\x12\x11\x66leetspeak.server\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x33\x66leetspeak/src/common/proto/fleetspeak/common.proto\x1a>fleetspeak/src/server/proto/fleetspeak_server/broadcasts.proto\x1a<fleetspeak/src/server/proto/fleetspeak_server/resource.proto\"X\n\x16\x43reateBroadcastRequest\x12/\n\tbroadcast\x18\x01 \x01(\x0b\x32\x1c.fleetspeak.server.Broadcast\x12\r\n\x05limit\x18\x02 \x01(\x04\"3\n\x1bListActiveBroadcastsRequest\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\"P\n\x1cListActiveBroadcastsResponse\x12\x30\n\nbroadcasts\x18\x01 \x03(\x0b\x32\x1c.fleetspeak.server.Broadcast\"(\n\x12ListClientsRequest\x12\x12\n\nclient_ids\x18\x01 \x03(\x0c\"A\n\x13ListClientsResponse\x12*\n\x07\x63lients\x18\x01 \x03(\x0b\x32\x19.fleetspeak.server.Client\"\xfb\x01\n\x06\x43lient\x12\x11\n\tclient_id\x18\x01 \x01(\x0c\x12!\n\x06labels\x18\x02 \x03(\x0b\x32\x11.fleetspeak.Label\x12\x35\n\x11last_contact_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1c\n\x14last_contact_address\x18\x04 \x01(\t\x12!\n\x19last_contact_streaming_to\x18\x07 \x01(\t\x12.\n\nlast_clock\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0b\x62lacklisted\x18\x06 \x01(\x08\"-\n\x17GetMessageStatusRequest\x12\x12\n\nmessage_id\x18\x01 \x01(\x0c\"2\n\x1c\x44\x65letePendingMessagesRequest\x12\x12\n\nclient_ids\x18\x01 \x03(\x0c\"a\n\x19GetPendingMessagesRequest\x12\x12\n\nclient_ids\x18\x01 \x03(\x0c\x12\x0e\n\x06offset\x18\x02 \x01(\x04\x12\r\n\x05limit\x18\x03 \x01(\x04\x12\x11\n\twant_data\x18\x04 \x01(\x08\"C\n\x1aGetPendingMessagesResponse\x12%\n\x08messages\x18\x01 \x03(\x0b\x32\x13.fleetspeak.Message\"3\n\x1dGetPendingMessageCountRequest\x12\x12\n\nclient_ids\x18\x01 \x03(\x0c\"/\n\x1eGetPendingMessageCountResponse\x12\r\n\x05\x63ount\x18\x01 \x01(\x04\"x\n\x18GetMessageStatusResponse\x12\x31\n\rcreation_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12)\n\x06result\x18\x02 \x01(\x0b\x32\x19.fleetspeak.MessageResult\"I\n\x10StoreFileRequest\x12\x14\n\x0cservice_name\x18\x01 \x01(\t\x12\x11\n\tfile_name\x18\x02 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x03 \x01(\x0c\".\n\x19ListClientContactsRequest\x12\x11\n\tclient_id\x18\x01 \x01(\x0c\"P\n\x1aListClientContactsResponse\x12\x32\n\x08\x63ontacts\x18\x01 \x03(\x0b\x32 .fleetspeak.server.ClientContact\"\x84\x01\n\rClientContact\x12\x12\n\nsent_nonce\x18\x01 \x01(\x06\x12\x16\n\x0ereceived_nonce\x18\x02 \x01(\x06\x12\x18\n\x10observed_address\x18\x03 \x01(\t\x12-\n\ttimestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"+\n\x16\x42lacklistClientRequest\x12\x11\n\tclient_id\x18\x01 \x01(\x0c\"\xa3\x01\n&FetchClientResourceUsageRecordsRequest\x12\x11\n\tclient_id\x18\x01 \x01(\x0c\x12\x33\n\x0fstart_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rend_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"h\n\'FetchClientResourceUsageRecordsResponse\x12=\n\x07records\x18\x01 \x03(\x0b\x32,.fleetspeak.server.ClientResourceUsageRecord2\xc6\n\n\x05\x41\x64min\x12X\n\x0f\x43reateBroadcast\x12).fleetspeak.server.CreateBroadcastRequest\x1a\x18.fleetspeak.EmptyMessage\"\x00\x12y\n\x14ListActiveBroadcasts\x12..fleetspeak.server.ListActiveBroadcastsRequest\x1a/.fleetspeak.server.ListActiveBroadcastsResponse\"\x00\x12^\n\x0bListClients\x12%.fleetspeak.server.ListClientsRequest\x1a&.fleetspeak.server.ListClientsResponse\"\x00\x12s\n\x12ListClientContacts\x12,.fleetspeak.server.ListClientContactsRequest\x1a-.fleetspeak.server.ListClientContactsResponse\"\x00\x12m\n\x10GetMessageStatus\x12*.fleetspeak.server.GetMessageStatusRequest\x1a+.fleetspeak.server.GetMessageStatusResponse\"\x00\x12@\n\rInsertMessage\x12\x13.fleetspeak.Message\x1a\x18.fleetspeak.EmptyMessage\"\x00\x12\x64\n\x15\x44\x65letePendingMessages\x12/.fleetspeak.server.DeletePendingMessagesRequest\x1a\x18.fleetspeak.EmptyMessage\"\x00\x12s\n\x12GetPendingMessages\x12,.fleetspeak.server.GetPendingMessagesRequest\x1a-.fleetspeak.server.GetPendingMessagesResponse\"\x00\x12\x7f\n\x16GetPendingMessageCount\x12\x30.fleetspeak.server.GetPendingMessageCountRequest\x1a\x31.fleetspeak.server.GetPendingMessageCountResponse\"\x00\x12L\n\tStoreFile\x12#.fleetspeak.server.StoreFileRequest\x1a\x18.fleetspeak.EmptyMessage\"\x00\x12\x41\n\tKeepAlive\x12\x18.fleetspeak.EmptyMessage\x1a\x18.fleetspeak.EmptyMessage\"\x00\x12X\n\x0f\x42lacklistClient\x12).fleetspeak.server.BlacklistClientRequest\x1a\x18.fleetspeak.EmptyMessage\"\x00\x12\x9a\x01\n\x1f\x46\x65tchClientResourceUsageRecords\x12\x39.fleetspeak.server.FetchClientResourceUsageRecordsRequest\x1a:.fleetspeak.server.FetchClientResourceUsageRecordsResponse\"\x00\x42LZJgithub.com/google/fleetspeak/fleetspeak/src/server/proto/fleetspeak_serverb\x06proto3')
   ,
   dependencies=[google_dot_protobuf_dot_timestamp__pb2.DESCRIPTOR,fleetspeak_dot_src_dot_common_dot_proto_dot_fleetspeak_dot_common__pb2.DESCRIPTOR,fleetspeak_dot_src_dot_server_dot_proto_dot_fleetspeak__server_dot_broadcasts__pb2.DESCRIPTOR,fleetspeak_dot_src_dot_server_dot_proto_dot_fleetspeak__server_dot_resource__pb2.DESCRIPTOR,])
 
 
 
 
 _CREATEBROADCASTREQUEST = _descriptor.Descriptor(
@@ -324,14 +324,159 @@
   oneofs=[
   ],
   serialized_start=927,
   serialized_end=977,
 )
 
 
+_GETPENDINGMESSAGESREQUEST = _descriptor.Descriptor(
+  name='GetPendingMessagesRequest',
+  full_name='fleetspeak.server.GetPendingMessagesRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='client_ids', full_name='fleetspeak.server.GetPendingMessagesRequest.client_ids', index=0,
+      number=1, type=12, cpp_type=9, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='offset', full_name='fleetspeak.server.GetPendingMessagesRequest.offset', index=1,
+      number=2, type=4, cpp_type=4, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='limit', full_name='fleetspeak.server.GetPendingMessagesRequest.limit', index=2,
+      number=3, type=4, cpp_type=4, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='want_data', full_name='fleetspeak.server.GetPendingMessagesRequest.want_data', index=3,
+      number=4, type=8, cpp_type=7, label=1,
+      has_default_value=False, default_value=False,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=979,
+  serialized_end=1076,
+)
+
+
+_GETPENDINGMESSAGESRESPONSE = _descriptor.Descriptor(
+  name='GetPendingMessagesResponse',
+  full_name='fleetspeak.server.GetPendingMessagesResponse',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='messages', full_name='fleetspeak.server.GetPendingMessagesResponse.messages', index=0,
+      number=1, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=1078,
+  serialized_end=1145,
+)
+
+
+_GETPENDINGMESSAGECOUNTREQUEST = _descriptor.Descriptor(
+  name='GetPendingMessageCountRequest',
+  full_name='fleetspeak.server.GetPendingMessageCountRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='client_ids', full_name='fleetspeak.server.GetPendingMessageCountRequest.client_ids', index=0,
+      number=1, type=12, cpp_type=9, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=1147,
+  serialized_end=1198,
+)
+
+
+_GETPENDINGMESSAGECOUNTRESPONSE = _descriptor.Descriptor(
+  name='GetPendingMessageCountResponse',
+  full_name='fleetspeak.server.GetPendingMessageCountResponse',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='count', full_name='fleetspeak.server.GetPendingMessageCountResponse.count', index=0,
+      number=1, type=4, cpp_type=4, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=1200,
+  serialized_end=1247,
+)
+
+
 _GETMESSAGESTATUSRESPONSE = _descriptor.Descriptor(
   name='GetMessageStatusResponse',
   full_name='fleetspeak.server.GetMessageStatusResponse',
   filename=None,
   file=DESCRIPTOR,
   containing_type=None,
   fields=[
@@ -357,16 +502,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=979,
-  serialized_end=1099,
+  serialized_start=1249,
+  serialized_end=1369,
 )
 
 
 _STOREFILEREQUEST = _descriptor.Descriptor(
   name='StoreFileRequest',
   full_name='fleetspeak.server.StoreFileRequest',
   filename=None,
@@ -402,16 +547,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1101,
-  serialized_end=1174,
+  serialized_start=1371,
+  serialized_end=1444,
 )
 
 
 _LISTCLIENTCONTACTSREQUEST = _descriptor.Descriptor(
   name='ListClientContactsRequest',
   full_name='fleetspeak.server.ListClientContactsRequest',
   filename=None,
@@ -433,16 +578,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1176,
-  serialized_end=1222,
+  serialized_start=1446,
+  serialized_end=1492,
 )
 
 
 _LISTCLIENTCONTACTSRESPONSE = _descriptor.Descriptor(
   name='ListClientContactsResponse',
   full_name='fleetspeak.server.ListClientContactsResponse',
   filename=None,
@@ -464,16 +609,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1224,
-  serialized_end=1304,
+  serialized_start=1494,
+  serialized_end=1574,
 )
 
 
 _CLIENTCONTACT = _descriptor.Descriptor(
   name='ClientContact',
   full_name='fleetspeak.server.ClientContact',
   filename=None,
@@ -516,16 +661,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1307,
-  serialized_end=1439,
+  serialized_start=1577,
+  serialized_end=1709,
 )
 
 
 _BLACKLISTCLIENTREQUEST = _descriptor.Descriptor(
   name='BlacklistClientRequest',
   full_name='fleetspeak.server.BlacklistClientRequest',
   filename=None,
@@ -547,16 +692,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1441,
-  serialized_end=1484,
+  serialized_start=1711,
+  serialized_end=1754,
 )
 
 
 _FETCHCLIENTRESOURCEUSAGERECORDSREQUEST = _descriptor.Descriptor(
   name='FetchClientResourceUsageRecordsRequest',
   full_name='fleetspeak.server.FetchClientResourceUsageRecordsRequest',
   filename=None,
@@ -592,16 +737,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1487,
-  serialized_end=1650,
+  serialized_start=1757,
+  serialized_end=1920,
 )
 
 
 _FETCHCLIENTRESOURCEUSAGERECORDSRESPONSE = _descriptor.Descriptor(
   name='FetchClientResourceUsageRecordsResponse',
   full_name='fleetspeak.server.FetchClientResourceUsageRecordsResponse',
   filename=None,
@@ -623,24 +768,25 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1652,
-  serialized_end=1756,
+  serialized_start=1922,
+  serialized_end=2026,
 )
 
 _CREATEBROADCASTREQUEST.fields_by_name['broadcast'].message_type = fleetspeak_dot_src_dot_server_dot_proto_dot_fleetspeak__server_dot_broadcasts__pb2._BROADCAST
 _LISTACTIVEBROADCASTSRESPONSE.fields_by_name['broadcasts'].message_type = fleetspeak_dot_src_dot_server_dot_proto_dot_fleetspeak__server_dot_broadcasts__pb2._BROADCAST
 _LISTCLIENTSRESPONSE.fields_by_name['clients'].message_type = _CLIENT
 _CLIENT.fields_by_name['labels'].message_type = fleetspeak_dot_src_dot_common_dot_proto_dot_fleetspeak_dot_common__pb2._LABEL
 _CLIENT.fields_by_name['last_contact_time'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _CLIENT.fields_by_name['last_clock'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
+_GETPENDINGMESSAGESRESPONSE.fields_by_name['messages'].message_type = fleetspeak_dot_src_dot_common_dot_proto_dot_fleetspeak_dot_common__pb2._MESSAGE
 _GETMESSAGESTATUSRESPONSE.fields_by_name['creation_time'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _GETMESSAGESTATUSRESPONSE.fields_by_name['result'].message_type = fleetspeak_dot_src_dot_common_dot_proto_dot_fleetspeak_dot_common__pb2._MESSAGERESULT
 _LISTCLIENTCONTACTSRESPONSE.fields_by_name['contacts'].message_type = _CLIENTCONTACT
 _CLIENTCONTACT.fields_by_name['timestamp'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _FETCHCLIENTRESOURCEUSAGERECORDSREQUEST.fields_by_name['start_timestamp'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _FETCHCLIENTRESOURCEUSAGERECORDSREQUEST.fields_by_name['end_timestamp'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _FETCHCLIENTRESOURCEUSAGERECORDSRESPONSE.fields_by_name['records'].message_type = fleetspeak_dot_src_dot_server_dot_proto_dot_fleetspeak__server_dot_resource__pb2._CLIENTRESOURCEUSAGERECORD
@@ -648,14 +794,18 @@
 DESCRIPTOR.message_types_by_name['ListActiveBroadcastsRequest'] = _LISTACTIVEBROADCASTSREQUEST
 DESCRIPTOR.message_types_by_name['ListActiveBroadcastsResponse'] = _LISTACTIVEBROADCASTSRESPONSE
 DESCRIPTOR.message_types_by_name['ListClientsRequest'] = _LISTCLIENTSREQUEST
 DESCRIPTOR.message_types_by_name['ListClientsResponse'] = _LISTCLIENTSRESPONSE
 DESCRIPTOR.message_types_by_name['Client'] = _CLIENT
 DESCRIPTOR.message_types_by_name['GetMessageStatusRequest'] = _GETMESSAGESTATUSREQUEST
 DESCRIPTOR.message_types_by_name['DeletePendingMessagesRequest'] = _DELETEPENDINGMESSAGESREQUEST
+DESCRIPTOR.message_types_by_name['GetPendingMessagesRequest'] = _GETPENDINGMESSAGESREQUEST
+DESCRIPTOR.message_types_by_name['GetPendingMessagesResponse'] = _GETPENDINGMESSAGESRESPONSE
+DESCRIPTOR.message_types_by_name['GetPendingMessageCountRequest'] = _GETPENDINGMESSAGECOUNTREQUEST
+DESCRIPTOR.message_types_by_name['GetPendingMessageCountResponse'] = _GETPENDINGMESSAGECOUNTRESPONSE
 DESCRIPTOR.message_types_by_name['GetMessageStatusResponse'] = _GETMESSAGESTATUSRESPONSE
 DESCRIPTOR.message_types_by_name['StoreFileRequest'] = _STOREFILEREQUEST
 DESCRIPTOR.message_types_by_name['ListClientContactsRequest'] = _LISTCLIENTCONTACTSREQUEST
 DESCRIPTOR.message_types_by_name['ListClientContactsResponse'] = _LISTCLIENTCONTACTSRESPONSE
 DESCRIPTOR.message_types_by_name['ClientContact'] = _CLIENTCONTACT
 DESCRIPTOR.message_types_by_name['BlacklistClientRequest'] = _BLACKLISTCLIENTREQUEST
 DESCRIPTOR.message_types_by_name['FetchClientResourceUsageRecordsRequest'] = _FETCHCLIENTRESOURCEUSAGERECORDSREQUEST
@@ -714,14 +864,42 @@
 DeletePendingMessagesRequest = _reflection.GeneratedProtocolMessageType('DeletePendingMessagesRequest', (_message.Message,), {
   'DESCRIPTOR' : _DELETEPENDINGMESSAGESREQUEST,
   '__module__' : 'fleetspeak.src.server.proto.fleetspeak_server.admin_pb2'
   # @@protoc_insertion_point(class_scope:fleetspeak.server.DeletePendingMessagesRequest)
   })
 _sym_db.RegisterMessage(DeletePendingMessagesRequest)
 
+GetPendingMessagesRequest = _reflection.GeneratedProtocolMessageType('GetPendingMessagesRequest', (_message.Message,), {
+  'DESCRIPTOR' : _GETPENDINGMESSAGESREQUEST,
+  '__module__' : 'fleetspeak.src.server.proto.fleetspeak_server.admin_pb2'
+  # @@protoc_insertion_point(class_scope:fleetspeak.server.GetPendingMessagesRequest)
+  })
+_sym_db.RegisterMessage(GetPendingMessagesRequest)
+
+GetPendingMessagesResponse = _reflection.GeneratedProtocolMessageType('GetPendingMessagesResponse', (_message.Message,), {
+  'DESCRIPTOR' : _GETPENDINGMESSAGESRESPONSE,
+  '__module__' : 'fleetspeak.src.server.proto.fleetspeak_server.admin_pb2'
+  # @@protoc_insertion_point(class_scope:fleetspeak.server.GetPendingMessagesResponse)
+  })
+_sym_db.RegisterMessage(GetPendingMessagesResponse)
+
+GetPendingMessageCountRequest = _reflection.GeneratedProtocolMessageType('GetPendingMessageCountRequest', (_message.Message,), {
+  'DESCRIPTOR' : _GETPENDINGMESSAGECOUNTREQUEST,
+  '__module__' : 'fleetspeak.src.server.proto.fleetspeak_server.admin_pb2'
+  # @@protoc_insertion_point(class_scope:fleetspeak.server.GetPendingMessageCountRequest)
+  })
+_sym_db.RegisterMessage(GetPendingMessageCountRequest)
+
+GetPendingMessageCountResponse = _reflection.GeneratedProtocolMessageType('GetPendingMessageCountResponse', (_message.Message,), {
+  'DESCRIPTOR' : _GETPENDINGMESSAGECOUNTRESPONSE,
+  '__module__' : 'fleetspeak.src.server.proto.fleetspeak_server.admin_pb2'
+  # @@protoc_insertion_point(class_scope:fleetspeak.server.GetPendingMessageCountResponse)
+  })
+_sym_db.RegisterMessage(GetPendingMessageCountResponse)
+
 GetMessageStatusResponse = _reflection.GeneratedProtocolMessageType('GetMessageStatusResponse', (_message.Message,), {
   'DESCRIPTOR' : _GETMESSAGESTATUSRESPONSE,
   '__module__' : 'fleetspeak.src.server.proto.fleetspeak_server.admin_pb2'
   # @@protoc_insertion_point(class_scope:fleetspeak.server.GetMessageStatusResponse)
   })
 _sym_db.RegisterMessage(GetMessageStatusResponse)
 
@@ -779,16 +957,16 @@
 
 _ADMIN = _descriptor.ServiceDescriptor(
   name='Admin',
   full_name='fleetspeak.server.Admin',
   file=DESCRIPTOR,
   index=0,
   serialized_options=None,
-  serialized_start=1759,
-  serialized_end=2863,
+  serialized_start=2029,
+  serialized_end=3379,
   methods=[
   _descriptor.MethodDescriptor(
     name='CreateBroadcast',
     full_name='fleetspeak.server.Admin.CreateBroadcast',
     index=0,
     containing_service=None,
     input_type=_CREATEBROADCASTREQUEST,
@@ -846,44 +1024,62 @@
     index=6,
     containing_service=None,
     input_type=_DELETEPENDINGMESSAGESREQUEST,
     output_type=fleetspeak_dot_src_dot_common_dot_proto_dot_fleetspeak_dot_common__pb2._EMPTYMESSAGE,
     serialized_options=None,
   ),
   _descriptor.MethodDescriptor(
+    name='GetPendingMessages',
+    full_name='fleetspeak.server.Admin.GetPendingMessages',
+    index=7,
+    containing_service=None,
+    input_type=_GETPENDINGMESSAGESREQUEST,
+    output_type=_GETPENDINGMESSAGESRESPONSE,
+    serialized_options=None,
+  ),
+  _descriptor.MethodDescriptor(
+    name='GetPendingMessageCount',
+    full_name='fleetspeak.server.Admin.GetPendingMessageCount',
+    index=8,
+    containing_service=None,
+    input_type=_GETPENDINGMESSAGECOUNTREQUEST,
+    output_type=_GETPENDINGMESSAGECOUNTRESPONSE,
+    serialized_options=None,
+  ),
+  _descriptor.MethodDescriptor(
     name='StoreFile',
     full_name='fleetspeak.server.Admin.StoreFile',
-    index=7,
+    index=9,
     containing_service=None,
     input_type=_STOREFILEREQUEST,
     output_type=fleetspeak_dot_src_dot_common_dot_proto_dot_fleetspeak_dot_common__pb2._EMPTYMESSAGE,
     serialized_options=None,
   ),
   _descriptor.MethodDescriptor(
     name='KeepAlive',
     full_name='fleetspeak.server.Admin.KeepAlive',
-    index=8,
+    index=10,
     containing_service=None,
     input_type=fleetspeak_dot_src_dot_common_dot_proto_dot_fleetspeak_dot_common__pb2._EMPTYMESSAGE,
     output_type=fleetspeak_dot_src_dot_common_dot_proto_dot_fleetspeak_dot_common__pb2._EMPTYMESSAGE,
     serialized_options=None,
   ),
   _descriptor.MethodDescriptor(
     name='BlacklistClient',
     full_name='fleetspeak.server.Admin.BlacklistClient',
-    index=9,
+    index=11,
     containing_service=None,
     input_type=_BLACKLISTCLIENTREQUEST,
     output_type=fleetspeak_dot_src_dot_common_dot_proto_dot_fleetspeak_dot_common__pb2._EMPTYMESSAGE,
     serialized_options=None,
   ),
   _descriptor.MethodDescriptor(
     name='FetchClientResourceUsageRecords',
     full_name='fleetspeak.server.Admin.FetchClientResourceUsageRecords',
-    index=10,
+    index=12,
     containing_service=None,
     input_type=_FETCHCLIENTRESOURCEUSAGERECORDSREQUEST,
     output_type=_FETCHCLIENTRESOURCEUSAGERECORDSRESPONSE,
     serialized_options=None,
   ),
 ])
 _sym_db.RegisterServiceDescriptor(_ADMIN)
```

### Comparing `fleetspeak-0.1.8/fleetspeak/src/server/proto/fleetspeak_server/admin_pb2_grpc.py` & `fleetspeak-0.1.9/fleetspeak/src/server/proto/fleetspeak_server/admin_pb2_grpc.py`

 * *Files 12% similar despite different names*

```diff
@@ -46,14 +46,24 @@
         response_deserializer=fleetspeak_dot_src_dot_common_dot_proto_dot_fleetspeak_dot_common__pb2.EmptyMessage.FromString,
         )
     self.DeletePendingMessages = channel.unary_unary(
         '/fleetspeak.server.Admin/DeletePendingMessages',
         request_serializer=fleetspeak_dot_src_dot_server_dot_proto_dot_fleetspeak__server_dot_admin__pb2.DeletePendingMessagesRequest.SerializeToString,
         response_deserializer=fleetspeak_dot_src_dot_common_dot_proto_dot_fleetspeak_dot_common__pb2.EmptyMessage.FromString,
         )
+    self.GetPendingMessages = channel.unary_unary(
+        '/fleetspeak.server.Admin/GetPendingMessages',
+        request_serializer=fleetspeak_dot_src_dot_server_dot_proto_dot_fleetspeak__server_dot_admin__pb2.GetPendingMessagesRequest.SerializeToString,
+        response_deserializer=fleetspeak_dot_src_dot_server_dot_proto_dot_fleetspeak__server_dot_admin__pb2.GetPendingMessagesResponse.FromString,
+        )
+    self.GetPendingMessageCount = channel.unary_unary(
+        '/fleetspeak.server.Admin/GetPendingMessageCount',
+        request_serializer=fleetspeak_dot_src_dot_server_dot_proto_dot_fleetspeak__server_dot_admin__pb2.GetPendingMessageCountRequest.SerializeToString,
+        response_deserializer=fleetspeak_dot_src_dot_server_dot_proto_dot_fleetspeak__server_dot_admin__pb2.GetPendingMessageCountResponse.FromString,
+        )
     self.StoreFile = channel.unary_unary(
         '/fleetspeak.server.Admin/StoreFile',
         request_serializer=fleetspeak_dot_src_dot_server_dot_proto_dot_fleetspeak__server_dot_admin__pb2.StoreFileRequest.SerializeToString,
         response_deserializer=fleetspeak_dot_src_dot_common_dot_proto_dot_fleetspeak_dot_common__pb2.EmptyMessage.FromString,
         )
     self.KeepAlive = channel.unary_unary(
         '/fleetspeak.server.Admin/KeepAlive',
@@ -125,14 +135,28 @@
   def DeletePendingMessages(self, request, context):
     """DeletePendingMessages clears message queues for given clients.
     """
     context.set_code(grpc.StatusCode.UNIMPLEMENTED)
     context.set_details('Method not implemented!')
     raise NotImplementedError('Method not implemented!')
 
+  def GetPendingMessages(self, request, context):
+    """Returns the pending messages for given clients.
+    """
+    context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+    context.set_details('Method not implemented!')
+    raise NotImplementedError('Method not implemented!')
+
+  def GetPendingMessageCount(self, request, context):
+    """Returns the number of pending messages for the given clients.
+    """
+    context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+    context.set_details('Method not implemented!')
+    raise NotImplementedError('Method not implemented!')
+
   def StoreFile(self, request, context):
     """StoreFile inserts a file into the Fleetspeak system.
     """
     context.set_code(grpc.StatusCode.UNIMPLEMENTED)
     context.set_details('Method not implemented!')
     raise NotImplementedError('Method not implemented!')
 
@@ -193,14 +217,24 @@
           response_serializer=fleetspeak_dot_src_dot_common_dot_proto_dot_fleetspeak_dot_common__pb2.EmptyMessage.SerializeToString,
       ),
       'DeletePendingMessages': grpc.unary_unary_rpc_method_handler(
           servicer.DeletePendingMessages,
           request_deserializer=fleetspeak_dot_src_dot_server_dot_proto_dot_fleetspeak__server_dot_admin__pb2.DeletePendingMessagesRequest.FromString,
           response_serializer=fleetspeak_dot_src_dot_common_dot_proto_dot_fleetspeak_dot_common__pb2.EmptyMessage.SerializeToString,
       ),
+      'GetPendingMessages': grpc.unary_unary_rpc_method_handler(
+          servicer.GetPendingMessages,
+          request_deserializer=fleetspeak_dot_src_dot_server_dot_proto_dot_fleetspeak__server_dot_admin__pb2.GetPendingMessagesRequest.FromString,
+          response_serializer=fleetspeak_dot_src_dot_server_dot_proto_dot_fleetspeak__server_dot_admin__pb2.GetPendingMessagesResponse.SerializeToString,
+      ),
+      'GetPendingMessageCount': grpc.unary_unary_rpc_method_handler(
+          servicer.GetPendingMessageCount,
+          request_deserializer=fleetspeak_dot_src_dot_server_dot_proto_dot_fleetspeak__server_dot_admin__pb2.GetPendingMessageCountRequest.FromString,
+          response_serializer=fleetspeak_dot_src_dot_server_dot_proto_dot_fleetspeak__server_dot_admin__pb2.GetPendingMessageCountResponse.SerializeToString,
+      ),
       'StoreFile': grpc.unary_unary_rpc_method_handler(
           servicer.StoreFile,
           request_deserializer=fleetspeak_dot_src_dot_server_dot_proto_dot_fleetspeak__server_dot_admin__pb2.StoreFileRequest.FromString,
           response_serializer=fleetspeak_dot_src_dot_common_dot_proto_dot_fleetspeak_dot_common__pb2.EmptyMessage.SerializeToString,
       ),
       'KeepAlive': grpc.unary_unary_rpc_method_handler(
           servicer.KeepAlive,
```

### Comparing `fleetspeak-0.1.8/fleetspeak/src/osquery/proto/fleetspeak_osquery/osquery_pb2.py` & `fleetspeak-0.1.9/fleetspeak/src/osquery/proto/fleetspeak_osquery/osquery_pb2.py`

 * *Files identical despite different names*

### Comparing `fleetspeak-0.1.8/fleetspeak/client_connector/testing/testclient_launcher.py` & `fleetspeak-0.1.9/fleetspeak/client_connector/testing/testclient_launcher.py`

 * *Files identical despite different names*

### Comparing `fleetspeak-0.1.8/fleetspeak/client_connector/testing/testclient.py` & `fleetspeak-0.1.9/fleetspeak/client_connector/testing/testclient.py`

 * *Files identical despite different names*

### Comparing `fleetspeak-0.1.8/fleetspeak/client_connector/connector.py` & `fleetspeak-0.1.9/fleetspeak/client_connector/connector.py`

 * *Files identical despite different names*

### Comparing `fleetspeak-0.1.8/fleetspeak.egg-info/SOURCES.txt` & `fleetspeak-0.1.9/fleetspeak.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fleetspeak-0.1.8/fleetspeak.egg-info/PKG-INFO` & `fleetspeak-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: fleetspeak
-Version: 0.1.8
+Version: 0.1.9
 Summary: Fleetspeak
 Home-page: https://github.com/google/fleetspeak
 Maintainer: GRR Development Team
 Maintainer-email: grr-dev@googlegroups.com
 License: Apache License, Version 2.0
 Description: Fleetspeak is a framework for communicating with a fleet of machines, with a focus on security monitoring and basic administrative use cases. It is a subproject of GRR ( https://github.com/google/grr/blob/master/README.md ), and can be seen as an effort to modularizing and modernizing its communication mechanism.
 Platform: UNKNOWN
```

### Comparing `fleetspeak-0.1.8/PKG-INFO` & `fleetspeak-0.1.9/fleetspeak.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: fleetspeak
-Version: 0.1.8
+Version: 0.1.9
 Summary: Fleetspeak
 Home-page: https://github.com/google/fleetspeak
 Maintainer: GRR Development Team
 Maintainer-email: grr-dev@googlegroups.com
 License: Apache License, Version 2.0
 Description: Fleetspeak is a framework for communicating with a fleet of machines, with a focus on security monitoring and basic administrative use cases. It is a subproject of GRR ( https://github.com/google/grr/blob/master/README.md ), and can be seen as an effort to modularizing and modernizing its communication mechanism.
 Platform: UNKNOWN
```

