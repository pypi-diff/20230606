# Comparing `tmp/yyxx_game_pkg-2023.5.4.1.tar.gz` & `tmp/yyxx_game_pkg-2023.6.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yyxx_game_pkg-2023.5.4.1.tar", max compression
+gzip compressed data, was "yyxx_game_pkg-2023.6.6.1.tar", max compression
```

## Comparing `yyxx_game_pkg-2023.5.4.1.tar` & `yyxx_game_pkg-2023.6.6.1.tar`

### file list

```diff
@@ -1,89 +1,114 @@
--rw-r--r--   0        0        0     3888 2023-05-04 04:10:07.938087 yyxx_game_pkg-2023.5.4.1/README.md
--rw-r--r--   0        0        0     1170 2023-05-04 04:10:20.550173 yyxx_game_pkg-2023.5.4.1/pyproject.toml
--rw-r--r--   0        0        0       68 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/__init__.py
--rw-r--r--   0        0        0       83 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/dbops/__init__.py
--rw-r--r--   0        0        0     1341 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/dbops/mysql_op.py
--rw-r--r--   0        0        0       70 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/dispatch/__init__.py
--rw-r--r--   0        0        0       70 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/dispatch/config/__init__.py
--rw-r--r--   0        0        0     1228 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/dispatch/config/celery_local_config.py
--rw-r--r--   0        0        0      660 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/dispatch/rules/__init__.py
--rw-r--r--   0        0        0     1348 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/dispatch/rules/rule_temp.py
--rw-r--r--   0        0        0      580 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/dispatch/test_dispatch.py
--rw-r--r--   0        0        0       84 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/helpers/__init__.py
--rw-r--r--   0        0        0      522 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/helpers/test_mysql_helper.py
--rw-r--r--   0        0        0      455 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/helpers/test_pika_helper.py
--rw-r--r--   0        0        0      481 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/helpers/test_redis_helper.py
--rw-r--r--   0        0        0       70 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/submit/__init__.py
--rw-r--r--   0        0        0       70 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/submit/schedule_rule/__init__.py
--rw-r--r--   0        0        0       70 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/submit/schedule_rule/schedule/__init__.py
--rw-r--r--   0        0        0       70 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/submit/schedule_rule/schedule/statistic_task/__init__.py
--rw-r--r--   0        0        0      431 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/submit/schedule_rule/schedule/statistic_task/schedule_statistic_collect_test.py
--rw-r--r--   0        0        0      413 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/submit/schedule_rule/schedule/statistic_task/schedule_statistic_task_test.py
--rw-r--r--   0        0        0       70 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/submit/schedule_rule/schedule/work_flow/__init__.py
--rw-r--r--   0        0        0     1217 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/submit/schedule_rule/schedule/work_flow/schedule_work_flow_test.py
--rw-r--r--   0        0        0      305 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/submit/submit.json
--rw-r--r--   0        0        0     1250 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/submit/test_submit.py
--rw-r--r--   0        0        0      235 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/test_ip2region.py
--rw-r--r--   0        0        0      513 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/test_logger.py
--rw-r--r--   0        0        0      960 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/test_xtrace.py
--rw-r--r--   0        0        0       81 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/utils/__init__.py
--rw-r--r--   0        0        0       70 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/xcelery/__init__.py
--rw-r--r--   0        0        0       70 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/xcelery/config/__init__.py
--rw-r--r--   0        0        0     1226 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/xcelery/config/celery_local_config.py
--rw-r--r--   0        0        0      747 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/xcelery/task_register.py
--rw-r--r--   0        0        0      299 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/tests/xcelery/test_celery.py
--rw-r--r--   0        0        0       69 2023-05-04 04:10:07.942087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/__init__.py
--rw-r--r--   0        0        0       83 2023-05-04 04:10:07.946087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/__init__.py
--rw-r--r--   0        0        0     1331 2023-05-04 04:10:07.946087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/base.py
--rw-r--r--   0        0        0     1295 2023-05-04 04:10:07.946087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/ch_op.py
--rw-r--r--   0        0        0     5597 2023-05-04 04:10:07.946087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/das_api.py
--rw-r--r--   0        0        0     1911 2023-05-04 04:10:07.946087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/es_op.py
--rw-r--r--   0        0        0     1678 2023-05-04 04:10:07.946087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/hdfs_op.py
--rw-r--r--   0        0        0      979 2023-05-04 04:10:07.946087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/mongo_op.py
--rw-r--r--   0        0        0     3955 2023-05-04 04:10:07.946087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/mysql_op.py
--rw-r--r--   0        0        0       81 2023-05-04 04:10:07.946087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/helpers/__init__.py
--rw-r--r--   0        0        0     2408 2023-05-04 04:10:07.946087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/helpers/mysql_helper.py
--rw-r--r--   0        0        0     1266 2023-05-04 04:10:07.946087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/helpers/pika_helper.py
--rw-r--r--   0        0        0     2850 2023-05-04 04:10:07.946087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/helpers/redis_helper.py
--rw-r--r--   0        0        0       79 2023-05-04 04:10:07.946087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/ip2region/__init__.py
--rw-r--r--   0        0        0 11070130 2023-05-04 04:10:08.018087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/ip2region/ip2region.xdb
--rw-r--r--   0        0        0      604 2023-05-04 04:10:08.018087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/ip2region/ip_x.py
--rw-r--r--   0        0        0     5735 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/ip2region/xdbSearcher.py
--rw-r--r--   0        0        0       81 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/logger/__init__.py
--rw-r--r--   0        0        0     2326 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/logger/config.py
--rw-r--r--   0        0        0     3467 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/logger/handlers.py
--rw-r--r--   0        0        0     2154 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/logger/log.py
--rw-r--r--   0        0        0       70 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/__init__.py
--rw-r--r--   0        0        0       68 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/__init__.py
--rw-r--r--   0        0        0       70 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/common/__init__.py
--rw-r--r--   0        0        0     1514 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/common/common.py
--rw-r--r--   0        0        0       69 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/core/__init__.py
--rw-r--r--   0        0        0      805 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/core/manager.py
--rw-r--r--   0        0        0     1042 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/core/structs.py
--rw-r--r--   0        0        0     5533 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/core/workflows.py
--rw-r--r--   0        0        0      604 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/dispatch.py
--rw-r--r--   0        0        0       70 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/logic/__init__.py
--rw-r--r--   0        0        0     4402 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/logic/task_logic.py
--rw-r--r--   0        0        0      809 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/route.py
--rw-r--r--   0        0        0      677 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/rules/__init__.py
--rw-r--r--   0        0        0      689 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/rules/rule_base.py
--rw-r--r--   0        0        0     4270 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/rules/rule_workflow.py
--rw-r--r--   0        0        0      667 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/log.py
--rw-r--r--   0        0        0       70 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/submit/__init__.py
--rw-r--r--   0        0        0       70 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/submit/logic/__init__.py
--rw-r--r--   0        0        0     5961 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/submit/logic/submit_logic.py
--rw-r--r--   0        0        0      987 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/submit/submit.py
--rw-r--r--   0        0        0       70 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/xcelery/__init__.py
--rw-r--r--   0        0        0     2206 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/xcelery/instance.py
--rw-r--r--   0        0        0     1183 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/xcelery/task_base.py
--rw-r--r--   0        0        0       83 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/__init__.py
--rw-r--r--   0        0        0     5652 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/decorator.py
--rw-r--r--   0        0        0     2845 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/profiler.py
--rw-r--r--   0        0        0     3068 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/xListStr.py
--rw-r--r--   0        0        0     6099 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/xdataframe.py
--rw-r--r--   0        0        0     6161 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/xdate.py
--rw-r--r--   0        0        0     3091 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/xhttp.py
--rw-r--r--   0        0        0      971 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/xmath.py
--rw-r--r--   0        0        0       69 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/xtrace/__init__.py
--rw-r--r--   0        0        0     2858 2023-05-04 04:10:08.022087 yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/xtrace/helper.py
--rw-r--r--   0        0        0     5505 1970-01-01 00:00:00.000000 yyxx_game_pkg-2023.5.4.1/PKG-INFO
+-rw-r--r--   0        0        0     4895 2023-06-06 06:43:26.107574 yyxx_game_pkg-2023.6.6.1/README.md
+-rw-r--r--   0        0        0     1791 2023-06-06 06:43:36.863481 yyxx_game_pkg-2023.6.6.1/pyproject.toml
+-rw-r--r--   0        0        0       68 2023-06-06 06:43:26.107574 yyxx_game_pkg-2023.6.6.1/tests/__init__.py
+-rw-r--r--   0        0        0       83 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/tests/dbops/__init__.py
+-rw-r--r--   0        0        0     1341 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/tests/dbops/mysql_op.py
+-rw-r--r--   0        0        0       70 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/tests/dispatch/__init__.py
+-rw-r--r--   0        0        0       70 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/tests/dispatch/config/__init__.py
+-rw-r--r--   0        0        0     1228 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/tests/dispatch/config/celery_local_config.py
+-rw-r--r--   0        0        0      660 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/tests/dispatch/rules/__init__.py
+-rw-r--r--   0        0        0     1348 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/tests/dispatch/rules/rule_temp.py
+-rw-r--r--   0        0        0      580 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/tests/dispatch/test_dispatch.py
+-rw-r--r--   0        0        0       84 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/tests/helpers/__init__.py
+-rw-r--r--   0        0        0      522 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/tests/helpers/test_mysql_helper.py
+-rw-r--r--   0        0        0      455 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/tests/helpers/test_pika_helper.py
+-rw-r--r--   0        0        0      481 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/tests/helpers/test_redis_helper.py
+-rw-r--r--   0        0        0       70 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/tests/submit/__init__.py
+-rw-r--r--   0        0        0       70 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/tests/submit/schedule_rule/__init__.py
+-rw-r--r--   0        0        0       70 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/tests/submit/schedule_rule/schedule/__init__.py
+-rw-r--r--   0        0        0       70 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/tests/submit/schedule_rule/schedule/statistic_task/__init__.py
+-rw-r--r--   0        0        0      431 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/tests/submit/schedule_rule/schedule/statistic_task/schedule_statistic_collect_test.py
+-rw-r--r--   0        0        0      413 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/tests/submit/schedule_rule/schedule/statistic_task/schedule_statistic_task_test.py
+-rw-r--r--   0        0        0       70 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/tests/submit/schedule_rule/schedule/work_flow/__init__.py
+-rw-r--r--   0        0        0     1217 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/tests/submit/schedule_rule/schedule/work_flow/schedule_work_flow_test.py
+-rw-r--r--   0        0        0      305 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/tests/submit/submit.json
+-rw-r--r--   0        0        0     1250 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/tests/submit/test_submit.py
+-rw-r--r--   0        0        0      235 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/tests/test_ip2region.py
+-rw-r--r--   0        0        0      513 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/tests/test_logger.py
+-rw-r--r--   0        0        0      960 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/tests/test_xtrace.py
+-rw-r--r--   0        0        0       81 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/tests/utils/__init__.py
+-rw-r--r--   0        0        0       70 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/tests/xcelery/__init__.py
+-rw-r--r--   0        0        0       70 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/tests/xcelery/config/__init__.py
+-rw-r--r--   0        0        0     1226 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/tests/xcelery/config/celery_local_config.py
+-rw-r--r--   0        0        0      747 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/tests/xcelery/task_register.py
+-rw-r--r--   0        0        0      299 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/tests/xcelery/test_celery.py
+-rw-r--r--   0        0        0       69 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/__init__.py
+-rw-r--r--   0        0        0      124 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/center_api/__init__.py
+-rw-r--r--   0        0        0     5166 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/center_api/model/Operator.py
+-rw-r--r--   0        0        0     1505 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/center_api/model/OperatorServer.py
+-rw-r--r--   0        0        0     2572 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/center_api/model/RechargeConfig.py
+-rw-r--r--   0        0        0     2600 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/center_api/model/TableFieldConf.py
+-rw-r--r--   0        0        0      124 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/center_api/model/__init__.py
+-rw-r--r--   0        0        0      124 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/center_api/sdk/__init__.py
+-rw-r--r--   0        0        0     4378 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/center_api/sdk/check_token.py
+-rw-r--r--   0        0        0     5897 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/center_api/sdk/map_core.py
+-rw-r--r--   0        0        0     3335 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/center_api/sdk/recharge.py
+-rw-r--r--   0        0        0     6894 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/conf/__init__.py
+-rw-r--r--   0        0        0     2053 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/conf/global_settings.py
+-rw-r--r--   0        0        0      128 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/crypto/__init__.py
+-rw-r--r--   0        0        0     1164 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/crypto/aes.py
+-rw-r--r--   0        0        0     1113 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/crypto/basic.py
+-rw-r--r--   0        0        0     1344 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/crypto/make_sign.py
+-rw-r--r--   0        0        0     2652 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/crypto/rsa.py
+-rw-r--r--   0        0        0       83 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/dbops/__init__.py
+-rw-r--r--   0        0        0     1331 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/dbops/base.py
+-rw-r--r--   0        0        0     1304 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/dbops/ch_op.py
+-rw-r--r--   0        0        0     5596 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/dbops/das_api.py
+-rw-r--r--   0        0        0     1911 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/dbops/es_op.py
+-rw-r--r--   0        0        0     1678 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/dbops/hdfs_op.py
+-rw-r--r--   0        0        0      979 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/dbops/mongo_op.py
+-rw-r--r--   0        0        0     3955 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/dbops/mysql_op.py
+-rw-r--r--   0        0        0       81 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/helpers/__init__.py
+-rw-r--r--   0        0        0     2686 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/helpers/mysql_helper.py
+-rw-r--r--   0        0        0     3215 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/helpers/op_helper.py
+-rw-r--r--   0        0        0     1266 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/helpers/pika_helper.py
+-rw-r--r--   0        0        0     2966 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/helpers/redis_helper.py
+-rw-r--r--   0        0        0       79 2023-06-06 06:43:26.111574 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/ip2region/__init__.py
+-rw-r--r--   0        0        0 11070130 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/ip2region/ip2region.xdb
+-rw-r--r--   0        0        0      604 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/ip2region/ip_x.py
+-rw-r--r--   0        0        0     5735 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/ip2region/xdbSearcher.py
+-rw-r--r--   0        0        0       81 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/logger/__init__.py
+-rw-r--r--   0        0        0     2326 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/logger/config.py
+-rw-r--r--   0        0        0     3467 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/logger/handlers.py
+-rw-r--r--   0        0        0     2154 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/logger/log.py
+-rw-r--r--   0        0        0       70 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/stat/__init__.py
+-rw-r--r--   0        0        0       68 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/stat/dispatch/__init__.py
+-rw-r--r--   0        0        0       70 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/stat/dispatch/common/__init__.py
+-rw-r--r--   0        0        0     1514 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/stat/dispatch/common/common.py
+-rw-r--r--   0        0        0       69 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/stat/dispatch/core/__init__.py
+-rw-r--r--   0        0        0      805 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/stat/dispatch/core/manager.py
+-rw-r--r--   0        0        0     1042 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/stat/dispatch/core/structs.py
+-rw-r--r--   0        0        0     5533 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/stat/dispatch/core/workflows.py
+-rw-r--r--   0        0        0      604 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/stat/dispatch/dispatch.py
+-rw-r--r--   0        0        0       70 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/stat/dispatch/logic/__init__.py
+-rw-r--r--   0        0        0     4402 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/stat/dispatch/logic/task_logic.py
+-rw-r--r--   0        0        0      809 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/stat/dispatch/route.py
+-rw-r--r--   0        0        0      677 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/stat/dispatch/rules/__init__.py
+-rw-r--r--   0        0        0      689 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/stat/dispatch/rules/rule_base.py
+-rw-r--r--   0        0        0     4270 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/stat/dispatch/rules/rule_workflow.py
+-rw-r--r--   0        0        0      667 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/stat/log.py
+-rw-r--r--   0        0        0       70 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/stat/submit/__init__.py
+-rw-r--r--   0        0        0       70 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/stat/submit/logic/__init__.py
+-rw-r--r--   0        0        0     5961 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/stat/submit/logic/submit_logic.py
+-rw-r--r--   0        0        0      987 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/stat/submit/submit.py
+-rw-r--r--   0        0        0       70 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/stat/xcelery/__init__.py
+-rw-r--r--   0        0        0     2206 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/stat/xcelery/instance.py
+-rw-r--r--   0        0        0     1183 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/stat/xcelery/task_base.py
+-rw-r--r--   0        0        0      428 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/template/__init__.py
+-rw-r--r--   0        0        0      132 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/template/sdk/cookiecutter.json
+-rw-r--r--   0        0        0     3930 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/check_token.py
+-rw-r--r--   0        0        0      624 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/map_factor.py
+-rw-r--r--   0        0        0     4027 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/template/sdk/sdk_{{cookiecutter.sdk_name}}/recharge.py
+-rw-r--r--   0        0        0       83 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/utils/__init__.py
+-rw-r--r--   0        0        0     5652 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/utils/decorator.py
+-rw-r--r--   0        0        0     3135 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/utils/error_code.py
+-rw-r--r--   0        0        0     2845 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/utils/profiler.py
+-rw-r--r--   0        0        0     3068 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/utils/xListStr.py
+-rw-r--r--   0        0        0     8580 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/utils/xdataframe.py
+-rw-r--r--   0        0        0     7442 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/utils/xdate.py
+-rw-r--r--   0        0        0     3653 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/utils/xhttp.py
+-rw-r--r--   0        0        0      971 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/utils/xmath.py
+-rw-r--r--   0        0        0      573 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/utils/xstring.py
+-rw-r--r--   0        0        0       69 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/xtrace/__init__.py
+-rw-r--r--   0        0        0     2858 2023-06-06 06:43:26.179573 yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/xtrace/helper.py
+-rw-r--r--   0        0        0     6864 1970-01-01 00:00:00.000000 yyxx_game_pkg-2023.6.6.1/PKG-INFO
```

### Comparing `yyxx_game_pkg-2023.5.4.1/README.md` & `yyxx_game_pkg-2023.6.6.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -62,14 +62,47 @@
 3.配置虚拟环境并激活
 ```shell
 - poetry env use python3
 - poetry env list
 - poetry shell
 ```
 
