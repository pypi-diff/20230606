# Comparing `tmp/dlt-0.2.9.tar.gz` & `tmp/dlt-0.2.9a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlt-0.2.9.tar", max compression
+gzip compressed data, was "dlt-0.2.9a0.tar", max compression
```

## Comparing `dlt-0.2.9.tar` & `dlt-0.2.9a0.tar`

### file list

```diff
@@ -1,214 +1,208 @@
--rw-r--r--   0        0        0    11343 2022-06-03 15:05:59.024600 dlt-0.2.9/LICENSE.txt
--rw-r--r--   0        0        0     4214 2023-04-30 21:17:44.388805 dlt-0.2.9/README.md
--rw-r--r--   0        0        0     1711 2023-04-30 21:17:44.388805 dlt-0.2.9/dlt/__init__.py
--rw-r--r--   0        0        0        0 2023-04-30 21:17:44.388805 dlt-0.2.9/dlt/cli/__init__.py
--rw-r--r--   0        0        0    16519 2023-05-29 18:11:09.008705 dlt-0.2.9/dlt/cli/_dlt.py
--rw-r--r--   0        0        0     3886 2023-05-29 14:13:02.418979 dlt-0.2.9/dlt/cli/config_toml_writer.py
--rw-r--r--   0        0        0    14636 2023-05-29 18:11:09.008705 dlt-0.2.9/dlt/cli/deploy_command.py
--rw-r--r--   0        0        0    14722 2023-05-29 18:11:09.008705 dlt-0.2.9/dlt/cli/deploy_command_helpers.py
--rw-r--r--   0        0        0     1853 2023-04-30 21:17:44.388805 dlt-0.2.9/dlt/cli/echo.py
--rw-r--r--   0        0        0      435 2023-03-23 14:48:32.551618 dlt-0.2.9/dlt/cli/exceptions.py
--rw-r--r--   0        0        0    18722 2023-05-29 18:11:09.008705 dlt-0.2.9/dlt/cli/init_command.py
--rw-r--r--   0        0        0    10503 2023-05-28 13:56:42.331452 dlt-0.2.9/dlt/cli/pipeline_command.py
--rw-r--r--   0        0        0     9422 2023-05-14 20:33:31.539348 dlt-0.2.9/dlt/cli/pipeline_files.py
--rw-r--r--   0        0        0     4505 2023-05-24 16:38:22.528779 dlt-0.2.9/dlt/cli/source_detection.py
--rw-r--r--   0        0        0     1899 2023-05-23 16:25:33.987923 dlt-0.2.9/dlt/cli/telemetry_command.py
--rw-r--r--   0        0        0     3753 2023-05-29 18:11:09.008705 dlt-0.2.9/dlt/cli/utils.py
--rw-r--r--   0        0        0      307 2023-03-23 14:48:32.551618 dlt-0.2.9/dlt/common/__init__.py
--rw-r--r--   0        0        0     1265 2022-08-24 09:42:09.472789 dlt-0.2.9/dlt/common/arithmetics.py
--rw-r--r--   0        0        0      442 2023-05-29 14:13:02.418979 dlt-0.2.9/dlt/common/configuration/__init__.py
--rw-r--r--   0        0        0     5078 2023-05-24 16:38:22.528779 dlt-0.2.9/dlt/common/configuration/accessors.py
--rw-r--r--   0        0        0     3469 2023-05-07 23:03:04.659469 dlt-0.2.9/dlt/common/configuration/container.py
--rw-r--r--   0        0        0     6741 2023-05-29 14:13:02.418979 dlt-0.2.9/dlt/common/configuration/exceptions.py
--rw-r--r--   0        0        0     7912 2023-04-22 20:26:30.632198 dlt-0.2.9/dlt/common/configuration/inject.py
--rw-r--r--   0        0        0     1791 2023-05-14 20:33:31.539348 dlt-0.2.9/dlt/common/configuration/paths.py
--rw-r--r--   0        0        0      306 2023-05-07 23:03:04.659469 dlt-0.2.9/dlt/common/configuration/providers/__init__.py
--rw-r--r--   0        0        0      664 2023-05-29 14:13:02.418979 dlt-0.2.9/dlt/common/configuration/providers/airflow.py
--rw-r--r--   0        0        0     1116 2023-05-07 23:03:04.659469 dlt-0.2.9/dlt/common/configuration/providers/context.py
--rw-r--r--   0        0        0     1335 2023-05-07 23:03:04.659469 dlt-0.2.9/dlt/common/configuration/providers/dictionary.py
--rw-r--r--   0        0        0     1981 2023-05-07 23:03:04.659469 dlt-0.2.9/dlt/common/configuration/providers/environ.py
--rw-r--r--   0        0        0     3662 2023-05-29 14:13:02.418979 dlt-0.2.9/dlt/common/configuration/providers/google_secrets.py
--rw-r--r--   0        0        0     1306 2023-05-24 16:38:22.538779 dlt-0.2.9/dlt/common/configuration/providers/provider.py
--rw-r--r--   0        0        0    12390 2023-05-29 14:13:02.418979 dlt-0.2.9/dlt/common/configuration/providers/toml.py
--rw-r--r--   0        0        0    17872 2023-05-29 14:13:02.418979 dlt-0.2.9/dlt/common/configuration/resolve.py
--rw-r--r--   0        0        0      971 2023-05-29 14:13:02.418979 dlt-0.2.9/dlt/common/configuration/specs/__init__.py
--rw-r--r--   0        0        0     1817 2023-05-07 23:03:04.659469 dlt-0.2.9/dlt/common/configuration/specs/api_credentials.py
--rw-r--r--   0        0        0     2109 2023-05-29 14:13:02.418979 dlt-0.2.9/dlt/common/configuration/specs/aws_credentials.py
--rw-r--r--   0        0        0    14214 2023-05-29 14:13:02.418979 dlt-0.2.9/dlt/common/configuration/specs/base_configuration.py
--rw-r--r--   0        0        0     5483 2023-05-29 14:13:02.418979 dlt-0.2.9/dlt/common/configuration/specs/config_providers_context.py
--rw-r--r--   0        0        0     2792 2023-03-23 14:48:32.551618 dlt-0.2.9/dlt/common/configuration/specs/config_section_context.py
--rw-r--r--   0        0        0     1818 2023-05-24 16:38:22.538779 dlt-0.2.9/dlt/common/configuration/specs/connection_string_credentials.py
--rw-r--r--   0        0        0     2125 2023-04-24 18:26:21.111453 dlt-0.2.9/dlt/common/configuration/specs/exceptions.py
--rw-r--r--   0        0        0    12725 2023-05-07 23:03:04.669469 dlt-0.2.9/dlt/common/configuration/specs/gcp_credentials.py
--rw-r--r--   0        0        0      725 2023-05-07 23:03:04.669469 dlt-0.2.9/dlt/common/configuration/specs/known_sections.py
--rw-r--r--   0        0        0     2455 2023-04-30 21:17:44.388805 dlt-0.2.9/dlt/common/configuration/specs/run_configuration.py
--rw-r--r--   0        0        0     6036 2023-05-29 14:13:02.418979 dlt-0.2.9/dlt/common/configuration/utils.py
--rw-r--r--   0        0        0      142 2023-03-23 14:48:32.551618 dlt-0.2.9/dlt/common/data_types/__init__.py
--rw-r--r--   0        0        0     6306 2023-03-23 14:48:32.551618 dlt-0.2.9/dlt/common/data_types/type_helpers.py
--rw-r--r--   0        0        0      214 2023-03-23 14:48:32.551618 dlt-0.2.9/dlt/common/data_types/typing.py
--rw-r--r--   0        0        0      260 2023-03-23 14:48:20.701618 dlt-0.2.9/dlt/common/data_writers/__init__.py
--rw-r--r--   0        0        0     5893 2023-03-23 14:48:32.551618 dlt-0.2.9/dlt/common/data_writers/buffered.py
--rw-r--r--   0        0        0     2400 2023-05-29 14:13:02.418979 dlt-0.2.9/dlt/common/data_writers/escape.py
--rw-r--r--   0        0        0      962 2023-03-23 14:48:32.551618 dlt-0.2.9/dlt/common/data_writers/exceptions.py
--rw-r--r--   0        0        0     5159 2023-03-23 14:48:32.551618 dlt-0.2.9/dlt/common/data_writers/writers.py
--rw-r--r--   0        0        0      189 2023-05-29 18:11:09.008705 dlt-0.2.9/dlt/common/destination/__init__.py
--rw-r--r--   0        0        0     2206 2023-04-05 08:03:40.638919 dlt-0.2.9/dlt/common/destination/capabilities.py
--rw-r--r--   0        0        0    11099 2023-05-29 18:11:09.008705 dlt-0.2.9/dlt/common/destination/reference.py
--rw-r--r--   0        0        0     6451 2023-05-25 21:23:38.949428 dlt-0.2.9/dlt/common/exceptions.py
--rw-r--r--   0        0        0     4954 2023-03-23 14:48:32.551618 dlt-0.2.9/dlt/common/git.py
--rw-r--r--   0        0        0     5253 2023-05-14 20:33:31.539348 dlt-0.2.9/dlt/common/json/__init__.py
--rw-r--r--   0        0        0     1802 2023-04-10 08:12:53.769595 dlt-0.2.9/dlt/common/json/_orjson.py
--rw-r--r--   0        0        0     2939 2023-04-10 08:12:53.769595 dlt-0.2.9/dlt/common/json/_simplejson.py
--rw-r--r--   0        0        0     1536 2023-04-29 12:58:55.943219 dlt-0.2.9/dlt/common/jsonpath.py
--rw-r--r--   0        0        0      232 2023-03-23 14:48:32.551618 dlt-0.2.9/dlt/common/normalizers/__init__.py
--rw-r--r--   0        0        0     1197 2023-05-07 23:03:04.669469 dlt-0.2.9/dlt/common/normalizers/configuration.py
--rw-r--r--   0        0        0      472 2023-03-23 14:48:32.551618 dlt-0.2.9/dlt/common/normalizers/exceptions.py
--rw-r--r--   0        0        0     1644 2023-04-06 15:27:24.759561 dlt-0.2.9/dlt/common/normalizers/json/__init__.py
--rw-r--r--   0        0        0    13382 2023-05-14 20:33:31.539348 dlt-0.2.9/dlt/common/normalizers/json/relational.py
--rw-r--r--   0        0        0       64 2023-03-23 14:48:32.551618 dlt-0.2.9/dlt/common/normalizers/naming/__init__.py
--rw-r--r--   0        0        0      807 2023-03-23 14:48:32.551618 dlt-0.2.9/dlt/common/normalizers/naming/direct.py
--rw-r--r--   0        0        0     1069 2023-03-23 14:48:32.551618 dlt-0.2.9/dlt/common/normalizers/naming/duck_case.py
--rw-r--r--   0        0        0      792 2023-03-23 14:48:32.551618 dlt-0.2.9/dlt/common/normalizers/naming/exceptions.py
--rw-r--r--   0        0        0     3753 2023-04-05 08:03:40.638919 dlt-0.2.9/dlt/common/normalizers/naming/naming.py
--rw-r--r--   0        0        0     3002 2023-03-23 14:48:32.551618 dlt-0.2.9/dlt/common/normalizers/naming/snake_case.py
--rw-r--r--   0        0        0      358 2023-04-02 09:09:15.855769 dlt-0.2.9/dlt/common/normalizers/typing.py
--rw-r--r--   0        0        0     2337 2023-04-06 15:27:24.759561 dlt-0.2.9/dlt/common/normalizers/utils.py
--rw-r--r--   0        0        0      451 2023-03-23 14:48:32.551618 dlt-0.2.9/dlt/common/pendulum.py
--rw-r--r--   0        0        0    19221 2023-05-29 18:11:09.008705 dlt-0.2.9/dlt/common/pipeline.py
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.551618 dlt-0.2.9/dlt/common/reflection/__init__.py
--rw-r--r--   0        0        0      374 2023-03-23 14:48:32.551618 dlt-0.2.9/dlt/common/reflection/function_visitor.py
--rw-r--r--   0        0        0     4891 2023-04-09 16:39:04.593180 dlt-0.2.9/dlt/common/reflection/spec.py
--rw-r--r--   0        0        0     5069 2023-04-24 18:26:21.111453 dlt-0.2.9/dlt/common/reflection/utils.py
--rw-r--r--   0        0        0      174 2023-04-30 21:17:44.388805 dlt-0.2.9/dlt/common/runners/__init__.py
--rw-r--r--   0        0        0      705 2023-05-24 16:38:22.538779 dlt-0.2.9/dlt/common/runners/configuration.py
--rw-r--r--   0        0        0     2635 2023-05-14 11:08:47.420838 dlt-0.2.9/dlt/common/runners/pool_runner.py
--rw-r--r--   0        0        0     4046 2023-03-23 14:48:32.561618 dlt-0.2.9/dlt/common/runners/runnable.py
--rw-r--r--   0        0        0     3145 2023-03-23 14:48:32.561618 dlt-0.2.9/dlt/common/runners/stdout.py
--rw-r--r--   0        0        0     2137 2023-03-23 14:48:32.561618 dlt-0.2.9/dlt/common/runners/synth_pickle.py
--rw-r--r--   0        0        0      105 2023-04-30 21:17:44.388805 dlt-0.2.9/dlt/common/runners/typing.py
--rw-r--r--   0        0        0     5590 2023-05-07 23:03:04.669469 dlt-0.2.9/dlt/common/runners/venv.py
--rw-r--r--   0        0        0       36 2023-04-30 21:17:44.398805 dlt-0.2.9/dlt/common/runtime/__init__.py
--rw-r--r--   0        0        0    13441 2023-04-30 21:17:44.398805 dlt-0.2.9/dlt/common/runtime/collector.py
--rw-r--r--   0        0        0     4501 2023-05-14 20:33:31.539348 dlt-0.2.9/dlt/common/runtime/exec_info.py
--rw-r--r--   0        0        0      647 2023-04-30 21:17:44.398805 dlt-0.2.9/dlt/common/runtime/init.py
--rw-r--r--   0        0        0     4002 2023-04-30 21:17:44.398805 dlt-0.2.9/dlt/common/runtime/logger.py
--rw-r--r--   0        0        0     2052 2023-04-30 21:17:44.398805 dlt-0.2.9/dlt/common/runtime/prometheus.py
--rw-r--r--   0        0        0     7170 2023-05-14 20:33:31.539348 dlt-0.2.9/dlt/common/runtime/segment.py
--rw-r--r--   0        0        0     2493 2023-04-30 21:17:44.398805 dlt-0.2.9/dlt/common/runtime/sentry.py
--rw-r--r--   0        0        0     2027 2023-04-30 21:17:44.398805 dlt-0.2.9/dlt/common/runtime/signals.py
--rw-r--r--   0        0        0      616 2023-04-03 18:50:36.893525 dlt-0.2.9/dlt/common/runtime/slack.py
--rw-r--r--   0        0        0      720 2023-04-30 21:17:44.398805 dlt-0.2.9/dlt/common/runtime/telemetry.py
--rw-r--r--   0        0        0      387 2023-04-03 18:50:36.893525 dlt-0.2.9/dlt/common/schema/__init__.py
--rw-r--r--   0        0        0     1927 2023-03-23 14:48:32.561618 dlt-0.2.9/dlt/common/schema/detections.py
--rw-r--r--   0        0        0     2974 2023-03-23 14:48:32.561618 dlt-0.2.9/dlt/common/schema/exceptions.py
--rw-r--r--   0        0        0    25164 2023-05-29 14:13:02.418979 dlt-0.2.9/dlt/common/schema/schema.py
--rw-r--r--   0        0        0     3004 2023-04-22 20:26:30.632198 dlt-0.2.9/dlt/common/schema/typing.py
--rw-r--r--   0        0        0    23087 2023-04-30 21:17:44.398805 dlt-0.2.9/dlt/common/schema/utils.py
--rw-r--r--   0        0        0     1467 2023-05-24 16:38:22.538779 dlt-0.2.9/dlt/common/source.py
--rw-r--r--   0        0        0      554 2023-05-24 16:38:22.538779 dlt-0.2.9/dlt/common/storages/__init__.py
--rw-r--r--   0        0        0     1649 2023-05-24 16:38:22.538779 dlt-0.2.9/dlt/common/storages/configuration.py
--rw-r--r--   0        0        0     1906 2023-03-23 14:48:32.561618 dlt-0.2.9/dlt/common/storages/data_item_storage.py
--rw-r--r--   0        0        0     2804 2023-04-03 18:50:36.893525 dlt-0.2.9/dlt/common/storages/exceptions.py
--rw-r--r--   0        0        0    10891 2023-05-14 20:33:31.539348 dlt-0.2.9/dlt/common/storages/file_storage.py
--rw-r--r--   0        0        0     2690 2023-05-24 16:38:22.538779 dlt-0.2.9/dlt/common/storages/live_schema_storage.py
--rw-r--r--   0        0        0    21812 2023-05-24 16:38:22.538779 dlt-0.2.9/dlt/common/storages/load_storage.py
--rw-r--r--   0        0        0     2409 2023-05-24 16:38:22.538779 dlt-0.2.9/dlt/common/storages/normalize_storage.py
--rw-r--r--   0        0        0     8434 2023-05-24 16:38:22.538779 dlt-0.2.9/dlt/common/storages/schema_storage.py
--rw-r--r--   0        0        0     2525 2023-04-24 18:26:21.111453 dlt-0.2.9/dlt/common/storages/versioned_storage.py
--rw-r--r--   0        0        0     2634 2023-05-07 23:03:04.669469 dlt-0.2.9/dlt/common/time.py
--rw-r--r--   0        0        0     4736 2023-04-03 18:50:36.893525 dlt-0.2.9/dlt/common/typing.py
--rw-r--r--   0        0        0    14239 2023-05-24 16:38:22.538779 dlt-0.2.9/dlt/common/utils.py
--rw-r--r--   0        0        0     3686 2023-03-23 14:48:32.561618 dlt-0.2.9/dlt/common/validation.py
--rw-r--r--   0        0        0     1185 2023-03-23 14:48:32.561618 dlt-0.2.9/dlt/common/wei.py
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.561618 dlt-0.2.9/dlt/destinations/__init__.py
--rw-r--r--   0        0        0      437 2023-03-23 14:48:32.561618 dlt-0.2.9/dlt/destinations/bigquery/README.md
--rw-r--r--   0        0        0     1813 2023-04-05 08:03:40.638919 dlt-0.2.9/dlt/destinations/bigquery/__init__.py
--rw-r--r--   0        0        0    12370 2023-05-29 14:13:02.418979 dlt-0.2.9/dlt/destinations/bigquery/bigquery.py
--rw-r--r--   0        0        0      386 2023-05-07 23:03:04.669469 dlt-0.2.9/dlt/destinations/bigquery/configuration.py
--rw-r--r--   0        0        0    10342 2023-05-07 23:03:04.669469 dlt-0.2.9/dlt/destinations/bigquery/sql_client.py
--rw-r--r--   0        0        0     1935 2023-04-05 08:03:40.638919 dlt-0.2.9/dlt/destinations/duckdb/__init__.py
--rw-r--r--   0        0        0     7207 2023-05-29 14:13:02.418979 dlt-0.2.9/dlt/destinations/duckdb/configuration.py
--rw-r--r--   0        0        0     2754 2023-03-23 14:48:32.561618 dlt-0.2.9/dlt/destinations/duckdb/duck.py
--rw-r--r--   0        0        0     6936 2023-04-21 22:25:54.789942 dlt-0.2.9/dlt/destinations/duckdb/sql_client.py
--rw-r--r--   0        0        0     1671 2023-03-23 14:48:32.561618 dlt-0.2.9/dlt/destinations/dummy/__init__.py
--rw-r--r--   0        0        0      736 2023-04-03 18:50:36.893525 dlt-0.2.9/dlt/destinations/dummy/configuration.py
--rw-r--r--   0        0        0     4989 2023-05-29 14:13:02.418979 dlt-0.2.9/dlt/destinations/dummy/dummy.py
--rw-r--r--   0        0        0     4159 2023-04-05 08:03:40.638919 dlt-0.2.9/dlt/destinations/exceptions.py
--rw-r--r--   0        0        0     1678 2023-05-29 14:13:02.418979 dlt-0.2.9/dlt/destinations/filesystem/__init__.py
--rw-r--r--   0        0        0     2253 2023-05-29 14:13:02.418979 dlt-0.2.9/dlt/destinations/filesystem/configuration.py
--rw-r--r--   0        0        0     4935 2023-05-29 14:13:02.418979 dlt-0.2.9/dlt/destinations/filesystem/filesystem.py
--rw-r--r--   0        0        0     1419 2023-05-29 14:13:02.418979 dlt-0.2.9/dlt/destinations/filesystem/filesystem_client.py
--rw-r--r--   0        0        0     5005 2023-05-29 14:13:02.418979 dlt-0.2.9/dlt/destinations/insert_job_client.py
--rw-r--r--   0        0        0    15639 2023-05-29 14:13:02.418979 dlt-0.2.9/dlt/destinations/job_client_impl.py
--rw-r--r--   0        0        0     1303 2023-04-05 08:03:40.638919 dlt-0.2.9/dlt/destinations/job_impl.py
--rw-r--r--   0        0        0      251 2023-03-23 14:48:32.561618 dlt-0.2.9/dlt/destinations/postgres/README.md
--rw-r--r--   0        0        0     1934 2023-04-05 08:03:40.638919 dlt-0.2.9/dlt/destinations/postgres/__init__.py
--rw-r--r--   0        0        0     1316 2023-05-29 18:11:09.008705 dlt-0.2.9/dlt/destinations/postgres/configuration.py
--rw-r--r--   0        0        0     3025 2023-03-23 14:48:32.561618 dlt-0.2.9/dlt/destinations/postgres/postgres.py
--rw-r--r--   0        0        0     6074 2023-05-07 23:03:04.669469 dlt-0.2.9/dlt/destinations/postgres/sql_client.py
--rw-r--r--   0        0        0     1159 2023-04-03 18:50:36.893525 dlt-0.2.9/dlt/destinations/redshift/README.md
--rw-r--r--   0        0        0     1905 2023-04-05 08:03:40.638919 dlt-0.2.9/dlt/destinations/redshift/__init__.py
--rw-r--r--   0        0        0      570 2023-05-07 23:03:04.669469 dlt-0.2.9/dlt/destinations/redshift/configuration.py
--rw-r--r--   0        0        0     3761 2023-03-23 14:48:32.561618 dlt-0.2.9/dlt/destinations/redshift/redshift.py
--rw-r--r--   0        0        0     7117 2023-05-28 13:56:42.341452 dlt-0.2.9/dlt/destinations/sql_client.py
--rw-r--r--   0        0        0    10090 2023-05-28 13:56:42.341452 dlt-0.2.9/dlt/destinations/sql_merge_job.py
--rw-r--r--   0        0        0     1931 2023-04-24 18:26:21.111453 dlt-0.2.9/dlt/destinations/typing.py
--rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.2.9/dlt/extract/__init__.py
--rw-r--r--   0        0        0    26237 2023-05-28 13:56:42.341452 dlt-0.2.9/dlt/extract/decorators.py
--rw-r--r--   0        0        0    12645 2023-04-30 21:17:44.398805 dlt-0.2.9/dlt/extract/exceptions.py
--rw-r--r--   0        0        0     8451 2023-05-24 16:38:22.538779 dlt-0.2.9/dlt/extract/extract.py
--rw-r--r--   0        0        0    14954 2023-05-24 16:38:22.538779 dlt-0.2.9/dlt/extract/incremental.py
--rw-r--r--   0        0        0    31816 2023-05-29 14:13:02.418979 dlt-0.2.9/dlt/extract/pipe.py
--rw-r--r--   0        0        0     9683 2023-05-24 16:38:22.538779 dlt-0.2.9/dlt/extract/schema.py
--rw-r--r--   0        0        0    36350 2023-05-28 13:56:42.341452 dlt-0.2.9/dlt/extract/source.py
--rw-r--r--   0        0        0     4308 2023-05-24 16:38:22.538779 dlt-0.2.9/dlt/extract/typing.py
--rw-r--r--   0        0        0      593 2023-04-06 20:38:35.239561 dlt-0.2.9/dlt/extract/utils.py
--rw-r--r--   0        0        0        0 2022-08-14 16:06:42.572263 dlt-0.2.9/dlt/helpers/__init__.py
--rw-r--r--   0        0        0    13783 2023-05-28 13:56:42.341452 dlt-0.2.9/dlt/helpers/airflow_helper.py
--rw-r--r--   0        0        0     2907 2023-03-23 14:48:32.561618 dlt-0.2.9/dlt/helpers/dbt/__init__.py
--rw-r--r--   0        0        0     1220 2023-03-23 14:48:32.561618 dlt-0.2.9/dlt/helpers/dbt/configuration.py
--rw-r--r--   0        0        0     6137 2023-03-23 14:48:32.561618 dlt-0.2.9/dlt/helpers/dbt/dbt_utils.py
--rw-r--r--   0        0        0      758 2023-03-23 14:48:32.561618 dlt-0.2.9/dlt/helpers/dbt/exceptions.py
--rw-r--r--   0        0        0     3583 2023-03-23 14:48:32.561618 dlt-0.2.9/dlt/helpers/dbt/profiles.yml
--rw-r--r--   0        0        0    13032 2023-04-30 21:17:44.398805 dlt-0.2.9/dlt/helpers/dbt/runner.py
--rw-r--r--   0        0        0     2490 2023-05-29 14:13:02.438979 dlt-0.2.9/dlt/helpers/pandas_helper.py
--rw-r--r--   0        0        0     1035 2023-03-23 14:48:32.571618 dlt-0.2.9/dlt/helpers/parquet.py
--rw-r--r--   0        0        0    13378 2023-05-29 14:13:02.438979 dlt-0.2.9/dlt/helpers/streamlit_helper.py
--rw-r--r--   0        0        0       31 2023-03-23 14:48:32.571618 dlt-0.2.9/dlt/load/__init__.py
--rw-r--r--   0        0        0     1005 2023-05-24 16:38:22.538779 dlt-0.2.9/dlt/load/configuration.py
--rw-r--r--   0        0        0     1993 2023-04-05 08:03:40.638919 dlt-0.2.9/dlt/load/exceptions.py
--rw-r--r--   0        0        0    19925 2023-05-29 14:13:02.418979 dlt-0.2.9/dlt/load/load.py
--rw-r--r--   0        0        0       32 2023-03-23 14:48:32.571618 dlt-0.2.9/dlt/normalize/__init__.py
--rw-r--r--   0        0        0     1101 2023-05-24 16:38:22.538779 dlt-0.2.9/dlt/normalize/configuration.py
--rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.2.9/dlt/normalize/exceptions.py
--rw-r--r--   0        0        0    16538 2023-05-24 16:38:22.538779 dlt-0.2.9/dlt/normalize/normalize.py
--rw-r--r--   0        0        0     1880 2023-03-23 14:48:32.571618 dlt-0.2.9/dlt/pipeline/README.md
--rw-r--r--   0        0        0    13081 2023-05-28 13:56:42.341452 dlt-0.2.9/dlt/pipeline/__init__.py
--rw-r--r--   0        0        0     1858 2023-04-30 21:17:44.398805 dlt-0.2.9/dlt/pipeline/configuration.py
--rw-r--r--   0        0        0      379 2023-05-24 16:38:22.538779 dlt-0.2.9/dlt/pipeline/current.py
--rw-r--r--   0        0        0     4829 2023-03-23 14:48:32.571618 dlt-0.2.9/dlt/pipeline/dbt.py
--rw-r--r--   0        0        0     3100 2023-05-28 13:56:42.341452 dlt-0.2.9/dlt/pipeline/exceptions.py
--rw-r--r--   0        0        0     8731 2023-05-25 19:30:59.799428 dlt-0.2.9/dlt/pipeline/helpers.py
--rw-r--r--   0        0        0      122 2023-04-06 15:27:24.759561 dlt-0.2.9/dlt/pipeline/mark.py
--rw-r--r--   0        0        0    58764 2023-05-29 14:13:02.438979 dlt-0.2.9/dlt/pipeline/pipeline.py
--rw-r--r--   0        0        0      985 2023-04-30 21:17:44.398805 dlt-0.2.9/dlt/pipeline/progress.py
--rw-r--r--   0        0        0     4200 2023-04-10 08:12:53.769595 dlt-0.2.9/dlt/pipeline/state_sync.py
--rw-r--r--   0        0        0     7990 2023-04-03 18:50:36.903525 dlt-0.2.9/dlt/pipeline/trace.py
--rw-r--r--   0        0        0     4625 2023-05-29 18:11:09.018705 dlt-0.2.9/dlt/pipeline/track.py
--rw-r--r--   0        0        0       91 2023-03-23 14:48:32.571618 dlt-0.2.9/dlt/pipeline/typing.py
--rw-r--r--   0        0        0        0 2022-06-03 13:18:25.174600 dlt-0.2.9/dlt/py.typed
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.571618 dlt-0.2.9/dlt/reflection/__init__.py
--rw-r--r--   0        0        0      563 2023-03-23 14:48:32.571618 dlt-0.2.9/dlt/reflection/names.py
--rw-r--r--   0        0        0     5617 2023-05-07 23:03:04.669469 dlt-0.2.9/dlt/reflection/script_inspector.py
--rw-r--r--   0        0        0     6186 2023-03-23 14:48:32.571618 dlt-0.2.9/dlt/reflection/script_visitor.py
--rw-r--r--   0        0        0      124 2023-05-07 23:03:04.669469 dlt-0.2.9/dlt/sources/__init__.py
--rw-r--r--   0        0        0      320 2023-05-07 23:03:04.669469 dlt-0.2.9/dlt/sources/credentials.py
--rw-r--r--   0        0        0        0 2023-03-23 14:48:32.571618 dlt-0.2.9/dlt/sources/helpers/__init__.py
--rw-r--r--   0        0        0      574 2023-03-23 14:48:37.261618 dlt-0.2.9/dlt/sources/helpers/requests/__init__.py
--rw-r--r--   0        0        0     9243 2023-05-29 14:13:02.418979 dlt-0.2.9/dlt/sources/helpers/requests/retry.py
--rw-r--r--   0        0        0     1336 2023-03-23 14:48:32.571618 dlt-0.2.9/dlt/sources/helpers/requests/session.py
--rw-r--r--   0        0        0      679 2023-04-06 15:27:24.759561 dlt-0.2.9/dlt/sources/helpers/transform.py
--rw-r--r--   0        0        0     1125 2023-04-22 20:26:30.632198 dlt-0.2.9/dlt/version.py
--rw-r--r--   0        0        0     4305 2023-05-29 14:16:01.278979 dlt-0.2.9/pyproject.toml
--rw-r--r--   0        0        0     7681 1970-01-01 00:00:00.000000 dlt-0.2.9/setup.py
--rw-r--r--   0        0        0     7684 1970-01-01 00:00:00.000000 dlt-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0    11343 2022-06-03 15:05:59.024600 dlt-0.2.9a0/LICENSE.txt
+-rw-r--r--   0        0        0     4214 2023-04-30 21:17:44.388805 dlt-0.2.9a0/README.md
+-rw-r--r--   0        0        0     1711 2023-04-30 21:17:44.388805 dlt-0.2.9a0/dlt/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-30 21:17:44.388805 dlt-0.2.9a0/dlt/cli/__init__.py
+-rw-r--r--   0        0        0    15909 2023-05-07 23:03:04.659469 dlt-0.2.9a0/dlt/cli/_dlt.py
+-rw-r--r--   0        0        0     3858 2023-05-07 23:03:04.659469 dlt-0.2.9a0/dlt/cli/config_toml_writer.py
+-rw-r--r--   0        0        0    16665 2023-05-14 20:33:31.539348 dlt-0.2.9a0/dlt/cli/deploy_command.py
+-rw-r--r--   0        0        0     1853 2023-04-30 21:17:44.388805 dlt-0.2.9a0/dlt/cli/echo.py
+-rw-r--r--   0        0        0      435 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/cli/exceptions.py
+-rw-r--r--   0        0        0    18827 2023-05-22 18:37:04.876212 dlt-0.2.9a0/dlt/cli/init_command.py
+-rw-r--r--   0        0        0    10489 2023-05-22 18:37:04.876212 dlt-0.2.9a0/dlt/cli/pipeline_command.py
+-rw-r--r--   0        0        0     9422 2023-05-14 20:33:31.539348 dlt-0.2.9a0/dlt/cli/pipeline_files.py
+-rw-r--r--   0        0        0     4505 2023-05-22 18:37:04.876212 dlt-0.2.9a0/dlt/cli/source_detection.py
+-rw-r--r--   0        0        0     1899 2023-04-22 20:26:30.632198 dlt-0.2.9a0/dlt/cli/telemetry_command.py
+-rw-r--r--   0        0        0     3757 2023-04-30 21:17:44.388805 dlt-0.2.9a0/dlt/cli/utils.py
+-rw-r--r--   0        0        0      307 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/common/__init__.py
+-rw-r--r--   0        0        0     1265 2022-08-24 09:42:09.472789 dlt-0.2.9a0/dlt/common/arithmetics.py
+-rw-r--r--   0        0        0      428 2023-05-22 18:37:04.886212 dlt-0.2.9a0/dlt/common/configuration/__init__.py
+-rw-r--r--   0        0        0     5078 2023-05-22 18:37:04.886212 dlt-0.2.9a0/dlt/common/configuration/accessors.py
+-rw-r--r--   0        0        0     3469 2023-05-07 23:03:04.659469 dlt-0.2.9a0/dlt/common/configuration/container.py
+-rw-r--r--   0        0        0     5884 2023-04-22 20:26:30.632198 dlt-0.2.9a0/dlt/common/configuration/exceptions.py
+-rw-r--r--   0        0        0     7912 2023-04-22 20:26:30.632198 dlt-0.2.9a0/dlt/common/configuration/inject.py
+-rw-r--r--   0        0        0     1791 2023-05-14 20:33:31.539348 dlt-0.2.9a0/dlt/common/configuration/paths.py
+-rw-r--r--   0        0        0      306 2023-05-07 23:03:04.659469 dlt-0.2.9a0/dlt/common/configuration/providers/__init__.py
+-rw-r--r--   0        0        0     1108 2023-05-19 14:44:37.212613 dlt-0.2.9a0/dlt/common/configuration/providers/airflow.py
+-rw-r--r--   0        0        0     1116 2023-05-07 23:03:04.659469 dlt-0.2.9a0/dlt/common/configuration/providers/context.py
+-rw-r--r--   0        0        0     1335 2023-05-07 23:03:04.659469 dlt-0.2.9a0/dlt/common/configuration/providers/dictionary.py
+-rw-r--r--   0        0        0     1981 2023-05-07 23:03:04.659469 dlt-0.2.9a0/dlt/common/configuration/providers/environ.py
+-rw-r--r--   0        0        0     8349 2023-05-22 21:42:58.160654 dlt-0.2.9a0/dlt/common/configuration/providers/google_secrets.py
+-rw-r--r--   0        0        0     1306 2023-05-22 18:37:04.886212 dlt-0.2.9a0/dlt/common/configuration/providers/provider.py
+-rw-r--r--   0        0        0     6560 2023-05-22 18:37:04.886212 dlt-0.2.9a0/dlt/common/configuration/providers/toml.py
+-rw-r--r--   0        0        0    17262 2023-05-22 18:37:04.886212 dlt-0.2.9a0/dlt/common/configuration/resolve.py
+-rw-r--r--   0        0        0      912 2023-05-22 18:37:04.886212 dlt-0.2.9a0/dlt/common/configuration/specs/__init__.py
+-rw-r--r--   0        0        0     1817 2023-05-07 23:03:04.659469 dlt-0.2.9a0/dlt/common/configuration/specs/api_credentials.py
+-rw-r--r--   0        0        0    13108 2023-05-22 18:37:04.886212 dlt-0.2.9a0/dlt/common/configuration/specs/base_configuration.py
+-rw-r--r--   0        0        0     5521 2023-05-14 20:33:31.539348 dlt-0.2.9a0/dlt/common/configuration/specs/config_providers_context.py
+-rw-r--r--   0        0        0     2792 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/common/configuration/specs/config_section_context.py
+-rw-r--r--   0        0        0     1818 2023-05-22 18:37:04.896212 dlt-0.2.9a0/dlt/common/configuration/specs/connection_string_credentials.py
+-rw-r--r--   0        0        0     2125 2023-04-24 18:26:21.111453 dlt-0.2.9a0/dlt/common/configuration/specs/exceptions.py
+-rw-r--r--   0        0        0    12725 2023-05-07 23:03:04.669469 dlt-0.2.9a0/dlt/common/configuration/specs/gcp_credentials.py
+-rw-r--r--   0        0        0      725 2023-05-07 23:03:04.669469 dlt-0.2.9a0/dlt/common/configuration/specs/known_sections.py
+-rw-r--r--   0        0        0     2455 2023-04-30 21:17:44.388805 dlt-0.2.9a0/dlt/common/configuration/specs/run_configuration.py
+-rw-r--r--   0        0        0     6026 2023-05-07 23:03:04.669469 dlt-0.2.9a0/dlt/common/configuration/utils.py
+-rw-r--r--   0        0        0      142 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/common/data_types/__init__.py
+-rw-r--r--   0        0        0     6306 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/common/data_types/type_helpers.py
+-rw-r--r--   0        0        0      214 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/common/data_types/typing.py
+-rw-r--r--   0        0        0      260 2023-03-23 14:48:20.701618 dlt-0.2.9a0/dlt/common/data_writers/__init__.py
+-rw-r--r--   0        0        0     5893 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/common/data_writers/buffered.py
+-rw-r--r--   0        0        0     2395 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/common/data_writers/escape.py
+-rw-r--r--   0        0        0      962 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/common/data_writers/exceptions.py
+-rw-r--r--   0        0        0     5159 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/common/data_writers/writers.py
+-rw-r--r--   0        0        0       97 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/common/destination/__init__.py
+-rw-r--r--   0        0        0     2206 2023-04-05 08:03:40.638919 dlt-0.2.9a0/dlt/common/destination/capabilities.py
+-rw-r--r--   0        0        0    10682 2023-05-22 18:37:04.896212 dlt-0.2.9a0/dlt/common/destination/reference.py
+-rw-r--r--   0        0        0     6451 2023-05-22 18:37:04.896212 dlt-0.2.9a0/dlt/common/exceptions.py
+-rw-r--r--   0        0        0     4954 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/common/git.py
+-rw-r--r--   0        0        0     5253 2023-05-14 20:33:31.539348 dlt-0.2.9a0/dlt/common/json/__init__.py
+-rw-r--r--   0        0        0     1802 2023-04-10 08:12:53.769595 dlt-0.2.9a0/dlt/common/json/_orjson.py
+-rw-r--r--   0        0        0     2939 2023-04-10 08:12:53.769595 dlt-0.2.9a0/dlt/common/json/_simplejson.py
+-rw-r--r--   0        0        0     1536 2023-04-29 12:58:55.943219 dlt-0.2.9a0/dlt/common/jsonpath.py
+-rw-r--r--   0        0        0      232 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/common/normalizers/__init__.py
+-rw-r--r--   0        0        0     1197 2023-05-07 23:03:04.669469 dlt-0.2.9a0/dlt/common/normalizers/configuration.py
+-rw-r--r--   0        0        0      472 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/common/normalizers/exceptions.py
+-rw-r--r--   0        0        0     1644 2023-04-06 15:27:24.759561 dlt-0.2.9a0/dlt/common/normalizers/json/__init__.py
+-rw-r--r--   0        0        0    13382 2023-05-14 20:33:31.539348 dlt-0.2.9a0/dlt/common/normalizers/json/relational.py
+-rw-r--r--   0        0        0       64 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/common/normalizers/naming/__init__.py
+-rw-r--r--   0        0        0      807 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/common/normalizers/naming/direct.py
+-rw-r--r--   0        0        0     1069 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/common/normalizers/naming/duck_case.py
+-rw-r--r--   0        0        0      792 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/common/normalizers/naming/exceptions.py
+-rw-r--r--   0        0        0     3753 2023-04-05 08:03:40.638919 dlt-0.2.9a0/dlt/common/normalizers/naming/naming.py
+-rw-r--r--   0        0        0     3002 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/common/normalizers/naming/snake_case.py
+-rw-r--r--   0        0        0      358 2023-04-02 09:09:15.855769 dlt-0.2.9a0/dlt/common/normalizers/typing.py
+-rw-r--r--   0        0        0     2337 2023-04-06 15:27:24.759561 dlt-0.2.9a0/dlt/common/normalizers/utils.py
+-rw-r--r--   0        0        0      451 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/common/pendulum.py
+-rw-r--r--   0        0        0    19121 2023-05-22 18:37:04.896212 dlt-0.2.9a0/dlt/common/pipeline.py
+-rw-r--r--   0        0        0        0 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/common/reflection/__init__.py
+-rw-r--r--   0        0        0      374 2023-03-23 14:48:32.551618 dlt-0.2.9a0/dlt/common/reflection/function_visitor.py
+-rw-r--r--   0        0        0     4891 2023-04-09 16:39:04.593180 dlt-0.2.9a0/dlt/common/reflection/spec.py
+-rw-r--r--   0        0        0     5069 2023-04-24 18:26:21.111453 dlt-0.2.9a0/dlt/common/reflection/utils.py
+-rw-r--r--   0        0        0      174 2023-04-30 21:17:44.388805 dlt-0.2.9a0/dlt/common/runners/__init__.py
+-rw-r--r--   0        0        0      705 2023-05-22 18:37:04.896212 dlt-0.2.9a0/dlt/common/runners/configuration.py
+-rw-r--r--   0        0        0     2635 2023-05-14 11:08:47.420838 dlt-0.2.9a0/dlt/common/runners/pool_runner.py
+-rw-r--r--   0        0        0     4046 2023-03-23 14:48:32.561618 dlt-0.2.9a0/dlt/common/runners/runnable.py
+-rw-r--r--   0        0        0     3145 2023-03-23 14:48:32.561618 dlt-0.2.9a0/dlt/common/runners/stdout.py
+-rw-r--r--   0        0        0     2137 2023-03-23 14:48:32.561618 dlt-0.2.9a0/dlt/common/runners/synth_pickle.py
+-rw-r--r--   0        0        0      105 2023-04-30 21:17:44.388805 dlt-0.2.9a0/dlt/common/runners/typing.py
+-rw-r--r--   0        0        0     5590 2023-05-07 23:03:04.669469 dlt-0.2.9a0/dlt/common/runners/venv.py
+-rw-r--r--   0        0        0       36 2023-04-30 21:17:44.398805 dlt-0.2.9a0/dlt/common/runtime/__init__.py
+-rw-r--r--   0        0        0    13441 2023-04-30 21:17:44.398805 dlt-0.2.9a0/dlt/common/runtime/collector.py
+-rw-r--r--   0        0        0     4501 2023-05-14 20:33:31.539348 dlt-0.2.9a0/dlt/common/runtime/exec_info.py
+-rw-r--r--   0        0        0      647 2023-04-30 21:17:44.398805 dlt-0.2.9a0/dlt/common/runtime/init.py
+-rw-r--r--   0        0        0     4002 2023-04-30 21:17:44.398805 dlt-0.2.9a0/dlt/common/runtime/logger.py
+-rw-r--r--   0        0        0     2052 2023-04-30 21:17:44.398805 dlt-0.2.9a0/dlt/common/runtime/prometheus.py
+-rw-r--r--   0        0        0     7170 2023-05-14 20:33:31.539348 dlt-0.2.9a0/dlt/common/runtime/segment.py
+-rw-r--r--   0        0        0     2493 2023-04-30 21:17:44.398805 dlt-0.2.9a0/dlt/common/runtime/sentry.py
+-rw-r--r--   0        0        0     2027 2023-04-30 21:17:44.398805 dlt-0.2.9a0/dlt/common/runtime/signals.py
+-rw-r--r--   0        0        0      616 2023-04-03 18:50:36.893525 dlt-0.2.9a0/dlt/common/runtime/slack.py
+-rw-r--r--   0        0        0      720 2023-04-30 21:17:44.398805 dlt-0.2.9a0/dlt/common/runtime/telemetry.py
+-rw-r--r--   0        0        0      387 2023-04-03 18:50:36.893525 dlt-0.2.9a0/dlt/common/schema/__init__.py
+-rw-r--r--   0        0        0     1927 2023-03-23 14:48:32.561618 dlt-0.2.9a0/dlt/common/schema/detections.py
+-rw-r--r--   0        0        0     2974 2023-03-23 14:48:32.561618 dlt-0.2.9a0/dlt/common/schema/exceptions.py
+-rw-r--r--   0        0        0    25175 2023-04-09 16:39:04.593180 dlt-0.2.9a0/dlt/common/schema/schema.py
+-rw-r--r--   0        0        0     3004 2023-04-22 20:26:30.632198 dlt-0.2.9a0/dlt/common/schema/typing.py
+-rw-r--r--   0        0        0    23087 2023-04-30 21:17:44.398805 dlt-0.2.9a0/dlt/common/schema/utils.py
+-rw-r--r--   0        0        0     1467 2023-05-22 18:37:04.896212 dlt-0.2.9a0/dlt/common/source.py
+-rw-r--r--   0        0        0      554 2023-05-22 18:37:04.896212 dlt-0.2.9a0/dlt/common/storages/__init__.py
+-rw-r--r--   0        0        0     1649 2023-05-22 18:37:04.896212 dlt-0.2.9a0/dlt/common/storages/configuration.py
+-rw-r--r--   0        0        0     1906 2023-03-23 14:48:32.561618 dlt-0.2.9a0/dlt/common/storages/data_item_storage.py
+-rw-r--r--   0        0        0     2804 2023-04-03 18:50:36.893525 dlt-0.2.9a0/dlt/common/storages/exceptions.py
+-rw-r--r--   0        0        0    10891 2023-05-14 20:33:31.539348 dlt-0.2.9a0/dlt/common/storages/file_storage.py
+-rw-r--r--   0        0        0     2690 2023-05-22 18:37:04.896212 dlt-0.2.9a0/dlt/common/storages/live_schema_storage.py
+-rw-r--r--   0        0        0    21812 2023-05-22 18:37:04.896212 dlt-0.2.9a0/dlt/common/storages/load_storage.py
+-rw-r--r--   0        0        0     2409 2023-05-22 18:37:04.896212 dlt-0.2.9a0/dlt/common/storages/normalize_storage.py
+-rw-r--r--   0        0        0     8434 2023-05-22 18:37:04.906212 dlt-0.2.9a0/dlt/common/storages/schema_storage.py
+-rw-r--r--   0        0        0     2525 2023-04-24 18:26:21.111453 dlt-0.2.9a0/dlt/common/storages/versioned_storage.py
+-rw-r--r--   0        0        0     2634 2023-05-07 23:03:04.669469 dlt-0.2.9a0/dlt/common/time.py
+-rw-r--r--   0        0        0     4736 2023-04-03 18:50:36.893525 dlt-0.2.9a0/dlt/common/typing.py
+-rw-r--r--   0        0        0    14239 2023-05-22 20:03:28.546212 dlt-0.2.9a0/dlt/common/utils.py
+-rw-r--r--   0        0        0     3686 2023-03-23 14:48:32.561618 dlt-0.2.9a0/dlt/common/validation.py
+-rw-r--r--   0        0        0     1185 2023-03-23 14:48:32.561618 dlt-0.2.9a0/dlt/common/wei.py
+-rw-r--r--   0        0        0        0 2023-03-23 14:48:32.561618 dlt-0.2.9a0/dlt/destinations/__init__.py
+-rw-r--r--   0        0        0      437 2023-03-23 14:48:32.561618 dlt-0.2.9a0/dlt/destinations/bigquery/README.md
+-rw-r--r--   0        0        0     1813 2023-04-05 08:03:40.638919 dlt-0.2.9a0/dlt/destinations/bigquery/__init__.py
+-rw-r--r--   0        0        0    12347 2023-05-22 18:37:04.906212 dlt-0.2.9a0/dlt/destinations/bigquery/bigquery.py
+-rw-r--r--   0        0        0      386 2023-05-07 23:03:04.669469 dlt-0.2.9a0/dlt/destinations/bigquery/configuration.py
+-rw-r--r--   0        0        0    10342 2023-05-07 23:03:04.669469 dlt-0.2.9a0/dlt/destinations/bigquery/sql_client.py
+-rw-r--r--   0        0        0     1935 2023-04-05 08:03:40.638919 dlt-0.2.9a0/dlt/destinations/duckdb/__init__.py
+-rw-r--r--   0        0        0     7008 2023-05-07 23:03:04.669469 dlt-0.2.9a0/dlt/destinations/duckdb/configuration.py
+-rw-r--r--   0        0        0     2754 2023-03-23 14:48:32.561618 dlt-0.2.9a0/dlt/destinations/duckdb/duck.py
+-rw-r--r--   0        0        0     6936 2023-04-21 22:25:54.789942 dlt-0.2.9a0/dlt/destinations/duckdb/sql_client.py
+-rw-r--r--   0        0        0     1671 2023-03-23 14:48:32.561618 dlt-0.2.9a0/dlt/destinations/dummy/__init__.py
+-rw-r--r--   0        0        0      736 2023-04-03 18:50:36.893525 dlt-0.2.9a0/dlt/destinations/dummy/configuration.py
+-rw-r--r--   0        0        0     4975 2023-05-22 18:37:04.906212 dlt-0.2.9a0/dlt/destinations/dummy/dummy.py
+-rw-r--r--   0        0        0     4159 2023-04-05 08:03:40.638919 dlt-0.2.9a0/dlt/destinations/exceptions.py
+-rw-r--r--   0        0        0     4983 2023-05-22 18:37:04.906212 dlt-0.2.9a0/dlt/destinations/insert_job_client.py
+-rw-r--r--   0        0        0    15625 2023-05-22 18:37:04.906212 dlt-0.2.9a0/dlt/destinations/job_client_impl.py
+-rw-r--r--   0        0        0     1303 2023-04-05 08:03:40.638919 dlt-0.2.9a0/dlt/destinations/job_impl.py
+-rw-r--r--   0        0        0      251 2023-03-23 14:48:32.561618 dlt-0.2.9a0/dlt/destinations/postgres/README.md
+-rw-r--r--   0        0        0     1934 2023-04-05 08:03:40.638919 dlt-0.2.9a0/dlt/destinations/postgres/__init__.py
+-rw-r--r--   0        0        0     1232 2023-05-07 23:03:04.669469 dlt-0.2.9a0/dlt/destinations/postgres/configuration.py
+-rw-r--r--   0        0        0     3025 2023-03-23 14:48:32.561618 dlt-0.2.9a0/dlt/destinations/postgres/postgres.py
+-rw-r--r--   0        0        0     6074 2023-05-07 23:03:04.669469 dlt-0.2.9a0/dlt/destinations/postgres/sql_client.py
+-rw-r--r--   0        0        0     1159 2023-04-03 18:50:36.893525 dlt-0.2.9a0/dlt/destinations/redshift/README.md
+-rw-r--r--   0        0        0     1905 2023-04-05 08:03:40.638919 dlt-0.2.9a0/dlt/destinations/redshift/__init__.py
+-rw-r--r--   0        0        0      570 2023-05-07 23:03:04.669469 dlt-0.2.9a0/dlt/destinations/redshift/configuration.py
+-rw-r--r--   0        0        0     3761 2023-03-23 14:48:32.561618 dlt-0.2.9a0/dlt/destinations/redshift/redshift.py
+-rw-r--r--   0        0        0     7110 2023-04-29 12:58:55.953219 dlt-0.2.9a0/dlt/destinations/sql_client.py
+-rw-r--r--   0        0        0    10101 2023-04-09 16:39:04.593180 dlt-0.2.9a0/dlt/destinations/sql_merge_job.py
+-rw-r--r--   0        0        0     1931 2023-04-24 18:26:21.111453 dlt-0.2.9a0/dlt/destinations/typing.py
+-rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.2.9a0/dlt/extract/__init__.py
+-rw-r--r--   0        0        0    26199 2023-05-22 18:37:04.906212 dlt-0.2.9a0/dlt/extract/decorators.py
+-rw-r--r--   0        0        0    12645 2023-04-30 21:17:44.398805 dlt-0.2.9a0/dlt/extract/exceptions.py
+-rw-r--r--   0        0        0     8451 2023-05-22 18:37:04.906212 dlt-0.2.9a0/dlt/extract/extract.py
+-rw-r--r--   0        0        0    14954 2023-05-22 18:37:04.906212 dlt-0.2.9a0/dlt/extract/incremental.py
+-rw-r--r--   0        0        0    31737 2023-05-22 18:37:04.906212 dlt-0.2.9a0/dlt/extract/pipe.py
+-rw-r--r--   0        0        0     9683 2023-05-22 18:37:10.826212 dlt-0.2.9a0/dlt/extract/schema.py
+-rw-r--r--   0        0        0    36384 2023-05-22 21:03:03.346212 dlt-0.2.9a0/dlt/extract/source.py
+-rw-r--r--   0        0        0     4308 2023-05-22 18:37:10.826212 dlt-0.2.9a0/dlt/extract/typing.py
+-rw-r--r--   0        0        0      593 2023-04-06 20:38:35.239561 dlt-0.2.9a0/dlt/extract/utils.py
+-rw-r--r--   0        0        0        0 2022-08-14 16:06:42.572263 dlt-0.2.9a0/dlt/helpers/__init__.py
+-rw-r--r--   0        0        0      267 2023-05-14 20:33:31.539348 dlt-0.2.9a0/dlt/helpers/airflow.py
+-rw-r--r--   0        0        0     2907 2023-03-23 14:48:32.561618 dlt-0.2.9a0/dlt/helpers/dbt/__init__.py
+-rw-r--r--   0        0        0     1220 2023-03-23 14:48:32.561618 dlt-0.2.9a0/dlt/helpers/dbt/configuration.py
+-rw-r--r--   0        0        0     6137 2023-03-23 14:48:32.561618 dlt-0.2.9a0/dlt/helpers/dbt/dbt_utils.py
+-rw-r--r--   0        0        0      758 2023-03-23 14:48:32.561618 dlt-0.2.9a0/dlt/helpers/dbt/exceptions.py
+-rw-r--r--   0        0        0     3583 2023-03-23 14:48:32.561618 dlt-0.2.9a0/dlt/helpers/dbt/profiles.yml
+-rw-r--r--   0        0        0    13032 2023-04-30 21:17:44.398805 dlt-0.2.9a0/dlt/helpers/dbt/runner.py
+-rw-r--r--   0        0        0     2490 2023-05-14 20:33:31.539348 dlt-0.2.9a0/dlt/helpers/pandas.py
+-rw-r--r--   0        0        0     1035 2023-03-23 14:48:32.571618 dlt-0.2.9a0/dlt/helpers/parquet.py
+-rw-r--r--   0        0        0    13371 2023-04-30 21:17:44.398805 dlt-0.2.9a0/dlt/helpers/streamlit.py
+-rw-r--r--   0        0        0       31 2023-03-23 14:48:32.571618 dlt-0.2.9a0/dlt/load/__init__.py
+-rw-r--r--   0        0        0     1005 2023-05-22 18:37:04.906212 dlt-0.2.9a0/dlt/load/configuration.py
+-rw-r--r--   0        0        0     1993 2023-04-05 08:03:40.638919 dlt-0.2.9a0/dlt/load/exceptions.py
+-rw-r--r--   0        0        0    19928 2023-05-22 18:37:04.906212 dlt-0.2.9a0/dlt/load/load.py
+-rw-r--r--   0        0        0       32 2023-03-23 14:48:32.571618 dlt-0.2.9a0/dlt/normalize/__init__.py
+-rw-r--r--   0        0        0     1101 2023-05-22 18:37:04.906212 dlt-0.2.9a0/dlt/normalize/configuration.py
+-rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 dlt-0.2.9a0/dlt/normalize/exceptions.py
+-rw-r--r--   0        0        0    16538 2023-05-22 18:37:04.916212 dlt-0.2.9a0/dlt/normalize/normalize.py
+-rw-r--r--   0        0        0     1880 2023-03-23 14:48:32.571618 dlt-0.2.9a0/dlt/pipeline/README.md
+-rw-r--r--   0        0        0    13138 2023-04-30 21:17:44.398805 dlt-0.2.9a0/dlt/pipeline/__init__.py
+-rw-r--r--   0        0        0     1858 2023-04-30 21:17:44.398805 dlt-0.2.9a0/dlt/pipeline/configuration.py
+-rw-r--r--   0        0        0      379 2023-05-22 18:37:04.916212 dlt-0.2.9a0/dlt/pipeline/current.py
+-rw-r--r--   0        0        0     4829 2023-03-23 14:48:32.571618 dlt-0.2.9a0/dlt/pipeline/dbt.py
+-rw-r--r--   0        0        0     2891 2023-04-30 21:17:44.398805 dlt-0.2.9a0/dlt/pipeline/exceptions.py
+-rw-r--r--   0        0        0     8764 2023-05-07 23:03:04.669469 dlt-0.2.9a0/dlt/pipeline/helpers.py
+-rw-r--r--   0        0        0      122 2023-04-06 15:27:24.759561 dlt-0.2.9a0/dlt/pipeline/mark.py
+-rw-r--r--   0        0        0    56453 2023-05-22 18:37:10.826212 dlt-0.2.9a0/dlt/pipeline/pipeline.py
+-rw-r--r--   0        0        0      985 2023-04-30 21:17:44.398805 dlt-0.2.9a0/dlt/pipeline/progress.py
+-rw-r--r--   0        0        0     4200 2023-04-10 08:12:53.769595 dlt-0.2.9a0/dlt/pipeline/state_sync.py
+-rw-r--r--   0        0        0     7990 2023-04-03 18:50:36.903525 dlt-0.2.9a0/dlt/pipeline/trace.py
+-rw-r--r--   0        0        0     4563 2023-04-03 18:50:36.903525 dlt-0.2.9a0/dlt/pipeline/track.py
+-rw-r--r--   0        0        0       91 2023-03-23 14:48:32.571618 dlt-0.2.9a0/dlt/pipeline/typing.py
+-rw-r--r--   0        0        0        0 2022-06-03 13:18:25.174600 dlt-0.2.9a0/dlt/py.typed
+-rw-r--r--   0        0        0        0 2023-03-23 14:48:32.571618 dlt-0.2.9a0/dlt/reflection/__init__.py
+-rw-r--r--   0        0        0      563 2023-03-23 14:48:32.571618 dlt-0.2.9a0/dlt/reflection/names.py
+-rw-r--r--   0        0        0     5617 2023-05-07 23:03:04.669469 dlt-0.2.9a0/dlt/reflection/script_inspector.py
+-rw-r--r--   0        0        0     6186 2023-03-23 14:48:32.571618 dlt-0.2.9a0/dlt/reflection/script_visitor.py
+-rw-r--r--   0        0        0      124 2023-05-07 23:03:04.669469 dlt-0.2.9a0/dlt/sources/__init__.py
+-rw-r--r--   0        0        0      320 2023-05-07 23:03:04.669469 dlt-0.2.9a0/dlt/sources/credentials.py
+-rw-r--r--   0        0        0        0 2023-03-23 14:48:32.571618 dlt-0.2.9a0/dlt/sources/helpers/__init__.py
+-rw-r--r--   0        0        0      574 2023-03-23 14:48:37.261618 dlt-0.2.9a0/dlt/sources/helpers/requests/__init__.py
+-rw-r--r--   0        0        0     9106 2023-05-14 20:33:31.539348 dlt-0.2.9a0/dlt/sources/helpers/requests/retry.py
+-rw-r--r--   0        0        0     1336 2023-03-23 14:48:32.571618 dlt-0.2.9a0/dlt/sources/helpers/requests/session.py
+-rw-r--r--   0        0        0      679 2023-04-06 15:27:24.759561 dlt-0.2.9a0/dlt/sources/helpers/transform.py
+-rw-r--r--   0        0        0     1125 2023-04-22 20:26:30.632198 dlt-0.2.9a0/dlt/version.py
+-rw-r--r--   0        0        0     4056 2023-05-22 21:06:28.566212 dlt-0.2.9a0/pyproject.toml
+-rw-r--r--   0        0        0     7371 1970-01-01 00:00:00.000000 dlt-0.2.9a0/setup.py
+-rw-r--r--   0        0        0     7323 1970-01-01 00:00:00.000000 dlt-0.2.9a0/PKG-INFO
```

### Comparing `dlt-0.2.9/LICENSE.txt` & `dlt-0.2.9a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/README.md` & `dlt-0.2.9a0/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/__init__.py` & `dlt-0.2.9a0/dlt/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/cli/_dlt.py` & `dlt-0.2.9a0/dlt/cli/_dlt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from typing import Any, Sequence, Optional
+from typing import Any, Sequence
 import yaml
 import os
 import argparse
 import click
 
 from dlt.version import __version__
 from dlt.common import json
 from dlt.common.schema import Schema
 from dlt.common.typing import DictStrAny
 from dlt.common.runners import Venv
 
 import dlt.cli.echo as fmt
 from dlt.cli import utils
 from dlt.cli.init_command import init_command, list_pipelines_command, DLT_INIT_DOCS_URL, DEFAULT_PIPELINES_REPO
