# Comparing `tmp/c2cwsgiutils-5.2.1.tar.gz` & `tmp/c2cwsgiutils-5.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c2cwsgiutils-5.2.1.tar", max compression
+gzip compressed data, was "c2cwsgiutils-5.2.2.tar", max compression
```

## Comparing `c2cwsgiutils-5.2.1.tar` & `c2cwsgiutils-5.2.2.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0     1304 2023-02-07 11:48:54.646982 c2cwsgiutils-5.2.1/LICENSE
--rw-r--r--   0        0        0    28624 2023-02-07 11:48:54.646982 c2cwsgiutils-5.2.1/README.md
--rw-r--r--   0        0        0     3997 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/__init__.py
--rw-r--r--   0        0        0     1500 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/acceptance/__init__.py
--rw-r--r--   0        0        0     4620 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/acceptance/composition.py
--rw-r--r--   0        0        0     9109 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/acceptance/connection.py
--rw-r--r--   0        0        0     4475 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/acceptance/image.py
--rw-r--r--   0        0        0     2329 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/acceptance/print.py
--rw-r--r--   0        0        0     2072 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/acceptance/utils.py
--rw-r--r--   0        0        0     9314 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/auth.py
--rw-r--r--   0        0        0     4160 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/broadcast/__init__.py
--rw-r--r--   0        0        0      615 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/broadcast/interface.py
--rw-r--r--   0        0        0     1062 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/broadcast/local.py
--rw-r--r--   0        0        0     5058 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/broadcast/redis.py
--rw-r--r--   0        0        0      272 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/broadcast/utils.py
--rw-r--r--   0        0        0     3050 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/client_info.py
--rw-r--r--   0        0        0     1496 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/config_utils.py
--rw-r--r--   0        0        0      839 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/coverage_setup.py
--rw-r--r--   0        0        0    16288 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/db.py
--rw-r--r--   0        0        0     3049 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/db_maintenance_view.py
--rw-r--r--   0        0        0     1239 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/debug/__init__.py
--rw-r--r--   0        0        0     4364 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/debug/_listeners.py
--rw-r--r--   0        0        0     7507 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/debug/_views.py
--rw-r--r--   0        0        0     2328 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/debug/utils.py
--rw-r--r--   0        0        0     6723 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/errors.py
--rw-r--r--   0        0        0    21068 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/health_check.py
--rw-r--r--   0        0        0    17356 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/index.py
--rw-r--r--   0        0        0      628 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/loader.py
--rw-r--r--   0        0        0     3337 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/logging_view.py
--rw-r--r--   0        0        0     3425 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/metrics.py
--rw-r--r--   0        0        0     2691 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/models_graph.py
--rw-r--r--   0        0        0     1698 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/pretty_json.py
--rw-r--r--   0        0        0      739 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/profiler.py
--rw-r--r--   0        0        0     2062 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/prometheus.py
--rw-r--r--   0        0        0        0 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/py.typed
--rw-r--r--   0        0        0     1346 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/pyramid.py
--rw-r--r--   0        0        0     3703 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/pyramid_logging.py
--rw-r--r--   0        0        0     1478 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/redis_stats.py
--rw-r--r--   0        0        0     4527 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/redis_utils.py
--rw-r--r--   0        0        0     3823 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/request_tracking/__init__.py
--rw-r--r--   0        0        0      577 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/request_tracking/_sql.py
--rw-r--r--   0        0        0        0 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/scripts/__init__.py
--rwxr-xr-x   0        0        0     4147 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/scripts/check_es.py
--rwxr-xr-x   0        0        0     1998 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/scripts/genversion.py
--rwxr-xr-x   0        0        0     9629 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/scripts/stats_db.py
--rwxr-xr-x   0        0        0     2096 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/scripts/test_print.py
--rw-r--r--   0        0        0     5002 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/sentry.py
--rw-r--r--   0        0        0     1567 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/services.py
--rw-r--r--   0        0        0     3494 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/setup_process.py
--rw-r--r--   0        0        0      876 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/sql_profiler/__init__.py
--rw-r--r--   0        0        0     3680 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/sql_profiler/_impl.py
--rw-r--r--   0        0        0     1552 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/sqlalchemylogger/README.md
--rw-r--r--   0        0        0        0 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/sqlalchemylogger/__init__.py
--rw-r--r--   0        0        0      752 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/sqlalchemylogger/_filters.py
--rw-r--r--   0        0        0     1477 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/sqlalchemylogger/_models.py
--rw-r--r--   0        0        0      460 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/sqlalchemylogger/examples/example.py
--rw-r--r--   0        0        0     4809 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/sqlalchemylogger/handlers.py
--rw-r--r--   0        0        0    11480 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/stats.py
--rw-r--r--   0        0        0      971 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/stats_pyramid/__init__.py
--rw-r--r--   0        0        0     2840 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/stats_pyramid/_db_spy.py
--rw-r--r--   0        0        0     2943 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/stats_pyramid/_pyramid_spy.py
--rw-r--r--   0        0        0      527 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/stats_pyramid/_views.py
--rw-r--r--   0        0        0     1817 2023-02-07 11:48:54.650983 c2cwsgiutils-5.2.1/c2cwsgiutils/version.py
--rw-r--r--   0        0        0     5297 2023-02-07 11:58:29.443923 c2cwsgiutils-5.2.1/pyproject.toml
--rw-r--r--   0        0        0    31538 1970-01-01 00:00:00.000000 c2cwsgiutils-5.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1304 2023-03-13 09:54:12.392344 c2cwsgiutils-5.2.2/LICENSE
+-rw-r--r--   0        0        0    28624 2023-03-13 09:54:12.392344 c2cwsgiutils-5.2.2/README.md
+-rw-r--r--   0        0        0     3997 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/__init__.py
+-rw-r--r--   0        0        0     1500 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/acceptance/__init__.py
+-rw-r--r--   0        0        0     4620 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/acceptance/composition.py
+-rw-r--r--   0        0        0     9195 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/acceptance/connection.py
+-rw-r--r--   0        0        0     4491 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/acceptance/image.py
+-rw-r--r--   0        0        0     2329 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/acceptance/print.py
+-rw-r--r--   0        0        0     2072 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/acceptance/utils.py
+-rw-r--r--   0        0        0     9314 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/auth.py
+-rw-r--r--   0        0        0     4160 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/broadcast/__init__.py
+-rw-r--r--   0        0        0      615 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/broadcast/interface.py
+-rw-r--r--   0        0        0     1062 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/broadcast/local.py
+-rw-r--r--   0        0        0     5058 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/broadcast/redis.py
+-rw-r--r--   0        0        0      272 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/broadcast/utils.py
+-rw-r--r--   0        0        0     3050 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/client_info.py
+-rw-r--r--   0        0        0     1496 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/config_utils.py
+-rw-r--r--   0        0        0      839 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/coverage_setup.py
+-rw-r--r--   0        0        0    16140 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/db.py
+-rw-r--r--   0        0        0     3049 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/db_maintenance_view.py
+-rw-r--r--   0        0        0     1239 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/debug/__init__.py
+-rw-r--r--   0        0        0     4364 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/debug/_listeners.py
+-rw-r--r--   0        0        0     7507 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/debug/_views.py
+-rw-r--r--   0        0        0     2328 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/debug/utils.py
+-rw-r--r--   0        0        0     6723 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/errors.py
+-rw-r--r--   0        0        0    20766 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/health_check.py
+-rw-r--r--   0        0        0    17356 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/index.py
+-rw-r--r--   0        0        0      628 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/loader.py
+-rw-r--r--   0        0        0     3337 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/logging_view.py
+-rw-r--r--   0        0        0     3425 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/metrics.py
+-rw-r--r--   0        0        0     2691 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/models_graph.py
+-rw-r--r--   0        0        0     1698 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/pretty_json.py
+-rw-r--r--   0        0        0      739 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/profiler.py
+-rw-r--r--   0        0        0     2062 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/prometheus.py
+-rw-r--r--   0        0        0        0 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/py.typed
+-rw-r--r--   0        0        0     1346 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/pyramid.py
+-rw-r--r--   0        0        0     3703 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/pyramid_logging.py
+-rw-r--r--   0        0        0     1478 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/redis_stats.py
+-rw-r--r--   0        0        0     4527 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/redis_utils.py
+-rw-r--r--   0        0        0     3823 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/request_tracking/__init__.py
+-rw-r--r--   0        0        0      577 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/request_tracking/_sql.py
+-rw-r--r--   0        0        0        0 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/scripts/__init__.py
+-rwxr-xr-x   0        0        0     4147 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/scripts/check_es.py
+-rwxr-xr-x   0        0        0     1998 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/scripts/genversion.py
+-rwxr-xr-x   0        0        0     9594 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/scripts/stats_db.py
+-rwxr-xr-x   0        0        0     2096 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/scripts/test_print.py
+-rw-r--r--   0        0        0     5002 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/sentry.py
+-rw-r--r--   0        0        0     1567 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/services.py
+-rw-r--r--   0        0        0     3494 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/setup_process.py
+-rw-r--r--   0        0        0      876 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/sql_profiler/__init__.py
+-rw-r--r--   0        0        0     3680 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/sql_profiler/_impl.py
+-rw-r--r--   0        0        0     1552 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/sqlalchemylogger/README.md
+-rw-r--r--   0        0        0        0 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/sqlalchemylogger/__init__.py
+-rw-r--r--   0        0        0      752 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/sqlalchemylogger/_filters.py
+-rw-r--r--   0        0        0     1477 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/sqlalchemylogger/_models.py
+-rw-r--r--   0        0        0      460 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/sqlalchemylogger/examples/example.py
+-rw-r--r--   0        0        0     4809 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/sqlalchemylogger/handlers.py
+-rw-r--r--   0        0        0    11480 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/stats.py
+-rw-r--r--   0        0        0      971 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/stats_pyramid/__init__.py
+-rw-r--r--   0        0        0     2840 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/stats_pyramid/_db_spy.py
+-rw-r--r--   0        0        0     2943 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/stats_pyramid/_pyramid_spy.py
+-rw-r--r--   0        0        0      527 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/stats_pyramid/_views.py
+-rw-r--r--   0        0        0     1817 2023-03-13 09:54:12.396344 c2cwsgiutils-5.2.2/c2cwsgiutils/version.py
+-rw-r--r--   0        0        0     5299 2023-03-13 10:01:29.045817 c2cwsgiutils-5.2.2/pyproject.toml
+-rw-r--r--   0        0        0    31538 1970-01-01 00:00:00.000000 c2cwsgiutils-5.2.2/PKG-INFO
```

### Comparing `c2cwsgiutils-5.2.1/LICENSE` & `c2cwsgiutils-5.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/README.md` & `c2cwsgiutils-5.2.2/README.md`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/__init__.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/__init__.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/acceptance/__init__.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/acceptance/__init__.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/acceptance/composition.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/acceptance/composition.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/acceptance/connection.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/acceptance/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         cache_expected: CacheExpected = CacheExpected.NO,
         **kwargs: Any,
     ) -> Optional[str]:
         """Get the given URL (relative to the root of API)."""
         with self.session.get(self.base_url + url, headers=self._merge_headers(headers, cors), **kwargs) as r:
             check_response(r, expected_status, cache_expected=cache_expected)
             self._check_cors(cors, r)
-            return None if r.status_code == 204 else r.text
+            return None if r.status_code == 204 else r.text  # type: ignore
 
     def get_raw(
         self,
         url: str,
         expected_status: int = 200,
         headers: Optional[Mapping[str, str]] = None,
         cors: bool = True,
@@ -86,16 +86,17 @@
             self.base_url + url,
             headers=self._merge_headers(headers, cors),
             stream=True,
             **kwargs,
         ) as r:
             check_response(r, expected_status, cache_expected=cache_expected)
             self._check_cors(cors, r)
-            r.raw.decode_content = True
-            doc = etree.parse(r.raw)  # nosec
+            r.raw.decode_content = True  # type: ignore
+            raw = r.raw  # type: ignore
+            doc = etree.parse(raw)  # nosec
             if schema is not None:
                 with open(schema, encoding="utf-8") as schema_file:
                     xml_schema = etree.XMLSchema(etree.parse(schema_file))  # nosec
                 xml_schema.assertValid(doc)
             return doc
 
     def post_json(
@@ -143,15 +144,15 @@
     ) -> Optional[str]:
         """POST the given URL (relative to the root of API)."""
         with self.session.post(
             self.base_url + url, headers=self._merge_headers(headers, cors), **kwargs
         ) as r:
             check_response(r, expected_status, cache_expected)
             self._check_cors(cors, r)
-            return None if r.status_code == 204 else r.text
+            return None if r.status_code == 204 else r.text  # type: ignore
 
     def put_json(
         self,
         url: str,
         expected_status: int = 200,
         headers: Optional[Mapping[str, str]] = None,
         cors: bool = True,
```

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/acceptance/image.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/acceptance/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     expected = skimage.io.imread(expected_filename)
     assert expected is not None, "Wrong image: " + expected_filename
 
     if mask is not None:
         expected[mask == 0] = [255, 255, 255]
 
     score, diff = skimage.metrics.structural_similarity(
-        expected, image_to_check, multichannel=True, full=True
+        expected, image_to_check, multichannel=True, full=True, channel_axis=2
     )
     diff = (255 - diff * 255).astype("uint8")
 
     if diff is None:
         skimage.io.imsave(result_filename, image_to_check)
         assert diff is not None, "No diff generated"
     if score < level:
```

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/acceptance/print.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/acceptance/print.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/acceptance/utils.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/acceptance/utils.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/auth.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/auth.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/broadcast/__init__.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/broadcast/__init__.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/broadcast/interface.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/broadcast/interface.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/broadcast/local.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/broadcast/local.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/broadcast/redis.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/broadcast/redis.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/client_info.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/client_info.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/config_utils.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/config_utils.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/coverage_setup.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/coverage_setup.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/db.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/db.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,31 @@
 """SQLalchemy models."""
 import logging
 import re
 import warnings
-from typing import Any, Callable, Iterable, Optional, Pattern, Tuple, Union, cast
+from typing import TYPE_CHECKING, Any, Callable, Iterable, Optional, Pattern, Tuple, Union, cast
 
 import pyramid.config
 import pyramid.config.settings
 import pyramid.request
 import sqlalchemy.engine
 import sqlalchemy.orm
 import transaction
 import zope.sqlalchemy
 from sqlalchemy import engine_from_config
-from sqlalchemy.orm import sessionmaker
 from zope.sqlalchemy import register
 
+if TYPE_CHECKING:
+    scoped_session = sqlalchemy.orm.scoped_session[sqlalchemy.orm.Session]
+    sessionmaker = sqlalchemy.orm.sessionmaker[sqlalchemy.orm.Session]
+else:
+    scoped_session = sqlalchemy.orm.scoped_session
+    sessionmaker = sqlalchemy.orm.sessionmaker
+
+
 LOG = logging.getLogger(__name__)
 RE_COMPILE: Callable[[str], Pattern[str]] = re.compile
 
 force_readonly = False
 
 
 class Tweens:
@@ -31,15 +38,15 @@
 def setup_session(
     config: pyramid.config.Configurator,
     master_prefix: str,
     slave_prefix: Optional[str] = None,
     force_master: Optional[Iterable[str]] = None,
     force_slave: Optional[Iterable[str]] = None,
 ) -> Tuple[
-    Union[sqlalchemy.orm.Session, sqlalchemy.orm.scoped_session[sqlalchemy.orm.Session]],
+    Union[sqlalchemy.orm.Session, scoped_session],
     sqlalchemy.engine.Engine,
     sqlalchemy.engine.Engine,
 ]:
     """
     Create a SQLAlchemy session.
 
     With an accompanying tween that switches between the master and the slave DB
@@ -91,15 +98,15 @@
     config: Optional[pyramid.config.Configurator],
     name: str,
     url: str,
     slave_url: Optional[str] = None,
     force_master: Optional[Iterable[str]] = None,
     force_slave: Optional[Iterable[str]] = None,
     **engine_config: Any,
-) -> Union[sqlalchemy.orm.Session, sqlalchemy.orm.scoped_session[sqlalchemy.orm.Session]]:
+) -> Union[sqlalchemy.orm.Session, scoped_session]:
     """
     Create a SQLAlchemy session.
 
     With an accompanying tween that switches between the master and the slave DB
     connection.
 
     The slave DB will be used for anything that is GET and OPTIONS queries. The master DB will be used for
@@ -143,15 +150,15 @@
     db_session.c2c_ro_bind = ro_engine  # type: ignore
     return db_session
 
 
 def _add_tween(
     config: pyramid.config.Configurator,
     name: str,
-    db_session: sqlalchemy.orm.scoped_session[sqlalchemy.orm.Session],
+    db_session: scoped_session,
     force_master: Optional[Iterable[str]],
     force_slave: Optional[Iterable[str]],
 ) -> None:
     master_paths: Iterable[Pattern[str]] = (
         list(map(RE_COMPILE, force_master)) if force_master is not None else []
     )
     slave_paths: Iterable[Pattern[str]] = (
@@ -197,15 +204,15 @@
 
         return db_chooser_tween
 
     setattr(tweens, name, db_chooser_tween_factory)
     config.add_tween("c2cwsgiutils.db.tweens." + name, over="pyramid_tm.tm_tween_factory")
 
 
-class SessionFactory(sessionmaker[sqlalchemy.orm.Session]):  # pylint: disable=unsubscriptable-object
+class SessionFactory(sessionmaker):
     """The custom session factory that manage the read only and read write sessions."""
 
     def __init__(
         self,
         force_master: Optional[Iterable[str]],
         force_slave: Optional[Iterable[str]],
         ro_engine: sqlalchemy.engine.Engine,
@@ -222,15 +229,15 @@
     def engine_name(self, readwrite: bool) -> str:
         if readwrite:
             return cast(str, self.rw_engine.c2c_name)  # type: ignore
         return cast(str, self.ro_engine.c2c_name)  # type: ignore
 
     def __call__(  # type: ignore
         self, request: Optional[pyramid.request.Request], readwrite: Optional[bool] = None, **local_kw: Any
-    ) -> sqlalchemy.orm.scoped_session[sqlalchemy.orm.Session]:
+    ) -> scoped_session:
         if readwrite is not None:
             if readwrite and not force_readonly:
                 LOG.debug("Using %s database", self.rw_engine.c2c_name)  # type: ignore
                 self.configure(bind=self.rw_engine)
             else:
                 LOG.debug("Using %s database", self.ro_engine.c2c_name)  # type: ignore
                 self.configure(bind=self.ro_engine)
@@ -258,23 +265,23 @@
 ) -> sqlalchemy.engine.Engine:
     """Get the engine from the settings."""
     return engine_from_config(settings, prefix)
 
 
 def get_session_factory(
     engine: sqlalchemy.engine.Engine,
-) -> sessionmaker[sqlalchemy.orm.Session]:  # pylint: disable=unsubscriptable-object
+) -> sessionmaker:
     """Get the session factory from the engine."""
     factory = sessionmaker()
     factory.configure(bind=engine)
     return factory
 
 
 def get_tm_session(
-    session_factory: sessionmaker[sqlalchemy.orm.Session],  # pylint: disable=unsubscriptable-object
+    session_factory: sessionmaker,
     transaction_manager: transaction.TransactionManager,
 ) -> sqlalchemy.orm.Session:
     """
     Get a ``sqlalchemy.orm.Session`` instance backed by a transaction.
 
     This function will hook the session to the transaction manager which
     will take care of committing any changes.
@@ -334,15 +341,15 @@
     return dbsession
 
 
 def get_tm_session_pyramid(
     session_factory: SessionFactory,
     transaction_manager: transaction.TransactionManager,
     request: pyramid.request.Request,
-) -> sqlalchemy.orm.scoped_session[sqlalchemy.orm.Session]:
+) -> scoped_session:
     """
     Get a ``sqlalchemy.orm.Session`` instance backed by a transaction.
 
     Same as ``get_tm_session`` to be used in a pyramid request.
     """
     dbsession = session_factory(request=request)
     zope.sqlalchemy.register(dbsession, transaction_manager=transaction_manager)
```

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/db_maintenance_view.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/db_maintenance_view.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/debug/__init__.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/debug/__init__.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/debug/_listeners.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/debug/_listeners.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/debug/_views.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/debug/_views.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/debug/utils.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/debug/utils.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/errors.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/errors.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/health_check.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/health_check.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,27 +11,45 @@
 import re
 import subprocess  # nosec
 import time
 import traceback
 from collections import Counter
 from enum import Enum
 from types import TracebackType