+4.添加包
+
+关于`poetry`的使用，参考文档：[http://yydocs.yyxxgame.com/web/#/183/1758](http://yydocs.yyxxgame.com/web/#/183/1758)
+
+```shell
+- poetry add numpy  # 基本使用
+- poetry add numpy --optional  # 添加额外包（针对项目单独使用的包）
+```
+> 如果使用`--optional`，需要手动修改`pyproject.toml`文件
+>   - 1.在`[tool.poetry.extras]`增加相应`extra`分组和包
+>   - 2.命令行`poetry lock`更新`poetry.lock`文件
+>   - 3.命令行`poetry install -E center_api`安装`optional`中的包
+
+```toml
+# example
+[tool.poetry.extras]
+center_api = ["flask", "numpy"]
+stat = ["pandas", "numpy"]
+```
+
+5.安装依赖
+```shell
+# 开发 yyxxgame-pkg 安装依赖
+# 安装基础依赖，以及额外center_api依赖
+- poetry install -E stat
+- poetry install -E stat -E center_api  # 安装多个额外依赖
+- poetry install --extras "stat center_api"
+
+# 项目中使用 yyxxgame-pkg 安装依赖
+- poetry add yyxx-game-pkg[stat]
+- pip install yyxx-game-pkg[stat]
+```
+
 ### 文件目录说明
 ```
 yyxxgame-pkg 
 ├── README.md
 ├── gen_version.py
 ├── images
 │   └── logo.png
```

#### html2text {}

```diff
@@ -11,28 +11,42 @@
 (#æ¨¡åä»ç») - [xtrace](#xtrace) - [stat](#stat) - [ä»£ç ç¤ºä¾]
 (#ä»£ç ç¤ºä¾) - [çæ¬æ§å¶](#çæ¬æ§å¶) ### ä¸ææå ######
 ç¯å¢éç½® 1.ç¯å¢å®è£python3.11ä»¥ä¸çæ¬ ###### å®è£æ­¥éª¤
 1.Cloneä»£ç  ```shell git clone https://github.com/yyxxgame/yyxxgame-pkg.git
 ``` 2.å®è£poetry ```shell - curl -sSL https://install.python-poetry.org |
 python3 - export PATH="/root/.local/bin:$PATH" ```
 3.éç½®èæç¯å¢å¹¶æ¿æ´» ```shell - poetry env use python3 - poetry env
-list - poetry shell ``` ### æä»¶ç®å½è¯´æ ``` yyxxgame-pkg âââ
-README.md âââ gen_version.py âââ images âÂ Â  âââ logo.png
-âââ poetry.lock âââ pyproject.toml âââ tests âÂ Â 
-âââ __init__.py âÂ Â  âââ dispatch âÂ Â  âââ submit
-âÂ Â  âââ test_ip2region.py âÂ Â  âââ test_logger.py âÂ Â 
-âââ test_xtrace.py âÂ Â  âââ utils âÂ Â  âââ xcelery
-âââ yyxx_game_pkg âââ __init__.py âââ helpers âââ
-ip2region âââ logger âââ stat âââ utils âââ xtrace ```
-### é¨ç½² ###### develop æäº¤æ³¨éä¸­æ·»å `
-[BUILD]`å³é®å­å¹¶æ¨éä¼è§¦ågithub actionsçdevçæ¬æå»ºå¹¶åå¸å°
-[yyxx-game-pkg-dev](https://pypi.org/project/yyxx-game-pkg-dev/) ###### release
-æ°å»º`tag`å¹¶æ¨éä¼è§¦ågithub actionsçæ­£å¼çæ¬æå»ºå¹¶åå¸å°
-[yyxx-game-pkg](https://pypi.org/project/yyxx-game-pkg/) ### æ¨¡åä»ç»
-yyxxgame-pkgåå«ä»¥ä¸æ¨¡åï¼ ###### xtrace `xtrace`
+list - poetry shell ``` 4.æ·»å å å³äº`poetry`çä½¿ç¨ï¼åèææ¡£ï¼
+[http://yydocs.yyxxgame.com/web/#/183/1758](http://yydocs.yyxxgame.com/web/#/
+183/1758) ```shell - poetry add numpy # åºæ¬ä½¿ç¨ - poetry add numpy --
+optional # æ·»å é¢å¤åï¼éå¯¹é¡¹ç®åç¬ä½¿ç¨çåï¼ ``` >
+å¦æä½¿ç¨`--optional`ï¼éè¦æå¨ä¿®æ¹`pyproject.toml`æä»¶ > - 1.å¨`
+[tool.poetry.extras]`å¢å ç¸åº`extra`åç»åå > - 2.å½ä»¤è¡`poetry
+lock`æ´æ°`poetry.lock`æä»¶ > - 3.å½ä»¤è¡`poetry install -
+E center_api`å®è£`optional`ä¸­çå ```toml # example [tool.poetry.extras]
+center_api = ["flask", "numpy"] stat = ["pandas", "numpy"] ``` 5.å®è£ä¾èµ
+```shell # å¼å yyxxgame-pkg å®è£ä¾èµ #
+å®è£åºç¡ä¾èµï¼ä»¥åé¢å¤center_apiä¾èµ - poetry install -E stat -
+poetry install -E stat -E center_api # å®è£å¤ä¸ªé¢å¤ä¾èµ - poetry
+install --extras "stat center_api" # é¡¹ç®ä¸­ä½¿ç¨ yyxxgame-pkg å®è£ä¾èµ
+- poetry add yyxx-game-pkg[stat] - pip install yyxx-game-pkg[stat] ``` ###
+æä»¶ç®å½è¯´æ ``` yyxxgame-pkg âââ README.md âââ
+gen_version.py âââ images âÂ Â  âââ logo.png âââ
+poetry.lock âââ pyproject.toml âââ tests âÂ Â  âââ
+__init__.py âÂ Â  âââ dispatch âÂ Â  âââ submit âÂ Â 
+âââ test_ip2region.py âÂ Â  âââ test_logger.py âÂ Â  âââ
+test_xtrace.py âÂ Â  âââ utils âÂ Â  âââ xcelery âââ
+yyxx_game_pkg âââ __init__.py âââ helpers âââ ip2region
+âââ logger âââ stat âââ utils âââ xtrace ``` ### é¨ç½²
+###### develop æäº¤æ³¨éä¸­æ·»å `[BUILD]`å³é®å­å¹¶æ¨éä¼è§¦ågithub
+actionsçdevçæ¬æå»ºå¹¶åå¸å°[yyxx-game-pkg-dev](https://pypi.org/
+project/yyxx-game-pkg-dev/) ###### release æ°å»º`tag`å¹¶æ¨éä¼è§¦ågithub
+actionsçæ­£å¼çæ¬æå»ºå¹¶åå¸å°[yyxx-game-pkg](https://pypi.org/
+project/yyxx-game-pkg/) ### æ¨¡åä»ç» yyxxgame-pkgåå«ä»¥ä¸æ¨¡åï¼
+###### xtrace `xtrace`
 æ¨¡åå°è£äºé¾è·¯è¿½è¸ªçå¸®å©ç±»ï¼å¯ä»¥å¸®å©å¼åäººåå¿«éå°å®ç°é¾è·¯è¿½è¸ªåè½ã
 ###### stat
 `stat`æ¨¡ååå«yyxxgameåé¨ç»è®¡ä¸å¡çåºå±æ¡æ¶ï¼ç®ååå«`dispatch`ã`submit`ã`xceleryå ä¸ªæ¨¡å`
 ### ä»£ç ç¤ºä¾ åè[test](https://github.com/yyxxgame/yyxxgame-pkg/tree/
 master/tests) ä¸­çè°ç¨ä¾å­ ### çæ¬æ§å¶
 è¯¥é¡¹ç®ä½¿ç¨Gitè¿è¡çæ¬ç®¡çãæ¨å¯ä»¥å¨repositoryåçå½åå¯ç¨çæ¬ã
 [your-project-path]:yyxxgame/yyxxgame-pkg [contributors-shield]: https://
