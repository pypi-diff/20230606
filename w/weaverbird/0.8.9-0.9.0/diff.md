# Comparing `tmp/weaverbird-0.8.9.tar.gz` & `tmp/weaverbird-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weaverbird-0.8.9.tar", last modified: Mon Nov 22 10:56:21 2021, max compression
+gzip compressed data, was "weaverbird-0.9.0.tar", last modified: Tue Dec  7 09:04:20 2021, max compression
```

## Comparing `weaverbird-0.8.9.tar` & `weaverbird-0.9.0.tar`

### file list

```diff
@@ -1,187 +1,188 @@
-drwxrwxr-x   0 d4rk3r    (1000) d4rk3r    (1000)        0 2021-11-22 10:56:21.127286 weaverbird-0.8.9/
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      205 2021-11-22 10:56:21.127286 weaverbird-0.8.9/PKG-INFO
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      844 2021-11-22 10:52:25.000000 weaverbird-0.8.9/README.md
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      339 2021-11-22 10:52:25.000000 weaverbird-0.8.9/pyproject.toml
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     1066 2021-11-22 10:56:21.127286 weaverbird-0.8.9/setup.cfg
-drwxrwxr-x   0 d4rk3r    (1000) d4rk3r    (1000)        0 2021-11-22 10:56:21.115286 weaverbird-0.8.9/src/
-drwxrwxr-x   0 d4rk3r    (1000) d4rk3r    (1000)        0 2021-11-22 10:56:21.115286 weaverbird-0.8.9/src/weaverbird/
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)        0 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/__init__.py
-drwxrwxr-x   0 d4rk3r    (1000) d4rk3r    (1000)        0 2021-11-22 10:56:21.115286 weaverbird-0.8.9/src/weaverbird/backends/
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)        0 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/__init__.py
-drwxrwxr-x   0 d4rk3r    (1000) d4rk3r    (1000)        0 2021-11-22 10:56:21.115286 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)       92 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/__init__.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     3306 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/pipeline_executor.py
-drwxrwxr-x   0 d4rk3r    (1000) d4rk3r    (1000)        0 2021-11-22 10:56:21.119286 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     3207 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/__init__.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     1790 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/addmissingdates.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     1880 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/aggregate.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      687 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/append.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      974 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/argmax.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      974 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/argmin.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      443 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/comparetext.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      574 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/concatenate.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      791 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/convert.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      641 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/cumsum.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     6697 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/date_extract.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      380 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/delete.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      373 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/domain.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      412 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/duplicate.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      819 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/duration.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     1461 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/evolution.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      413 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/fillna.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      436 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/filter.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      545 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/formula.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      461 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/fromdate.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     1450 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/ifthenelse.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      889 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/join.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      415 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/lowercase.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      790 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/moving_average.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      642 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/percentage.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      621 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/pivot.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      799 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/rank.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      390 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/rename.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      555 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/replace.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     1709 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/rollup.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      367 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/select.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      483 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/sort.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      562 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/split.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     1645 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/statistics.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     1022 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/substring.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      386 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/text.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      600 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/todate.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      682 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/top.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     3290 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/totals.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      414 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/trim.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      398 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/uniquegroups.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      610 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/unpivot.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      415 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/uppercase.py
-drwxrwxr-x   0 d4rk3r    (1000) d4rk3r    (1000)        0 2021-11-22 10:56:21.119286 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/utils/
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)        0 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/utils/__init__.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     1015 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/utils/cast.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     2019 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/utils/cleaning.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      756 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/utils/combination.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     1610 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/utils/condition.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     1447 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/utils/formula.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     5964 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/waterfall.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      794 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/types.py
-drwxrwxr-x   0 d4rk3r    (1000) d4rk3r    (1000)        0 2021-11-22 10:56:21.119286 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      123 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/__init__.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)    22608 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/metadata.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     2495 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/sql_pipeline_translator.py
-drwxrwxr-x   0 d4rk3r    (1000) d4rk3r    (1000)        0 2021-11-22 10:56:21.123286 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     2933 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/__init__.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     1631 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/aggregate.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     3153 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/append.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     2527 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/argmax.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     2527 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/argmin.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     2313 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/concatenate.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     3145 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/convert.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     2764 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/cumsum.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     1914 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/customsql.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     2924 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/dateextract.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     1722 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/delete.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     2260 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/duplicate.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     2305 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/duration.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     2752 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/evolution.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     1490 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/fillna.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     1349 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/filter.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     2480 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/formula.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     2277 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/fromdate.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     3005 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/ifthenelse.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     3358 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/join.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     2059 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/lowercase.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     2891 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/percentage.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     3260 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/pivot.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     2963 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/rank.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     2278 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/rename.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     2669 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/replace.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     1699 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/rollup.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     1861 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/select.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     2380 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/sort.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     2830 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/split.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     2817 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/substring.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     1728 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/table.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     2221 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/text.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     2280 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/todate.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     2467 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/top.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     5489 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/totals.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     2382 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/uniquegroups.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     2956 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/unpivot.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     2051 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/uppercase.py
-drwxrwxr-x   0 d4rk3r    (1000) d4rk3r    (1000)        0 2021-11-22 10:56:21.123286 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/utils/
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)        0 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/utils/__init__.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     6592 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/utils/aggregation.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      859 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/utils/combination.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)    17760 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/utils/query_transformation.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     1354 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/backends/sql_translator/types.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      298 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/exceptions.py
-drwxrwxr-x   0 d4rk3r    (1000) d4rk3r    (1000)        0 2021-11-22 10:56:21.123286 weaverbird-0.8.9/src/weaverbird/pipeline/
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)       95 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/__init__.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     1328 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/conditions.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      263 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/dates.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     4015 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/pipeline.py
-drwxrwxr-x   0 d4rk3r    (1000) d4rk3r    (1000)        0 2021-11-22 10:56:21.127286 weaverbird-0.8.9/src/weaverbird/pipeline/steps/
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     2329 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/__init__.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      817 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/addmissingdates.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     1991 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/aggregate.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      435 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/append.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      519 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/argmax.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      559 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/argmin.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      682 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/comparetext.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      597 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/concatenate.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      340 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/convert.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      643 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/cumsum.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      392 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/customsql.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     1432 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/date_extract.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      259 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/delete.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      171 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/domain.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      265 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/duplicate.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      933 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/duration.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     1012 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/evolution.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      658 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/fillna.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      378 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/filter.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      412 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/formula.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      247 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/fromdate.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      897 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/ifthenelse.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      659 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/join.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      233 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/lowercase.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      549 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/moving_average.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      385 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/percentage.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      592 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/pivot.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      722 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/rank.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      857 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/rename.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      604 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/replace.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     1296 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/rollup.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      280 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/select.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      444 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/sort.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      476 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/split.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      866 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/statistics.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      375 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/substring.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      170 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/table.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      397 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/text.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      282 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/todate.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      561 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/top.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     1233 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/totals.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      255 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/trim.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      514 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/uniquegroups.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      678 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/unpivot.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      233 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/uppercase.py
-drwxrwxr-x   0 d4rk3r    (1000) d4rk3r    (1000)        0 2021-11-22 10:56:21.127286 weaverbird-0.8.9/src/weaverbird/pipeline/steps/utils/
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)        0 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/utils/__init__.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      446 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/utils/base.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      132 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/utils/combination.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      404 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/utils/render_variables.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      265 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/utils/validation.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      926 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/steps/waterfall.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      164 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/pipeline/types.py
-drwxrwxr-x   0 d4rk3r    (1000) d4rk3r    (1000)        0 2021-11-22 10:56:21.127286 weaverbird-0.8.9/src/weaverbird/utils/
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)       64 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/utils/__init__.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      338 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/utils/iter.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      308 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/utils/size.py
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      231 2021-11-22 10:52:25.000000 weaverbird-0.8.9/src/weaverbird/utils/stopwatch.py
-drwxrwxr-x   0 d4rk3r    (1000) d4rk3r    (1000)        0 2021-11-22 10:56:21.115286 weaverbird-0.8.9/src/weaverbird.egg-info/
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      205 2021-11-22 10:56:21.000000 weaverbird-0.8.9/src/weaverbird.egg-info/PKG-INFO
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)     8522 2021-11-22 10:56:21.000000 weaverbird-0.8.9/src/weaverbird.egg-info/SOURCES.txt
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)        1 2021-11-22 10:56:21.000000 weaverbird-0.8.9/src/weaverbird.egg-info/dependency_links.txt
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)      360 2021-11-22 10:56:21.000000 weaverbird-0.8.9/src/weaverbird.egg-info/requires.txt
--rw-rw-r--   0 d4rk3r    (1000) d4rk3r    (1000)       11 2021-11-22 10:56:21.000000 weaverbird-0.8.9/src/weaverbird.egg-info/top_level.txt
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-12-07 09:04:20.960612 weaverbird-0.9.0/
+-rw-rw-r--   0 david     (1000) david     (1000)      205 2021-12-07 09:04:20.960612 weaverbird-0.9.0/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)      844 2021-11-24 14:07:16.000000 weaverbird-0.9.0/README.md
+-rw-rw-r--   0 david     (1000) david     (1000)      339 2021-11-24 14:07:16.000000 weaverbird-0.9.0/pyproject.toml
+-rw-rw-r--   0 david     (1000) david     (1000)     1089 2021-12-07 09:04:20.964612 weaverbird-0.9.0/setup.cfg
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-12-07 09:04:20.940612 weaverbird-0.9.0/src/
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-12-07 09:04:20.944612 weaverbird-0.9.0/src/weaverbird/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-12-07 09:04:20.944612 weaverbird-0.9.0/src/weaverbird/backends/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-12-07 09:04:20.944612 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/
+-rw-rw-r--   0 david     (1000) david     (1000)       92 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3306 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/pipeline_executor.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-12-07 09:04:20.948612 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/
+-rw-rw-r--   0 david     (1000) david     (1000)     3207 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1790 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/addmissingdates.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1880 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/aggregate.py
+-rw-rw-r--   0 david     (1000) david     (1000)      687 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/append.py
+-rw-rw-r--   0 david     (1000) david     (1000)      974 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/argmax.py
+-rw-rw-r--   0 david     (1000) david     (1000)      974 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/argmin.py
+-rw-rw-r--   0 david     (1000) david     (1000)      443 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/comparetext.py
+-rw-rw-r--   0 david     (1000) david     (1000)      574 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/concatenate.py
+-rw-rw-r--   0 david     (1000) david     (1000)      791 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/convert.py
+-rw-rw-r--   0 david     (1000) david     (1000)      641 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/cumsum.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6697 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/date_extract.py
+-rw-rw-r--   0 david     (1000) david     (1000)      380 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/delete.py
+-rw-rw-r--   0 david     (1000) david     (1000)      373 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/domain.py
+-rw-rw-r--   0 david     (1000) david     (1000)      412 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/duplicate.py
+-rw-rw-r--   0 david     (1000) david     (1000)      819 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/duration.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1461 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/evolution.py
+-rw-rw-r--   0 david     (1000) david     (1000)      413 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/fillna.py
+-rw-rw-r--   0 david     (1000) david     (1000)      436 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/filter.py
+-rw-rw-r--   0 david     (1000) david     (1000)      545 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/formula.py
+-rw-rw-r--   0 david     (1000) david     (1000)      461 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/fromdate.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1450 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/ifthenelse.py
+-rw-rw-r--   0 david     (1000) david     (1000)      889 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/join.py
+-rw-rw-r--   0 david     (1000) david     (1000)      415 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/lowercase.py
+-rw-rw-r--   0 david     (1000) david     (1000)      790 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/moving_average.py
+-rw-rw-r--   0 david     (1000) david     (1000)      642 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/percentage.py
+-rw-rw-r--   0 david     (1000) david     (1000)      621 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/pivot.py
+-rw-rw-r--   0 david     (1000) david     (1000)      799 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/rank.py
+-rw-rw-r--   0 david     (1000) david     (1000)      390 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/rename.py
+-rw-rw-r--   0 david     (1000) david     (1000)      555 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/replace.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1709 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/rollup.py
+-rw-rw-r--   0 david     (1000) david     (1000)      367 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/select.py
+-rw-rw-r--   0 david     (1000) david     (1000)      483 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/sort.py
+-rw-rw-r--   0 david     (1000) david     (1000)      562 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/split.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1645 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/statistics.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1022 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/substring.py
+-rw-rw-r--   0 david     (1000) david     (1000)      386 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/text.py
+-rw-rw-r--   0 david     (1000) david     (1000)      600 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/todate.py
+-rw-rw-r--   0 david     (1000) david     (1000)      682 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/top.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3290 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/totals.py
+-rw-rw-r--   0 david     (1000) david     (1000)      414 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/trim.py
+-rw-rw-r--   0 david     (1000) david     (1000)      398 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/uniquegroups.py
+-rw-rw-r--   0 david     (1000) david     (1000)      610 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/unpivot.py
+-rw-rw-r--   0 david     (1000) david     (1000)      415 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/uppercase.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-12-07 09:04:20.948612 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/utils/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/utils/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1015 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/utils/cast.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2019 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/utils/cleaning.py
+-rw-rw-r--   0 david     (1000) david     (1000)      756 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/utils/combination.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2677 2021-12-07 09:01:59.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/utils/condition.py
+-rw-rw-r--   0 david     (1000) david     (1000)      848 2021-12-07 09:01:59.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/utils/dates.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1447 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/utils/formula.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5964 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/waterfall.py
+-rw-rw-r--   0 david     (1000) david     (1000)      794 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/types.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-12-07 09:04:20.952612 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/
+-rw-rw-r--   0 david     (1000) david     (1000)      123 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    22608 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/metadata.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2495 2021-12-06 13:41:05.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/sql_pipeline_translator.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-12-07 09:04:20.956612 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/
+-rw-rw-r--   0 david     (1000) david     (1000)     2933 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1631 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/aggregate.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3153 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/append.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2527 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/argmax.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2527 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/argmin.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2313 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/concatenate.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3145 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/convert.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2764 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/cumsum.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1914 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/customsql.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2924 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/dateextract.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1722 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/delete.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2260 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/duplicate.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2305 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/duration.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2752 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/evolution.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1490 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/fillna.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1349 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/filter.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2480 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/formula.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2277 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/fromdate.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3005 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/ifthenelse.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3358 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/join.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2059 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/lowercase.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2891 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/percentage.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3260 2021-12-07 09:01:56.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/pivot.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2963 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/rank.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2278 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/rename.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2669 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/replace.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1699 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/rollup.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1861 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/select.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2380 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/sort.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2830 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/split.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2817 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/substring.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1728 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/table.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2221 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/text.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2280 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/todate.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2467 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/top.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5489 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/totals.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2382 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/uniquegroups.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2956 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/unpivot.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2051 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/uppercase.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-12-07 09:04:20.956612 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/utils/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/utils/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6592 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/utils/aggregation.py
+-rw-rw-r--   0 david     (1000) david     (1000)      859 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/utils/combination.py
+-rw-rw-r--   0 david     (1000) david     (1000)    18828 2021-12-07 09:01:59.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/utils/query_transformation.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1354 2021-12-07 09:01:56.000000 weaverbird-0.9.0/src/weaverbird/backends/sql_translator/types.py
+-rw-rw-r--   0 david     (1000) david     (1000)      298 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/exceptions.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-12-07 09:04:20.956612 weaverbird-0.9.0/src/weaverbird/pipeline/
+-rw-rw-r--   0 david     (1000) david     (1000)       95 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1599 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/conditions.py
+-rw-rw-r--   0 david     (1000) david     (1000)      321 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/dates.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4015 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/pipeline.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-12-07 09:04:20.960612 weaverbird-0.9.0/src/weaverbird/pipeline/steps/
+-rw-rw-r--   0 david     (1000) david     (1000)     2329 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      817 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/addmissingdates.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1991 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/aggregate.py
+-rw-rw-r--   0 david     (1000) david     (1000)      435 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/append.py
+-rw-rw-r--   0 david     (1000) david     (1000)      519 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/argmax.py
+-rw-rw-r--   0 david     (1000) david     (1000)      559 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/argmin.py
+-rw-rw-r--   0 david     (1000) david     (1000)      682 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/comparetext.py
+-rw-rw-r--   0 david     (1000) david     (1000)      597 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/concatenate.py
+-rw-rw-r--   0 david     (1000) david     (1000)      340 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/convert.py
+-rw-rw-r--   0 david     (1000) david     (1000)      643 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/cumsum.py
+-rw-rw-r--   0 david     (1000) david     (1000)      392 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/customsql.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1432 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/date_extract.py
+-rw-rw-r--   0 david     (1000) david     (1000)      259 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/delete.py
+-rw-rw-r--   0 david     (1000) david     (1000)      171 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/domain.py
+-rw-rw-r--   0 david     (1000) david     (1000)      265 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/duplicate.py
+-rw-rw-r--   0 david     (1000) david     (1000)      933 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/duration.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1012 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/evolution.py
+-rw-rw-r--   0 david     (1000) david     (1000)      658 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/fillna.py
+-rw-rw-r--   0 david     (1000) david     (1000)      378 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/filter.py
+-rw-rw-r--   0 david     (1000) david     (1000)      412 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/formula.py
+-rw-rw-r--   0 david     (1000) david     (1000)      247 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/fromdate.py
+-rw-rw-r--   0 david     (1000) david     (1000)      897 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/ifthenelse.py
+-rw-rw-r--   0 david     (1000) david     (1000)      659 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/join.py
+-rw-rw-r--   0 david     (1000) david     (1000)      233 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/lowercase.py
+-rw-rw-r--   0 david     (1000) david     (1000)      549 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/moving_average.py
+-rw-rw-r--   0 david     (1000) david     (1000)      385 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/percentage.py
+-rw-rw-r--   0 david     (1000) david     (1000)      592 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/pivot.py
+-rw-rw-r--   0 david     (1000) david     (1000)      722 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/rank.py
+-rw-rw-r--   0 david     (1000) david     (1000)      857 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/rename.py
+-rw-rw-r--   0 david     (1000) david     (1000)      604 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/replace.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1296 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/rollup.py
+-rw-rw-r--   0 david     (1000) david     (1000)      280 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/select.py
+-rw-rw-r--   0 david     (1000) david     (1000)      444 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/sort.py
+-rw-rw-r--   0 david     (1000) david     (1000)      476 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/split.py
+-rw-rw-r--   0 david     (1000) david     (1000)      866 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/statistics.py
+-rw-rw-r--   0 david     (1000) david     (1000)      375 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/substring.py
+-rw-rw-r--   0 david     (1000) david     (1000)      170 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/table.py
+-rw-rw-r--   0 david     (1000) david     (1000)      397 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/text.py
+-rw-rw-r--   0 david     (1000) david     (1000)      282 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/todate.py
+-rw-rw-r--   0 david     (1000) david     (1000)      561 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/top.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1233 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/totals.py
+-rw-rw-r--   0 david     (1000) david     (1000)      255 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/trim.py
+-rw-rw-r--   0 david     (1000) david     (1000)      514 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/uniquegroups.py
+-rw-rw-r--   0 david     (1000) david     (1000)      678 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/unpivot.py
+-rw-rw-r--   0 david     (1000) david     (1000)      233 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/uppercase.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-12-07 09:04:20.960612 weaverbird-0.9.0/src/weaverbird/pipeline/steps/utils/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/utils/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      446 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/utils/base.py
+-rw-rw-r--   0 david     (1000) david     (1000)      132 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/utils/combination.py
+-rw-rw-r--   0 david     (1000) david     (1000)      404 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/utils/render_variables.py
+-rw-rw-r--   0 david     (1000) david     (1000)      265 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/utils/validation.py
+-rw-rw-r--   0 david     (1000) david     (1000)      926 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/steps/waterfall.py
+-rw-rw-r--   0 david     (1000) david     (1000)      164 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/pipeline/types.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-12-07 09:04:20.960612 weaverbird-0.9.0/src/weaverbird/utils/
+-rw-rw-r--   0 david     (1000) david     (1000)       64 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/utils/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      338 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/utils/iter.py
+-rw-rw-r--   0 david     (1000) david     (1000)      308 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/utils/size.py
+-rw-rw-r--   0 david     (1000) david     (1000)      231 2021-11-24 14:07:16.000000 weaverbird-0.9.0/src/weaverbird/utils/stopwatch.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2021-12-07 09:04:20.944612 weaverbird-0.9.0/src/weaverbird.egg-info/
+-rw-rw-r--   0 david     (1000) david     (1000)      205 2021-12-07 09:04:20.000000 weaverbird-0.9.0/src/weaverbird.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     8583 2021-12-07 09:04:20.000000 weaverbird-0.9.0/src/weaverbird.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2021-12-07 09:04:20.000000 weaverbird-0.9.0/src/weaverbird.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)      382 2021-12-07 09:04:20.000000 weaverbird-0.9.0/src/weaverbird.egg-info/requires.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       11 2021-12-07 09:04:20.000000 weaverbird-0.9.0/src/weaverbird.egg-info/top_level.txt
```

### Comparing `weaverbird-0.8.9/README.md` & `weaverbird-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/setup.cfg` & `weaverbird-0.9.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = weaverbird
-version = 0.8.9
+version = 0.9.0
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.8
 install_requires = 