-from typing import Any, Callable, Dict, List, Literal, Mapping, Optional, Tuple, Type, Union, cast
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Dict,
+    List,
+    Literal,
+    Mapping,
+    Optional,
+    Tuple,
+    Type,
+    Union,
+    cast,
+)
 
 import pyramid.config
 import pyramid.request
 import requests
 import sqlalchemy.engine
 import sqlalchemy.orm
 import sqlalchemy.sql
 from pyramid.httpexceptions import HTTPNotFound
 
 import c2cwsgiutils.db
 from c2cwsgiutils import auth, broadcast, config_utils, redis_utils, stats, version
 
+if TYPE_CHECKING:
+    scoped_session = sqlalchemy.orm.scoped_session[sqlalchemy.orm.Session]
+else:
+    scoped_session = sqlalchemy.orm.scoped_session
+
 LOG = logging.getLogger(__name__)
 ALEMBIC_HEAD_RE = re.compile(r"^([a-f0-9]+) \(head\)\n$")
 
 
 class EngineType(Enum):
     """The type of engine."""
 
@@ -55,15 +73,15 @@
         return self.json
 
 
 class _Binding:
     def name(self) -> str:
         raise NotImplementedError()
 
-    def __enter__(self) -> sqlalchemy.orm.scoped_session[sqlalchemy.orm.Session]:
+    def __enter__(self) -> scoped_session:
         raise NotImplementedError()
 
     def __exit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc_value: Optional[BaseException],
         exc_traceback: Optional[TracebackType],
