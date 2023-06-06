# Comparing `tmp/qpd-0.4.1.tar.gz` & `tmp/qpd-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qpd-0.4.1.tar", last modified: Sun Apr 16 21:36:59 2023, max compression
+gzip compressed data, was "qpd-0.4.2.tar", last modified: Tue Jun  6 07:23:44 2023, max compression
```

## Comparing `qpd-0.4.1.tar` & `qpd-0.4.2.tar`

### file list

```diff
@@ -1,81 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:36:59.349794 qpd-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-16 21:36:16.000000 qpd-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-04-16 21:36:59.349794 qpd-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-04-16 21:36:16.000000 qpd-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:36:59.341794 qpd-0.4.1/_qpd_antlr/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-16 21:36:16.000000 qpd-0.4.1/_qpd_antlr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    98636 2023-04-16 21:36:16.000000 qpd-0.4.1/_qpd_antlr/sqlLexer.py
--rw-r--r--   0 runner    (1001) docker     (123)   785012 2023-04-16 21:36:16.000000 qpd-0.4.1/_qpd_antlr/sqlParser.py
--rw-r--r--   0 runner    (1001) docker     (123)    46840 2023-04-16 21:36:16.000000 qpd-0.4.1/_qpd_antlr/sqlVisitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:36:59.341794 qpd-0.4.1/qpd/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-16 21:36:16.000000 qpd-0.4.1/qpd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:36:59.341794 qpd-0.4.1/qpd/_parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 21:36:16.000000 qpd-0.4.1/qpd/_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-04-16 21:36:16.000000 qpd-0.4.1/qpd/_parser/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-16 21:36:16.000000 qpd-0.4.1/qpd/_parser/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    38946 2023-04-16 21:36:16.000000 qpd-0.4.1/qpd/_parser/visitors.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-16 21:36:16.000000 qpd-0.4.1/qpd/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-04-16 21:36:16.000000 qpd-0.4.1/qpd/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-04-16 21:36:16.000000 qpd-0.4.1/qpd/pandas_like.py
--rw-r--r--   0 runner    (1001) docker     (123)     9429 2023-04-16 21:36:16.000000 qpd-0.4.1/qpd/qpd_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-16 21:36:16.000000 qpd-0.4.1/qpd/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-04-16 21:36:16.000000 qpd-0.4.1/qpd/specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9826 2023-04-16 21:36:16.000000 qpd-0.4.1/qpd/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:36:59.341794 qpd-0.4.1/qpd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-04-16 21:36:59.000000 qpd-0.4.1/qpd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-16 21:36:59.000000 qpd-0.4.1/qpd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 21:36:59.000000 qpd-0.4.1/qpd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-16 21:36:59.000000 qpd-0.4.1/qpd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-16 21:36:59.000000 qpd-0.4.1/qpd.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:36:59.345794 qpd-0.4.1/qpd_dask/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-16 21:36:16.000000 qpd-0.4.1/qpd_dask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26426 2023-04-16 21:36:16.000000 qpd-0.4.1/qpd_dask/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:36:59.345794 qpd-0.4.1/qpd_pandas/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-16 21:36:16.000000 qpd-0.4.1/qpd_pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22191 2023-04-16 21:36:16.000000 qpd-0.4.1/qpd_pandas/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:36:59.345794 qpd-0.4.1/qpd_ray/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-16 21:36:16.000000 qpd-0.4.1/qpd_ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25388 2023-04-16 21:36:16.000000 qpd-0.4.1/qpd_ray/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:36:59.345794 qpd-0.4.1/qpd_test/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-16 21:36:16.000000 qpd-0.4.1/qpd_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-04-16 21:36:16.000000 qpd-0.4.1/qpd_test/benchmark_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)    51754 2023-04-16 21:36:16.000000 qpd-0.4.1/qpd_test/engine_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)    35955 2023-04-16 21:36:16.000000 qpd-0.4.1/qpd_test/sql_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-04-16 21:36:16.000000 qpd-0.4.1/qpd_test/tests_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-04-16 21:36:16.000000 qpd-0.4.1/qpd_test/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:36:59.345794 qpd-0.4.1/qpd_version/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-16 21:36:16.000000 qpd-0.4.1/qpd_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-04-16 21:36:59.349794 qpd-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-16 21:36:16.000000 qpd-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:36:59.345794 qpd-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 21:36:16.000000 qpd-0.4.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:36:59.345794 qpd-0.4.1/tests/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 21:36:16.000000 qpd-0.4.1/tests/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-16 21:36:16.000000 qpd-0.4.1/tests/benchmark/test_pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:36:59.345794 qpd-0.4.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 21:36:16.000000 qpd-0.4.1/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:36:59.345794 qpd-0.4.1/tests/unit/qpd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 21:36:16.000000 qpd-0.4.1/tests/unit/qpd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:36:59.345794 qpd-0.4.1/tests/unit/qpd/_parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 21:36:16.000000 qpd-0.4.1/tests/unit/qpd/_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-04-16 21:36:16.000000 qpd-0.4.1/tests/unit/qpd/_parser/test_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-04-16 21:36:16.000000 qpd-0.4.1/tests/unit/qpd/_parser/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    28065 2023-04-16 21:36:16.000000 qpd-0.4.1/tests/unit/qpd/_parser/test_visitors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-04-16 21:36:16.000000 qpd-0.4.1/tests/unit/qpd/test_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-04-16 21:36:16.000000 qpd-0.4.1/tests/unit/qpd/test_specs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-16 21:36:16.000000 qpd-0.4.1/tests/unit/qpd/test_workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:36:59.349794 qpd-0.4.1/tests/unit/qpd_dask/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 21:36:16.000000 qpd-0.4.1/tests/unit/qpd_dask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-16 21:36:16.000000 qpd-0.4.1/tests/unit/qpd_dask/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-04-16 21:36:16.000000 qpd-0.4.1/tests/unit/qpd_dask/test_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:36:59.349794 qpd-0.4.1/tests/unit/qpd_pandas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 21:36:16.000000 qpd-0.4.1/tests/unit/qpd_pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-16 21:36:16.000000 qpd-0.4.1/tests/unit/qpd_pandas/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-04-16 21:36:16.000000 qpd-0.4.1/tests/unit/qpd_pandas/test_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:36:59.349794 qpd-0.4.1/tests/unit/qpd_ray/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 21:36:16.000000 qpd-0.4.1/tests/unit/qpd_ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-04-16 21:36:16.000000 qpd-0.4.1/tests/unit/qpd_ray/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-04-16 21:36:16.000000 qpd-0.4.1/tests/unit/qpd_ray/test_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 21:36:59.349794 qpd-0.4.1/tests/unit/qpd_test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 21:36:16.000000 qpd-0.4.1/tests/unit/qpd_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-16 21:36:16.000000 qpd-0.4.1/tests/unit/qpd_test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:23:44.431127 qpd-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-06 07:22:49.000000 qpd-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-06-06 07:23:44.431127 qpd-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-06-06 07:22:49.000000 qpd-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:23:44.427127 qpd-0.4.2/qpd/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-06 07:22:49.000000 qpd-0.4.2/qpd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:23:44.431127 qpd-0.4.2/qpd/_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 07:22:49.000000 qpd-0.4.2/qpd/_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-06-06 07:22:49.000000 qpd-0.4.2/qpd/_parser/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-06 07:22:49.000000 qpd-0.4.2/qpd/_parser/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38946 2023-06-06 07:22:49.000000 qpd-0.4.2/qpd/_parser/visitors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-06 07:22:49.000000 qpd-0.4.2/qpd/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-06-06 07:22:49.000000 qpd-0.4.2/qpd/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9438 2023-06-06 07:22:49.000000 qpd-0.4.2/qpd/qpd_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-06 07:22:49.000000 qpd-0.4.2/qpd/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-06-06 07:22:49.000000 qpd-0.4.2/qpd/specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9826 2023-06-06 07:22:49.000000 qpd-0.4.2/qpd/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:23:44.427127 qpd-0.4.2/qpd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-06-06 07:23:44.000000 qpd-0.4.2/qpd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-06 07:23:44.000000 qpd-0.4.2/qpd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 07:23:44.000000 qpd-0.4.2/qpd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-06 07:23:44.000000 qpd-0.4.2/qpd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-06 07:23:44.000000 qpd-0.4.2/qpd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:23:44.431127 qpd-0.4.2/qpd_dask/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-06 07:22:49.000000 qpd-0.4.2/qpd_dask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26462 2023-06-06 07:22:49.000000 qpd-0.4.2/qpd_dask/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:23:44.431127 qpd-0.4.2/qpd_pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-06 07:22:49.000000 qpd-0.4.2/qpd_pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22062 2023-06-06 07:22:49.000000 qpd-0.4.2/qpd_pandas/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:23:44.431127 qpd-0.4.2/qpd_ray/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-06 07:22:49.000000 qpd-0.4.2/qpd_ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25424 2023-06-06 07:22:49.000000 qpd-0.4.2/qpd_ray/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:23:44.431127 qpd-0.4.2/qpd_test/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-06 07:22:49.000000 qpd-0.4.2/qpd_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-06-06 07:22:49.000000 qpd-0.4.2/qpd_test/benchmark_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51754 2023-06-06 07:22:49.000000 qpd-0.4.2/qpd_test/engine_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35955 2023-06-06 07:22:49.000000 qpd-0.4.2/qpd_test/sql_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-06-06 07:22:49.000000 qpd-0.4.2/qpd_test/tests_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-06 07:22:49.000000 qpd-0.4.2/qpd_test/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 07:23:44.431127 qpd-0.4.2/qpd_version/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-06 07:22:49.000000 qpd-0.4.2/qpd_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-06 07:23:44.431127 qpd-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-06 07:22:49.000000 qpd-0.4.2/setup.py
```

### Comparing `qpd-0.4.1/LICENSE` & `qpd-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qpd-0.4.1/PKG-INFO` & `qpd-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qpd
-Version: 0.4.1
+Version: 0.4.2
 Summary: Query Pandas Using SQL
 Home-page: http://github.com/goodwanghan/qpd
 Author: Han Wang
 Author-email: goodwanghan@gmail.com
 License: Apache-2.0
 Description: # Query Pandas-like Dataframes Using SQL
         
