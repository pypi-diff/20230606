# Comparing `tmp/hiku-0.7.0rc8.tar.gz` & `tmp/hiku-0.7.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hiku-0.7.0rc8.tar", last modified: Wed Aug 24 15:35:55 2022, max compression
+gzip compressed data, was "dist/hiku-0.7.0rc9.tar", last modified: Sat Oct  1 16:41:52 2022, max compression
```

## Comparing `hiku-0.7.0rc8.tar` & `hiku-0.7.0rc9.tar`

### file list

```diff
@@ -1,91 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 15:35:55.000000 hiku-0.7.0rc8/
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4812 2022-08-24 15:35:55.000000 hiku-0.7.0rc8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3036 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 15:35:55.000000 hiku-0.7.0rc8/hiku/
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2228 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/builder.py
--rw-r--r--   0 runner    (1001) docker     (121)      942 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 15:35:55.000000 hiku-0.7.0rc8/hiku/denormalize/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/denormalize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2572 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/denormalize/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1374 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/denormalize/graphql.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 15:35:55.000000 hiku-0.7.0rc8/hiku/directives/
--rw-r--r--   0 runner    (1001) docker     (121)      671 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/directives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10249 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/edn.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 15:35:55.000000 hiku-0.7.0rc8/hiku/endpoint/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/endpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6318 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/endpoint/graphql.py
--rw-r--r--   0 runner    (1001) docker     (121)    19160 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 15:35:55.000000 hiku-0.7.0rc8/hiku/executors/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1524 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/executors/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (121)      826 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/executors/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2676 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/executors/queue.py
--rw-r--r--   0 runner    (1001) docker     (121)      840 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/executors/sync.py
--rw-r--r--   0 runner    (1001) docker     (121)      847 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/executors/threads.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 15:35:55.000000 hiku-0.7.0rc8/hiku/export/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2353 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/export/graphql.py
--rw-r--r--   0 runner    (1001) docker     (121)      918 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/export/protobuf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1135 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/export/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 15:35:55.000000 hiku-0.7.0rc8/hiku/expr/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/expr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6186 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/expr/checker.py
--rw-r--r--   0 runner    (1001) docker     (121)     5493 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/expr/compiler.py
--rw-r--r--   0 runner    (1001) docker     (121)     6224 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/expr/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     3131 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/expr/nodes.py
--rw-r--r--   0 runner    (1001) docker     (121)     4437 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/expr/refs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 15:35:55.000000 hiku-0.7.0rc8/hiku/federation/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/federation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      438 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/federation/denormalize.py
--rw-r--r--   0 runner    (1001) docker     (121)     1490 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/federation/directive.py
--rw-r--r--   0 runner    (1001) docker     (121)     6216 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/federation/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (121)     2680 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/federation/engine.py
--rw-r--r--   0 runner    (1001) docker     (121)     6061 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/federation/introspection.py
--rw-r--r--   0 runner    (1001) docker     (121)     8819 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/federation/sdl.py
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/federation/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/federation/validate.py
--rw-r--r--   0 runner    (1001) docker     (121)    20614 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 15:35:55.000000 hiku-0.7.0rc8/hiku/introspection/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/introspection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    26266 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/introspection/graphql.py
--rw-r--r--   0 runner    (1001) docker     (121)     1202 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/introspection/types.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 15:35:55.000000 hiku-0.7.0rc8/hiku/protobuf/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/protobuf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      380 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/protobuf/query.proto
--rw-r--r--   0 runner    (1001) docker     (121)     8068 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/protobuf/query_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)     7421 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/query.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 15:35:55.000000 hiku-0.7.0rc8/hiku/readers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15841 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/readers/graphql.py
--rw-r--r--   0 runner    (1001) docker     (121)     2238 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/readers/protobuf.py
--rw-r--r--   0 runner    (1001) docker     (121)     2759 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/readers/simple.py
--rw-r--r--   0 runner    (1001) docker     (121)     6556 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/result.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 15:35:55.000000 hiku-0.7.0rc8/hiku/sources/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2085 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/sources/aiopg.py
--rw-r--r--   0 runner    (1001) docker     (121)     5586 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/sources/graph.py
--rw-r--r--   0 runner    (1001) docker     (121)     6298 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/sources/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1697 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/sources/sqlalchemy_async.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 15:35:55.000000 hiku-0.7.0rc8/hiku/telemetry/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/telemetry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6005 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/telemetry/prometheus.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 15:35:55.000000 hiku-0.7.0rc8/hiku/typedef/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/typedef/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4364 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/typedef/kinko.py
--rw-r--r--   0 runner    (1001) docker     (121)      271 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/typedef/types.py
--rw-r--r--   0 runner    (1001) docker     (121)     8656 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/types.py
--rw-r--r--   0 runner    (1001) docker     (121)      920 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 15:35:55.000000 hiku-0.7.0rc8/hiku/validate/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/validate/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     6452 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/validate/graph.py
--rw-r--r--   0 runner    (1001) docker     (121)    13308 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/hiku/validate/query.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 15:35:55.000000 hiku-0.7.0rc8/hiku.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4812 2022-08-24 15:35:54.000000 hiku-0.7.0rc8/hiku.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1678 2022-08-24 15:35:54.000000 hiku-0.7.0rc8/hiku.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-24 15:35:54.000000 hiku-0.7.0rc8/hiku.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-08-24 15:35:54.000000 hiku-0.7.0rc8/hiku.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-24 15:35:55.000000 hiku-0.7.0rc8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1429 2022-08-24 15:35:29.000000 hiku-0.7.0rc8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-01 16:41:52.000000 hiku-0.7.0rc9/
+-rw-r--r--   0 runner    (1001) docker     (121)      147 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     4812 2022-10-01 16:41:52.000000 hiku-0.7.0rc9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3036 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-01 16:41:52.000000 hiku-0.7.0rc9/hiku/
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2228 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/builder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3799 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)      942 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-01 16:41:52.000000 hiku-0.7.0rc9/hiku/denormalize/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/denormalize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2572 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/denormalize/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1374 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/denormalize/graphql.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-01 16:41:52.000000 hiku-0.7.0rc9/hiku/directives/
+-rw-r--r--   0 runner    (1001) docker     (121)      887 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/directives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10249 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/edn.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-01 16:41:52.000000 hiku-0.7.0rc9/hiku/endpoint/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/endpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6318 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/endpoint/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24077 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-01 16:41:52.000000 hiku-0.7.0rc9/hiku/executors/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1524 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/executors/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (121)      826 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/executors/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2676 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/executors/queue.py
+-rw-r--r--   0 runner    (1001) docker     (121)      866 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/executors/sync.py
+-rw-r--r--   0 runner    (1001) docker     (121)      847 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/executors/threads.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-01 16:41:52.000000 hiku-0.7.0rc9/hiku/export/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2353 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/export/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (121)      918 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/export/protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1135 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/export/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-01 16:41:52.000000 hiku-0.7.0rc9/hiku/expr/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/expr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6186 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/expr/checker.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5493 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/expr/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6224 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/expr/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3131 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/expr/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4437 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/expr/refs.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-01 16:41:52.000000 hiku-0.7.0rc9/hiku/federation/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/federation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      438 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/federation/denormalize.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1490 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/federation/directive.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6216 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/federation/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2716 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/federation/engine.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6061 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/federation/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8819 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/federation/sdl.py
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/federation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      354 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/federation/validate.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20614 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-01 16:41:52.000000 hiku-0.7.0rc9/hiku/introspection/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/introspection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26733 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/introspection/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1202 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/introspection/types.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-01 16:41:52.000000 hiku-0.7.0rc9/hiku/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/protobuf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      380 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/protobuf/query.proto
+-rw-r--r--   0 runner    (1001) docker     (121)     8068 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/protobuf/query_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8281 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/query.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-01 16:41:52.000000 hiku-0.7.0rc9/hiku/readers/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17396 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/readers/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2238 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/readers/protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2759 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/readers/simple.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6684 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/result.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-01 16:41:52.000000 hiku-0.7.0rc9/hiku/sources/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2085 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/sources/aiopg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5629 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/sources/graph.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6298 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/sources/sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1697 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/sources/sqlalchemy_async.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-01 16:41:52.000000 hiku-0.7.0rc9/hiku/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/telemetry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6005 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/telemetry/prometheus.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-01 16:41:52.000000 hiku-0.7.0rc9/hiku/typedef/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/typedef/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4364 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/typedef/kinko.py
+-rw-r--r--   0 runner    (1001) docker     (121)      271 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/typedef/types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8656 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/types.py
+-rw-r--r--   0 runner    (1001) docker     (121)      965 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-01 16:41:52.000000 hiku-0.7.0rc9/hiku/validate/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      178 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/validate/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6452 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/validate/graph.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13308 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/hiku/validate/query.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-01 16:41:52.000000 hiku-0.7.0rc9/hiku.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4812 2022-10-01 16:41:52.000000 hiku-0.7.0rc9/hiku.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1692 2022-10-01 16:41:52.000000 hiku-0.7.0rc9/hiku.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-01 16:41:52.000000 hiku-0.7.0rc9/hiku.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-10-01 16:41:52.000000 hiku-0.7.0rc9/hiku.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-01 16:41:52.000000 hiku-0.7.0rc9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1429 2022-10-01 16:41:41.000000 hiku-0.7.0rc9/setup.py
```

### Comparing `hiku-0.7.0rc8/PKG-INFO` & `hiku-0.7.0rc9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiku
-Version: 0.7.0rc8
+Version: 0.7.0rc9
 Summary: Library to implement Graph APIs
 Home-page: https://github.com/evo-company/hiku
 Author: Vladimir Magamedov
 Author-email: vladimir@magamedov.com
 License: BSD-3-Clause
 Description: Hiku
         ====