@@ -75,30 +93,28 @@
     def __init__(self, session: c2cwsgiutils.db.SessionFactory, readwrite: bool):
         self.session = session
         self.readwrite = readwrite
 
     def name(self) -> str:
         return self.session.engine_name(self.readwrite)
 
-    def __enter__(self) -> sqlalchemy.orm.scoped_session[sqlalchemy.orm.Session]:
+    def __enter__(self) -> scoped_session:
         return self.session(None, self.readwrite)
 
 
 class _OldBinding(_Binding):
-    def __init__(
-        self, session: sqlalchemy.orm.scoped_session[sqlalchemy.orm.Session], engine: sqlalchemy.engine.Engine
-    ):
+    def __init__(self, session: scoped_session, engine: sqlalchemy.engine.Engine):
         self.session = session
         self.engine = engine
         self.prev_bind = None
 
     def name(self) -> str:
         return cast(str, self.engine.c2c_name)  # type: ignore
 
-    def __enter__(self) -> sqlalchemy.orm.scoped_session[sqlalchemy.orm.Session]:
+    def __enter__(self) -> scoped_session:
         self.prev_bind = self.session.bind  # type: ignore
         self.session.bind = self.engine
         return self.session
 
     def __exit__(
         self,
         exc_type: Optional[Type[BaseException]],
@@ -106,27 +122,27 @@
         exc_traceback: Optional[TracebackType],
     ) -> Literal[False]:
         self.session.bind = self.prev_bind
         return False
 
 
 def _get_binding_class(
-    session: Union[sqlalchemy.orm.scoped_session[sqlalchemy.orm.Session], c2cwsgiutils.db.SessionFactory],
+    session: Union[scoped_session, c2cwsgiutils.db.SessionFactory],
     ro_engin: sqlalchemy.engine.Engine,
     rw_engin: sqlalchemy.engine.Engine,
     readwrite: bool,
 ) -> _Binding:
     if isinstance(session, c2cwsgiutils.db.SessionFactory):
         return _NewBinding(session, readwrite)
     else:
         return _OldBinding(session, ro_engin if readwrite else rw_engin)
 
 
 def _get_bindings(
-    session: Union[sqlalchemy.orm.scoped_session[sqlalchemy.orm.Session], c2cwsgiutils.db.SessionFactory],
+    session: Union[scoped_session, c2cwsgiutils.db.SessionFactory],
     engine_type: EngineType,
 ) -> List[_Binding]:
     if isinstance(session, c2cwsgiutils.db.SessionFactory):
         ro_engin = session.ro_engine
         rw_engin = session.rw_engine
     else:
         ro_engin = session.c2c_ro_bind  # type: ignore