@@ -23,14 +23,15 @@
 dev = 
 	pytest >= 6.1.1, < 7
 	pytest-cov >= 2.10.1, < 3
 	black == 20.8b1
 	flake8 == 3.8.4
 	isort == 5.6.4
 	mypy == 0.910
+	types-python-dateutil
 	pytest-mock >= 3.3.1, < 4
 	toucan-connectors > 0 # required so we can use nosql_apply_parameters_to_query during tests
 	pytest-benchmark >= 3.4.1, < 4
 	docker == 5.0.0
 	sqlalchemy == 1.4.22
 	pymysql == 1.0.2
 	cryptography == 3.4.7
```

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/pipeline_executor.py` & `weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/pipeline_executor.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/__init__.py` & `weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/addmissingdates.py` & `weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/addmissingdates.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/aggregate.py` & `weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/aggregate.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/append.py` & `weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/append.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/argmax.py` & `weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/argmax.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/argmin.py` & `weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/argmin.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/concatenate.py` & `weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/concatenate.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/convert.py` & `weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/convert.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/cumsum.py` & `weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/cumsum.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/date_extract.py` & `weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/date_extract.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/duration.py` & `weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/duration.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/evolution.py` & `weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/evolution.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/formula.py` & `weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/formula.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/ifthenelse.py` & `weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/ifthenelse.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/join.py` & `weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/join.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/moving_average.py` & `weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/moving_average.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/percentage.py` & `weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/percentage.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/pivot.py` & `weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/pivot.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/rank.py` & `weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/rank.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/replace.py` & `weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/replace.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/rollup.py` & `weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/rollup.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/split.py` & `weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/split.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/statistics.py` & `weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/statistics.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/substring.py` & `weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/substring.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/todate.py` & `weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/todate.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/top.py` & `weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/top.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/totals.py` & `weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/totals.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/unpivot.py` & `weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/unpivot.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/utils/cast.py` & `weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/utils/cast.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/utils/cleaning.py` & `weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/utils/cleaning.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/utils/combination.py` & `weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/utils/combination.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/utils/formula.py` & `weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/utils/formula.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/steps/waterfall.py` & `weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/steps/waterfall.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/pandas_executor/types.py` & `weaverbird-0.9.0/src/weaverbird/backends/pandas_executor/types.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/metadata.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/metadata.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/sql_pipeline_translator.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/sql_pipeline_translator.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/__init__.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/aggregate.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/aggregate.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/append.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/append.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/argmax.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/argmax.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/argmin.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/argmin.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/concatenate.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/concatenate.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/convert.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/convert.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/cumsum.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/cumsum.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/customsql.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/customsql.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/dateextract.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/dateextract.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/delete.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/delete.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/duplicate.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/duplicate.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/duration.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/duration.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/evolution.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/evolution.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/fillna.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/fillna.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/filter.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/filter.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/formula.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/formula.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/fromdate.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/fromdate.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/ifthenelse.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/ifthenelse.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/join.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/join.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/lowercase.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/lowercase.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/percentage.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/percentage.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/pivot.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/pivot.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/rank.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/rank.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/rename.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/rename.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/replace.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/replace.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/rollup.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/rollup.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/select.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/select.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/sort.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/sort.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/split.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/split.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/substring.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/substring.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/table.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/table.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/text.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/text.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/todate.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/todate.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/top.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/top.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/totals.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/totals.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/uniquegroups.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/uniquegroups.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/unpivot.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/unpivot.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/uppercase.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/uppercase.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/utils/aggregation.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/utils/aggregation.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/utils/combination.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/utils/combination.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/steps/utils/query_transformation.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/steps/utils/query_transformation.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,27 +5,31 @@
 from weaverbird.backends.sql_translator.metadata import ColumnMetadata, SqlQueryMetadataManager
 from weaverbird.backends.sql_translator.types import SQLQuery
 from weaverbird.pipeline.conditions import (
     ComparisonCondition,
     Condition,
     ConditionComboAnd,
     ConditionComboOr,
+    DateBoundCondition,
     InclusionCondition,
     MatchCondition,
     NullCondition,
 )
+from weaverbird.pipeline.dates import RelativeDate
 from weaverbird.pipeline.steps import AggregateStep
 
 SQL_COMPARISON_OPERATORS = {
     'eq': '=',
     'ne': '!=',
     'lt': '<',
     'le': '<=',
     'gt': '>',
     'ge': '>=',
+    'from': '>=',
+    'until': '<=',
 }
 
 SQL_NULLITY_OPERATORS = {
     'isnull': 'IS NULL',
     'notnull': 'IS NOT NULL',
 }
 
@@ -63,14 +67,37 @@
     elif isinstance(condition, MatchCondition):
         # just to escape single quotes from crashing the snowflakeSQL query
         if type(condition.value) == str:
             condition.value = sanitize_input(condition.value)
         query += f"{condition.column} {SQL_MATCH_OPERATORS[condition.operator]} '{condition.value}'"
     elif isinstance(condition, InclusionCondition):
         query += f'{condition.column} {SQL_INCLUSION_OPERATORS[condition.operator]} {str(tuple(condition.value))}'
+
+    elif isinstance(condition, DateBoundCondition):
+
+        value = condition.value
+        if isinstance(value, RelativeDate):
+            if value.operator == 'until':
+                sign = -1
+            elif value.operator == 'from':
+                sign = 1
+            else:
+                raise NotImplementedError
+            value_query_part = f"dateadd({ value.duration }, { sign * value.quantity }, '{ value.date.isoformat() }'::DATE)"
+        else:
+            value_query_part = f"to_timestamp('{ value.isoformat() }')"
+
+        # Remove time info from the column to filter on
+        column = f'to_timestamp({ condition.column })'
+        column_without_time = f"DATE_TRUNC('DAY', { column })"
+        # Do the same with the value to compare it to
+        value_without_time = f"DATE_TRUNC('DAY', { value_query_part })"
+
+        query += f'{ column_without_time } { SQL_COMPARISON_OPERATORS[condition.operator] } { value_without_time }'
+
     elif isinstance(condition, ConditionComboAnd):
         query = apply_condition(condition.and_[0], query)
         for c in condition.and_[1:]:
             query = apply_condition(c, f'{query} AND ')
     elif isinstance(condition, ConditionComboOr):
         query = apply_condition(condition.or_[0], query)
         for c in condition.or_[1:]:
```

