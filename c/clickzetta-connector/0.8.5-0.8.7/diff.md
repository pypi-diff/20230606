# Comparing `tmp/clickzetta-connector-0.8.5.tar.gz` & `tmp/clickzetta-connector-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickzetta-connector-0.8.5.tar", last modified: Tue May 30 14:05:02 2023, max compression
+gzip compressed data, was "clickzetta-connector-0.8.7.tar", last modified: Tue Jun  6 07:48:36 2023, max compression
```

## Comparing `clickzetta-connector-0.8.5.tar` & `clickzetta-connector-0.8.7.tar`

### file list

```diff
@@ -1,147 +1,147 @@
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-30 14:05:02.935343 clickzetta-connector-0.8.5/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       49 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/MANIFEST.in
--rw-r--r--   0 lihanmiao   (501) staff       (20)      387 2023-05-30 14:05:02.935214 clickzetta-connector-0.8.5/PKG-INFO
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-30 14:05:02.922782 clickzetta-connector-0.8.5/clickzetta/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      159 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     9899 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/_helpers.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-30 14:05:02.923709 clickzetta-connector-0.8.5/clickzetta/bulkload/
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/bulkload/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7196 2023-05-30 13:49:26.000000 clickzetta-connector-0.8.5/clickzetta/bulkload/bulkload_enums.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4387 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/bulkload/bulkload_stream.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    14842 2023-05-30 08:58:01.000000 clickzetta-connector-0.8.5/clickzetta/bulkload/bulkload_writer.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      483 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/bulkload/cz_table.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    21726 2023-05-30 03:03:43.000000 clickzetta-connector-0.8.5/clickzetta/client.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-30 14:05:02.924662 clickzetta-connector-0.8.5/clickzetta/dbapi/
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1677 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/dbapi/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1000 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/dbapi/_helpers.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2761 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/dbapi/connection.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2899 2023-05-30 03:03:57.000000 clickzetta-connector-0.8.5/clickzetta/dbapi/cursor.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1100 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/dbapi/exceptions.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1131 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/dbapi/types.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7203 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/enums.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-30 14:05:02.920745 clickzetta-connector-0.8.5/clickzetta/proto/
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-30 14:05:02.931395 clickzetta-connector-0.8.5/clickzetta/proto/generated/
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2488 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/account_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/account_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1623 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/block_bloom_filter_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/block_bloom_filter_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1078 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/bucket_info_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/bucket_info_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1233 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/compression_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/compression_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1739 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/connection_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/connection_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     5567 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/data_type_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/data_type_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4689 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/expression_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/expression_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1251 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/file_format_type_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/file_format_type_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3623 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/file_meta_data_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/file_meta_data_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1087 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/file_system_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/file_system_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2232 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/function_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/function_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1106 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/hash_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/hash_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    18361 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/ingestion_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    20165 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/ingestion_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6794 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/input_split_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/input_split_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     5520 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/job_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/job_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1683 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/job_result_cache_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/job_result_cache_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    11392 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/kudu_common_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/kudu_common_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4271 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/metadata_entity_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/metadata_entity_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1300 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/network_policy_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/network_policy_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2847 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/object_identifier_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/object_identifier_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    35572 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/operator_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/operator_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1430 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/pb_util_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/pb_util_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1130 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/property_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/property_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1861 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/rm_app_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/rm_app_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1354 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/role_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/role_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2102 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/row_operations_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/row_operations_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      944 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/schema_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/schema_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1509 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/share_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/share_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     5493 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/statistics_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/statistics_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)    11527 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/table_common_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/table_common_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3834 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/table_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/table_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4089 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/virtual_cluster_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/virtual_cluster_meta_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6210 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/virtual_cluster_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/virtual_cluster_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1382 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/virtual_cluster_size_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/virtual_cluster_size_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1836 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/virtual_value_info_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/virtual_value_info_pb2_grpc.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1208 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/workspace_meta_pb2.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta/proto/generated/workspace_meta_pb2_grpc.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-30 14:05:02.934544 clickzetta-connector-0.8.5/clickzetta/proto/source/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      770 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/proto/source/account.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1549 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/proto/source/block_bloom_filter.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      190 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/proto/source/bucket_info.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1017 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/proto/source/compression.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      413 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/proto/source/connection_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2033 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/proto/source/data_type.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1697 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/proto/source/expression.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      284 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/proto/source/file_format_type.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1781 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/proto/source/file_meta_data.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      121 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/proto/source/file_system.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      643 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/proto/source/function_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1007 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/proto/source/hash.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     8197 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/proto/source/ingestion.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2908 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/proto/source/input_split.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2134 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/proto/source/job_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      444 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/proto/source/job_result_cache_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)    18379 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/proto/source/kudu_common.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1417 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/proto/source/metadata_entity.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      311 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/proto/source/network_policy.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1071 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/proto/source/object_identifier.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)    16166 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/proto/source/operator.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1805 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/proto/source/pb_util.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      157 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/proto/source/property.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      515 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/proto/source/rm_app_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      232 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/proto/source/role_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3795 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/proto/source/row_operations.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)       81 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/proto/source/schema.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      312 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/proto/source/share_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2539 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/proto/source/statistics.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4801 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/proto/source/table_common.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1895 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/proto/source/table_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2387 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/proto/source/virtual_cluster.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1337 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/proto/source/virtual_cluster_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      253 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/proto/source/virtual_cluster_size.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1034 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/proto/source/virtual_value_info.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)      376 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/proto/source/workspace_meta.proto
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7167 2023-05-30 03:03:57.000000 clickzetta-connector-0.8.5/clickzetta/query_result.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6368 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/schema.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3557 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/session.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4780 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/standard_sql.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2277 2023-05-26 08:14:07.000000 clickzetta-connector-0.8.5/clickzetta/table.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)       21 2023-05-30 14:04:49.000000 clickzetta-connector-0.8.5/clickzetta/version.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-05-30 14:05:02.935076 clickzetta-connector-0.8.5/clickzetta_connector.egg-info/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      387 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta_connector.egg-info/PKG-INFO
--rw-r--r--   0 lihanmiao   (501) staff       (20)     5988 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta_connector.egg-info/SOURCES.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta_connector.egg-info/dependency_links.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta_connector.egg-info/not-zip-safe
--rw-r--r--   0 lihanmiao   (501) staff       (20)      630 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta_connector.egg-info/requires.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       11 2023-05-30 14:05:02.000000 clickzetta-connector-0.8.5/clickzetta_connector.egg-info/top_level.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-05-30 14:05:02.935384 clickzetta-connector-0.8.5/setup.cfg
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2907 2023-05-30 14:04:49.000000 clickzetta-connector-0.8.5/setup.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-06 07:48:36.330946 clickzetta-connector-0.8.7/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       49 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/MANIFEST.in
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      387 2023-06-06 07:48:36.330794 clickzetta-connector-0.8.7/PKG-INFO
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-06 07:48:36.317147 clickzetta-connector-0.8.7/clickzetta/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      159 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     9863 2023-06-06 07:11:17.000000 clickzetta-connector-0.8.7/clickzetta/_helpers.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-06 07:48:36.318258 clickzetta-connector-0.8.7/clickzetta/bulkload/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/bulkload/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7196 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/bulkload/bulkload_enums.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4386 2023-06-06 06:47:54.000000 clickzetta-connector-0.8.7/clickzetta/bulkload/bulkload_stream.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    14842 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/bulkload/bulkload_writer.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      483 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/bulkload/cz_table.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    21821 2023-06-06 07:44:26.000000 clickzetta-connector-0.8.7/clickzetta/client.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-06 07:48:36.319258 clickzetta-connector-0.8.7/clickzetta/dbapi/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1677 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/dbapi/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1000 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/dbapi/_helpers.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2845 2023-06-06 07:27:43.000000 clickzetta-connector-0.8.7/clickzetta/dbapi/connection.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2899 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/dbapi/cursor.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1100 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/dbapi/exceptions.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1131 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/dbapi/types.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7183 2023-06-06 07:11:17.000000 clickzetta-connector-0.8.7/clickzetta/enums.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-06 07:48:36.315188 clickzetta-connector-0.8.7/clickzetta/proto/
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-06 07:48:36.326424 clickzetta-connector-0.8.7/clickzetta/proto/generated/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2488 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/account_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/account_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1623 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/block_bloom_filter_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/block_bloom_filter_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1078 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/bucket_info_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-06-06 07:48:35.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/bucket_info_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1233 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/compression_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/compression_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1739 2023-06-06 07:48:35.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/connection_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/connection_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     5567 2023-06-06 07:48:35.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/data_type_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/data_type_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4689 2023-06-06 07:48:35.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/expression_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/expression_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1251 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/file_format_type_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/file_format_type_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3623 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/file_meta_data_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-06-06 07:48:35.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/file_meta_data_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1087 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/file_system_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/file_system_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2232 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/function_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/function_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1106 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/hash_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/hash_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    18361 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/ingestion_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    20165 2023-06-06 07:48:35.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/ingestion_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     6794 2023-06-06 07:48:35.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/input_split_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/input_split_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     5520 2023-06-06 07:48:35.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/job_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/job_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1683 2023-06-06 07:48:35.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/job_result_cache_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-06-06 07:48:35.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/job_result_cache_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    11392 2023-06-06 07:48:35.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/kudu_common_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/kudu_common_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4271 2023-06-06 07:48:35.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/metadata_entity_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/metadata_entity_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1300 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/network_policy_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/network_policy_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2847 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/object_identifier_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/object_identifier_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    35572 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/operator_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/operator_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1430 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/pb_util_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/pb_util_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1130 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/property_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/property_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1861 2023-06-06 07:48:35.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/rm_app_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/rm_app_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1354 2023-06-06 07:48:35.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/role_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-06-06 07:48:35.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/role_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2102 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/row_operations_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/row_operations_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      944 2023-06-06 07:48:35.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/schema_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-06-06 07:48:35.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/schema_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1509 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/share_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/share_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     5493 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/statistics_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/statistics_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    11527 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/table_common_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/table_common_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3834 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/table_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-06-06 07:48:35.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/table_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4089 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/virtual_cluster_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/virtual_cluster_meta_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     6210 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/virtual_cluster_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-06-06 07:48:35.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/virtual_cluster_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1382 2023-06-06 07:48:35.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/virtual_cluster_size_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/virtual_cluster_size_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1836 2023-06-06 07:48:35.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/virtual_value_info_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-06-06 07:48:35.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/virtual_value_info_pb2_grpc.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1208 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/workspace_meta_pb2.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      166 2023-06-06 07:48:35.000000 clickzetta-connector-0.8.7/clickzetta/proto/generated/workspace_meta_pb2_grpc.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-06 07:48:36.330003 clickzetta-connector-0.8.7/clickzetta/proto/source/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      770 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/proto/source/account.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1549 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/proto/source/block_bloom_filter.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      190 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/proto/source/bucket_info.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1017 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/proto/source/compression.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      413 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/proto/source/connection_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2033 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/proto/source/data_type.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1697 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/proto/source/expression.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      284 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/proto/source/file_format_type.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1781 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/proto/source/file_meta_data.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      121 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/proto/source/file_system.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      643 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/proto/source/function_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1007 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/proto/source/hash.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     8197 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/proto/source/ingestion.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2908 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/proto/source/input_split.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2134 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/proto/source/job_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      444 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/proto/source/job_result_cache_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    18379 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/proto/source/kudu_common.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1417 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/proto/source/metadata_entity.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      311 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/proto/source/network_policy.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1071 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/proto/source/object_identifier.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    16166 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/proto/source/operator.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1805 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/proto/source/pb_util.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      157 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/proto/source/property.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      515 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/proto/source/rm_app_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      232 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/proto/source/role_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3795 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/proto/source/row_operations.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       81 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/proto/source/schema.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      312 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/proto/source/share_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2539 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/proto/source/statistics.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4801 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/proto/source/table_common.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1895 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/proto/source/table_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2387 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/proto/source/virtual_cluster.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1337 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/proto/source/virtual_cluster_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      253 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/proto/source/virtual_cluster_size.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1034 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/proto/source/virtual_value_info.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      376 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/proto/source/workspace_meta.proto
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7167 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/query_result.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     6368 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/schema.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3557 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/session.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4780 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/standard_sql.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2277 2023-06-01 02:26:20.000000 clickzetta-connector-0.8.7/clickzetta/table.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       21 2023-06-06 07:48:30.000000 clickzetta-connector-0.8.7/clickzetta/version.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-06 07:48:36.330606 clickzetta-connector-0.8.7/clickzetta_connector.egg-info/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      387 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta_connector.egg-info/PKG-INFO
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     5988 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta_connector.egg-info/not-zip-safe
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      630 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta_connector.egg-info/requires.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       11 2023-06-06 07:48:36.000000 clickzetta-connector-0.8.7/clickzetta_connector.egg-info/top_level.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-06-06 07:48:36.330993 clickzetta-connector-0.8.7/setup.cfg
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2926 2023-06-06 06:47:54.000000 clickzetta-connector-0.8.7/setup.py
```

### Comparing `clickzetta-connector-0.8.5/clickzetta/_helpers.py` & `clickzetta-connector-0.8.7/clickzetta/_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 _PROJECT_PREFIX_PATTERN = re.compile(
     r"""
     (?P<project_id>\S+\:[^.]+)\.(?P<dataset_id>[^.]+)(?:$|\.(?P<custom_id>[^.]+)$)
 """,
     re.VERBOSE,
 )
 