@@ -191,16 +207,16 @@
         if self.name:
             self.add_redis_check(level=2)
             if version.get_version() is not None:
                 self.add_version_check(level=2)
 
     def add_db_session_check(
         self,
-        session: Union[sqlalchemy.orm.scoped_session[sqlalchemy.orm.Session], c2cwsgiutils.db.SessionFactory],
-        query_cb: Optional[Callable[[sqlalchemy.orm.scoped_session[sqlalchemy.orm.Session]], Any]] = None,
+        session: Union[scoped_session, c2cwsgiutils.db.SessionFactory],
+        query_cb: Optional[Callable[[scoped_session], Any]] = None,
         at_least_one_model: Optional[object] = None,
         level: int = 1,
         engine_type: EngineType = EngineType.READ_AND_WRITE,
     ) -> None:
         """
         Check a DB session is working. You can specify either query_cb or at_least_one_model.
 
@@ -219,15 +235,15 @@
         for binding in _get_bindings(session, engine_type):
             name, cb = self._create_db_engine_check(binding, query_cb)
             assert name
             self._checks.append((name, cb, level))
 
     def add_alembic_check(
         self,
-        session: sqlalchemy.orm.scoped_session[sqlalchemy.orm.Session],
+        session: scoped_session,
         alembic_ini_path: str,
         level: int = 2,
         name: str = "alembic",
         version_schema: Optional[str] = None,
         version_table: Optional[str] = None,
     ) -> None:
         """
