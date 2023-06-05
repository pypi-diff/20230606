# Comparing `tmp/elastic-apm-6.9.0.tar.gz` & `tmp/elastic-apm-6.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/elastic-apm-6.9.0.tar", last modified: Wed Mar 30 00:38:07 2022, max compression
+gzip compressed data, was "dist/elastic-apm-6.9.1.tar", last modified: Wed Mar 30 14:52:58 2022, max compression
```

## Comparing `elastic-apm-6.9.0.tar` & `elastic-apm-6.9.1.tar`

### file list

```diff
@@ -1,196 +1,196 @@
-drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 00:38:07.000000 elastic-apm-6.9.0/
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)      110 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/MANIFEST.in
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3409 2022-03-30 00:38:07.000000 elastic-apm-6.9.0/PKG-INFO
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1639 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/README.rst
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)      243 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/pyproject.toml
-drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 00:38:07.000000 elastic-apm-6.9.0/elastic_apm.egg-info/
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)       11 2022-03-30 00:38:06.000000 elastic-apm-6.9.0/elastic_apm.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)      196 2022-03-30 00:38:06.000000 elastic-apm-6.9.0/elastic_apm.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3409 2022-03-30 00:38:06.000000 elastic-apm-6.9.0/elastic_apm.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)        1 2022-03-30 00:38:06.000000 elastic-apm-6.9.0/elastic_apm.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)        1 2022-03-30 00:38:06.000000 elastic-apm-6.9.0/elastic_apm.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     6109 2022-03-30 00:38:06.000000 elastic-apm-6.9.0/elastic_apm.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3722 2022-03-30 00:38:07.000000 elastic-apm-6.9.0/setup.cfg
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1587 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/LICENSE
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     5666 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/setup.py
-drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 00:38:07.000000 elastic-apm-6.9.0/elasticapm/
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)    27813 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/base.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1658 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/version.py
-drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 00:38:07.000000 elastic-apm-6.9.0/elasticapm/transport/
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3919 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/transport/http_base.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)    17151 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/transport/base.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1615 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/transport/__init__.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1916 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/transport/http_urllib3.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1840 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/transport/exceptions.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)    10187 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/transport/http.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2767 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/__init__.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2944 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/middleware.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)    11210 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/processors.py
-drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 00:38:07.000000 elastic-apm-6.9.0/elasticapm/context/
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2757 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/context/base.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2631 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/context/__init__.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3690 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/context/contextvars.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3621 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/context/threadlocal.py
-drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 00:38:07.000000 elastic-apm-6.9.0/elasticapm/instrumentation/
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1591 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/__init__.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     6247 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/register.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2123 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/control.py
-drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 00:38:07.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3795 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/cassandra.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2224 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/pyodbc.py
-drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 00:38:07.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/django/
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1591 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/django/__init__.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2926 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/django/template.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)    11103 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/base.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1591 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/__init__.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     5517 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/httplib2.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2875 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/requests.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2123 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/jinja2.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     4308 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/redis.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2492 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/mysql_connector.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3450 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/sqlite.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)    18231 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/azure.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2520 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/mysql.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2239 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/pymysql.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3507 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/pylibmc.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     9953 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/dbapi2.py
-drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 00:38:07.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/asyncio/
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3201 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/asyncio/aiopg.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     4308 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/asyncio/aioredis.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1852 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/asyncio/base.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1591 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/asyncio/__init__.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     4521 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/asyncio/aiohttp_client.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2132 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/asyncio/sleep.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3775 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/asyncio/asyncpg.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3532 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/asyncio/elasticsearch.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3047 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/asyncio/aiomysql.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     4455 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/graphql.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2105 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/zlib.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     5210 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/elasticsearch.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3243 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/python_memcached.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     6348 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/urllib3.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     4134 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/pymemcache.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     8918 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/botocore.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     5949 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/pymongo.py
-drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 00:38:07.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/httpx/
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1591 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/httpx/__init__.py
-drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 00:38:07.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/httpx/sync/
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1591 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/httpx/sync/__init__.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2761 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/httpx/sync/httpx.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     4606 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/httpx/sync/httpcore.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3679 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/httpx/utils.py
-drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 00:38:07.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/httpx/async/
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1591 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/httpx/async/__init__.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2835 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/httpx/async/httpx.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     5052 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/httpx/async/httpcore.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     5929 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/psycopg2.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     5330 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/urllib.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     5909 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/tornado.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2890 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/instrumentation/packages/pymssql.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)    46159 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/traces.py
-drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 00:38:07.000000 elastic-apm-6.9.0/elasticapm/conf/
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3557 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/conf/constants.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)    33272 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/conf/__init__.py
-drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 00:38:07.000000 elastic-apm-6.9.0/elasticapm/handlers/
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)    10430 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/handlers/logging.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     4275 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/handlers/logbook.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1588 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/handlers/__init__.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2584 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/handlers/structlog.py
-drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 00:38:07.000000 elastic-apm-6.9.0/elasticapm/utils/
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2038 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/utils/logging.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     7099 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/utils/__init__.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     9859 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/utils/disttracing.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     9013 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/utils/encoding.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     4480 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/utils/threading.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     7562 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/utils/cloud.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     4927 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/utils/wsgi.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2536 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/utils/deprecation.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3663 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/utils/compat.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     4432 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/utils/cgroup.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)    13233 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/utils/stacks.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2520 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/utils/json_encoder.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3760 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/utils/time.py
-drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 00:38:07.000000 elastic-apm-6.9.0/elasticapm/utils/wrapt/
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)    20127 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/utils/wrapt/decorators.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)      699 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/utils/wrapt/__init__.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)    81870 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/utils/wrapt/_wrappers.c
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)    32389 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/utils/wrapt/wrappers.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     7726 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/utils/wrapt/importer.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     4059 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/utils/wrapt/arguments.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2348 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/utils/module_import.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     8212 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/events.py
-drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 00:38:07.000000 elastic-apm-6.9.0/elasticapm/metrics/
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1591 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/metrics/__init__.py
-drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 00:38:07.000000 elastic-apm-6.9.0/elasticapm/metrics/sets/
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1591 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/metrics/sets/__init__.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2902 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/metrics/sets/cpu_psutil.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)    11817 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/metrics/sets/cpu_linux.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1752 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/metrics/sets/breakdown.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     5454 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/metrics/sets/prometheus.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1870 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/metrics/sets/cpu.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)    18491 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/metrics/base_metrics.py
-drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 00:38:07.000000 elastic-apm-6.9.0/elasticapm/contrib/
-drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 00:38:07.000000 elastic-apm-6.9.0/elasticapm/contrib/django/
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1801 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/django/__init__.py
-drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 00:38:07.000000 elastic-apm-6.9.0/elasticapm/contrib/django/celery/
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1588 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/django/celery/__init__.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1862 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/django/celery/models.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     4454 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/django/utils.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3410 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/django/handlers.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     7943 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/django/apps.py
-drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 00:38:07.000000 elastic-apm-6.9.0/elasticapm/contrib/django/middleware/
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     9379 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/django/middleware/__init__.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2302 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/django/middleware/wsgi.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2244 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/django/context_processors.py
-drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 00:38:07.000000 elastic-apm-6.9.0/elasticapm/contrib/django/management/
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1591 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/django/management/__init__.py
-drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 00:38:07.000000 elastic-apm-6.9.0/elasticapm/contrib/django/management/commands/
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1519 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/django/management/commands/__init__.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)    13175 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/django/management/commands/elasticapm.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)    11720 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/django/client.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1591 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/__init__.py
-drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 00:38:07.000000 elastic-apm-6.9.0/elasticapm/contrib/celery/
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     5754 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/celery/__init__.py
-drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 00:38:07.000000 elastic-apm-6.9.0/elasticapm/contrib/sanic/
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2745 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/sanic/sanic_types.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     4282 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/sanic/patch.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)    15973 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/sanic/__init__.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     6108 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/sanic/utils.py
-drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 00:38:07.000000 elastic-apm-6.9.0/elasticapm/contrib/tornado/
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3097 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/tornado/__init__.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3385 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/tornado/utils.py
-drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 00:38:07.000000 elastic-apm-6.9.0/elasticapm/contrib/asyncio/
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1591 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/asyncio/__init__.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3338 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/asyncio/traces.py
-drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 00:38:07.000000 elastic-apm-6.9.0/elasticapm/contrib/zerorpc/
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3902 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/zerorpc/__init__.py
-drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 00:38:07.000000 elastic-apm-6.9.0/elasticapm/contrib/twisted/
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2462 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/twisted/__init__.py
-drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 00:38:07.000000 elastic-apm-6.9.0/elasticapm/contrib/starlette/
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)    10279 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/starlette/__init__.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     4853 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/starlette/utils.py
-drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 00:38:07.000000 elastic-apm-6.9.0/elasticapm/contrib/aiohttp/
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2346 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/aiohttp/__init__.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     5955 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/aiohttp/middleware.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2647 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/aiohttp/utils.py
-drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 00:38:07.000000 elastic-apm-6.9.0/elasticapm/contrib/opentelemetry/
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1644 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/opentelemetry/__init__.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3044 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/opentelemetry/utils.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     5619 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/opentelemetry/context.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)    12751 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/opentelemetry/span.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)    13192 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/opentelemetry/trace.py
-drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 00:38:07.000000 elastic-apm-6.9.0/elasticapm/contrib/opentracing/
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1886 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/opentracing/__init__.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     5879 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/opentracing/span.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     6245 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/opentracing/tracer.py
-drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 00:38:07.000000 elastic-apm-6.9.0/elasticapm/contrib/serverless/
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1983 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/serverless/__init__.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)    19224 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/serverless/aws.py
-drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 00:38:07.000000 elastic-apm-6.9.0/elasticapm/contrib/pylons/
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2162 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/pylons/__init__.py
-drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 00:38:07.000000 elastic-apm-6.9.0/elasticapm/contrib/flask/
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     8570 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/flask/__init__.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3614 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/flask/utils.py
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1838 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/paste.py
-drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 00:38:07.000000 elastic-apm-6.9.0/elasticapm/contrib/rq/
--rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2402 2022-03-30 00:17:38.000000 elastic-apm-6.9.0/elasticapm/contrib/rq/__init__.py
+drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)      110 2022-03-30 14:32:05.000000 elastic-apm-6.9.1/MANIFEST.in
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3409 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/PKG-INFO
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1639 2022-03-30 14:32:05.000000 elastic-apm-6.9.1/README.rst
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)      243 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/pyproject.toml
+drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/elastic_apm.egg-info/
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)       11 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/elastic_apm.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)      196 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/elastic_apm.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3409 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/elastic_apm.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)        1 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/elastic_apm.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)        1 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/elastic_apm.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     6109 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/elastic_apm.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3722 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/setup.cfg
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1587 2022-03-30 14:32:05.000000 elastic-apm-6.9.1/LICENSE
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     5666 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/setup.py
+drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/elasticapm/
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)    27813 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/base.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1658 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/version.py
+drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/elasticapm/transport/
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3919 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/transport/http_base.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)    17151 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/transport/base.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1615 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/transport/__init__.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1916 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/transport/http_urllib3.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1840 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/transport/exceptions.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)    10187 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/transport/http.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2767 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/__init__.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2944 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/middleware.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)    11210 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/processors.py
+drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/elasticapm/context/
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2757 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/context/base.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2631 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/context/__init__.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3690 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/context/contextvars.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3621 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/context/threadlocal.py
+drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/elasticapm/instrumentation/
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1591 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/__init__.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     6247 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/register.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2123 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/control.py
+drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3795 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/cassandra.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2224 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/pyodbc.py
+drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/django/
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1591 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/django/__init__.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2926 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/django/template.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)    11103 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/base.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1591 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/__init__.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     5517 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/httplib2.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2875 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/requests.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2123 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/jinja2.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     4308 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/redis.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2492 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/mysql_connector.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3450 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/sqlite.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)    18231 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/azure.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2520 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/mysql.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2239 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/pymysql.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3507 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/pylibmc.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     9953 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/dbapi2.py
+drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/asyncio/
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3201 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/asyncio/aiopg.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     4308 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/asyncio/aioredis.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1852 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/asyncio/base.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1591 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/asyncio/__init__.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     4521 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/asyncio/aiohttp_client.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2132 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/asyncio/sleep.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3775 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/asyncio/asyncpg.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3532 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/asyncio/elasticsearch.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3047 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/asyncio/aiomysql.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     4455 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/graphql.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2105 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/zlib.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     5210 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/elasticsearch.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3243 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/python_memcached.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     6348 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/urllib3.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     4134 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/pymemcache.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     8918 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/botocore.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     5949 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/pymongo.py
+drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/httpx/
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1591 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/httpx/__init__.py
+drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/httpx/sync/
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1591 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/httpx/sync/__init__.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2761 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/httpx/sync/httpx.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     4606 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/httpx/sync/httpcore.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3679 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/httpx/utils.py
+drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/httpx/async/
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1591 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/httpx/async/__init__.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2835 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/httpx/async/httpx.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     5052 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/httpx/async/httpcore.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     5929 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/psycopg2.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     5330 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/urllib.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     5909 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/tornado.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2890 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/instrumentation/packages/pymssql.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)    46163 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/traces.py
+drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/elasticapm/conf/
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3557 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/conf/constants.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)    33272 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/conf/__init__.py
+drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/elasticapm/handlers/
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)    10430 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/handlers/logging.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     4275 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/handlers/logbook.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1588 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/handlers/__init__.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2584 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/handlers/structlog.py
+drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/elasticapm/utils/
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2038 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/utils/logging.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     7099 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/utils/__init__.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     9859 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/utils/disttracing.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     9013 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/utils/encoding.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     4480 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/utils/threading.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     7562 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/utils/cloud.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     4927 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/utils/wsgi.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2536 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/utils/deprecation.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3663 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/utils/compat.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     4432 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/utils/cgroup.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)    13233 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/utils/stacks.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2520 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/utils/json_encoder.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3760 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/utils/time.py
+drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/elasticapm/utils/wrapt/
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)    20127 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/utils/wrapt/decorators.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)      699 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/utils/wrapt/__init__.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)    81870 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/utils/wrapt/_wrappers.c
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)    32389 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/utils/wrapt/wrappers.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     7726 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/utils/wrapt/importer.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     4059 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/utils/wrapt/arguments.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2348 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/utils/module_import.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     8212 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/events.py
+drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/elasticapm/metrics/
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1591 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/metrics/__init__.py
+drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/elasticapm/metrics/sets/
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1591 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/metrics/sets/__init__.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2902 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/metrics/sets/cpu_psutil.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)    11817 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/metrics/sets/cpu_linux.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1752 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/metrics/sets/breakdown.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     5454 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/metrics/sets/prometheus.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1870 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/metrics/sets/cpu.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)    18491 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/metrics/base_metrics.py
+drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/elasticapm/contrib/
+drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/elasticapm/contrib/django/
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1801 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/django/__init__.py
+drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/elasticapm/contrib/django/celery/
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1588 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/django/celery/__init__.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1862 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/django/celery/models.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     4454 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/django/utils.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3410 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/django/handlers.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     7943 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/django/apps.py
+drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/elasticapm/contrib/django/middleware/
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     9379 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/django/middleware/__init__.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2302 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/django/middleware/wsgi.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2244 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/django/context_processors.py
+drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/elasticapm/contrib/django/management/
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1591 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/django/management/__init__.py
+drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/elasticapm/contrib/django/management/commands/
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1519 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/django/management/commands/__init__.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)    13175 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/django/management/commands/elasticapm.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)    11720 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/django/client.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1591 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/__init__.py
+drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/elasticapm/contrib/celery/
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     5754 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/celery/__init__.py
+drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/elasticapm/contrib/sanic/
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2745 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/sanic/sanic_types.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     4282 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/sanic/patch.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)    15973 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/sanic/__init__.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     6108 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/sanic/utils.py
+drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/elasticapm/contrib/tornado/
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3097 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/tornado/__init__.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3385 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/tornado/utils.py
+drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/elasticapm/contrib/asyncio/
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1591 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/asyncio/__init__.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3338 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/asyncio/traces.py
+drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/elasticapm/contrib/zerorpc/
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3902 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/zerorpc/__init__.py
+drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/elasticapm/contrib/twisted/
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2462 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/twisted/__init__.py
+drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/elasticapm/contrib/starlette/
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)    10279 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/starlette/__init__.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     4853 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/starlette/utils.py
+drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/elasticapm/contrib/aiohttp/
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2346 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/aiohttp/__init__.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     5955 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/aiohttp/middleware.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2647 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/aiohttp/utils.py
+drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/elasticapm/contrib/opentelemetry/
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1644 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/opentelemetry/__init__.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3044 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/opentelemetry/utils.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     5619 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/opentelemetry/context.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)    12751 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/opentelemetry/span.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)    13192 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/opentelemetry/trace.py
+drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/elasticapm/contrib/opentracing/
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1886 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/opentracing/__init__.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     5879 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/opentracing/span.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     6245 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/opentracing/tracer.py
+drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/elasticapm/contrib/serverless/
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1983 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/serverless/__init__.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)    19224 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/serverless/aws.py
+drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/elasticapm/contrib/pylons/
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2162 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/pylons/__init__.py
+drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/elasticapm/contrib/flask/
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     8570 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/flask/__init__.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     3614 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/flask/utils.py
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     1838 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/paste.py
+drwxr-xr-x   0 jenkins   (1165) jenkins   (1166)        0 2022-03-30 14:52:58.000000 elastic-apm-6.9.1/elasticapm/contrib/rq/
+-rw-r--r--   0 jenkins   (1165) jenkins   (1166)     2402 2022-03-30 14:32:06.000000 elastic-apm-6.9.1/elasticapm/contrib/rq/__init__.py
```

### Comparing `elastic-apm-6.9.0/PKG-INFO` & `elastic-apm-6.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elastic-apm
-Version: 6.9.0
+Version: 6.9.1
 Summary: The official Python module for Elastic APM
 Home-page: https://github.com/elastic/apm-agent-python
 Author: Elastic, Inc
 License: BSD
 Project-URL: Release notes, https://www.elastic.co/guide/en/apm/agent/python/current/release-notes.html
 Project-URL: Documentation, https://www.elastic.co/guide/en/apm/agent/python/current/index.html
 Project-URL: Tracker, https://github.com/elastic/apm-agent-python/issues
