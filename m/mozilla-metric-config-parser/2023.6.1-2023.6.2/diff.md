# Comparing `tmp/mozilla-metric-config-parser-2023.6.1.tar.gz` & `tmp/mozilla-metric-config-parser-2023.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozilla-metric-config-parser-2023.6.1.tar", last modified: Mon Jun  5 20:19:37 2023, max compression
+gzip compressed data, was "mozilla-metric-config-parser-2023.6.2.tar", last modified: Tue Jun  6 17:16:51 2023, max compression
```

## Comparing `mozilla-metric-config-parser-2023.6.1.tar` & `mozilla-metric-config-parser-2023.6.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:19:37.804196 mozilla-metric-config-parser-2023.6.1/
--rw-r--r--   0 root         (0) root         (0)    16725 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      632 2023-06-05 20:19:37.804196 mozilla-metric-config-parser-2023.6.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      279 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:19:37.800196 mozilla-metric-config-parser-2023.6.1/metric_config_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7062 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/alert.py
--rw-r--r--   0 root         (0) root         (0)     7048 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/analysis.py
--rw-r--r--   0 root         (0) root         (0)     2774 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/cli.py
--rw-r--r--   0 root         (0) root         (0)    26273 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/config.py
--rw-r--r--   0 root         (0) root         (0)     8172 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/data_source.py
--rw-r--r--   0 root         (0) root         (0)     1602 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/definition.py
--rw-r--r--   0 root         (0) root         (0)     3493 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/dimension.py
--rw-r--r--   0 root         (0) root         (0)      804 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/errors.py
--rw-r--r--   0 root         (0) root         (0)     9608 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/experiment.py
--rw-r--r--   0 root         (0) root         (0)     2619 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/exposure_signal.py
--rw-r--r--   0 root         (0) root         (0)     1143 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/function.py
--rw-r--r--   0 root         (0) root         (0)    12463 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/metric.py
--rw-r--r--   0 root         (0) root         (0)     3130 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/metric_group.py
--rw-r--r--   0 root         (0) root         (0)     6640 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/monitoring.py
--rw-r--r--   0 root         (0) root         (0)     1718 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/outcome.py
--rw-r--r--   0 root         (0) root         (0)     3386 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/parameter.py
--rw-r--r--   0 root         (0) root         (0)     3278 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/population.py
--rw-r--r--   0 root         (0) root         (0)      317 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/pre_treatment.py
--rw-r--r--   0 root         (0) root         (0)     5138 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/project.py
--rw-r--r--   0 root         (0) root         (0)     8103 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/segment.py
--rw-r--r--   0 root         (0) root         (0)     4207 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/sql.py
--rw-r--r--   0 root         (0) root         (0)      129 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/statistic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:19:37.804196 mozilla-metric-config-parser-2023.6.1/metric_config_parser/templates/
--rw-r--r--   0 root         (0) root         (0)      145 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/templates/data_source_query.sql
--rw-r--r--   0 root         (0) root         (0)     2691 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/templates/metrics_query.sql
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:19:37.804196 mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5118 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:19:37.804196 mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/integration/
--rw-r--r--   0 root         (0) root         (0)     4708 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/integration/test_config_integration.py
--rw-r--r--   0 root         (0) root         (0)     2428 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_alert.py
--rw-r--r--   0 root         (0) root         (0)    19957 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_analysis.py
--rw-r--r--   0 root         (0) root         (0)    12702 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_config.py
--rw-r--r--   0 root         (0) root         (0)     9856 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_experiment.py
--rw-r--r--   0 root         (0) root         (0)     1581 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_function.py
--rw-r--r--   0 root         (0) root         (0)     2608 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_metric.py
--rw-r--r--   0 root         (0) root         (0)     8522 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_monitoring.py
--rw-r--r--   0 root         (0) root         (0)    11358 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_outcomes.py
--rw-r--r--   0 root         (0) root         (0)      458 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_parameter.py
--rw-r--r--   0 root         (0) root         (0)     2035 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_population.py
--rw-r--r--   0 root         (0) root         (0)     2808 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_project.py
--rw-r--r--   0 root         (0) root         (0)     3322 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_sql.py
--rw-r--r--   0 root         (0) root         (0)      575 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/metric_config_parser/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:19:37.804196 mozilla-metric-config-parser-2023.6.1/mozilla_metric_config_parser.egg-info/
--rw-r--r--   0 root         (0) root         (0)      632 2023-06-05 20:19:37.000000 mozilla-metric-config-parser-2023.6.1/mozilla_metric_config_parser.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1941 2023-06-05 20:19:37.000000 mozilla-metric-config-parser-2023.6.1/mozilla_metric_config_parser.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 20:19:37.000000 mozilla-metric-config-parser-2023.6.1/mozilla_metric_config_parser.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       70 2023-06-05 20:19:37.000000 mozilla-metric-config-parser-2023.6.1/mozilla_metric_config_parser.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      251 2023-06-05 20:19:37.000000 mozilla-metric-config-parser-2023.6.1/mozilla_metric_config_parser.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-05 20:19:37.000000 mozilla-metric-config-parser-2023.6.1/mozilla_metric_config_parser.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       67 2023-06-05 20:19:37.808196 mozilla-metric-config-parser-2023.6.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1540 2023-06-05 20:19:28.000000 mozilla-metric-config-parser-2023.6.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:16:51.755847 mozilla-metric-config-parser-2023.6.2/
+-rw-r--r--   0 root         (0) root         (0)    16725 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      632 2023-06-06 17:16:51.755847 mozilla-metric-config-parser-2023.6.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      279 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:16:51.751847 mozilla-metric-config-parser-2023.6.2/metric_config_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/metric_config_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7062 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/metric_config_parser/alert.py
+-rw-r--r--   0 root         (0) root         (0)     7048 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/metric_config_parser/analysis.py
+-rw-r--r--   0 root         (0) root         (0)     2774 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/metric_config_parser/cli.py
+-rw-r--r--   0 root         (0) root         (0)    27863 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/metric_config_parser/config.py
+-rw-r--r--   0 root         (0) root         (0)     8172 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/metric_config_parser/data_source.py
+-rw-r--r--   0 root         (0) root         (0)     1602 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/metric_config_parser/definition.py
+-rw-r--r--   0 root         (0) root         (0)     3493 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/metric_config_parser/dimension.py
+-rw-r--r--   0 root         (0) root         (0)      804 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/metric_config_parser/errors.py
+-rw-r--r--   0 root         (0) root         (0)     9608 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/metric_config_parser/experiment.py
+-rw-r--r--   0 root         (0) root         (0)     2619 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/metric_config_parser/exposure_signal.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/metric_config_parser/function.py
+-rw-r--r--   0 root         (0) root         (0)    12463 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/metric_config_parser/metric.py
+-rw-r--r--   0 root         (0) root         (0)     3130 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/metric_config_parser/metric_group.py
+-rw-r--r--   0 root         (0) root         (0)     6640 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/metric_config_parser/monitoring.py
+-rw-r--r--   0 root         (0) root         (0)     1718 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/metric_config_parser/outcome.py
+-rw-r--r--   0 root         (0) root         (0)     3386 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/metric_config_parser/parameter.py
+-rw-r--r--   0 root         (0) root         (0)     3278 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/metric_config_parser/population.py
+-rw-r--r--   0 root         (0) root         (0)      317 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/metric_config_parser/pre_treatment.py
+-rw-r--r--   0 root         (0) root         (0)     5138 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/metric_config_parser/project.py
+-rw-r--r--   0 root         (0) root         (0)     8103 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/metric_config_parser/segment.py
+-rw-r--r--   0 root         (0) root         (0)     4207 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/metric_config_parser/sql.py
+-rw-r--r--   0 root         (0) root         (0)      129 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/metric_config_parser/statistic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:16:51.751847 mozilla-metric-config-parser-2023.6.2/metric_config_parser/templates/
+-rw-r--r--   0 root         (0) root         (0)      145 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/metric_config_parser/templates/data_source_query.sql
+-rw-r--r--   0 root         (0) root         (0)     2691 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/metric_config_parser/templates/metrics_query.sql
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:16:51.751847 mozilla-metric-config-parser-2023.6.2/metric_config_parser/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/metric_config_parser/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5118 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/metric_config_parser/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:16:51.755847 mozilla-metric-config-parser-2023.6.2/metric_config_parser/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)     4708 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/metric_config_parser/tests/integration/test_config_integration.py
+-rw-r--r--   0 root         (0) root         (0)     2428 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/metric_config_parser/tests/test_alert.py
+-rw-r--r--   0 root         (0) root         (0)    19957 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/metric_config_parser/tests/test_analysis.py
+-rw-r--r--   0 root         (0) root         (0)    14533 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/metric_config_parser/tests/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     9856 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/metric_config_parser/tests/test_experiment.py
+-rw-r--r--   0 root         (0) root         (0)     1581 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/metric_config_parser/tests/test_function.py
+-rw-r--r--   0 root         (0) root         (0)     2608 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/metric_config_parser/tests/test_metric.py
+-rw-r--r--   0 root         (0) root         (0)     8522 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/metric_config_parser/tests/test_monitoring.py
+-rw-r--r--   0 root         (0) root         (0)    11358 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/metric_config_parser/tests/test_outcomes.py
+-rw-r--r--   0 root         (0) root         (0)      458 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/metric_config_parser/tests/test_parameter.py
+-rw-r--r--   0 root         (0) root         (0)     2035 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/metric_config_parser/tests/test_population.py
+-rw-r--r--   0 root         (0) root         (0)     2808 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/metric_config_parser/tests/test_project.py
+-rw-r--r--   0 root         (0) root         (0)     3322 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/metric_config_parser/tests/test_sql.py
+-rw-r--r--   0 root         (0) root         (0)      575 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/metric_config_parser/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:16:51.755847 mozilla-metric-config-parser-2023.6.2/mozilla_metric_config_parser.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      632 2023-06-06 17:16:51.000000 mozilla-metric-config-parser-2023.6.2/mozilla_metric_config_parser.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1941 2023-06-06 17:16:51.000000 mozilla-metric-config-parser-2023.6.2/mozilla_metric_config_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 17:16:51.000000 mozilla-metric-config-parser-2023.6.2/mozilla_metric_config_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2023-06-06 17:16:51.000000 mozilla-metric-config-parser-2023.6.2/mozilla_metric_config_parser.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      251 2023-06-06 17:16:51.000000 mozilla-metric-config-parser-2023.6.2/mozilla_metric_config_parser.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-06 17:16:51.000000 mozilla-metric-config-parser-2023.6.2/mozilla_metric_config_parser.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       67 2023-06-06 17:16:51.755847 mozilla-metric-config-parser-2023.6.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1540 2023-06-06 17:16:43.000000 mozilla-metric-config-parser-2023.6.2/setup.py
```

### Comparing `mozilla-metric-config-parser-2023.6.1/LICENSE` & `mozilla-metric-config-parser-2023.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.1/PKG-INFO` & `mozilla-metric-config-parser-2023.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozilla-metric-config-parser
-Version: 2023.6.1
+Version: 2023.6.2
 Summary: Parses metric configuration files
 Home-page: https://github.com/mozilla/metric-config-parser
 Author: Mozilla Corporation
 Author-email: fx-data-dev@mozilla.org
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: testing
```

### Comparing `mozilla-metric-config-parser-2023.6.1/metric_config_parser/alert.py` & `mozilla-metric-config-parser-2023.6.2/metric_config_parser/alert.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.1/metric_config_parser/analysis.py` & `mozilla-metric-config-parser-2023.6.2/metric_config_parser/analysis.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.1/metric_config_parser/cli.py` & `mozilla-metric-config-parser-2023.6.2/metric_config_parser/cli.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.1/metric_config_parser/config.py` & `mozilla-metric-config-parser-2023.6.2/metric_config_parser/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import List, Optional, Union
 
 import attr
 import jinja2
 import toml
 from git import Repo
 from git.exc import InvalidGitRepositoryError