@@ -119,26 +119,27 @@
         be guaranteed, but there will be no performance advantage. So for Spark, please use Spark SQL.
         If you use Fugue SQL on Spark backend, it will also directly use Spark to run the SQL statements.
         We don't see the value to make QPD run on Spark.
         
         
         ## Update History
         
+        * 0.4.2: Refactor to use the latest triad, fix packaging issues
         * 0.4.1: Make Pandas 2 compatible
         * 0.4.0: Support arbitrary column name
         * 0.2.6: Update pandas indexer import
         * 0.2.5: Update antlr to 4.9
         * 0.2.4: Fix a bug: set operations will alter the input dataframe to add columns
         * 0.2.3: Refactor and extract out PandasLikeUtils class
         * 0.2.2: Accept constant select without `FROM`, `SELECT 1 AS a, 'b' AS b`
         * <= 0.2.1: Pandas, Dask, Ray SQL support
         
 Keywords: pandas sql
 Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `qpd-0.4.1/README.md` & `qpd-0.4.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -111,14 +111,15 @@
 be guaranteed, but there will be no performance advantage. So for Spark, please use Spark SQL.
 If you use Fugue SQL on Spark backend, it will also directly use Spark to run the SQL statements.
 We don't see the value to make QPD run on Spark.
 
 
 ## Update History
 
+* 0.4.2: Refactor to use the latest triad, fix packaging issues
 * 0.4.1: Make Pandas 2 compatible
 * 0.4.0: Support arbitrary column name
 * 0.2.6: Update pandas indexer import
 * 0.2.5: Update antlr to 4.9
 * 0.2.4: Fix a bug: set operations will alter the input dataframe to add columns
 * 0.2.3: Refactor and extract out PandasLikeUtils class
 * 0.2.2: Accept constant select without `FROM`, `SELECT 1 AS a, 'b' AS b`
```