```

### Comparing `elastic-apm-6.9.0/README.rst` & `elastic-apm-6.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elastic_apm.egg-info/PKG-INFO` & `elastic-apm-6.9.1/elastic_apm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elastic-apm
-Version: 6.9.0
+Version: 6.9.1
 Summary: The official Python module for Elastic APM
 Home-page: https://github.com/elastic/apm-agent-python
 Author: Elastic, Inc
 License: BSD
 Project-URL: Release notes, https://www.elastic.co/guide/en/apm/agent/python/current/release-notes.html
 Project-URL: Documentation, https://www.elastic.co/guide/en/apm/agent/python/current/index.html
 Project-URL: Tracker, https://github.com/elastic/apm-agent-python/issues
```

### Comparing `elastic-apm-6.9.0/elastic_apm.egg-info/SOURCES.txt` & `elastic-apm-6.9.1/elastic_apm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/setup.cfg` & `elastic-apm-6.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/LICENSE` & `elastic-apm-6.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/setup.py` & `elastic-apm-6.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/base.py` & `elastic-apm-6.9.1/elasticapm/base.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/version.py` & `elastic-apm-6.9.1/elasticapm/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,9 +24,9 @@
 #  FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 #  DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 #  SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 #  CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 #  OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 #  OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = (6, 9, 0)