```

### Comparing `hiku-0.7.0rc8/README.rst` & `hiku-0.7.0rc9/README.rst`

 * *Files identical despite different names*

### Comparing `hiku-0.7.0rc8/hiku/builder.py` & `hiku-0.7.0rc9/hiku/builder.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.0rc8/hiku/compat.py` & `hiku-0.7.0rc9/hiku/compat.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.0rc8/hiku/denormalize/base.py` & `hiku-0.7.0rc9/hiku/denormalize/base.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.0rc8/hiku/denormalize/graphql.py` & `hiku-0.7.0rc9/hiku/denormalize/graphql.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.0rc8/hiku/edn.py` & `hiku-0.7.0rc9/hiku/edn.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.0rc8/hiku/endpoint/graphql.py` & `hiku-0.7.0rc9/hiku/endpoint/graphql.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.0rc8/hiku/executors/asyncio.py` & `hiku-0.7.0rc9/hiku/executors/asyncio.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.0rc8/hiku/executors/base.py` & `hiku-0.7.0rc9/hiku/executors/base.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.0rc8/hiku/executors/queue.py` & `hiku-0.7.0rc9/hiku/executors/queue.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.0rc8/hiku/executors/sync.py` & `hiku-0.7.0rc9/hiku/executors/sync.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 class FutureLike:
 
     def __init__(self, result: T) -> None:
         self._result = result
 