+from git.objects.commit import Commit
 from jinja2 import StrictUndefined
 from pytz import UTC
 
 from metric_config_parser.data_source import DataSourceDefinition
 from metric_config_parser.definition import DefinitionSpec, DefinitionSpecSub
 from metric_config_parser.function import FunctionsSpec
 from metric_config_parser.monitoring import MonitoringSpec
@@ -492,33 +493,69 @@
 
                 # find the commit that got added just before the `timestamp`
                 rev = "HEAD"  # use the HEAD commit by default if no other commits exist
 
                 # make sure the most recent commit is checked out by checking out the main branch
                 tmp_repo.git.checkout(repo.main_branch)
 
+                # keep track of more recent commits to go back to in case invalid configs
+                # got checked into main that cannot be parsed
+                newer_commits: List[Commit] = []
+
                 # start iterating through all commits starting at HEAD
                 for commit in tmp_repo.iter_commits("HEAD"):
                     # check if the commit timestamp is older than the reference timestamp
                     if commit.committed_datetime <= timestamp:
                         rev = commit.hexsha
                         break
 
+                    newer_commits.insert(0, commit)
+
                 if commit:
                     # if there is no commit that is older than the reference timestamp,
                     # use the oldest commit that we could find (= last commit)
                     rev = commit.hexsha
 
                 # checkout that commit
                 tmp_repo.git.checkout(rev)
 
                 # load configs as they were at the time of the commit
