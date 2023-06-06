# Comparing `tmp/toolsql-0.5.3.tar.gz` & `tmp/toolsql-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolsql-0.5.3.tar", last modified: Sat May 27 22:44:13 2023, max compression
+gzip compressed data, was "toolsql-0.6.0.tar", last modified: Tue Jun  6 00:14:34 2023, max compression
```

## Comparing `toolsql-0.5.3.tar` & `toolsql-0.6.0.tar`

### file list

```diff
@@ -1,92 +1,92 @@
--rw-r--r--   0        0        0       97 2023-01-27 20:52:41.456006 toolsql-0.5.3/.gitignore
--rw-r--r--   0        0        0     1084 2022-12-07 18:42:43.242114 toolsql-0.5.3/LICENSE
--rw-r--r--   0        0        0     4659 2023-04-11 15:37:42.827266 toolsql-0.5.3/README.md
--rw-r--r--   0        0        0        0 2022-12-07 18:42:43.251690 toolsql-0.5.3/py.typed
--rw-r--r--   0        0        0      649 2023-04-15 22:58:00.373193 toolsql-0.5.3/pyproject.toml
--rw-r--r--   0        0        0      263 2023-01-21 18:52:09.694776 toolsql-0.5.3/tests/README.md
--rw-r--r--   0        0        0        0 2023-01-22 21:52:27.654376 toolsql-0.5.3/tests/conf/__init__.py
--rw-r--r--   0        0        0     1670 2023-01-28 01:59:10.345388 toolsql-0.5.3/tests/conf/conf_db_configs.py
--rw-r--r--   0        0        0     2120 2023-04-15 22:57:06.210871 toolsql-0.5.3/tests/conf/conf_helpers.py
--rw-r--r--   0        0        0     8392 2023-03-01 01:29:02.029340 toolsql-0.5.3/tests/conf/conf_tables.py
--rw-r--r--   0        0        0       62 2023-01-22 21:48:58.241419 toolsql-0.5.3/tests/conf/conf_write_queries.py
--rw-r--r--   0        0        0     4511 2023-02-03 00:06:54.451338 toolsql-0.5.3/tests/conftest.py
--rw-r--r--   0        0        0     2432 2023-03-05 03:27:04.199101 toolsql-0.5.3/tests/test_aggregations.py
--rw-r--r--   0        0        0     2220 2023-02-13 08:03:37.896687 toolsql-0.5.3/tests/test_column_expressions.py
--rw-r--r--   0        0        0     2084 2023-03-01 07:37:14.269608 toolsql-0.5.3/tests/test_dbms_metadata.py
--rw-r--r--   0        0        0     5206 2023-03-05 03:26:24.446611 toolsql-0.5.3/tests/test_delete.py
--rw-r--r--   0        0        0     2526 2023-03-05 07:24:19.484344 toolsql-0.5.3/tests/test_exceptions.py
--rw-r--r--   0        0        0    14606 2023-03-05 04:37:15.341481 toolsql-0.5.3/tests/test_insert.py
--rw-r--r--   0        0        0     1242 2023-03-01 07:35:46.632270 toolsql-0.5.3/tests/test_multicolumn_indices.py
--rw-r--r--   0        0        0     1075 2023-03-05 03:27:08.232652 toolsql-0.5.3/tests/test_renaming_results.py
--rw-r--r--   0        0        0    12107 2023-03-05 03:28:04.000994 toolsql-0.5.3/tests/test_select.py
--rw-r--r--   0        0        0     2003 2023-02-12 01:16:45.228226 toolsql-0.5.3/tests/test_summary.py
--rw-r--r--   0        0        0     8908 2023-03-06 02:50:19.508898 toolsql-0.5.3/tests/test_transactions.py
--rw-r--r--   0        0        0     3478 2023-03-05 03:30:56.862706 toolsql-0.5.3/tests/test_update.py
--rw-r--r--   0        0        0      233 2023-05-27 22:42:22.514459 toolsql-0.5.3/toolsql/__init__.py
--rw-r--r--   0        0        0       51 2023-04-11 15:27:03.745564 toolsql-0.5.3/toolsql/dbs/__init__.py
--rw-r--r--   0        0        0        1 2023-01-25 07:09:40.611833 toolsql-0.5.3/toolsql/dbs/db_classes/__init__.py
--rw-r--r--   0        0        0     4877 2023-04-12 01:43:17.868464 toolsql-0.5.3/toolsql/dbs/db_classes/abstract_db.py
--rw-r--r--   0        0        0    19071 2023-04-27 21:02:35.060364 toolsql-0.5.3/toolsql/dbs/db_classes/postgresql_db.py
--rw-r--r--   0        0        0     9559 2023-04-27 20:53:47.906206 toolsql-0.5.3/toolsql/dbs/db_classes/sqlite_db.py
--rw-r--r--   0        0        0     1251 2023-02-12 00:58:17.129402 toolsql-0.5.3/toolsql/dbs/db_utils.py
--rw-r--r--   0        0        0      920 2023-04-27 20:38:29.627687 toolsql-0.5.3/toolsql/dbs/login_utils.py
--rw-r--r--   0        0        0       84 2023-01-30 03:42:00.561041 toolsql-0.5.3/toolsql/drivers/__init__.py
--rw-r--r--   0        0        0      149 2023-02-02 22:58:21.072982 toolsql-0.5.3/toolsql/drivers/conn_utils/__init__.py
--rw-r--r--   0        0        0     1618 2023-03-19 18:55:10.095445 toolsql-0.5.3/toolsql/drivers/conn_utils/conn_attributes.py
--rw-r--r--   0        0        0     1986 2023-04-12 00:38:59.125862 toolsql-0.5.3/toolsql/drivers/conn_utils/connect_utils.py
--rw-r--r--   0        0        0      953 2023-02-03 05:07:04.778141 toolsql-0.5.3/toolsql/drivers/conn_utils/db_config_utils.py
--rw-r--r--   0        0        0     4853 2023-03-06 02:50:00.401901 toolsql-0.5.3/toolsql/drivers/conn_utils/transaction_utils.py
--rw-r--r--   0        0        0     1833 2023-03-27 19:30:33.769865 toolsql-0.5.3/toolsql/drivers/conn_utils/uri_utils.py
--rw-r--r--   0        0        0        0 2023-01-19 23:23:14.797191 toolsql-0.5.3/toolsql/drivers/driver_classes/__init__.py
--rw-r--r--   0        0        0     3437 2023-04-11 15:48:57.844239 toolsql-0.5.3/toolsql/drivers/driver_classes/abstract_driver.py
--rw-r--r--   0        0        0     1686 2023-03-22 00:04:08.425756 toolsql-0.5.3/toolsql/drivers/driver_classes/aiosqlite_driver.py
--rw-r--r--   0        0        0     7509 2023-05-27 22:41:16.199157 toolsql-0.5.3/toolsql/drivers/driver_classes/connectorx_driver.py
--rw-r--r--   0        0        0     4133 2023-04-11 15:55:51.938956 toolsql-0.5.3/toolsql/drivers/driver_classes/dbapi_driver.py
--rw-r--r--   0        0        0     3878 2023-03-27 19:32:22.818512 toolsql-0.5.3/toolsql/drivers/driver_classes/psycopg_driver.py
--rw-r--r--   0        0        0     2290 2023-03-22 00:03:41.799839 toolsql-0.5.3/toolsql/drivers/driver_classes/sqlite3_driver.py
--rw-r--r--   0        0        0     3968 2023-02-11 22:48:18.364943 toolsql-0.5.3/toolsql/drivers/driver_utils.py
--rw-r--r--   0        0        0       92 2023-02-03 19:35:08.076396 toolsql-0.5.3/toolsql/executors/__init__.py
--rw-r--r--   0        0        0      127 2023-01-30 03:14:58.462588 toolsql-0.5.3/toolsql/executors/ddl_executors/__init__.py
--rw-r--r--   0        0        0     2153 2023-02-01 21:30:22.128642 toolsql-0.5.3/toolsql/executors/ddl_executors/alter_executors.py
--rw-r--r--   0        0        0     2504 2023-04-27 01:37:34.473367 toolsql-0.5.3/toolsql/executors/ddl_executors/create_executors.py
--rw-r--r--   0        0        0     1153 2023-03-28 18:19:02.990162 toolsql-0.5.3/toolsql/executors/ddl_executors/drop_executors.py
--rw-r--r--   0        0        0     4105 2023-04-12 01:56:12.421844 toolsql-0.5.3/toolsql/executors/ddl_executors/metadata_executors.py
--rw-r--r--   0        0        0      128 2023-01-30 03:15:43.131090 toolsql-0.5.3/toolsql/executors/dml_executors/__init__.py
--rw-r--r--   0        0        0     2584 2023-03-28 19:49:02.476403 toolsql-0.5.3/toolsql/executors/dml_executors/delete_executors.py
--rw-r--r--   0        0        0     3409 2023-03-21 23:26:17.745727 toolsql-0.5.3/toolsql/executors/dml_executors/insert_executors.py
--rw-r--r--   0        0        0    19646 2023-05-27 22:33:57.076215 toolsql-0.5.3/toolsql/executors/dml_executors/select_executors.py
--rw-r--r--   0        0        0     2843 2023-02-12 04:21:29.361650 toolsql-0.5.3/toolsql/executors/dml_executors/update_executors.py
--rw-r--r--   0        0        0       59 2023-02-26 07:01:46.454118 toolsql-0.5.3/toolsql/executors/summary_executors/__init__.py
--rw-r--r--   0        0        0     3424 2023-03-28 18:23:04.706576 toolsql-0.5.3/toolsql/executors/summary_executors/summary_prints.py
--rw-r--r--   0        0        0     2201 2023-02-12 02:23:37.024146 toolsql-0.5.3/toolsql/executors/summary_executors/summary_usage.py
--rw-r--r--   0        0        0      102 2023-02-26 22:29:04.008347 toolsql-0.5.3/toolsql/formats/__init__.py
--rw-r--r--   0        0        0     4144 2023-04-11 15:35:31.235749 toolsql-0.5.3/toolsql/formats/encoding_format_utils.py
--rw-r--r--   0        0        0     2045 2023-04-11 15:35:17.654255 toolsql-0.5.3/toolsql/formats/json_format_utils.py
--rw-r--r--   0        0        0     5533 2023-04-11 15:35:06.683633 toolsql-0.5.3/toolsql/formats/row_format_utils.py
--rw-r--r--   0        0        0        0 2023-02-01 00:04:45.871374 toolsql-0.5.3/toolsql/py.typed
--rw-r--r--   0        0        0       61 2023-01-27 04:00:11.947543 toolsql-0.5.3/toolsql/schemas/__init__.py
--rw-r--r--   0        0        0     4240 2023-02-26 21:30:57.707911 toolsql-0.5.3/toolsql/schemas/datatype_utils.py
--rw-r--r--   0        0        0     5576 2023-04-27 20:46:22.127450 toolsql-0.5.3/toolsql/schemas/shorthand_utils.py
--rw-r--r--   0        0        0      147 2023-03-05 04:53:25.455675 toolsql-0.5.3/toolsql/spec/__init__.py
--rw-r--r--   0        0        0     1184 2023-03-05 07:23:00.086051 toolsql-0.5.3/toolsql/spec/exceptions.py
--rw-r--r--   0        0        0     2130 2023-03-06 07:52:30.415917 toolsql-0.5.3/toolsql/spec/typedata.py
--rw-r--r--   0        0        0      148 2023-03-27 21:12:23.119118 toolsql-0.5.3/toolsql/spec/typedefs/__init__.py
--rw-r--r--   0        0        0      234 2023-01-25 21:23:06.637935 toolsql-0.5.3/toolsql/spec/typedefs/dataset_types.py
--rw-r--r--   0        0        0     1504 2023-02-12 00:16:22.417559 toolsql-0.5.3/toolsql/spec/typedefs/driver_types.py
--rw-r--r--   0        0        0      109 2023-03-27 20:31:11.573302 toolsql-0.5.3/toolsql/spec/typedefs/permission_types.py
--rw-r--r--   0        0        0     4031 2023-04-27 20:45:29.560935 toolsql-0.5.3/toolsql/spec/typedefs/schema_types.py
--rw-r--r--   0        0        0     5568 2023-04-11 15:36:02.595008 toolsql-0.5.3/toolsql/spec/typedefs/statement_types.py
--rw-r--r--   0        0        0     2645 2023-04-11 15:34:42.673529 toolsql-0.5.3/toolsql/spec/typeguards.py
--rw-r--r--   0        0        0      125 2023-02-03 22:03:30.312085 toolsql-0.5.3/toolsql/statements/__init__.py
--rw-r--r--   0        0        0       96 2023-01-30 01:01:07.284310 toolsql-0.5.3/toolsql/statements/ddl_statements/__init__.py
--rw-r--r--   0        0        0     2631 2023-02-01 20:55:53.683307 toolsql-0.5.3/toolsql/statements/ddl_statements/alter_statements.py
--rw-r--r--   0        0        0     8586 2023-04-27 20:52:25.616132 toolsql-0.5.3/toolsql/statements/ddl_statements/create_statements.py
--rw-r--r--   0        0        0      636 2023-02-01 20:52:53.962533 toolsql-0.5.3/toolsql/statements/ddl_statements/drop_statements.py
--rw-r--r--   0        0        0      132 2023-01-30 01:01:54.106030 toolsql-0.5.3/toolsql/statements/dml_statements/__init__.py
--rw-r--r--   0        0        0     1712 2023-02-13 08:35:53.659371 toolsql-0.5.3/toolsql/statements/dml_statements/delete_statements.py
--rw-r--r--   0        0        0     6978 2023-02-27 06:35:28.865971 toolsql-0.5.3/toolsql/statements/dml_statements/insert_statements.py
--rw-r--r--   0        0        0     4472 2023-02-13 08:35:08.066374 toolsql-0.5.3/toolsql/statements/dml_statements/select_statements.py
--rw-r--r--   0        0        0     3280 2023-02-13 08:35:26.310154 toolsql-0.5.3/toolsql/statements/dml_statements/update_statements.py
--rw-r--r--   0        0        0    13253 2023-04-27 05:59:35.674096 toolsql-0.5.3/toolsql/statements/statement_utils.py
--rw-r--r--   0        0        0     1509 2023-02-04 01:31:44.402064 toolsql-0.5.3/toolsql/statements/summary_statements.py
--rw-r--r--   0        0        0     5088 1970-01-01 00:00:00.000000 toolsql-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0       97 2023-01-27 20:52:41.456006 toolsql-0.6.0/.gitignore
+-rw-r--r--   0        0        0     1084 2022-12-07 18:42:43.242114 toolsql-0.6.0/LICENSE
+-rw-r--r--   0        0        0     4659 2023-04-11 15:37:42.827266 toolsql-0.6.0/README.md
+-rw-r--r--   0        0        0        0 2022-12-07 18:42:43.251690 toolsql-0.6.0/py.typed
+-rw-r--r--   0        0        0      641 2023-06-06 00:10:10.812770 toolsql-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      263 2023-01-21 18:52:09.694776 toolsql-0.6.0/tests/README.md
+-rw-r--r--   0        0        0        0 2023-01-22 21:52:27.654376 toolsql-0.6.0/tests/conf/__init__.py
+-rw-r--r--   0        0        0     1670 2023-01-28 01:59:10.345388 toolsql-0.6.0/tests/conf/conf_db_configs.py
+-rw-r--r--   0        0        0     2120 2023-04-15 22:57:06.210871 toolsql-0.6.0/tests/conf/conf_helpers.py
+-rw-r--r--   0        0        0     8392 2023-03-01 01:29:02.029340 toolsql-0.6.0/tests/conf/conf_tables.py
+-rw-r--r--   0        0        0       62 2023-01-22 21:48:58.241419 toolsql-0.6.0/tests/conf/conf_write_queries.py
+-rw-r--r--   0        0        0     4511 2023-02-03 00:06:54.451338 toolsql-0.6.0/tests/conftest.py
+-rw-r--r--   0        0        0     2432 2023-03-05 03:27:04.199101 toolsql-0.6.0/tests/test_aggregations.py
+-rw-r--r--   0        0        0     2220 2023-02-13 08:03:37.896687 toolsql-0.6.0/tests/test_column_expressions.py
+-rw-r--r--   0        0        0     2084 2023-03-01 07:37:14.269608 toolsql-0.6.0/tests/test_dbms_metadata.py
+-rw-r--r--   0        0        0     5206 2023-03-05 03:26:24.446611 toolsql-0.6.0/tests/test_delete.py
+-rw-r--r--   0        0        0     2526 2023-03-05 07:24:19.484344 toolsql-0.6.0/tests/test_exceptions.py
+-rw-r--r--   0        0        0    14606 2023-03-05 04:37:15.341481 toolsql-0.6.0/tests/test_insert.py
+-rw-r--r--   0        0        0     1242 2023-03-01 07:35:46.632270 toolsql-0.6.0/tests/test_multicolumn_indices.py
+-rw-r--r--   0        0        0     1075 2023-03-05 03:27:08.232652 toolsql-0.6.0/tests/test_renaming_results.py
+-rw-r--r--   0        0        0    12107 2023-03-05 03:28:04.000994 toolsql-0.6.0/tests/test_select.py
+-rw-r--r--   0        0        0     2003 2023-02-12 01:16:45.228226 toolsql-0.6.0/tests/test_summary.py
+-rw-r--r--   0        0        0     8908 2023-03-06 02:50:19.508898 toolsql-0.6.0/tests/test_transactions.py
+-rw-r--r--   0        0        0     3478 2023-03-05 03:30:56.862706 toolsql-0.6.0/tests/test_update.py
+-rw-r--r--   0        0        0      233 2023-06-06 00:11:05.007551 toolsql-0.6.0/toolsql/__init__.py
+-rw-r--r--   0        0        0       51 2023-04-11 15:27:03.745564 toolsql-0.6.0/toolsql/dbs/__init__.py
+-rw-r--r--   0        0        0        1 2023-01-25 07:09:40.611833 toolsql-0.6.0/toolsql/dbs/db_classes/__init__.py
+-rw-r--r--   0        0        0     4877 2023-04-12 01:43:17.868464 toolsql-0.6.0/toolsql/dbs/db_classes/abstract_db.py
+-rw-r--r--   0        0        0    19071 2023-04-27 21:02:35.060364 toolsql-0.6.0/toolsql/dbs/db_classes/postgresql_db.py
+-rw-r--r--   0        0        0     9559 2023-04-27 20:53:47.906206 toolsql-0.6.0/toolsql/dbs/db_classes/sqlite_db.py
+-rw-r--r--   0        0        0     1251 2023-02-12 00:58:17.129402 toolsql-0.6.0/toolsql/dbs/db_utils.py
+-rw-r--r--   0        0        0      920 2023-04-27 20:38:29.627687 toolsql-0.6.0/toolsql/dbs/login_utils.py
+-rw-r--r--   0        0        0       84 2023-01-30 03:42:00.561041 toolsql-0.6.0/toolsql/drivers/__init__.py
+-rw-r--r--   0        0        0      149 2023-02-02 22:58:21.072982 toolsql-0.6.0/toolsql/drivers/conn_utils/__init__.py
+-rw-r--r--   0        0        0     1618 2023-03-19 18:55:10.095445 toolsql-0.6.0/toolsql/drivers/conn_utils/conn_attributes.py
+-rw-r--r--   0        0        0     1986 2023-04-12 00:38:59.125862 toolsql-0.6.0/toolsql/drivers/conn_utils/connect_utils.py
+-rw-r--r--   0        0        0      953 2023-02-03 05:07:04.778141 toolsql-0.6.0/toolsql/drivers/conn_utils/db_config_utils.py
+-rw-r--r--   0        0        0     4853 2023-03-06 02:50:00.401901 toolsql-0.6.0/toolsql/drivers/conn_utils/transaction_utils.py
+-rw-r--r--   0        0        0     1833 2023-03-27 19:30:33.769865 toolsql-0.6.0/toolsql/drivers/conn_utils/uri_utils.py
+-rw-r--r--   0        0        0        0 2023-01-19 23:23:14.797191 toolsql-0.6.0/toolsql/drivers/driver_classes/__init__.py
+-rw-r--r--   0        0        0     3437 2023-04-11 15:48:57.844239 toolsql-0.6.0/toolsql/drivers/driver_classes/abstract_driver.py
+-rw-r--r--   0        0        0     1686 2023-03-22 00:04:08.425756 toolsql-0.6.0/toolsql/drivers/driver_classes/aiosqlite_driver.py
+-rw-r--r--   0        0        0     7509 2023-05-27 22:41:16.199157 toolsql-0.6.0/toolsql/drivers/driver_classes/connectorx_driver.py
+-rw-r--r--   0        0        0     4133 2023-04-11 15:55:51.938956 toolsql-0.6.0/toolsql/drivers/driver_classes/dbapi_driver.py
+-rw-r--r--   0        0        0     3878 2023-03-27 19:32:22.818512 toolsql-0.6.0/toolsql/drivers/driver_classes/psycopg_driver.py
+-rw-r--r--   0        0        0     2290 2023-03-22 00:03:41.799839 toolsql-0.6.0/toolsql/drivers/driver_classes/sqlite3_driver.py
+-rw-r--r--   0        0        0     3968 2023-02-11 22:48:18.364943 toolsql-0.6.0/toolsql/drivers/driver_utils.py
+-rw-r--r--   0        0        0       92 2023-02-03 19:35:08.076396 toolsql-0.6.0/toolsql/executors/__init__.py
+-rw-r--r--   0        0        0      127 2023-01-30 03:14:58.462588 toolsql-0.6.0/toolsql/executors/ddl_executors/__init__.py
+-rw-r--r--   0        0        0     2153 2023-02-01 21:30:22.128642 toolsql-0.6.0/toolsql/executors/ddl_executors/alter_executors.py
+-rw-r--r--   0        0        0     2504 2023-04-27 01:37:34.473367 toolsql-0.6.0/toolsql/executors/ddl_executors/create_executors.py
+-rw-r--r--   0        0        0     1153 2023-03-28 18:19:02.990162 toolsql-0.6.0/toolsql/executors/ddl_executors/drop_executors.py
+-rw-r--r--   0        0        0     4105 2023-04-12 01:56:12.421844 toolsql-0.6.0/toolsql/executors/ddl_executors/metadata_executors.py
+-rw-r--r--   0        0        0      128 2023-01-30 03:15:43.131090 toolsql-0.6.0/toolsql/executors/dml_executors/__init__.py
+-rw-r--r--   0        0        0     2584 2023-03-28 19:49:02.476403 toolsql-0.6.0/toolsql/executors/dml_executors/delete_executors.py
+-rw-r--r--   0        0        0     3409 2023-03-21 23:26:17.745727 toolsql-0.6.0/toolsql/executors/dml_executors/insert_executors.py
+-rw-r--r--   0        0        0    19646 2023-05-27 22:33:57.076215 toolsql-0.6.0/toolsql/executors/dml_executors/select_executors.py
+-rw-r--r--   0        0        0     2843 2023-02-12 04:21:29.361650 toolsql-0.6.0/toolsql/executors/dml_executors/update_executors.py
+-rw-r--r--   0        0        0       59 2023-02-26 07:01:46.454118 toolsql-0.6.0/toolsql/executors/summary_executors/__init__.py
+-rw-r--r--   0        0        0     3424 2023-03-28 18:23:04.706576 toolsql-0.6.0/toolsql/executors/summary_executors/summary_prints.py
+-rw-r--r--   0        0        0     2201 2023-02-12 02:23:37.024146 toolsql-0.6.0/toolsql/executors/summary_executors/summary_usage.py
+-rw-r--r--   0        0        0      102 2023-02-26 22:29:04.008347 toolsql-0.6.0/toolsql/formats/__init__.py
+-rw-r--r--   0        0        0     4144 2023-04-11 15:35:31.235749 toolsql-0.6.0/toolsql/formats/encoding_format_utils.py
+-rw-r--r--   0        0        0     2045 2023-04-11 15:35:17.654255 toolsql-0.6.0/toolsql/formats/json_format_utils.py
+-rw-r--r--   0        0        0     5533 2023-04-11 15:35:06.683633 toolsql-0.6.0/toolsql/formats/row_format_utils.py
+-rw-r--r--   0        0        0        0 2023-02-01 00:04:45.871374 toolsql-0.6.0/toolsql/py.typed
+-rw-r--r--   0        0        0       61 2023-01-27 04:00:11.947543 toolsql-0.6.0/toolsql/schemas/__init__.py
+-rw-r--r--   0        0        0     4240 2023-02-26 21:30:57.707911 toolsql-0.6.0/toolsql/schemas/datatype_utils.py
+-rw-r--r--   0        0        0     5576 2023-04-27 20:46:22.127450 toolsql-0.6.0/toolsql/schemas/shorthand_utils.py
+-rw-r--r--   0        0        0      147 2023-03-05 04:53:25.455675 toolsql-0.6.0/toolsql/spec/__init__.py
+-rw-r--r--   0        0        0     1184 2023-03-05 07:23:00.086051 toolsql-0.6.0/toolsql/spec/exceptions.py
+-rw-r--r--   0        0        0     2130 2023-03-06 07:52:30.415917 toolsql-0.6.0/toolsql/spec/typedata.py
+-rw-r--r--   0        0        0      148 2023-03-27 21:12:23.119118 toolsql-0.6.0/toolsql/spec/typedefs/__init__.py
+-rw-r--r--   0        0        0      234 2023-01-25 21:23:06.637935 toolsql-0.6.0/toolsql/spec/typedefs/dataset_types.py
+-rw-r--r--   0        0        0     1504 2023-02-12 00:16:22.417559 toolsql-0.6.0/toolsql/spec/typedefs/driver_types.py
+-rw-r--r--   0        0        0      109 2023-03-27 20:31:11.573302 toolsql-0.6.0/toolsql/spec/typedefs/permission_types.py
+-rw-r--r--   0        0        0     4031 2023-04-27 20:45:29.560935 toolsql-0.6.0/toolsql/spec/typedefs/schema_types.py
+-rw-r--r--   0        0        0     5568 2023-04-11 15:36:02.595008 toolsql-0.6.0/toolsql/spec/typedefs/statement_types.py
+-rw-r--r--   0        0        0     2645 2023-04-11 15:34:42.673529 toolsql-0.6.0/toolsql/spec/typeguards.py
+-rw-r--r--   0        0        0      125 2023-02-03 22:03:30.312085 toolsql-0.6.0/toolsql/statements/__init__.py
+-rw-r--r--   0        0        0       96 2023-01-30 01:01:07.284310 toolsql-0.6.0/toolsql/statements/ddl_statements/__init__.py
+-rw-r--r--   0        0        0     2631 2023-02-01 20:55:53.683307 toolsql-0.6.0/toolsql/statements/ddl_statements/alter_statements.py
+-rw-r--r--   0        0        0     8586 2023-04-27 20:52:25.616132 toolsql-0.6.0/toolsql/statements/ddl_statements/create_statements.py
+-rw-r--r--   0        0        0      636 2023-02-01 20:52:53.962533 toolsql-0.6.0/toolsql/statements/ddl_statements/drop_statements.py
+-rw-r--r--   0        0        0      132 2023-01-30 01:01:54.106030 toolsql-0.6.0/toolsql/statements/dml_statements/__init__.py
+-rw-r--r--   0        0        0     1712 2023-02-13 08:35:53.659371 toolsql-0.6.0/toolsql/statements/dml_statements/delete_statements.py
+-rw-r--r--   0        0        0     6978 2023-02-27 06:35:28.865971 toolsql-0.6.0/toolsql/statements/dml_statements/insert_statements.py
+-rw-r--r--   0        0        0     4472 2023-02-13 08:35:08.066374 toolsql-0.6.0/toolsql/statements/dml_statements/select_statements.py
+-rw-r--r--   0        0        0     3280 2023-02-13 08:35:26.310154 toolsql-0.6.0/toolsql/statements/dml_statements/update_statements.py
+-rw-r--r--   0        0        0    13253 2023-04-27 05:59:35.674096 toolsql-0.6.0/toolsql/statements/statement_utils.py
+-rw-r--r--   0        0        0     1509 2023-02-04 01:31:44.402064 toolsql-0.6.0/toolsql/statements/summary_statements.py
+-rw-r--r--   0        0        0     5080 1970-01-01 00:00:00.000000 toolsql-0.6.0/PKG-INFO
```

### Comparing `toolsql-0.5.3/LICENSE` & `toolsql-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/README.md` & `toolsql-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/pyproject.toml` & `toolsql-0.6.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 license = {file = "LICENSE"}
 dependencies = [
     "typing_extensions>=4.2.0",
     "toolstr >=0.9.1, <0.10",
     "polars >=0.17.2, <0.18",
     "aiosqlite >=0.18.0, <0.19",
     "psycopg >=3.1.8, <3.2",
-    "connectorx >=0.3.2a3, <0.3.3",
+    "connectorx ==0.3.2a5",
 ]
 
 [tool.mypy]
 python_version = "3.9"
 strict = true
 implicit_reexport = true
 files = ["toolsql"]