-    def result(self) -> T:
+    def result(self) -> T:  # type: ignore[type-var]
         return self._result
 
 
 class SyncExecutor(BaseSyncExecutor):
 
     def submit(
         self,
```

### Comparing `hiku-0.7.0rc8/hiku/executors/threads.py` & `hiku-0.7.0rc9/hiku/executors/threads.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.0rc8/hiku/export/graphql.py` & `hiku-0.7.0rc9/hiku/export/graphql.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.0rc8/hiku/export/protobuf.py` & `hiku-0.7.0rc9/hiku/export/protobuf.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.0rc8/hiku/export/simple.py` & `hiku-0.7.0rc9/hiku/export/simple.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.0rc8/hiku/expr/checker.py` & `hiku-0.7.0rc9/hiku/expr/checker.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.0rc8/hiku/expr/compiler.py` & `hiku-0.7.0rc9/hiku/expr/compiler.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.0rc8/hiku/expr/core.py` & `hiku-0.7.0rc9/hiku/expr/core.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.0rc8/hiku/expr/nodes.py` & `hiku-0.7.0rc9/hiku/expr/nodes.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.0rc8/hiku/expr/refs.py` & `hiku-0.7.0rc9/hiku/expr/refs.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.0rc8/hiku/federation/directive.py` & `hiku-0.7.0rc9/hiku/federation/directive.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.0rc8/hiku/federation/endpoint.py` & `hiku-0.7.0rc9/hiku/federation/endpoint.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.0rc8/hiku/federation/engine.py` & `hiku-0.7.0rc9/hiku/federation/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 
     def execute_entities(
         self,
         graph: Graph,
         query: Node,
         ctx: Dict
     ) -> Union[Proxy, Awaitable[Proxy]]:
+        path = ('_entities',)
         entities_link = query.fields_map['_entities']
         query = entities_link.node
         representations = entities_link.options['representations']
 
         queue = Queue(self.executor)
         task_set = queue.fork(None)
         query_workflow = Query(queue, task_set, graph, query, Context(ctx))
@@ -61,15 +62,15 @@
                 ident = rep[key]
 
                 type_ids_map[typename].append(ident)
 
         for typename in type_ids_map:
             ids = type_ids_map[typename]
             node = graph.nodes_map[typename]
-            query_workflow.process_node(node, query, ids)
+            query_workflow.process_node(path, node, query, ids)
 
         return self.executor.process(queue, query_workflow)
 
     def execute_query(
         self,
         graph: Graph,
         query: Node,
```

### Comparing `hiku-0.7.0rc8/hiku/federation/introspection.py` & `hiku-0.7.0rc9/hiku/federation/introspection.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.0rc8/hiku/federation/sdl.py` & `hiku-0.7.0rc9/hiku/federation/sdl.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.0rc8/hiku/graph.py` & `hiku-0.7.0rc9/hiku/graph.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.0rc8/hiku/introspection/graphql.py` & `hiku-0.7.0rc9/hiku/introspection/graphql.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,14 +117,28 @@
                 name='reason',
                 type_ident=SCALAR('String'),
                 description='Deprecation reason.',
                 default_value=None,
             ),
         ],
     ),