+__version__ = (6, 9, 1)
 VERSION = ".".join(map(str, __version__))
```

### Comparing `elastic-apm-6.9.0/elasticapm/transport/http_base.py` & `elastic-apm-6.9.1/elasticapm/transport/http_base.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/transport/base.py` & `elastic-apm-6.9.1/elasticapm/transport/base.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/transport/__init__.py` & `elastic-apm-6.9.1/elasticapm/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/transport/http_urllib3.py` & `elastic-apm-6.9.1/elasticapm/transport/http_urllib3.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/transport/exceptions.py` & `elastic-apm-6.9.1/elasticapm/transport/exceptions.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/transport/http.py` & `elastic-apm-6.9.1/elasticapm/transport/http.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/__init__.py` & `elastic-apm-6.9.1/elasticapm/__init__.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/middleware.py` & `elastic-apm-6.9.1/elasticapm/middleware.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/processors.py` & `elastic-apm-6.9.1/elasticapm/processors.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/context/base.py` & `elastic-apm-6.9.1/elasticapm/context/base.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/context/__init__.py` & `elastic-apm-6.9.1/elasticapm/context/__init__.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/context/contextvars.py` & `elastic-apm-6.9.1/elasticapm/context/contextvars.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/context/threadlocal.py` & `elastic-apm-6.9.1/elasticapm/context/threadlocal.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/__init__.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/__init__.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/register.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/register.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/control.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/control.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/cassandra.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/cassandra.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/pyodbc.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/pyodbc.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/django/__init__.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/django/__init__.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/django/template.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/django/template.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/base.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/base.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/__init__.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/httplib2.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/httplib2.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/requests.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/requests.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/jinja2.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/jinja2.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/redis.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/redis.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/mysql_connector.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/mysql_connector.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/sqlite.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/sqlite.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/azure.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/azure.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/mysql.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/mysql.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/pymysql.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/pymysql.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/pylibmc.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/pylibmc.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/dbapi2.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/dbapi2.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/asyncio/aiopg.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/asyncio/aiopg.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/asyncio/aioredis.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/asyncio/aioredis.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/asyncio/base.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/asyncio/base.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/asyncio/__init__.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/asyncio/aiohttp_client.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/asyncio/aiohttp_client.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/asyncio/sleep.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/asyncio/sleep.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/asyncio/asyncpg.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/asyncio/asyncpg.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/asyncio/elasticsearch.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/asyncio/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/asyncio/aiomysql.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/asyncio/aiomysql.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/graphql.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/graphql.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/zlib.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/zlib.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/elasticsearch.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/python_memcached.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/python_memcached.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/urllib3.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/urllib3.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/pymemcache.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/pymemcache.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/botocore.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/botocore.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/pymongo.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/pymongo.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/httpx/__init__.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/httpx/__init__.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/httpx/sync/__init__.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/httpx/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/httpx/sync/httpx.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/httpx/sync/httpx.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/httpx/sync/httpcore.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/httpx/sync/httpcore.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/httpx/utils.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/httpx/utils.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/httpx/async/__init__.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/httpx/async/__init__.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/httpx/async/httpx.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/httpx/async/httpx.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/httpx/async/httpcore.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/httpx/async/httpcore.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/psycopg2.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/psycopg2.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/urllib.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/urllib.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/tornado.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/tornado.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/instrumentation/packages/pymssql.py` & `elastic-apm-6.9.1/elasticapm/instrumentation/packages/pymssql.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/traces.py` & `elastic-apm-6.9.1/elasticapm/traces.py`

 * *Files 1% similar despite different names*

```diff
@@ -573,15 +573,15 @@
                 if "otel_attributes" in self.context:
                     if "otel" not in result:
                         result["otel"] = {"attributes": self.context.pop("otel_attributes")}
                     else:
                         result["otel"]["attributes"] = self.context.pop("otel_attributes")
             else:
                 # Attributes map to labels for older versions
