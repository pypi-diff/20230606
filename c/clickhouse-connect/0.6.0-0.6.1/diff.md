# Comparing `tmp/clickhouse-connect-0.6.0.tar.gz` & `tmp/clickhouse-connect-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickhouse-connect-0.6.0.tar", last modified: Tue Jun  6 00:37:16 2023, max compression
+gzip compressed data, was "clickhouse-connect-0.6.1.tar", last modified: Tue Jun  6 14:00:08 2023, max compression
```

## Comparing `clickhouse-connect-0.6.0.tar` & `clickhouse-connect-0.6.1.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:37:16.911337 clickhouse-connect-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-06-06 00:37:16.911337 clickhouse-connect-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:37:16.903337 clickhouse-connect-0.6.0/clickhouse_connect/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:37:16.907337 clickhouse-connect-0.6.0/clickhouse_connect/cc_sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/cc_sqlalchemy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:37:16.907337 clickhouse-connect-0.6.0/clickhouse_connect/cc_sqlalchemy/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/cc_sqlalchemy/datatypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/cc_sqlalchemy/datatypes/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13547 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/cc_sqlalchemy/datatypes/sqltypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:37:16.907337 clickhouse-connect-0.6.0/clickhouse_connect/cc_sqlalchemy/ddl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/cc_sqlalchemy/ddl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/cc_sqlalchemy/ddl/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/cc_sqlalchemy/ddl/tableengine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/cc_sqlalchemy/dialect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/cc_sqlalchemy/inspector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:37:16.907337 clickhouse-connect-0.6.0/clickhouse_connect/cc_sqlalchemy/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/cc_sqlalchemy/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/cc_sqlalchemy/sql/ddlcompiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/cc_sqlalchemy/sql/preparer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:37:16.907337 clickhouse-connect-0.6.0/clickhouse_connect/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/datatypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14785 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/datatypes/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/datatypes/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/datatypes/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/datatypes/network.py
--rw-r--r--   0 runner    (1001) docker     (123)    11140 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/datatypes/numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/datatypes/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/datatypes/special.py
--rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/datatypes/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     8548 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/datatypes/temporal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:37:16.907337 clickhouse-connect-0.6.0/clickhouse_connect/dbapi/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/dbapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/dbapi/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/dbapi/cursor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:37:16.911337 clickhouse-connect-0.6.0/clickhouse_connect/driver/
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/driver/buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    38874 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/driver/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/driver/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/driver/compression.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/driver/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/driver/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/driver/ctypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/driver/dataconv.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/driver/ddl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/driver/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/driver/external.py
--rw-r--r--   0 runner    (1001) docker     (123)    21102 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/driver/httpclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/driver/httputil.py
--rw-r--r--   0 runner    (1001) docker     (123)     8426 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/driver/insert.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/driver/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/driver/npconv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/driver/npquery.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/driver/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/driver/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    20182 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/driver/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/driver/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/driver/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/driver/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:37:16.911337 clickhouse-connect-0.6.0/clickhouse_connect/driverc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/driverc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/json_impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:37:16.911337 clickhouse-connect-0.6.0/clickhouse_connect/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/tools/datagen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/clickhouse_connect/tools/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 00:37:16.907337 clickhouse-connect-0.6.0/clickhouse_connect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-06-06 00:37:16.000000 clickhouse-connect-0.6.0/clickhouse_connect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-06-06 00:37:16.000000 clickhouse-connect-0.6.0/clickhouse_connect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 00:37:16.000000 clickhouse-connect-0.6.0/clickhouse_connect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-06 00:37:16.000000 clickhouse-connect-0.6.0/clickhouse_connect.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-06 00:37:16.000000 clickhouse-connect-0.6.0/clickhouse_connect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-06 00:37:16.000000 clickhouse-connect-0.6.0/clickhouse_connect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 00:37:16.911337 clickhouse-connect-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-06-06 00:37:14.000000 clickhouse-connect-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:00:08.738327 clickhouse-connect-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-06 14:00:08.738327 clickhouse-connect-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:00:08.730327 clickhouse-connect-0.6.1/clickhouse_connect/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:00:08.730327 clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:00:08.730327 clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/datatypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/datatypes/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13547 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/datatypes/sqltypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:00:08.734327 clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/ddl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/ddl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/ddl/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/ddl/tableengine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/dialect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/inspector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:00:08.734327 clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/sql/ddlcompiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/sql/preparer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:00:08.734327 clickhouse-connect-0.6.1/clickhouse_connect/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/datatypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14785 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/datatypes/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/datatypes/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/datatypes/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/datatypes/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11140 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/datatypes/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/datatypes/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/datatypes/special.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6185 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/datatypes/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8548 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/datatypes/temporal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:00:08.734327 clickhouse-connect-0.6.1/clickhouse_connect/dbapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/dbapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/dbapi/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/dbapi/cursor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:00:08.738327 clickhouse-connect-0.6.1/clickhouse_connect/driver/
+-rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38874 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/ctypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/dataconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/ddl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/external.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21102 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/httpclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/httputil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8426 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/insert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/npconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/npquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20182 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driver/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:00:08.738327 clickhouse-connect-0.6.1/clickhouse_connect/driverc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/driverc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/json_impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:00:08.738327 clickhouse-connect-0.6.1/clickhouse_connect/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/tools/datagen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect/tools/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 14:00:08.730327 clickhouse-connect-0.6.1/clickhouse_connect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/clickhouse_connect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 14:00:08.738327 clickhouse-connect-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-06-06 14:00:08.000000 clickhouse-connect-0.6.1/setup.py
```

### Comparing `clickhouse-connect-0.6.0/LICENSE` & `clickhouse-connect-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/PKG-INFO` & `clickhouse-connect-0.6.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: clickhouse-connect
-Version: 0.6.0
-Summary: ClickHouse Database Core Driver
+Version: 0.6.1
+Summary: ClickHouse Database Core Driver for Python, Pandas, and Superset
 Home-page: https://github.com/ClickHouse/clickhouse-connect
 Author: ClickHouse Inc.
 Author-email: clients@clickhouse.com
 License: Apache License 2.0
 Keywords: clickhouse,superset,sqlalchemy,http,driver
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -23,42 +23,42 @@
 Provides-Extra: orjson
 Provides-Extra: pandas
 Provides-Extra: sqlalchemy
 License-File: LICENSE
 
 ## ClickHouse Connect
 
