# Comparing `tmp/dbt-teradata-1.3.0.0.tar.gz` & `tmp/dbt-teradata-1.3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-teradata-1.3.0.0.tar", last modified: Fri Apr  7 11:39:49 2023, max compression
+gzip compressed data, was "dbt-teradata-1.3.3.0.tar", last modified: Tue Apr 18 07:37:56 2023, max compression
```

## Comparing `dbt-teradata-1.3.0.0.tar` & `dbt-teradata-1.3.3.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:39:49.812340 dbt-teradata-1.3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-07 11:39:24.000000 dbt-teradata-1.3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21235 2023-04-07 11:39:49.812340 dbt-teradata-1.3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20969 2023-04-07 11:39:24.000000 dbt-teradata-1.3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:39:49.808340 dbt-teradata-1.3.0.0/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:39:49.808340 dbt-teradata-1.3.0.0/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:39:49.808340 dbt-teradata-1.3.0.0/dbt/adapters/teradata/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-07 11:39:24.000000 dbt-teradata-1.3.0.0/dbt/adapters/teradata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-07 11:39:48.000000 dbt-teradata-1.3.0.0/dbt/adapters/teradata/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-07 11:39:24.000000 dbt-teradata-1.3.0.0/dbt/adapters/teradata/column.py
--rw-r--r--   0 runner    (1001) docker     (123)     9499 2023-04-07 11:39:24.000000 dbt-teradata-1.3.0.0/dbt/adapters/teradata/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-04-07 11:39:24.000000 dbt-teradata-1.3.0.0/dbt/adapters/teradata/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-07 11:39:24.000000 dbt-teradata-1.3.0.0/dbt/adapters/teradata/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:39:49.808340 dbt-teradata-1.3.0.0/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:39:49.808340 dbt-teradata-1.3.0.0/dbt/include/teradata/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-07 11:39:24.000000 dbt-teradata-1.3.0.0/dbt/include/teradata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-07 11:39:24.000000 dbt-teradata-1.3.0.0/dbt/include/teradata/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:39:49.808340 dbt-teradata-1.3.0.0/dbt/include/teradata/macros/
--rw-r--r--   0 runner    (1001) docker     (123)     9880 2023-04-07 11:39:24.000000 dbt-teradata-1.3.0.0/dbt/include/teradata/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-07 11:39:24.000000 dbt-teradata-1.3.0.0/dbt/include/teradata/macros/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-04-07 11:39:24.000000 dbt-teradata-1.3.0.0/dbt/include/teradata/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:39:49.808340 dbt-teradata-1.3.0.0/dbt/include/teradata/macros/materializations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:39:49.812340 dbt-teradata-1.3.0.0/dbt/include/teradata/macros/materializations/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-07 11:39:24.000000 dbt-teradata-1.3.0.0/dbt/include/teradata/macros/materializations/incremental/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-04-07 11:39:24.000000 dbt-teradata-1.3.0.0/dbt/include/teradata/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-07 11:39:24.000000 dbt-teradata-1.3.0.0/dbt/include/teradata/macros/materializations/incremental/strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:39:49.812340 dbt-teradata-1.3.0.0/dbt/include/teradata/macros/materializations/seed/
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-04-07 11:39:24.000000 dbt-teradata-1.3.0.0/dbt/include/teradata/macros/materializations/seed/seed.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:39:49.812340 dbt-teradata-1.3.0.0/dbt/include/teradata/macros/materializations/snapshot/
--rw-r--r--   0 runner    (1001) docker     (123)    10294 2023-04-07 11:39:24.000000 dbt-teradata-1.3.0.0/dbt/include/teradata/macros/materializations/snapshot/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-07 11:39:24.000000 dbt-teradata-1.3.0.0/dbt/include/teradata/macros/materializations/snapshot/snapshot_merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-07 11:39:24.000000 dbt-teradata-1.3.0.0/dbt/include/teradata/macros/materializations/snapshot/strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:39:49.812340 dbt-teradata-1.3.0.0/dbt/include/teradata/macros/materializations/test/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-07 11:39:24.000000 dbt-teradata-1.3.0.0/dbt/include/teradata/macros/materializations/test/test.sql
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-07 11:39:24.000000 dbt-teradata-1.3.0.0/dbt/include/teradata/sample_profiles.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:39:49.812340 dbt-teradata-1.3.0.0/dbt_teradata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21235 2023-04-07 11:39:49.000000 dbt-teradata-1.3.0.0/dbt_teradata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-07 11:39:49.000000 dbt-teradata-1.3.0.0/dbt_teradata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 11:39:49.000000 dbt-teradata-1.3.0.0/dbt_teradata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-07 11:39:49.000000 dbt-teradata-1.3.0.0/dbt_teradata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-07 11:39:49.000000 dbt-teradata-1.3.0.0/dbt_teradata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-07 11:39:49.812340 dbt-teradata-1.3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-04-07 11:39:48.000000 dbt-teradata-1.3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:37:56.970270 dbt-teradata-1.3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-18 07:37:19.000000 dbt-teradata-1.3.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21235 2023-04-18 07:37:56.970270 dbt-teradata-1.3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20969 2023-04-18 07:37:19.000000 dbt-teradata-1.3.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:37:56.970270 dbt-teradata-1.3.3.0/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:37:56.970270 dbt-teradata-1.3.3.0/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:37:56.970270 dbt-teradata-1.3.3.0/dbt/adapters/teradata/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-18 07:37:19.000000 dbt-teradata-1.3.3.0/dbt/adapters/teradata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-18 07:37:54.000000 dbt-teradata-1.3.3.0/dbt/adapters/teradata/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-18 07:37:19.000000 dbt-teradata-1.3.3.0/dbt/adapters/teradata/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9499 2023-04-18 07:37:19.000000 dbt-teradata-1.3.3.0/dbt/adapters/teradata/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-04-18 07:37:19.000000 dbt-teradata-1.3.3.0/dbt/adapters/teradata/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-18 07:37:19.000000 dbt-teradata-1.3.3.0/dbt/adapters/teradata/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:37:56.970270 dbt-teradata-1.3.3.0/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:37:56.970270 dbt-teradata-1.3.3.0/dbt/include/teradata/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-18 07:37:19.000000 dbt-teradata-1.3.3.0/dbt/include/teradata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-18 07:37:19.000000 dbt-teradata-1.3.3.0/dbt/include/teradata/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:37:56.970270 dbt-teradata-1.3.3.0/dbt/include/teradata/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)     9880 2023-04-18 07:37:19.000000 dbt-teradata-1.3.3.0/dbt/include/teradata/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-18 07:37:19.000000 dbt-teradata-1.3.3.0/dbt/include/teradata/macros/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-04-18 07:37:19.000000 dbt-teradata-1.3.3.0/dbt/include/teradata/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:37:56.970270 dbt-teradata-1.3.3.0/dbt/include/teradata/macros/materializations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:37:56.970270 dbt-teradata-1.3.3.0/dbt/include/teradata/macros/materializations/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-18 07:37:19.000000 dbt-teradata-1.3.3.0/dbt/include/teradata/macros/materializations/incremental/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-04-18 07:37:19.000000 dbt-teradata-1.3.3.0/dbt/include/teradata/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-18 07:37:19.000000 dbt-teradata-1.3.3.0/dbt/include/teradata/macros/materializations/incremental/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:37:56.970270 dbt-teradata-1.3.3.0/dbt/include/teradata/macros/materializations/seed/
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-04-18 07:37:19.000000 dbt-teradata-1.3.3.0/dbt/include/teradata/macros/materializations/seed/seed.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:37:56.970270 dbt-teradata-1.3.3.0/dbt/include/teradata/macros/materializations/snapshot/
+-rw-r--r--   0 runner    (1001) docker     (123)    10294 2023-04-18 07:37:19.000000 dbt-teradata-1.3.3.0/dbt/include/teradata/macros/materializations/snapshot/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-18 07:37:19.000000 dbt-teradata-1.3.3.0/dbt/include/teradata/macros/materializations/snapshot/snapshot_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-18 07:37:19.000000 dbt-teradata-1.3.3.0/dbt/include/teradata/macros/materializations/snapshot/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:37:56.970270 dbt-teradata-1.3.3.0/dbt/include/teradata/macros/materializations/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-18 07:37:19.000000 dbt-teradata-1.3.3.0/dbt/include/teradata/macros/materializations/test/test.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-18 07:37:19.000000 dbt-teradata-1.3.3.0/dbt/include/teradata/sample_profiles.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:37:56.970270 dbt-teradata-1.3.3.0/dbt_teradata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21235 2023-04-18 07:37:56.000000 dbt-teradata-1.3.3.0/dbt_teradata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-18 07:37:56.000000 dbt-teradata-1.3.3.0/dbt_teradata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 07:37:56.000000 dbt-teradata-1.3.3.0/dbt_teradata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-18 07:37:56.000000 dbt-teradata-1.3.3.0/dbt_teradata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-18 07:37:56.000000 dbt-teradata-1.3.3.0/dbt_teradata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 07:37:56.970270 dbt-teradata-1.3.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-18 07:37:54.000000 dbt-teradata-1.3.3.0/setup.py
```

### Comparing `dbt-teradata-1.3.0.0/LICENSE` & `dbt-teradata-1.3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.3.0.0/PKG-INFO` & `dbt-teradata-1.3.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-teradata
-Version: 1.3.0.0
+Version: 1.3.3.0
 Summary: The Teradata adapter plugin for dbt (data build tool)
 Home-page: https://github.com/Teradata/dbt-teradata
 Author: Teradata Corporation
 Author-email: developers@teradata.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dbt-teradata-1.3.0.0/README.md` & `dbt-teradata-1.3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.3.0.0/dbt/adapters/teradata/__init__.py` & `dbt-teradata-1.3.3.0/dbt/adapters/teradata/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.3.0.0/dbt/adapters/teradata/column.py` & `dbt-teradata-1.3.3.0/dbt/adapters/teradata/column.py`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.3.0.0/dbt/adapters/teradata/connections.py` & `dbt-teradata-1.3.3.0/dbt/adapters/teradata/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.3.0.0/dbt/adapters/teradata/impl.py` & `dbt-teradata-1.3.3.0/dbt/adapters/teradata/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.3.0.0/dbt/adapters/teradata/relation.py` & `dbt-teradata-1.3.3.0/dbt/adapters/teradata/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.3.0.0/dbt/include/teradata/macros/adapters.sql` & `dbt-teradata-1.3.3.0/dbt/include/teradata/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.3.0.0/dbt/include/teradata/macros/apply_grants.sql` & `dbt-teradata-1.3.3.0/dbt/include/teradata/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.3.0.0/dbt/include/teradata/macros/catalog.sql` & `dbt-teradata-1.3.3.0/dbt/include/teradata/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.3.0.0/dbt/include/teradata/macros/materializations/incremental/helpers.sql` & `dbt-teradata-1.3.3.0/dbt/include/teradata/macros/materializations/incremental/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.3.0.0/dbt/include/teradata/macros/materializations/incremental/incremental.sql` & `dbt-teradata-1.3.3.0/dbt/include/teradata/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.3.0.0/dbt/include/teradata/macros/materializations/incremental/strategies.sql` & `dbt-teradata-1.3.3.0/dbt/include/teradata/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.3.0.0/dbt/include/teradata/macros/materializations/seed/seed.sql` & `dbt-teradata-1.3.3.0/dbt/include/teradata/macros/materializations/seed/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.3.0.0/dbt/include/teradata/macros/materializations/snapshot/snapshot.sql` & `dbt-teradata-1.3.3.0/dbt/include/teradata/macros/materializations/snapshot/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.3.0.0/dbt/include/teradata/macros/materializations/snapshot/snapshot_merge.sql` & `dbt-teradata-1.3.3.0/dbt/include/teradata/macros/materializations/snapshot/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.3.0.0/dbt/include/teradata/macros/materializations/test/test.sql` & `dbt-teradata-1.3.3.0/dbt/include/teradata/macros/materializations/test/test.sql`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.3.0.0/dbt_teradata.egg-info/PKG-INFO` & `dbt-teradata-1.3.3.0/dbt_teradata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-teradata