```

### Comparing `yyxx_game_pkg-2023.5.4.1/pyproject.toml` & `yyxx_game_pkg-2023.6.6.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-equires = [ "poetry-core",]
+requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "yyxx-game-pkg"
-version = "v2023.05.04.001"
+version = "v2023.06.06.001"
 description = "yyxx game custom module"
 authors = [ "yyxx-game",]
 license = "MIT"
 homepage = "https://github.com/yyxxgame/yyxxgame-pkg"
 repository = "https://github.com/yyxxgame/yyxxgame-pkg"
 readme = "README.md"
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
@@ -18,24 +18,57 @@
 [[tool.poetry.packages]]
 include = "tests"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <4"
 toml = "^0.10.2"
 opentelemetry-api = "^1.16.0"
-opentelemetry-exporter-jaeger = "^1.16.0"
 opentelemetry-sdk = "^1.16.0"
+opentelemetry-exporter-jaeger = "^1.16.0"
 opentelemetry-instrumentation-requests = "^0.37b0"
-requests = "^2.28.2"
+opentelemetry-instrumentation-fastapi = "0.37b.0"
+opentelemetry-instrumentation-celery = "0.37b0"
 line-profiler = "^4.0.3"
-celery = "^5.2.7"
-fastapi = "^0.94.0"
-uvicorn = "^0.21.0"
 redis = "^4.5.1"