-from dlt.cli.deploy_command import PipelineWasNotRun, deploy_command, DLT_DEPLOY_DOCS_URL, DeploymentMethods, COMMAND_DEPLOY_REPO_LOCATION
+from dlt.cli.deploy_command import PipelineWasNotRun, deploy_command, DLT_DEPLOY_DOCS_URL
 from dlt.cli.pipeline_command import pipeline_command, DLT_PIPELINE_COMMAND_DOCS_URL
 from dlt.cli.telemetry_command import DLT_TELEMETRY_DOCS_URL, change_telemetry_status_command, telemetry_status_command
 from dlt.pipeline.exceptions import CannotRestorePipelineException
 
 
 @utils.track_command("init", False, "pipeline_name", "destination_name")
 def init_command_wrapper(pipeline_name: str, destination_name: str, use_generic_template: bool, repo_location: str, branch: str) -> int:
@@ -38,58 +38,48 @@
         click.secho(str(ex), err=True, fg="red")
         fmt.note("Please refer to %s for further assistance" % fmt.bold(DLT_INIT_DOCS_URL))
         return -1
     return 0
 
 
 @utils.track_command("deploy", False, "deployment_method")
-def deploy_command_wrapper(
-    pipeline_script_path: str,
-    deployment_method: str,
-    schedule: Optional[str],
-    run_on_push: bool,
-    run_on_dispatch: bool,
-    repo_location: str,
-    branch: Optional[str]) -> int:
+def deploy_command_wrapper(pipeline_script_path: str, deployment_method: str, schedule: str, run_on_push: bool, run_on_dispatch: bool, branch: str) -> int:
     try:
         utils.ensure_git_command("deploy")
     except Exception as ex:
         click.secho(str(ex), err=True, fg="red")
         return -1
 
     from git import InvalidGitRepositoryError, NoSuchPathError
     try:
-        deploy_command(pipeline_script_path, deployment_method, schedule, run_on_push, run_on_dispatch, repo_location, branch)
+        deploy_command(pipeline_script_path, deployment_method, schedule, run_on_push, run_on_dispatch, branch)
     except (CannotRestorePipelineException, PipelineWasNotRun) as ex:
         click.secho(str(ex), err=True, fg="red")
         fmt.note("You must run the pipeline locally successfully at least once in order to deploy it.")
         fmt.note("Please refer to %s for further assistance" % fmt.bold(DLT_DEPLOY_DOCS_URL))
         return -1
     except InvalidGitRepositoryError:
         click.secho(
-            "No git repository found for pipeline script %s." % fmt.bold(pipeline_script_path),
+            "No git repository found for pipeline script %s.\nAdd your local code to Github as described here: %s" % (fmt.bold(pipeline_script_path), fmt.bold("https://docs.github.com/en/get-started/importing-your-projects-to-github/importing-source-code-to-github/adding-locally-hosted-code-to-github")),
             err=True,
             fg="red"
         )
-        fmt.note("If you do not have a repository yet, you can do either of:")
-        fmt.note("- Run the following command to initialize new repository: %s" % fmt.bold("git init"))
-        fmt.note("- Add your local code to Github as described here: %s" % fmt.bold("https://docs.github.com/en/get-started/importing-your-projects-to-github/importing-source-code-to-github/adding-locally-hosted-code-to-github"))
+        fmt.note("If you do not have a repository yet, the easiest way to proceed is to create one on Github and then clone it here.")
         fmt.note("Please refer to %s for further assistance" % fmt.bold(DLT_DEPLOY_DOCS_URL))
         return -1
     except NoSuchPathError as path_ex:
         click.secho(
             "The pipeline script does not exist\n%s" % str(path_ex),
             err=True,
             fg="red"
         )
         return -1
     except Exception as ex:
         click.secho(str(ex), err=True, fg="red")
         fmt.note("Please refer to %s for further assistance" % fmt.bold(DLT_DEPLOY_DOCS_URL))