-                configs = self.from_local_repo(
-                    tmp_repo, repo.path, self.is_private, repo.main_branch, is_tmp_repo=True
-                )
+                try:
+                    configs = self.from_local_repo(
+                        tmp_repo, repo.path, self.is_private, repo.main_branch, is_tmp_repo=True
+                    )
+                except Exception as e:
+                    could_load_configs = False
+
+                    # iterate through newer commits to find one that can be parsed
+                    for newer_commit in newer_commits:
+                        tmp_repo.git.checkout(newer_commit.hexsha)
+
+                        try:
+                            configs = self.from_local_repo(
+                                tmp_repo,
+                                repo.path,
+                                self.is_private,
+                                repo.main_branch,
+                                is_tmp_repo=True,
+                            )
+                            could_load_configs = True
+                            print(
+                                f"Error parsing config files as of {timestamp}: {e}. "
+                                + f"Using newer version instead of commit {newer_commit.hexsha}"
+                            )
+                            break
+                        except Exception:
+                            # continue searching
+                            pass
+
+                    if not could_load_configs:
+                        # there is no newer commit, current state is broken
+                        raise e
+
                 configs.repos = [repo]  # point to the original repo, instead of the temporary one
 
                 if config_collection is None:
                     config_collection = configs
                 else:
                     config_collection.merge(configs)