### Comparing `qpd-0.4.1/qpd/_parser/sql.py` & `qpd-0.4.2/qpd/_parser/sql.py`

 * *Files identical despite different names*

### Comparing `qpd-0.4.1/qpd/_parser/utils.py` & `qpd-0.4.2/qpd/_parser/utils.py`

 * *Files identical despite different names*

### Comparing `qpd-0.4.1/qpd/_parser/visitors.py` & `qpd-0.4.2/qpd/_parser/visitors.py`

 * *Files identical despite different names*

### Comparing `qpd-0.4.1/qpd/constants.py` & `qpd-0.4.2/qpd/constants.py`

 * *Files identical despite different names*

### Comparing `qpd-0.4.1/qpd/dataframe.py` & `qpd-0.4.2/qpd/dataframe.py`

 * *Files identical despite different names*

### Comparing `qpd-0.4.1/qpd/qpd_engine.py` & `qpd-0.4.2/qpd/qpd_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from abc import ABC, abstractmethod
 from builtins import bool
 from typing import Any, Dict, List, Tuple
 
+from triad.utils.assertion import assert_or_throw
+from triad.utils.pandas_like import PandasLikeUtils
+
 from qpd.dataframe import Column, DataFrame
 from qpd.specs import (
     AggFunctionSpec,
     ArgumentSpec,
     IsValueSpec,
     OrderBySpec,
     WindowFunctionSpec,
 )