### Comparing `weaverbird-0.8.9/src/weaverbird/backends/sql_translator/types.py` & `weaverbird-0.9.0/src/weaverbird/backends/sql_translator/types.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/pipeline/conditions.py` & `weaverbird-0.9.0/src/weaverbird/pipeline/conditions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from abc import ABC
+from datetime import datetime
 from typing import Any, List, Literal, Union
 
 from pydantic import BaseModel, Field
 
+from weaverbird.pipeline.dates import RelativeDate
 from weaverbird.pipeline.types import ColumnName, PopulatedWithFieldnames
 
 
 class BaseCondition(BaseModel):
     ...
 
 
@@ -29,15 +31,27 @@
 
 class MatchCondition(BaseCondition):
     column: ColumnName
     operator: Literal['matches', 'notmatches']
     value: str
 
 
-SimpleCondition = Union[ComparisonCondition, InclusionCondition, NullCondition, MatchCondition]
+class DateBoundCondition(BaseModel):
+    column: ColumnName
+    operator: Literal['from', 'until']
+    value: Union[RelativeDate, datetime, str]
+
+
+SimpleCondition = Union[
+    ComparisonCondition,
+    InclusionCondition,
+    NullCondition,
+    MatchCondition,
+    DateBoundCondition,
+]
 
 
 class BaseConditionCombo(BaseCondition, ABC):
     class Config(PopulatedWithFieldnames):
         ...
 
     def to_dict(self):
