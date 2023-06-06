# Comparing `tmp/dbt-clickzetta-0.2.6.tar.gz` & `tmp/dbt-clickzetta-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-clickzetta-0.2.6.tar", last modified: Mon Jun  5 11:10:23 2023, max compression
+gzip compressed data, was "dbt-clickzetta-0.2.7.tar", last modified: Mon Jun  5 11:38:53 2023, max compression
```

## Comparing `dbt-clickzetta-0.2.6.tar` & `dbt-clickzetta-0.2.7.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 11:10:23.589383 dbt-clickzetta-0.2.6/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       47 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.6/MANIFEST.in
--rw-r--r--   0 lihanmiao   (501) staff       (20)      659 2023-06-05 11:10:23.589248 dbt-clickzetta-0.2.6/PKG-INFO
--rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.6/README.md
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 11:10:23.583792 dbt-clickzetta-0.2.6/dbt/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       76 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.6/dbt/__init__.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 11:10:23.583031 dbt-clickzetta-0.2.6/dbt/adapters/
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 11:10:23.584894 dbt-clickzetta-0.2.6/dbt/adapters/clickzetta/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      611 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.6/dbt/adapters/clickzetta/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)       18 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.6/dbt/adapters/clickzetta/__version__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1425 2023-05-28 10:16:48.000000 dbt-clickzetta-0.2.6/dbt/adapters/clickzetta/column.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7157 2023-06-05 09:21:52.000000 dbt-clickzetta-0.2.6/dbt/adapters/clickzetta/connections.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)     6958 2023-06-05 11:10:19.000000 dbt-clickzetta-0.2.6/dbt/adapters/clickzetta/impl.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)      698 2023-06-05 09:54:42.000000 dbt-clickzetta-0.2.6/dbt/adapters/clickzetta/relation.py
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 11:10:23.583123 dbt-clickzetta-0.2.6/dbt/include/
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 11:10:23.585359 dbt-clickzetta-0.2.6/dbt/include/clickzetta/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       52 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.6/dbt/include/clickzetta/__init__.py
--rw-r--r--   0 lihanmiao   (501) staff       (20)       77 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.6/dbt/include/clickzetta/dbt_project.yml
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 11:10:23.585563 dbt-clickzetta-0.2.6/dbt/include/clickzetta/macros/
--rw-r--r--   0 lihanmiao   (501) staff       (20)    14274 2023-06-05 11:06:31.000000 dbt-clickzetta-0.2.6/dbt/include/clickzetta/macros/adapters.sql
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 11:10:23.586210 dbt-clickzetta-0.2.6/dbt/include/clickzetta/macros/materializations/
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 11:10:23.586785 dbt-clickzetta-0.2.6/dbt/include/clickzetta/macros/materializations/incremental/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      881 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.6/dbt/include/clickzetta/macros/materializations/incremental/column_helpers.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3419 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.6/dbt/include/clickzetta/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     3822 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.6/dbt/include/clickzetta/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2150 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.6/dbt/include/clickzetta/macros/materializations/incremental/validate.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1655 2023-06-05 08:55:29.000000 dbt-clickzetta-0.2.6/dbt/include/clickzetta/macros/materializations/seed.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     7258 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.6/dbt/include/clickzetta/macros/materializations/snapshot.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1728 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.6/dbt/include/clickzetta/macros/materializations/table.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      119 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.6/dbt/include/clickzetta/macros/materializations/view.sql
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 11:10:23.588520 dbt-clickzetta-0.2.6/dbt/include/clickzetta/macros/utils/
--rw-r--r--   0 lihanmiao   (501) staff       (20)       92 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.6/dbt/include/clickzetta/macros/utils/any_value.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      136 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.6/dbt/include/clickzetta/macros/utils/array_append.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      113 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.6/dbt/include/clickzetta/macros/utils/array_concat.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      114 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.6/dbt/include/clickzetta/macros/utils/array_construct.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      326 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.6/dbt/include/clickzetta/macros/utils/assert_not_null.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)       89 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.6/dbt/include/clickzetta/macros/utils/bool_or.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)       92 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.6/dbt/include/clickzetta/macros/utils/concat.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2135 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.6/dbt/include/clickzetta/macros/utils/dateadd.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)     4619 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.6/dbt/include/clickzetta/macros/utils/datediff.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      112 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.6/dbt/include/clickzetta/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      563 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.6/dbt/include/clickzetta/macros/utils/listagg.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      563 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.6/dbt/include/clickzetta/macros/utils/split_part.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)       85 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.6/dbt/include/clickzetta/macros/utils/timestamps.sql
--rw-r--r--   0 lihanmiao   (501) staff       (20)      304 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.6/dbt/include/clickzetta/profile_template.yml
-drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 11:10:23.589073 dbt-clickzetta-0.2.6/dbt_clickzetta.egg-info/
--rw-r--r--   0 lihanmiao   (501) staff       (20)      659 2023-06-05 11:10:23.000000 dbt-clickzetta-0.2.6/dbt_clickzetta.egg-info/PKG-INFO
--rw-r--r--   0 lihanmiao   (501) staff       (20)     1848 2023-06-05 11:10:23.000000 dbt-clickzetta-0.2.6/dbt_clickzetta.egg-info/SOURCES.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-06-05 11:10:23.000000 dbt-clickzetta-0.2.6/dbt_clickzetta.egg-info/dependency_links.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-06-05 11:10:23.000000 dbt-clickzetta-0.2.6/dbt_clickzetta.egg-info/not-zip-safe
--rw-r--r--   0 lihanmiao   (501) staff       (20)       44 2023-06-05 11:10:23.000000 dbt-clickzetta-0.2.6/dbt_clickzetta.egg-info/requires.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)        4 2023-06-05 11:10:23.000000 dbt-clickzetta-0.2.6/dbt_clickzetta.egg-info/top_level.txt
--rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-06-05 11:10:23.589422 dbt-clickzetta-0.2.6/setup.cfg
--rw-r--r--   0 lihanmiao   (501) staff       (20)     2929 2023-06-05 11:10:19.000000 dbt-clickzetta-0.2.6/setup.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 11:38:53.643904 dbt-clickzetta-0.2.7/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       47 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.7/MANIFEST.in
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      659 2023-06-05 11:38:53.643772 dbt-clickzetta-0.2.7/PKG-INFO
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        0 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.7/README.md
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 11:38:53.638046 dbt-clickzetta-0.2.7/dbt/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       76 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.7/dbt/__init__.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 11:38:53.637328 dbt-clickzetta-0.2.7/dbt/adapters/
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 11:38:53.639054 dbt-clickzetta-0.2.7/dbt/adapters/clickzetta/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      611 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.7/dbt/adapters/clickzetta/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       18 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.7/dbt/adapters/clickzetta/__version__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1425 2023-05-28 10:16:48.000000 dbt-clickzetta-0.2.7/dbt/adapters/clickzetta/column.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7158 2023-06-05 11:23:36.000000 dbt-clickzetta-0.2.7/dbt/adapters/clickzetta/connections.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     6958 2023-06-05 11:10:19.000000 dbt-clickzetta-0.2.7/dbt/adapters/clickzetta/impl.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      698 2023-06-05 09:54:42.000000 dbt-clickzetta-0.2.7/dbt/adapters/clickzetta/relation.py
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 11:38:53.637423 dbt-clickzetta-0.2.7/dbt/include/
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 11:38:53.639496 dbt-clickzetta-0.2.7/dbt/include/clickzetta/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       52 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.7/dbt/include/clickzetta/__init__.py
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       77 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.7/dbt/include/clickzetta/dbt_project.yml
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 11:38:53.639694 dbt-clickzetta-0.2.7/dbt/include/clickzetta/macros/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)    14274 2023-06-05 11:06:31.000000 dbt-clickzetta-0.2.7/dbt/include/clickzetta/macros/adapters.sql
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 11:38:53.640346 dbt-clickzetta-0.2.7/dbt/include/clickzetta/macros/materializations/
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 11:38:53.640848 dbt-clickzetta-0.2.7/dbt/include/clickzetta/macros/materializations/incremental/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      881 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.7/dbt/include/clickzetta/macros/materializations/incremental/column_helpers.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3419 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.7/dbt/include/clickzetta/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     3822 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.7/dbt/include/clickzetta/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2150 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.7/dbt/include/clickzetta/macros/materializations/incremental/validate.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1655 2023-06-05 08:55:29.000000 dbt-clickzetta-0.2.7/dbt/include/clickzetta/macros/materializations/seed.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     7258 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.7/dbt/include/clickzetta/macros/materializations/snapshot.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1728 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.7/dbt/include/clickzetta/macros/materializations/table.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      119 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.7/dbt/include/clickzetta/macros/materializations/view.sql
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 11:38:53.642966 dbt-clickzetta-0.2.7/dbt/include/clickzetta/macros/utils/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       92 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.7/dbt/include/clickzetta/macros/utils/any_value.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      136 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.7/dbt/include/clickzetta/macros/utils/array_append.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      113 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.7/dbt/include/clickzetta/macros/utils/array_concat.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      114 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.7/dbt/include/clickzetta/macros/utils/array_construct.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      326 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.7/dbt/include/clickzetta/macros/utils/assert_not_null.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       89 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.7/dbt/include/clickzetta/macros/utils/bool_or.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       92 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.7/dbt/include/clickzetta/macros/utils/concat.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2135 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.7/dbt/include/clickzetta/macros/utils/dateadd.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     4619 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.7/dbt/include/clickzetta/macros/utils/datediff.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      112 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.7/dbt/include/clickzetta/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      563 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.7/dbt/include/clickzetta/macros/utils/listagg.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      368 2023-06-05 11:37:14.000000 dbt-clickzetta-0.2.7/dbt/include/clickzetta/macros/utils/nullcheck.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      563 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.7/dbt/include/clickzetta/macros/utils/split_part.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       85 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.7/dbt/include/clickzetta/macros/utils/timestamps.sql
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      304 2023-05-27 20:56:12.000000 dbt-clickzetta-0.2.7/dbt/include/clickzetta/profile_template.yml
+drwxr-xr-x   0 lihanmiao   (501) staff       (20)        0 2023-06-05 11:38:53.643617 dbt-clickzetta-0.2.7/dbt_clickzetta.egg-info/
+-rw-r--r--   0 lihanmiao   (501) staff       (20)      659 2023-06-05 11:38:53.000000 dbt-clickzetta-0.2.7/dbt_clickzetta.egg-info/PKG-INFO
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     1898 2023-06-05 11:38:53.000000 dbt-clickzetta-0.2.7/dbt_clickzetta.egg-info/SOURCES.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-06-05 11:38:53.000000 dbt-clickzetta-0.2.7/dbt_clickzetta.egg-info/dependency_links.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        1 2023-06-05 11:38:53.000000 dbt-clickzetta-0.2.7/dbt_clickzetta.egg-info/not-zip-safe
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       44 2023-06-05 11:38:53.000000 dbt-clickzetta-0.2.7/dbt_clickzetta.egg-info/requires.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)        4 2023-06-05 11:38:53.000000 dbt-clickzetta-0.2.7/dbt_clickzetta.egg-info/top_level.txt
+-rw-r--r--   0 lihanmiao   (501) staff       (20)       38 2023-06-05 11:38:53.643958 dbt-clickzetta-0.2.7/setup.cfg
+-rw-r--r--   0 lihanmiao   (501) staff       (20)     2929 2023-06-05 11:38:47.000000 dbt-clickzetta-0.2.7/setup.py
```

### Comparing `dbt-clickzetta-0.2.6/dbt/adapters/clickzetta/__init__.py` & `dbt-clickzetta-0.2.7/dbt/adapters/clickzetta/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.6/dbt/adapters/clickzetta/column.py` & `dbt-clickzetta-0.2.7/dbt/adapters/clickzetta/column.py`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.6/dbt/adapters/clickzetta/connections.py` & `dbt-clickzetta-0.2.7/dbt/adapters/clickzetta/connections.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,14 +183,15 @@
         else:
             table = dbt.clients.agate_helper.empty_table()
         return response, table
 
     def add_standard_query(self, sql: str, **kwargs) -> Tuple[Connection, Any]:
         return super().add_query(self._add_query_comment(sql), **kwargs)
 
+
     def add_query(
             self,
             sql: str,
             auto_begin: bool = True,
             bindings: Optional[Any] = None,
             abridge_sql_log: bool = False,
     ) -> Tuple[Connection, Any]:  # type: ignore
```