-opentelemetry-instrumentation-fastapi = "0.37b.0"
-pika = "^1.3.1"
 pymysql = "^1.0.2"
+pika = "^1.3.1"
 dbutils = "^3.0.2"
-opentelemetry-instrumentation-celery = "0.37b0"
 ujson = "^5.7.0"
+requests = "2.27.1"
+celery = "^5.2.7"
+uvicorn = "^0.21.0"
 pandas = "^1.5.3"
-opentelemetry-instrumentation-django = "0.37b0"
+pycryptodome = "^3.17"
+
+[tool.poetry.extras]
+stat = [ "fastapi",]
+server_center = [ "django", "pillow", "filetype",]
+center_api = [ "flask", "cookiecutter",]
+
+[tool.poetry.dependencies.fastapi]
+version = "^0.94.0"
+optional = true
+
+[tool.poetry.dependencies.pillow]
+version = "^9.5.0"
+optional = true
+
+[tool.poetry.dependencies.filetype]
+version = "^1.2.0"
+optional = true
+
+[tool.poetry.dependencies.django]
+version = "^4.2.1"
+optional = true
+
+[tool.poetry.dependencies.flask]
+version = "^2.3.2"
+optional = true
+
+[tool.poetry.dependencies.cookiecutter]
+version = "^2.1.1"
+optional = true
+
+[tool.poetry.group.dev.dependencies]
+black = "^23.3.0"
+flake8-isort = "^6.0.0"
+pre-commit = "^3.3.2"
```

### Comparing `yyxx_game_pkg-2023.5.4.1/tests/dbops/mysql_op.py` & `yyxx_game_pkg-2023.6.6.1/tests/dbops/mysql_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.4.1/tests/dispatch/config/celery_local_config.py` & `yyxx_game_pkg-2023.6.6.1/tests/dispatch/config/celery_local_config.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.4.1/tests/dispatch/rules/__init__.py` & `yyxx_game_pkg-2023.6.6.1/tests/dispatch/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.4.1/tests/dispatch/rules/rule_temp.py` & `yyxx_game_pkg-2023.6.6.1/tests/dispatch/rules/rule_temp.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.4.1/tests/dispatch/test_dispatch.py` & `yyxx_game_pkg-2023.6.6.1/tests/dispatch/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.4.1/tests/helpers/test_mysql_helper.py` & `yyxx_game_pkg-2023.6.6.1/tests/helpers/test_mysql_helper.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.4.1/tests/submit/schedule_rule/schedule/work_flow/schedule_work_flow_test.py` & `yyxx_game_pkg-2023.6.6.1/tests/submit/schedule_rule/schedule/work_flow/schedule_work_flow_test.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.4.1/tests/submit/test_submit.py` & `yyxx_game_pkg-2023.6.6.1/tests/submit/test_submit.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.4.1/tests/test_logger.py` & `yyxx_game_pkg-2023.6.6.1/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.4.1/tests/test_xtrace.py` & `yyxx_game_pkg-2023.6.6.1/tests/test_xtrace.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.4.1/tests/xcelery/config/celery_local_config.py` & `yyxx_game_pkg-2023.6.6.1/tests/xcelery/config/celery_local_config.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.4.1/tests/xcelery/task_register.py` & `yyxx_game_pkg-2023.6.6.1/tests/xcelery/task_register.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/base.py` & `yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/dbops/base.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/ch_op.py` & `yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/dbops/ch_op.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         获取单条数据
         :param sql:
         :return:
         """
         res_df = self.get_all_df(sql)
         if not res_df.empty:
             return res_df.iloc[0]
-        return pd.Series()
+        return pd.Series(dtype=str)
 
     def get_all_df(self, sql):
         """
         获取所有数据 dataframe
         :param sql:
         :return:
         """
```

### Comparing `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/das_api.py` & `yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/dbops/das_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
         clickhouse 执行 sql (数据插入)
         :param das_url: das_http_url
         :param post_data: {
             "sql": sql,                     # sql语句
         }
         :return:
         """