-                attributes = self.context.pop("otel_attributes")
+                attributes = self.context.pop("otel_attributes", {})
                 if attributes and ("tags" not in self.context):
                     self.context["tags"] = {}
                 for key, value in attributes.items():
                     self.context["tags"][key] = value
             result["context"] = self.context
         if self.frames:
             result["stacktrace"] = self.frames
```

### Comparing `elastic-apm-6.9.0/elasticapm/conf/constants.py` & `elastic-apm-6.9.1/elasticapm/conf/constants.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/conf/__init__.py` & `elastic-apm-6.9.1/elasticapm/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/handlers/logging.py` & `elastic-apm-6.9.1/elasticapm/handlers/logging.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/handlers/logbook.py` & `elastic-apm-6.9.1/elasticapm/handlers/logbook.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/handlers/__init__.py` & `elastic-apm-6.9.1/elasticapm/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/handlers/structlog.py` & `elastic-apm-6.9.1/elasticapm/handlers/structlog.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/utils/logging.py` & `elastic-apm-6.9.1/elasticapm/utils/logging.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/utils/__init__.py` & `elastic-apm-6.9.1/elasticapm/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/utils/disttracing.py` & `elastic-apm-6.9.1/elasticapm/utils/disttracing.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/utils/encoding.py` & `elastic-apm-6.9.1/elasticapm/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/utils/threading.py` & `elastic-apm-6.9.1/elasticapm/utils/threading.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/utils/cloud.py` & `elastic-apm-6.9.1/elasticapm/utils/cloud.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/utils/wsgi.py` & `elastic-apm-6.9.1/elasticapm/utils/wsgi.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/utils/deprecation.py` & `elastic-apm-6.9.1/elasticapm/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/utils/compat.py` & `elastic-apm-6.9.1/elasticapm/utils/compat.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/utils/cgroup.py` & `elastic-apm-6.9.1/elasticapm/utils/cgroup.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/utils/stacks.py` & `elastic-apm-6.9.1/elasticapm/utils/stacks.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/utils/json_encoder.py` & `elastic-apm-6.9.1/elasticapm/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/utils/time.py` & `elastic-apm-6.9.1/elasticapm/utils/time.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/utils/wrapt/decorators.py` & `elastic-apm-6.9.1/elasticapm/utils/wrapt/decorators.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/utils/wrapt/__init__.py` & `elastic-apm-6.9.1/elasticapm/utils/wrapt/__init__.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/utils/wrapt/_wrappers.c` & `elastic-apm-6.9.1/elasticapm/utils/wrapt/_wrappers.c`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/utils/wrapt/wrappers.py` & `elastic-apm-6.9.1/elasticapm/utils/wrapt/wrappers.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/utils/wrapt/importer.py` & `elastic-apm-6.9.1/elasticapm/utils/wrapt/importer.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/utils/wrapt/arguments.py` & `elastic-apm-6.9.1/elasticapm/utils/wrapt/arguments.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/utils/module_import.py` & `elastic-apm-6.9.1/elasticapm/utils/module_import.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/events.py` & `elastic-apm-6.9.1/elasticapm/events.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/metrics/__init__.py` & `elastic-apm-6.9.1/elasticapm/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/metrics/sets/__init__.py` & `elastic-apm-6.9.1/elasticapm/metrics/sets/__init__.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/metrics/sets/cpu_psutil.py` & `elastic-apm-6.9.1/elasticapm/metrics/sets/cpu_psutil.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/metrics/sets/cpu_linux.py` & `elastic-apm-6.9.1/elasticapm/metrics/sets/cpu_linux.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/metrics/sets/breakdown.py` & `elastic-apm-6.9.1/elasticapm/metrics/sets/breakdown.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/metrics/sets/prometheus.py` & `elastic-apm-6.9.1/elasticapm/metrics/sets/prometheus.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/metrics/sets/cpu.py` & `elastic-apm-6.9.1/elasticapm/metrics/sets/cpu.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/metrics/base_metrics.py` & `elastic-apm-6.9.1/elasticapm/metrics/base_metrics.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/django/__init__.py` & `elastic-apm-6.9.1/elasticapm/contrib/django/__init__.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/django/celery/__init__.py` & `elastic-apm-6.9.1/elasticapm/contrib/django/celery/__init__.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/django/celery/models.py` & `elastic-apm-6.9.1/elasticapm/contrib/django/celery/models.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/django/utils.py` & `elastic-apm-6.9.1/elasticapm/contrib/django/utils.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/django/handlers.py` & `elastic-apm-6.9.1/elasticapm/contrib/django/handlers.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/django/apps.py` & `elastic-apm-6.9.1/elasticapm/contrib/django/apps.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/django/middleware/__init__.py` & `elastic-apm-6.9.1/elasticapm/contrib/django/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/django/middleware/wsgi.py` & `elastic-apm-6.9.1/elasticapm/contrib/django/middleware/wsgi.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/django/context_processors.py` & `elastic-apm-6.9.1/elasticapm/contrib/django/context_processors.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/django/management/__init__.py` & `elastic-apm-6.9.1/elasticapm/contrib/django/management/__init__.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/django/management/commands/__init__.py` & `elastic-apm-6.9.1/elasticapm/contrib/django/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/django/management/commands/elasticapm.py` & `elastic-apm-6.9.1/elasticapm/contrib/django/management/commands/elasticapm.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/django/client.py` & `elastic-apm-6.9.1/elasticapm/contrib/django/client.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/__init__.py` & `elastic-apm-6.9.1/elasticapm/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/celery/__init__.py` & `elastic-apm-6.9.1/elasticapm/contrib/celery/__init__.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/sanic/sanic_types.py` & `elastic-apm-6.9.1/elasticapm/contrib/sanic/sanic_types.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/sanic/patch.py` & `elastic-apm-6.9.1/elasticapm/contrib/sanic/patch.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/sanic/__init__.py` & `elastic-apm-6.9.1/elasticapm/contrib/sanic/__init__.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/sanic/utils.py` & `elastic-apm-6.9.1/elasticapm/contrib/sanic/utils.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/tornado/__init__.py` & `elastic-apm-6.9.1/elasticapm/contrib/tornado/__init__.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/tornado/utils.py` & `elastic-apm-6.9.1/elasticapm/contrib/tornado/utils.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/asyncio/__init__.py` & `elastic-apm-6.9.1/elasticapm/contrib/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/asyncio/traces.py` & `elastic-apm-6.9.1/elasticapm/contrib/asyncio/traces.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/zerorpc/__init__.py` & `elastic-apm-6.9.1/elasticapm/contrib/zerorpc/__init__.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/twisted/__init__.py` & `elastic-apm-6.9.1/elasticapm/contrib/twisted/__init__.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/starlette/__init__.py` & `elastic-apm-6.9.1/elasticapm/contrib/starlette/__init__.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/starlette/utils.py` & `elastic-apm-6.9.1/elasticapm/contrib/starlette/utils.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/aiohttp/__init__.py` & `elastic-apm-6.9.1/elasticapm/contrib/aiohttp/__init__.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/aiohttp/middleware.py` & `elastic-apm-6.9.1/elasticapm/contrib/aiohttp/middleware.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/aiohttp/utils.py` & `elastic-apm-6.9.1/elasticapm/contrib/aiohttp/utils.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/opentelemetry/__init__.py` & `elastic-apm-6.9.1/elasticapm/contrib/opentelemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/opentelemetry/utils.py` & `elastic-apm-6.9.1/elasticapm/contrib/opentelemetry/utils.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/opentelemetry/context.py` & `elastic-apm-6.9.1/elasticapm/contrib/opentelemetry/context.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/opentelemetry/span.py` & `elastic-apm-6.9.1/elasticapm/contrib/opentelemetry/span.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/opentelemetry/trace.py` & `elastic-apm-6.9.1/elasticapm/contrib/opentelemetry/trace.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/opentracing/__init__.py` & `elastic-apm-6.9.1/elasticapm/contrib/opentracing/__init__.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/opentracing/span.py` & `elastic-apm-6.9.1/elasticapm/contrib/opentracing/span.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/opentracing/tracer.py` & `elastic-apm-6.9.1/elasticapm/contrib/opentracing/tracer.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/serverless/__init__.py` & `elastic-apm-6.9.1/elasticapm/contrib/serverless/__init__.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/serverless/aws.py` & `elastic-apm-6.9.1/elasticapm/contrib/serverless/aws.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/pylons/__init__.py` & `elastic-apm-6.9.1/elasticapm/contrib/pylons/__init__.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/flask/__init__.py` & `elastic-apm-6.9.1/elasticapm/contrib/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/flask/utils.py` & `elastic-apm-6.9.1/elasticapm/contrib/flask/utils.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/paste.py` & `elastic-apm-6.9.1/elasticapm/contrib/paste.py`

 * *Files identical despite different names*

### Comparing `elastic-apm-6.9.0/elasticapm/contrib/rq/__init__.py` & `elastic-apm-6.9.1/elasticapm/contrib/rq/__init__.py`

 * *Files identical despite different names*

