# Comparing `tmp/pinecone-client-2.2.2rc3.tar.gz` & `tmp/pinecone_client-3.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinecone-client-2.2.2rc3.tar", last modified: Mon Jun  5 23:17:38 2023, max compression
+gzip compressed data
```

## Comparing `pinecone-client-2.2.2rc3.tar` & `pinecone_client-3.0.0rc2.tar`

### file list

```diff
@@ -1,90 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:17:38.874214 pinecone-client-2.2.2rc3/
--rw-r--r--   0 runner    (1001) docker     (123)    12723 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-06-05 23:17:38.874214 pinecone-client-2.2.2rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:17:38.866213 pinecone-client-2.2.2rc3/pinecone/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/__environment__
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/__version__
--rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:17:38.866213 pinecone-client-2.2.2rc3/pinecone/core/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/api_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/api_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:17:38.866213 pinecone-client-2.2.2rc3/pinecone/core/client/
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:17:38.866213 pinecone-client-2.2.2rc3/pinecone/core/client/api/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43961 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/client/api/index_operations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    38289 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/client/api/vector_operations_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    36997 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/client/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:17:38.866213 pinecone-client-2.2.2rc3/pinecone/core/client/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/client/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17845 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:17:38.870214 pinecone-client-2.2.2rc3/pinecone/core/client/model/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/client/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11635 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/client/model/approximated_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11698 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/client/model/collection_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    11707 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/client/model/create_collection_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    16268 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/client/model/create_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12916 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/client/model/delete_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11755 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/client/model/describe_index_stats_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12954 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/client/model/describe_index_stats_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11664 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/client/model/fetch_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12242 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/client/model/hnsw_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11441 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/client/model/index_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    13694 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/client/model/index_meta_database.py
--rw-r--r--   0 runner    (1001) docker     (123)    11641 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/client/model/index_meta_database_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    11786 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/client/model/index_meta_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    11571 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/client/model/namespace_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/client/model/patch_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/client/model/protobuf_any.py
--rw-r--r--   0 runner    (1001) docker     (123)    12416 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/client/model/protobuf_null_value.py
--rw-r--r--   0 runner    (1001) docker     (123)    15518 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/client/model/query_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    12307 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/client/model/query_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    13273 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/client/model/query_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)    11770 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/client/model/rpc_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/client/model/scored_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)    11760 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/client/model/single_query_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    11562 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/client/model/sparse_values.py
--rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/client/model/update_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11947 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/client/model/upsert_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11309 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/client/model/upsert_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12705 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/client/model/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)    80289 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/client/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:17:38.870214 pinecone-client-2.2.2rc3/pinecone/core/client/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12819 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/client/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:17:38.874214 pinecone-client-2.2.2rc3/pinecone/core/grpc/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37787 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/grpc/index_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:17:38.874214 pinecone-client-2.2.2rc3/pinecone/core/grpc/protos/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/grpc/protos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34942 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/grpc/protos/vector_column_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9908 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/grpc/protos/vector_column_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    57479 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/grpc/protos/vector_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/grpc/protos/vector_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/grpc/retry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:17:38.874214 pinecone-client-2.2.2rc3/pinecone/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/core/utils/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    30364 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     9465 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pinecone/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 23:17:38.874214 pinecone-client-2.2.2rc3/pinecone_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-06-05 23:17:38.000000 pinecone-client-2.2.2rc3/pinecone_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-06-05 23:17:38.000000 pinecone-client-2.2.2rc3/pinecone_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 23:17:38.000000 pinecone-client-2.2.2rc3/pinecone_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-05 23:17:38.000000 pinecone-client-2.2.2rc3/pinecone_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-05 23:17:38.000000 pinecone-client-2.2.2rc3/pinecone_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-05 23:17:38.000000 pinecone-client-2.2.2rc3/pinecone_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/requirements-grpc.txt
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-05 23:17:38.874214 pinecone-client-2.2.2rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-06-05 23:17:33.000000 pinecone-client-2.2.2rc3/setup.py
+-rw-r--r--   0        0        0      479 1970-01-01 00:00:00.000000 pinecone_client-3.0.0rc2/local_dependencies/index_service/Cargo.toml
+-rw-r--r--   0     1001      123     2738 2023-04-03 16:53:40.000000 pinecone_client-3.0.0rc2/local_dependencies/index_service/README.md
+-rw-r--r--   0     1001      123     1033 2023-04-03 16:53:40.000000 pinecone_client-3.0.0rc2/local_dependencies/index_service/build.rs
+-rw-r--r--   0     1001      123      157 2023-04-03 16:53:41.000000 pinecone_client-3.0.0rc2/local_dependencies/index_service/src/lib.rs
+-rw-r--r--   0        0        0      866 1970-01-01 00:00:00.000000 pinecone_client-3.0.0rc2/local_dependencies/client_sdk/Cargo.toml
+-rw-r--r--   0     1001      123      981 2023-04-03 16:53:40.000000 pinecone_client-3.0.0rc2/local_dependencies/client_sdk/build.rs
+-rw-r--r--   0     1001      123    10137 2023-04-03 16:53:40.000000 pinecone_client-3.0.0rc2/local_dependencies/client_sdk/src/client/control_plane.rs
+-rw-r--r--   0     1001      123    11914 2023-04-03 16:53:40.000000 pinecone_client-3.0.0rc2/local_dependencies/client_sdk/src/client/grpc.rs
+-rw-r--r--   0     1001      123       58 2023-04-03 16:53:40.000000 pinecone_client-3.0.0rc2/local_dependencies/client_sdk/src/client/mod.rs
+-rw-r--r--   0     1001      123     9139 2023-04-03 16:53:40.000000 pinecone_client-3.0.0rc2/local_dependencies/client_sdk/src/client/pinecone_client.rs
+-rw-r--r--   0     1001      123     8765 2023-04-03 16:53:40.000000 pinecone_client-3.0.0rc2/local_dependencies/client_sdk/src/data_types.rs
+-rw-r--r--   0     1001      123     9041 2023-04-03 16:53:40.000000 pinecone_client-3.0.0rc2/local_dependencies/client_sdk/src/index.rs
+-rw-r--r--   0     1001      123       66 2023-04-03 16:53:40.000000 pinecone_client-3.0.0rc2/local_dependencies/client_sdk/src/lib.rs
+-rw-r--r--   0     1001      123     8428 2023-04-03 16:53:40.000000 pinecone_client-3.0.0rc2/local_dependencies/client_sdk/src/proto/vector_service.proto
+-rw-r--r--   0     1001      123     9898 2023-04-03 16:53:40.000000 pinecone_client-3.0.0rc2/local_dependencies/client_sdk/src/utils/conversions.rs
+-rw-r--r--   0     1001      123     3817 2023-04-03 16:53:40.000000 pinecone_client-3.0.0rc2/local_dependencies/client_sdk/src/utils/errors.rs
+-rw-r--r--   0     1001      123       65 2023-04-03 16:53:40.000000 pinecone_client-3.0.0rc2/local_dependencies/client_sdk/src/utils/mod.rs
+-rw-r--r--   0     1001      123     8328 2023-04-03 16:53:40.000000 pinecone_client-3.0.0rc2/local_dependencies/client_sdk/src/utils/python_conversions.rs
+-rw-r--r--   0        0        0      539 1970-01-01 00:00:00.000000 pinecone_client-3.0.0rc2/Cargo.toml
+-rw-r--r--   0     1001      123      685 2023-04-03 16:53:40.000000 pinecone_client-3.0.0rc2/.gitignore
+-rw-r--r--   0        0        0  2827950 2023-04-03 16:55:28.000000 pinecone_client-3.0.0rc2/protoc-22.2-linux-x86_64.zip
+-rw-r--r--   0     1001      123     1383 2023-04-03 16:53:40.000000 pinecone_client-3.0.0rc2/pyproject.toml
+-rw-r--r--   0     1001      123    10608 2023-04-03 16:53:40.000000 pinecone_client-3.0.0rc2/src/client.rs
+-rw-r--r--   0     1001      123     2514 2023-04-03 16:53:40.000000 pinecone_client-3.0.0rc2/src/data_types.rs
+-rw-r--r--   0     1001      123    15027 2023-04-03 16:53:40.000000 pinecone_client-3.0.0rc2/src/index.rs
+-rw-r--r--   0     1001      123      760 2023-04-03 16:53:40.000000 pinecone_client-3.0.0rc2/src/lib.rs
+-rw-r--r--   0     1001      123     3093 2023-04-03 16:53:40.000000 pinecone_client-3.0.0rc2/src/utils/errors.rs
+-rw-r--r--   0     1001      123       16 2023-04-03 16:53:40.000000 pinecone_client-3.0.0rc2/src/utils/mod.rs
+-rw-r--r--   0        0        0    55939 2023-04-03 16:56:33.000000 pinecone_client-3.0.0rc2/Cargo.lock
+-rw-r--r--   0        0        0     1455 1970-01-01 00:00:00.000000 pinecone_client-3.0.0rc2/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