-from triad.utils.assertion import assert_or_throw
-from qpd.pandas_like import PandasLikeUtils
 
 
 class QPDEngine(ABC):
     def __call__(self, func_name: str, *args: Any, **kwargs: Any) -> Any:
         return getattr(self, func_name)(*args, **kwargs)
 
     def rename(self, col: Column, name: str) -> Column:
```

### Comparing `qpd-0.4.1/qpd/run.py` & `qpd-0.4.2/qpd/run.py`

 * *Files identical despite different names*

### Comparing `qpd-0.4.1/qpd/specs.py` & `qpd-0.4.2/qpd/specs.py`

 * *Files identical despite different names*

### Comparing `qpd-0.4.1/qpd/workflow.py` & `qpd-0.4.2/qpd/workflow.py`

 * *Files identical despite different names*

### Comparing `qpd-0.4.1/qpd.egg-info/PKG-INFO` & `qpd-0.4.2/qpd.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qpd
-Version: 0.4.1
+Version: 0.4.2
 Summary: Query Pandas Using SQL
 Home-page: http://github.com/goodwanghan/qpd
 Author: Han Wang
 Author-email: goodwanghan@gmail.com
 License: Apache-2.0
 Description: # Query Pandas-like Dataframes Using SQL
         
@@ -119,26 +119,27 @@
         be guaranteed, but there will be no performance advantage. So for Spark, please use Spark SQL.
         If you use Fugue SQL on Spark backend, it will also directly use Spark to run the SQL statements.
         We don't see the value to make QPD run on Spark.
         
         
         ## Update History
         
+        * 0.4.2: Refactor to use the latest triad, fix packaging issues
         * 0.4.1: Make Pandas 2 compatible
         * 0.4.0: Support arbitrary column name
         * 0.2.6: Update pandas indexer import
         * 0.2.5: Update antlr to 4.9
         * 0.2.4: Fix a bug: set operations will alter the input dataframe to add columns
         * 0.2.3: Refactor and extract out PandasLikeUtils class
         * 0.2.2: Accept constant select without `FROM`, `SELECT 1 AS a, 'b' AS b`
         * <= 0.2.1: Pandas, Dask, Ray SQL support
         
 Keywords: pandas sql
 Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `qpd-0.4.1/qpd_dask/engine.py` & `qpd-0.4.2/qpd_dask/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from typing import Any, Callable, Dict, List, Tuple
 
 import dask.array as np
 import dask.dataframe as pd
 import numpy
 import pandas
-from qpd import PandasLikeUtils, QPDEngine, run_sql
+from triad.utils.assertion import assert_or_throw
+from triad.utils.pandas_like import PandasLikeUtils
+
+from qpd import QPDEngine, run_sql
 from qpd.dataframe import Column, DataFrame
 from qpd.specs import (
     AggFunctionSpec,
     ArgumentSpec,
     OrderBySpec,
     RollingWindowFrame,
     WindowFunctionSpec,
 )
 from qpd_pandas.engine import _RowsIndexer
-from triad.utils.assertion import assert_or_throw
 
 
 def run_sql_on_dask(
     sql: str, dfs: Dict[str, Any], ignore_case: bool = False
 ) -> pd.DataFrame:
     return run_sql(QPDDaskEngine(), sql, dfs, ignore_case=ignore_case)
```

### Comparing `qpd-0.4.1/qpd_pandas/engine.py` & `qpd-0.4.2/qpd_pandas/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 from typing import Any, Callable, Dict, List, Optional, Tuple
 
 import numpy as np
 import pandas as pd
 from pandas.api.indexers import BaseIndexer
