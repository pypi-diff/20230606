# Comparing `tmp/deepview-profile-0.12.2.tar.gz` & `tmp/deepview_profile-0.12.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepview-profile-0.12.2.tar", max compression
+gzip compressed data, was "deepview_profile-0.12.3.tar", max compression
```

## Comparing `deepview-profile-0.12.2.tar` & `deepview_profile-0.12.3.tar`

### file list

```diff
@@ -1,73 +1,74 @@
--rw-r--r--   0        0        0    10173 2022-11-29 16:49:51.810194 deepview-profile-0.12.2/LICENSE
--rw-r--r--   0        0        0     5824 2023-04-20 15:13:52.998459 deepview-profile-0.12.2/README.md
--rw-r--r--   0        0        0      324 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/__init__.py
--rw-r--r--   0        0        0     1123 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/__main__.py
--rw-r--r--   0        0        0        0 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/analysis/__init__.py
--rw-r--r--   0        0        0     7313 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/analysis/request_manager.py
--rw-r--r--   0        0        0     1664 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/analysis/runner.py
--rw-r--r--   0        0        0    23297 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/analysis/session.py
--rw-r--r--   0        0        0     1373 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/analysis/static.py
--rw-r--r--   0        0        0        0 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/commands/__init__.py
--rw-r--r--   0        0        0     2002 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/commands/interactive.py
--rw-r--r--   0        0        0     3021 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/commands/measurements.py
--rw-r--r--   0        0        0     1729 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/commands/memory.py
--rw-r--r--   0        0        0     2749 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/commands/prediction_models.py
--rw-r--r--   0        0        0     1788 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/commands/time.py
--rw-r--r--   0        0        0      879 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/config/__init__.py
--rw-r--r--   0        0        0      150 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/data/__init__.py
--rw-r--r--   0        0        0      598 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/data/hints.yml
--rw-r--r--   0        0        0        0 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/db/__init__.py
--rw-r--r--   0        0        0     2968 2023-04-20 16:33:06.385513 deepview-profile-0.12.2/deepview_profile/db/database.py
--rw-r--r--   0        0        0        0 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/energy/__init__.py
--rw-r--r--   0        0        0     3727 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/energy/measurer.py
--rw-r--r--   0        0        0      722 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/error_printing.py
--rw-r--r--   0        0        0      683 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/evaluate.py
--rw-r--r--   0        0        0     3297 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/exceptions.py
--rw-r--r--   0        0        0     1914 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/initialization.py
--rw-r--r--   0        0        0        0 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/io/__init__.py
--rw-r--r--   0        0        0     4440 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/io/connection.py
--rw-r--r--   0        0        0     2452 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/io/connection_acceptor.py
--rw-r--r--   0        0        0     2062 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/io/connection_manager.py
--rw-r--r--   0        0        0      765 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/io/sentinel.py
--rw-r--r--   0        0        0     2261 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/lru_cache.py
--rw-r--r--   0        0        0        0 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/models/__init__.py
--rw-r--r--   0        0        0     3832 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/models/analysis.py
--rw-r--r--   0        0        0     1061 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/models/source_map.py
--rw-r--r--   0        0        0      455 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/nvml.py
--rw-r--r--   0        0        0     1245 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/profiler/__init__.py
--rw-r--r--   0        0        0     3054 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/profiler/autograd.py
--rw-r--r--   0        0        0     2943 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/profiler/backward.py
--rw-r--r--   0        0        0     8500 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/profiler/iteration.py
--rw-r--r--   0        0        0     5301 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/profiler/operation.py
--rw-r--r--   0        0        0        0 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/protocol/__init__.py
--rw-r--r--   0        0        0     5862 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/protocol/message_handler.py
--rw-r--r--   0        0        0     3385 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/protocol/message_sender.py
--rw-r--r--   0        0        0        0 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/protocol_gen/__init__.py
--rw-r--r--   0        0        0    64719 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/protocol_gen/innpv_pb2.py
--rw-r--r--   0        0        0     3441 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/server.py
--rw-r--r--   0        0        0     1067 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/skyline.py
--rw-r--r--   0        0        0        0 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/tests/__init__.py
--rw-r--r--   0        0        0     7188 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/tests/test_lru_cache.py
--rw-r--r--   0        0        0        0 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/tracking/__init__.py
--rw-r--r--   0        0        0      779 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/tracking/backward_interceptor.py
--rw-r--r--   0        0        0     1109 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/tracking/base.py
--rw-r--r--   0        0        0    10919 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/tracking/breakdown.py
--rw-r--r--   0        0        0     1439 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/tracking/call_stack.py
--rw-r--r--   0        0        0     4106 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/tracking/callable_tracker.py
--rw-r--r--   0        0        0     1630 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/tracking/hook_manager.py
--rw-r--r--   0        0        0        0 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/tracking/memory/__init__.py
--rw-r--r--   0        0        0     8090 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/tracking/memory/activations.py
--rw-r--r--   0        0        0     4085 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/tracking/memory/report.py
--rw-r--r--   0        0        0     3437 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/tracking/memory/report_queries.py
--rw-r--r--   0        0        0     1903 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/tracking/memory/weights.py
--rw-r--r--   0        0        0        0 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/tracking/time/__init__.py
--rw-r--r--   0        0        0     2634 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/tracking/time/operation.py
--rw-r--r--   0        0        0     2199 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/tracking/time/report.py
--rw-r--r--   0        0        0     1267 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/tracking/time/report_queries.py
--rw-r--r--   0        0        0     6258 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/tracking/tracker.py
--rw-r--r--   0        0        0      362 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/tracking/utils.py
--rw-r--r--   0        0        0     2680 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/user_code_utils.py
--rw-r--r--   0        0        0     1884 2023-04-20 14:57:42.364394 deepview-profile-0.12.2/deepview_profile/version_utils.py
--rw-r--r--   0        0        0     1089 2023-04-20 16:38:46.232525 deepview-profile-0.12.2/pyproject.toml
--rw-r--r--   0        0        0     7363 2023-04-20 16:39:55.941080 deepview-profile-0.12.2/setup.py
--rw-r--r--   0        0        0     7053 2023-04-20 16:39:55.941570 deepview-profile-0.12.2/PKG-INFO
+-rw-r--r--   0        0        0    10173 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/LICENSE
+-rw-r--r--   0        0        0     5277 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/README.md
+-rw-r--r--   0        0        0      324 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/__init__.py
+-rw-r--r--   0        0        0     1111 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/analysis/__init__.py
+-rw-r--r--   0        0        0     7331 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/analysis/request_manager.py
+-rw-r--r--   0        0        0     1673 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/analysis/runner.py
+-rw-r--r--   0        0        0    24642 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/analysis/session.py
+-rw-r--r--   0        0        0     1373 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/analysis/static.py
+-rw-r--r--   0        0        0        0 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/commands/__init__.py
+-rw-r--r--   0        0        0     1937 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/commands/interactive.py
+-rw-r--r--   0        0        0     2974 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/commands/measurements.py
+-rw-r--r--   0        0        0     1682 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/commands/memory.py
+-rw-r--r--   0        0        0     2702 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/commands/prediction_models.py
+-rw-r--r--   0        0        0     1741 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/commands/time.py
+-rw-r--r--   0        0        0      879 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/config/__init__.py
+-rw-r--r--   0        0        0      150 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/data/__init__.py
+-rw-r--r--   0        0        0      598 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/data/hints.yml
+-rw-r--r--   0        0        0        0 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/db/__init__.py
+-rw-r--r--   0        0        0     3023 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/db/database.py
+-rw-r--r--   0        0        0        0 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/energy/__init__.py
+-rw-r--r--   0        0        0     3742 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/energy/measurer.py
+-rw-r--r--   0        0        0      722 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/error_printing.py
+-rw-r--r--   0        0        0      671 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/evaluate.py
+-rw-r--r--   0        0        0     3297 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/exceptions.py
+-rw-r--r--   0        0        0     1969 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/initialization.py
+-rw-r--r--   0        0        0        0 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/io/__init__.py
+-rw-r--r--   0        0        0     4442 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/io/connection.py
+-rw-r--r--   0        0        0     2452 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/io/connection_acceptor.py
+-rw-r--r--   0        0        0     2062 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/io/connection_manager.py
+-rw-r--r--   0        0        0      765 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/io/sentinel.py
+-rw-r--r--   0        0        0     2261 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/lru_cache.py
+-rw-r--r--   0        0        0        0 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/models/__init__.py
+-rw-r--r--   0        0        0     3776 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/models/analysis.py
+-rw-r--r--   0        0        0     1061 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/models/source_map.py
+-rw-r--r--   0        0        0      455 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/nvml.py
+-rw-r--r--   0        0        0     1245 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/profiler/__init__.py
+-rw-r--r--   0        0        0     3054 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/profiler/autograd.py
+-rw-r--r--   0        0        0     2943 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/profiler/backward.py
+-rw-r--r--   0        0        0     8616 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/profiler/iteration.py
+-rw-r--r--   0        0        0     5301 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/profiler/operation.py
+-rw-r--r--   0        0        0        0 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/protocol/__init__.py
+-rw-r--r--   0        0        0     5861 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/protocol/message_handler.py
+-rw-r--r--   0        0        0     3312 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/protocol/message_sender.py
+-rw-r--r--   0        0        0        0 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/protocol_gen/__init__.py
+-rw-r--r--   0        0        0    65924 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/protocol_gen/innpv_pb2.py
+-rw-r--r--   0        0        0     3441 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/server.py
+-rw-r--r--   0        0        0     1043 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/skyline.py
+-rw-r--r--   0        0        0        0 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/tests/__init__.py
+-rw-r--r--   0        0        0     7163 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/tests/test_lru_cache.py
+-rw-r--r--   0        0        0        0 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/tracking/__init__.py
+-rw-r--r--   0        0        0      779 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/tracking/backward_interceptor.py
+-rw-r--r--   0        0        0     1109 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/tracking/base.py
+-rw-r--r--   0        0        0    10919 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/tracking/breakdown.py
+-rw-r--r--   0        0        0     1439 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/tracking/call_stack.py
+-rw-r--r--   0        0        0     4106 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/tracking/callable_tracker.py
+-rw-r--r--   0        0        0     1630 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/tracking/hook_manager.py
+-rw-r--r--   0        0        0        0 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/tracking/memory/__init__.py
+-rw-r--r--   0        0        0     8087 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/tracking/memory/activations.py
+-rw-r--r--   0        0        0     4075 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/tracking/memory/report.py
+-rw-r--r--   0        0        0     3437 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/tracking/memory/report_queries.py
+-rw-r--r--   0        0        0     1993 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/tracking/memory/weights.py
+-rw-r--r--   0        0        0        0 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/tracking/time/__init__.py
+-rw-r--r--   0        0        0     2621 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/tracking/time/operation.py
+-rw-r--r--   0        0        0     2189 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/tracking/time/report.py
+-rw-r--r--   0        0        0     1267 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/tracking/time/report_queries.py
+-rw-r--r--   0        0        0     6258 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/tracking/tracker.py
+-rw-r--r--   0        0        0      349 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/tracking/utils.py
+-rw-r--r--   0        0        0     2670 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/user_code_utils.py
+-rw-r--r--   0        0        0     8983 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/util_weak.py
+-rw-r--r--   0        0        0      180 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/utils.py
+-rw-r--r--   0        0        0     1884 2023-06-06 16:05:43.318826 deepview_profile-0.12.3/deepview_profile/version_utils.py
+-rw-r--r--   0        0        0     1244 2023-06-06 16:06:03.950406 deepview_profile-0.12.3/pyproject.toml
+-rw-r--r--   0        0        0     6557 1970-01-01 00:00:00.000000 deepview_profile-0.12.3/PKG-INFO
```

### Comparing `deepview-profile-0.12.2/LICENSE` & `deepview_profile-0.12.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.2/README.md` & `deepview_profile-0.12.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 [![](https://img.shields.io/pypi/v/deepview-profile.svg)](https://pypi.org/project/deepview-profile/)
 
 DeepView.Profile is a tool to profile and debug the training performance of [PyTorch](https://pytorch.org) neural networks.
 
 - [Installation](#installation)
 - [Usage example](#getting-started)
 - [Development Environment Setup](#dev-setup)
-- [Release Process](#release-process)
 - [Release History](#release-history)
 - [Meta](#meta)
 - [Contributing](#contributing)
 
 <h2 id="installation">Installation</h2>
 
 DeepView.Profile works with *GPU-based* neural networks that are implemented in [PyTorch](https://pytorch.org).
@@ -75,26 +74,14 @@
 
 <h2 id="dev-setup">Development Environment Setup</h2>
 
 From the project root, do
 ```zsh
 poetry install
 ```
-<h2 id="release-process">Release Process</h2>
-
-1. Make sure you're on main branch and it is clean
-1. Run [tools/prepare-release.sh](tools/prepare-release.sh) which will:
-    * Increment the version
-    * Create a release branch
-    * Create a release PR
-1. After the PR is merged [build-and-publish-new-version.yml](.github/workflows/build-and-publish-new-version.yml) GitHub action will:
-    * build the Python Wheels
-    * GitHub release
-    * Publish to Test PyPI
-    * Subject to approval publish to PyPI
 
 <h2 id="release-history">Release History</h2>
 
 See [Releases](https://github.com/CentML/DeepView.Profile/releases)
 
 <h2 id="meta">Meta</h2>
```

### Comparing `deepview-profile-0.12.2/deepview_profile/__main__.py` & `deepview_profile-0.12.3/deepview_profile/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import argparse
-import enum
 import sys
 
 import deepview_profile
 import deepview_profile.commands.interactive
 import deepview_profile.commands.memory
 import deepview_profile.commands.time
```

### Comparing `deepview-profile-0.12.2/deepview_profile/analysis/request_manager.py` & `deepview_profile-0.12.3/deepview_profile/analysis/request_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
 import math
 import time
 from concurrent.futures import ThreadPoolExecutor
 
 from deepview_profile.analysis.runner import analyze_project
-from deepview_profile.config import Config
 from deepview_profile.exceptions import AnalysisError
 from deepview_profile.nvml import NVML
 import deepview_profile.protocol_gen.innpv_pb2 as pm
 
 logger = logging.getLogger(__name__)
 
 
@@ -131,15 +130,15 @@
                 *(context.address),
                 elapsed_time,
             )
 
         except AnalysisError as ex:
             self._enqueue_response(self._send_analysis_error, ex, context)
 
-        except:
+        except Exception:
             logger.exception(
                 'Exception occurred when handling analysis request.')
             self._enqueue_response(
                 self._send_analysis_error,
                 AnalysisError(
                     'An unexpected error occurred when analyzing your model. '
                     'Please file a bug report and then restart DeepView.'
@@ -160,42 +159,42 @@
         throughput.predicted_max_samples_per_second = math.nan
         self._message_sender.send_throughput_response(throughput, context)
 
     def _send_breakdown_response(self, breakdown, context):
         # Called from the main executor. Do not call directly!
         try:
             self._message_sender.send_breakdown_response(breakdown, context)
-        except:
+        except Exception:
             logger.exception(
                 'Exception occurred when sending a breakdown response.')
 
     def _send_analysis_error(self, exception, context):
         # Called from the main executor. Do not call directly!
         try:
             self._message_sender.send_analysis_error(exception, context)
-        except:
+        except Exception:
             logger.exception(
                 'Exception occurred when sending an analysis error.')
 
     def _send_throughput_response(self, throughput, context):
         # Called from the main executor. Do not call directly!
         try:
             self._message_sender.send_throughput_response(throughput, context)
-        except:
+        except Exception:
             logger.exception(
                 'Exception occurred when sending a throughput response.')
 
     def _send_habitat_response(self, habitat_resp, context):
         # Called from the main executor. Do not call directly!
         try:
             self._message_sender.send_habitat_response(habitat_resp, context)
-        except:
+        except Exception:
             logger.exception(
                 'Exception occurred when sending a DeepView.Predict response.')
 
     def _send_energy_response(self, energy_resp, context):
         # Called from the main executor. Do not call directly!
         try:
             self._message_sender.send_energy_response(energy_resp, context)
-        except:
+        except Exception:
             logger.exception(
-                'Exception occurred when sending an energy response.')
+                'Exception occurred when sending an energy response.')
```

### Comparing `deepview-profile-0.12.2/deepview_profile/analysis/runner.py` & `deepview_profile-0.12.3/deepview_profile/analysis/runner.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import argparse
 import logging
 import os
 
 import torch
 from deepview_profile.analysis.session import AnalysisSession
 from deepview_profile.nvml import NVML
-
+from deepview_profile.utils import release_memory
 
 def analyze_project(project_root, entry_point, nvml):
-    torch.cuda.empty_cache()
+    release_memory()
     session = AnalysisSession.new_from(project_root, entry_point)
     yield session.measure_breakdown(nvml)
-    torch.cuda.empty_cache()
+    release_memory()
     yield session.measure_throughput()
-    torch.cuda.empty_cache()
+    release_memory()
 
     print("analyze_project: running deepview_predict()")
     yield session.habitat_predict()
-    torch.cuda.empty_cache()
+    release_memory()
 
     print("analyze_project: running energy_compute()")
     yield session.energy_compute()
-    torch.cuda.empty_cache()
+    release_memory()
 
 
 def main():
     # This is used for development and debugging purposes
     parser = argparse.ArgumentParser()
     parser.add_argument("entry_point", type=str)
     args = parser.parse_args()
```

### Comparing `deepview-profile-0.12.2/deepview_profile/analysis/session.py` & `deepview_profile-0.12.3/deepview_profile/analysis/session.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,43 +39,46 @@
 INPUT_PROVIDER_NAME = "deepview_input_provider"
 ITERATION_PROVIDER_NAME = "deepview_iteration_provider"
 BATCH_SIZE_ARG = "batch_size"
 
 
 # Habitat variables
 Context = collections.namedtuple(
-    'Context',
-    ['origin_device', 'profiler', 'percentile'],
+    "Context",
+    ["origin_device", "profiler", "percentile"],
 )
 
+
 class AnalysisSession:
     def __init__(
         self,
         project_root,
         entry_point,
         path_to_entry_point_dir,
         model_provider,
         input_provider,
         iteration_provider,
         batch_size,
-        entry_point_static_analyzer
+        entry_point_static_analyzer,
     ):
         self._project_root = project_root
         self._entry_point = entry_point
         self._path_to_entry_point_dir = path_to_entry_point_dir
         self._model_provider = model_provider
         self._input_provider = input_provider
         self._iteration_provider = iteration_provider
         self._batch_size = batch_size
         self._entry_point_static_analyzer = entry_point_static_analyzer
         self._profiler = None
         self._memory_usage_percentage = None
         self._batch_size_iteration_run_time_ms = None
         self._batch_size_peak_usage_bytes = None
-        self._energy_table_interface = EnergyTableInterface(DatabaseInterface().connection)
+        self._energy_table_interface = EnergyTableInterface(
+            DatabaseInterface().connection
+        )
 
     @classmethod
     def new_from(cls, project_root, entry_point):
         path_to_entry_point = os.path.join(project_root, entry_point)
         # Note: This is not necessarily the same as project_root because the
         #       entry_point could be in a subdirectory.
         path_to_entry_point_dir = os.path.dirname(path_to_entry_point)
@@ -88,45 +91,47 @@
         )
 
         # 2. Check that the model provider and input provider functions exist
         if MODEL_PROVIDER_NAME not in scope:
             raise AnalysisError(
                 "The project entry point file is missing a model provider "
                 "function. Please add a model provider function named "
-                "\"{}\".".format(MODEL_PROVIDER_NAME)
+                '"{}".'.format(MODEL_PROVIDER_NAME)
             ).with_file_context(entry_point)
 
         if INPUT_PROVIDER_NAME not in scope:
             raise AnalysisError(
                 "The project entry point file is missing an input provider "
                 "function. Please add an input provider function named "
-                "\"{}\".".format(INPUT_PROVIDER_NAME)
+                '"{}".'.format(INPUT_PROVIDER_NAME)
             ).with_file_context(entry_point)
 
         if ITERATION_PROVIDER_NAME not in scope:
             raise AnalysisError(
                 "The project entry point file is missing an iteration "
                 "provider function. Please add an iteration provider function "
-                "named \"{}\".".format(ITERATION_PROVIDER_NAME)
+                'named "{}".'.format(ITERATION_PROVIDER_NAME)
             ).with_file_context(entry_point)
 
         batch_size = _validate_providers_signatures(
             scope[MODEL_PROVIDER_NAME],
             scope[INPUT_PROVIDER_NAME],
             scope[ITERATION_PROVIDER_NAME],
             entry_point,
         )
 
-        model_provider, input_provider, iteration_provider = (
-            _wrap_providers_with_validators(
-                scope[MODEL_PROVIDER_NAME],
-                scope[INPUT_PROVIDER_NAME],
-                scope[ITERATION_PROVIDER_NAME],
-                entry_point,
-            )
+        (
+            model_provider,
+            input_provider,
+            iteration_provider,
+        ) = _wrap_providers_with_validators(
+            scope[MODEL_PROVIDER_NAME],
+            scope[INPUT_PROVIDER_NAME],
+            scope[ITERATION_PROVIDER_NAME],
+            entry_point,
         )
 
         return cls(
             project_root,
             entry_point,
             path_to_entry_point_dir,
             model_provider,
@@ -134,67 +139,81 @@
             iteration_provider,
             batch_size,
             StaticAnalyzer(entry_point_code, entry_point_ast),
         )
 
     def energy_compute(self) -> pm.EnergyResponse:
         energy_measurer = EnergyMeasurer()
-        
+
         model = self._model_provider()
         inputs = self._input_provider()
         iteration = self._iteration_provider(model)
         resp = pm.EnergyResponse()
 
         try:
             energy_measurer.begin_measurement()
             iterations = 20
             for _ in range(iterations):
                 iteration(*inputs)
             energy_measurer.end_measurement()
-        except PermissionError as err:
-            # Remind user to set their CPU permissions
-            print(err)
-            
-        resp.total_consumption = energy_measurer.total_energy()/float(iterations)
-        resp.batch_size = self._batch_size
+            resp.total_consumption = energy_measurer.total_energy() / float(iterations)
+            resp.batch_size = self._batch_size
 
-        components = []
-        components_joules = []
+            components = []
+            components_joules = []
 
-        if energy_measurer.cpu_energy() is not None:
-            cpu_component = pm.EnergyConsumptionComponent()
-            cpu_component.component_type = pm.ENERGY_CPU_DRAM
-            cpu_component.consumption_joules = energy_measurer.cpu_energy()/float(iterations)
-            components.append(cpu_component)
-            components_joules.append(cpu_component.consumption_joules)
-        else:
-            cpu_component = pm.EnergyConsumptionComponent()
-            cpu_component.component_type = pm.ENERGY_CPU_DRAM
-            cpu_component.consumption_joules = 0.0
-            components.append(cpu_component)
-            components_joules.append(cpu_component.consumption_joules)
-        
-        gpu_component = pm.EnergyConsumptionComponent()
-        gpu_component.component_type = pm.ENERGY_NVIDIA
-        gpu_component.consumption_joules = energy_measurer.gpu_energy()/float(iterations)
-        components.append(gpu_component)
-        components_joules.append(gpu_component.consumption_joules)
-        
-        resp.components.extend(components)
-    
-        # get last 10 runs if they exist
-        path_to_entry_point = os.path.join(self._project_root, self._entry_point)
-        past_runs = self._energy_table_interface.get_latest_n_entries_of_entry_point(10, path_to_entry_point)
-        resp.past_measurements.extend(_convert_to_energy_responses(past_runs))
-
-        # add current run to database
-        current_entry = [path_to_entry_point] + components_joules
-        current_entry.append(self._batch_size)
-        self._energy_table_interface.add_entry(current_entry)
-        return resp
+            if energy_measurer.cpu_energy() is not None:
+                cpu_component = pm.EnergyConsumptionComponent()
+                cpu_component.component_type = pm.ENERGY_CPU_DRAM
+                cpu_component.consumption_joules = energy_measurer.cpu_energy() / float(
+                    iterations
+                )
+                components.append(cpu_component)
+                components_joules.append(cpu_component.consumption_joules)
+            else:
+                cpu_component = pm.EnergyConsumptionComponent()
+                cpu_component.component_type = pm.ENERGY_CPU_DRAM
+                cpu_component.consumption_joules = 0.0
+                components.append(cpu_component)
+                components_joules.append(cpu_component.consumption_joules)
+
+            gpu_component = pm.EnergyConsumptionComponent()
+            gpu_component.component_type = pm.ENERGY_NVIDIA
+            gpu_component.consumption_joules = energy_measurer.gpu_energy() / float(
+                iterations
+            )
+            components.append(gpu_component)
+            components_joules.append(gpu_component.consumption_joules)
+
+            resp.components.extend(components)
+
+            # get last 10 runs if they exist
+            path_to_entry_point = os.path.join(self._project_root, self._entry_point)
+            past_runs = (
+                self._energy_table_interface.get_latest_n_entries_of_entry_point(
+                    10, path_to_entry_point
+                )
+            )
+            resp.past_measurements.extend(_convert_to_energy_responses(past_runs))
+
+            # add current run to database
+            current_entry = [path_to_entry_point] + components_joules
+            current_entry.append(self._batch_size)
+            self._energy_table_interface.add_entry(current_entry)
+        except AnalysisError as ex:
+            message = str(ex)
+            logger.error(message)
+            resp.analysis_error.error_message = message
+        except Exception:
+            logger.error("There was an error obtaining energy measurements")
+            resp.analysis_error.error_message = (
+                "There was an error obtaining energy measurements"
+            )
+        finally:
+            return resp
 
     def habitat_compute_threshold(self, runnable, context):
         tracker = habitat.OperationTracker(context.origin_device)
         with tracker.track():
             runnable()
 
         run_times = []
@@ -204,112 +223,125 @@
                 continue
             run_times.append(op.forward.run_time_ms)
             if op.backward is not None:
                 run_times.append(op.backward.run_time_ms)
 
         return np.percentile(run_times, context.percentile)
 
-
     def habitat_predict(self):
         resp = pm.HabitatResponse()
-        if not habitat_found: 
+        if not habitat_found:
             logger.debug("Skipping deepview predictions, returning empty response.")
             return resp
 
-        print("deepview_predict: begin")
-        DEVICES = [
-            habitat.Device.P100,
-            habitat.Device.P4000,
-            habitat.Device.RTX2070,
-            habitat.Device.RTX2080Ti,
-            habitat.Device.T4,
-            habitat.Device.V100,
-            habitat.Device.A100,
-            habitat.Device.RTX3090,
-            habitat.Device.A40,
-            habitat.Device.A4000,
-            habitat.Device.RTX4000
-        ]
-
-        # Detect source GPU
-        pynvml.nvmlInit()
-        if pynvml.nvmlDeviceGetCount() == 0:
-            raise Exception("NVML failed to find a GPU. PLease ensure that you have a NVIDIA GPU installed and that the drivers are functioning correctly.")
-
-        # TODO: Consider profiling on not only the first detected GPU
-        nvml_handle = pynvml.nvmlDeviceGetHandleByIndex(0)
-        source_device_name = pynvml.nvmlDeviceGetName(nvml_handle).decode("utf-8")
-        split_source_device_name = re.split(r"-|\s|_|\\|/", source_device_name)
-        source_device = None if logging.root.level > logging.DEBUG else habitat.Device.T4
-        for device in DEVICES:
-            if device.name in split_source_device_name:
-                source_device = device
-        pynvml.nvmlShutdown()
-        if not source_device:
-            logger.debug("Skipping DeepView predictions, source not in list of supported GPUs.")
-            src = pm.HabitatDevicePrediction()
-            src.device_name = 'unavailable'
-            src.runtime_ms = -1
-            resp.predictions.append(src)
-            return resp
-
-        print("deepview_predict: detected source device", source_device.name)
+        try:
+            print("deepview_predict: begin")
+            DEVICES = [
+                habitat.Device.P100,
+                habitat.Device.P4000,
+                habitat.Device.RTX2070,
+                habitat.Device.RTX2080Ti,
+                habitat.Device.T4,
+                habitat.Device.V100,
+                habitat.Device.A100,
+                habitat.Device.RTX3090,
+                habitat.Device.A40,
+                habitat.Device.A4000,
+                habitat.Device.RTX4000,
+            ]
+
+            # Detect source GPU
+            pynvml.nvmlInit()
+            if pynvml.nvmlDeviceGetCount() == 0:
+                raise Exception("NVML failed to find a GPU. Please ensure that you \
+                have a NVIDIA GPU installed and that the drivers are functioning \
+                correctly.")
+
+            # TODO: Consider profiling on not only the first detected GPU
+            nvml_handle = pynvml.nvmlDeviceGetHandleByIndex(0)
+            source_device_name = pynvml.nvmlDeviceGetName(nvml_handle).decode("utf-8")
+            split_source_device_name = re.split(r"-|\s|_|\\|/", source_device_name)
+            source_device = (
+                None if logging.root.level > logging.DEBUG else habitat.Device.T4
+            )
+            for device in DEVICES:
+                if device.name in split_source_device_name:
+                    source_device = device
+            pynvml.nvmlShutdown()
+            if not source_device:
+                logger.debug(
+                    "Skipping DeepView predictions,\
+                    source not in list of supported GPUs."
+                )
+                src = pm.HabitatDevicePrediction()
+                src.device_name = "unavailable"
+                src.runtime_ms = -1
+                resp.predictions.append(src)
+                return resp
 
-        # get model
-        model = self._model_provider()
-        inputs = self._input_provider()
-        iteration = self._iteration_provider(model)
+            print("deepview_predict: detected source device", source_device.name)
 
-        def runnable():
-            iteration(*inputs)
+            # get model
+            model = self._model_provider()
+            inputs = self._input_provider()
+            iteration = self._iteration_provider(model)
 
-        profiler = RunTimeProfiler()
+            def runnable():
+                iteration(*inputs)
 
-        context = Context(
-            origin_device=source_device,
-            profiler=profiler,
-            percentile=99.5
-        )
+            profiler = RunTimeProfiler()
 
-        threshold = self.habitat_compute_threshold(runnable, context)
-        
-        tracker = habitat.OperationTracker(
-            device=context.origin_device,
-            metrics=[
-                habitat.Metric.SinglePrecisionFLOPEfficiency,
-                habitat.Metric.DRAMReadBytes,
-                habitat.Metric.DRAMWriteBytes,
-            ],
-            metrics_threshold_ms=threshold,
-        )
+            context = Context(
+                origin_device=source_device, profiler=profiler, percentile=99.5
+            )
 
-        with tracker.track():
-            iteration(*inputs)
+            threshold = self.habitat_compute_threshold(runnable, context)
 
-        print("deepview_predict: tracing on origin device")
-        trace = tracker.get_tracked_trace()
+            tracker = habitat.OperationTracker(
+                device=context.origin_device,
+                metrics=[
+                    habitat.Metric.SinglePrecisionFLOPEfficiency,
+                    habitat.Metric.DRAMReadBytes,
+                    habitat.Metric.DRAMWriteBytes,
+                ],
+                metrics_threshold_ms=threshold,
+            )
 
-        src = pm.HabitatDevicePrediction()
-        src.device_name = 'source'
-        src.runtime_ms = trace.run_time_ms
-        resp.predictions.append(src)
-
-        for device in DEVICES:
-            print("deepview_predict: predicting for", device)
-            predicted_trace = trace.to_device(device)
-
-            pred = pm.HabitatDevicePrediction()
-            pred.device_name = device.name
-            pred.runtime_ms = predicted_trace.run_time_ms
-            resp.predictions.append(pred)
+            with tracker.track():
+                iteration(*inputs)
 
-        print(f"returning {len(resp.predictions)} predictions.")
+            print("deepview_predict: tracing on origin device")
+            trace = tracker.get_tracked_trace()
 
-        return resp 
+            src = pm.HabitatDevicePrediction()
+            src.device_name = "source"
+            src.runtime_ms = trace.run_time_ms
+            resp.predictions.append(src)
 
+            for device in DEVICES:
+                print("deepview_predict: predicting for", device)
+                predicted_trace = trace.to_device(device)
+
+                pred = pm.HabitatDevicePrediction()
+                pred.device_name = device.name
+                pred.runtime_ms = predicted_trace.run_time_ms
+                resp.predictions.append(pred)
+
+            print(f"returning {len(resp.predictions)} predictions.")
+        except AnalysisError as ex:
+            message = str(ex)
+            logger.error(message)
+            resp.analysis_error.error_message = message
+        except Exception:
+            logger.error("There was an error running DeepView Predict")
+            resp.analysis_error.error_message = (
+                "There was an error running DeepView Predict"
+            )
+        finally:
+            return resp
 
     def measure_breakdown(self, nvml):
         # 1. Measure the breakdown entries
         self._prepare_for_memory_profiling()
         tracker = self._get_tracker_instance()
         tracker.track_memory()
         tracker.track_run_time()
@@ -317,31 +349,31 @@
         del tracker
 
         # 2. Measure the overall iteration run time
         if self._batch_size_iteration_run_time_ms is None:
             if self._profiler is None:
                 self._initialize_iteration_profiler()
 
-            (self._batch_size_iteration_run_time_ms,
-             self._batch_size_peak_usage_bytes,
-             _) = self._profiler.measure_run_time_ms(self._batch_size)
+            (
+                self._batch_size_iteration_run_time_ms,
+                self._batch_size_peak_usage_bytes,
+                _,
+            ) = self._profiler.measure_run_time_ms(self._batch_size)
 
         # 3. Serialize the measured data
         bm = pm.BreakdownResponse()
         bm.batch_size = self._batch_size
         bm.peak_usage_bytes = breakdown.peak_usage_bytes
         bm.memory_capacity_bytes = nvml.get_memory_capacity().total
         bm.iteration_run_time_ms = self._batch_size_iteration_run_time_ms
         breakdown.operations.serialize_to_protobuf(bm.operation_tree)
         breakdown.weights.serialize_to_protobuf(bm.weight_tree)
 
         # 4. Bookkeeping for the throughput measurements
-        self._memory_usage_percentage = (
-            bm.peak_usage_bytes / bm.memory_capacity_bytes
-        )
+        self._memory_usage_percentage = bm.peak_usage_bytes / bm.memory_capacity_bytes
 
         return bm
 
     def measure_throughput(self):
         if self._profiler is None:
             self._initialize_iteration_profiler()
 
@@ -357,30 +389,30 @@
         if len(samples) == 0 or samples[0].batch_size != self._batch_size:
             raise AnalysisError(
                 "Something went wrong with DeepView.Profile when measuring your "
                 "model's throughput. Please file a bug."
             )
 
         # 2. Begin filling in the throughput response
-        measured_throughput = (
-            samples[0].batch_size / samples[0].run_time_ms * 1000
-        )
+        logger.debug("sampling results", samples)
+        measured_throughput = samples[0].batch_size / samples[0].run_time_ms * 1000
         throughput = pm.ThroughputResponse()
         throughput.samples_per_second = measured_throughput
         throughput.predicted_max_samples_per_second = math.nan
         throughput.can_manipulate_batch_size = False
 
         # 3. Determine whether we have information about the batch size
         #    location in the code
         batch_info = self._entry_point_static_analyzer.batch_size_location()
         if batch_info is not None:
             throughput.batch_size_context.line_number = batch_info[0]
             throughput.can_manipulate_batch_size = batch_info[1]
             throughput.batch_size_context.file_path.components.extend(
-                self._entry_point.split(os.sep))
+                self._entry_point.split(os.sep)
+            )
 
         # 4. If we do not have enough throughput samples, we cannot build any
         #    prediction models so just return the message as-is
         if len(samples) != num_samples:
             return throughput
 
         # 5. Build and validate the prediction models for run time (throughput)
@@ -405,36 +437,34 @@
         throughput.peak_usage_bytes.bias = peak_usage_model[1]
 
         predicted_max_throughput = 1000.0 / run_time_model[0]
 
         # Our prediction can be inaccurate due to sampling error or incorrect
         # assumptions. In these cases, we ignore our prediction. At the very
         # minimum, a good linear model has a positive slope and bias.
-        if (run_time_model[0] < 1e-3 or run_time_model[1] < 1e-3 or
-                measured_throughput > predicted_max_throughput):
+        # if (run_time_model[0] < 1e-3 or run_time_model[1] < 1e-3 or
+        if run_time_model[0] < 1e-3 or measured_throughput > predicted_max_throughput:
             return throughput
 
         throughput.predicted_max_samples_per_second = predicted_max_throughput
         throughput.run_time_ms.slope = run_time_model[0]
         throughput.run_time_ms.bias = run_time_model[1]
 
         return throughput
 
     def measure_peak_usage_bytes(self):
         self._prepare_for_memory_profiling()
         # Run one iteration to initialize the gradients
-        with user_code_environment(
-                self._path_to_entry_point_dir, self._project_root):
+        with user_code_environment(self._path_to_entry_point_dir, self._project_root):
             model = self._model_provider()
             iteration = self._iteration_provider(model)
             iteration(*self._input_provider(batch_size=self._batch_size))
 
         torch.cuda.reset_max_memory_allocated()
-        with user_code_environment(
-                self._path_to_entry_point_dir, self._project_root):
+        with user_code_environment(self._path_to_entry_point_dir, self._project_root):
             # NOTE: It's important to run at least 2 iterations here. It turns
             #       out that >= 2 iterations is the number of iterations needed
             #       to get a stable measurement of the total memory
             #       consumption. When using Adam, if you run one iteration, the
             #       memory usage ends up being too low by a constant factor.
             for _ in range(2):
                 iteration(*(self._input_provider(batch_size=self._batch_size)))
@@ -470,20 +500,19 @@
 
     def _get_tracker_instance(self):
         return Tracker(
             model_provider=self._model_provider,
             iteration_provider=self._iteration_provider,
             input_provider=self._input_provider,
             project_root=self._project_root,
-            user_code_path=self._path_to_entry_point_dir
+            user_code_path=self._path_to_entry_point_dir,
         )
 
 
-def _run_entry_point(
-        path_to_entry_point, path_to_entry_point_dir, project_root):
+def _run_entry_point(path_to_entry_point, path_to_entry_point_dir, project_root):
     with open(path_to_entry_point) as file:
         code_str = file.read()
     with exceptions_as_analysis_errors(project_root):
         tree = ast.parse(code_str, filename=path_to_entry_point)
         code = compile(tree, path_to_entry_point, mode="exec")
     with user_code_environment(path_to_entry_point_dir, project_root):
         scope = {}
@@ -500,17 +529,19 @@
     model_sig = inspect.signature(model_provider)
     if len(model_sig.parameters) != 0:
         raise AnalysisError(
             "The model provider function cannot have any parameters."
         ).with_file_context(entry_point)
 
     input_sig = inspect.signature(input_provider)
-    if (len(input_sig.parameters) != 1 or
-            BATCH_SIZE_ARG not in input_sig.parameters or
-            type(input_sig.parameters[BATCH_SIZE_ARG].default) is not int):
+    if (
+        len(input_sig.parameters) != 1
+        or BATCH_SIZE_ARG not in input_sig.parameters
+        or type(input_sig.parameters[BATCH_SIZE_ARG].default) is not int
+    ):
         raise AnalysisError(
             "The input provider function must have exactly one '{}' "
             "parameter with an integral default "
             "value.".format(BATCH_SIZE_ARG)
         ).with_file_context(entry_point)
     batch_size = input_sig.parameters[BATCH_SIZE_ARG].default
 
@@ -551,17 +582,17 @@
                 "The input provider function must return an iterable that "
                 "contains the inputs for the model. If your model only takes "
                 "a single tensor as input, return a single element tuple or "
                 "list in your input provider (e.g., 'return [the_input]')."
             ).with_file_context(entry_point)
 
         try:
-            input_iter = iter(inputs)
+            iter(inputs)
             return inputs
-        except TypeError as ex:
+        except TypeError:
             raise AnalysisError(
                 "The input provider function must return an iterable that "
                 "contains the inputs for the model."
             ).with_file_context(entry_point)
 
     def iteration_provider_wrapped(model):
         iteration = iteration_provider(model)
@@ -584,27 +615,30 @@
     y_np = np.array(y)
     x_np = np.array(x)
     stacked = np.vstack([x_np, np.ones(len(x_np))]).T
     slope, bias = np.linalg.lstsq(stacked, y_np, rcond=None)[0]
     # Linear model: y = slope * x + bias
     return slope, bias
 
-def _convert_to_energy_responses(entries: list)-> List[pm.EnergyResponse]:
+
+def _convert_to_energy_responses(entries: list) -> List[pm.EnergyResponse]:
     energy_response_list = []
     for entry in entries:
         if EnergyTableInterface.is_valid_entry_with_timestamp(entry):
             energy_response = pm.EnergyResponse()
             cpu_component = pm.EnergyConsumptionComponent()
             cpu_component.component_type = pm.ENERGY_CPU_DRAM
             cpu_component.consumption_joules = entry[1]
-                
+
             gpu_component = pm.EnergyConsumptionComponent()
             gpu_component.component_type = pm.ENERGY_NVIDIA
             gpu_component.consumption_joules = entry[2]
-            
-            energy_response.total_consumption = gpu_component.consumption_joules+cpu_component.consumption_joules 
+
+            energy_response.total_consumption = (
+                gpu_component.consumption_joules + cpu_component.consumption_joules
+            )
             energy_response.components.extend([cpu_component, gpu_component])
 
             energy_response.batch_size = entry[3]
             energy_response_list.append(energy_response)
-            
+
     return energy_response_list
```

### Comparing `deepview-profile-0.12.2/deepview_profile/analysis/static.py` & `deepview_profile-0.12.3/deepview_profile/analysis/static.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.2/deepview_profile/commands/interactive.py` & `deepview_profile-0.12.3/deepview_profile/commands/interactive.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import logging
 import signal
-import subprocess
 import threading
 
 from deepview_profile.initialization import (
     check_skyline_preconditions,
     initialize_skyline,
 )
 
@@ -44,15 +43,14 @@
         help="The location of the log file.",
     )
     parser.add_argument(
         "--debug", action="store_true", help="Log debug messages.")
     parser.set_defaults(func=main)
 
 def actual_main(args):
-    from deepview_profile.config import Config
     from deepview_profile.server import SkylineServer
 
     should_shutdown = threading.Event()
 
     def signal_handler(signal, frame):
         should_shutdown.set()
```

### Comparing `deepview-profile-0.12.2/deepview_profile/commands/measurements.py` & `deepview_profile-0.12.3/deepview_profile/commands/measurements.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,15 +56,14 @@
     peak_usage_bytes = session.measure_peak_usage_bytes()
     thpt_msg = session.measure_throughput()
     return thpt_msg.samples_per_second, peak_usage_bytes
 
 
 def actual_main(args):
     from deepview_profile.analysis.session import AnalysisSession
-    from deepview_profile.config import Config
     from deepview_profile.exceptions import AnalysisError
 
     if os.path.exists(args.output):
         print(
             "ERROR: The specified output file already exists.",
             file=sys.stderr,
         )
```

### Comparing `deepview-profile-0.12.2/deepview_profile/commands/memory.py` & `deepview_profile-0.12.3/deepview_profile/commands/memory.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     parser.add_argument(
         "--debug", action="store_true", help="Log debug messages.")
     parser.set_defaults(func=main)
 
 
 def actual_main(args):
     from deepview_profile.analysis.session import AnalysisSession
-    from deepview_profile.config import Config
     from deepview_profile.exceptions import AnalysisError
 
     if os.path.exists(args.output):
         print(
             "ERROR: The specified output file already exists.",
             file=sys.stderr,
         )
```

### Comparing `deepview-profile-0.12.2/deepview_profile/commands/prediction_models.py` & `deepview_profile-0.12.3/deepview_profile/commands/prediction_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,14 @@
         (thpt_msg.peak_usage_bytes.slope, thpt_msg.peak_usage_bytes.bias),
         (thpt_msg.run_time_ms.slope, thpt_msg.run_time_ms.bias),
     )
 
 
 def actual_main(args):
     from deepview_profile.analysis.session import AnalysisSession
-    from deepview_profile.config import Config
     from deepview_profile.exceptions import AnalysisError
 
     if os.path.exists(args.output):
         print(
             "ERROR: The specified output file already exists.",
             file=sys.stderr,
         )
```

### Comparing `deepview-profile-0.12.2/deepview_profile/commands/time.py` & `deepview_profile-0.12.3/deepview_profile/commands/time.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,14 @@
     parser.add_argument(
         "--debug", action="store_true", help="Log debug messages.")
     parser.set_defaults(func=main)
 
 
 def actual_main(args):
     from deepview_profile.analysis.session import AnalysisSession
-    from deepview_profile.config import Config
     from deepview_profile.exceptions import AnalysisError
 
     if os.path.exists(args.output):
         print(
             "ERROR: The specified output file already exists.",
             file=sys.stderr,
         )
```

### Comparing `deepview-profile-0.12.2/deepview_profile/config/__init__.py` & `deepview_profile-0.12.3/deepview_profile/config/__init__.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.2/deepview_profile/data/hints.yml` & `deepview_profile-0.12.3/deepview_profile/data/hints.yml`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.2/deepview_profile/db/database.py` & `deepview_profile-0.12.3/deepview_profile/db/database.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-import datetime 
+import datetime
 import os
 import sqlite3
 
 BASE_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 DB_PATH = os.path.join(BASE_DIR, "deepview.sqlite3")
 
 class DatabaseInterface:
     def __init__(self, database_name=DB_PATH) -> None:
-        self.connection = sqlite3.connect(database_name, detect_types=sqlite3.PARSE_DECLTYPES|sqlite3.PARSE_COLNAMES)
+        self.connection = sqlite3.connect(
+            database_name, detect_types=sqlite3.PARSE_DECLTYPES|sqlite3.PARSE_COLNAMES
+        )
         self.create_energy_table()
 
     def create_energy_table(self) -> None:
         self.connection.cursor().execute("CREATE TABLE IF NOT EXISTS ENERGY ( \
             entry_point TEXT, \
             cpu_component REAL, \
             gpu_component REAL, \
@@ -42,17 +44,17 @@
         '''
         return len(entry) == 5 and type(entry[0]) == str and type(entry[1]) == float \
             and type(entry[2]) == float and type(entry[3]) == int \
             and type(entry[4]) == datetime.datetime
 
     def add_entry(self, entry: list) -> bool:
         '''
-        Validates an entry and then adds that entry into the Energy table. Note that current timestamp is added 
-        by this function. Returns False if the entry is not a valid format, or if the insertion failed. Else
-        returns True
+        Validates an entry and then adds that entry into the Energy table. Note that
+        current timestamp is added by this function. Returns False if the entry is
+        not a valid format, or if the insertion failed. Else returns True
         '''
         if self.is_valid_entry(entry):
             try:
                 entry.append(datetime.datetime.now())
                 cursor = self.database_connection.cursor()
                 cursor.execute("INSERT INTO ENERGY VALUES(?, ?, ?, ?, ?)", entry)
                 self.database_connection.commit()
@@ -65,9 +67,12 @@
 
     def get_latest_n_entries_of_entry_point(self, n: int, entry_point: str) -> list:
         '''
         Gets the n latest entries of a given entry point
         '''
         params = [entry_point, n]
         cursor = self.database_connection.cursor()
-        results = cursor.execute("SELECT * FROM ENERGY WHERE entry_point=? ORDER BY ts DESC LIMIT ?;", params).fetchall()
-        return results
+        results = cursor.execute(
+            "SELECT * FROM ENERGY WHERE entry_point=? ORDER BY ts DESC LIMIT ?;",
+            params
+        ).fetchall()
+        return results
```

### Comparing `deepview-profile-0.12.2/deepview_profile/energy/measurer.py` & `deepview_profile-0.12.3/deepview_profile/energy/measurer.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,45 +15,48 @@
     def measurer_init(self):
         self.sensor = None
         try:
             self.sensor = Sensor()
             energy = self.sensor.energy()
             self.last_cpu = np.array(energy[0::2])
             self.last_dram = np.array(energy[1::2])
-        except Exception as e:
-            print("Warning. Failed to get CPU energy. You need to set the right permissions for pyRAPL")
+        except Exception:
+            print("Warning. Failed to get CPU energy. \
+                  You need to set the right permissions for pyRAPL")
             print("eg. $ sudo chmod -R a+r /sys/class/powercap/intel-rapl")
 
     def measurer_measure(self):
         # Get energy consumed so far (since last CPU reset)
-        if self.sensor is None: return
+        if self.sensor is None:
+            return
 
         energy = self.sensor.energy()
         cpu = np.array(energy[0::2])
         dram = np.array(energy[1::2])
 
         # Compare against last measurement to determine energy since last measure
         diff_cpu = cpu - self.last_cpu
-        diff_dram = dram - self.last_dram
-        
+        dram - self.last_dram
+
         # 1J = 10^6 uJ
         # The cpu used this much since the last measurement
         # We have mW = 1000*J/s = 1000*(uJ/10^6)/s
         cpu_total = np.sum(diff_cpu)
         cpu_mW = 1000 * (cpu_total / 1e6) / self.interval
         self.power.append(cpu_mW)
 
         self.last_cpu = cpu
         self.last_dram = dram
 
     def measurer_deallocate(self):
         pass
 
     def total_energy(self):
-        if len(self.power) == 0: return None
+        if len(self.power) == 0:
+            return None
 
         # J = W * s,    1W = 1000 mW
         energy = self.interval * sum(self.power) / 1000.0
         return energy
 
 class GPUMeasurer:
     def __init__(self, interval):
@@ -119,10 +122,10 @@
             e = self.measurers[m].total_energy()
             if e is not None:
                 total_energy += e
         return total_energy
 
     def cpu_energy(self):
         return self.measurers["cpu"].total_energy()
-    
+
     def gpu_energy(self):
         return self.measurers["gpu"].total_energy()
```

### Comparing `deepview-profile-0.12.2/deepview_profile/error_printing.py` & `deepview_profile-0.12.3/deepview_profile/error_printing.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.2/deepview_profile/evaluate.py` & `deepview_profile-0.12.3/deepview_profile/evaluate.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import argparse
-import enum
 import sys
 
 import deepview_profile.commands.measurements
 import deepview_profile.commands.prediction_models
 
 
 def main():
```

### Comparing `deepview-profile-0.12.2/deepview_profile/exceptions.py` & `deepview_profile-0.12.3/deepview_profile/exceptions.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.2/deepview_profile/initialization.py` & `deepview_profile-0.12.3/deepview_profile/initialization.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-import os
 import sys
 
 logger = logging.getLogger(__name__)
 
 
 def check_skyline_preconditions(args):
     """
@@ -38,19 +37,19 @@
     logging.basicConfig(**kwargs)
 
 
 def _validate_dependencies():
     # NOTE: If you make a change here, make sure to update the INSTALL_REQUIRES
     #       list in setup.py as well.
     try:
-        import yaml # pyyaml on PyPI
-        import pynvml # nvidia-ml-py3 on PyPI
-        import google.protobuf # protobuf on PyPI
-        import numpy
-        import torch
+        import yaml # pyyaml on PyPI # noqa: F401
+        import pynvml # nvidia-ml-py3 on PyPI # noqa: F401
+        import google.protobuf # protobuf on PyPI # noqa: F401
+        import numpy # noqa: F401
+        import torch # noqa: F401
         return True
     except ImportError as ex:
         logger.error(
             "DeepView could not find the '%s' module, which is a required "
             "dependency. Please make sure all the required dependencies are "
             "installed before launching DeepView. If you use a package "
             "manager, these dependencies will be automatically installed for "
```

### Comparing `deepview-profile-0.12.2/deepview_profile/io/connection.py` & `deepview_profile-0.12.3/deepview_profile/io/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,25 +87,25 @@
                     try:
                         self._handler_function(
                             buffer[:message_length], self.address)
                     finally:
                         buffer = buffer[message_length:]
                         message_length = -1
 
-        except:
+        except Exception:
             logger.exception("Connection unexpectedly stopping...")
-    
+
     @property
     def project_root(self):
         return self._project_root
 
     @property
     def entry_point(self):
         return self._entry_point
-    
+
     def set_project_paths(self, project_root, entry_point):
         self._project_root = project_root
         self._entry_point = entry_point
 
 class ConnectionState:
     def __init__(self):
         # NOTE: This counter is modified by a thread in the main executor, but
```

### Comparing `deepview-profile-0.12.2/deepview_profile/io/connection_acceptor.py` & `deepview_profile-0.12.3/deepview_profile/io/connection_acceptor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-import os
+import logging
 import select
 import socket
-import logging
 from threading import Thread
 
 from deepview_profile.io.sentinel import Sentinel
 
 logger = logging.getLogger(__name__)
 
 
@@ -74,10 +73,10 @@
                     self._sentinel.consume_exit_signal()
                     break
 
                 socket, address = self._server_socket.accept()
                 host, port = address
                 logger.debug("Accepted a connection to (%s:%d).", host, port)
                 self._handler_function(socket, address)
-        except:
+        except Exception:
             logging.exception(
                 "DeepView has unexpectedly stopped accepting connections.")
```

### Comparing `deepview-profile-0.12.2/deepview_profile/io/connection_manager.py` & `deepview_profile-0.12.3/deepview_profile/io/connection_manager.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.2/deepview_profile/io/sentinel.py` & `deepview_profile-0.12.3/deepview_profile/io/sentinel.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.2/deepview_profile/lru_cache.py` & `deepview_profile-0.12.3/deepview_profile/lru_cache.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.2/deepview_profile/models/analysis.py` & `deepview_profile-0.12.3/deepview_profile/models/analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from deepview_profile.models.source_map import Position
 
 
 class OperationInfo:
     def __init__(self, bound_name, op_name, ast_node, position, perf_hints):
         self.bound_name = bound_name
         self.op_name = op_name
         self.ast_node = ast_node
```

### Comparing `deepview-profile-0.12.2/deepview_profile/models/source_map.py` & `deepview_profile-0.12.3/deepview_profile/models/source_map.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.2/deepview_profile/profiler/__init__.py` & `deepview_profile-0.12.3/deepview_profile/profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.2/deepview_profile/profiler/autograd.py` & `deepview_profile-0.12.3/deepview_profile/profiler/autograd.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.2/deepview_profile/profiler/backward.py` & `deepview_profile-0.12.3/deepview_profile/profiler/backward.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.2/deepview_profile/profiler/iteration.py` & `deepview_profile-0.12.3/deepview_profile/profiler/iteration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import collections
 import logging
-
 import torch
 
 from deepview_profile.exceptions import AnalysisError
 from deepview_profile.user_code_utils import user_code_environment
+from deepview_profile.utils import release_memory
 
 logger = logging.getLogger(__name__)
 
 IterationSample = collections.namedtuple(
     "IterationSample", ["batch_size", "run_time_ms", "peak_usage_bytes"])
 
 
@@ -45,14 +45,15 @@
     def measure_run_time_ms(self, batch_size, initial_repetitions=None):
         """
         Measures the iteration run time in milliseconds.
 
         NOTE: This method will raise a RuntimeError if there is not enough GPU
               memory to run the iteration.
         """
+
         with user_code_environment(
                 self._path_to_entry_point_dir, self._project_root):
             inputs = self._input_provider(batch_size=batch_size)
             # Warm up
             self._iteration(*inputs)
 
         torch.cuda.synchronize()
@@ -92,29 +93,31 @@
         min_profile_time_ms = 2000
         max_repetitions = max(max_repetitions, min_profile_time_ms / lesser)
 
         logger.debug("Iters: %d, Measured: %f", repetitions, lesser)
         while repetitions <= max_repetitions:
             doubled = repetitions * 2
             greater = measure(doubled) / doubled
-            logger.debug("Iters: %d, Measured: %f (range: %f)", doubled, greater, max(lesser, greater) / min(lesser, greater))
+            logger.debug("Iters: %d, Measured: %f (range: %f)",\
+                         doubled, greater, max(lesser, greater) / min(lesser, greater))
 
             # Stop when the difference between the measurements is less than 5%
             if (max(lesser, greater) / min(lesser, greater)) < 1.05:
                 break
 
             repetitions = doubled
             lesser = greater
 
         return min(lesser, greater), peak_usage_bytes, repetitions
 
     def measure_run_time_ms_catch_oom(
             self, batch_size, initial_repetitions=None):
         # This function is useful when we want to explicitly handle OOM errors
         # without aborting the profiling.
+        release_memory()
         try:
             return (
                 None,
                 self.measure_run_time_ms(batch_size, initial_repetitions),
             )
         except AnalysisError as ex:
             message = str(ex)
@@ -215,10 +218,10 @@
         base = lower if is_increasing else upper
         mult = 1 if is_increasing else -1
 
         # increase the growth amount for batch sizes to better account for small
         # models whose initial batch size is much smaller than the maximum possible.
         tiers = [100, 20, 10, 5]
         for t in tiers:
-            if diff >= t: return base + mult * t
-
+            if diff >= t:
+                return base + mult * t
         return base + mult
```

### Comparing `deepview-profile-0.12.2/deepview_profile/profiler/operation.py` & `deepview_profile-0.12.3/deepview_profile/profiler/operation.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.2/deepview_profile/protocol/message_handler.py` & `deepview_profile-0.12.3/deepview_profile/protocol/message_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import collections
 import logging
 import os
 
-from deepview_profile.exceptions import AnalysisError, NoConnectionError
+from deepview_profile.exceptions import NoConnectionError
 
 import deepview_profile.protocol_gen.innpv_pb2 as pm
 
 logger = logging.getLogger(__name__)
 
 RequestContext = collections.namedtuple(
     'RequestContext',
@@ -76,30 +76,31 @@
             self._connection_manager.remove_connection(context.address)
             logger.error(
                 'DeepView is out of date. Please update to the latest versions '
                 'of the DeepView command line interface and plugin.'
             )
             return
 
-        
+
         if not _validate_paths(message.project_root,  message.entry_point):
-            # Change this to the error related to 
+            # Change this to the error related to
             self._message_sender.send_protocol_error(
                 pm.ProtocolError.ErrorCode.UNSUPPORTED_PROTOCOL_VERSION,
                 context,
             )
             self._connection_manager.remove_connection(context.address)
             logger.error(
                 'Invalid project root or entry point.'
             )
             return
         logger.info("Connection addr:(%s:%d)", *context.address)
         logger.info("Project Root:   %s", message.project_root)
         logger.info("Entry Point:    %s", message.entry_point)
-        self._connection_manager.get_connection(context.address).set_project_paths(message.project_root, message.entry_point)
+        self._connection_manager.get_connection(context.address)\
+            .set_project_paths(message.project_root, message.entry_point)
 
         context.state.initialized = True
         self._message_sender.send_initialize_response(context)
 
     def _handle_analysis_request(self, message, context):
         if not context.state.initialized:
             self._message_sender.send_protocol_error(
@@ -146,13 +147,12 @@
                     'Invalid message type "{}".'.format(message_type))
         except NoConnectionError:
             logger.debug(
                 'Dropping message from (%s:%d) because it is no longer '
                 'connected.',
                 *address,
             )
-        except:
+        except Exception:
             logger.exception(
                 'Processing message from (%s:%d) resulted in an exception.',
                 *address,
             )
-
```

### Comparing `deepview-profile-0.12.2/deepview_profile/protocol/message_sender.py` & `deepview_profile-0.12.3/deepview_profile/protocol/message_sender.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import os
 import logging
 import pynvml
 import platform
-from random import random
 
-from deepview_profile.config import Config
 from deepview_profile.exceptions import NoConnectionError
 
 import deepview_profile.protocol_gen.innpv_pb2 as pm
 
 logger = logging.getLogger(__name__)
 
 
@@ -60,15 +58,15 @@
         self._send_message(message, 'analysis_error', context)
 
     def send_throughput_response(self, throughput, context):
         self._send_message(throughput, 'throughput', context)
 
     def send_habitat_response(self, habitat_resp, context):
         self._send_message(habitat_resp, 'habitat', context)
-    
+
     def send_energy_response(self, energy_resp, context):
         self._send_message(energy_resp, 'energy', context)
 
     def _send_message(self, message, payload_name, context):
         try:
             connection = self._connection_manager.get_connection(
                 context.address)
```

### Comparing `deepview-profile-0.12.2/deepview_profile/protocol_gen/innpv_pb2.py` & `deepview_profile-0.12.3/deepview_profile/protocol_gen/innpv_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='innpv.proto',
   package='innpv.protocol',
   syntax='proto3',
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\x0binnpv.proto\x12\x0einnpv.protocol\"\xcf\x01\n\nFromClient\x12\x17\n\x0fsequence_number\x18\x01 \x01(\r\x12\x37\n\ninitialize\x18\x02 \x01(\x0b\x32!.innpv.protocol.InitializeRequestH\x00\x12\x33\n\x08\x61nalysis\x18\x03 \x01(\x0b\x32\x1f.innpv.protocol.AnalysisRequestH\x00\x12/\n\x07generic\x18\x04 \x01(\x0b\x32\x1c.innpv.protocol.GenericEventH\x00\x42\t\n\x07payload\">\n\x0cGenericEvent\x12\x12\n\nevent_type\x18\x01 \x01(\t\x12\x1a\n\x12optional_arguments\x18\x02 \x01(\t\"X\n\x11InitializeRequest\x12\x18\n\x10protocol_version\x18\x01 \x01(\r\x12\x14\n\x0cproject_root\x18\x02 \x01(\t\x12\x13\n\x0b\x65ntry_point\x18\x03 \x01(\t\"(\n\x0f\x41nalysisRequest\x12\x15\n\rmock_response\x18\x01 \x01(\x08\"\xcf\x03\n\nFromServer\x12\x17\n\x0fsequence_number\x18\x01 \x01(\r\x12.\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x1d.innpv.protocol.ProtocolErrorH\x00\x12\x38\n\ninitialize\x18\x03 \x01(\x0b\x32\".innpv.protocol.InitializeResponseH\x00\x12\x37\n\x0e\x61nalysis_error\x18\x05 \x01(\x0b\x32\x1d.innpv.protocol.AnalysisErrorH\x00\x12\x38\n\nthroughput\x18\x06 \x01(\x0b\x32\".innpv.protocol.ThroughputResponseH\x00\x12\x36\n\tbreakdown\x18\x08 \x01(\x0b\x32!.innpv.protocol.BreakdownResponseH\x00\x12\x32\n\x07habitat\x18\t \x01(\x0b\x32\x1f.innpv.protocol.HabitatResponseH\x00\x12\x30\n\x06\x65nergy\x18\n \x01(\x0b\x32\x1e.innpv.protocol.EnergyResponseH\x00\x42\t\n\x07payloadJ\x04\x08\x04\x10\x05J\x04\x08\x07\x10\x08R\x0cmemory_usageR\x08run_time\"B\n\x17HabitatDevicePrediction\x12\x13\n\x0b\x64\x65vice_name\x18\x01 \x01(\t\x12\x12\n\nruntime_ms\x18\x02 \x01(\x02\"O\n\x0fHabitatResponse\x12<\n\x0bpredictions\x18\x01 \x03(\x0b\x32\'.innpv.protocol.HabitatDevicePrediction\"\xba\x01\n\x0e\x45nergyResponse\x12\x19\n\x11total_consumption\x18\x01 \x01(\x02\x12>\n\ncomponents\x18\x02 \x03(\x0b\x32*.innpv.protocol.EnergyConsumptionComponent\x12\x12\n\nbatch_size\x18\x03 \x01(\x05\x12\x39\n\x11past_measurements\x18\x04 \x03(\x0b\x32\x1e.innpv.protocol.EnergyResponse\"\x80\x01\n\x1a\x45nergyConsumptionComponent\x12\x46\n\x0e\x63omponent_type\x18\x01 \x01(\x0e\x32..innpv.protocol.EnergyConsumptionComponentType\x12\x1a\n\x12\x63onsumption_joules\x18\x02 \x01(\x02\"\x8c\x01\n\x12InitializeResponse\x12\x1b\n\x13server_project_root\x18\x01 \x01(\t\x12)\n\x0b\x65ntry_point\x18\x02 \x01(\x0b\x32\x14.innpv.protocol.Path\x12.\n\x08hardware\x18\x03 \x01(\x0b\x32\x1c.innpv.protocol.HardwareInfo\"[\n\rAnalysisError\x12\x15\n\rerror_message\x18\x01 \x01(\t\x12\x33\n\x0c\x66ile_context\x18\x02 \x01(\x0b\x32\x1d.innpv.protocol.FileReference\"\xa1\x02\n\x12ThroughputResponse\x12\x1a\n\x12samples_per_second\x18\x01 \x01(\x02\x12(\n predicted_max_samples_per_second\x18\x02 \x01(\x02\x12\x30\n\x0brun_time_ms\x18\x03 \x01(\x0b\x32\x1b.innpv.protocol.LinearModel\x12\x35\n\x10peak_usage_bytes\x18\x04 \x01(\x0b\x32\x1b.innpv.protocol.LinearModel\x12\x39\n\x12\x62\x61tch_size_context\x18\x05 \x01(\x0b\x32\x1d.innpv.protocol.FileReference\x12!\n\x19\x63\x61n_manipulate_batch_size\x18\x06 \x01(\x08\"\xea\x01\n\x11\x42reakdownResponse\x12\x18\n\x10peak_usage_bytes\x18\x01 \x01(\x04\x12\x1d\n\x15memory_capacity_bytes\x18\x02 \x01(\x04\x12\x1d\n\x15iteration_run_time_ms\x18\x03 \x01(\x02\x12\x12\n\nbatch_size\x18\x06 \x01(\r\x12\x35\n\x0eoperation_tree\x18\x04 \x03(\x0b\x32\x1d.innpv.protocol.BreakdownNode\x12\x32\n\x0bweight_tree\x18\x05 \x03(\x0b\x32\x1d.innpv.protocol.BreakdownNode\"\xca\x01\n\rProtocolError\x12;\n\nerror_code\x18\x01 \x01(\x0e\x32\'.innpv.protocol.ProtocolError.ErrorCode\"|\n\tErrorCode\x12\x0b\n\x07UNKNOWN\x10\x00\x12 \n\x1cUNSUPPORTED_PROTOCOL_VERSION\x10\x01\x12\x1c\n\x18UNINITIALIZED_CONNECTION\x10\x02\x12\"\n\x1e\x41LREADY_INITIALIZED_CONNECTION\x10\x03\"\x1a\n\x04Path\x12\x12\n\ncomponents\x18\x01 \x03(\t\"M\n\rFileReference\x12\'\n\tfile_path\x18\x01 \x01(\x0b\x32\x14.innpv.protocol.Path\x12\x13\n\x0bline_number\x18\x02 \x01(\r\"\xce\x01\n\rBreakdownNode\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x14\n\x0cnum_children\x18\x02 \x01(\r\x12/\n\x08\x63ontexts\x18\x03 \x03(\x0b\x32\x1d.innpv.protocol.FileReference\x12\x32\n\toperation\x18\x04 \x01(\x0b\x32\x1d.innpv.protocol.OperationDataH\x00\x12,\n\x06weight\x18\x05 \x01(\x0b\x32\x1a.innpv.protocol.WeightDataH\x00\x42\x06\n\x04\x64\x61ta\"{\n\x0b\x43ontextInfo\x12.\n\x07\x63ontext\x18\x01 \x01(\x0b\x32\x1d.innpv.protocol.FileReference\x12\x13\n\x0brun_time_ms\x18\x02 \x01(\x02\x12\x12\n\nsize_bytes\x18\x03 \x01(\x04\x12\x13\n\x0binvocations\x18\x04 \x01(\r\"\x83\x01\n\rOperationData\x12\x12\n\nforward_ms\x18\x01 \x01(\x02\x12\x13\n\x0b\x62\x61\x63kward_ms\x18\x02 \x01(\x02\x12\x12\n\nsize_bytes\x18\x03 \x01(\x04\x12\x35\n\x10\x63ontext_info_map\x18\x04 \x03(\x0b\x32\x1b.innpv.protocol.ContextInfo\"9\n\nWeightData\x12\x12\n\nsize_bytes\x18\x01 \x01(\x04\x12\x17\n\x0fgrad_size_bytes\x18\x02 \x01(\x04\"*\n\x0bLinearModel\x12\r\n\x05slope\x18\x01 \x01(\x01\x12\x0c\n\x04\x62ias\x18\x02 \x01(\x01\":\n\x0cHardwareInfo\x12\x10\n\x08hostname\x18\x01 \x01(\t\x12\n\n\x02os\x18\x02 \x01(\t\x12\x0c\n\x04gpus\x18\x03 \x03(\t\"\x1b\n\x13MemoryUsageResponseJ\x04\x08\x01\x10\x65\"\x17\n\x0fRunTimeResponseJ\x04\x08\x01\x10\x65\"\x17\n\x0f\x41\x63tivationEntryJ\x04\x08\x01\x10\x65\"\x13\n\x0bWeightEntryJ\x04\x08\x01\x10\x65\"\x14\n\x0cRunTimeEntryJ\x04\x08\x01\x10\x65*`\n\x1e\x45nergyConsumptionComponentType\x12\x16\n\x12\x45NERGY_UNSPECIFIED\x10\x00\x12\x13\n\x0f\x45NERGY_CPU_DRAM\x10\x01\x12\x11\n\rENERGY_NVIDIA\x10\x02\x62\x06proto3'
+  serialized_pb=b'\n\x0binnpv.proto\x12\x0einnpv.protocol\"\xcf\x01\n\nFromClient\x12\x17\n\x0fsequence_number\x18\x01 \x01(\r\x12\x37\n\ninitialize\x18\x02 \x01(\x0b\x32!.innpv.protocol.InitializeRequestH\x00\x12\x33\n\x08\x61nalysis\x18\x03 \x01(\x0b\x32\x1f.innpv.protocol.AnalysisRequestH\x00\x12/\n\x07generic\x18\x04 \x01(\x0b\x32\x1c.innpv.protocol.GenericEventH\x00\x42\t\n\x07payload\">\n\x0cGenericEvent\x12\x12\n\nevent_type\x18\x01 \x01(\t\x12\x1a\n\x12optional_arguments\x18\x02 \x01(\t\"X\n\x11InitializeRequest\x12\x18\n\x10protocol_version\x18\x01 \x01(\r\x12\x14\n\x0cproject_root\x18\x02 \x01(\t\x12\x13\n\x0b\x65ntry_point\x18\x03 \x01(\t\"(\n\x0f\x41nalysisRequest\x12\x15\n\rmock_response\x18\x01 \x01(\x08\"\xcf\x03\n\nFromServer\x12\x17\n\x0fsequence_number\x18\x01 \x01(\r\x12.\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x1d.innpv.protocol.ProtocolErrorH\x00\x12\x38\n\ninitialize\x18\x03 \x01(\x0b\x32\".innpv.protocol.InitializeResponseH\x00\x12\x37\n\x0e\x61nalysis_error\x18\x05 \x01(\x0b\x32\x1d.innpv.protocol.AnalysisErrorH\x00\x12\x38\n\nthroughput\x18\x06 \x01(\x0b\x32\".innpv.protocol.ThroughputResponseH\x00\x12\x36\n\tbreakdown\x18\x08 \x01(\x0b\x32!.innpv.protocol.BreakdownResponseH\x00\x12\x32\n\x07habitat\x18\t \x01(\x0b\x32\x1f.innpv.protocol.HabitatResponseH\x00\x12\x30\n\x06\x65nergy\x18\n \x01(\x0b\x32\x1e.innpv.protocol.EnergyResponseH\x00\x42\t\n\x07payloadJ\x04\x08\x04\x10\x05J\x04\x08\x07\x10\x08R\x0cmemory_usageR\x08run_time\"B\n\x17HabitatDevicePrediction\x12\x13\n\x0b\x64\x65vice_name\x18\x01 \x01(\t\x12\x12\n\nruntime_ms\x18\x02 \x01(\x02\"\x86\x01\n\x0fHabitatResponse\x12<\n\x0bpredictions\x18\x01 \x03(\x0b\x32\'.innpv.protocol.HabitatDevicePrediction\x12\x35\n\x0e\x61nalysis_error\x18\x02 \x01(\x0b\x32\x1d.innpv.protocol.AnalysisError\"\xf1\x01\n\x0e\x45nergyResponse\x12\x19\n\x11total_consumption\x18\x01 \x01(\x02\x12>\n\ncomponents\x18\x02 \x03(\x0b\x32*.innpv.protocol.EnergyConsumptionComponent\x12\x12\n\nbatch_size\x18\x03 \x01(\x05\x12\x39\n\x11past_measurements\x18\x04 \x03(\x0b\x32\x1e.innpv.protocol.EnergyResponse\x12\x35\n\x0e\x61nalysis_error\x18\x05 \x01(\x0b\x32\x1d.innpv.protocol.AnalysisError\"\x80\x01\n\x1a\x45nergyConsumptionComponent\x12\x46\n\x0e\x63omponent_type\x18\x01 \x01(\x0e\x32..innpv.protocol.EnergyConsumptionComponentType\x12\x1a\n\x12\x63onsumption_joules\x18\x02 \x01(\x02\"\x8c\x01\n\x12InitializeResponse\x12\x1b\n\x13server_project_root\x18\x01 \x01(\t\x12)\n\x0b\x65ntry_point\x18\x02 \x01(\x0b\x32\x14.innpv.protocol.Path\x12.\n\x08hardware\x18\x03 \x01(\x0b\x32\x1c.innpv.protocol.HardwareInfo\"[\n\rAnalysisError\x12\x15\n\rerror_message\x18\x01 \x01(\t\x12\x33\n\x0c\x66ile_context\x18\x02 \x01(\x0b\x32\x1d.innpv.protocol.FileReference\"\xa1\x02\n\x12ThroughputResponse\x12\x1a\n\x12samples_per_second\x18\x01 \x01(\x02\x12(\n predicted_max_samples_per_second\x18\x02 \x01(\x02\x12\x30\n\x0brun_time_ms\x18\x03 \x01(\x0b\x32\x1b.innpv.protocol.LinearModel\x12\x35\n\x10peak_usage_bytes\x18\x04 \x01(\x0b\x32\x1b.innpv.protocol.LinearModel\x12\x39\n\x12\x62\x61tch_size_context\x18\x05 \x01(\x0b\x32\x1d.innpv.protocol.FileReference\x12!\n\x19\x63\x61n_manipulate_batch_size\x18\x06 \x01(\x08\"\xea\x01\n\x11\x42reakdownResponse\x12\x18\n\x10peak_usage_bytes\x18\x01 \x01(\x04\x12\x1d\n\x15memory_capacity_bytes\x18\x02 \x01(\x04\x12\x1d\n\x15iteration_run_time_ms\x18\x03 \x01(\x02\x12\x12\n\nbatch_size\x18\x06 \x01(\r\x12\x35\n\x0eoperation_tree\x18\x04 \x03(\x0b\x32\x1d.innpv.protocol.BreakdownNode\x12\x32\n\x0bweight_tree\x18\x05 \x03(\x0b\x32\x1d.innpv.protocol.BreakdownNode\"\xca\x01\n\rProtocolError\x12;\n\nerror_code\x18\x01 \x01(\x0e\x32\'.innpv.protocol.ProtocolError.ErrorCode\"|\n\tErrorCode\x12\x0b\n\x07UNKNOWN\x10\x00\x12 \n\x1cUNSUPPORTED_PROTOCOL_VERSION\x10\x01\x12\x1c\n\x18UNINITIALIZED_CONNECTION\x10\x02\x12\"\n\x1e\x41LREADY_INITIALIZED_CONNECTION\x10\x03\"\x1a\n\x04Path\x12\x12\n\ncomponents\x18\x01 \x03(\t\"M\n\rFileReference\x12\'\n\tfile_path\x18\x01 \x01(\x0b\x32\x14.innpv.protocol.Path\x12\x13\n\x0bline_number\x18\x02 \x01(\r\"\xce\x01\n\rBreakdownNode\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x14\n\x0cnum_children\x18\x02 \x01(\r\x12/\n\x08\x63ontexts\x18\x03 \x03(\x0b\x32\x1d.innpv.protocol.FileReference\x12\x32\n\toperation\x18\x04 \x01(\x0b\x32\x1d.innpv.protocol.OperationDataH\x00\x12,\n\x06weight\x18\x05 \x01(\x0b\x32\x1a.innpv.protocol.WeightDataH\x00\x42\x06\n\x04\x64\x61ta\"{\n\x0b\x43ontextInfo\x12.\n\x07\x63ontext\x18\x01 \x01(\x0b\x32\x1d.innpv.protocol.FileReference\x12\x13\n\x0brun_time_ms\x18\x02 \x01(\x02\x12\x12\n\nsize_bytes\x18\x03 \x01(\x04\x12\x13\n\x0binvocations\x18\x04 \x01(\r\"\x83\x01\n\rOperationData\x12\x12\n\nforward_ms\x18\x01 \x01(\x02\x12\x13\n\x0b\x62\x61\x63kward_ms\x18\x02 \x01(\x02\x12\x12\n\nsize_bytes\x18\x03 \x01(\x04\x12\x35\n\x10\x63ontext_info_map\x18\x04 \x03(\x0b\x32\x1b.innpv.protocol.ContextInfo\"9\n\nWeightData\x12\x12\n\nsize_bytes\x18\x01 \x01(\x04\x12\x17\n\x0fgrad_size_bytes\x18\x02 \x01(\x04\"*\n\x0bLinearModel\x12\r\n\x05slope\x18\x01 \x01(\x01\x12\x0c\n\x04\x62ias\x18\x02 \x01(\x01\":\n\x0cHardwareInfo\x12\x10\n\x08hostname\x18\x01 \x01(\t\x12\n\n\x02os\x18\x02 \x01(\t\x12\x0c\n\x04gpus\x18\x03 \x03(\t\"\x1b\n\x13MemoryUsageResponseJ\x04\x08\x01\x10\x65\"\x17\n\x0fRunTimeResponseJ\x04\x08\x01\x10\x65\"\x17\n\x0f\x41\x63tivationEntryJ\x04\x08\x01\x10\x65\"\x13\n\x0bWeightEntryJ\x04\x08\x01\x10\x65\"\x14\n\x0cRunTimeEntryJ\x04\x08\x01\x10\x65*`\n\x1e\x45nergyConsumptionComponentType\x12\x16\n\x12\x45NERGY_UNSPECIFIED\x10\x00\x12\x13\n\x0f\x45NERGY_CPU_DRAM\x10\x01\x12\x11\n\rENERGY_NVIDIA\x10\x02\x62\x06proto3'
 )
 
 _ENERGYCONSUMPTIONCOMPONENTTYPE = _descriptor.EnumDescriptor(
   name='EnergyConsumptionComponentType',
   full_name='innpv.protocol.EnergyConsumptionComponentType',
   filename=None,
   file=DESCRIPTOR,
@@ -44,16 +44,16 @@
       name='ENERGY_NVIDIA', index=2, number=2,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=3202,
-  serialized_end=3298,
+  serialized_start=3313,
+  serialized_end=3409,
 )
 _sym_db.RegisterEnumDescriptor(_ENERGYCONSUMPTIONCOMPONENTTYPE)
 
 EnergyConsumptionComponentType = enum_type_wrapper.EnumTypeWrapper(_ENERGYCONSUMPTIONCOMPONENTTYPE)
 ENERGY_UNSPECIFIED = 0
 ENERGY_CPU_DRAM = 1
 ENERGY_NVIDIA = 2
@@ -85,16 +85,16 @@
       name='ALREADY_INITIALIZED_CONNECTION', index=3, number=3,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=2216,
-  serialized_end=2340,
+  serialized_start=2327,
+  serialized_end=2451,
 )
 _sym_db.RegisterEnumDescriptor(_PROTOCOLERROR_ERRORCODE)
 
 
 _FROMCLIENT = _descriptor.Descriptor(
   name='FromClient',
   full_name='innpv.protocol.FromClient',
@@ -406,28 +406,35 @@
     _descriptor.FieldDescriptor(
       name='predictions', full_name='innpv.protocol.HabitatResponse.predictions', index=0,
       number=1, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='analysis_error', full_name='innpv.protocol.HabitatResponse.analysis_error', index=1,
+      number=2, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
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
-  serialized_start=971,
-  serialized_end=1050,
+  serialized_start=972,
+  serialized_end=1106,
 )
 
 
 _ENERGYRESPONSE = _descriptor.Descriptor(
   name='EnergyResponse',
   full_name='innpv.protocol.EnergyResponse',
   filename=None,
@@ -459,28 +466,35 @@
     _descriptor.FieldDescriptor(
       name='past_measurements', full_name='innpv.protocol.EnergyResponse.past_measurements', index=3,
       number=4, type=11, cpp_type=10, label=3,
       has_default_value=False, default_value=[],
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='analysis_error', full_name='innpv.protocol.EnergyResponse.analysis_error', index=4,
+      number=5, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
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
-  serialized_start=1053,
-  serialized_end=1239,
+  serialized_start=1109,
+  serialized_end=1350,
 )
 
 
 _ENERGYCONSUMPTIONCOMPONENT = _descriptor.Descriptor(
   name='EnergyConsumptionComponent',
   full_name='innpv.protocol.EnergyConsumptionComponent',
   filename=None,
@@ -510,16 +524,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1242,
-  serialized_end=1370,
+  serialized_start=1353,
+  serialized_end=1481,
 )
 
 
 _INITIALIZERESPONSE = _descriptor.Descriptor(
   name='InitializeResponse',
   full_name='innpv.protocol.InitializeResponse',
   filename=None,
@@ -556,16 +570,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1373,
-  serialized_end=1513,
+  serialized_start=1484,
+  serialized_end=1624,
 )
 
 
 _ANALYSISERROR = _descriptor.Descriptor(
   name='AnalysisError',
   full_name='innpv.protocol.AnalysisError',
   filename=None,
@@ -595,16 +609,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1515,
-  serialized_end=1606,
+  serialized_start=1626,
+  serialized_end=1717,
 )
 
 
 _THROUGHPUTRESPONSE = _descriptor.Descriptor(
   name='ThroughputResponse',
   full_name='innpv.protocol.ThroughputResponse',
   filename=None,
@@ -662,16 +676,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1609,
-  serialized_end=1898,
+  serialized_start=1720,
+  serialized_end=2009,
 )
 
 
 _BREAKDOWNRESPONSE = _descriptor.Descriptor(
   name='BreakdownResponse',
   full_name='innpv.protocol.BreakdownResponse',
   filename=None,
@@ -729,16 +743,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1901,
-  serialized_end=2135,
+  serialized_start=2012,
+  serialized_end=2246,
 )
 
 
 _PROTOCOLERROR = _descriptor.Descriptor(
   name='ProtocolError',
   full_name='innpv.protocol.ProtocolError',
   filename=None,
@@ -762,16 +776,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2138,
-  serialized_end=2340,
+  serialized_start=2249,
+  serialized_end=2451,
 )
 
 
 _PATH = _descriptor.Descriptor(
   name='Path',
   full_name='innpv.protocol.Path',
   filename=None,
@@ -794,16 +808,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2342,
-  serialized_end=2368,
+  serialized_start=2453,
+  serialized_end=2479,
 )
 
 
 _FILEREFERENCE = _descriptor.Descriptor(
   name='FileReference',
   full_name='innpv.protocol.FileReference',
   filename=None,
@@ -833,16 +847,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2370,
-  serialized_end=2447,
+  serialized_start=2481,
+  serialized_end=2558,
 )
 
 
 _BREAKDOWNNODE = _descriptor.Descriptor(
   name='BreakdownNode',
   full_name='innpv.protocol.BreakdownNode',
   filename=None,
@@ -898,16 +912,16 @@
   oneofs=[
     _descriptor.OneofDescriptor(
       name='data', full_name='innpv.protocol.BreakdownNode.data',
       index=0, containing_type=None,
       create_key=_descriptor._internal_create_key,
     fields=[]),
   ],
-  serialized_start=2450,
-  serialized_end=2656,
+  serialized_start=2561,
+  serialized_end=2767,
 )
 
 
 _CONTEXTINFO = _descriptor.Descriptor(
   name='ContextInfo',
   full_name='innpv.protocol.ContextInfo',
   filename=None,
@@ -951,16 +965,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2658,
-  serialized_end=2781,
+  serialized_start=2769,
+  serialized_end=2892,
 )
 
 
 _OPERATIONDATA = _descriptor.Descriptor(
   name='OperationData',
   full_name='innpv.protocol.OperationData',
   filename=None,
@@ -1004,16 +1018,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2784,
-  serialized_end=2915,
+  serialized_start=2895,
+  serialized_end=3026,
 )
 
 
 _WEIGHTDATA = _descriptor.Descriptor(
   name='WeightData',
   full_name='innpv.protocol.WeightData',
   filename=None,
@@ -1043,16 +1057,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2917,
-  serialized_end=2974,
+  serialized_start=3028,
+  serialized_end=3085,
 )
 
 
 _LINEARMODEL = _descriptor.Descriptor(
   name='LinearModel',
   full_name='innpv.protocol.LinearModel',
   filename=None,
@@ -1082,16 +1096,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2976,
-  serialized_end=3018,
+  serialized_start=3087,
+  serialized_end=3129,
 )
 
 
 _HARDWAREINFO = _descriptor.Descriptor(
   name='HardwareInfo',
   full_name='innpv.protocol.HardwareInfo',
   filename=None,
@@ -1128,16 +1142,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3020,
-  serialized_end=3078,
+  serialized_start=3131,
+  serialized_end=3189,
 )
 
 
 _MEMORYUSAGERESPONSE = _descriptor.Descriptor(
   name='MemoryUsageResponse',
   full_name='innpv.protocol.MemoryUsageResponse',
   filename=None,
@@ -1153,16 +1167,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3080,
-  serialized_end=3107,
+  serialized_start=3191,
+  serialized_end=3218,
 )
 
 
 _RUNTIMERESPONSE = _descriptor.Descriptor(
   name='RunTimeResponse',
   full_name='innpv.protocol.RunTimeResponse',
   filename=None,
@@ -1178,16 +1192,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3109,
-  serialized_end=3132,
+  serialized_start=3220,
+  serialized_end=3243,
 )
 
 
 _ACTIVATIONENTRY = _descriptor.Descriptor(
   name='ActivationEntry',
   full_name='innpv.protocol.ActivationEntry',
   filename=None,
@@ -1203,16 +1217,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3134,
-  serialized_end=3157,
+  serialized_start=3245,
+  serialized_end=3268,
 )
 
 
 _WEIGHTENTRY = _descriptor.Descriptor(
   name='WeightEntry',
   full_name='innpv.protocol.WeightEntry',
   filename=None,
@@ -1228,16 +1242,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3159,
-  serialized_end=3178,
+  serialized_start=3270,
+  serialized_end=3289,
 )
 
 
 _RUNTIMEENTRY = _descriptor.Descriptor(
   name='RunTimeEntry',
   full_name='innpv.protocol.RunTimeEntry',
   filename=None,
@@ -1253,16 +1267,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3180,
-  serialized_end=3200,
+  serialized_start=3291,
+  serialized_end=3311,
 )
 
 _FROMCLIENT.fields_by_name['initialize'].message_type = _INITIALIZEREQUEST
 _FROMCLIENT.fields_by_name['analysis'].message_type = _ANALYSISREQUEST
 _FROMCLIENT.fields_by_name['generic'].message_type = _GENERICEVENT
 _FROMCLIENT.oneofs_by_name['payload'].fields.append(
   _FROMCLIENT.fields_by_name['initialize'])
@@ -1298,16 +1312,18 @@
 _FROMSERVER.oneofs_by_name['payload'].fields.append(
   _FROMSERVER.fields_by_name['habitat'])
 _FROMSERVER.fields_by_name['habitat'].containing_oneof = _FROMSERVER.oneofs_by_name['payload']
 _FROMSERVER.oneofs_by_name['payload'].fields.append(
   _FROMSERVER.fields_by_name['energy'])
 _FROMSERVER.fields_by_name['energy'].containing_oneof = _FROMSERVER.oneofs_by_name['payload']
 _HABITATRESPONSE.fields_by_name['predictions'].message_type = _HABITATDEVICEPREDICTION
+_HABITATRESPONSE.fields_by_name['analysis_error'].message_type = _ANALYSISERROR
 _ENERGYRESPONSE.fields_by_name['components'].message_type = _ENERGYCONSUMPTIONCOMPONENT
 _ENERGYRESPONSE.fields_by_name['past_measurements'].message_type = _ENERGYRESPONSE
+_ENERGYRESPONSE.fields_by_name['analysis_error'].message_type = _ANALYSISERROR
 _ENERGYCONSUMPTIONCOMPONENT.fields_by_name['component_type'].enum_type = _ENERGYCONSUMPTIONCOMPONENTTYPE
 _INITIALIZERESPONSE.fields_by_name['entry_point'].message_type = _PATH
 _INITIALIZERESPONSE.fields_by_name['hardware'].message_type = _HARDWAREINFO
 _ANALYSISERROR.fields_by_name['file_context'].message_type = _FILEREFERENCE
 _THROUGHPUTRESPONSE.fields_by_name['run_time_ms'].message_type = _LINEARMODEL
 _THROUGHPUTRESPONSE.fields_by_name['peak_usage_bytes'].message_type = _LINEARMODEL
 _THROUGHPUTRESPONSE.fields_by_name['batch_size_context'].message_type = _FILEREFERENCE
```

### Comparing `deepview-profile-0.12.2/deepview_profile/server.py` & `deepview_profile-0.12.3/deepview_profile/server.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.2/deepview_profile/skyline.py` & `deepview_profile-0.12.3/deepview_profile/skyline.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import argparse
-import enum
 import sys
 
-import toml
 
 import deepview_profile
 import deepview_profile.commands.interactive
 import deepview_profile.commands.memory
 import deepview_profile.commands.time
```

### Comparing `deepview-profile-0.12.2/deepview_profile/tests/test_lru_cache.py` & `deepview_profile-0.12.3/deepview_profile/tests/test_lru_cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         self.assertEqual(self.list.size, 3)
         self.assertNotEqual(self.list.front, self.list.back)
         self.assertEqual(self.list_to_array(), [(3, 3), (2, 2), (1, 1)])
 
     def test_list_move_three(self):
         n1 = self.list.add_to_front(1, 1)
         n2 = self.list.add_to_front(2, 2)
-        n3 = self.list.add_to_front(3, 3)
+        self.list.add_to_front(3, 3)
 
         self.list.move_to_front(n1)
         self.assertEqual(self.list_to_array(), [(1, 1), (3, 3), (2, 2)])
         self.assertEqual(
             self.list_to_array(backward=True), [(2, 2), (3, 3), (1, 1)])
         self.assertEqual(self.list.size, 3)
 
@@ -136,15 +136,15 @@
         self.assertEqual(self.list_to_array(), [(2, 2), (1, 1), (3, 3)])
         self.assertEqual(
             self.list_to_array(backward=True), [(3, 3), (1, 1), (2, 2)])
         self.assertEqual(self.list.size, 3)
 
     def test_list_move_two(self):
         n1 = self.list.add_to_front(1, 1)
-        n2 = self.list.add_to_front(2, 2)
+        self.list.add_to_front(2, 2)
         self.assertEqual(self.list_to_array(), [(2, 2), (1, 1)])
 
         self.list.move_to_front(n1)
         self.assertEqual(self.list_to_array(), [(1, 1), (2, 2)])
 
     def test_list_move_one(self):
         n1 = self.list.add_to_front(1, 1)
@@ -166,27 +166,27 @@
         removed = self.list.remove_back()
         self.assertEqual(n1, removed)
         self.assertEqual(self.list.size, 0)
         self.assertEqual(self.list_to_array(), [])
 
     def test_list_remove_back_two(self):
         n1 = self.list.add_to_front(1, 1)
-        n2 = self.list.add_to_front(2, 2)
+        self.list.add_to_front(2, 2)
         self.assertEqual(self.list.size, 2)
         self.assertEqual(self.list_to_array(), [(2, 2), (1, 1)])
         removed = self.list.remove_back()
         self.assertEqual(removed, n1)
         self.assertEqual(self.list_to_array(), [(2, 2)])
         self.assertEqual(self.list_to_array(backward=True), [(2, 2)])
         self.assertEqual(self.list.size, 1)
 
     def test_list_remove_back_three(self):
         n1 = self.list.add_to_front(1, 1)
-        n2 = self.list.add_to_front(2, 2)
-        n3 = self.list.add_to_front(3, 3)
+        self.list.add_to_front(2, 2)
+        self.list.add_to_front(3, 3)
         self.assertEqual(self.list.size, 3)
         self.assertEqual(self.list_to_array(), [(3, 3), (2, 2), (1, 1)])
         removed = self.list.remove_back()
         self.assertEqual(removed, n1)
         self.assertEqual(self.list_to_array(), [(3, 3), (2, 2)])
         self.assertEqual(self.list_to_array(backward=True), [(2, 2), (3, 3)])
         self.assertEqual(self.list.size, 2)
```

### Comparing `deepview-profile-0.12.2/deepview_profile/tracking/backward_interceptor.py` & `deepview_profile-0.12.3/deepview_profile/tracking/backward_interceptor.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.2/deepview_profile/tracking/base.py` & `deepview_profile-0.12.3/deepview_profile/tracking/base.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.2/deepview_profile/tracking/breakdown.py` & `deepview_profile-0.12.3/deepview_profile/tracking/breakdown.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.2/deepview_profile/tracking/call_stack.py` & `deepview_profile-0.12.3/deepview_profile/tracking/call_stack.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.2/deepview_profile/tracking/callable_tracker.py` & `deepview_profile-0.12.3/deepview_profile/tracking/callable_tracker.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.2/deepview_profile/tracking/hook_manager.py` & `deepview_profile-0.12.3/deepview_profile/tracking/hook_manager.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.2/deepview_profile/tracking/memory/activations.py` & `deepview_profile-0.12.3/deepview_profile/tracking/memory/activations.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,15 +175,15 @@
 
 def _extract_gradient_functions_in_topological_order(model_output):
     """
     Given a model output (Tensor or nested list/tuple of Tensors), build a
     topological ordering of their gradient functions.
     """
     if isinstance(model_output, tuple) or isinstance(model_output, list):
-        tensors = _flatten_and_filter_tensors(tensor_iterable)
+        tensors = _flatten_and_filter_tensors(model_output)
     elif (isinstance(model_output, torch.Tensor) and
           model_output.grad_fn is not None):
         tensors = [model_output]
     else:
         return []
 
     result = []
```

### Comparing `deepview-profile-0.12.2/deepview_profile/tracking/memory/report.py` & `deepview_profile-0.12.3/deepview_profile/tracking/memory/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import collections
 import enum
-import os
 
 from deepview_profile.tracking.base import ReportBase, ReportBuilderBase
 import deepview_profile.tracking.memory.report_queries as queries
 
 
 WeightEntry = collections.namedtuple(
     'WeightEntry',
```

### Comparing `deepview-profile-0.12.2/deepview_profile/tracking/memory/report_queries.py` & `deepview_profile-0.12.3/deepview_profile/tracking/memory/report_queries.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.2/deepview_profile/tracking/memory/weights.py` & `deepview_profile-0.12.3/deepview_profile/tracking/memory/weights.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import torch
 import inspect
-import weakref
 
 from deepview_profile.tracking.base import TrackerBase
 from deepview_profile.tracking.call_stack import CallStack
 from deepview_profile.tracking.hook_manager import HookManager
 from deepview_profile.tracking.utils import tensor_size_bytes
-
+from deepview_profile.util_weak import WeakTensorKeyDictionary
 
 class WeightsTracker(TrackerBase):
     def __init__(self, project_root):
         super().__init__()
         self._hook_manager = HookManager()
-        self._module_parameters = weakref.WeakKeyDictionary()
+        self._module_parameters = WeakTensorKeyDictionary()
         self._project_root = project_root
 
     def start_tracking(self):
         super().start_tracking()
         self._hook_manager.attach_hook(
             torch.nn.Module,
             'register_parameter',
@@ -44,14 +43,14 @@
         self.populate_report(builder)
 
     def _register_parameter_hook_creator(self, func):
         def hook(*args, **kwargs):
             name = args[1]
             parameter = args[2]
             retval = func(*args, **kwargs)
-            if parameter is not None:
+            if parameter is not None and parameter not in self._module_parameters:
                 self._module_parameters[parameter] = (
                     name,
                     CallStack.from_here(self._project_root, start_from=2),
                 )
             return retval
         return hook
```

### Comparing `deepview-profile-0.12.2/deepview_profile/tracking/time/operation.py` & `deepview_profile-0.12.3/deepview_profile/tracking/time/operation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import collections
 
-import torch
 
 from deepview_profile.tracking.call_stack import CallStack
 from deepview_profile.tracking.base import TrackerBase
 from deepview_profile.tracking.callable_tracker import CallableTracker
 from deepview_profile.tracking.utils import remove_dunder
 from deepview_profile.profiler.operation import OperationProfiler
```

### Comparing `deepview-profile-0.12.2/deepview_profile/tracking/time/report.py` & `deepview_profile-0.12.3/deepview_profile/tracking/time/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import collections
-import os
 
 from deepview_profile.tracking.base import ReportBase, ReportBuilderBase
 import deepview_profile.tracking.time.report_queries as queries
 
 RunTimeEntry = collections.namedtuple(
     'RunTimeEntry',
     ['operation_name',
```

### Comparing `deepview-profile-0.12.2/deepview_profile/tracking/time/report_queries.py` & `deepview_profile-0.12.3/deepview_profile/tracking/time/report_queries.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.2/deepview_profile/tracking/tracker.py` & `deepview_profile-0.12.3/deepview_profile/tracking/tracker.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.2/deepview_profile/user_code_utils.py` & `deepview_profile-0.12.3/deepview_profile/user_code_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import contextlib
-import os
 import sys
 
 from deepview_profile.exceptions import exceptions_as_analysis_errors
 
 
 @contextlib.contextmanager
 def user_code_environment(script_root_path, project_root):
```

### Comparing `deepview-profile-0.12.2/deepview_profile/version_utils.py` & `deepview_profile-0.12.3/deepview_profile/version_utils.py`

 * *Files identical despite different names*

### Comparing `deepview-profile-0.12.2/pyproject.toml` & `deepview_profile-0.12.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deepview-profile"
-version = "0.12.2"
+version = "0.12.3"
 description = "Interactive performance profiling and debugging tool for PyTorch neural networks."
 authors = ["CentML <support@centml.ai>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/CentML/DeepView.Profile"
 keywords = ["pytorch", "neural networks", "debugger", "profiler"]
 classifiers = [
@@ -32,10 +32,17 @@
 nvidia-ml-py3 = "*"
 toml = "^0.10.2"
 pyRAPL = "^0.2.3"
 deepview-predict = "*"
 
 [tool.poetry.dev-dependencies]
 
+[tool.poetry.group.dev.dependencies]
+ruff = "^0.0.267"
+pre-commit = "2.21.0"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.ruff]
+extend-exclude = ["examples", "deepview_profile/protocol_gen/"]
```

### Comparing `deepview-profile-0.12.2/PKG-INFO` & `deepview_profile-0.12.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: deepview-profile
-Version: 0.12.2
+Version: 0.12.3
 Summary: Interactive performance profiling and debugging tool for PyTorch neural networks.
 Home-page: https://github.com/CentML/DeepView.Profile
 License: Apache-2.0
 Keywords: pytorch,neural networks,debugger,profiler
 Author: CentML
 Author-email: support@centml.ai
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Debuggers
 Requires-Dist: deepview-predict
 Requires-Dist: numpy (>=1.15.2,<2.0.0)
 Requires-Dist: nvidia-ml-py3
 Requires-Dist: protobuf (==3.18.3)
 Requires-Dist: pyRAPL (>=0.2.3,<0.3.0)
 Requires-Dist: pyyaml
@@ -35,15 +36,14 @@
 [![](https://img.shields.io/pypi/v/deepview-profile.svg)](https://pypi.org/project/deepview-profile/)
 
 DeepView.Profile is a tool to profile and debug the training performance of [PyTorch](https://pytorch.org) neural networks.
 
 - [Installation](#installation)
 - [Usage example](#getting-started)
 - [Development Environment Setup](#dev-setup)
-- [Release Process](#release-process)
 - [Release History](#release-history)
 - [Meta](#meta)
 - [Contributing](#contributing)
 
 <h2 id="installation">Installation</h2>
 
 DeepView.Profile works with *GPU-based* neural networks that are implemented in [PyTorch](https://pytorch.org).
@@ -106,26 +106,14 @@
 
 <h2 id="dev-setup">Development Environment Setup</h2>
 
 From the project root, do
 ```zsh
 poetry install
 ```
-<h2 id="release-process">Release Process</h2>
-
-1. Make sure you're on main branch and it is clean
-1. Run [tools/prepare-release.sh](tools/prepare-release.sh) which will:
-    * Increment the version
-    * Create a release branch
-    * Create a release PR
-1. After the PR is merged [build-and-publish-new-version.yml](.github/workflows/build-and-publish-new-version.yml) GitHub action will:
-    * build the Python Wheels
-    * GitHub release
-    * Publish to Test PyPI
-    * Subject to approval publish to PyPI
 
 <h2 id="release-history">Release History</h2>
 
 See [Releases](https://github.com/CentML/DeepView.Profile/releases)
 
 <h2 id="meta">Meta</h2>
```