-CZ_EMULATOR_HOST = "https://dev-api.zettadecision.com"
+CZ_EMULATOR_HOST = "CZ_EMULATOR_HOST"
 
-_DEFAULT_HOST = "https://dev-api.zettadecision.com"
+_DEFAULT_HOST = "localhost:8080"
 
 
 def _get_click_zetta_host():
     return os.environ.get(CZ_EMULATOR_HOST, _DEFAULT_HOST)
 
 
 def _not_null(value, field):
```

### Comparing `clickzetta-connector-0.8.5/clickzetta/bulkload/bulkload_enums.py` & `clickzetta-connector-0.8.7/clickzetta/bulkload/bulkload_enums.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/bulkload/bulkload_stream.py` & `clickzetta-connector-0.8.7/clickzetta/bulkload/bulkload_stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             sql_error_msg = current_stream.get_sql_error()
             _logger.info(
                 "Get BulkLoadStream:" + self.meta_data.get_stream_id() + ", state:" + state.name + ",time:" + str(
                     try_time))
             if state == BulkLoadState.COMMIT_SUCCESS or state == BulkLoadState.COMMIT_FAILED:
                 break
             else:
-                time.sleep(10)
+                time.sleep(2)
         if state != BulkLoadState.COMMIT_SUCCESS:
             _logger.error(
                 "BulkLoadStream:" + self.get_stream_id() + " sync commit failed or timeout with state:" + state.name
                 + " with error:" + sql_error_msg)
             raise IOError(
                 "BulkLoadStream:" + self.get_stream_id() + " sync commit failed or timeout with state:" + state.name
                 + " with error:" + sql_error_msg)