-from qpd import PandasLikeUtils, QPDEngine, run_sql
+from triad.utils.assertion import assert_or_throw
+from triad.utils.pandas_like import PandasUtils
+
+from qpd import QPDEngine, run_sql
 from qpd.dataframe import Column, DataFrame
 from qpd.specs import (
     AggFunctionSpec,
     ArgumentSpec,
     OrderBySpec,
     RollingWindowFrame,
     WindowFunctionSpec,
 )
-from triad.utils.assertion import assert_or_throw
 
 
 def run_sql_on_pandas(
     sql: str, dfs: Dict[str, Any], ignore_case: bool = False
 ) -> pd.DataFrame:
     return run_sql(QPDPandasEngine(), sql, dfs, ignore_case=ignore_case)
 
 
-class PandasUtils(PandasLikeUtils[pd.DataFrame, pd.Series]):
-    def concat_dfs(self, *dfs: pd.DataFrame) -> pd.DataFrame:
-        return pd.concat(list(dfs))
-
-
 class QPDPandasEngine(QPDEngine):
     @property
     def pl_utils(self) -> PandasUtils:
         return PandasUtils()
 
     def to_df(self, obj: Any) -> DataFrame:
         if isinstance(obj, DataFrame):
```

### Comparing `qpd-0.4.1/qpd_ray/engine.py` & `qpd-0.4.2/qpd_ray/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from typing import Any, Callable, Dict, List, Tuple, Union
 
 import modin.pandas as pd
 import numpy
 import pandas
-from qpd import PandasLikeUtils, QPDEngine, run_sql
+from triad.utils.assertion import assert_or_throw
+from triad.utils.pandas_like import PandasLikeUtils
+
+from qpd import QPDEngine, run_sql
 from qpd.dataframe import Column, DataFrame
 from qpd.specs import (
     AggFunctionSpec,
     ArgumentSpec,
     OrderBySpec,
     RollingWindowFrame,
     WindowFunctionSpec,
 )
 from qpd_pandas.engine import _RowsIndexer
-from triad.utils.assertion import assert_or_throw
 
 
 def run_sql_on_ray(
     sql: str, dfs: Dict[str, Any], ignore_case: bool = False
 ) -> pd.DataFrame:
     return run_sql(QPDRayEngine(), sql, dfs, ignore_case=ignore_case)
```

### Comparing `qpd-0.4.1/qpd_test/benchmark_suite.py` & `qpd-0.4.2/qpd_test/benchmark_suite.py`

 * *Files identical despite different names*

### Comparing `qpd-0.4.1/qpd_test/engine_suite.py` & `qpd-0.4.2/qpd_test/engine_suite.py`

 * *Files identical despite different names*

### Comparing `qpd-0.4.1/qpd_test/sql_suite.py` & `qpd-0.4.2/qpd_test/sql_suite.py`

 * *Files identical despite different names*

### Comparing `qpd-0.4.1/qpd_test/tests_base.py` & `qpd-0.4.2/qpd_test/tests_base.py`

 * *Files identical despite different names*

### Comparing `qpd-0.4.1/qpd_test/utils.py` & `qpd-0.4.2/qpd_test/utils.py`

 * *Files identical despite different names*

### Comparing `qpd-0.4.1/setup.py` & `qpd-0.4.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,41 +14,41 @@
 
 with open("README.md") as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name="qpd",
     version=get_version(),
-    packages=find_packages(),
+    packages=find_packages(include=["qpd*"]),
     description="Query Pandas Using SQL",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     license="Apache-2.0",
     author="Han Wang",
     author_email="goodwanghan@gmail.com",
     keywords="pandas sql",
     url="http://github.com/goodwanghan/qpd",
     install_requires=[
         "pandas>=1.2.0",
-        "triad>=0.8.0",
+        "triad>=0.9.0",
         "adagio",
         "antlr4-python3-runtime>=4.11.1,<4.12",
     ],
     extras_require={
         "dask": ["dask[dataframe,distributed]", "cloudpickle>=1.4.0"],
         # "ray": ["pandas>=1.1.2", "modin[ray]>=0.8.1.1"],
         "all": [
             "dask[dataframe,distributed]",
             "cloudpickle>=1.4.0",
             # "modin[ray]",
         ],
     },
     classifiers=[
         # "3 - Alpha", "4 - Beta" or "5 - Production/Stable"
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
```