@@ -255,15 +271,15 @@
         assert version_schema
 
         if version_table is None:
             version_table = config.get(name, "version_table", fallback="alembic_version")
         assert version_table
 
         class _Check:
-            def __init__(self, session: sqlalchemy.orm.scoped_session[sqlalchemy.orm.Session]) -> None:
+            def __init__(self, session: scoped_session) -> None:
                 self.session = session
 
             def __call__(self, request: pyramid.request.Request) -> str:
                 assert version_schema
                 assert version_table
                 for binding in _get_bindings(self.session, EngineType.READ_AND_WRITE):
                     with binding as binded_session:
@@ -499,15 +515,15 @@
             if is_auth or os.environ.get("DEVELOPMENT", "0") != "0":
                 failure["stacktrace"] = traceback.format_exc()
             results["failures"][name] = failure
 
     @staticmethod
     def _create_db_engine_check(
         binding: _Binding,
-        query_cb: Callable[[sqlalchemy.orm.scoped_session[sqlalchemy.orm.Session]], None],
+        query_cb: Callable[[scoped_session], None],
     ) -> Tuple[str, Callable[[pyramid.request.Request], None]]:
         def check(request: pyramid.request.Request) -> None:
             with binding as session:
                 if stats.USE_TAGS:
                     key = ["sql", "manual", "health_check", "db"]
                     tags: Optional[Dict[str, str]] = {"con": binding.name()}
                 else:
@@ -515,16 +531,16 @@
                     tags = None
                 with stats.timer_context(key, tags):
                     return query_cb(session)
 
         return "db_engine_" + binding.name(), check
 
     @staticmethod
-    def _at_least_one(model: Any) -> Callable[[sqlalchemy.orm.scoped_session[sqlalchemy.orm.Session]], Any]:
-        def query(session: sqlalchemy.orm.scoped_session[sqlalchemy.orm.Session]) -> None:
+    def _at_least_one(model: Any) -> Callable[[scoped_session], Any]:
+        def query(session: scoped_session) -> None:
             result = session.query(model).first()
             if result is None:
                 raise HTTPNotFound(model.__name__ + " record not found")
 
         return query