-A high performance core database driver for connecting ClickHouse to Python
+A high performance core database driver for connecting ClickHouse to Python, Pandas, and Superset
 * Pandas DataFrames
 * Numpy Arrays
 * PyArrow Tables
+* Superset Connector
 * SQLAlchemy 1.3 and 1.4 (limited feature set)
 
 ClickHouse Connect currently uses the ClickHouse HTTP interface for maximum compatibility.  
 
 
 ### Installation
 
 ```
 pip install clickhouse-connect
 ```
 
 ClickHouse Connect requires Python 3.7 or higher. 
 
 
-### Warning -- ZStd errors with versions 0.5.21 and below
-Versions prior to 0.5.22 are not compatible with urllib3 version 2+ when using zstd compression.  If you encounter
-such errors please upgrade to clickhouse-connect 0.5.22+ or downgrade your urllib3 version to 1.x
-
-
-### Superset Compatibility
-Starting with v0.6.0, clickhouse-connect no longer includes a Superset EngineSpec.  Instead, the relevant EngineSpec
-has been moved to the core Apache Superset project as of Superset v2.1.0.  If you have issues connecting to earlier
+### Superset Connectivity
+ClickHouse Connect is fully integrated with Apache Superset.  Previous versions of ClickHouse Connect utilized a
+dynamically loaded Superset Engine Spec, but as of Superset v2.1.0 the engine spec was incorporated into the main
+Apache Superset project and removed from clickhouse-connect in v0.6.0.  If you have issues connecting to earlier
 versions of Superset, please use clickhouse-connect v0.5.25.
 
+When creating a Superset Data Source, either use the provided connection dialog, or a SqlAlchemy DSN in the form
+`clickhousedb://{username}:{password}@{host}:{port}`.
+
 
 ### SQLAlchemy Implementation
 ClickHouse Connect incorporates a minimal SQLAlchemy implementation (without any ORM features) for compatibility with
 Superset.  It has only been tested against SQLAlchemy versions 1.3.x and 1.4.x, and is unlikely to work with more
 complex SQLAlchemy applications.