### Comparing `dbt-clickzetta-0.2.6/dbt/adapters/clickzetta/impl.py` & `dbt-clickzetta-0.2.7/dbt/adapters/clickzetta/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.6/dbt/adapters/clickzetta/relation.py` & `dbt-clickzetta-0.2.7/dbt/adapters/clickzetta/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.6/dbt/include/clickzetta/macros/adapters.sql` & `dbt-clickzetta-0.2.7/dbt/include/clickzetta/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.6/dbt/include/clickzetta/macros/materializations/incremental/column_helpers.sql` & `dbt-clickzetta-0.2.7/dbt/include/clickzetta/macros/materializations/incremental/column_helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.6/dbt/include/clickzetta/macros/materializations/incremental/incremental.sql` & `dbt-clickzetta-0.2.7/dbt/include/clickzetta/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.6/dbt/include/clickzetta/macros/materializations/incremental/strategies.sql` & `dbt-clickzetta-0.2.7/dbt/include/clickzetta/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.6/dbt/include/clickzetta/macros/materializations/incremental/validate.sql` & `dbt-clickzetta-0.2.7/dbt/include/clickzetta/macros/materializations/incremental/validate.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.6/dbt/include/clickzetta/macros/materializations/seed.sql` & `dbt-clickzetta-0.2.7/dbt/include/clickzetta/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.6/dbt/include/clickzetta/macros/materializations/snapshot.sql` & `dbt-clickzetta-0.2.7/dbt/include/clickzetta/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.6/dbt/include/clickzetta/macros/materializations/table.sql` & `dbt-clickzetta-0.2.7/dbt/include/clickzetta/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.6/dbt/include/clickzetta/macros/utils/dateadd.sql` & `dbt-clickzetta-0.2.7/dbt/include/clickzetta/macros/utils/dateadd.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.6/dbt/include/clickzetta/macros/utils/datediff.sql` & `dbt-clickzetta-0.2.7/dbt/include/clickzetta/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.6/dbt/include/clickzetta/macros/utils/listagg.sql` & `dbt-clickzetta-0.2.7/dbt/include/clickzetta/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.6/dbt/include/clickzetta/macros/utils/split_part.sql` & `dbt-clickzetta-0.2.7/dbt/include/clickzetta/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt-clickzetta-0.2.6/dbt_clickzetta.egg-info/SOURCES.txt` & `dbt-clickzetta-0.2.7/dbt_clickzetta.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 dbt/include/clickzetta/macros/utils/assert_not_null.sql
 dbt/include/clickzetta/macros/utils/bool_or.sql
 dbt/include/clickzetta/macros/utils/concat.sql
 dbt/include/clickzetta/macros/utils/dateadd.sql
 dbt/include/clickzetta/macros/utils/datediff.sql
 dbt/include/clickzetta/macros/utils/escape_single_quotes.sql
 dbt/include/clickzetta/macros/utils/listagg.sql
+dbt/include/clickzetta/macros/utils/nullcheck.sql
 dbt/include/clickzetta/macros/utils/split_part.sql
 dbt/include/clickzetta/macros/utils/timestamps.sql
 dbt_clickzetta.egg-info/PKG-INFO
 dbt_clickzetta.egg-info/SOURCES.txt
 dbt_clickzetta.egg-info/dependency_links.txt
 dbt_clickzetta.egg-info/not-zip-safe
 dbt_clickzetta.egg-info/requires.txt
```

### Comparing `dbt-clickzetta-0.2.6/setup.py` & `dbt-clickzetta-0.2.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     parts = _get_plugin_version_dict()
     minor = "{major}.{minor}.0".format(**parts)
     pre = parts["prekind"] + "1" if parts["prekind"] else ""
     return f"{minor}{pre}"
 
 
 package_name = "dbt-clickzetta"
-package_version = "0.2.6"
+package_version = "0.2.7"
 dbt_core_version = _get_dbt_core_version()
 description = """The ClickZetta adapter plugin for dbt"""
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
```