```

### Comparing `mozilla-metric-config-parser-2023.6.1/metric_config_parser/data_source.py` & `mozilla-metric-config-parser-2023.6.2/metric_config_parser/data_source.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.1/metric_config_parser/definition.py` & `mozilla-metric-config-parser-2023.6.2/metric_config_parser/definition.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.1/metric_config_parser/dimension.py` & `mozilla-metric-config-parser-2023.6.2/metric_config_parser/dimension.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.1/metric_config_parser/errors.py` & `mozilla-metric-config-parser-2023.6.2/metric_config_parser/errors.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.1/metric_config_parser/experiment.py` & `mozilla-metric-config-parser-2023.6.2/metric_config_parser/experiment.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.1/metric_config_parser/exposure_signal.py` & `mozilla-metric-config-parser-2023.6.2/metric_config_parser/exposure_signal.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.1/metric_config_parser/function.py` & `mozilla-metric-config-parser-2023.6.2/metric_config_parser/function.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.1/metric_config_parser/metric.py` & `mozilla-metric-config-parser-2023.6.2/metric_config_parser/metric.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.1/metric_config_parser/metric_group.py` & `mozilla-metric-config-parser-2023.6.2/metric_config_parser/metric_group.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.1/metric_config_parser/monitoring.py` & `mozilla-metric-config-parser-2023.6.2/metric_config_parser/monitoring.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.1/metric_config_parser/outcome.py` & `mozilla-metric-config-parser-2023.6.2/metric_config_parser/outcome.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.1/metric_config_parser/parameter.py` & `mozilla-metric-config-parser-2023.6.2/metric_config_parser/parameter.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.1/metric_config_parser/population.py` & `mozilla-metric-config-parser-2023.6.2/metric_config_parser/population.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.1/metric_config_parser/project.py` & `mozilla-metric-config-parser-2023.6.2/metric_config_parser/project.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.1/metric_config_parser/segment.py` & `mozilla-metric-config-parser-2023.6.2/metric_config_parser/segment.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.1/metric_config_parser/sql.py` & `mozilla-metric-config-parser-2023.6.2/metric_config_parser/sql.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.1/metric_config_parser/templates/metrics_query.sql` & `mozilla-metric-config-parser-2023.6.2/metric_config_parser/templates/metrics_query.sql`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/conftest.py` & `mozilla-metric-config-parser-2023.6.2/metric_config_parser/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/integration/test_config_integration.py` & `mozilla-metric-config-parser-2023.6.2/metric_config_parser/tests/integration/test_config_integration.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_alert.py` & `mozilla-metric-config-parser-2023.6.2/metric_config_parser/tests/test_alert.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_analysis.py` & `mozilla-metric-config-parser-2023.6.2/metric_config_parser/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_config.py` & `mozilla-metric-config-parser-2023.6.2/metric_config_parser/tests/test_config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import datetime
+import shutil
 from pathlib import Path
 from textwrap import dedent
 
 import pytest
 import pytz
 import toml
+from git import Repo
 
 from metric_config_parser.analysis import AnalysisSpec
 from metric_config_parser.config import (
     Config,
     ConfigCollection,
     DefaultConfig,
     DefinitionConfig,
     Outcome,
 )
 from metric_config_parser.errors import DefinitionNotFound
 from metric_config_parser.outcome import OutcomeSpec
 
+TEST_DIR = Path(__file__).parent
+
 
 class TestConfigIntegration:
     config_str = dedent(
         """
         [metrics]
         weekly = ["active_hours"]
 
@@ -376,7 +380,54 @@
         assert config_collection is not None
 
     def test_config_from_subdir_too_deep(self, local_tmp_repo):
         nested_path = Path(local_tmp_repo) / "metrics" / "jetstream"
 
         with pytest.raises(Exception):
             ConfigCollection.from_github_repo(nested_path, depth=1)
+
+    def test_as_of_broken_commit(self, tmp_path):
+        r = Repo.init(tmp_path)
+        r.config_writer().set_value("user", "name", "test").release()
+        r.config_writer().set_value("user", "email", "test@example.com").release()
+
+        # check in broken file
+        broken_config = dedent(
+            """
+            friendly_name = "Performance outcomes"
+            description = "Outcomes related to performance"
+
+            [metrics]
+            weekly = ["speed"]
+            overall = ["speed"]
+
+            [metrics.speed]
+            data_source = "main"
+            select_expression = "1"
+
+            [metrics.speed.statistics.bootstrap_mean]
+            """
+        )
+        outcome_path = tmp_path / "jetstream" / "outcomes" / "firefox_desktop"
+        outcome_path.mkdir(parents=True, exist_ok=True)
+        (outcome_path / "performance.toml").write_text(broken_config)
+        r.git.add(".")
+        r.git.commit("-m", "commit", "--date", "Mon 20 Aug 2020 20:19:19 UTC")
+
+        with pytest.raises(Exception):
+            ConfigCollection.from_github_repo(tmp_path / "jetstream")
+
+        with pytest.raises(Exception):
+            ConfigCollection.from_github_repo(tmp_path / "jetstream").as_of(
+                pytz.UTC.localize(datetime.datetime(2023, 5, 21))
+            )
+
+        # check in valid files
+        shutil.copytree(TEST_DIR / "data", tmp_path, dirs_exist_ok=True)
+        r.git.add(".")
+        r.git.commit("-m", "commit", "--date", "Mon 25 Aug 2020 20:00:19 UTC")
+
+        configs = ConfigCollection.from_github_repo(tmp_path / "jetstream")
+        assert configs.outcomes is not None
+
+        configs = configs.as_of(pytz.UTC.localize(datetime.datetime(2023, 5, 21)))
+        assert configs.outcomes is not None
```