-        b_ok, res = DasApi._post(das_url, "/das/ch/query", post_data=post_data)
+        b_ok, res = DasApi._post(das_url, "/das/ch/exec", post_data=post_data)
         if not b_ok:
             raise Exception(res)
         return b_ok
 
 
 # if __name__ == '__main__':
 # post_type = "das/mgo/query"
```

### Comparing `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/es_op.py` & `yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/dbops/es_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/hdfs_op.py` & `yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/dbops/hdfs_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/mongo_op.py` & `yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/dbops/mongo_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/dbops/mysql_op.py` & `yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/dbops/mysql_op.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/helpers/mysql_helper.py` & `yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/helpers/mysql_helper.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,67 +2,65 @@
 """
 @File: mysql_helper.py
 @Author: ltw
 @Time: 2023/3/22
 """
 import pymysql
 from dbutils.pooled_db import PooledDB
-from yyxx_game_pkg.utils.decorator import except_monitor, log_execute_time_monitor, singleton_unique_obj_args
-from yyxx_game_pkg.logger.log import root_log
-
-
-# #################### 模块对外接口 ####################
-def get_dbpool(config: dict):
-    class Config(MysqlConfig):
-        HOST = config["host"]
-        PORT = config["port"]
-        USER = config["user"]
-        PASSWD = config["password"]
-        DB = config["db"]
-        USE_UNICODE = config.get("use_unicode", True)
-        CHARSET = config.get("charset", "utf8")
-        MAX_CACHED = config.get("maxcached", 0)
-        MAX_CONNECTIONS = config.get("maxconnections", 0)
+from pymysql.cursors import Cursor
 