+    # TODO: make cached directive pluggable ?
+    Directive(
+        name='cached',
+        locations=['FIELD', 'FRAGMENT_SPREAD', 'INLINE_FRAGMENT'],
+        description='Caches node and all its fields',
+        args=[
+            Directive.Argument(
+                name='ttl',
+                type_ident=NON_NULL(SCALAR('Int')),
+                description='How long field will live in cache.',
+                default_value=None,
+            ),
+        ],
+    ),
 )
 
 
 def _async_wrapper(func: t.Callable) -> t.Callable:
     async def wrapper(*args: t.Any, **kwargs: t.Any) -> t.Any:
         return func(*args, **kwargs)
     return wrapper
```

### Comparing `hiku-0.7.0rc8/hiku/introspection/types.py` & `hiku-0.7.0rc9/hiku/introspection/types.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.0rc8/hiku/protobuf/query_pb2.py` & `hiku-0.7.0rc9/hiku/protobuf/query_pb2.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.0rc8/hiku/query.py` & `hiku-0.7.0rc9/hiku/query.py`

 * *Files 13% similar despite different names*

```diff
@@ -43,17 +43,21 @@
     .. _edn: https://github.com/edn-format/edn
     .. _Datomic Pull API: http://docs.datomic.com/pull.html
     .. _om.next: https://github.com/omcljs/om/wiki/Documentation-(om.next)
 """
 import typing as t
 
 from itertools import chain
-from collections import OrderedDict
+from collections import (
+    OrderedDict,
+    defaultdict,
+)
 from collections.abc import Sequence
 
+from .directives import QueryDirective
 from .utils import cached_property
 
 T = t.TypeVar('T', bound='Base')
 
 
 def _compute_hash(obj: t.Any) -> int:
     if isinstance(obj, dict):
@@ -118,52 +122,65 @@
 class Field(FieldBase):
     """Represents a field of the node
 
     :param name: name of the field
     :param optional options: field options -- mapping of names to values
     :param optional alias: field's name in result
     """
-    __attrs__ = ('name', 'options', 'alias')
+    __attrs__ = ('name', 'options', 'alias', 'directives')
 
     def __init__(
         self,
         name: str,
         options: t.Optional[t.Dict[str, t.Any]] = None,
-        alias: t.Optional[str] = None
+        alias: t.Optional[str] = None,
+        directives: t.Optional[t.Tuple[QueryDirective, ...]] = None,
     ):
         self.name = name
         self.options = options
         self.alias = alias
+        self.directives = directives or ()
+
+    @cached_property
+    def directives_map(self) -> OrderedDict:
+        return OrderedDict((d.name, d) for d in self.directives)
 
     def accept(self, visitor: 'QueryVisitor') -> t.Any:
         return visitor.visit_field(self)
 
 
 class Link(FieldBase):
     """Represents a link to the node
 
     :param name: name of the link
     :param node: collection of fields and links --
                  :py:class:`~hiku.query.Node`
     :param optional options: link options -- mapping of names to values
     :param optional alias: link's name in result
     """
-    __attrs__ = ('name', 'node', 'options', 'alias')
+    __attrs__ = ('name', 'node', 'options', 'alias', 'directives')
 
     def __init__(
         self,
         name: str,
         node: 'Node',
         options: t.Optional[t.Dict[str, t.Any]] = None,
-        alias: t.Optional[str] = None
+        alias: t.Optional[str] = None,
+        directives: t.Optional[t.Tuple[QueryDirective, ...]] = None,
     ):
         self.name = name
         self.node = node
         self.options = options
         self.alias = alias
+        # TODO does one link can have multiple directives with same name ?
+        self.directives = directives or ()
+
+    @cached_property
+    def directives_map(self) -> OrderedDict:
+        return OrderedDict((d.name, d) for d in self.directives)
 
     def accept(self, visitor: 'QueryVisitor') -> t.Any:
         return visitor.visit_link(self)
 
 
 class Node(Base):
     """Represents collection of fields and links