### Comparing `mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_experiment.py` & `mozilla-metric-config-parser-2023.6.2/metric_config_parser/tests/test_experiment.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_function.py` & `mozilla-metric-config-parser-2023.6.2/metric_config_parser/tests/test_function.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_metric.py` & `mozilla-metric-config-parser-2023.6.2/metric_config_parser/tests/test_metric.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_monitoring.py` & `mozilla-metric-config-parser-2023.6.2/metric_config_parser/tests/test_monitoring.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_outcomes.py` & `mozilla-metric-config-parser-2023.6.2/metric_config_parser/tests/test_outcomes.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_population.py` & `mozilla-metric-config-parser-2023.6.2/metric_config_parser/tests/test_population.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_project.py` & `mozilla-metric-config-parser-2023.6.2/metric_config_parser/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.1/metric_config_parser/tests/test_sql.py` & `mozilla-metric-config-parser-2023.6.2/metric_config_parser/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.1/metric_config_parser/util.py` & `mozilla-metric-config-parser-2023.6.2/metric_config_parser/util.py`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.1/mozilla_metric_config_parser.egg-info/PKG-INFO` & `mozilla-metric-config-parser-2023.6.2/mozilla_metric_config_parser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozilla-metric-config-parser
-Version: 2023.6.1
+Version: 2023.6.2
 Summary: Parses metric configuration files
 Home-page: https://github.com/mozilla/metric-config-parser
 Author: Mozilla Corporation
 Author-email: fx-data-dev@mozilla.org
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: testing
```

### Comparing `mozilla-metric-config-parser-2023.6.1/mozilla_metric_config_parser.egg-info/SOURCES.txt` & `mozilla-metric-config-parser-2023.6.2/mozilla_metric_config_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mozilla-metric-config-parser-2023.6.1/setup.py` & `mozilla-metric-config-parser-2023.6.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,9 +60,9 @@
     long_description=text_from_file("README.md"),
     long_description_content_type="text/markdown",
     python_requires=">=3.6",
     entry_points="""
         [console_scripts]
         metric-config-parser=metric_config_parser.cli:cli
     """,
-    version="2023.6.1",
+    version="2023.6.2",
 )
```