```

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/index.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/index.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/loader.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/loader.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/logging_view.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/logging_view.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/metrics.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/metrics.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/models_graph.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/models_graph.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/pretty_json.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/pretty_json.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/profiler.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/profiler.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/prometheus.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/prometheus.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/pyramid.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/pyramid.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/pyramid_logging.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/pyramid_logging.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/redis_stats.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/redis_stats.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/redis_utils.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/redis_utils.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/request_tracking/__init__.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/request_tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/request_tracking/_sql.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/request_tracking/_sql.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/scripts/check_es.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/scripts/check_es.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/scripts/genversion.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/scripts/genversion.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/scripts/stats_db.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/scripts/stats_db.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 #!/usr/bin/env python3
 """Emits statsd gauges for every tables of a database."""
 import argparse
 import logging
 import os
 import sys
 import time
-from typing import Dict, List, Optional
+from typing import TYPE_CHECKING, Dict, List, Optional
 
 import sqlalchemy
 import sqlalchemy.exc
 import sqlalchemy.orm
 import transaction
 from zope.sqlalchemy import register
 
 import c2cwsgiutils.setup_process
 from c2cwsgiutils import stats
 from c2cwsgiutils.prometheus import PushgatewayGroupPublisher
 
+if TYPE_CHECKING:
+    scoped_session = sqlalchemy.orm.scoped_session[sqlalchemy.orm.Session]
+else:
+    scoped_session = sqlalchemy.orm.scoped_session
+
 LOG = logging.getLogger(__name__)
 
 
 def _parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(description=__doc__)
     c2cwsgiutils.setup_process.fill_arguments(parser)
     parser.add_argument("--db", type=str, required=True, help="DB connection string")
@@ -96,29 +101,29 @@
 
     def report_error(self) -> None:
         if self._error is not None:
             raise self._error
 
 
 def do_table(
-    session: sqlalchemy.orm.scoped_session[sqlalchemy.orm.Session],
+    session: scoped_session,
     schema: str,
     table: str,
     reporter: Reporter,
 ) -> None:
     """Do the stats on a table."""
     _do_table_count(reporter, schema, session, table)
     _do_table_size(reporter, schema, session, table)
     _do_indexes(reporter, schema, session, table)
 
 
 def _do_indexes(
     reporter: Reporter,
     schema: str,
-    session: sqlalchemy.orm.scoped_session[sqlalchemy.orm.Session],
+    session: scoped_session,
     table: str,
 ) -> None:
     for index_name, size_main, size_fsm, number_of_scans, tuples_read, tuples_fetched in session.execute(
         sqlalchemy.text(
             """
     SELECT
          foo.indexname,
@@ -157,15 +162,15 @@
                 tags={"schema": schema, "table": table, "index": index_name, "action": action},
             )
 
 
 def _do_table_size(
     reporter: Reporter,
     schema: str,
-    session: sqlalchemy.orm.scoped_session[sqlalchemy.orm.Session],
+    session: scoped_session,
     table: str,
 ) -> None:
     result = session.execute(
         sqlalchemy.text(
             """
     SELECT pg_table_size(c.oid) AS total_bytes
     FROM pg_class c
@@ -180,15 +185,15 @@
     (size,) = result
     reporter.do_report([schema, table], size, kind="size", tags={"schema": schema, "table": table})
 
 
 def _do_table_count(
     reporter: Reporter,
     schema: str,
-    session: sqlalchemy.orm.scoped_session[sqlalchemy.orm.Session],
+    session: scoped_session,
     table: str,
 ) -> None:
     # We request and estimation of the count as a real count is very slow on big tables
     # and seems to cause replicatin lags. This estimate is updated on ANALYZE and VACUUM.
     result = session.execute(
         sqlalchemy.text(  # nosec
             "SELECT reltuples::bigint AS count FROM pg_class "
@@ -197,17 +202,15 @@
         )
     ).fetchone()
     assert result is not None
     (count,) = result
     reporter.do_report([schema, table], count, kind="count", tags={"schema": schema, "table": table})
 
 
-def do_extra(
-    session: sqlalchemy.orm.scoped_session[sqlalchemy.orm.Session], extra: str, reporter: Reporter
-) -> None:
+def do_extra(session: scoped_session, extra: str, reporter: Reporter) -> None:
     """Do an extra report."""
     for metric, count in session.execute(sqlalchemy.text(extra)):
         reporter.do_report(str(metric).split("."), count, kind="count", tags={"metric": metric})
 
 
 def _do_dtats_db(args: argparse.Namespace) -> None:
     reporter = Reporter(args)
```

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/scripts/test_print.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/scripts/test_print.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/sentry.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/sentry.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/services.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/services.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/setup_process.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/setup_process.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/sql_profiler/__init__.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/sql_profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/sql_profiler/_impl.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/sql_profiler/_impl.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/sqlalchemylogger/README.md` & `c2cwsgiutils-5.2.2/c2cwsgiutils/sqlalchemylogger/README.md`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/sqlalchemylogger/_filters.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/sqlalchemylogger/_filters.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/sqlalchemylogger/_models.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/sqlalchemylogger/_models.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/sqlalchemylogger/handlers.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/sqlalchemylogger/handlers.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/stats.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/stats.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/stats_pyramid/__init__.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/stats_pyramid/__init__.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/stats_pyramid/_db_spy.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/stats_pyramid/_db_spy.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/stats_pyramid/_pyramid_spy.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/stats_pyramid/_pyramid_spy.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/stats_pyramid/_views.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/stats_pyramid/_views.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/c2cwsgiutils/version.py` & `c2cwsgiutils-5.2.2/c2cwsgiutils/version.py`

 * *Files identical despite different names*