@@ -194,31 +211,34 @@
     def accept(self, visitor: 'QueryVisitor') -> t.Any:
         return visitor.visit_node(self)
 
 
 def _merge(nodes: t.Iterable[Node]) -> t.Iterator[t.Union[Field, Link]]:
     fields = set()
     links = {}
+    link_directives: t.DefaultDict[t.Tuple, t.List] = defaultdict(list)
     to_merge = OrderedDict()
     for field in chain.from_iterable(e.fields for e in nodes):
         key = (field.name, field.options_hash, field.alias)
         if field.__class__ is Link:
             field = t.cast(Link, field)
             if key not in to_merge:
                 to_merge[key] = [field.node]
                 links[key] = field
             else:
                 to_merge[key].append(field.node)
+            link_directives[key].extend(field.directives)
         else:
             if key not in fields:
                 fields.add(key)
                 yield field
     for key, values in to_merge.items():
         link = links[key]
-        yield link.copy(node=merge(values))
+        directives = link_directives[key]
+        yield link.copy(node=merge(values), directives=tuple(directives))
 
 
 def merge(nodes: t.Iterable[Node]) -> Node:
     """Merges multiple queries into one query
 
     :param nodes: queries, represented as list of :py:class:`~hiku.query.Node`
     :return: merged query as one :py:class:`~hiku.query.Node`
```

### Comparing `hiku-0.7.0rc8/hiku/readers/graphql.py` & `hiku-0.7.0rc9/hiku/readers/graphql.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,18 @@
     Callable,
 )
 from functools import lru_cache
 
 from graphql.language import ast
 from graphql.language.parser import parse
 
+from ..directives import (
+    QueryDirective,
+    Cached,
+)
 from ..query import Node, Field, Link, merge
 from ..telemetry.prometheus import (
     QUERY_CACHE_HITS,
     QUERY_CACHE_MISSES,
 )
 
 
@@ -212,36 +216,78 @@
                 raise TypeError('@include directive does not accept "{}" '
                                 'argument'
                                 .format(include_arg.name.value))
             return not self.visit(include_arg.value)  # type: ignore[attr-defined] # noqa: E501
 
         return None
 
+    def _get_directive(
+        self,
+        name: str,
+        obj: ast.SelectionNode
+    ) -> Optional[ast.DirectiveNode]:
+        return next((d for d in obj.directives if d.name.value == name), None)
+
+    def _is_cached(self, obj: ast.SelectionNode) -> Optional[Cached]:
+        if not obj.directives:
+            return None
+
+        cached = self._get_directive('cached', obj)
+        if cached is None:
+            return None
+
+        if len(cached.arguments) != 1:
+            raise TypeError('@cached directive accepts exactly one '
+                            'argument, {} provided'
+                            .format(len(cached.arguments)))
+        cached_arg = cached.arguments[0]
+        if cached_arg.name.value != 'ttl':
+            raise TypeError('@cached directive does not accept "{}" '
+                            'argument'
+                            .format(cached_arg.name.value))
+        ttl = self.visit(cached_arg.value)  # type: ignore[attr-defined]
+        if not isinstance(ttl, int):
+            raise TypeError('@cached ttl argument must be an integer')
+
+        return Cached(ttl)
+
     def visit_field(
         self, obj: ast.FieldNode
     ) -> Iterator[Union[Field, Link]]:
         if self._should_skip(obj):
             return
 
+        # TODO: add plugins functionality to parse custom directives
+        directives: List[QueryDirective] = []
+        cached = self._is_cached(obj)
+        if cached is not None:
+            directives.append(cached)
+
         if obj.arguments:
             options = {arg.name.value: self.visit(arg.value)  # type: ignore[attr-defined] # noqa: E501
                        for arg in obj.arguments}
         else:
             options = None
 
         if obj.alias is not None:
             alias = obj.alias.value
         else:
             alias = None
 
         if obj.selection_set is None:
-            yield Field(obj.name.value, options=options, alias=alias)
+            yield Field(
+                obj.name.value, options=options,
+                alias=alias, directives=tuple(directives)
+            )
         else:
             node = Node(list(self.visit(obj.selection_set)))  # type: ignore[attr-defined] # noqa: E501
-            yield Link(obj.name.value, node, options=options, alias=alias)
+            yield Link(
+                obj.name.value, node, options=options,
+                alias=alias, directives=tuple(directives)
+            )
 
     def visit_variable(self, obj: ast.VariableNode) -> Any:
         return self.lookup_variable(obj.name.value)
 
     def visit_null_value(self, obj: ast.NullValueNode) -> None:
         return None
```

### Comparing `hiku-0.7.0rc8/hiku/readers/protobuf.py` & `hiku-0.7.0rc9/hiku/readers/protobuf.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.0rc8/hiku/readers/simple.py` & `hiku-0.7.0rc9/hiku/readers/simple.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.0rc8/hiku/result.py` & `hiku-0.7.0rc9/hiku/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,17 @@
     def __init__(self, node: str, ident: t.Any) -> None:
         self.node = node
         self.ident = ident
 
     def __repr__(self) -> str:
         return '<{}[{!r}]>'.format(self.node, self.ident)
 
+    def __hash__(self) -> int:
+        return hash((self.node, self.ident))
+
 
 ROOT = Reference('__root__', '__root__')
 
 
 class Index(defaultdict):
 
     def __init__(self) -> None:
@@ -67,14 +70,15 @@
     def finish(self) -> None:
         for value in self.values():
             value.default_factory = None
         self.default_factory = None
 
 
 class Proxy:
+    """Proxy is a dict-like interface to index."""
     __slots__ = ('__idx__', '__ref__', '__node__')
 
     def __init__(self, index: Index, reference: Reference, node: Node) -> None:
         self.__idx__ = index
         self.__ref__ = reference
         self.__node__ = node
```

### Comparing `hiku-0.7.0rc8/hiku/sources/aiopg.py` & `hiku-0.7.0rc9/hiku/sources/aiopg.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.0rc8/hiku/sources/graph.py` & `hiku-0.7.0rc9/hiku/sources/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,14 +156,15 @@
         self,
         fields: List[FieldGroup],
         ids: List,
         queue: Queue,
         ctx: Context,
         task_set: TaskSet
     ) -> Callable[[], List[List]]:
+        path = tuple(['this'])
         this_graph_link = Link(THIS, Sequence[TypeRef[self.node]], None, requires=None)  # type: ignore # noqa: E501
 
         reqs = merge([gf.func.reqs for gf, _ in fields])  # type: ignore[union-attr]  # noqa: E501
         procs = [gf.func.proc for gf, _ in fields]  # type: ignore[union-attr]
         option_values = []
         for gf, qf in fields:
             if gf.options and qf.options:
@@ -174,17 +175,17 @@
                 option_values.append([])
 
         this_query_link = reqs.fields_map[THIS]
         other_reqs = query.Node([r for r in reqs.fields
                                  if r.name != THIS])
 
         q = Query(queue, task_set, self.graph, reqs, ctx)
-        q.process_link(self.graph.root, this_graph_link, this_query_link,
+        q.process_link(path, self.graph.root, this_graph_link, this_query_link,
                        None, ids)
-        q.process_node(self.graph.root, other_reqs, None)
+        q.process_node(path, self.graph.root, other_reqs, None)
         return _create_result_proc(q, procs, option_values)
 
     def compile(self, expr: Expr) -> BoundExpr:
         return BoundExpr(self, expr)
 
     def c(self, expr: Expr) -> BoundExpr:
         return self.compile(expr)
```

### Comparing `hiku-0.7.0rc8/hiku/sources/sqlalchemy.py` & `hiku-0.7.0rc9/hiku/sources/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.0rc8/hiku/sources/sqlalchemy_async.py` & `hiku-0.7.0rc9/hiku/sources/sqlalchemy_async.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.0rc8/hiku/telemetry/prometheus.py` & `hiku-0.7.0rc9/hiku/telemetry/prometheus.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.0rc8/hiku/typedef/kinko.py` & `hiku-0.7.0rc9/hiku/typedef/kinko.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.0rc8/hiku/types.py` & `hiku-0.7.0rc9/hiku/types.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.0rc8/hiku/utils.py` & `hiku-0.7.0rc9/hiku/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import sys
+from functools import wraps
 from typing import (
     NewType,
     cast,
     Callable,
     Any,
     TypeVar,
     List,
@@ -34,10 +35,11 @@
 
 
 T = TypeVar('T')
 P = ParamSpec('P')
 
 
 def listify(func: Callable[P, Iterator[T]]) -> Callable[P, List[T]]:
+    @wraps(func)
     def wrapper(*args: P.args, **kwargs: P.kwargs) -> List[T]:
         return list(func(*args, **kwargs))
     return wrapper
```

### Comparing `hiku-0.7.0rc8/hiku/validate/graph.py` & `hiku-0.7.0rc9/hiku/validate/graph.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.0rc8/hiku/validate/query.py` & `hiku-0.7.0rc9/hiku/validate/query.py`

 * *Files identical despite different names*

### Comparing `hiku-0.7.0rc8/hiku.egg-info/PKG-INFO` & `hiku-0.7.0rc9/hiku.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiku
-Version: 0.7.0rc8
+Version: 0.7.0rc9
 Summary: Library to implement Graph APIs
 Home-page: https://github.com/evo-company/hiku
 Author: Vladimir Magamedov
 Author-email: vladimir@magamedov.com
 License: BSD-3-Clause
 Description: Hiku
         ====
```

### Comparing `hiku-0.7.0rc8/hiku.egg-info/SOURCES.txt` & `hiku-0.7.0rc9/hiku.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 MANIFEST.in
 README.rst
 setup.py
 hiku/__init__.py
 hiku/builder.py
+hiku/cache.py
 hiku/compat.py
 hiku/edn.py
 hiku/engine.py
 hiku/graph.py
 hiku/query.py
 hiku/result.py
 hiku/types.py
```

### Comparing `hiku-0.7.0rc8/setup.py` & `hiku-0.7.0rc9/setup.py`

 * *Files identical despite different names*