```

### Comparing `clickzetta-connector-0.8.5/clickzetta/bulkload/bulkload_writer.py` & `clickzetta-connector-0.8.7/clickzetta/bulkload/bulkload_writer.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/client.py` & `clickzetta-connector-0.8.7/clickzetta/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from __future__ import absolute_import
 from __future__ import division
 
 import time
 
 import clickzetta
-import sqlalchemy
+from sqlalchemy.engine.url import make_url
 import json
 import random
 import os
 import requests.exceptions
 import typing
 from typing import (
     Any,
@@ -63,66 +63,66 @@
 }
 
 DEFAULT_INSTANCE_ID = 100
 
 
 class Client(object):
 
-    def __init__(self, login_params: LoginParams = None, workspace: str = None, instance_name: str = None,
-                 vc_name: str = None, cz_url: str = None, base_url: str = None, schema: str = None):
+    def __init__(self, username: str = None, password: str = None, instance: str = None, workspace: str = None,
+                 vcluster: str = None, cz_url: str = None, service: str = None, schema: str = None):
         if cz_url is not None:
             self._parse_url(cz_url)
-            self.token = self.log_in_cz(self.login_params)
+            self.token = self.log_in_cz(username, password, instance)
             self.instance_id = 0
         else:
-            default_base_url = _get_click_zetta_host()
-            if base_url is None:
-                self.base_url = default_base_url
+            if service is None:
+                raise ValueError('ClickZetta connection url `service` is required.')
             else:
-                self.base_url = base_url
+                self.service = service
             self.token = None
             self.workspace = workspace
-            self.instance_name = instance_name
-            self.vc_name = vc_name
-            self.login_params = login_params
+            self.instance = instance
+            self.vcluster = vcluster
             self.session = None
             self.instance_id = 0
-            self.username = login_params.username
+            self.username = username
             self.schema = schema
+            self.password = password
 
     def _parse_url(self, url: string):
-        url = sqlalchemy.make_url(url)
+        url = make_url(url)
         query = dict(url.query)
 
-        self.instance_name = url.host.split('.')[0]
-        length = len(self.instance_name) + 1
+        self.instance = url.host.split('.')[0]
+        length = len(self.instance) + 1
 
-        self.base_url = 'https://' + url.host[length:]
+        self.service = 'https://' + url.host[length:]
         self.workspace = url.database
         self.username = url.username
-        pwd = url.password
+        self.password = url.password
 
-        if 'virtualcluster' in query or 'virtualCluster' in query:
+        if 'virtualcluster' in query or 'virtualCluster' in query or 'vcluster' in query:
             if 'virtualcluster' in query:
-                self.vc_name = query.pop('virtualcluster')
+                self.vcluster = query.pop('virtualcluster')
             elif 'virtualCluster' in query:
-                self.vc_name = query.pop('virtualCluster')
+                self.vcluster = query.pop('virtualCluster')
+            else:
+                self.vcluster = query.pop('vcluster')
         else:
-            raise ValueError('url must have `virtualcluster` parameter.')
+            raise ValueError('url must have `virtualcluster` or `virtualCluster` or `vcluster` parameter.')
         if 'schema' in query:
             self.schema = query.pop('schema')
 
