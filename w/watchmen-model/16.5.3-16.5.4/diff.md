# Comparing `tmp/watchmen_model-16.5.3.tar.gz` & `tmp/watchmen_model-16.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchmen_model-16.5.3.tar", max compression
+gzip compressed data, was "watchmen_model-16.5.4.tar", max compression
```

## Comparing `watchmen_model-16.5.3.tar` & `watchmen_model-16.5.4.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0     1061 2023-06-05 01:29:03.524124 watchmen_model-16.5.3/LICENSE
--rw-r--r--   0        0        0      463 2023-06-05 01:29:03.524124 watchmen_model-16.5.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-05 01:29:03.524124 watchmen_model-16.5.3/src/watchmen_model/__init__.py
--rw-r--r--   0        0        0     1412 2023-06-05 01:29:03.524124 watchmen_model-16.5.3/src/watchmen_model/admin/__init__.py
--rw-r--r--   0        0        0      194 2023-06-05 01:29:03.524124 watchmen_model-16.5.3/src/watchmen_model/admin/conditional.py
--rw-r--r--   0        0        0     1165 2023-06-05 01:29:03.524124 watchmen_model-16.5.3/src/watchmen_model/admin/enumeration.py
--rw-r--r--   0        0        0     3283 2023-06-05 01:29:03.524124 watchmen_model-16.5.3/src/watchmen_model/admin/factor.py
--rw-r--r--   0        0        0     4897 2023-06-05 01:29:03.524124 watchmen_model-16.5.3/src/watchmen_model/admin/pipeline.py
--rw-r--r--   0        0        0     1518 2023-06-05 01:29:03.524124 watchmen_model-16.5.3/src/watchmen_model/admin/pipeline_action.py
--rw-r--r--   0        0        0      590 2023-06-05 01:29:03.524124 watchmen_model-16.5.3/src/watchmen_model/admin/pipeline_action_delete.py
--rw-r--r--   0        0        0      984 2023-06-05 01:29:03.524124 watchmen_model-16.5.3/src/watchmen_model/admin/pipeline_action_read.py
--rw-r--r--   0        0        0     1217 2023-06-05 01:29:03.524124 watchmen_model-16.5.3/src/watchmen_model/admin/pipeline_action_system.py
--rw-r--r--   0        0        0     3419 2023-06-05 01:29:03.524124 watchmen_model-16.5.3/src/watchmen_model/admin/pipeline_action_write.py
--rw-r--r--   0        0        0     2420 2023-06-05 01:29:03.524124 watchmen_model-16.5.3/src/watchmen_model/admin/pipeline_graphic.py
--rw-r--r--   0        0        0     1518 2023-06-05 01:29:03.524124 watchmen_model-16.5.3/src/watchmen_model/admin/space.py
--rw-r--r--   0        0        0     1591 2023-06-05 01:29:03.524124 watchmen_model-16.5.3/src/watchmen_model/admin/topic.py
--rw-r--r--   0        0        0     1681 2023-06-05 01:29:03.524124 watchmen_model-16.5.3/src/watchmen_model/admin/topic_snapshot.py
--rw-r--r--   0        0        0      549 2023-06-05 01:29:03.524124 watchmen_model-16.5.3/src/watchmen_model/admin/user.py
--rw-r--r--   0        0        0      409 2023-06-05 01:29:03.524124 watchmen_model-16.5.3/src/watchmen_model/admin/user_group.py
--rw-r--r--   0        0        0      134 2023-06-05 01:29:03.524124 watchmen_model-16.5.3/src/watchmen_model/analysis/__init__.py
--rw-r--r--   0        0        0      642 2023-06-05 01:29:03.524124 watchmen_model-16.5.3/src/watchmen_model/analysis/factor_index.py
--rw-r--r--   0        0        0      995 2023-06-05 01:29:03.524124 watchmen_model-16.5.3/src/watchmen_model/analysis/pipeline_index.py
--rw-r--r--   0        0        0     2201 2023-06-05 01:29:03.524124 watchmen_model-16.5.3/src/watchmen_model/chart/__init__.py
--rw-r--r--   0        0        0    14167 2023-06-05 01:29:03.524124 watchmen_model-16.5.3/src/watchmen_model/chart/chart.py
--rw-r--r--   0        0        0      395 2023-06-05 01:29:03.524124 watchmen_model-16.5.3/src/watchmen_model/chart/chart_basic_structure.py
--rw-r--r--   0        0        0      500 2023-06-05 01:29:03.524124 watchmen_model-16.5.3/src/watchmen_model/chart/chart_basic_style.py
--rw-r--r--   0        0        0      478 2023-06-05 01:29:03.524124 watchmen_model-16.5.3/src/watchmen_model/chart/chart_enums.py
--rw-r--r--   0        0        0      848 2023-06-05 01:29:03.524124 watchmen_model-16.5.3/src/watchmen_model/chart/chart_settings.py
--rw-r--r--   0        0        0      356 2023-06-05 01:29:03.524124 watchmen_model-16.5.3/src/watchmen_model/chart/chart_types.py
--rw-r--r--   0        0        0     1541 2023-06-05 01:29:03.524124 watchmen_model-16.5.3/src/watchmen_model/common/__init__.py
--rw-r--r--   0        0        0      337 2023-06-05 01:29:03.524124 watchmen_model-16.5.3/src/watchmen_model/common/data_result_set.py
--rw-r--r--   0        0        0      273 2023-06-05 01:29:03.524124 watchmen_model-16.5.3/src/watchmen_model/common/graphic.py
--rw-r--r--   0        0        0     1382 2023-06-05 01:29:03.524124 watchmen_model-16.5.3/src/watchmen_model/common/model.py
--rw-r--r--   0        0        0      476 2023-06-05 01:29:03.524124 watchmen_model-16.5.3/src/watchmen_model/common/pagination.py
--rw-r--r--   0        0        0     4851 2023-06-05 01:29:03.524124 watchmen_model-16.5.3/src/watchmen_model/common/parameter_and_condition.py
--rw-r--r--   0        0        0      431 2023-06-05 01:29:03.524124 watchmen_model-16.5.3/src/watchmen_model/common/storable.py
--rw-r--r--   0        0        0      763 2023-06-05 01:29:03.524124 watchmen_model-16.5.3/src/watchmen_model/common/tuple.py
--rw-r--r--   0        0        0     2390 2023-06-05 01:29:03.524124 watchmen_model-16.5.3/src/watchmen_model/common/tuple_ids.py
--rw-r--r--   0        0        0      580 2023-06-05 01:29:03.524124 watchmen_model-16.5.3/src/watchmen_model/console/__init__.py
--rw-r--r--   0        0        0      308 2023-06-05 01:29:03.524124 watchmen_model-16.5.3/src/watchmen_model/console/connected_space.py
--rw-r--r--   0        0        0     2060 2023-06-05 01:29:03.524124 watchmen_model-16.5.3/src/watchmen_model/console/connected_space_graphic.py
--rw-r--r--   0        0        0     2211 2023-06-05 01:29:03.524124 watchmen_model-16.5.3/src/watchmen_model/console/dashboard.py
--rw-r--r--   0        0        0      173 2023-06-05 01:29:03.524124 watchmen_model-16.5.3/src/watchmen_model/console/data_result_set.py
--rw-r--r--   0        0        0     5354 2023-06-05 01:29:03.528123 watchmen_model-16.5.3/src/watchmen_model/console/report.py
--rw-r--r--   0        0        0     5911 2023-06-05 01:29:03.528123 watchmen_model-16.5.3/src/watchmen_model/console/subject.py
--rw-r--r--   0        0        0      290 2023-06-05 01:29:03.528123 watchmen_model-16.5.3/src/watchmen_model/console/utils.py
--rw-r--r--   0        0        0      525 2023-06-05 01:29:03.528123 watchmen_model-16.5.3/src/watchmen_model/dqc/__init__.py
--rw-r--r--   0        0        0      620 2023-06-05 01:29:03.528123 watchmen_model-16.5.3/src/watchmen_model/dqc/catalog.py
--rw-r--r--   0        0        0     5590 2023-06-05 01:29:03.528123 watchmen_model-16.5.3/src/watchmen_model/dqc/dqc_pipelines.py
--rw-r--r--   0        0        0     2786 2023-06-05 01:29:03.528123 watchmen_model-16.5.3/src/watchmen_model/dqc/dqc_topics.py
--rw-r--r--   0        0        0      586 2023-06-05 01:29:03.528123 watchmen_model-16.5.3/src/watchmen_model/dqc/monitor_data.py
--rw-r--r--   0        0        0      681 2023-06-05 01:29:03.528123 watchmen_model-16.5.3/src/watchmen_model/dqc/monitor_job_lock.py
--rw-r--r--   0        0        0     3485 2023-06-05 01:29:03.528123 watchmen_model-16.5.3/src/watchmen_model/dqc/monitor_rule.py
--rw-r--r--   0        0        0       43 2023-06-05 01:29:03.528123 watchmen_model-16.5.3/src/watchmen_model/dqc/topic_profile.py
--rw-r--r--   0        0        0       71 2023-06-05 01:29:03.528123 watchmen_model-16.5.3/src/watchmen_model/gui/__init__.py
--rw-r--r--   0        0        0      362 2023-06-05 01:29:03.528123 watchmen_model-16.5.3/src/watchmen_model/gui/favorite.py
--rw-r--r--   0        0        0      289 2023-06-05 01:29:03.528123 watchmen_model-16.5.3/src/watchmen_model/gui/last_snapshot.py
--rw-r--r--   0        0        0     1462 2023-06-05 01:29:03.528123 watchmen_model-16.5.3/src/watchmen_model/indicator/__init__.py
--rw-r--r--   0        0        0      605 2023-06-05 01:29:03.528123 watchmen_model-16.5.3/src/watchmen_model/indicator/achievement_plugin_task.py
--rw-r--r--   0        0        0     4170 2023-06-05 01:29:03.528123 watchmen_model-16.5.3/src/watchmen_model/indicator/bucket.py
--rw-r--r--   0        0        0     3319 2023-06-05 01:29:03.528123 watchmen_model-16.5.3/src/watchmen_model/indicator/derived_objective.py
--rw-r--r--   0        0        0     3156 2023-06-05 01:29:03.528123 watchmen_model-16.5.3/src/watchmen_model/indicator/indicator.py
--rw-r--r--   0        0        0      972 2023-06-05 01:29:03.528123 watchmen_model-16.5.3/src/watchmen_model/indicator/measure_method.py
--rw-r--r--   0        0        0    13782 2023-06-05 01:29:03.528123 watchmen_model-16.5.3/src/watchmen_model/indicator/objective.py
--rw-r--r--   0        0        0        0 2023-06-05 01:29:03.528123 watchmen_model-16.5.3/src/watchmen_model/lineage/__init__.py
--rw-r--r--   0        0        0      378 2023-06-05 01:29:03.528123 watchmen_model-16.5.3/src/watchmen_model/lineage/lineage_graph.py
--rw-r--r--   0        0        0      629 2023-06-05 01:29:03.528123 watchmen_model-16.5.3/src/watchmen_model/pipeline_kernel/__init__.py
--rw-r--r--   0        0        0     6634 2023-06-05 01:29:03.528123 watchmen_model-16.5.3/src/watchmen_model/pipeline_kernel/pipeline_monitor_log.py
--rw-r--r--   0        0        0      237 2023-06-05 01:29:03.528123 watchmen_model-16.5.3/src/watchmen_model/pipeline_kernel/pipeline_monitor_pipelines.py
--rw-r--r--   0        0        0     4790 2023-06-05 01:29:03.528123 watchmen_model-16.5.3/src/watchmen_model/pipeline_kernel/pipeline_monitor_topics.py
--rw-r--r--   0        0        0     1154 2023-06-05 01:29:03.528123 watchmen_model-16.5.3/src/watchmen_model/pipeline_kernel/pipeline_trigger_data.py
--rw-r--r--   0        0        0      187 2023-06-05 01:29:03.528123 watchmen_model-16.5.3/src/watchmen_model/system/PackageVersion.py
--rw-r--r--   0        0        0      383 2023-06-05 01:29:03.528123 watchmen_model-16.5.3/src/watchmen_model/system/__init__.py
--rw-r--r--   0        0        0     1392 2023-06-05 01:29:03.528123 watchmen_model-16.5.3/src/watchmen_model/system/data_source.py
--rw-r--r--   0        0        0      534 2023-06-05 01:29:03.528123 watchmen_model-16.5.3/src/watchmen_model/system/external_writer.py
--rw-r--r--   0        0        0      325 2023-06-05 01:29:03.528123 watchmen_model-16.5.3/src/watchmen_model/system/key_store.py
--rw-r--r--   0        0        0      338 2023-06-05 01:29:03.528123 watchmen_model-16.5.3/src/watchmen_model/system/operation.py
--rw-r--r--   0        0        0      588 2023-06-05 01:29:03.528123 watchmen_model-16.5.3/src/watchmen_model/system/plugin.py
--rw-r--r--   0        0        0     1755 2023-06-05 01:29:03.528123 watchmen_model-16.5.3/src/watchmen_model/system/sql_query_performance.py
--rw-r--r--   0        0        0      193 2023-06-05 01:29:03.528123 watchmen_model-16.5.3/src/watchmen_model/system/tenant.py
--rw-r--r--   0        0        0      443 2023-06-05 01:29:03.528123 watchmen_model-16.5.3/src/watchmen_model/system/token.py
--rw-r--r--   0        0        0        0 2023-06-05 01:29:03.528123 watchmen_model-16.5.3/src/watchmen_model/webhook/__init__.py
--rw-r--r--   0        0        0      576 2023-06-05 01:29:03.528123 watchmen_model-16.5.3/src/watchmen_model/webhook/event_defination.py
--rw-r--r--   0        0        0     1265 2023-06-05 01:29:03.528123 watchmen_model-16.5.3/src/watchmen_model/webhook/notification_defination.py
--rw-r--r--   0        0        0      983 2023-06-05 01:29:03.528123 watchmen_model-16.5.3/src/watchmen_model/webhook/subscription_event.py
--rw-r--r--   0        0        0      536 2023-06-05 01:29:03.528123 watchmen_model-16.5.3/src/watchmen_model/webhook/subscription_event_lock.py
--rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 watchmen_model-16.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/LICENSE
+-rw-r--r--   0        0        0      463 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/__init__.py
+-rw-r--r--   0        0        0     1412 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/admin/__init__.py
+-rw-r--r--   0        0        0      194 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/admin/conditional.py
+-rw-r--r--   0        0        0     1165 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/admin/enumeration.py
+-rw-r--r--   0        0        0     3283 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/admin/factor.py
+-rw-r--r--   0        0        0     4897 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/admin/pipeline.py
+-rw-r--r--   0        0        0     1518 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/admin/pipeline_action.py
+-rw-r--r--   0        0        0      590 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/admin/pipeline_action_delete.py
+-rw-r--r--   0        0        0      984 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/admin/pipeline_action_read.py
+-rw-r--r--   0        0        0     1217 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/admin/pipeline_action_system.py
+-rw-r--r--   0        0        0     3419 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/admin/pipeline_action_write.py
+-rw-r--r--   0        0        0     2420 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/admin/pipeline_graphic.py
+-rw-r--r--   0        0        0     1518 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/admin/space.py
+-rw-r--r--   0        0        0     1591 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/admin/topic.py
+-rw-r--r--   0        0        0     1681 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/admin/topic_snapshot.py
+-rw-r--r--   0        0        0      549 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/admin/user.py
+-rw-r--r--   0        0        0      409 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/admin/user_group.py
+-rw-r--r--   0        0        0      134 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/analysis/__init__.py
+-rw-r--r--   0        0        0      642 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/analysis/factor_index.py
+-rw-r--r--   0        0        0      995 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/analysis/pipeline_index.py
+-rw-r--r--   0        0        0     2201 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/chart/__init__.py
+-rw-r--r--   0        0        0    14167 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/chart/chart.py
+-rw-r--r--   0        0        0      395 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/chart/chart_basic_structure.py
+-rw-r--r--   0        0        0      500 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/chart/chart_basic_style.py
+-rw-r--r--   0        0        0      478 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/chart/chart_enums.py
+-rw-r--r--   0        0        0      848 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/chart/chart_settings.py
+-rw-r--r--   0        0        0      356 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/chart/chart_types.py
+-rw-r--r--   0        0        0     1541 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/common/__init__.py
+-rw-r--r--   0        0        0      337 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/common/data_result_set.py
+-rw-r--r--   0        0        0      273 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/common/graphic.py
+-rw-r--r--   0        0        0     1382 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/common/model.py
+-rw-r--r--   0        0        0      476 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/common/pagination.py
+-rw-r--r--   0        0        0     4851 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/common/parameter_and_condition.py
+-rw-r--r--   0        0        0      431 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/common/storable.py
+-rw-r--r--   0        0        0      763 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/common/tuple.py
+-rw-r--r--   0        0        0     2390 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/common/tuple_ids.py
+-rw-r--r--   0        0        0      580 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/console/__init__.py
+-rw-r--r--   0        0        0      308 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/console/connected_space.py
+-rw-r--r--   0        0        0     2060 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/console/connected_space_graphic.py
+-rw-r--r--   0        0        0     2211 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/console/dashboard.py
+-rw-r--r--   0        0        0      173 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/console/data_result_set.py
+-rw-r--r--   0        0        0     5354 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/console/report.py
+-rw-r--r--   0        0        0     5932 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/console/subject.py
+-rw-r--r--   0        0        0      290 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/console/utils.py
+-rw-r--r--   0        0        0      525 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/dqc/__init__.py
+-rw-r--r--   0        0        0      620 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/dqc/catalog.py
+-rw-r--r--   0        0        0     5590 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/dqc/dqc_pipelines.py
+-rw-r--r--   0        0        0     2786 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/dqc/dqc_topics.py
+-rw-r--r--   0        0        0      586 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/dqc/monitor_data.py
+-rw-r--r--   0        0        0      681 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/dqc/monitor_job_lock.py
+-rw-r--r--   0        0        0     3485 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/dqc/monitor_rule.py
+-rw-r--r--   0        0        0       43 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/dqc/topic_profile.py
+-rw-r--r--   0        0        0       71 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/gui/__init__.py
+-rw-r--r--   0        0        0      362 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/gui/favorite.py
+-rw-r--r--   0        0        0      289 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/gui/last_snapshot.py
+-rw-r--r--   0        0        0     1462 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/indicator/__init__.py
+-rw-r--r--   0        0        0      605 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/indicator/achievement_plugin_task.py
+-rw-r--r--   0        0        0     4170 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/indicator/bucket.py
+-rw-r--r--   0        0        0     3319 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/indicator/derived_objective.py
+-rw-r--r--   0        0        0     3156 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/indicator/indicator.py
+-rw-r--r--   0        0        0      972 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/indicator/measure_method.py
+-rw-r--r--   0        0        0    13782 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/indicator/objective.py
+-rw-r--r--   0        0        0        0 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/lineage/__init__.py
+-rw-r--r--   0        0        0      378 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/lineage/lineage_graph.py
+-rw-r--r--   0        0        0      629 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/pipeline_kernel/__init__.py
+-rw-r--r--   0        0        0     6634 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/pipeline_kernel/pipeline_monitor_log.py
+-rw-r--r--   0        0        0      237 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/pipeline_kernel/pipeline_monitor_pipelines.py
+-rw-r--r--   0        0        0     4790 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/pipeline_kernel/pipeline_monitor_topics.py
+-rw-r--r--   0        0        0     1154 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/pipeline_kernel/pipeline_trigger_data.py
+-rw-r--r--   0        0        0      187 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/system/PackageVersion.py
+-rw-r--r--   0        0        0      383 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/system/__init__.py
+-rw-r--r--   0        0        0     1392 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/system/data_source.py
+-rw-r--r--   0        0        0      534 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/system/external_writer.py
+-rw-r--r--   0        0        0      325 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/system/key_store.py
+-rw-r--r--   0        0        0      338 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/system/operation.py
+-rw-r--r--   0        0        0      588 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/system/plugin.py
+-rw-r--r--   0        0        0     1755 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/system/sql_query_performance.py
+-rw-r--r--   0        0        0      193 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/system/tenant.py
+-rw-r--r--   0        0        0      443 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/system/token.py
+-rw-r--r--   0        0        0        0 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/webhook/__init__.py
+-rw-r--r--   0        0        0      576 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/webhook/event_defination.py
+-rw-r--r--   0        0        0     1265 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/webhook/notification_defination.py
+-rw-r--r--   0        0        0      983 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/webhook/subscription_event.py
+-rw-r--r--   0        0        0      536 2023-06-06 01:45:59.137402 watchmen_model-16.5.4/src/watchmen_model/webhook/subscription_event_lock.py
+-rw-r--r--   0        0        0      565 1970-01-01 00:00:00.000000 watchmen_model-16.5.4/PKG-INFO
```

### Comparing `watchmen_model-16.5.3/LICENSE` & `watchmen_model-16.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/admin/__init__.py` & `watchmen_model-16.5.4/src/watchmen_model/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/admin/enumeration.py` & `watchmen_model-16.5.4/src/watchmen_model/admin/enumeration.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/admin/factor.py` & `watchmen_model-16.5.4/src/watchmen_model/admin/factor.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/admin/pipeline.py` & `watchmen_model-16.5.4/src/watchmen_model/admin/pipeline.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/admin/pipeline_action.py` & `watchmen_model-16.5.4/src/watchmen_model/admin/pipeline_action.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/admin/pipeline_action_delete.py` & `watchmen_model-16.5.4/src/watchmen_model/admin/pipeline_action_delete.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/admin/pipeline_action_read.py` & `watchmen_model-16.5.4/src/watchmen_model/admin/pipeline_action_read.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/admin/pipeline_action_system.py` & `watchmen_model-16.5.4/src/watchmen_model/admin/pipeline_action_system.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/admin/pipeline_action_write.py` & `watchmen_model-16.5.4/src/watchmen_model/admin/pipeline_action_write.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/admin/pipeline_graphic.py` & `watchmen_model-16.5.4/src/watchmen_model/admin/pipeline_graphic.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/admin/space.py` & `watchmen_model-16.5.4/src/watchmen_model/admin/space.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/admin/topic.py` & `watchmen_model-16.5.4/src/watchmen_model/admin/topic.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/admin/topic_snapshot.py` & `watchmen_model-16.5.4/src/watchmen_model/admin/topic_snapshot.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/admin/user.py` & `watchmen_model-16.5.4/src/watchmen_model/admin/user.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/analysis/factor_index.py` & `watchmen_model-16.5.4/src/watchmen_model/analysis/factor_index.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/analysis/pipeline_index.py` & `watchmen_model-16.5.4/src/watchmen_model/analysis/pipeline_index.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/chart/__init__.py` & `watchmen_model-16.5.4/src/watchmen_model/chart/__init__.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/chart/chart.py` & `watchmen_model-16.5.4/src/watchmen_model/chart/chart.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/chart/chart_settings.py` & `watchmen_model-16.5.4/src/watchmen_model/chart/chart_settings.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/common/__init__.py` & `watchmen_model-16.5.4/src/watchmen_model/common/__init__.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/common/model.py` & `watchmen_model-16.5.4/src/watchmen_model/common/model.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/common/parameter_and_condition.py` & `watchmen_model-16.5.4/src/watchmen_model/common/parameter_and_condition.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/common/tuple.py` & `watchmen_model-16.5.4/src/watchmen_model/common/tuple.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/common/tuple_ids.py` & `watchmen_model-16.5.4/src/watchmen_model/common/tuple_ids.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/console/__init__.py` & `watchmen_model-16.5.4/src/watchmen_model/console/__init__.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/console/connected_space_graphic.py` & `watchmen_model-16.5.4/src/watchmen_model/console/connected_space_graphic.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/console/dashboard.py` & `watchmen_model-16.5.4/src/watchmen_model/console/dashboard.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/console/report.py` & `watchmen_model-16.5.4/src/watchmen_model/console/report.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/console/subject.py` & `watchmen_model-16.5.4/src/watchmen_model/console/subject.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,14 +168,15 @@
 	AVERAGE = 'avg'
 	MAXIMUM = 'max'
 	MINIMUM = 'min'
 
 
 class SubjectDatasetCriteriaIndicator(BaseModel):
 	name: str = None