-        return -1
         # TODO: display stack trace if with debug flag
     return 0
 
 
 @utils.track_command("pipeline", True, "operation")
 def pipeline_command_wrapper(
         operation: str, pipeline_name: str, pipelines_dir: str, verbosity: int, **command_kwargs: Any
@@ -194,38 +184,32 @@
     init_cmd.add_argument("destination", nargs='?', help="Name of a destination ie. bigquery or redshift")
     init_cmd.add_argument("--location", default=DEFAULT_PIPELINES_REPO, help="Advanced. Uses a specific url or local path to pipelines repository.")
     init_cmd.add_argument("--branch", default=None, help="Advanced. Uses specific branch of the init repository to fetch the template.")
     init_cmd.add_argument("--generic", default=False, action="store_true", help="When present uses a generic template with all the dlt loading code present will be used. Otherwise a debug template is used that can be immediately run to get familiar with the dlt sources.")
 
     deploy_cmd = subparsers.add_parser("deploy", help="Creates a deployment package for a selected pipeline script")
     deploy_cmd.add_argument("pipeline_script_path", metavar="pipeline-script-path", help="Path to a pipeline script")
-    deploy_cmd.add_argument(
-        "deployment_method",
-        metavar="deployment-method",
-        choices=list(map(lambda value: value.value, DeploymentMethods.__members__.values())),
-        default=DeploymentMethods.github_actions.value,
-        help="Deployment method: %s" % ", ".join(map(lambda value: value.value, DeploymentMethods.__members__.values())))
-    deploy_cmd.add_argument("--schedule", required=False, help="A schedule with which to run the pipeline, in cron format. Example: '*/30 * * * *' will run the pipeline every 30 minutes.")
+    deploy_cmd.add_argument("deployment_method", metavar="deployment-method", choices=["github-action"], default="github-action", help="Deployment method")
+    deploy_cmd.add_argument("--schedule", required=True, help="A schedule with which to run the pipeline, in cron format. Example: '*/30 * * * *' will run the pipeline every 30 minutes.")
     deploy_cmd.add_argument("--run-manually", default=True, action="store_true", help="Allows the pipeline to be run manually form Github Actions UI.")
     deploy_cmd.add_argument("--run-on-push", default=False, action="store_true", help="Runs the pipeline with every push to the repository.")
-    deploy_cmd.add_argument("--location", default=COMMAND_DEPLOY_REPO_LOCATION, help="Advanced. Uses a specific url or local path to pipelines repository.")
     deploy_cmd.add_argument("--branch", default=None, help="Advanced. Uses specific branch of the deploy repository to fetch the template.")
 
     schema = subparsers.add_parser("schema", help="Shows, converts and upgrades schemas")
     schema.add_argument("file", help="Schema file name, in yaml or json format, will autodetect based on extension")
     schema.add_argument("--format", choices=["json", "yaml"], default="yaml", help="Display schema in this format")
     schema.add_argument("--remove-defaults", action="store_true", help="Does not show default hint values")
 
     pipe_cmd = subparsers.add_parser("pipeline", help="Operations on pipelines that were ran locally")
     pipe_cmd.add_argument("--list-pipelines", "-l",  default=False, action="store_true", help="List local pipelines")
     pipe_cmd.add_argument("pipeline_name", nargs='?', help="Pipeline name")
     pipe_cmd.add_argument("--pipelines-dir", help="Pipelines working directory", default=None)
     pipe_cmd.add_argument("--verbose", "-v", action='count', default=0, help="Provides more information for certain commands.", dest="verbosity")
     # pipe_cmd.add_argument("--dataset-name", help="Dataset name used to sync destination when local pipeline state is missing.")
-    # pipe_cmd.add_argument("--destination", help="Destination name used to sync when local pipeline state is missing.")
+    # pipe_cmd.add_argument("--destination", help="Destination name used to to sync when local pipeline state is missing.")
 
     pipeline_subparsers = pipe_cmd.add_subparsers(dest="operation", required=False)
 
     pipe_cmd_sync_parent = argparse.ArgumentParser(add_help=False)
     pipe_cmd_sync_parent.add_argument("--destination", help="Sync from this destination when local pipeline state is missing.")
     pipe_cmd_sync_parent.add_argument("--dataset-name", help="Dataset name to sync from when local pipeline state is missing.")
 
@@ -281,15 +265,15 @@
         else:
             if not args.pipeline or not args.destination:
                 init_cmd.print_usage()
                 return -1
             else:
                 return init_command_wrapper(args.pipeline, args.destination, args.generic, args.location, args.branch)
     elif args.command == "deploy":
-        return deploy_command_wrapper(args.pipeline_script_path, args.deployment_method, args.schedule, args.run_on_push, args.run_manually, args.location, args.branch)
+        return deploy_command_wrapper(args.pipeline_script_path, args.deployment_method, args.schedule, args.run_on_push, args.run_manually, args.branch)
     elif args.command == "telemetry":
         return telemetry_status_command_wrapper()
     else:
         print_help(parser)
         return -1
```

### Comparing `dlt-0.2.9/dlt/cli/config_toml_writer.py` & `dlt-0.2.9a0/dlt/cli/config_toml_writer.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,16 +59,17 @@
     if name in toml_table and not overwrite_existing:
         return
     # do not dump final fields
     if is_final_type(hint) or is_optional_type(hint):
         return
     # get the inner hint to generate cool examples
     hint = extract_inner_hint(hint)
+
     if is_base_configuration_inner_hint(hint):
-        inner_table = tomlkit.table(is_super_table=True)
+        inner_table = tomlkit.table(False)
         write_spec(inner_table, hint(), overwrite_existing)
         if len(inner_table) > 0:
             toml_table[name] = inner_table
     else:
         if default_value is None:
             example_value = generate_typed_example(name, hint)
             toml_table[name] = example_value
@@ -88,14 +89,14 @@
 
 
 def write_values(toml: TOMLContainer, values: Iterable[WritableConfigValue], overwrite_existing: bool) -> None:
     for value in values:
         toml_table: TOMLTable = toml  # type: ignore
         for section in value.sections:
             if section not in toml_table:
-                inner_table = tomlkit.table(is_super_table=True)
+                inner_table = tomlkit.table(True)
                 toml_table[section] = inner_table
                 toml_table = inner_table
             else:
                 toml_table = toml_table[section]  # type: ignore
 
         write_value(toml_table, value.name, value.hint, overwrite_existing, default_value=value.default_value, is_default_of_interest=True)
```

### Comparing `dlt-0.2.9/dlt/cli/deploy_command.py` & `dlt-0.2.9a0/dlt/cli/deploy_command.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,277 +1,308 @@
+from itertools import chain
 import os
-from typing import Optional, Any
+import re
+from typing import List
+from astunparse import unparse
 import yaml
-from enum import Enum
-from importlib.metadata import version as pkg_version
+from yaml import Dumper
+import cron_descriptor
+# import pkg_resources
+import pipdeptree
 
-from dlt.common.configuration.providers import SECRETS_TOML
+import dlt
+
+from dlt.common.configuration.exceptions import LookupTrace
+from dlt.common.configuration.providers import ConfigTomlProvider, EnvironProvider, SECRETS_TOML
 from dlt.common.configuration.paths import make_dlt_settings_path
 from dlt.common.configuration.utils import serialize_value
-from dlt.common.git import is_dirty
+from dlt.common.git import get_origin, get_repo, is_dirty
+from dlt.common.configuration.specs.run_configuration import get_default_pipeline_name
+from dlt.common.reflection.utils import evaluate_node_literal
+from dlt.common.pipeline import LoadInfo
+from dlt.common.storages import FileStorage
+from dlt.common.typing import StrAny
+from dlt.common.utils import set_working_dir
+
+from dlt.reflection import names as n
 
 from dlt.cli import utils
 from dlt.cli import echo as fmt
-from dlt.cli.deploy_command_helpers import (BaseDeployment, ask_files_overwrite, generate_pip_freeze, github_origin_to_url, serialize_templated_yaml,
-                                            wrap_template_str, PipelineWasNotRun)
-
-from dlt.version import DLT_PKG_NAME
+from dlt.cli.exceptions import CliCommandException
 
-from dlt.common.destination.reference import DestinationReference
 
 REQUIREMENTS_GITHUB_ACTION = "requirements_github_action.txt"
+GITHUB_URL = "https://github.com/"
 DLT_DEPLOY_DOCS_URL = "https://dlthub.com/docs/walkthroughs/deploy-a-pipeline"
-DLT_AIRFLOW_GCP_DOCS_URL = "https://dlthub.com/docs/running-in-production/orchestrators/airflow-gcp-cloud-composer"
-AIRFLOW_GETTING_STARTED = "https://airflow.apache.org/docs/apache-airflow/stable/start.html"
-AIRFLOW_DAG_TEMPLATE_SCRIPT = "dag_template.py"
-AIRFLOW_CLOUDBUILD_YAML = "cloudbuild.yaml"
-COMMAND_REPO_LOCATION = "https://github.com/dlt-hub/dlt-%s-template.git"
-COMMAND_DEPLOY_REPO_LOCATION = COMMAND_REPO_LOCATION % "deploy"
-
-
-class DeploymentMethods(Enum):
-    github_actions = "github-action"
-    airflow_composer = "airflow-composer"
-
-
-def deploy_command(
-    pipeline_script_path: str,
-    deployment_method: str,
-    schedule: Optional[str],
-    run_on_push: bool,
-    run_on_dispatch: bool,
-    repo_location: str,
-    branch: Optional[str] = None,
-) -> None:
+
+
+def deploy_command(pipeline_script_path: str, deployment_method: str, schedule: str, run_on_push: bool, run_on_dispatch: bool, branch: str = None) -> None:
     # get current repo local folder
-    deployment_obj: BaseDeployment = None
-    if deployment_method == DeploymentMethods.github_actions.value:
-        deployment_obj = GithubActionDeployment(
-            pipeline_script_path=pipeline_script_path,
-            schedule=schedule,
-            run_on_push=run_on_push,
-            run_on_dispatch=run_on_dispatch,
-            repo_location=repo_location,
-            branch=branch
-        )
-    elif deployment_method == DeploymentMethods.airflow_composer.value:
-        deployment_obj = AirflowDeployment(
-            pipeline_script_path=pipeline_script_path,
-            schedule=schedule,
-            run_on_push=run_on_push,
-            run_on_dispatch=run_on_dispatch,
-            repo_location=repo_location,
-            branch=branch
-        )
-    else:
-        raise ValueError(f"Deployment method '{deployment_method}' is not supported. Only {', '.join([m.value for m in DeploymentMethods])} are available.'")
-
-    deployment_obj.run_deployment()
-
-
-class GithubActionDeployment(BaseDeployment):
-    def _generate_workflow(self, *args: Optional[Any]) -> None:
-        self.deployment_method = DeploymentMethods.github_actions.value
-        if self.schedule_description is None:
-            raise ValueError(
-                f"Setting 'schedule' for '{self.deployment_method}' is required! Use deploy command as 'dlt deploy chess.py {self.deployment_method} --schedule \"*/30 * * * *\"'."
-            )
-        workflow = self._create_new_workflow()
-        serialized_workflow = serialize_templated_yaml(workflow)
-        serialized_workflow_name = f"run_{self.state['pipeline_name']}_workflow.yml"
-        self.artifacts['serialized_workflow'] = serialized_workflow
-        self.artifacts['serialized_workflow_name'] = serialized_workflow_name
+    with get_repo(pipeline_script_path) as repo:
+        repo_storage = FileStorage(str(repo.working_dir))
 
-        # pip freeze special requirements file
-        with self.template_storage.open_file(os.path.join(self.deployment_method, "requirements_blacklist.txt")) as f:
-            requirements_blacklist = f.readlines()
-        requirements_txt = generate_pip_freeze(requirements_blacklist, REQUIREMENTS_GITHUB_ACTION)
-        requirements_txt_name = REQUIREMENTS_GITHUB_ACTION
-        # if repo_storage.has_file(utils.REQUIREMENTS_TXT):
-        self.artifacts['requirements_txt'] = requirements_txt
-        self.artifacts['requirements_txt_name'] = requirements_txt_name
+        # check origin
+        try:
+            origin = get_origin(repo)
+            if "github.com" not in origin:
+                raise CliCommandException("deploy", f"Your current repository origin is not set to github but to {origin}.\nYou must change it to be able to run the pipelines with github actions: https://docs.github.com/en/get-started/getting-started-with-git/managing-remote-repositories")
+        except ValueError:
+            raise CliCommandException("deploy", "Your current repository has no origin set. Please set it up to be able to run the pipelines with github actions: https://docs.github.com/en/get-started/importing-your-projects-to-github/importing-source-code-to-github/adding-locally-hosted-code-to-github")
+
+        # convert to path relative to repo
+        repo_pipeline_script_path = repo_storage.from_wd_to_relative_path(pipeline_script_path)
+        # load pipeline script and extract full_refresh and pipelines_dir args
+        pipeline_script = repo_storage.load(repo_pipeline_script_path)
+        visitor = utils.parse_init_script("deploy", pipeline_script, pipeline_script_path)
+        if n.RUN not in visitor.known_calls:
+            raise CliCommandException("deploy", f"The pipeline script {pipeline_script_path} does not seem to run the pipeline.")
+        # full_refresh = False
+        pipelines_dir: str = None
+        pipeline_name: str = None
+
+        if n.PIPELINE in visitor.known_calls:
+            for call_args in visitor.known_calls[n.PIPELINE]:
+                f_r_node = call_args.arguments.get("full_refresh")
+                if f_r_node:
+                    f_r_value = evaluate_node_literal(f_r_node)
+                    if f_r_value is None:
+                        fmt.warning(f"The value of `full_refresh` in call to `dlt.pipeline` cannot be determined from {unparse(f_r_node).strip()}. We assume that you know what you are doing :)")
+                    if f_r_value is True:
+                        if fmt.confirm("The value of 'full_refresh' is set to True. Do you want to abort to set it to False?", default=True):
+                            return
+                p_d_node = call_args.arguments.get("pipelines_dir")
+                if p_d_node:
+                    pipelines_dir = evaluate_node_literal(p_d_node)
+                    if pipelines_dir is None:
+                        raise CliCommandException("deploy", f"The value of 'pipelines_dir' argument in call to `dlt_pipeline` cannot be determined from {unparse(p_d_node).strip()}. Pipeline working dir will be found. Pass it directly with --pipelines-dir option.")
+                p_n_node = call_args.arguments.get("pipeline_name")
+                if p_n_node:
+                    pipeline_name = evaluate_node_literal(p_n_node)
+                    if pipeline_name is None:
+                        raise CliCommandException("deploy", f"The value of 'pipeline_name' argument in call to `dlt_pipeline` cannot be determined from {unparse(p_d_node).strip()}. Pipeline working dir will be found. Pass it directly with --pipeline-name option.")
+
+        if pipelines_dir:
+            pipelines_dir = os.path.abspath(pipelines_dir)
+
+        # change the working dir to the script working dir
+        with set_working_dir(os.path.split(pipeline_script_path)[0]):
+            # use script name to derive pipeline name
+            if not pipeline_name:
+                pipeline_name = dlt.config.get("pipeline_name")
+                if not pipeline_name:
+                    pipeline_name = get_default_pipeline_name(pipeline_script_path)
+                    fmt.warning(f"Using default pipeline name {pipeline_name}. The pipeline name is not passed as argument to dlt.pipeline nor configured via config provides ie. config.toml")
+            # attach to pipeline name, get state and trace
+            pipeline = dlt.attach(pipeline_name=pipeline_name, pipelines_dir=pipelines_dir)
+            # trace must exist and end with successful loading step
+            trace = pipeline.last_trace
+            if trace is None or len(trace.steps) == 0:
+                raise PipelineWasNotRun("Pipeline run trace could not be found. Please run the pipeline at least once locally.")
+            last_step = trace.steps[-1]
+            if last_step.step_exception is not None:
+                raise PipelineWasNotRun(f"The last pipeline run ended with error. Please make sure that pipeline runs correctly before deployment.\n{last_step.step_exception}")
+            if not isinstance(last_step.step_info, LoadInfo):
+                raise PipelineWasNotRun("The last pipeline run did not reach the load step. Please run the pipeline locally until it loads data into destination.")
+            # add destination name and dataset name to env
+            state = pipeline.state
+            config_prov = ConfigTomlProvider()
+            env_prov= EnvironProvider()
+            envs: List[LookupTrace] = [
+                # LookupTrace(env_prov.name, (), "destination_name", state["destination"]),
+                LookupTrace(env_prov.name, (), "dataset_name", state["dataset_name"])
+            ]
+            secret_envs: List[LookupTrace] = []
+            for resolved_value in trace.resolved_config_values:
+                if resolved_value.is_secret_hint:
+                    # generate special forms for all secrets
+                    secret_envs.append(LookupTrace(env_prov.name, tuple(resolved_value.sections), resolved_value.key, resolved_value.value))
+                    # fmt.echo(f"{resolved_value.key}:{resolved_value.value}{type(resolved_value.value)} in {resolved_value.sections} is SECRET")
+                else:
+                    # move all config values that are not in config.toml into env
+                    if resolved_value.provider_name != config_prov.name:
+                        envs.append(LookupTrace(env_prov.name, tuple(resolved_value.sections), resolved_value.key, resolved_value.value))
+                        # fmt.echo(f"{resolved_value.key} in {resolved_value.sections} moved to CONFIG")
 
-    def _make_modification(self) -> None:
-        if not self.repo_storage.has_folder(utils.GITHUB_WORKFLOWS_DIR):
-            self.repo_storage.create_folder(utils.GITHUB_WORKFLOWS_DIR)
-
-        self.repo_storage.save(
-            os.path.join(utils.GITHUB_WORKFLOWS_DIR, self.artifacts["serialized_workflow_name"]),
-            self.artifacts["serialized_workflow"]
-        )
-        self.repo_storage.save(self.artifacts["requirements_txt_name"], self.artifacts["requirements_txt"])
+        # validate schedule
+        schedule_description = cron_descriptor.get_description(schedule)
 
-    def _create_new_workflow(self) -> Any:
-        with self.template_storage.open_file(os.path.join(self.deployment_method, "run_pipeline_workflow.yml")) as f:
+        template_storage = utils.clone_command_repo("deploy", branch)
+        # template_storage = FileStorage("/home/rudolfix/src/python-dlt-deploy-template")
+
+        # load workload yaml
+        with template_storage.open_file(os.path.join(deployment_method, "run_pipeline_workflow.yml")) as f:
             workflow = yaml.safe_load(f)
         # customize the workflow
-        workflow["name"] = f"Run {self.state['pipeline_name']} pipeline from {self.pipeline_script_path}"
-        if self.run_on_push is False:
+        workflow["name"] = f"Run {state['pipeline_name']} pipeline from {pipeline_script_path}"
+        if run_on_push is False:
             del workflow["on"]["push"]
-        if self.run_on_dispatch is False:
+        if run_on_dispatch is False:
             del workflow["on"]["workflow_dispatch"]
-        workflow["on"]["schedule"] = [{"cron": self.schedule}]
+        workflow["on"]["schedule"] = [{"cron": schedule}]
         workflow["env"] = {}
-        for env_var in self.envs:
-            env_key = self.env_prov.get_key_name(env_var.key, *env_var.sections)
+        for env_var in envs:
+            env_key = env_prov.get_key_name(env_var.key, *env_var.sections)
             # print(serialize_value(env_var.value))
             workflow["env"][env_key] = str(serialize_value(env_var.value))
-        for secret_var in self.secret_envs:
-            env_key = self.env_prov.get_key_name(secret_var.key, *secret_var.sections)
+        for secret_var in secret_envs:
+            env_key = env_prov.get_key_name(secret_var.key, *secret_var.sections)
             workflow["env"][env_key] = wrap_template_str("secrets.%s") % env_key
 
         # run the correct script at the end
         last_workflow_step = workflow["jobs"]["run_pipeline"]["steps"][-1]
         assert last_workflow_step["run"] == "python pipeline.py"
         # must run in the directory of the script
-        wf_run_path, wf_run_name = os.path.split(self.repo_pipeline_script_path)
+        wf_run_path, wf_run_name = os.path.split(repo_pipeline_script_path)
         if wf_run_path:
             run_cd_cmd = f"cd '{wf_run_path}' && "
         else:
             run_cd_cmd = ""
         last_workflow_step["run"] = f"{run_cd_cmd}python '{wf_run_name}'"
+        serialized_workflow = serialize_templated_yaml(workflow)
+        serialized_workflow_name = f"run_{state['pipeline_name']}_workflow.yml"
 
-        return workflow
+        # pip freeze special requirements file
+        with template_storage.open_file(os.path.join(deployment_method, "requirements_blacklist.txt")) as f:
+            requirements_blacklist = f.readlines()
+        requirements_txt = generate_pip_freeze(requirements_blacklist)
+        requirements_txt_name = REQUIREMENTS_GITHUB_ACTION
 
-    def _echo_instructions(self, *args: Optional[Any]) -> None:
+        # if repo_storage.has_file(utils.REQUIREMENTS_TXT):
         fmt.echo("Your %s deployment for pipeline %s in script %s is ready!" % (
-            fmt.bold(self.deployment_method), fmt.bold(self.state["pipeline_name"]), fmt.bold(self.pipeline_script_path)
+            fmt.bold(deployment_method), fmt.bold(state["pipeline_name"]), fmt.bold(pipeline_script_path)
         ))
         #  It contains all relevant configurations and references to credentials that are needed to run the pipeline
         fmt.echo("* A github workflow file %s was created in %s." % (
-            fmt.bold(self.artifacts["serialized_workflow_name"]), fmt.bold(utils.GITHUB_WORKFLOWS_DIR)
+            fmt.bold(serialized_workflow_name), fmt.bold(utils.GITHUB_WORKFLOWS_DIR)
         ))
         fmt.echo("* The schedule with which the pipeline is run is: %s.%s%s" % (
-            fmt.bold(self.schedule_description),
-            " You can also run the pipeline manually." if self.run_on_dispatch else "",
-            " Pipeline will also run on each push to the repository." if self.run_on_push else "",
+            fmt.bold(schedule_description),
+            " You can also run the pipeline manually." if run_on_dispatch else "",
+            " Pipeline will also run on each push to the repository." if run_on_push else "",
         ))
-        fmt.echo(
-            "* The dependencies that will be used to run the pipeline are stored in %s. If you change add more dependencies, remember to refresh your deployment by running the same 'deploy' command again." % fmt.bold(
-                self.artifacts['requirements_txt_name'])
-        )
+        fmt.echo("* The dependencies that will be used to run the pipeline are stored in %s. If you change add more dependencies, remember to refresh your deployment by running the same 'deploy' command again." % fmt.bold(requirements_txt_name))
         fmt.echo()
-        if len(self.secret_envs) == 0 and len(self.envs) == 0:
-            fmt.echo("1. Your pipeline does not seem to need any secrets.")
-        else:
-            fmt.echo("You should now add the secrets to github repository secrets, commit and push the pipeline files to github.")
-            fmt.echo("1. Add the following secret values (typically stored in %s): \n%s\nin %s" % (
-                fmt.bold(make_dlt_settings_path(SECRETS_TOML)),
-                fmt.bold("\n".join(self.env_prov.get_key_name(s_v.key, *s_v.sections) for s_v in self.secret_envs)),
-                fmt.bold(github_origin_to_url(self.origin, "/settings/secrets/actions"))
-            ))
+        fmt.echo("You should now add the secrets to github repository secrets, commit and push the pipeline files to github.")
+        fmt.echo("1. Add the following secret values (typically stored in %s): \n%s\nin %s" % (
+            fmt.bold(make_dlt_settings_path(SECRETS_TOML)),
+            fmt.bold("\n".join(env_prov.get_key_name(s_v.key, *s_v.sections) for s_v in secret_envs)),
+            fmt.bold(github_origin_to_url(origin, "/settings/secrets/actions"))
+        ))
+        fmt.echo()
+        # if fmt.confirm("Do you want to list the values of the secrets in the format suitable for github?", default=True):
+        for s_v in secret_envs:
+            fmt.secho("Name:", fg="green")
+            fmt.echo(fmt.bold(env_prov.get_key_name(s_v.key, *s_v.sections)))
+            fmt.secho("Secret:", fg="green")
+            fmt.echo(s_v.value)
             fmt.echo()
-            self._echo_secrets()
 
         fmt.echo("2. Add stage deployment files to commit. Use your Git UI or the following command")
-        new_req_path = self.repo_storage.from_relative_path_to_wd(self.artifacts['requirements_txt_name'])
-        new_workflow_path = self.repo_storage.from_relative_path_to_wd(os.path.join(utils.GITHUB_WORKFLOWS_DIR, self.artifacts['serialized_workflow_name']))
-        fmt.echo(fmt.bold(
-            f"git add {new_req_path} {new_workflow_path}"))
+        fmt.echo(fmt.bold(f"git add {repo_storage.from_relative_path_to_wd(requirements_txt_name)} {repo_storage.from_relative_path_to_wd(os.path.join(utils.GITHUB_WORKFLOWS_DIR, serialized_workflow_name))}"))
         fmt.echo()
         fmt.echo("3. Commit the files above. Use your Git UI or the following command")
-        fmt.echo(fmt.bold(f"git commit -m 'run {self.state['pipeline_name']} pipeline with github action'"))
-        if is_dirty(self.repo):
+        fmt.echo(fmt.bold(f"git commit -m 'run {state['pipeline_name']} pipeline with github action'"))
+        if is_dirty(repo):
             fmt.warning("You have modified files in your repository. Do not forget to push changes to your pipeline script as well!")
         fmt.echo()
         fmt.echo("4. Push changes to github. Use your Git UI or the following command")
         fmt.echo(fmt.bold("git push origin"))
         fmt.echo()
         fmt.echo("5. Your pipeline should be running! You can monitor it here:")
-        fmt.echo(fmt.bold(github_origin_to_url(self.origin, f"/actions/workflows/{self.artifacts['serialized_workflow_name']}")))
+        fmt.echo(fmt.bold(github_origin_to_url(origin, f"/actions/workflows/{serialized_workflow_name}")))
 
+        if not repo_storage.has_folder(utils.GITHUB_WORKFLOWS_DIR):
+            repo_storage.create_folder(utils.GITHUB_WORKFLOWS_DIR)
 
-class AirflowDeployment(BaseDeployment):
-    def _generate_workflow(self, *args: Optional[Any]) -> None:
-        self.deployment_method = DeploymentMethods.airflow_composer.value
+        repo_storage.save(os.path.join(utils.GITHUB_WORKFLOWS_DIR, serialized_workflow_name), serialized_workflow)
+        repo_storage.save(requirements_txt_name, requirements_txt)
 
-        req_dep = f"{DLT_PKG_NAME}[{DestinationReference.to_name(self.state['destination'])}]"
-        req_dep_line = f"{req_dep}>={pkg_version(DLT_PKG_NAME)}"
 
-        self.artifacts["requirements_txt"] = req_dep_line
-
-        dag_script_name = f"dag_{self.state['pipeline_name']}.py"
-        self.artifacts["dag_script_name"] = dag_script_name
-
-        cloudbuild_file = self.template_storage.load(os.path.join(self.deployment_method, AIRFLOW_CLOUDBUILD_YAML))
-        self.artifacts["cloudbuild_file"] = cloudbuild_file
-
-        # TODO: rewrite dag file to at least set the schedule
-        dag_file = self.template_storage.load(os.path.join(self.deployment_method, AIRFLOW_DAG_TEMPLATE_SCRIPT))
-        self.artifacts["dag_file"] = dag_file
-
-        # ask user if to overwrite the files
-        dest_cloud_build = os.path.join(utils.AIRFLOW_BUILD_FOLDER, AIRFLOW_CLOUDBUILD_YAML)
-        dest_dag_script = os.path.join(utils.AIRFLOW_DAGS_FOLDER, dag_script_name)
-        ask_files_overwrite([dest_cloud_build, dest_dag_script])
-
-    def _make_modification(self) -> None:
-        if not self.repo_storage.has_folder(utils.AIRFLOW_DAGS_FOLDER):
-            self.repo_storage.create_folder(utils.AIRFLOW_DAGS_FOLDER)
-
-        if not self.repo_storage.has_folder(utils.AIRFLOW_BUILD_FOLDER):
-            self.repo_storage.create_folder(utils.AIRFLOW_BUILD_FOLDER)
-
-        self.repo_storage.save(
-            os.path.join(utils.AIRFLOW_BUILD_FOLDER, AIRFLOW_CLOUDBUILD_YAML),
-            self.artifacts["cloudbuild_file"]
-        )
-        self.repo_storage.save(
-            os.path.join(utils.AIRFLOW_DAGS_FOLDER, self.artifacts["dag_script_name"]),
-            self.artifacts["dag_file"]
-        )
-
-    def _echo_instructions(self, *args: Optional[Any]) -> None:
-        fmt.echo("Your %s deployment for pipeline %s is ready!" % (
-            fmt.bold(self.deployment_method), fmt.bold(self.state["pipeline_name"]),
-        ))
-        fmt.echo("* The airflow %s file was created in %s." % (
-            fmt.bold(AIRFLOW_CLOUDBUILD_YAML), fmt.bold(utils.AIRFLOW_BUILD_FOLDER)
-        ))
-        fmt.echo("* The %s script was created in %s." % (
-            fmt.bold(self.artifacts["dag_script_name"]), fmt.bold(utils.AIRFLOW_DAGS_FOLDER)
-        ))
+class PipelineWasNotRun(CliCommandException):
+    def __init__(self, msg: str) -> None:
+        super().__init__("deploy", msg, None)
+
+
+def str_representer(dumper: yaml.Dumper, data: str) -> yaml.ScalarNode:
+    # format multiline strings as blocks with the exception of placeholders
+    # that will be expanded as yaml
+    if len(data.splitlines()) > 1 and "{{ toYaml" not in data:  # check for multiline string
+        return dumper.represent_scalar('tag:yaml.org,2002:str', data, style='|')
+    return dumper.represent_scalar('tag:yaml.org,2002:str', data)
+
+
+def wrap_template_str(s: str) -> str:
+    return "${{ %s }}" % s
+
+
+def serialize_templated_yaml(tree: StrAny) -> str:
+    old_representer = Dumper.yaml_representers[str]
+    try:
+        yaml.add_representer(str, str_representer)
+        # pretty serialize yaml
+        serialized: str = yaml.dump(tree, allow_unicode=True, default_flow_style=False, sort_keys=False)
+        # removes apostrophes around the template
+        serialized = re.sub(r"'([\s\n]*?\${{.+?}})'",
+                            r"\1",
+                            serialized,
+                            flags=re.DOTALL)
+        # print(serialized)
+        # fix the new lines in templates ending }}
+        serialized = re.sub(r"(\${{.+)\n.+(}})",
+                            r"\1 \2",
+                            serialized)
+        return serialized
+    finally:
+        yaml.add_representer(str, old_representer)
+
+
+def generate_pip_freeze(requirements_blacklist: List[str]) -> str:
+
+    pkgs = pipdeptree.get_installed_distributions(local_only=True, user_only=False)
+
+    # construct graph with all packages
+    tree = pipdeptree.PackageDAG.from_pkgs(pkgs)
+    nodes = tree.keys()
+    branch_keys = {r.key for r in chain.from_iterable(tree.values())}
+    # all the top level packages
+    nodes = [p for p in nodes if p.key not in branch_keys]
+
+    # compute excludes to compute includes as set difference
+    excludes = set(req.strip() for req in requirements_blacklist if not req.strip().startswith("#"))
+    includes = [node.project_name for node in nodes if node.project_name not in excludes]
+
+    # prepare new filtered DAG
+    tree = tree.sort()
+    tree = tree.filter(includes, None)
+    nodes = tree.keys()
+    branch_keys = {r.key for r in chain.from_iterable(tree.values())}
+    nodes = [p for p in nodes if p.key not in branch_keys]
+
+    # detect and warn on conflict
+    conflicts = pipdeptree.conflicting_deps(tree)
+    cycles = pipdeptree.cyclic_deps(tree)
+    if conflicts:
+        fmt.warning(f"Unable to create dependencies for the github action. Please edit {REQUIREMENTS_GITHUB_ACTION} yourself")
+        pipdeptree.render_conflicts_text(conflicts)
+        pipdeptree.render_cycles_text(cycles)
         fmt.echo()
+        # do not create package because it will most probably fail
+        return "# please provide valid dependencies including dlt package"
 
-        fmt.echo("You must prepare your repository first:")
+    lines = [node.render(None, False) for node in nodes]
+    return "\n".join(lines)
 
-        fmt.echo("1. Import your sources in %s, change default_args if necessary." % (fmt.bold(self.artifacts["dag_script_name"])))
-        fmt.echo("2. Run airflow pipeline locally.\nSee Airflow getting started: %s" % (fmt.bold(AIRFLOW_GETTING_STARTED)))
-        fmt.echo()
 
-        fmt.echo("If you are planning run the pipeline with Google Cloud Composer, follow the next instructions:\n")
-        fmt.echo("1. Read this doc and set up the Environment: %s" % (
-            fmt.bold(DLT_AIRFLOW_GCP_DOCS_URL)
-        ))
-        fmt.echo("2. Set _BUCKET_NAME up in %s/%s file. " % (
-            fmt.bold(utils.AIRFLOW_BUILD_FOLDER), fmt.bold(AIRFLOW_CLOUDBUILD_YAML),
-        ))
-        if len(self.secret_envs) == 0 and len(self.envs) == 0:
-            fmt.echo("3. Your pipeline does not seem to need any secrets.")
-        else:
-            fmt.echo("3. Add the following secret values (typically stored in %s): \n%s\n%s\nin ENVIRONMENT VARIABLES using Google Composer UI" % (
-                fmt.bold(make_dlt_settings_path(SECRETS_TOML)),
-                fmt.bold("\n".join(self.env_prov.get_key_name(s_v.key, *s_v.sections) for s_v in self.secret_envs)),
-                fmt.bold("\n".join(self.env_prov.get_key_name(v.key, *v.sections) for v in self.envs)),
-            ))
-            fmt.echo()
-            # if fmt.confirm("Do you want to list the environment variables in the format suitable for Airflow?", default=True):
-            self._echo_secrets()
-            self._echo_envs()
-
-        fmt.echo("4. Add dlt package below using Google Composer UI.")
-        fmt.echo(fmt.bold(self.artifacts["requirements_txt"]))
-        fmt.note("You may need to add more packages ie. when your source requires additional dependencies")
-        fmt.echo("5. Commit and push the pipeline files to github:")
-        fmt.echo("a. Add stage deployment files to commit. Use your Git UI or the following command")
-
-        dag_script_path = self.repo_storage.from_relative_path_to_wd(os.path.join(utils.AIRFLOW_DAGS_FOLDER, self.artifacts["dag_script_name"]))
-        cloudbuild_path = self.repo_storage.from_relative_path_to_wd(os.path.join(utils.AIRFLOW_BUILD_FOLDER, AIRFLOW_CLOUDBUILD_YAML))
-        fmt.echo(fmt.bold(f"git add {dag_script_path} {cloudbuild_path}"))
-
-        fmt.echo("b. Commit the files above. Use your Git UI or the following command")
-        fmt.echo(fmt.bold(f"git commit -m 'initiate {self.state['pipeline_name']} pipeline with Airflow'"))
-        if is_dirty(self.repo):
-            fmt.warning("You have modified files in your repository. Do not forget to push changes to your pipeline script as well!")
-        fmt.echo("c. Push changes to github. Use your Git UI or the following command")
-        fmt.echo(fmt.bold("git push origin"))
-        fmt.echo("6. You should see your pipeline in Airflow.")
+def github_origin_to_url(origin: str, path: str) -> str:
+    # repository origin must end with .git
+    if origin.endswith(".git"):
+        origin = origin[:-4]
+    if origin.startswith("git@github.com:"):
+        origin = origin[15:]
+
+    if not origin.startswith(GITHUB_URL):
+        origin = GITHUB_URL + origin
+    #https://github.com/dlt-hub/data-loading-zoomcamp.git
+    #git@github.com:dlt-hub/data-loading-zoomcamp.git
+
+    # https://github.com/dlt-hub/data-loading-zoomcamp/settings/secrets/actions
+    return origin + path
```

### Comparing `dlt-0.2.9/dlt/cli/echo.py` & `dlt-0.2.9a0/dlt/cli/echo.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/cli/init_command.py` & `dlt-0.2.9a0/dlt/cli/init_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from dlt.common.configuration.paths import get_dlt_settings_dir, make_dlt_settings_path
 from dlt.common.configuration.specs import known_sections
 from dlt.common.configuration.providers import CONFIG_TOML, SECRETS_TOML, ConfigTomlProvider, SecretsTomlProvider
 from dlt.common.normalizers import default_normalizers, import_normalizers
 from dlt.common.pipeline import get_dlt_repos_dir
 from dlt.common.source import _SOURCES
 from dlt.version import DLT_PKG_NAME, __version__
-from dlt.common.destination import DestinationReference
+from dlt.common.destination.reference import DestinationReference
 from dlt.common.reflection.utils import rewrite_python_script
 from dlt.common.schema.exceptions import InvalidSchemaName
 from dlt.common.storages.file_storage import FileStorage
 
 import dlt.reflection.names as n
 from dlt.reflection.script_inspector import inspect_pipeline_script, load_script_module
 
@@ -274,15 +274,16 @@
         # for verified pipelines place in the specific source section
         required_secrets, required_config, checked_sources = source_detection.detect_source_configs(_SOURCES, pipeline_name, (known_sections.SOURCES, pipeline_name))
 
     if len(checked_sources) == 0:
         raise CliCommandException("init", f"The pipeline script {pipeline_files.pipeline_script} is not creating or importing any sources or resources")
 
     # add destination spec to required secrets
-    required_secrets["destinations:" + destination_name] = WritableConfigValue(destination_name, destination_spec, None, ("destination",))
+    credentials_type = destination_spec().get_resolvable_fields()["credentials"]
+    required_secrets["destinations:" + destination_name] = WritableConfigValue("credentials", credentials_type, None, ("destination", destination_name))
     # add the global telemetry to required config
     required_config["runtime.dlthub_telemetry"] = WritableConfigValue("dlthub_telemetry", bool, utils.get_telemetry_status(), ("runtime", ))
 
     # modify the script
     script_lines = rewrite_python_script(visitor.source_lines, transformed_nodes)
     dest_script_source = "".join(script_lines)
     # validate by parsing
```

### Comparing `dlt-0.2.9/dlt/cli/pipeline_command.py` & `dlt-0.2.9a0/dlt/cli/pipeline_command.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,19 +52,19 @@
         if operation == "sync":
             return  # No need to sync again
 
     fmt.echo("Found pipeline %s in %s" % (fmt.bold(p.pipeline_name), fmt.bold(p.pipelines_dir)))
 
     if operation == "show":
         from dlt.common.runtime import signals
-        from dlt.helpers import streamlit_helper
+        from dlt.helpers import streamlit
 
         with signals.delayed_signals():
             venv = Venv.restore_current()
-            for line in iter_stdout(venv, "streamlit", "run", streamlit_helper.__file__, pipeline_name):
+            for line in iter_stdout(venv, "streamlit", "run", streamlit.__file__, pipeline_name):
                 fmt.echo(line)
 
     if operation == "info":
         state: TSourceState = p.state  # type: ignore
         fmt.echo("Synchronized state:")
         for k, v in state.items():
             if not isinstance(v, dict):
```

### Comparing `dlt-0.2.9/dlt/cli/pipeline_files.py` & `dlt-0.2.9a0/dlt/cli/pipeline_files.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/cli/source_detection.py` & `dlt-0.2.9a0/dlt/cli/source_detection.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/cli/telemetry_command.py` & `dlt-0.2.9a0/dlt/cli/telemetry_command.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/cli/utils.py` & `dlt-0.2.9a0/dlt/cli/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,27 +16,26 @@
 from dlt.common.configuration.specs import RunConfiguration
 
 from dlt.reflection.script_visitor import PipelineScriptVisitor
 
 from dlt.cli.exceptions import CliCommandException
 
 
+COMMAND_REPO_LOCATION = "https://github.com/dlt-hub/python-dlt-%s-template.git"
 REQUIREMENTS_TXT = "requirements.txt"
 PYPROJECT_TOML = "pyproject.toml"
 GITHUB_WORKFLOWS_DIR = os.path.join(".github", "workflows")
-AIRFLOW_DAGS_FOLDER = os.path.join("dags")
-AIRFLOW_BUILD_FOLDER = os.path.join("build")
 LOCAL_COMMAND_REPO_FOLDER = "repos"
 MODULE_INIT = "__init__.py"
 
 
-def clone_command_repo(repo_location: str, branch: str) -> FileStorage:
+def clone_command_repo(command: str, branch: str) -> FileStorage:
     template_dir = tempfile.mkdtemp()
     # TODO: handle ImportError (no git command available) gracefully
-    with git.clone_repo(repo_location, template_dir, branch=branch):
+    with git.clone_repo(COMMAND_REPO_LOCATION % command, template_dir, branch=branch):
         return FileStorage(template_dir)
 
 
 def parse_init_script(command: str, script_source: str, init_script_name: str) -> PipelineScriptVisitor:
     # parse the script first
     tree = ast.parse(source=script_source)
     set_ast_parents(tree)
```

### Comparing `dlt-0.2.9/dlt/common/arithmetics.py` & `dlt-0.2.9a0/dlt/common/arithmetics.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/configuration/accessors.py` & `dlt-0.2.9a0/dlt/common/configuration/accessors.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/configuration/container.py` & `dlt-0.2.9a0/dlt/common/configuration/container.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/configuration/exceptions.py` & `dlt-0.2.9a0/dlt/common/configuration/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,18 +10,14 @@
     value: Any
 
 
 class ConfigurationException(DltException, TerminalException):
     pass
 
 
-class ConfigurationValueError(ConfigurationException, ValueError):
-    pass
-
-
 class ContainerException(DltException):
     """base exception for all exceptions related to injectable container"""
     pass
 
 
 class ConfigProviderException(ConfigurationException):
     """base exceptions for all exceptions raised by config providers"""
@@ -48,36 +44,21 @@
             msg += f'\tfor field "{f}" config providers and keys were tried in following order:\n'
             for tr in field_traces:
                 msg += f'\t\tIn {tr.provider} key {tr.key} was not found.\n'
         msg += "Please refer to https://dlthub.com/docs/general-usage/credentials for more information\n"
         return msg
 
 
-class UnmatchedConfigHintResolversException(ConfigurationException):
-    """Raised when using `@resolve_type` on a field that doesn't exist in the spec"""
-    def __init__(self, spec_name: str, field_names: Sequence[str]) -> None:
-        self.field_names = field_names
-        self.spec_name = spec_name
-        example = f">>> class {spec_name}(BaseConfiguration)\n" + "\n".join(f">>>    {name}: Any" for name in field_names)
-        msg = (
-            f"The config spec {spec_name} has dynamic type resolvers for fields: {field_names} "
-            "but these fields are not defined in the spec.\n"
-            "When using @resolve_type() decorator, Add the fields with 'Any' or another common type hint, example:\n"
-            f"\n{example}"
-        )
-        super().__init__(msg)
-
-
 class FinalConfigFieldException(ConfigurationException):
     """rises when field was annotated as final ie Final[str] and the value is modified by config provider"""
     def __init__(self, spec_name: str, field: str) -> None:
         super().__init__(f"Field {field} in spec {spec_name} is final but is being changed by a config provider")
 
 
-class ConfigValueCannotBeCoercedException(ConfigurationValueError):
+class ConfigValueCannotBeCoercedException(ConfigurationException, ValueError):
     """raises when value returned by config provider cannot be coerced to hinted type"""
 
     def __init__(self, field_name: str, field_value: Any, hint: type) -> None:
         self.field_name = field_name
         self.field_value = field_value
         self.hint = hint
         super().__init__('Configured value for field %s cannot be coerced into type %s' % (field_name, str(hint)))
```

### Comparing `dlt-0.2.9/dlt/common/configuration/inject.py` & `dlt-0.2.9a0/dlt/common/configuration/inject.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/configuration/paths.py` & `dlt-0.2.9a0/dlt/common/configuration/paths.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/configuration/providers/airflow.py` & `dlt-0.2.9a0/dlt/common/configuration/providers/airflow.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,36 @@
+import tomlkit
 from airflow.models import Variable
 
-from .toml import VaultTomlProvider
+from .toml import BaseTomlProvider
 
+AIRFLOW_SECRETS_TOML_VARIABLE_KEY = 'dlt_secrets_toml'
 
-class AirflowSecretsTomlProvider(VaultTomlProvider):
-    def __init__(self, only_secrets: bool = False, only_toml_fragments: bool = False) -> None:
-        super().__init__(only_secrets, only_toml_fragments)
+
+class AirflowSecretsTomlProvider(BaseTomlProvider):
+    def __init__(
+        self, variable_key: str = AIRFLOW_SECRETS_TOML_VARIABLE_KEY
+    ) -> None:
+        """Reads TOML configuration data from an Airflow variable specified
+        by the `variable_key` and initializes a BaseTomlProvider with the
+        parsed content.
+
+        Args:
+            variable_key (str, optional): The Airflow variable key to read secrets from.
+                Defaults to AIRFLOW_SECRETS_TOML_VARIABLE_KEY.
+        """
+        toml_content = self._read_toml_from_airflow(variable_key)
+        super().__init__(toml_content)
+
+    def _read_toml_from_airflow(
+        self, variable_key: str
+    ) -> tomlkit.TOMLDocument:
+        toml_string = Variable.get(variable_key)
+        return tomlkit.parse(toml_string)
 
     @property
     def name(self) -> str:
         return 'Airflow Secrets TOML Provider'
 
-    def _look_vault(self, full_key: str, hint: type) -> str:
-        """Get Airflow Variable with given `full_key`, return None if not found"""
-        return Variable.get(full_key, default_var=None)  # type: ignore
-
     @property
     def supports_secrets(self) -> bool:
         return True
```

### Comparing `dlt-0.2.9/dlt/common/configuration/providers/context.py` & `dlt-0.2.9a0/dlt/common/configuration/providers/context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/configuration/providers/dictionary.py` & `dlt-0.2.9a0/dlt/common/configuration/providers/dictionary.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/configuration/providers/environ.py` & `dlt-0.2.9a0/dlt/common/configuration/providers/environ.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/configuration/providers/provider.py` & `dlt-0.2.9a0/dlt/common/configuration/providers/provider.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/configuration/resolve.py` & `dlt-0.2.9a0/dlt/common/configuration/resolve.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 from dlt.common.typing import AnyType, StrAny, TSecretValue, get_all_types_of_class_in_union, is_final_type, is_optional_type, is_union
 
 from dlt.common.configuration.specs.base_configuration import BaseConfiguration, CredentialsConfiguration, is_secret_hint, extract_inner_hint, is_context_inner_hint, is_base_configuration_inner_hint
 from dlt.common.configuration.specs.config_section_context import ConfigSectionContext
 from dlt.common.configuration.container import Container
 from dlt.common.configuration.specs.config_providers_context import ConfigProvidersContext
 from dlt.common.configuration.utils import log_traces, deserialize_value
-from dlt.common.configuration.exceptions import (
-    FinalConfigFieldException, LookupTrace, ConfigFieldMissingException, ConfigurationWrongTypeException,
-    ValueNotSecretException, InvalidNativeValue, UnmatchedConfigHintResolversException)
+from dlt.common.configuration.exceptions import (FinalConfigFieldException, LookupTrace, ConfigFieldMissingException, ConfigurationWrongTypeException, ValueNotSecretException, InvalidNativeValue)
 
 TConfiguration = TypeVar("TConfiguration", bound=BaseConfiguration)
 
 
 def resolve_configuration(config: TConfiguration, *, sections: Tuple[str, ...] = (), explicit_value: Any = None, accept_partial: bool = False) -> TConfiguration:
     if not isinstance(config, BaseConfiguration):
         raise ConfigurationWrongTypeException(type(config))
@@ -115,17 +113,14 @@
         accept_partial: bool
     ) -> None:
 
     fields = config.get_resolvable_fields()
     unresolved_fields: Dict[str, Sequence[LookupTrace]] = {}
 
     for key, hint in fields.items():