```

### Comparing `weaverbird-0.8.9/src/weaverbird/pipeline/pipeline.py` & `weaverbird-0.9.0/src/weaverbird/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/pipeline/steps/__init__.py` & `weaverbird-0.9.0/src/weaverbird/pipeline/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/pipeline/steps/addmissingdates.py` & `weaverbird-0.9.0/src/weaverbird/pipeline/steps/addmissingdates.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/pipeline/steps/aggregate.py` & `weaverbird-0.9.0/src/weaverbird/pipeline/steps/aggregate.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/pipeline/steps/argmax.py` & `weaverbird-0.9.0/src/weaverbird/pipeline/steps/argmax.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/pipeline/steps/argmin.py` & `weaverbird-0.9.0/src/weaverbird/pipeline/steps/argmin.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/pipeline/steps/comparetext.py` & `weaverbird-0.9.0/src/weaverbird/pipeline/steps/comparetext.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/pipeline/steps/concatenate.py` & `weaverbird-0.9.0/src/weaverbird/pipeline/steps/concatenate.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/pipeline/steps/cumsum.py` & `weaverbird-0.9.0/src/weaverbird/pipeline/steps/cumsum.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/pipeline/steps/date_extract.py` & `weaverbird-0.9.0/src/weaverbird/pipeline/steps/date_extract.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/pipeline/steps/duration.py` & `weaverbird-0.9.0/src/weaverbird/pipeline/steps/duration.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/pipeline/steps/evolution.py` & `weaverbird-0.9.0/src/weaverbird/pipeline/steps/evolution.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/pipeline/steps/fillna.py` & `weaverbird-0.9.0/src/weaverbird/pipeline/steps/fillna.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/pipeline/steps/ifthenelse.py` & `weaverbird-0.9.0/src/weaverbird/pipeline/steps/ifthenelse.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/pipeline/steps/join.py` & `weaverbird-0.9.0/src/weaverbird/pipeline/steps/join.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/pipeline/steps/moving_average.py` & `weaverbird-0.9.0/src/weaverbird/pipeline/steps/moving_average.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/pipeline/steps/pivot.py` & `weaverbird-0.9.0/src/weaverbird/pipeline/steps/pivot.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/pipeline/steps/rank.py` & `weaverbird-0.9.0/src/weaverbird/pipeline/steps/rank.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/pipeline/steps/rename.py` & `weaverbird-0.9.0/src/weaverbird/pipeline/steps/rename.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/pipeline/steps/replace.py` & `weaverbird-0.9.0/src/weaverbird/pipeline/steps/replace.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/pipeline/steps/rollup.py` & `weaverbird-0.9.0/src/weaverbird/pipeline/steps/rollup.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/pipeline/steps/statistics.py` & `weaverbird-0.9.0/src/weaverbird/pipeline/steps/statistics.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/pipeline/steps/top.py` & `weaverbird-0.9.0/src/weaverbird/pipeline/steps/top.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/pipeline/steps/totals.py` & `weaverbird-0.9.0/src/weaverbird/pipeline/steps/totals.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/pipeline/steps/uniquegroups.py` & `weaverbird-0.9.0/src/weaverbird/pipeline/steps/uniquegroups.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/pipeline/steps/unpivot.py` & `weaverbird-0.9.0/src/weaverbird/pipeline/steps/unpivot.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird/pipeline/steps/waterfall.py` & `weaverbird-0.9.0/src/weaverbird/pipeline/steps/waterfall.py`

 * *Files identical despite different names*

### Comparing `weaverbird-0.8.9/src/weaverbird.egg-info/SOURCES.txt` & `weaverbird-0.9.0/src/weaverbird.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 src/weaverbird/backends/pandas_executor/steps/uppercase.py
 src/weaverbird/backends/pandas_executor/steps/waterfall.py
 src/weaverbird/backends/pandas_executor/steps/utils/__init__.py
 src/weaverbird/backends/pandas_executor/steps/utils/cast.py
 src/weaverbird/backends/pandas_executor/steps/utils/cleaning.py
 src/weaverbird/backends/pandas_executor/steps/utils/combination.py
 src/weaverbird/backends/pandas_executor/steps/utils/condition.py
+src/weaverbird/backends/pandas_executor/steps/utils/dates.py
 src/weaverbird/backends/pandas_executor/steps/utils/formula.py
 src/weaverbird/backends/sql_translator/__init__.py
 src/weaverbird/backends/sql_translator/metadata.py
 src/weaverbird/backends/sql_translator/sql_pipeline_translator.py
 src/weaverbird/backends/sql_translator/types.py
 src/weaverbird/backends/sql_translator/steps/__init__.py
 src/weaverbird/backends/sql_translator/steps/aggregate.py
```