```

### Comparing `toolsql-0.5.3/tests/conf/conf_db_configs.py` & `toolsql-0.6.0/tests/conf/conf_db_configs.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/tests/conf/conf_helpers.py` & `toolsql-0.6.0/tests/conf/conf_helpers.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/tests/conf/conf_tables.py` & `toolsql-0.6.0/tests/conf/conf_tables.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/tests/conftest.py` & `toolsql-0.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/tests/test_aggregations.py` & `toolsql-0.6.0/tests/test_aggregations.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/tests/test_column_expressions.py` & `toolsql-0.6.0/tests/test_column_expressions.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/tests/test_dbms_metadata.py` & `toolsql-0.6.0/tests/test_dbms_metadata.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/tests/test_delete.py` & `toolsql-0.6.0/tests/test_delete.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/tests/test_exceptions.py` & `toolsql-0.6.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/tests/test_insert.py` & `toolsql-0.6.0/tests/test_insert.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/tests/test_multicolumn_indices.py` & `toolsql-0.6.0/tests/test_multicolumn_indices.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/tests/test_renaming_results.py` & `toolsql-0.6.0/tests/test_renaming_results.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/tests/test_select.py` & `toolsql-0.6.0/tests/test_select.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/tests/test_summary.py` & `toolsql-0.6.0/tests/test_summary.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/tests/test_transactions.py` & `toolsql-0.6.0/tests/test_transactions.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/tests/test_update.py` & `toolsql-0.6.0/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/dbs/db_classes/abstract_db.py` & `toolsql-0.6.0/toolsql/dbs/db_classes/abstract_db.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/dbs/db_classes/postgresql_db.py` & `toolsql-0.6.0/toolsql/dbs/db_classes/postgresql_db.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/dbs/db_classes/sqlite_db.py` & `toolsql-0.6.0/toolsql/dbs/db_classes/sqlite_db.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/dbs/db_utils.py` & `toolsql-0.6.0/toolsql/dbs/db_utils.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/dbs/login_utils.py` & `toolsql-0.6.0/toolsql/dbs/login_utils.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/drivers/conn_utils/conn_attributes.py` & `toolsql-0.6.0/toolsql/drivers/conn_utils/conn_attributes.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/drivers/conn_utils/connect_utils.py` & `toolsql-0.6.0/toolsql/drivers/conn_utils/connect_utils.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/drivers/conn_utils/db_config_utils.py` & `toolsql-0.6.0/toolsql/drivers/conn_utils/db_config_utils.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/drivers/conn_utils/transaction_utils.py` & `toolsql-0.6.0/toolsql/drivers/conn_utils/transaction_utils.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/drivers/conn_utils/uri_utils.py` & `toolsql-0.6.0/toolsql/drivers/conn_utils/uri_utils.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/drivers/driver_classes/abstract_driver.py` & `toolsql-0.6.0/toolsql/drivers/driver_classes/abstract_driver.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/drivers/driver_classes/aiosqlite_driver.py` & `toolsql-0.6.0/toolsql/drivers/driver_classes/aiosqlite_driver.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/drivers/driver_classes/connectorx_driver.py` & `toolsql-0.6.0/toolsql/drivers/driver_classes/connectorx_driver.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/drivers/driver_classes/dbapi_driver.py` & `toolsql-0.6.0/toolsql/drivers/driver_classes/dbapi_driver.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/drivers/driver_classes/psycopg_driver.py` & `toolsql-0.6.0/toolsql/drivers/driver_classes/psycopg_driver.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/drivers/driver_classes/sqlite3_driver.py` & `toolsql-0.6.0/toolsql/drivers/driver_classes/sqlite3_driver.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/drivers/driver_utils.py` & `toolsql-0.6.0/toolsql/drivers/driver_utils.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/executors/ddl_executors/alter_executors.py` & `toolsql-0.6.0/toolsql/executors/ddl_executors/alter_executors.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/executors/ddl_executors/create_executors.py` & `toolsql-0.6.0/toolsql/executors/ddl_executors/create_executors.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/executors/ddl_executors/drop_executors.py` & `toolsql-0.6.0/toolsql/executors/ddl_executors/drop_executors.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/executors/ddl_executors/metadata_executors.py` & `toolsql-0.6.0/toolsql/executors/ddl_executors/metadata_executors.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/executors/dml_executors/delete_executors.py` & `toolsql-0.6.0/toolsql/executors/dml_executors/delete_executors.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/executors/dml_executors/insert_executors.py` & `toolsql-0.6.0/toolsql/executors/dml_executors/insert_executors.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/executors/dml_executors/select_executors.py` & `toolsql-0.6.0/toolsql/executors/dml_executors/select_executors.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/executors/dml_executors/update_executors.py` & `toolsql-0.6.0/toolsql/executors/dml_executors/update_executors.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/executors/summary_executors/summary_prints.py` & `toolsql-0.6.0/toolsql/executors/summary_executors/summary_prints.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/executors/summary_executors/summary_usage.py` & `toolsql-0.6.0/toolsql/executors/summary_executors/summary_usage.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/formats/encoding_format_utils.py` & `toolsql-0.6.0/toolsql/formats/encoding_format_utils.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/formats/json_format_utils.py` & `toolsql-0.6.0/toolsql/formats/json_format_utils.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/formats/row_format_utils.py` & `toolsql-0.6.0/toolsql/formats/row_format_utils.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/schemas/datatype_utils.py` & `toolsql-0.6.0/toolsql/schemas/datatype_utils.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/schemas/shorthand_utils.py` & `toolsql-0.6.0/toolsql/schemas/shorthand_utils.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/spec/exceptions.py` & `toolsql-0.6.0/toolsql/spec/exceptions.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/spec/typedata.py` & `toolsql-0.6.0/toolsql/spec/typedata.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/spec/typedefs/driver_types.py` & `toolsql-0.6.0/toolsql/spec/typedefs/driver_types.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/spec/typedefs/schema_types.py` & `toolsql-0.6.0/toolsql/spec/typedefs/schema_types.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/spec/typedefs/statement_types.py` & `toolsql-0.6.0/toolsql/spec/typedefs/statement_types.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/spec/typeguards.py` & `toolsql-0.6.0/toolsql/spec/typeguards.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/statements/ddl_statements/alter_statements.py` & `toolsql-0.6.0/toolsql/statements/ddl_statements/alter_statements.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/statements/ddl_statements/create_statements.py` & `toolsql-0.6.0/toolsql/statements/ddl_statements/create_statements.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/statements/ddl_statements/drop_statements.py` & `toolsql-0.6.0/toolsql/statements/ddl_statements/drop_statements.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/statements/dml_statements/delete_statements.py` & `toolsql-0.6.0/toolsql/statements/dml_statements/delete_statements.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/statements/dml_statements/insert_statements.py` & `toolsql-0.6.0/toolsql/statements/dml_statements/insert_statements.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/statements/dml_statements/select_statements.py` & `toolsql-0.6.0/toolsql/statements/dml_statements/select_statements.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/statements/dml_statements/update_statements.py` & `toolsql-0.6.0/toolsql/statements/dml_statements/update_statements.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/statements/statement_utils.py` & `toolsql-0.6.0/toolsql/statements/statement_utils.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/toolsql/statements/summary_statements.py` & `toolsql-0.6.0/toolsql/statements/summary_statements.py`

 * *Files identical despite different names*

### Comparing `toolsql-0.5.3/PKG-INFO` & `toolsql-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: toolsql
-Version: 0.5.3
+Version: 0.6.0
 Summary: toolsql is an async+sync sql builder+executor for sqlite+postgres
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: typing_extensions>=4.2.0
 Requires-Dist: toolstr >=0.9.1, <0.10
 Requires-Dist: polars >=0.17.2, <0.18
 Requires-Dist: aiosqlite >=0.18.0, <0.19
 Requires-Dist: psycopg >=3.1.8, <3.2
-Requires-Dist: connectorx >=0.3.2a3, <0.3.3
+Requires-Dist: connectorx ==0.3.2a5
 
 # toolsql
 
 toolsql makes it easy to build sql queries and execute those queries
 
 toolsql's goals:
 - provide identical interfaces to sqlite + postgresql
```