-Version: 1.3.0.0
+Version: 1.3.3.0
 Summary: The Teradata adapter plugin for dbt (data build tool)
 Home-page: https://github.com/Teradata/dbt-teradata
 Author: Teradata Corporation
 Author-email: developers@teradata.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dbt-teradata-1.3.0.0/dbt_teradata.egg-info/SOURCES.txt` & `dbt-teradata-1.3.3.0/dbt_teradata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-teradata-1.3.0.0/setup.py` & `dbt-teradata-1.3.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 if sys.version_info < (3, 7) or sys.version_info >= (3, 11):
     print('Error: dbt-teradata does not support this version of Python.')
     print('Please install Python 3.7 or higher but less than 3.11.')
     sys.exit(1)
 
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
-with open(os.path.join(this_directory, 'README.md')) as f:
+with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 package_name = "dbt-teradata"
-package_version = "1.3.0.0"
+package_version = "1.3.3.0"
 description = """The Teradata adapter plugin for dbt (data build tool)"""
 
 
 setup(
     name=package_name,
     version=package_version,
 
@@ -41,15 +41,15 @@
             'macros/*.sql',
             'macros/materializations/**/*.sql',
             'dbt_project.yml',
             'sample_profiles.yml',
         ],
     },
     install_requires=[
-        "dbt-core==1.3.0",
+        "dbt-core==1.3.3",
         "teradatasql>=16.20.0.0",
     ],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
 
         'License :: OSI Approved :: Apache Software License',
```