-        if key in config.__hint_resolvers__:
-            # Type hint for this field is created dynamically
-            hint = config.__hint_resolvers__[key](config)
         # get default and explicit values
         default_value = getattr(config, key, None)
         traces: List[LookupTrace] = []
 
         if explicit_values:
             explicit_value = explicit_values.get(key)
         else:
@@ -165,23 +160,14 @@
             unresolved_fields[key] = traces
         # set resolved value in config
         if default_value != current_value:
             if is_final_type(hint):
                 raise FinalConfigFieldException(type(config).__name__, key)
             setattr(config, key, current_value)
 
-    # Check for dynamic hint resolvers which have no corresponding fields
-    unmatched_hint_resolvers: List[str] = []
-    for field_name in config.__hint_resolvers__:
-        if field_name not in fields:
-            unmatched_hint_resolvers.append(field_name)
-
-    if unmatched_hint_resolvers:
-        raise UnmatchedConfigHintResolversException(type(config).__name__, unmatched_hint_resolvers)
-
     if unresolved_fields:
         raise ConfigFieldMissingException(type(config).__name__, unresolved_fields)
 
 
 def _resolve_config_field(
         key: str,
         hint: Type[Any],
```

### Comparing `dlt-0.2.9/dlt/common/configuration/specs/__init__.py` & `dlt-0.2.9a0/dlt/common/configuration/specs/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from .run_configuration import RunConfiguration  # noqa: F401
 from .base_configuration import BaseConfiguration, CredentialsConfiguration, CredentialsWithDefault, ContainerInjectableContext, extract_inner_hint, is_base_configuration_inner_hint, configspec  # noqa: F401
 from .config_section_context import ConfigSectionContext  # noqa: F401
 
 from .gcp_credentials import GcpServiceAccountCredentialsWithoutDefaults, GcpServiceAccountCredentials, GcpOAuthCredentialsWithoutDefaults, GcpOAuthCredentials, GcpCredentials  # noqa: F401
 from .connection_string_credentials import ConnectionStringCredentials  # noqa: F401
 from .api_credentials import OAuth2Credentials  # noqa: F401
-from .aws_credentials import AwsCredentials  # noqa: F401
 
 
 # backward compatibility for service account credentials
-from .gcp_credentials import GcpServiceAccountCredentialsWithoutDefaults as GcpClientCredentials, GcpServiceAccountCredentials as GcpClientCredentialsWithDefault  # noqa: F401
+from .gcp_credentials import GcpServiceAccountCredentialsWithoutDefaults as GcpClientCredentials, GcpServiceAccountCredentials as GcpClientCredentialsWithDefault  # noqa: F401
```

### Comparing `dlt-0.2.9/dlt/common/configuration/specs/api_credentials.py` & `dlt-0.2.9a0/dlt/common/configuration/specs/api_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/configuration/specs/base_configuration.py` & `dlt-0.2.9a0/dlt/common/configuration/specs/base_configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import inspect
 import contextlib
 import dataclasses
 from collections.abc import Mapping as C_Mapping
-from typing import Callable, List, Optional, Union, Any, Dict, Iterator, MutableMapping, Type, TYPE_CHECKING, get_args, get_origin, overload, ClassVar, TypeVar
-from functools import wraps
+from typing import Callable, List, Optional, Union, Any, Dict, Iterator, MutableMapping, Type, TYPE_CHECKING, get_args, get_origin, overload, ClassVar
 
 if TYPE_CHECKING:
     TDtcField = dataclasses.Field[Any]
 else:
     TDtcField = dataclasses.Field
 
 from dlt.common.typing import TAnyClass, TSecretValue, extract_inner_type, is_optional_type, is_union
@@ -94,34 +93,29 @@
 
     In comparison the Python dataclass, a spec implements full dictionary interface for its attributes, allows instance creation from ie. strings
     or other types (parsing, deserialization) and control over configuration resolution process. See `BaseConfiguration` and CredentialsConfiguration` for
     more information.
 
     """
     def wrap(cls: Type[TAnyClass]) -> Type[TAnyClass]:
-        cls.__hint_resolvers__ = {}  # type: ignore[attr-defined]
         is_context = issubclass(cls, _F_ContainerInjectableContext)
         # if type does not derive from BaseConfiguration then derive it
         with contextlib.suppress(NameError):
             if not issubclass(cls, BaseConfiguration):
                 # keep the original module
                 fields = {"__module__": cls.__module__, "__annotations__": getattr(cls, "__annotations__", {})}
                 cls = type(cls.__name__, (cls, _F_BaseConfiguration), fields)
         # get all annotations without corresponding attributes and set them to None
         for ann in cls.__annotations__:
             if not hasattr(cls, ann) and not ann.startswith(("__", "_abc_impl")):
                 setattr(cls, ann, None)
         # get all attributes without corresponding annotations
         for att_name, att_value in cls.__dict__.items():
             # skip callables, dunder names, class variables and some special names
-            if callable(att_value):
-                if hint_field_name := getattr(att_value, "__hint_for_field__", None):
-                    cls.__hint_resolvers__[hint_field_name] = att_value  # type: ignore[attr-defined]
-                continue
-            if not att_name.startswith(("__", "_abc_impl")) and not isinstance(att_value, (staticmethod, classmethod, property)):
+            if not callable(att_value) and not att_name.startswith(("__", "_abc_impl")) and not isinstance(att_value, (staticmethod, classmethod, property)):
                 if att_name not in cls.__annotations__:
                     raise ConfigFieldMissingTypeHintException(att_name, cls)
                 hint = cls.__annotations__[att_name]
                 # context can have any type
                 if not is_valid_hint(hint) and not is_context:
                     raise ConfigFieldTypeHintNotSupported(att_name, cls, hint)
         # do not generate repr as it may contain secret values
@@ -130,29 +124,27 @@
     # called with parenthesis
     if cls is None:
         return wrap
 
     return wrap(cls)
 
 
-
 @configspec
 class BaseConfiguration(MutableMapping[str, Any]):
 
     __is_resolved__: bool = dataclasses.field(default = False, init=False, repr=False)
     """True when all config fields were resolved and have a specified value type"""
     __section__: str = dataclasses.field(default = None, init=False, repr=False)
     """Obligatory section used by config providers when searching for keys, always present in the search path"""
     __exception__: Exception = dataclasses.field(default = None, init=False, repr=False)
     """Holds the exception that prevented the full resolution"""
     __config_gen_annotations__: ClassVar[List[str]] = []
     """Additional annotations for config generator, currently holds a list of fields of interest that have defaults"""
     __dataclass_fields__: ClassVar[Dict[str, TDtcField]]
     """Typing for dataclass fields"""
-    __hint_resolvers__: ClassVar[Dict[str, Callable[["BaseConfiguration"], Type[Any]]]] = {}
 
     def parse_native_representation(self, native_value: Any) -> None:
         """Initialize the configuration fields by parsing the `native_value` which should be a native representation of the configuration
         or credentials, for example database connection string or JSON serialized GCP service credentials file.
 
         ### Args:
             native_value (Any): A native representation of the configuration
@@ -173,20 +165,15 @@
             Any: A native representation of the configuration
         """
         raise NotImplementedError()
 
     @classmethod
     def get_resolvable_fields(cls) -> Dict[str, type]:
         """Returns a mapping of fields to their type hints. Dunders should not be resolved and are not returned"""
-        # Sort dynamic type hint fields last because they depend on other values
-        fields = sorted(
-            (f for f in cls.__dataclass_fields__.values() if not f.name.startswith("__")),
-            key=lambda f: f.name in cls.__hint_resolvers__
-        )
-        return {f.name: f.type for f in fields}
+        return {f.name:f.type for f in cls.__dataclass_fields__.values() if not f.name.startswith("__")}
 
     def is_resolved(self) -> bool:
         return self.__is_resolved__
 
     def is_partial(self) -> bool:
         """Returns True when any required resolvable field has its value missing."""
         if self.__is_resolved__:
@@ -318,20 +305,7 @@
 
     def add_extras(self) -> None:
         """Called right after context was added to the container. Benefits mostly the config provider injection context which adds extra providers using the initial ones."""
         pass
 
 
 _F_ContainerInjectableContext = ContainerInjectableContext
-
-
-TSpec = TypeVar("TSpec", bound=BaseConfiguration)
-THintResolver = Callable[[TSpec], Type[Any]]
-
-def resolve_type(field_name: str) -> Callable[[THintResolver[TSpec]], THintResolver[TSpec]]:
-    def decorator(func: THintResolver[TSpec]) -> THintResolver[TSpec]:
-        func.__hint_for_field__ = field_name  # type: ignore[attr-defined]
-        @wraps(func)
-        def wrapper(self: TSpec) -> Type[Any]:
-            return func(self)
-        return wrapper
-    return decorator
```

### Comparing `dlt-0.2.9/dlt/common/configuration/specs/config_providers_context.py` & `dlt-0.2.9a0/dlt/common/configuration/specs/config_providers_context.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,24 +61,20 @@
     def add_provider(self, provider: ConfigProvider) -> None:
         if provider.name in self:
             raise DuplicateConfigProviderException(provider.name)
         self.providers.append(provider)
 
     @staticmethod
     def initial_providers() -> List[ConfigProvider]:
-        return _initial_providers()
-
-
-def _initial_providers() -> List[ConfigProvider]:
-    providers = [
-        EnvironProvider(),
-        SecretsTomlProvider(add_global_config=True),
-        ConfigTomlProvider(add_global_config=True)
-    ]
-    return providers
+        providers = [
+            EnvironProvider(),
+            SecretsTomlProvider(add_global_config=True),
+            ConfigTomlProvider(add_global_config=True)
+        ]
+        return providers
 
 
 def _extra_providers() -> List[ConfigProvider]:
     from dlt.common.configuration.resolve import resolve_configuration
     providers_config = resolve_configuration(ConfigProvidersConfiguration())
     extra_providers = []
     if providers_config.enable_airflow_secrets:
@@ -105,33 +101,40 @@
 
     Depending on how DAG is defined this function may be called outside of task and
     task context will be not available. Still we want the provider to function so
     we just test if Airflow can be imported.
     """
     if not is_airflow_installed():
         return []
-    from dlt.common.configuration.providers.toml import SECRETS_TOML_KEY
 
     # hide stdio. airflow typically dumps tons of warnings and deprecations to stdout and stderr
     with contextlib.redirect_stdout(io.StringIO()), contextlib.redirect_stderr(io.StringIO()):
         from airflow.models import Variable # noqa
-        from dlt.common.configuration.providers.airflow import AirflowSecretsTomlProvider
-
-        secrets_toml_var = Variable.get(SECRETS_TOML_KEY, default_var=None)
 
-    if secrets_toml_var is None:
-        message = f"Airflow variable '{SECRETS_TOML_KEY}' not found. AirflowSecretsTomlProvider will not be used."
+        from dlt.common.configuration.providers.airflow import (
+            AirflowSecretsTomlProvider,
+            AIRFLOW_SECRETS_TOML_VARIABLE_KEY
+        )
+
+        secrets_toml_var = Variable.get(
+            AIRFLOW_SECRETS_TOML_VARIABLE_KEY,
+            default_var=None
+        )
+
+    if secrets_toml_var is not None:
+        return [AirflowSecretsTomlProvider()]
+    else:
+        message = f"Airflow variable '{AIRFLOW_SECRETS_TOML_VARIABLE_KEY}' not found. AirflowSecretsTomlProvider will not be used."
         try:
             # prefer logging to task logger
             from airflow.operators.python import get_current_context  # noqa
 
             ti = get_current_context()["ti"]
             ti.log.warning(message)
         except Exception:
             # otherwise log to dlt logger
             from dlt.common import logger
             if logger.is_logging():
                 logger.warning(message)
             else:
                 print(message)
-
-    return [AirflowSecretsTomlProvider()]
+        return []
```

### Comparing `dlt-0.2.9/dlt/common/configuration/specs/config_section_context.py` & `dlt-0.2.9a0/dlt/common/configuration/specs/config_section_context.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/configuration/specs/connection_string_credentials.py` & `dlt-0.2.9a0/dlt/common/configuration/specs/connection_string_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/configuration/specs/exceptions.py` & `dlt-0.2.9a0/dlt/common/configuration/specs/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/configuration/specs/gcp_credentials.py` & `dlt-0.2.9a0/dlt/common/configuration/specs/gcp_credentials.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/configuration/specs/known_sections.py` & `dlt-0.2.9a0/dlt/common/configuration/specs/known_sections.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/configuration/specs/run_configuration.py` & `dlt-0.2.9a0/dlt/common/configuration/specs/run_configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/configuration/utils.py` & `dlt-0.2.9a0/dlt/common/configuration/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,20 +110,20 @@
     return value
 
 
 
 def log_traces(config: Optional[BaseConfiguration], key: str, hint: Type[Any], value: Any, default_value: Any, traces: Sequence[LookupTrace]) -> None:
     from dlt.common import logger
 
-    # if logger.is_logging() and logger.log_level() == "DEBUG" and config:
-    #     logger.debug(f"Field {key} with type {hint} in {type(config).__name__} {'NOT RESOLVED' if value is None else 'RESOLVED'}")
+    if logger.is_logging() and logger.log_level() == "DEBUG" and config:
+        logger.debug(f"Field {key} with type {hint} in {type(config).__name__} {'NOT RESOLVED' if value is None else 'RESOLVED'}")
         # print(f"Field {key} with type {hint} in {type(config).__name__} {'NOT RESOLVED' if value is None else 'RESOLVED'}")
-        # for tr in traces:
-        #     # print(str(tr))
-        #     logger.debug(str(tr))
+        for tr in traces:
+            # print(str(tr))
+            logger.debug(str(tr))
     # store all traces with resolved values
     resolved_trace = next((trace for trace in traces if trace.value is not None), None)
     if resolved_trace is not None:
         path = f'{".".join(resolved_trace.sections)}.{key}'
         _RESOLVED_TRACES[path] = ResolvedValueTrace(key, resolved_trace.value, default_value, hint, resolved_trace.sections, resolved_trace.provider, config)
```

### Comparing `dlt-0.2.9/dlt/common/data_types/type_helpers.py` & `dlt-0.2.9a0/dlt/common/data_types/type_helpers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/data_writers/buffered.py` & `dlt-0.2.9a0/dlt/common/data_writers/buffered.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/data_writers/escape.py` & `dlt-0.2.9a0/dlt/common/data_writers/escape.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 import base64
 from typing import Any
 from datetime import date, datetime  # noqa: I251
 
-from dlt.common.json import json
+from dlt.common import json
 
 # use regex to escape characters in single pass
 SQL_ESCAPE_DICT = {"'": "''", "\\": "\\\\", "\n": "\\n", "\r": "\\r"}
 SQL_ESCAPE_RE = re.compile("|".join([re.escape(k) for k in sorted(SQL_ESCAPE_DICT, key=len, reverse=True)]), flags=re.DOTALL)
 
 
 def _escape_extended(v: str, prefix:str = "E'") -> str:
```

### Comparing `dlt-0.2.9/dlt/common/data_writers/exceptions.py` & `dlt-0.2.9a0/dlt/common/data_writers/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/data_writers/writers.py` & `dlt-0.2.9a0/dlt/common/data_writers/writers.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/destination/capabilities.py` & `dlt-0.2.9a0/dlt/common/destination/capabilities.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/destination/reference.py` & `dlt-0.2.9a0/dlt/common/destination/reference.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,26 +10,21 @@
 from dlt.common.configuration import configspec
 from dlt.common.configuration.specs import BaseConfiguration, CredentialsConfiguration
 from dlt.common.configuration.accessors import config
 from dlt.common.destination.capabilities import DestinationCapabilitiesContext
 from dlt.common.schema.utils import is_complete_column
 from dlt.common.storages import FileStorage
 from dlt.common.storages.load_storage import ParsedLoadJobFileName
-from dlt.common.utils import get_module_name
 
 
 @configspec(init=True)
 class DestinationClientConfiguration(BaseConfiguration):
     destination_name: str = None  # which destination to load data to
     credentials: Optional[CredentialsConfiguration]
 
-    def __str__(self) -> str:
-        """Return displayable destination location"""
-        return str(self.credentials)
-
     if TYPE_CHECKING:
         def __init__(self, destination_name: str = None, credentials: Optional[CredentialsConfiguration] = None) -> None:
             ...
 
 
 @configspec(init=True)
 class DestinationClientDwhConfiguration(DestinationClientConfiguration):
@@ -141,15 +136,15 @@
         Returns:
             Optional[TSchemaTables]: Returns an update that was applied at the destination.
         """
         self._verify_schema()
         return expected_update
 
     @abstractmethod
-    def start_file_load(self, table: TTableSchema, file_path: str, load_id: str) -> LoadJob:
+    def start_file_load(self, table: TTableSchema, file_path: str) -> LoadJob:
         """Creates a job for a particular `table` with content in `file_path`"""
         pass
 
     @abstractmethod
     def restore_file_load(self, file_path: str) -> LoadJob:
         pass
 
@@ -250,13 +245,7 @@
         try:
             c = destination_ref.spec()
             c.credentials
         except Exception:
             raise InvalidDestinationReference(destination)
 
         return destination_ref
-
-    @staticmethod
-    def to_name(destination: TDestinationReferenceArg) -> str:
-        if isinstance(destination, ModuleType):
-            return get_module_name(destination)
-        return destination.split(".")[-1]  # type: ignore
```

### Comparing `dlt-0.2.9/dlt/common/exceptions.py` & `dlt-0.2.9a0/dlt/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/git.py` & `dlt-0.2.9a0/dlt/common/git.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/json/__init__.py` & `dlt-0.2.9a0/dlt/common/json/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/json/_orjson.py` & `dlt-0.2.9a0/dlt/common/json/_orjson.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/json/_simplejson.py` & `dlt-0.2.9a0/dlt/common/json/_simplejson.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/jsonpath.py` & `dlt-0.2.9a0/dlt/common/jsonpath.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/normalizers/configuration.py` & `dlt-0.2.9a0/dlt/common/normalizers/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/normalizers/json/__init__.py` & `dlt-0.2.9a0/dlt/common/normalizers/json/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/normalizers/json/relational.py` & `dlt-0.2.9a0/dlt/common/normalizers/json/relational.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/normalizers/naming/direct.py` & `dlt-0.2.9a0/dlt/common/normalizers/naming/direct.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/normalizers/naming/duck_case.py` & `dlt-0.2.9a0/dlt/common/normalizers/naming/duck_case.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/normalizers/naming/exceptions.py` & `dlt-0.2.9a0/dlt/common/normalizers/naming/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/normalizers/naming/naming.py` & `dlt-0.2.9a0/dlt/common/normalizers/naming/naming.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/normalizers/naming/snake_case.py` & `dlt-0.2.9a0/dlt/common/normalizers/naming/snake_case.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/normalizers/utils.py` & `dlt-0.2.9a0/dlt/common/normalizers/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/pipeline.py` & `dlt-0.2.9a0/dlt/common/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from dlt.common.configuration import known_sections
 from dlt.common.configuration.container import Container
 from dlt.common.configuration.exceptions import ContextDefaultCannotBeCreated
 from dlt.common.configuration.specs import ContainerInjectableContext
 from dlt.common.configuration.specs.config_section_context import ConfigSectionContext
 from dlt.common.configuration.paths import get_dlt_data_dir
 from dlt.common.configuration.specs import RunConfiguration
-from dlt.common.destination import DestinationReference, TDestinationReferenceArg
+from dlt.common.destination.reference import DestinationReference, TDestinationReferenceArg
 from dlt.common.exceptions import DestinationHasFailedJobs, PipelineStateNotAvailable, ResourceNameNotAvailable, SourceSectionNotAvailable
 from dlt.common.schema import Schema
 from dlt.common.schema.typing import TColumnKey, TColumnSchema, TWriteDisposition
 from dlt.common.source import get_current_pipe_name
 from dlt.common.storages.load_storage import LoadPackageInfo
 from dlt.common.typing import DictStrAny, REPattern
 from dlt.common.jsonpath import delete_matches, TAnyJsonPath
@@ -212,17 +212,14 @@
         """Creates or returns exiting pipeline"""
         if not self._pipeline:
             # delayed pipeline creation
             self.activate(self._deferred_pipeline())
         return self._pipeline
 
     def activate(self, pipeline: SupportsPipeline) -> None:
-        # do not activate currently active pipeline
-        if pipeline == self._pipeline:
-            return
         self.deactivate()
         pipeline._set_context(True)
         self._pipeline = pipeline
 
     def is_active(self) -> bool:
         return self._pipeline is not None
```

### Comparing `dlt-0.2.9/dlt/common/reflection/spec.py` & `dlt-0.2.9a0/dlt/common/reflection/spec.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/reflection/utils.py` & `dlt-0.2.9a0/dlt/common/reflection/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/runners/configuration.py` & `dlt-0.2.9a0/dlt/common/runners/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/runners/pool_runner.py` & `dlt-0.2.9a0/dlt/common/runners/pool_runner.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/runners/runnable.py` & `dlt-0.2.9a0/dlt/common/runners/runnable.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/runners/stdout.py` & `dlt-0.2.9a0/dlt/common/runners/stdout.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/runners/synth_pickle.py` & `dlt-0.2.9a0/dlt/common/runners/synth_pickle.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/runners/venv.py` & `dlt-0.2.9a0/dlt/common/runners/venv.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/runtime/collector.py` & `dlt-0.2.9a0/dlt/common/runtime/collector.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/runtime/exec_info.py` & `dlt-0.2.9a0/dlt/common/runtime/exec_info.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/runtime/init.py` & `dlt-0.2.9a0/dlt/common/runtime/init.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/runtime/logger.py` & `dlt-0.2.9a0/dlt/common/runtime/logger.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/runtime/prometheus.py` & `dlt-0.2.9a0/dlt/common/runtime/prometheus.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/runtime/segment.py` & `dlt-0.2.9a0/dlt/common/runtime/segment.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/runtime/sentry.py` & `dlt-0.2.9a0/dlt/common/runtime/sentry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/runtime/signals.py` & `dlt-0.2.9a0/dlt/common/runtime/signals.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/runtime/slack.py` & `dlt-0.2.9a0/dlt/common/runtime/slack.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/runtime/telemetry.py` & `dlt-0.2.9a0/dlt/common/runtime/telemetry.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/schema/detections.py` & `dlt-0.2.9a0/dlt/common/schema/detections.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/schema/exceptions.py` & `dlt-0.2.9a0/dlt/common/schema/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/schema/schema.py` & `dlt-0.2.9a0/dlt/common/schema/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -318,15 +318,15 @@
 
     def to_pretty_json(self, remove_defaults: bool = True) -> str:
         d = self.to_dict(remove_defaults=remove_defaults)
         return json.dumps(d, pretty=True)
 
     def to_pretty_yaml(self, remove_defaults: bool = True) -> str:
         d = self.to_dict(remove_defaults=remove_defaults)
-        return yaml.dump(d, allow_unicode=True, default_flow_style=False, sort_keys=False)
+        return cast(str, yaml.dump(d, allow_unicode=True, default_flow_style=False, sort_keys=False))
 
     def clone(self) -> "Schema":
         d = deepcopy(self.to_dict())
         return Schema.from_dict(d)  # type: ignore
 
     def _infer_column(self, k: str, v: Any, data_type: TDataType = None, is_variant: bool = False) -> TColumnSchema:
         column_schema =  TColumnSchema(
```

### Comparing `dlt-0.2.9/dlt/common/schema/typing.py` & `dlt-0.2.9a0/dlt/common/schema/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/schema/utils.py` & `dlt-0.2.9a0/dlt/common/schema/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/source.py` & `dlt-0.2.9a0/dlt/common/source.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/storages/__init__.py` & `dlt-0.2.9a0/dlt/common/storages/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/storages/configuration.py` & `dlt-0.2.9a0/dlt/common/storages/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/storages/data_item_storage.py` & `dlt-0.2.9a0/dlt/common/storages/data_item_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/storages/exceptions.py` & `dlt-0.2.9a0/dlt/common/storages/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/storages/file_storage.py` & `dlt-0.2.9a0/dlt/common/storages/file_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/storages/live_schema_storage.py` & `dlt-0.2.9a0/dlt/common/storages/live_schema_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/storages/load_storage.py` & `dlt-0.2.9a0/dlt/common/storages/load_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/storages/normalize_storage.py` & `dlt-0.2.9a0/dlt/common/storages/normalize_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/storages/schema_storage.py` & `dlt-0.2.9a0/dlt/common/storages/schema_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/storages/versioned_storage.py` & `dlt-0.2.9a0/dlt/common/storages/versioned_storage.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/time.py` & `dlt-0.2.9a0/dlt/common/time.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/typing.py` & `dlt-0.2.9a0/dlt/common/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/utils.py` & `dlt-0.2.9a0/dlt/common/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/validation.py` & `dlt-0.2.9a0/dlt/common/validation.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/common/wei.py` & `dlt-0.2.9a0/dlt/common/wei.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/destinations/bigquery/__init__.py` & `dlt-0.2.9a0/dlt/destinations/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/destinations/bigquery/bigquery.py` & `dlt-0.2.9a0/dlt/destinations/bigquery/bigquery.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,16 +149,16 @@
                     raise LoadJobNotExistsException(file_path)
                 elif reason in BQ_TERMINAL_REASONS:
                     raise LoadJobTerminalException(file_path)
                 else:
                     raise DestinationTransientException(gace)
         return job
 
-    def start_file_load(self, table: TTableSchema, file_path: str, load_id: str) -> LoadJob:
-        job = super().start_file_load(table, file_path, load_id)
+    def start_file_load(self, table: TTableSchema, file_path: str) -> LoadJob:
+        job = super().start_file_load(table, file_path)
         if not job:
             try:
                 job = BigQueryLoadJob(
                     FileStorage.get_file_name_from_file_path(file_path),
                     self._create_load_job(table["name"], table["write_disposition"], file_path),
                     self.config.credentials
                 )
```

### Comparing `dlt-0.2.9/dlt/destinations/bigquery/sql_client.py` & `dlt-0.2.9a0/dlt/destinations/bigquery/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/destinations/duckdb/__init__.py` & `dlt-0.2.9a0/dlt/destinations/duckdb/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/destinations/duckdb/configuration.py` & `dlt-0.2.9a0/dlt/destinations/duckdb/configuration.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,23 +83,18 @@
         # do not set any paths for external database
         if self.database == ":external:":
             return
         # try the pipeline context
         is_default_path = False
         if self.database == ":pipeline:":
             self.database = self._path_in_pipeline(DEFAULT_DUCK_DB_NAME)
-        else:
-            # maybe get database
-            maybe_database, maybe_is_default_path = self._path_from_pipeline(DEFAULT_DUCK_DB_NAME)
-            # if pipeline context was not present or database was not set
-            if not self.database or not maybe_is_default_path:
-                # create database locally
-                is_default_path = maybe_is_default_path
-                self.database = maybe_database
-
+        # if pipeline context was not present or database was not set
+        if not self.database:
+            # create database locally
+            self.database, is_default_path = self._path_from_pipeline(DEFAULT_DUCK_DB_NAME)
         # always make database an abs path
         self.database = os.path.abspath(self.database)
         # do not save the default path into pipeline's local state
         if not is_default_path:
             self._path_to_pipeline(self.database)
 
     def _path_in_pipeline(self, rel_path: str) -> str:
```

### Comparing `dlt-0.2.9/dlt/destinations/duckdb/duck.py` & `dlt-0.2.9a0/dlt/destinations/duckdb/duck.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/destinations/duckdb/sql_client.py` & `dlt-0.2.9a0/dlt/destinations/duckdb/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/destinations/dummy/__init__.py` & `dlt-0.2.9a0/dlt/destinations/dummy/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/destinations/dummy/configuration.py` & `dlt-0.2.9a0/dlt/destinations/dummy/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/destinations/dummy/dummy.py` & `dlt-0.2.9a0/dlt/destinations/dummy/dummy.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
     def update_storage_schema(self, staging: bool = False, only_tables: Iterable[str] = None, expected_update: TSchemaTables = None) -> Optional[TSchemaTables]:
         applied_update = super().update_storage_schema(staging, only_tables, expected_update)
         if self.config.fail_schema_update:
             raise DestinationTransientException("Raise on schema update due to fail_schema_update config flag")
         return applied_update
 
-    def start_file_load(self, table: TTableSchema, file_path: str, load_id: str) -> LoadJob:
+    def start_file_load(self, table: TTableSchema, file_path: str) -> LoadJob:
         job_id = FileStorage.get_file_name_from_file_path(file_path)
         file_name = FileStorage.get_file_name_from_file_path(file_path)
         # return existing job if already there
         if job_id not in JOBS:
             JOBS[job_id] = self._create_job(file_name)
         else:
             job = JOBS[job_id]
```

### Comparing `dlt-0.2.9/dlt/destinations/exceptions.py` & `dlt-0.2.9a0/dlt/destinations/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/destinations/filesystem/__init__.py` & `dlt-0.2.9a0/dlt/destinations/postgres/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 from typing import Type
 
 from dlt.common.schema.schema import Schema
 from dlt.common.configuration import with_config, known_sections
 from dlt.common.configuration.accessors import config
+from dlt.common.data_writers.escape import escape_postgres_identifier, escape_postgres_literal
 from dlt.common.destination import DestinationCapabilitiesContext
-from dlt.common.destination.reference import JobClientBase, DestinationClientDwhConfiguration
+from dlt.common.destination.reference import JobClientBase, DestinationClientConfiguration
 
-from dlt.destinations.filesystem.configuration import FilesystemClientConfiguration
+from dlt.destinations.postgres.configuration import PostgresClientConfiguration
 
 
-@with_config(spec=FilesystemClientConfiguration, sections=(known_sections.DESTINATION, "filesystem",))
-def _configure(config: FilesystemClientConfiguration = config.value) -> FilesystemClientConfiguration:
+@with_config(spec=PostgresClientConfiguration, sections=(known_sections.DESTINATION, "postgres",))
+def _configure(config: PostgresClientConfiguration = config.value) -> PostgresClientConfiguration:
     return config
 
 
 def capabilities() -> DestinationCapabilitiesContext:
+    # https://www.postgresql.org/docs/current/limits.html
     caps = DestinationCapabilitiesContext()
-    caps.preferred_loader_file_format = "jsonl"
-    caps.supported_loader_file_formats = ["jsonl"]
-
-    caps.max_identifier_length = 127
-    caps.max_column_identifier_length = 127
-    caps.max_query_length = 1024 * 1024 * 1024
+    caps.preferred_loader_file_format = "insert_values"
+    caps.supported_loader_file_formats = ["insert_values", "sql"]
+    caps.escape_identifier = escape_postgres_identifier
+    caps.escape_literal = escape_postgres_literal
+    caps.max_identifier_length = 63
+    caps.max_column_identifier_length = 63
+    caps.max_query_length = 32 * 1024 * 1024
     caps.is_max_query_length_in_bytes = True
-    caps.max_text_data_type_length = 1024 * 1024
+    caps.max_text_data_type_length = 1024 * 1024 * 1024
     caps.is_max_text_data_type_length_in_bytes = True
-    caps.supports_ddl_transactions = False
+    caps.supports_ddl_transactions = True
 
     return caps
 
 
-def client(schema: Schema, initial_config: DestinationClientDwhConfiguration = config.value) -> JobClientBase:
+def client(schema: Schema, initial_config: DestinationClientConfiguration = config.value) -> JobClientBase:
     # import client when creating instance so capabilities and config specs can be accessed without dependencies installed
-    from dlt.destinations.filesystem.filesystem import FilesystemClient
+    from dlt.destinations.postgres.postgres import PostgresClient
 
-    return FilesystemClient(schema, _configure(initial_config))  # type: ignore
+    return PostgresClient(schema, _configure(initial_config))  # type: ignore
 
 
-def spec() -> Type[FilesystemClientConfiguration]:
-    return FilesystemClientConfiguration
+def spec() -> Type[DestinationClientConfiguration]:
+    return PostgresClientConfiguration
```

### Comparing `dlt-0.2.9/dlt/destinations/insert_job_client.py` & `dlt-0.2.9a0/dlt/destinations/insert_job_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             if write_disposition == "replace":
                 insert_sql.append("DELETE FROM {};".format(qualified_table_name))
             while content := f.read(self._sql_client.capabilities.max_query_length // 2):
                 # write INSERT
                 insert_sql.extend([header.format(qualified_table_name), values_mark, content])
                 # read one more line in order to
                 # 1. complete the content which ends at "random" position, not an end line
-                # 2. to modify its ending without a need to re-allocating the 8MB of "content"
+                # 2. to modify it's ending without a need to re-allocating the 8MB of "content"
                 until_nl = f.readline()
                 # if until next line contains just '\n' try to take another line so we can finish content properly
                 # TODO: write test for this case (content ends with ",")
                 if until_nl == "\n":
                     until_nl = f.readline()
                 until_nl = until_nl.strip("\n")
                 # if there was anything left, until_nl contains the last line
@@ -83,16 +83,16 @@
             LoadJob: Always a restored job completed
         """
         job = super().restore_file_load(file_path)
         if not job:
             job = EmptyLoadJob.from_file_path(file_path, "completed")
         return job
 
-    def start_file_load(self, table: TTableSchema, file_path: str, load_id: str) -> LoadJob:
-        job = super().start_file_load(table, file_path, load_id)
+    def start_file_load(self, table: TTableSchema, file_path: str) -> LoadJob:
+        job = super().start_file_load(table, file_path)
         if not job:
             # this is using sql_client internally and will raise a right exception
             job = InsertValuesLoadJob(table["name"], table["write_disposition"], file_path, self.sql_client)
         return job
 
     # TODO: implement indexes and primary keys for postgres
     def _get_in_table_constraints_sql(self, t: TTableSchema) -> str:
```

### Comparing `dlt-0.2.9/dlt/destinations/job_client_impl.py` & `dlt-0.2.9a0/dlt/destinations/job_client_impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
                 yield
         else:
             yield
 
     def create_merge_job(self, table_chain: Sequence[TTableSchema]) -> NewLoadJob:
         return SqlMergeJob.from_table_chain(table_chain, self.sql_client)
 
-    def start_file_load(self, table: TTableSchema, file_path: str, load_id: str) -> LoadJob:
+    def start_file_load(self, table: TTableSchema, file_path: str) -> LoadJob:
         """Starts SqlLoadJob for files ending with .sql or returns None to let derived classes to handle their specific jobs"""
         if SqlLoadJob.is_sql_job(file_path):
             # execute sql load job
             return SqlLoadJob(file_path, self.sql_client)
         return None
 
     def restore_file_load(self, file_path: str) -> LoadJob:
```

### Comparing `dlt-0.2.9/dlt/destinations/job_impl.py` & `dlt-0.2.9a0/dlt/destinations/job_impl.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/destinations/postgres/configuration.py` & `dlt-0.2.9a0/dlt/destinations/postgres/configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 from typing import Final, ClassVar, Any, List
 from sqlalchemy.engine import URL
 
 from dlt.common.configuration import configspec
 from dlt.common.configuration.specs import ConnectionStringCredentials
 from dlt.common.destination.reference import DestinationClientDwhConfiguration
-from dlt.common.typing import TSecretValue
 
 
 @configspec
 class PostgresCredentials(ConnectionStringCredentials):
     drivername: Final[str] = "postgresql"  # type: ignore
-    password: TSecretValue
-    host: str
     port: int = 5432
     connect_timeout: int = 15
 
     __config_gen_annotations__: ClassVar[List[str]] = ["port", "connect_timeout"]
 
     def parse_native_representation(self, native_value: Any) -> None:
         super().parse_native_representation(native_value)
```

### Comparing `dlt-0.2.9/dlt/destinations/postgres/postgres.py` & `dlt-0.2.9a0/dlt/destinations/postgres/postgres.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/destinations/postgres/sql_client.py` & `dlt-0.2.9a0/dlt/destinations/postgres/sql_client.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/destinations/redshift/README.md` & `dlt-0.2.9a0/dlt/destinations/redshift/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/destinations/redshift/__init__.py` & `dlt-0.2.9a0/dlt/destinations/redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/destinations/redshift/configuration.py` & `dlt-0.2.9a0/dlt/destinations/redshift/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/destinations/redshift/redshift.py` & `dlt-0.2.9a0/dlt/destinations/redshift/redshift.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/destinations/sql_client.py` & `dlt-0.2.9a0/dlt/destinations/sql_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
         self.fetchmany = curr.fetchmany  # type: ignore
         self.fetchone = curr.fetchone  # type: ignore
 
     def __getattr__(self, name: str) -> Any:
         return getattr(self.native_cursor, name)
 
     def df(self, chunk_size: int = None, **kwargs: Any) -> Optional[DataFrame]:
-        from dlt.helpers.pandas_helper import _wrap_result
+        from dlt.helpers.pandas import _wrap_result
 
         columns = [c[0] for c in self.native_cursor.description]
         if chunk_size is None:
             return _wrap_result(self.native_cursor.fetchall(), columns, **kwargs)
         else:
             df = _wrap_result(self.native_cursor.fetchmany(chunk_size), columns, **kwargs)
             # if no rows return None
```

### Comparing `dlt-0.2.9/dlt/destinations/sql_merge_job.py` & `dlt-0.2.9a0/dlt/destinations/sql_merge_job.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         try:
             sql = cls.gen_merge_sql(table_chain, sql_client)
             job = cls(file_info.job_id(), "running")
             job._save_text_file("\n".join(sql))
         except Exception:
             # return failed job
             failed_text = "Tried to generate a merge sql job for the following tables:"
-            tables_str = yaml.dump(table_chain, allow_unicode=True, default_flow_style=False, sort_keys=False)
+            tables_str = cast(str, yaml.dump(table_chain, allow_unicode=True, default_flow_style=False, sort_keys=False))
             job = cls(file_info.job_id(), "failed", pretty_format_exception())
             job._save_text_file("\n".join([failed_text, tables_str]))
         return job
 
     @classmethod
     def _gen_key_table_clauses(cls, primary_keys: Sequence[str], merge_keys: Sequence[str])-> List[str]:
         """Generate sql clauses to select rows to delete via merge and primary key. Return select all clause if no keys defined."""
```

### Comparing `dlt-0.2.9/dlt/destinations/typing.py` & `dlt-0.2.9a0/dlt/destinations/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/extract/decorators.py` & `dlt-0.2.9a0/dlt/extract/decorators.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,19 +146,21 @@
             # make schema available to the source
             with Container().injectable_context(SourceSchemaInjectableContext(schema)):
                 # configurations will be accessed in this section in the source
                 proxy = Container()[PipelineContext]
                 pipeline_name = None if not proxy.is_active() else proxy.pipeline().pipeline_name
                 with inject_section(ConfigSectionContext(pipeline_name=pipeline_name, sections=source_sections)):
                     rv = conf_f(*args, **kwargs)
-                    if rv is None:
-                        raise SourceDataIsNone(name)
-                    # if generator, consume it immediately
-                    if inspect.isgenerator(rv):
-                        rv = list(rv)
+
+            if rv is None:
+                raise SourceDataIsNone(name)
+
+            # if generator, consume it immediately
+            if inspect.isgenerator(rv):
+                rv = list(rv)
 
             # convert to source
             s = DltSource.from_data(name, source_section, schema.clone(), rv)
             # apply hints
             if max_table_nesting is not None:
                 s.max_table_nesting = max_table_nesting
             # enable root propagation
```

### Comparing `dlt-0.2.9/dlt/extract/exceptions.py` & `dlt-0.2.9a0/dlt/extract/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/extract/extract.py` & `dlt-0.2.9a0/dlt/extract/extract.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/extract/incremental.py` & `dlt-0.2.9a0/dlt/extract/incremental.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/extract/pipe.py` & `dlt-0.2.9a0/dlt/extract/pipe.py`

 * *Files 0% similar despite different names*

```diff
@@ -420,15 +420,15 @@
     @configspec
     class PipeIteratorConfiguration(BaseConfiguration):
         max_parallel_items: int = 20
         workers: int = 5
         futures_poll_interval: float = 0.01
         copy_on_fork: bool = False
 
-        __section__ = "extract"
+        __sections__ = "extract"
 
     def __init__(self, max_parallel_items: int, workers: int, futures_poll_interval: float) -> None:
         self.max_parallel_items = max_parallel_items
         self.workers = workers
         self.futures_poll_interval = futures_poll_interval
 
         self._async_pool: asyncio.AbstractEventLoop = None
@@ -462,15 +462,14 @@
         yield_parents: bool = True,
         *,
         max_parallel_items: int = 20,
         workers: int = 5,
         futures_poll_interval: float = 0.01,
         copy_on_fork: bool = False
     ) -> "PipeIterator":
-        # print(f"max_parallel_items: {max_parallel_items} workers: {workers}")
         extract = cls(max_parallel_items, workers, futures_poll_interval)
         # clone all pipes before iterating (recursively) as we will fork them (this add steps) and evaluate gens
         pipes = PipeIterator.clone_pipes(pipes)
 
         def _fork_pipeline(pipe: Pipe) -> None:
             if pipe.parent:
                 # fork the parent pipe
```

### Comparing `dlt-0.2.9/dlt/extract/schema.py` & `dlt-0.2.9a0/dlt/extract/schema.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/extract/source.py` & `dlt-0.2.9a0/dlt/extract/source.py`

 * *Files 1% similar despite different names*

```diff
@@ -290,15 +290,15 @@
             self._pipe.__dict__.update(gen.__dict__)
         else:
             self._bound = True
         return self
 
     @property
     def state(self) -> StrAny:
-        """Gets resource-scoped state from the active pipeline. PipelineStateNotAvailable is raised if pipeline context is not available"""
+        """Gets resource-scoped state from the existing pipeline context. If pipeline context is not available, PipelineStateNotAvailable is raised"""
         with self._get_config_section_context():
             return resource_state(self.name)
 
     def __call__(self, *args: Any, **kwargs: Any) -> "DltResource":
         """Binds the parametrized resources to passed arguments. Creates and returns a bound resource. Generators and iterators are not evaluated."""
         if self._bound:
             raise TypeError("Bound DltResource object is not callable")
@@ -665,15 +665,15 @@
     def run(self) -> SupportsPipelineRun:
         """A convenience method that will call `run` run on the currently active `dlt` pipeline. If pipeline instance is not found, one with default settings will be created."""
         self_run: SupportsPipelineRun = makefun.partial(Container()[PipelineContext].pipeline().run, *(), data=self)
         return self_run
 
     @property
     def state(self) -> StrAny:
-        """Gets source-scoped state from the active pipeline. PipelineStateNotAvailable is raised if no pipeline is active"""
+        """Gets source-scoped state from the existing pipeline context. If pipeline context is not available, PipelineStateNotAvailable is raised"""
         with self._get_config_section_context():
             return source_state()
 
     def clone(self) -> "DltSource":
         """Creates a deep copy of the source where copies of schema, resources and pipes are created"""
         # mind that resources and pipes are cloned when added to the DltResourcesDict in the source constructor
         return DltSource(self.name, self.section, self.schema.clone(), list(self._resources.values()))
```

### Comparing `dlt-0.2.9/dlt/extract/typing.py` & `dlt-0.2.9a0/dlt/extract/typing.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/extract/utils.py` & `dlt-0.2.9a0/dlt/extract/utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/helpers/dbt/__init__.py` & `dlt-0.2.9a0/dlt/helpers/dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/helpers/dbt/configuration.py` & `dlt-0.2.9a0/dlt/helpers/dbt/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/helpers/dbt/dbt_utils.py` & `dlt-0.2.9a0/dlt/helpers/dbt/dbt_utils.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/helpers/dbt/exceptions.py` & `dlt-0.2.9a0/dlt/helpers/dbt/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/helpers/dbt/profiles.yml` & `dlt-0.2.9a0/dlt/helpers/dbt/profiles.yml`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/helpers/dbt/runner.py` & `dlt-0.2.9a0/dlt/helpers/dbt/runner.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/helpers/pandas_helper.py` & `dlt-0.2.9a0/dlt/helpers/pandas.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/helpers/parquet.py` & `dlt-0.2.9a0/dlt/helpers/parquet.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/helpers/streamlit_helper.py` & `dlt-0.2.9a0/dlt/helpers/streamlit.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from dlt.common import pendulum
 from dlt.common.typing import AnyFun
 from dlt.common.schema.typing import LOADS_TABLE_NAME, VERSION_TABLE_NAME
 from dlt.common.configuration.exceptions import ConfigFieldMissingException
 from dlt.common.exceptions import MissingDependencyException
 
-from dlt.helpers.pandas_helper import pd
+from dlt.helpers.pandas import pd
 from dlt.pipeline import Pipeline
 from dlt.pipeline.exceptions import CannotRestorePipelineException
 from dlt.pipeline.state_sync import load_state_from_destination
 
 try:
     import streamlit as st
     # from streamlit import SECRETS_FILE_LOC, secrets
```

### Comparing `dlt-0.2.9/dlt/load/configuration.py` & `dlt-0.2.9a0/dlt/load/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/load/exceptions.py` & `dlt-0.2.9a0/dlt/load/exceptions.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/load/load.py` & `dlt-0.2.9a0/dlt/load/load.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
                 job_info = self.load_storage.parse_job_file_name(file_path)
                 if job_info.file_format not in self.capabilities.supported_loader_file_formats:
                     raise LoadClientUnsupportedFileFormats(job_info.file_format, self.capabilities.supported_loader_file_formats, file_path)
                 logger.info(f"Will load file {file_path} with table name {job_info.table_name}")
                 table = self.get_load_table(schema, file_path)
                 if table["write_disposition"] not in ["append", "replace", "merge"]:
                     raise LoadClientUnsupportedWriteDisposition(job_info.table_name, table["write_disposition"], file_path)
-                job = client.start_file_load(table, self.load_storage.storage.make_full_path(file_path), load_id)
+                job = client.start_file_load(table, self.load_storage.storage.make_full_path(file_path))
         except (DestinationTerminalException, TerminalValueError):
             # if job irreversibly cannot be started, mark it as failed
             logger.exception(f"Terminal problem when adding job {file_path}")
             job = EmptyLoadJob.from_file_path(file_path, "failed", pretty_format_exception())
         except (DestinationTransientException, Exception):
             # return no job so file stays in new jobs (root) folder
             logger.exception(f"Temporary problem when adding job {file_path}")
@@ -335,14 +335,14 @@
         dataset_name = None
         if isinstance(self.initial_client_config, DestinationClientDwhConfiguration):
             dataset_name = self.initial_client_config.dataset_name
 
         return LoadInfo(
             pipeline,
             self.initial_client_config.destination_name,
-            str(self.initial_client_config),
+            str(self.initial_client_config.credentials),
             dataset_name,
             list(load_ids),
             load_packages,
             started_at,
             pipeline.first_run
         )
```

### Comparing `dlt-0.2.9/dlt/normalize/configuration.py` & `dlt-0.2.9a0/dlt/normalize/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/normalize/normalize.py` & `dlt-0.2.9a0/dlt/normalize/normalize.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/pipeline/README.md` & `dlt-0.2.9a0/dlt/pipeline/README.md`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/pipeline/__init__.py` & `dlt-0.2.9a0/dlt/pipeline/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,16 @@
         export_schema_path,
         full_refresh,
         progress,
         False,
         last_config(**kwargs),
         kwargs["runtime"])
     # set it as current pipeline
-    p.activate()
+    Container()[PipelineContext].activate(p)
+
     return p
 
 
 @with_config(spec=PipelineConfiguration, auto_pipeline_section=True)
 def attach(
     pipeline_name: str = None,
     pipelines_dir: str = None,
@@ -146,15 +147,15 @@
     # if working_dir not provided use temp folder
     if not pipelines_dir:
         pipelines_dir = get_dlt_pipelines_dir()
     progress = collector_from_name(progress)
     # create new pipeline instance
     p = Pipeline(pipeline_name, pipelines_dir, pipeline_salt, None, None, None, None, None, full_refresh, progress, True, last_config(**kwargs), kwargs["runtime"])
     # set it as current pipeline
-    p.activate()
+    Container()[PipelineContext].activate(p)
     return p
 
 
 def run(
     data: Any,
     *,
     destination: TDestinationReferenceArg = None,
```

### Comparing `dlt-0.2.9/dlt/pipeline/configuration.py` & `dlt-0.2.9a0/dlt/pipeline/configuration.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/pipeline/dbt.py` & `dlt-0.2.9a0/dlt/pipeline/dbt.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/pipeline/exceptions.py` & `dlt-0.2.9a0/dlt/pipeline/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,12 +50,7 @@
 class PipelineHasPendingDataException(PipelineException):
     def __init__(self, pipeline_name: str, pipelines_dir: str) -> None:
         msg = (
             f" Operation failed because pipeline with name {pipeline_name} in working directory {pipelines_dir} contains pending extracted files or load packages. "
             "Use `dlt pipeline sync` to reset the local state then run this operation again."
         )
         super().__init__(pipeline_name, msg)
-
-
-class PipelineNotActive(PipelineException):
-    def __init__(self, pipeline_name: str) -> None:
-        super().__init__(pipeline_name, f"Pipeline {pipeline_name} is not active so it cannot be deactivated")
```

### Comparing `dlt-0.2.9/dlt/pipeline/helpers.py` & `dlt-0.2.9a0/dlt/pipeline/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from collections import defaultdict
 import contextlib
-from typing import Callable, Sequence, Iterable, Optional, Any, List, Iterator, Dict, Union, TypedDict
+from typing import Callable, Tuple, Iterable, Optional, Any, cast, List, Iterator, Dict, Union, TypedDict
 from itertools import chain
 
 from dlt.common.jsonpath import resolve_paths, TAnyJsonPath, compile_paths
 
 from dlt.common.exceptions import TerminalException
 from dlt.common.schema.utils import get_child_tables, group_tables_by_resource, compile_simple_regexes, compile_simple_regex
 from dlt.common.schema.typing import TSimpleRegex
@@ -12,30 +13,30 @@
 
 from dlt.pipeline.exceptions import PipelineStepFailed, PipelineHasPendingDataException
 from dlt.pipeline.typing import TPipelineStep
 from dlt.pipeline import Pipeline
 from dlt.common.pipeline import TSourceState, _reset_resource_state, sources_state, _delete_source_state_keys, _get_matching_resources
 
 
-def retry_load(retry_on_pipeline_steps: Sequence[TPipelineStep] = ("load",)) -> Callable[[BaseException], bool]:
+def retry_load(retry_on_pipeline_steps: Tuple[TPipelineStep, ...] = ("load",)) -> Callable[[Exception], bool]:
     """A retry strategy for Tenacity that, with default setting, will repeat `load` step for all exceptions that are not terminal
 
     Use this condition with tenacity `retry_if_exception`. Terminal exceptions are exceptions that will not go away when operations is repeated.
     Examples: missing configuration values, Authentication Errors, terminally failed jobs exceptions etc.
 
     >>> data = source(...)
     >>> for attempt in Retrying(stop=stop_after_attempt(3), retry=retry_if_exception(retry_load(())), reraise=True):
     >>>     with attempt:
     >>>         p.run(data)
 
     Args:
         retry_on_pipeline_steps (Tuple[TPipelineStep, ...], optional): which pipeline steps are allowed to be repeated. Default: "load"
 
     """
-    def _retry_load(ex: BaseException) -> bool:
+    def _retry_load(ex: Exception) -> bool:
         # do not retry in normalize or extract stages
         if isinstance(ex, PipelineStepFailed) and ex.step not in retry_on_pipeline_steps:
             return False
         # do not retry on terminal exceptions
         if isinstance(ex, TerminalException) or (ex.__context__ is not None and isinstance(ex.__context__, TerminalException)):
             return False
         return True
```

### Comparing `dlt-0.2.9/dlt/pipeline/pipeline.py` & `dlt-0.2.9a0/dlt/pipeline/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from dlt.common.schema.typing import TColumnKey, TColumnSchema, TSchemaTables, TWriteDisposition
 from dlt.common.storages.load_storage import LoadJobInfo, LoadPackageInfo
 from dlt.common.typing import TFun, TSecretValue
 from dlt.common.runners import pool_runner as runner
 from dlt.common.storages import LiveSchemaStorage, NormalizeStorage, LoadStorage, SchemaStorage, FileStorage, NormalizeStorageConfiguration, SchemaStorageConfiguration, LoadStorageConfiguration
 from dlt.common.destination import DestinationCapabilitiesContext
 from dlt.common.destination.reference import DestinationReference, JobClientBase, DestinationClientConfiguration, DestinationClientDwhConfiguration, TDestinationReferenceArg
-from dlt.common.pipeline import ExtractInfo, LoadInfo, NormalizeInfo, PipelineContext, SupportsPipeline, TPipelineLocalState, TPipelineState, StateInjectableContext
+from dlt.common.pipeline import ExtractInfo, LoadInfo, NormalizeInfo, SupportsPipeline, TPipelineLocalState, TPipelineState, StateInjectableContext
 from dlt.common.schema import Schema
 from dlt.common.utils import is_interactive
 
 from dlt.destinations.exceptions import DatabaseUndefinedRelation
 
 from dlt.extract.exceptions import DataItemRequiredForDynamicTableHints, SourceExhausted
 from dlt.extract.extract import ExtractorStorage, extract_with_schema
@@ -38,27 +38,25 @@
 from dlt.destinations.sql_client import SqlClientBase
 from dlt.destinations.job_client_impl import SqlJobClientBase
 from dlt.load.configuration import LoaderConfiguration
 from dlt.load import Load
 
 from dlt.pipeline.configuration import PipelineConfiguration
 from dlt.pipeline.progress import _Collector, _NULL_COLLECTOR
-from dlt.pipeline.exceptions import CannotRestorePipelineException, InvalidPipelineName, PipelineConfigMissing, PipelineNotActive, PipelineStepFailed, SqlClientNotAvailable
+from dlt.pipeline.exceptions import CannotRestorePipelineException, InvalidPipelineName, PipelineConfigMissing, PipelineStepFailed, SqlClientNotAvailable
 from dlt.pipeline.trace import PipelineTrace, PipelineStepTrace, load_trace, merge_traces, start_trace, start_trace_step, end_trace_step, end_trace
 from dlt.pipeline.typing import TPipelineStep
 from dlt.pipeline.state_sync import STATE_ENGINE_VERSION, load_state_from_destination, merge_state_if_changed, migrate_state, state_resource, json_encode_state, json_decode_state
 
 
 def with_state_sync(may_extract_state: bool = False) -> Callable[[TFun], TFun]:
 
     def decorator(f: TFun) -> TFun:
         @wraps(f)
         def _wrap(self: "Pipeline", *args: Any, **kwargs: Any) -> Any:
-            # activate pipeline so right state is always provided
-            self.activate()
             # backup and restore state
             should_extract_state = may_extract_state and self.config.restore_from_destination
             with self.managed_state(extract_state=should_extract_state) as state:
                 # add the state to container as a context
                 with self._container.injectable_context(StateInjectableContext(state=state)):
                     return f(self, *args, **kwargs)
 
@@ -216,15 +214,15 @@
             # we overwrite the state with the values from init
             self._set_destination(destination)  # changing the destination could be dangerous if pipeline has not loaded items
             self._set_dataset_name(dataset_name)
             self.credentials = credentials
             self._configure(import_schema_path, export_schema_path, must_attach_to_local_pipeline)
 
     def drop(self) -> "Pipeline":
-        """Deletes local pipeline state, schemas and any working files"""
+        """Deletes existing pipeline state, schemas and drops datasets at the destination if present"""
         # reset the pipeline working dir
         self._create_pipeline()
         # clone the pipeline
         return Pipeline(
             self.pipeline_name,
             self.pipelines_dir,
             self.pipeline_salt,
@@ -530,42 +528,14 @@
             if "_local" not in state:
                 state["_local"] = local_state
             self._props_to_state(state)
             self._save_state(state)
         except Exception as ex:
             raise PipelineStepFailed(self, "run", ex, None) from ex
 
-    def activate(self) -> None:
-        """Activates the pipeline
-
-        The active pipeline is used as a context for several `dlt` components. It provides state to sources and resources evaluated outside of
-        `pipeline.run` and `pipeline.extract` method. For example, if the source you use is accessing state in `dlt.source` decorated function, the state is provided
-        by active pipeline.
-
-        The name of active pipeline is used when resolving secrets and config values as the optional most outer section during value lookup. For example if pipeline
-        with name `chess_pipeline` is active and `dlt` looks for `BigQuery` configuration, it will look in `chess_pipeline.destination.bigquery.credentials` first and then in
-        `destination.bigquery.credentials`.
-
-        Active pipeline also provides the current DestinationCapabilitiesContext to other components ie. Schema instances. Among others, it sets the naming convention
-        and maximum identifier length.
-
-        Only one pipeline is active at a given time.
-
-        Pipeline created or attached with `dlt.pipeline`/'dlt.attach` is automatically activated. `run`, `load` and `extract` methods also activate pipeline.
-        """
-        Container()[PipelineContext].activate(self)
-
-    def deactivate(self) -> None:
-        """Deactivates the pipeline
-
-        Pipeline must be active in order to use this method. Please refer to `activate()` method for the explanation of active pipeline concept.
-        """
-        if not self.is_active:
-            raise PipelineNotActive(self.pipeline_name)
-        Container()[PipelineContext].deactivate()
 
     @property
     def has_data(self) -> bool:
         """Tells if the pipeline contains any data: schemas, extracted files, load packages or loaded packages in the destination"""
         return not self.first_run or bool(self.schema_names) or len(self.list_extracted_resources()) > 0 or len(self.list_normalized_load_packages()) > 0
 
     @property
@@ -655,24 +625,14 @@
         #     )
         if schema_name:
             schema = self.schemas[schema_name]
         else:
             schema = self.default_schema if self.default_schema_name else Schema(self.dataset_name)
         return self._sql_job_client(schema, credentials).sql_client
 
-    def _destination_client(self, schema_name: str = None, credentials: Any = None) -> JobClientBase:
-        """Get the destination job client for the configured destination"""
-        # TODO: duplicated code from self.sql_client()  ...
-        if schema_name:
-            schema = self.schemas[schema_name]
-        else:
-            schema = self.default_schema if self.default_schema_name else Schema(self.dataset_name)
-        client_config = self._get_destination_client_initial_config(credentials)
-        return self._get_destination_client(schema, client_config)
-
     def _sql_job_client(self, schema: Schema, credentials: Any = None) -> SqlJobClientBase:
         client_config = self._get_destination_client_initial_config(credentials)
         client = self._get_destination_client(schema , client_config)
         if isinstance(client, SqlJobClientBase):
             return client
         else:
             raise SqlClientNotAvailable(self.pipeline_name, self.destination.__name__)
```

### Comparing `dlt-0.2.9/dlt/pipeline/progress.py` & `dlt-0.2.9a0/dlt/pipeline/progress.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/pipeline/state_sync.py` & `dlt-0.2.9a0/dlt/pipeline/state_sync.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/pipeline/trace.py` & `dlt-0.2.9a0/dlt/pipeline/trace.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/pipeline/track.py` & `dlt-0.2.9a0/dlt/pipeline/track.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 from dlt.common import pendulum
 from dlt.common import logger
 from dlt.common.runtime.exec_info import github_info
 from dlt.common.runtime.segment import track as dlthub_telemetry_track
 from dlt.common.runtime.slack import send_slack_message
 from dlt.common.pipeline import LoadInfo, SupportsPipeline
-from dlt.common.destination import DestinationReference
 
 from dlt.pipeline.typing import TPipelineStep
 from dlt.pipeline.trace import PipelineTrace, PipelineStepTrace
 
 
 def _add_sentry_tags(span: Span, pipeline: SupportsPipeline) -> None:
     span.set_tag("pipeline_name", pipeline.pipeline_name)
@@ -79,15 +78,15 @@
     # disable automatic slack messaging until we can configure messages themselves
     # if step.step == "load":
     #     if pipeline.runtime_config.slack_incoming_hook and step.step_exception is None:
     #         slack_notify_load_success(pipeline.runtime_config.slack_incoming_hook, step_info, trace)
     dlthub_telemetry_track("pipeline", step.step, {
         "elapsed": (step.finished_at - trace.started_at).total_seconds(),
         "success": step.step_exception is None,
-        "destination_name": DestinationReference.to_name(pipeline.destination) if pipeline.destination else None,
+        "destination_name": pipeline.destination.__name__.split(".")[-1] if pipeline.destination else None,
         "transaction_id": trace.transaction_id
     })
 
 
 def on_end_trace(trace: PipelineTrace, pipeline: SupportsPipeline) -> None:
     if pipeline.runtime_config.sentry_dsn:
         # print(f"---END SENTRY TX: {trace.transaction_id} SCOPE: {Hub.current.scope}")
```

### Comparing `dlt-0.2.9/dlt/reflection/names.py` & `dlt-0.2.9a0/dlt/reflection/names.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/reflection/script_inspector.py` & `dlt-0.2.9a0/dlt/reflection/script_inspector.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/reflection/script_visitor.py` & `dlt-0.2.9a0/dlt/reflection/script_visitor.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/sources/helpers/requests/__init__.py` & `dlt-0.2.9a0/dlt/sources/helpers/requests/__init__.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/sources/helpers/requests/retry.py` & `dlt-0.2.9a0/dlt/sources/helpers/requests/retry.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,39 +129,37 @@
     >>>         return False
     >>>     return response.text == 'error'
 
     The retry is triggered when either any of the predicates or the default conditions based on status code/exception are `True`.
 
     ### Args:
         timeout: Timeout for requests in seconds. May be passed as `timedelta` or `float/int` number of seconds.
-        max_connections: Max connections per host in the HTTPAdapter pool
         raise_for_status: Whether to raise exception on error status codes (using `response.raise_for_status()`)
         session: Optional `requests.Session` instance to add the retry handler to. A new session is created by default.
         status_codes: Retry when response has any of these status codes. Default `429` and all `5xx` codes. Pass an empty list to disable retry based on status.
         exceptions: Retry on exception of given type(s). Default `(requests.Timeout, requests.ConnectionError)`. Pass an empty list to disable retry on exceptions.
         max_attempts: Max number of retry attempts before giving up
         condition: A predicate or a list of predicates to decide whether to retry. If any predicate returns `True` the request is retried
         backoff_factor: Multiplier used for exponential delay between retries
         respect_retry_after_header: Whether to use the `Retry-After` response header (when available) to determine the retry delay
         **session_attrs: Extra attributes that will be set on the session instance, e.g. `headers: {'Authorization': 'api-key'}` (see `requests.sessions.Session` for possible attributes)
     """
     def __init__(
         self,
         timeout: Optional[TimedeltaSeconds] = DEFAULT_TIMEOUT,
-        max_connections: int = 50,
         raise_for_status: bool = True,
         status_codes: Sequence[int] = DEFAULT_RETRY_STATUS,
         exceptions: Sequence[Type[Exception]] = DEFAULT_RETRY_EXCEPTIONS,
         max_attempts: int = DEFAULT_RETRY_ATTEMPTS,
         condition: Union[RetryPredicate, Sequence[RetryPredicate], None] = None,
         backoff_factor: float = DEFAULT_BACKOFF_FACTOR,
         respect_retry_after_header: bool = True,
         **session_attrs: Any
     ) -> None:
-        self._adapter = HTTPAdapter(pool_maxsize=max_connections)
+        self._adapter = HTTPAdapter()
         self._local = local()
         self._session_kwargs = dict(timeout=timeout, raise_for_status=raise_for_status)
         self._retry_kwargs = dict(
             status_codes=status_codes,
             exceptions=exceptions,
             max_attempts=max_attempts,
             condition=condition,
```

### Comparing `dlt-0.2.9/dlt/sources/helpers/requests/session.py` & `dlt-0.2.9a0/dlt/sources/helpers/requests/session.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/sources/helpers/transform.py` & `dlt-0.2.9a0/dlt/sources/helpers/transform.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/dlt/version.py` & `dlt-0.2.9a0/dlt/version.py`

 * *Files identical despite different names*

### Comparing `dlt-0.2.9/pyproject.toml` & `dlt-0.2.9a0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dlt"
-version = "0.2.9"
+version = "0.2.9a0"
 description = "DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run."
 authors = ["dltHub Inc. <services@dlthub.com>"]
 maintainers = [ "Marcin Rudolf <marcin@dlthub.com>", "Adrian Brudaru <adrian@dlthub.com>", "Ty Dunn <ty@dlthub.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/dlt-hub"
 repository = "https://github.com/dlt-hub/dlt"
@@ -66,18 +66,14 @@
 duckdb = {version = ">=0.6.1,<0.9.0", optional = true}
 
 dbt-core = {version = ">=1.3.0,<1.5.0", optional = true}
 dbt-redshift = {version = ">=1.3.0,<1.5.0", optional = true}
 dbt-bigquery = {version = ">=1.3.0,<1.5.0", optional = true}
 dbt-duckdb = {version = ">=1.3.0,<1.5.0", optional = true}
 psutil = "^5.9.5"
-s3fs = {version = "^2023.5.0", optional = true}
-gcsfs = {version = "^2023.5.0", optional = true}
-boto3 = {version = ">=1.26", optional = true}
-fsspec = "^2023.5.0"
 
 
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.4"
 mypy = "1.2.0"
 flake8 = "^5.0.0"
@@ -96,23 +92,20 @@
 flake8-tidy-imports = ">=4.8.0"
 flake8-encodings = "^0.5.0"
 flake8-builtins = "^1.5.3"
 types-SQLAlchemy = ">=1.4.53"
 
 [tool.poetry.extras]
 dbt = ["dbt-core", "dbt-redshift", "dbt-bigquery", "dbt-duckdb"]
-gcp = ["grpcio", "google-cloud-bigquery", "pyarrow", "db-dtypes", "gcsfs"]
+gcp = ["grpcio", "google-cloud-bigquery", "pyarrow", "db-dtypes"]
 # bigquery is alias on gcp extras
-bigquery = ["grpcio", "google-cloud-bigquery", "pyarrow", "db-dtypes", "gcsfs"]
+bigquery = ["grpcio", "google-cloud-bigquery", "pyarrow", "db-dtypes"]
 postgres = ["psycopg2-binary", "psycopg2cffi"]
 redshift = ["psycopg2-binary", "psycopg2cffi"]
 duckdb = ["duckdb"]
-filesystem = ["s3fs", "boto3"]
-s3 = ["s3fs", "boto3"]
-gs = ["gcsfs"]
 
 [tool.poetry.scripts]
 dlt = "dlt.cli._dlt:_main"
 
 [tool.poetry.group.dev.dependencies]
 requests-mock = "^1.10.0"
 types-click = "^7.1.8"
```

### Comparing `dlt-0.2.9/setup.py` & `dlt-0.2.9a0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,14 @@
  'dlt.common.runtime',
  'dlt.common.schema',
  'dlt.common.storages',
  'dlt.destinations',
  'dlt.destinations.bigquery',
  'dlt.destinations.duckdb',
  'dlt.destinations.dummy',
- 'dlt.destinations.filesystem',
  'dlt.destinations.postgres',
  'dlt.destinations.redshift',
  'dlt.extract',
  'dlt.helpers',
  'dlt.helpers.dbt',
  'dlt.load',
  'dlt.normalize',
@@ -46,15 +45,14 @@
  'SQLAlchemy>=1.4.0',
  'astunparse>=1.6.3',
  'asyncstdlib>=3.10.5',
  'cachetools>=5.2.0',
  'click>=7.1',
  'cron-descriptor>=1.2.32',
  'deprecated>=1.2.13,<2.0.0',
- 'fsspec>=2023.5.0,<2024.0.0',
  'gitpython>=3.1.29',
  'giturlparse>=0.10.0',
  'hexbytes>=0.2.2',
  'humanize>=4.4.0',
  'json-logging==1.4.1rc0',
  'jsonpath-ng>=1.5.3,<2.0.0',
  'makefun>=1.15.0',
@@ -74,39 +72,32 @@
  'typing-extensions>=4.0.0',
  'tzdata>=2022.1']
 
 extras_require = \
 {':platform_python_implementation != "PyPy"': ['orjson>=3.8.6,<4.0.0'],
  'bigquery': ['grpcio>=1.50.0',
               'google-cloud-bigquery>=2.26.0',
-              'pyarrow>=8.0.0',
-              'gcsfs>=2023.5.0,<2024.0.0'],
+              'pyarrow>=8.0.0'],
  'dbt': ['dbt-core>=1.3.0,<1.5.0',
          'dbt-redshift>=1.3.0,<1.5.0',
          'dbt-bigquery>=1.3.0,<1.5.0',
          'dbt-duckdb>=1.3.0,<1.5.0'],
  'duckdb': ['duckdb>=0.6.1,<0.9.0'],
- 'filesystem': ['s3fs>=2023.5.0,<2024.0.0', 'boto3>=1.26'],
- 'gcp': ['grpcio>=1.50.0',
-         'google-cloud-bigquery>=2.26.0',
-         'pyarrow>=8.0.0',
-         'gcsfs>=2023.5.0,<2024.0.0'],
- 'gs': ['gcsfs>=2023.5.0,<2024.0.0'],
+ 'gcp': ['grpcio>=1.50.0', 'google-cloud-bigquery>=2.26.0', 'pyarrow>=8.0.0'],
  'postgres': ['psycopg2-binary>=2.9.1'],
  'postgres:platform_python_implementation == "PyPy"': ['psycopg2cffi>=2.9.0'],
  'redshift': ['psycopg2-binary>=2.9.1'],
- 'redshift:platform_python_implementation == "PyPy"': ['psycopg2cffi>=2.9.0'],
- 's3': ['s3fs>=2023.5.0,<2024.0.0', 'boto3>=1.26']}
+ 'redshift:platform_python_implementation == "PyPy"': ['psycopg2cffi>=2.9.0']}
 
 entry_points = \
 {'console_scripts': ['dlt = dlt.cli._dlt:_main']}
 
 setup_kwargs = {
     'name': 'dlt',
-    'version': '0.2.9',
+    'version': '0.2.9a0',
     'description': 'DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run.',
     'long_description': '<h1 align="center">\n    <strong>data load tool (dlt) — the open-source Python library for data loading</strong>\n</h1>\n<p align="center">\nBe it a Google Colab notebook, AWS Lambda function, an Airflow DAG, your local laptop,<br/>or a GPT-4 assisted development playground—<strong>dlt</strong> can be dropped in anywhere.\n</p>\n\n<div align="center">\n  <a target="_blank" href="https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g" style="background:none">\n    <img src="https://img.shields.io/badge/slack-join-dlt.svg?labelColor=191937&color=6F6FF7&logo=slack" />\n  </a>\n  <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">\n    <img src="https://img.shields.io/pypi/v/dlt?labelColor=191937&color=6F6FF7">\n  </a>\n  <a target="_blank" href="https://pypi.org/project/dlt/" style="background:none">\n    <img src="https://img.shields.io/pypi/pyversions/dlt?labelColor=191937&color=6F6FF7">\n  </a>\n</div>\n\n## Installation\n\ndlt supports Python 3.8+.\n\n```bash\npip install dlt\n```\n\n## Quick Start\n\nLoad chess game data from chess.com API and save it in DuckDB:\n\n```python\nimport dlt\nfrom chess import chess # a utility function that grabs data from the chess.com API\n\n# create a dlt pipeline that will load chess game data to the DuckDB destination\npipeline = dlt.pipeline(\n    pipeline_name=\'chess_pipeline\',\n    destination=\'duckdb\',\n    dataset_name=\'games_data\'\n)\n\n# use chess.com API to grab data about a few players\ndata = chess([\'magnuscarlsen\', \'rpragchess\'], start_month=\'2022/11\', end_month=\'2022/12\')\n\n# extract, normalize, and load the data\npipeline.run(data)\n```\n\nTry it out in our **[Colab Demo](https://colab.research.google.com/drive/1NfSB1DpwbbHX9_t5vlalBTf13utwpMGx?usp=sharing)**\n\n## Features\n\n- **Automatic Schema:** Data structure inspection and schema creation for the destination.\n- **Data Normalization:** Consistent and verified data before loading.\n- **Seamless Integration:** Colab, AWS Lambda, Airflow, and local environments.\n- **Scalable:** Adapts to growing data needs in production.\n- **Easy Maintenance:** Clear data pipeline structure for updates.\n- **Rapid Exploration:** Quickly explore and gain insights from new data sources.\n- **Versatile Usage:** Suitable for ad-hoc exploration to advanced loading infrastructures.\n- **Start in Seconds with CLI:** Powerful CLI for managing, deploying and inspecting local pipelines.\n- **Incremental Loading:** Load only new or changed data and avoid loading old records again.\n- **Open Source:** Free and Apache 2.0 Licensed.\n\n## Ready to use Pipelines and Destinations\n\nExplore ready to use pipelines (e.g. Google Sheets) in the [Pipelines docs](https://dlthub.com/docs/pipelines/chess) and supported destinations (e.g. DuckDB) in the [Destinations docs](https://dlthub.com/docs/destinations/bigquery).\n\n## Documentation\n\nFor detailed usage and configuration, please refer to the [official documentation](https://dlthub.com/docs).\n\n## Examples\n\nYou can find examples for various use cases in the [examples](docs/examples) folder.\n\n## Get Involved\n\nThe dlt project is quickly growing, and we\'re excited to have you join our community! Here\'s how you can get involved:\n\n- **Connect with the Community**: Join other dlt users and contributors on our [Slack](https://join.slack.com/t/dlthub-community/shared_invite/zt-1slox199h-HAE7EQoXmstkP_bTqal65g)\n- **Report issues and suggest features**: Please use the [GitHub Issues](https://github.com/dlt-hub/dlt/issues) to report bugs or suggest new features. Before creating a new issue, make sure to search the tracker for possible duplicates and add a comment if you find one.\n- **Contribute Pipelines**: Pipelines are data processing steps that help move and transform data between various sources and destinations. Contribute your custom pipelines to the [dlt-hub/pipelines](https://github.com/dlt-hub/pipelines) to help other folks in handling their data tasks.\n- **Contribute code**: Check out our [contributing guidelines](CONTRIBUTING.md) for information on how to make a pull request.\n- **Improve documentation**: Help us enhance the dlt documentation.\n\n## License\n\nDLT is released under the [Apache 2.0 License](LICENSE.txt).\n',
     'author': 'dltHub Inc.',
     'author_email': 'services@dlthub.com',
     'maintainer': 'Marcin Rudolf',
     'maintainer_email': 'marcin@dlthub.com',
     'url': 'https://github.com/dlt-hub',
```

### Comparing `dlt-0.2.9/PKG-INFO` & `dlt-0.2.9a0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlt
-Version: 0.2.9
+Version: 0.2.9a0
 Summary: DLT is an open-source python-native scalable data loading framework that does not require any devops efforts to run.
 Home-page: https://github.com/dlt-hub
 License: Apache-2.0
 Keywords: etl
 Author: dltHub Inc.
 Author-email: services@dlthub.com
 Maintainer: Marcin Rudolf
@@ -20,36 +20,30 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: bigquery
 Provides-Extra: dbt
 Provides-Extra: duckdb
-Provides-Extra: filesystem
 Provides-Extra: gcp
-Provides-Extra: gs
 Provides-Extra: postgres
 Provides-Extra: redshift
-Provides-Extra: s3
 Requires-Dist: PyYAML (>=5.4.1)
 Requires-Dist: SQLAlchemy (>=1.4.0)
 Requires-Dist: astunparse (>=1.6.3)
 Requires-Dist: asyncstdlib (>=3.10.5)
-Requires-Dist: boto3 (>=1.26); extra == "filesystem" or extra == "s3"
 Requires-Dist: cachetools (>=5.2.0)
 Requires-Dist: click (>=7.1)
 Requires-Dist: cron-descriptor (>=1.2.32)
 Requires-Dist: dbt-bigquery (>=1.3.0,<1.5.0); extra == "dbt"
 Requires-Dist: dbt-core (>=1.3.0,<1.5.0); extra == "dbt"
 Requires-Dist: dbt-duckdb (>=1.3.0,<1.5.0); extra == "dbt"
 Requires-Dist: dbt-redshift (>=1.3.0,<1.5.0); extra == "dbt"
 Requires-Dist: deprecated (>=1.2.13,<2.0.0)
 Requires-Dist: duckdb (>=0.6.1,<0.9.0); extra == "duckdb"
-Requires-Dist: fsspec (>=2023.5.0,<2024.0.0)
-Requires-Dist: gcsfs (>=2023.5.0,<2024.0.0); extra == "gcp" or extra == "bigquery" or extra == "gs"
 Requires-Dist: gitpython (>=3.1.29)
 Requires-Dist: giturlparse (>=0.10.0)
 Requires-Dist: google-cloud-bigquery (>=2.26.0); extra == "gcp" or extra == "bigquery"
 Requires-Dist: grpcio (>=1.50.0); extra == "gcp" or extra == "bigquery"
 Requires-Dist: hexbytes (>=0.2.2)
 Requires-Dist: humanize (>=4.4.0)
 Requires-Dist: json-logging (==1.4.1rc0)
@@ -62,15 +56,14 @@
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.1); extra == "postgres" or extra == "redshift"
 Requires-Dist: psycopg2cffi (>=2.9.0); (platform_python_implementation == "PyPy") and (extra == "postgres" or extra == "redshift")
 Requires-Dist: pyarrow (>=8.0.0); extra == "gcp" or extra == "bigquery"
 Requires-Dist: pytz (>=2022.6)
 Requires-Dist: requests (>=2.26.0)
 Requires-Dist: requirements-parser (>=0.5.0)
-Requires-Dist: s3fs (>=2023.5.0,<2024.0.0); extra == "filesystem" or extra == "s3"
 Requires-Dist: semver (>=2.13.0)
 Requires-Dist: sentry-sdk (>=1.4.3)
 Requires-Dist: setuptools (>=65.6.0)
 Requires-Dist: simplejson (>=3.17.5)
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Requires-Dist: tomlkit (>=0.11.3)
 Requires-Dist: typing-extensions (>=4.0.0)
```