+	columnId:str = None
 	arithmetic: SubjectDatasetCriteriaIndicatorArithmetic = None
 	alias: str = None
 
 
 def construct_criteria_indicator(
 		indicator: Optional[Union[dict, SubjectDatasetCriteriaIndicator]]) -> Optional[SubjectDatasetCriteriaIndicator]:
 	if indicator is None:
```

### Comparing `watchmen_model-16.5.3/src/watchmen_model/dqc/__init__.py` & `watchmen_model-16.5.4/src/watchmen_model/dqc/__init__.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/dqc/catalog.py` & `watchmen_model-16.5.4/src/watchmen_model/dqc/catalog.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/dqc/dqc_pipelines.py` & `watchmen_model-16.5.4/src/watchmen_model/dqc/dqc_pipelines.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/dqc/dqc_topics.py` & `watchmen_model-16.5.4/src/watchmen_model/dqc/dqc_topics.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/dqc/monitor_data.py` & `watchmen_model-16.5.4/src/watchmen_model/dqc/monitor_data.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/dqc/monitor_job_lock.py` & `watchmen_model-16.5.4/src/watchmen_model/dqc/monitor_job_lock.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/dqc/monitor_rule.py` & `watchmen_model-16.5.4/src/watchmen_model/dqc/monitor_rule.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/indicator/__init__.py` & `watchmen_model-16.5.4/src/watchmen_model/indicator/__init__.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/indicator/achievement_plugin_task.py` & `watchmen_model-16.5.4/src/watchmen_model/indicator/achievement_plugin_task.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/indicator/bucket.py` & `watchmen_model-16.5.4/src/watchmen_model/indicator/bucket.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/indicator/derived_objective.py` & `watchmen_model-16.5.4/src/watchmen_model/indicator/derived_objective.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/indicator/indicator.py` & `watchmen_model-16.5.4/src/watchmen_model/indicator/indicator.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/indicator/measure_method.py` & `watchmen_model-16.5.4/src/watchmen_model/indicator/measure_method.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/indicator/objective.py` & `watchmen_model-16.5.4/src/watchmen_model/indicator/objective.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/pipeline_kernel/__init__.py` & `watchmen_model-16.5.4/src/watchmen_model/pipeline_kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/pipeline_kernel/pipeline_monitor_log.py` & `watchmen_model-16.5.4/src/watchmen_model/pipeline_kernel/pipeline_monitor_log.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/pipeline_kernel/pipeline_monitor_topics.py` & `watchmen_model-16.5.4/src/watchmen_model/pipeline_kernel/pipeline_monitor_topics.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/pipeline_kernel/pipeline_trigger_data.py` & `watchmen_model-16.5.4/src/watchmen_model/pipeline_kernel/pipeline_trigger_data.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/system/data_source.py` & `watchmen_model-16.5.4/src/watchmen_model/system/data_source.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/system/external_writer.py` & `watchmen_model-16.5.4/src/watchmen_model/system/external_writer.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/system/plugin.py` & `watchmen_model-16.5.4/src/watchmen_model/system/plugin.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/system/sql_query_performance.py` & `watchmen_model-16.5.4/src/watchmen_model/system/sql_query_performance.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/webhook/event_defination.py` & `watchmen_model-16.5.4/src/watchmen_model/webhook/event_defination.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/webhook/notification_defination.py` & `watchmen_model-16.5.4/src/watchmen_model/webhook/notification_defination.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/webhook/subscription_event.py` & `watchmen_model-16.5.4/src/watchmen_model/webhook/subscription_event.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/src/watchmen_model/webhook/subscription_event_lock.py` & `watchmen_model-16.5.4/src/watchmen_model/webhook/subscription_event_lock.py`

 * *Files identical despite different names*

### Comparing `watchmen_model-16.5.3/PKG-INFO` & `watchmen_model-16.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: watchmen-model
-Version: 16.5.3
+Version: 16.5.4
 Summary: 
 License: MIT
 Author: botlikes
 Author-email: 75356972+botlikes456@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic (>=1.9.0,<2.0.0)
 Requires-Dist: sqlparse (>=0.4.4,<0.5.0)
-Requires-Dist: watchmen-utilities (==16.5.3)
+Requires-Dist: watchmen-utilities (==16.5.4)
```