### Comparing `c2cwsgiutils-5.2.1/pyproject.toml` & `c2cwsgiutils-5.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 warn_redundant_casts = true
 warn_unused_ignores = true
 warn_return_any = true
 strict = true
 
 [tool.poetry]
 name = "c2cwsgiutils"
-version = "5.2.1"
+version = "5.2.2"
 description = "Common utilities for Camptocamp WSGI applications"
 readme = "README.md"
 authors = ["Camptocamp <info@camptocamp.com>"]
 keywords = ["geo", "gis", "sqlalchemy", "orm", "wsgi"]
 repository = "https://github.com/camptocamp/c2cwsgiutils"
 license = "BSD-2-Clause"
 classifiers = [
@@ -66,29 +66,29 @@
 client_info = "c2cwsgiutils.client_info:filter_factory"
 sentry = "c2cwsgiutils.sentry:filter_factory"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 requests = { version = "2.28.2" }
 pyyaml = { version = "6.0" }
-alembic = { version = "1.9.2", optional = true }
+alembic = { version = "1.9.4", optional = true }
 boltons = { version = "21.0.0", optional = true }
 cornice = { version = "6.0.1", optional = true }
 redis = { version = "4.4.2", optional = true }
 gunicorn = { version = "20.1.0", optional = true }
 lxml = { version = "4.9.2", optional = true }
 netifaces = { version = "0.11.0", optional = true }
 objgraph = { version = "3.5.0", optional = true }
 psycopg2 = { version = "2.9.5", optional = true }
 pyramid = { version = "2.0.1", optional = true }
 pyramid-tm = { version = "2.5", optional = true }
 sentry-sdk = { version = "1.14.0", optional = true }
 ujson = { version = "5.7.0", optional = true }
 cee_syslog_handler = { version = "0.6.0", optional = true }
-SQLAlchemy = { version = "2.0.0", optional = true }
+SQLAlchemy = { version = "2.0.4", optional = true }
 SQLAlchemy-Utils = { version = "0.39.0", optional = true }
 "zope.interface" = { version = "5.5.2", optional = true }
 "zope.sqlalchemy" = { version = "1.6", optional = true }
 pyjwt = { version = "2.6.0", optional = true }
 requests-oauthlib = { version = "1.3.1", optional = true }
 waitress = { version = "2.1.2", optional = true }
 scikit-image = { version = "0.19.3", optional = true }
@@ -148,19 +148,19 @@
 # pylint = { version = "2.15.6" }
 prospector = { extras = ["with_bandit", "with_mypy", "with_pyroma"], version = "1.8.4" }
 coverage = "7.1.0"
 junit2html = "30.1.3"
 pytest = "7.2.1"
 pytest-cov = "4.0.0"
 pytest-html = "3.2.0"
-types-pyyaml = "6.0.12.3"
-types-requests = "2.28.11.8"
-types-redis = "4.4.0.4"
-types-ujson = "5.7.0.0"
-types-python-dateutil = "2.8.19.6"
+types-pyyaml = "6.0.12.8"
+types-requests = "2.28.11.15"
+types-redis = "4.4.0.6"
+types-ujson = "5.7.0.1"
+types-python-dateutil = "2.8.19.10"
 typing_extensions = "4.4.0"
 
 [build-system]
 requires = [
   "poetry-core>=1.0.0",
   "poetry-dynamic-versioning[plugin]",
   "poetry-plugin-tweak-dependencies-version"
```

### Comparing `c2cwsgiutils-5.2.1/PKG-INFO` & `c2cwsgiutils-5.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c2cwsgiutils
-Version: 5.2.1
+Version: 5.2.2
 Summary: Common utilities for Camptocamp WSGI applications
 Home-page: https://github.com/camptocamp/c2cwsgiutils
 License: BSD-2-Clause
 Keywords: geo,gis,sqlalchemy,orm,wsgi
 Author: Camptocamp
 Author-email: info@camptocamp.com
 Requires-Python: >=3.8,<4.0
```