```

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/cc_sqlalchemy/datatypes/base.py` & `clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/datatypes/base.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/cc_sqlalchemy/datatypes/sqltypes.py` & `clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/datatypes/sqltypes.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/cc_sqlalchemy/ddl/custom.py` & `clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/ddl/custom.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/cc_sqlalchemy/ddl/tableengine.py` & `clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/ddl/tableengine.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/cc_sqlalchemy/dialect.py` & `clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/cc_sqlalchemy/inspector.py` & `clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/inspector.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/cc_sqlalchemy/sql/ddlcompiler.py` & `clickhouse-connect-0.6.1/clickhouse_connect/cc_sqlalchemy/sql/ddlcompiler.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/common.py` & `clickhouse-connect-0.6.1/clickhouse_connect/common.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/datatypes/base.py` & `clickhouse-connect-0.6.1/clickhouse_connect/datatypes/base.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/datatypes/container.py` & `clickhouse-connect-0.6.1/clickhouse_connect/datatypes/container.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/datatypes/format.py` & `clickhouse-connect-0.6.1/clickhouse_connect/datatypes/format.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/datatypes/network.py` & `clickhouse-connect-0.6.1/clickhouse_connect/datatypes/network.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/datatypes/numeric.py` & `clickhouse-connect-0.6.1/clickhouse_connect/datatypes/numeric.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/datatypes/registry.py` & `clickhouse-connect-0.6.1/clickhouse_connect/datatypes/registry.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/datatypes/special.py` & `clickhouse-connect-0.6.1/clickhouse_connect/datatypes/special.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/datatypes/string.py` & `clickhouse-connect-0.6.1/clickhouse_connect/datatypes/string.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/datatypes/temporal.py` & `clickhouse-connect-0.6.1/clickhouse_connect/datatypes/temporal.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/dbapi/__init__.py` & `clickhouse-connect-0.6.1/clickhouse_connect/dbapi/__init__.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/dbapi/connection.py` & `clickhouse-connect-0.6.1/clickhouse_connect/dbapi/connection.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/dbapi/cursor.py` & `clickhouse-connect-0.6.1/clickhouse_connect/dbapi/cursor.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/driver/__init__.py` & `clickhouse-connect-0.6.1/clickhouse_connect/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/driver/buffer.py` & `clickhouse-connect-0.6.1/clickhouse_connect/driver/buffer.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/driver/client.py` & `clickhouse-connect-0.6.1/clickhouse_connect/driver/client.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/driver/common.py` & `clickhouse-connect-0.6.1/clickhouse_connect/driver/common.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/driver/compression.py` & `clickhouse-connect-0.6.1/clickhouse_connect/driver/compression.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/driver/context.py` & `clickhouse-connect-0.6.1/clickhouse_connect/driver/context.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/driver/ctypes.py` & `clickhouse-connect-0.6.1/clickhouse_connect/driver/ctypes.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/driver/dataconv.py` & `clickhouse-connect-0.6.1/clickhouse_connect/driver/dataconv.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/driver/ddl.py` & `clickhouse-connect-0.6.1/clickhouse_connect/driver/ddl.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/driver/exceptions.py` & `clickhouse-connect-0.6.1/clickhouse_connect/driver/exceptions.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/driver/external.py` & `clickhouse-connect-0.6.1/clickhouse_connect/driver/external.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/driver/httpclient.py` & `clickhouse-connect-0.6.1/clickhouse_connect/driver/httpclient.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/driver/httputil.py` & `clickhouse-connect-0.6.1/clickhouse_connect/driver/httputil.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/driver/insert.py` & `clickhouse-connect-0.6.1/clickhouse_connect/driver/insert.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/driver/models.py` & `clickhouse-connect-0.6.1/clickhouse_connect/driver/models.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/driver/npquery.py` & `clickhouse-connect-0.6.1/clickhouse_connect/driver/npquery.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/driver/options.py` & `clickhouse-connect-0.6.1/clickhouse_connect/driver/options.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/driver/parser.py` & `clickhouse-connect-0.6.1/clickhouse_connect/driver/parser.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/driver/query.py` & `clickhouse-connect-0.6.1/clickhouse_connect/driver/query.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/driver/tools.py` & `clickhouse-connect-0.6.1/clickhouse_connect/driver/tools.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/driver/transform.py` & `clickhouse-connect-0.6.1/clickhouse_connect/driver/transform.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/driver/types.py` & `clickhouse-connect-0.6.1/clickhouse_connect/driver/types.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/entry_points.py` & `clickhouse-connect-0.6.1/clickhouse_connect/entry_points.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/json_impl.py` & `clickhouse-connect-0.6.1/clickhouse_connect/json_impl.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/tools/datagen.py` & `clickhouse-connect-0.6.1/clickhouse_connect/tools/datagen.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect/tools/testing.py` & `clickhouse-connect-0.6.1/clickhouse_connect/tools/testing.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect.egg-info/PKG-INFO` & `clickhouse-connect-0.6.1/clickhouse_connect.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: clickhouse-connect
-Version: 0.6.0
-Summary: ClickHouse Database Core Driver
+Version: 0.6.1
+Summary: ClickHouse Database Core Driver for Python, Pandas, and Superset
 Home-page: https://github.com/ClickHouse/clickhouse-connect
 Author: ClickHouse Inc.
 Author-email: clients@clickhouse.com
 License: Apache License 2.0
 Keywords: clickhouse,superset,sqlalchemy,http,driver
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
@@ -23,42 +23,42 @@
 Provides-Extra: orjson
 Provides-Extra: pandas
 Provides-Extra: sqlalchemy
 License-File: LICENSE
 
 ## ClickHouse Connect
 
-A high performance core database driver for connecting ClickHouse to Python
+A high performance core database driver for connecting ClickHouse to Python, Pandas, and Superset
 * Pandas DataFrames
 * Numpy Arrays
 * PyArrow Tables
+* Superset Connector
 * SQLAlchemy 1.3 and 1.4 (limited feature set)
 
 ClickHouse Connect currently uses the ClickHouse HTTP interface for maximum compatibility.  
 
 
 ### Installation
 
 ```
 pip install clickhouse-connect
 ```
 
 ClickHouse Connect requires Python 3.7 or higher. 
 
 
-### Warning -- ZStd errors with versions 0.5.21 and below
-Versions prior to 0.5.22 are not compatible with urllib3 version 2+ when using zstd compression.  If you encounter
-such errors please upgrade to clickhouse-connect 0.5.22+ or downgrade your urllib3 version to 1.x
-
-
-### Superset Compatibility
-Starting with v0.6.0, clickhouse-connect no longer includes a Superset EngineSpec.  Instead, the relevant EngineSpec
-has been moved to the core Apache Superset project as of Superset v2.1.0.  If you have issues connecting to earlier
+### Superset Connectivity
+ClickHouse Connect is fully integrated with Apache Superset.  Previous versions of ClickHouse Connect utilized a
+dynamically loaded Superset Engine Spec, but as of Superset v2.1.0 the engine spec was incorporated into the main
+Apache Superset project and removed from clickhouse-connect in v0.6.0.  If you have issues connecting to earlier
 versions of Superset, please use clickhouse-connect v0.5.25.
 
+When creating a Superset Data Source, either use the provided connection dialog, or a SqlAlchemy DSN in the form
+`clickhousedb://{username}:{password}@{host}:{port}`.
+
 
 ### SQLAlchemy Implementation
 ClickHouse Connect incorporates a minimal SQLAlchemy implementation (without any ORM features) for compatibility with
 Superset.  It has only been tested against SQLAlchemy versions 1.3.x and 1.4.x, and is unlikely to work with more
 complex SQLAlchemy applications.
```

### Comparing `clickhouse-connect-0.6.0/clickhouse_connect.egg-info/SOURCES.txt` & `clickhouse-connect-0.6.1/clickhouse_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.0/setup.py` & `clickhouse-connect-0.6.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         version = version_file.readline()
 
     setup(
         name='clickhouse-connect',
         author='ClickHouse Inc.',
         author_email='clients@clickhouse.com',
         keywords=['clickhouse', 'superset', 'sqlalchemy', 'http', 'driver'],
-        description='ClickHouse Database Core Driver',
+        description='ClickHouse Database Core Driver for Python, Pandas, and Superset',
         version=version,
         long_description=long_desc,
         long_description_content_type='text/markdown',
         package_data={'clickhouse_connect': ['VERSION']},
         url='https://github.com/ClickHouse/clickhouse-connect',
         packages=find_packages(exclude=['tests*']),
         python_requires='~=3.7',
```