-    return MysqlDbPool(Config())
+from yyxx_game_pkg.logger.log import root_log
+from yyxx_game_pkg.utils.decorator import (
+    except_monitor,
+    log_execute_time_monitor,
+    singleton_unique_obj_args,
+)
 
 
 # ####################################################
 class MysqlConfig:
     HOST = None
     PORT = None
     USER = None
     PASSWD = None
     DB = None
     USE_UNICODE = None
     CHARSET = None
     MAX_CACHED = None
     MAX_CONNECTIONS = None
+    CURSOR = None
 
     def __str__(self):
-        return "host:{},port:{},db:{},use_unicode:{},charset:{},max_cache:{},max_connections:{}".format(
-            self.HOST, self.PORT, self.DB, self.USE_UNICODE, self.CHARSET, self.MAX_CACHED, self.MAX_CONNECTIONS
+        return "host:{},port:{},db:{},use_unicode:{},charset:{},max_cache:{},max_connections:{},cursor:{}".format(
+            self.HOST,
+            self.PORT,
+            self.DB,
+            self.USE_UNICODE,
+            self.CHARSET,
+            self.MAX_CACHED,
+            self.MAX_CONNECTIONS,
+            self.CURSOR,
         )
 
 
 @singleton_unique_obj_args
 class MysqlDbPool(object):
-
     def __init__(self, config: MysqlConfig):
         self.DB_POOL = PooledDB(
             creator=pymysql,
             maxcached=config.MAX_CACHED,
             maxconnections=config.MAX_CONNECTIONS,
             host=config.HOST,
             port=config.PORT,
             user=config.USER,
             passwd=config.PASSWD,
             db=config.DB,
             use_unicode=config.USE_UNICODE,
             charset=config.CHARSET,
+            cursorclass=config.CURSOR,
         )
         root_log(f"<MysqlDbPool> init, info:{config}")
 
     @except_monitor
     @log_execute_time_monitor()
     def get_connection(self):
         return self.DB_POOL.connection()
@@ -70,7 +68,24 @@
     def close_connection(self):
         """
         关闭线程池,线程池最少占用1连接,100个进程跑1000个相同IP库的服时,最多会生成10W连接，所以需要关闭线程池，释放全部连接。
         优化点：以后可以相同IP的服务器共用1个线程池（现阶段sql查game库没有指定库名,改动地方多,搁置）
         :return:
         """
         self.DB_POOL.close()
+
+
+# #################### 模块对外接口 ####################
+def get_dbpool(config: dict) -> MysqlDbPool:
+    class Config(MysqlConfig):
+        HOST = config["host"]
+        PORT = config["port"]
+        USER = config["user"]
+        PASSWD = config["password"]
+        DB = config["db"]
+        USE_UNICODE = config.get("use_unicode", True)
+        CHARSET = config.get("charset", "utf8")
+        MAX_CACHED = config.get("maxcached", 0)
+        MAX_CONNECTIONS = config.get("maxconnections", 0)
+        CURSOR = config.get("cursor", Cursor)
+
+    return MysqlDbPool(Config())
```

### Comparing `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/helpers/pika_helper.py` & `yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/helpers/pika_helper.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/helpers/redis_helper.py` & `yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/helpers/redis_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,18 @@
 # -*- coding: utf-8 -*-
 """
 @File: redis_helper
 @Author: ltw
 @Time: 2023/3/9
 """
 import redis
+from yyxx_game_pkg.logger.log import root_log
 from yyxx_game_pkg.utils.decorator import singleton_unique_obj_args
 
 
-def get_redis(config: dict):
-    """
-    缓存redis
-    :return:
-    """
-
-    class Config(RedisConfig):
-        """
-        redis config
-        """
-
-        HOST = config["host"]
-        PORT = config["port"]
-        DB = config["db"]
-        PASSWORD = config["password"]
-        OVERDUE_SECOND = config.get("overdue_second", 86400)
-
-    return RedisHelper(Config())
-
-
 class RedisConfig:
     """
     redis config
     """
 
     HOST = None
     PORT = None
@@ -48,14 +29,15 @@
 @singleton_unique_obj_args
 class RedisHelper:
     def __init__(self, config: RedisConfig):
         connection_pool = redis.ConnectionPool(
             host=config.HOST, port=config.PORT, db=config.DB, password=config.PASSWORD
         )
         self.__r = redis.Redis(connection_pool=connection_pool)
+        root_log(f"<RedisHelper> init, info:{config}")
 
     @property
     def redis_cli(self):
         return self.__r
 
     def get_data(self, key):
         return self.__r.get(key)
@@ -119,7 +101,27 @@
         分片获取元素
         :param key:
         :param start:
         :param end:
         :return:
         """
         return self.__r.lrange(key, start, end)
+
+
+def get_redis(config: dict) -> RedisHelper:
+    """
+    缓存redis
+    :return:
+    """
+
+    class Config(RedisConfig):
+        """
+        redis config
+        """
+
+        HOST = config["host"]
+        PORT = config["port"]
+        DB = config["db"]
+        PASSWORD = config["password"]
+        OVERDUE_SECOND = config.get("overdue_second", 86400)
+
+    return RedisHelper(Config())
```

### Comparing `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/ip2region/ip2region.xdb` & `yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/ip2region/ip2region.xdb`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/ip2region/ip_x.py` & `yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/ip2region/ip_x.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/ip2region/xdbSearcher.py` & `yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/ip2region/xdbSearcher.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/logger/config.py` & `yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/logger/config.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/logger/handlers.py` & `yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/logger/handlers.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/logger/log.py` & `yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/logger/log.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/common/common.py` & `yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/stat/dispatch/common/common.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/core/manager.py` & `yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/stat/dispatch/core/manager.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/core/structs.py` & `yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/stat/dispatch/core/structs.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/core/workflows.py` & `yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/stat/dispatch/core/workflows.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/dispatch.py` & `yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/stat/dispatch/dispatch.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/logic/task_logic.py` & `yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/stat/dispatch/logic/task_logic.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/route.py` & `yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/stat/dispatch/route.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/rules/__init__.py` & `yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/stat/dispatch/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/rules/rule_base.py` & `yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/stat/dispatch/rules/rule_base.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/dispatch/rules/rule_workflow.py` & `yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/stat/dispatch/rules/rule_workflow.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/log.py` & `yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/stat/log.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/submit/logic/submit_logic.py` & `yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/stat/submit/logic/submit_logic.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/submit/submit.py` & `yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/stat/submit/submit.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/xcelery/instance.py` & `yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/stat/xcelery/instance.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/stat/xcelery/task_base.py` & `yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/stat/xcelery/task_base.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/decorator.py` & `yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/profiler.py` & `yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/xListStr.py` & `yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/utils/xListStr.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/xdate.py` & `yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/utils/xdate.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import time
 import datetime
 from enum import Enum
 
 DAY = 1
 WEEK = 2
 MONTH = 3
+VERSION = 4
 
 
 # 时间转换
 def str2date(date_str):
     """
     时间字符串转datetime obj
     """
@@ -77,31 +78,59 @@
     "2021-05-31 12:23:40" to "2021-05-31 23:59:59"
     :param date: datetime obj
     :return: datetime obj
     """
     return date2dt_day(date, 23, 59, 59)
 
 
-def day2date(day, fmt="%Y%m%d") -> datetime.datetime:
+def day2date(day, fmt="%Y%m%d", end=0) -> datetime.datetime:
     """
     "20210531" to "2021-05-31 00:00:00"
     :param day: 时间字符串
     :param fmt: 时间字符串格式 默认 "%Y%m%d"
+    :param end: 0: 00:00:00; 1: 23:59:59
     :return: datetime obj
     """
-    return datetime.datetime.strptime(str(day), fmt)
+    date = datetime.datetime.strptime(str(day), fmt)
+    if end:
+        return datetime.datetime(date.year, date.month, date.day, 23, 59, 59)
+    return date
+
+
+def day2str_date(day) -> str:
+    """
+    '20220301' -> '2022-03-01'
+    效率更高
+    """
+    day_s = str(day)
+    return day_s[:4] + '-' + day_s[4:6] + '-' + day_s[5:7]
 
 
 def date2day(date):
     """
     "2021-05-31 12:23:40" to "20210531"
     """
     return date.strftime("%Y%m%d")
 
 
+def date2date(date, _h=0, _m=0, _s=0, end=0):
+    """
+    "2021-05-31 12:23:40" to "2021-05-31 00:00:00"
+    :param date: datetime obj
+    :param _h: hour
+    :param _m: minute
+    :param _s: second
+    :param end: 0: 00:00:00; 1: 23:59:59
+    :return: datetime obj
+    """
+    if end:
+        return datetime.datetime(date.year, date.month, date.day, 23, 59, 59)
+    return datetime.datetime(date.year, date.month, date.day, int(_h), int(_m), int(_s))
+
+
 def day_diff(day1, day2):
     """
     day_diff(20210531, 20210529) -> 2
     """
     return (day2date(day2) - day2date(day1)).days
 
 
@@ -114,14 +143,21 @@
     :return:
     """
     if end:
         return date2dt_day_end(date) + datetime.timedelta(days=delta)
     return date2dt_day(date) + datetime.timedelta(days=delta)
 
 
+def add_days(date, delta, end=0):
+    """
+    易读接口
+    """
+    return delta_dt_day(date, delta, end)
+
+
 def date2stamp(dt_date):
     """
     datetime转时间戳
     """
     return time.mktime(dt_date.timetuple())
 
 
@@ -149,29 +185,37 @@
     sdate = datetime.datetime.strptime(str(date), fmt)
     _, _, s_week_day = sdate.isocalendar()
     sday = (sdate - datetime.timedelta(days=s_week_day - 1)).strftime("%Y-%m-%d")
     eday = (sdate - datetime.timedelta(days=s_week_day - 7)).strftime("%Y-%m-%d")
     return f"{sday}~{eday}"
 
 
-def date_type_trans(date, date_type=DAY, fmt="%Y%m%d"):
+def date_type_trans(day, date_type=DAY, fmt="%Y%m%d", version_configs=None):
     """
     周期时间格式化
-    :param date: 时间字符串
+    :param day: 时间字符串 20230201
     :param date_type: 周期类型(1: 天 2: 周 3: 月)
     :param fmt: 时间字符串格式 默认 "%Y%m%d"
+    :param version_configs: 版本配置list [[版本号, 开始day, 结束day]]
     :return: 周期字符串
     """
     if date_type == DAY:
-        return datetime.datetime.strptime(str(date), fmt).strftime("%Y-%m-%d")
+        return datetime.datetime.strptime(str(day), fmt).strftime("%Y-%m-%d")
     if date_type == WEEK:
-        return get_week_str(date, fmt)
+        return get_week_str(day, fmt)
     if date_type == MONTH:
-        return datetime.datetime.strptime(str(date), fmt).strftime("%Y年%m月")
-    return date
+        return datetime.datetime.strptime(str(day), fmt).strftime("%Y年%m月")
+    if date_type == VERSION:
+        if version_configs is None:
+            return day
+        for version, start_day, end_day in version_configs:
+            if start_day <= day <= end_day:
+                return f"{version}版本"
+        return "未配置版本"
+    return day
 
 
 def to_start_of_interval(_t: datetime.datetime, unit="minute", interval=5):
     """
     to_start_of_interval("2023-03-09 11:16:20", 'minute', interval=5) -> datetime(2023-03-09 11:15:00)
     to_start_of_interval("2023-03-09 11:16:20", 'hour', interval=1) -> datetime(2023-03-09 11:00:00)
     """
```

### Comparing `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/xhttp.py` & `yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/utils/xhttp.py`

 * *Files 15% similar despite different names*

```diff
@@ -103,7 +103,28 @@
 
     post_data_log = json.dumps(post_data, ensure_ascii=False)
     local_log(f"http_push_server url:{url} post_data: {post_data_log}")
 
     result = http_request(url, post_data, False, "get")
     local_log(f"http_push_server url:{url} res: {result}")
     return result
+
+
+def make_post_data(ex_params, api_key):
+    """
+    生成post_data
+    """
+    _t = int(time.time())
+    values = {"time": _t, "params": json.dumps(ex_params)}
+    keys = values.keys()
+    keys = sorted(keys)
+    params = []
+    for key in keys:
+        params.append(f"{key}={values[key]}")
+    params = "&".join(params)
+    timestamp = str(_t + (_t % 38975))
+    _tmp = md5(f"{params}{api_key}")
+    sign = md5(f"{timestamp}{_tmp}")
+
+    post_data = {"time": _t, "params": ex_params, "sign": sign}
+    post_data = set_params(post_data)
+    return post_data
```

### Comparing `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/utils/xmath.py` & `yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/utils/xmath.py`

 * *Files identical despite different names*

### Comparing `yyxx_game_pkg-2023.5.4.1/yyxx_game_pkg/xtrace/helper.py` & `yyxx_game_pkg-2023.6.6.1/yyxx_game_pkg/xtrace/helper.py`

 * *Files identical despite different names*