-        self.login_params = LoginParams(self.username, pwd, self.instance_name)
-
-    def log_in_cz(self, login_params: LoginParams) -> str:
+    def log_in_cz(self, username: str, password: str, instance: str) -> str:
         path = "/clickzetta-portal/user/loginSingle"
+        login_params = LoginParams(username, password, instance)
         api_repr = login_params.to_api_repr()
         data = json.dumps(api_repr)
         try:
-            api_response = requests.post(self.base_url + path, data=data, headers=HEADERS)
+            api_response = requests.post(self.service + path, data=data, headers=HEADERS)
             result = api_response.text
             result_dict = json.loads(result)
             if result_dict['data']['token'] is None:
                 raise requests.exceptions.RequestException("user:" + login_params.username + "is Unauthorized")
             else:
                 token = result_dict['data']['token']
                 return token
@@ -182,15 +182,15 @@
         table_identifier.instance_id = instance_id
         table_identifier.workspace = workspace
         table_identifier.schema_name = schema_name
         table_identifier.table_name = table_name
         commit_bulkload_request.identifier.CopyFrom(table_identifier)
         commit_bulkload_request.stream_id = stream_id
         commit_bulkload_request.execute_workspace = execute_workspace
-        commit_bulkload_request.execute_vc_name = execute_vc
+        commit_bulkload_request.execute_vcluster = execute_vc
         if commit_mode == BulkLoadCommitMode.COMMIT_STREAM:
             commit_bulkload_request.commit_mode = ingestion_pb2.CommitBulkLoadStreamRequest.CommitMode.COMMIT_STREAM
         elif commit_mode == BulkLoadCommitMode.ABORT_STREAM:
             commit_bulkload_request.commit_mode = ingestion_pb2.CommitBulkLoadStreamRequest.CommitMode.ABORT_STREAM
 
         response = self._gate_way_call(commit_bulkload_request, ingestion_pb2.MethodEnum.COMMIT_BULK_LOAD_STREAM_V2)
         response_pb = ParseDict(response, ingestion_pb2.CommitBulkLoadStreamResponse())
@@ -275,18 +275,18 @@
 
     def _gate_way_call(self, request, method: ingestion_pb2.MethodEnum):
         path = '/igs/gatewayEndpoint'
         gate_way_request = ingestion_pb2.GatewayRequest()
         gate_way_request.methodEnumValue = method
         gate_way_request.message = MessageToJson(request)
 
-        HEADERS['instanceName'] = self.instance_name
+        HEADERS['instanceName'] = self.instance
         HEADERS['X-ClickZetta-Token'] = self.token
         try:
-            api_response = requests.post(self.base_url + path, data=MessageToJson(gate_way_request), headers=HEADERS)
+            api_response = requests.post(self.service + path, data=MessageToJson(gate_way_request), headers=HEADERS)
             result = api_response.text
             result_dict = json.loads(result)
             if api_response.status_code != 200:
                 raise requests.exceptions.RequestException(
                     'gate_way_call return failed code.Error message:' + result_dict['message'])
             result_status = ParseDict(result_dict['status'], ingestion_pb2.GateWayResponseStatus)
             if result_status.code == ingestion_pb2.Code.SUCCESS:
@@ -310,16 +310,16 @@
             raise requests.exceptions.RequestException(
                 'gate_way_request error:{}'.format(e))
 
     def submit_sql_job(self, token: str, sql: str, parameters=None, schema=None) -> QueryResult:
         path = "/lh/submitJob"
         if 'test plain returns' in sql or 'test unicode returns' in sql:
             return QueryResult({})
-        table = Table(self.workspace, '', self.instance_name, self.vc_name)
-        vc = table.vc_name
+        table = Table(self.workspace, '', self.instance, self.vcluster)
+        vc = table.vcluster
         job_type = JobType.SQL_JOB
         format_unique_id = self._format_job_id()
         job_id = JobID(format_unique_id, table.workspace, DEFAULT_INSTANCE_ID)
         logging.info(
             "python sqlalchemy job id:" + format_unique_id)
         job_name = "SQL_JOB"
         user_id = 0
@@ -343,19 +343,19 @@
         user_agent = ""
 
         job_desc = JobDesc(vc, job_type, job_id, job_name, user_id, reqeust_mode, timeout, job_config, sql_job,
                            job_timeout_ms,
                            user_agent, 0)
         job_request = JobRequest(job_desc)
         data = json.dumps(job_request.to_api_repr())
-        HEADERS['instanceName'] = table.instance_name
+        HEADERS['instanceName'] = table.instance
         HEADERS['X-ClickZetta-Token'] = token
         logging.debug('BEGIN TO SEND REQUEST:' + sql + ' TO CZ SERVER, TIME:' + str(datetime.now()))
         try:
-            api_response = self.session.post(self.base_url + path, data=data, headers=HEADERS)
+            api_response = self.session.post(self.service + path, data=data, headers=HEADERS)
             api_response.encoding = 'utf-8'
             result = api_response.text
             result_dict = json.loads(result)
             get_job_result_dict = self.wait_job_finished(result_dict, job_id, HEADERS)
             logging.debug('GET RESPONSE FROM CZ SERVER FOR REQUEST:' + sql + ' TIME:' + str(datetime.now()))
             query_result = QueryResult(get_job_result_dict)
             return query_result
@@ -372,15 +372,15 @@
                 if status == "QUEUEING" or status == "SETUP" or status == "RUNNING":
                     account = clickzetta.enums.ClickZettaAccount(0)
                     get_job_result_request = clickzetta.enums.GetJobResultRequest(account, job_id, 0, '')
                     api_request = clickzetta.enums.APIJobRequest(get_job_result_request, '')
                     path = '/lh/getJob'
                     data = json.dumps(api_request.to_api_repr())
                     while True:
-                        get_job_result_response = self.session.post(self.base_url + path, data=data, headers=headers)
+                        get_job_result_response = self.session.post(self.service + path, data=data, headers=headers)
                         result = get_job_result_response.text
                         get_job_result_dict = json.loads(result)
                         if 'status' in get_job_result_dict:
                             if 'state' in get_job_result_dict['status']:
                                 if get_job_result_dict['status']['state'] == 'SUCCEED' or \
                                         get_job_result_dict['status']['state'] == 'FAILED':
                                     logging.info(
```

### Comparing `clickzetta-connector-0.8.5/clickzetta/dbapi/__init__.py` & `clickzetta-connector-0.8.7/clickzetta/dbapi/__init__.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/dbapi/_helpers.py` & `clickzetta-connector-0.8.7/clickzetta/dbapi/_helpers.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/dbapi/connection.py` & `clickzetta-connector-0.8.7/clickzetta/dbapi/connection.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,22 +29,22 @@
             self._owns_client = True
 
         self._client = client
         current_time = int(time.time())
         unique_key = self._client.login_params.username + "?" + self._client.login_params.instance_name
         if globals()['user_token_dict'].__contains__(unique_key):
             if current_time - globals()['user_token_time_dict'][unique_key] > 24 * 60 * 60:
-                new_token = self._client.log_in_cz(self._client.login_params)
+                new_token = self._client.log_in_cz(self._client.username, self._client.password, self._client.instance)
                 globals()['user_token_dict'][unique_key] = new_token
                 globals()['user_token_time_dict'][unique_key] = current_time
                 self._client.token = new_token
             else:
                 self._client.token = globals()['user_token_dict'][unique_key]
         else:
-            new_token = self._client.log_in_cz(self._client.login_params)
+            new_token = self._client.log_in_cz(self._client.username, self._client.password, self._client.instance)
             globals()['user_token_dict'][unique_key] = new_token
             globals()['user_token_time_dict'][unique_key] = current_time
             self._client.token = new_token
 
         if not globals()['https_session_inited']:
             session = requests.Session()
             session.mount(self._client.base_url, HTTPAdapter(pool_connections=20, pool_maxsize=100, max_retries=1000))
```

### Comparing `clickzetta-connector-0.8.5/clickzetta/dbapi/cursor.py` & `clickzetta-connector-0.8.7/clickzetta/dbapi/cursor.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/dbapi/exceptions.py` & `clickzetta-connector-0.8.7/clickzetta/dbapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/dbapi/types.py` & `clickzetta-connector-0.8.7/clickzetta/dbapi/types.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/enums.py` & `clickzetta-connector-0.8.7/clickzetta/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,19 +188,19 @@
         self._properties = {"jobDesc": job_desc.to_api_repr()}
 
     def to_api_repr(self) -> dict:
         return copy.deepcopy(self._properties)
 
 
 class LoginParams(object):
-    def __init__(self, username: string, password: string, instance_name: string):
+    def __init__(self, username: string, password: string, instance: string):
         self.username = username
         self.password = password
-        self.instance_name = instance_name
-        self._properties = {"username": username, "password": password, "instanceName": instance_name}
+        self.instance = instance
+        self._properties = {"username": username, "password": password, "instanceName": instance}
 
     def to_api_repr(self) -> dict:
         return copy.deepcopy(self._properties)
 
 
 class ErrorStatus(object):
     Unauthorized = "UNAUTHORIZED"
```

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/generated/account_pb2.py` & `clickzetta-connector-0.8.7/clickzetta/proto/generated/account_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/generated/block_bloom_filter_pb2.py` & `clickzetta-connector-0.8.7/clickzetta/proto/generated/block_bloom_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/generated/bucket_info_pb2.py` & `clickzetta-connector-0.8.7/clickzetta/proto/generated/bucket_info_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/generated/compression_pb2.py` & `clickzetta-connector-0.8.7/clickzetta/proto/generated/compression_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/generated/connection_meta_pb2.py` & `clickzetta-connector-0.8.7/clickzetta/proto/generated/connection_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/generated/data_type_pb2.py` & `clickzetta-connector-0.8.7/clickzetta/proto/generated/data_type_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/generated/expression_pb2.py` & `clickzetta-connector-0.8.7/clickzetta/proto/generated/expression_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/generated/file_format_type_pb2.py` & `clickzetta-connector-0.8.7/clickzetta/proto/generated/file_format_type_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/generated/file_meta_data_pb2.py` & `clickzetta-connector-0.8.7/clickzetta/proto/generated/file_meta_data_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/generated/file_system_pb2.py` & `clickzetta-connector-0.8.7/clickzetta/proto/generated/file_system_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/generated/function_meta_pb2.py` & `clickzetta-connector-0.8.7/clickzetta/proto/generated/function_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/generated/hash_pb2.py` & `clickzetta-connector-0.8.7/clickzetta/proto/generated/hash_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/generated/ingestion_pb2.py` & `clickzetta-connector-0.8.7/clickzetta/proto/generated/ingestion_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/generated/ingestion_pb2_grpc.py` & `clickzetta-connector-0.8.7/clickzetta/proto/generated/ingestion_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/generated/input_split_pb2.py` & `clickzetta-connector-0.8.7/clickzetta/proto/generated/input_split_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/generated/job_meta_pb2.py` & `clickzetta-connector-0.8.7/clickzetta/proto/generated/job_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/generated/job_result_cache_meta_pb2.py` & `clickzetta-connector-0.8.7/clickzetta/proto/generated/job_result_cache_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/generated/kudu_common_pb2.py` & `clickzetta-connector-0.8.7/clickzetta/proto/generated/kudu_common_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/generated/metadata_entity_pb2.py` & `clickzetta-connector-0.8.7/clickzetta/proto/generated/metadata_entity_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/generated/network_policy_pb2.py` & `clickzetta-connector-0.8.7/clickzetta/proto/generated/network_policy_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/generated/object_identifier_pb2.py` & `clickzetta-connector-0.8.7/clickzetta/proto/generated/object_identifier_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/generated/operator_pb2.py` & `clickzetta-connector-0.8.7/clickzetta/proto/generated/operator_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/generated/pb_util_pb2.py` & `clickzetta-connector-0.8.7/clickzetta/proto/generated/pb_util_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/generated/property_pb2.py` & `clickzetta-connector-0.8.7/clickzetta/proto/generated/property_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/generated/rm_app_meta_pb2.py` & `clickzetta-connector-0.8.7/clickzetta/proto/generated/rm_app_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/generated/role_meta_pb2.py` & `clickzetta-connector-0.8.7/clickzetta/proto/generated/role_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/generated/row_operations_pb2.py` & `clickzetta-connector-0.8.7/clickzetta/proto/generated/row_operations_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/generated/schema_pb2.py` & `clickzetta-connector-0.8.7/clickzetta/proto/generated/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/generated/share_meta_pb2.py` & `clickzetta-connector-0.8.7/clickzetta/proto/generated/share_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/generated/statistics_pb2.py` & `clickzetta-connector-0.8.7/clickzetta/proto/generated/statistics_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/generated/table_common_pb2.py` & `clickzetta-connector-0.8.7/clickzetta/proto/generated/table_common_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/generated/table_meta_pb2.py` & `clickzetta-connector-0.8.7/clickzetta/proto/generated/table_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/generated/virtual_cluster_meta_pb2.py` & `clickzetta-connector-0.8.7/clickzetta/proto/generated/virtual_cluster_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/generated/virtual_cluster_pb2.py` & `clickzetta-connector-0.8.7/clickzetta/proto/generated/virtual_cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/generated/virtual_cluster_size_pb2.py` & `clickzetta-connector-0.8.7/clickzetta/proto/generated/virtual_cluster_size_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/generated/virtual_value_info_pb2.py` & `clickzetta-connector-0.8.7/clickzetta/proto/generated/virtual_value_info_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/generated/workspace_meta_pb2.py` & `clickzetta-connector-0.8.7/clickzetta/proto/generated/workspace_meta_pb2.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/source/account.proto` & `clickzetta-connector-0.8.7/clickzetta/proto/source/account.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/source/block_bloom_filter.proto` & `clickzetta-connector-0.8.7/clickzetta/proto/source/block_bloom_filter.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/source/compression.proto` & `clickzetta-connector-0.8.7/clickzetta/proto/source/compression.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/source/data_type.proto` & `clickzetta-connector-0.8.7/clickzetta/proto/source/data_type.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/source/expression.proto` & `clickzetta-connector-0.8.7/clickzetta/proto/source/expression.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/source/file_meta_data.proto` & `clickzetta-connector-0.8.7/clickzetta/proto/source/file_meta_data.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/source/function_meta.proto` & `clickzetta-connector-0.8.7/clickzetta/proto/source/function_meta.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/source/hash.proto` & `clickzetta-connector-0.8.7/clickzetta/proto/source/hash.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/source/ingestion.proto` & `clickzetta-connector-0.8.7/clickzetta/proto/source/ingestion.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/source/input_split.proto` & `clickzetta-connector-0.8.7/clickzetta/proto/source/input_split.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/source/job_meta.proto` & `clickzetta-connector-0.8.7/clickzetta/proto/source/job_meta.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/source/kudu_common.proto` & `clickzetta-connector-0.8.7/clickzetta/proto/source/kudu_common.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/source/metadata_entity.proto` & `clickzetta-connector-0.8.7/clickzetta/proto/source/metadata_entity.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/source/object_identifier.proto` & `clickzetta-connector-0.8.7/clickzetta/proto/source/object_identifier.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/source/operator.proto` & `clickzetta-connector-0.8.7/clickzetta/proto/source/operator.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/source/pb_util.proto` & `clickzetta-connector-0.8.7/clickzetta/proto/source/pb_util.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/source/rm_app_meta.proto` & `clickzetta-connector-0.8.7/clickzetta/proto/source/rm_app_meta.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/source/row_operations.proto` & `clickzetta-connector-0.8.7/clickzetta/proto/source/row_operations.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/source/statistics.proto` & `clickzetta-connector-0.8.7/clickzetta/proto/source/statistics.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/source/table_common.proto` & `clickzetta-connector-0.8.7/clickzetta/proto/source/table_common.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/source/table_meta.proto` & `clickzetta-connector-0.8.7/clickzetta/proto/source/table_meta.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/source/virtual_cluster.proto` & `clickzetta-connector-0.8.7/clickzetta/proto/source/virtual_cluster.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/source/virtual_cluster_meta.proto` & `clickzetta-connector-0.8.7/clickzetta/proto/source/virtual_cluster_meta.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/proto/source/virtual_value_info.proto` & `clickzetta-connector-0.8.7/clickzetta/proto/source/virtual_value_info.proto`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/query_result.py` & `clickzetta-connector-0.8.7/clickzetta/query_result.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/schema.py` & `clickzetta-connector-0.8.7/clickzetta/schema.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/session.py` & `clickzetta-connector-0.8.7/clickzetta/session.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/standard_sql.py` & `clickzetta-connector-0.8.7/clickzetta/standard_sql.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta/table.py` & `clickzetta-connector-0.8.7/clickzetta/table.py`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta_connector.egg-info/SOURCES.txt` & `clickzetta-connector-0.8.7/clickzetta_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/clickzetta_connector.egg-info/requires.txt` & `clickzetta-connector-0.8.7/clickzetta_connector.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `clickzetta-connector-0.8.5/setup.py` & `clickzetta-connector-0.8.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import io
 import os
-import shutil
 import platform
 import subprocess
 
 import setuptools
 
 PROJECT_SRC_DIR = os.path.abspath(os.path.join(os.getcwd(), "../../.."))
 CURRENT_DIR = os.path.abspath(os.path.dirname(__file__))
 PROTO_DIR = os.path.abspath(os.path.join(CURRENT_DIR, "clickzetta/proto/source"))
 PROTO_OUT_DIR = os.path.abspath(os.path.join(CURRENT_DIR, "clickzetta/proto/generated"))
 
+os.makedirs(PROTO_OUT_DIR, exist_ok=True)
+
 for source_file in os.listdir(PROTO_DIR):
     subprocess.call(
         'python -m grpc_tools.protoc -I . --python_out=' + PROTO_OUT_DIR + ' --grpc_python_out=' + PROTO_OUT_DIR
         + ' --proto_path =' + PROTO_DIR + ' '
         + os.path.abspath(os.path.join(PROTO_DIR, source_file)), shell=True)
 
 for generated_file in os.listdir(PROTO_OUT_DIR):
```

