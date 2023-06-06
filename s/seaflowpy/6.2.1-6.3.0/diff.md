# Comparing `tmp/seaflowpy-6.2.1.tar.gz` & `tmp/seaflowpy-6.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaflowpy-6.2.1.tar", last modified: Wed May 17 22:09:20 2023, max compression
+gzip compressed data, was "seaflowpy-6.3.0.tar", last modified: Tue Jun  6 19:55:54 2023, max compression
```

## Comparing `seaflowpy-6.2.1.tar` & `seaflowpy-6.3.0.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:09:20.614244 seaflowpy-6.2.1/
--rw-r--r--   0 root         (0) root         (0)    35147 2016-05-27 19:28:44.000000 seaflowpy-6.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      196 2020-07-31 01:20:45.000000 seaflowpy-6.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6771 2023-05-17 22:09:20.614244 seaflowpy-6.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6399 2021-04-02 19:11:59.000000 seaflowpy-6.2.1/README.md
--rw-r--r--   0 root         (0) root         (0)      245 2023-05-17 22:09:20.614244 seaflowpy-6.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      954 2022-10-27 20:07:07.000000 seaflowpy-6.2.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:09:20.579244 seaflowpy-6.2.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:09:20.615244 seaflowpy-6.2.1/src/seaflowpy/
--rw-r--r--   0 root         (0) root         (0)      317 2022-10-26 23:57:59.000000 seaflowpy-6.2.1/src/seaflowpy/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-05-17 22:09:20.615244 seaflowpy-6.2.1/src/seaflowpy/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:09:20.589244 seaflowpy-6.2.1/src/seaflowpy/cli/
--rw-r--r--   0 root         (0) root         (0)       18 2020-03-25 18:47:11.000000 seaflowpy-6.2.1/src/seaflowpy/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)      872 2022-08-19 02:08:17.000000 seaflowpy-6.2.1/src/seaflowpy/cli/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:09:20.591244 seaflowpy-6.2.1/src/seaflowpy/cli/commands/
--rw-r--r--   0 root         (0) root         (0)      192 2022-08-19 02:07:55.000000 seaflowpy-6.2.1/src/seaflowpy/cli/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1025 2020-03-25 18:47:11.000000 seaflowpy-6.2.1/src/seaflowpy/cli/commands/dayofyear_cmd.py
--rw-r--r--   0 root         (0) root         (0)     5296 2020-07-19 21:48:09.000000 seaflowpy-6.2.1/src/seaflowpy/cli/commands/db_cmd.py
--rw-r--r--   0 root         (0) root         (0)    12247 2022-10-28 22:17:48.000000 seaflowpy-6.2.1/src/seaflowpy/cli/commands/evt_cmd.py
--rw-r--r--   0 root         (0) root         (0)     4970 2022-02-21 23:55:50.000000 seaflowpy-6.2.1/src/seaflowpy/cli/commands/filter_cmd.py
--rw-r--r--   0 root         (0) root         (0)     4876 2022-08-20 19:35:27.000000 seaflowpy-6.2.1/src/seaflowpy/cli/commands/opp_cmd.py
--rw-r--r--   0 root         (0) root         (0)     3999 2020-03-25 18:47:11.000000 seaflowpy-6.2.1/src/seaflowpy/cli/commands/sds2sfl_cmd.py
--rw-r--r--   0 root         (0) root         (0)    11035 2022-10-26 19:25:20.000000 seaflowpy-6.2.1/src/seaflowpy/cli/commands/sfl_cmd.py
--rw-r--r--   0 root         (0) root         (0)      194 2020-03-25 18:47:11.000000 seaflowpy-6.2.1/src/seaflowpy/cli/commands/version_cmd.py
--rw-r--r--   0 root         (0) root         (0)      889 2022-10-05 00:55:36.000000 seaflowpy-6.2.1/src/seaflowpy/cloud.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:09:20.592244 seaflowpy-6.2.1/src/seaflowpy/data/
--rw-r--r--   0 root         (0) root         (0)     4882 2022-02-17 23:58:06.000000 seaflowpy-6.2.1/src/seaflowpy/data/popcycle.sql
--rw-r--r--   0 root         (0) root         (0)    11780 2022-02-18 01:01:04.000000 seaflowpy-6.2.1/src/seaflowpy/db.py
--rw-r--r--   0 root         (0) root         (0)      405 2022-10-05 00:55:11.000000 seaflowpy-6.2.1/src/seaflowpy/errors.py
--rw-r--r--   0 root         (0) root         (0)    13696 2022-08-22 23:54:55.000000 seaflowpy-6.2.1/src/seaflowpy/fileio.py
--rw-r--r--   0 root         (0) root         (0)    13776 2022-04-21 21:40:19.000000 seaflowpy-6.2.1/src/seaflowpy/filterevt.py
--rw-r--r--   0 root         (0) root         (0)     1802 2020-03-25 18:47:11.000000 seaflowpy-6.2.1/src/seaflowpy/geo.py
--rw-r--r--   0 root         (0) root         (0)    11203 2022-12-02 21:17:41.000000 seaflowpy-6.2.1/src/seaflowpy/particleops.py
--rw-r--r--   0 root         (0) root         (0)    10280 2022-10-31 23:12:46.000000 seaflowpy-6.2.1/src/seaflowpy/sample.py
--rw-r--r--   0 root         (0) root         (0)     9411 2022-08-18 22:28:13.000000 seaflowpy-6.2.1/src/seaflowpy/seaflowfile.py
--rw-r--r--   0 root         (0) root         (0)    19632 2023-03-09 20:38:00.000000 seaflowpy-6.2.1/src/seaflowpy/sfl.py
--rw-r--r--   0 root         (0) root         (0)      788 2020-06-11 19:02:16.000000 seaflowpy-6.2.1/src/seaflowpy/time.py
--rw-r--r--   0 root         (0) root         (0)     3779 2022-10-05 00:08:13.000000 seaflowpy-6.2.1/src/seaflowpy/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:09:20.588244 seaflowpy-6.2.1/src/seaflowpy.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6771 2023-05-17 22:09:20.000000 seaflowpy-6.2.1/src/seaflowpy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2961 2023-05-17 22:09:20.000000 seaflowpy-6.2.1/src/seaflowpy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 22:09:20.000000 seaflowpy-6.2.1/src/seaflowpy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2023-05-17 22:09:20.000000 seaflowpy-6.2.1/src/seaflowpy.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       47 2023-05-17 22:09:20.000000 seaflowpy-6.2.1/src/seaflowpy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-17 22:09:20.000000 seaflowpy-6.2.1/src/seaflowpy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 22:09:20.000000 seaflowpy-6.2.1/src/seaflowpy.egg-info/zip-safe
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:09:20.596244 seaflowpy-6.2.1/tests/
--rw-r--r--   0 root         (0) root         (0)     4604 2022-02-18 03:14:13.000000 seaflowpy-6.2.1/tests/file_dates.parquet
--rw-r--r--   0 root         (0) root         (0)    15333 2020-06-30 22:53:10.000000 seaflowpy-6.2.1/tests/sfl.parquet
--rw-r--r--   0 root         (0) root         (0)    18822 2022-10-31 23:10:56.000000 seaflowpy-6.2.1/tests/test_evtopp.py
--rw-r--r--   0 root         (0) root         (0)     3705 2020-06-11 19:02:16.000000 seaflowpy-6.2.1/tests/test_geo.py
--rw-r--r--   0 root         (0) root         (0)     8000 2022-10-31 23:36:27.000000 seaflowpy-6.2.1/tests/test_sample.py
--rw-r--r--   0 root         (0) root         (0)    18787 2022-02-18 18:39:19.000000 seaflowpy-6.2.1/tests/test_seaflowfile.py
--rw-r--r--   0 root         (0) root         (0)     1104 2020-06-11 19:02:16.000000 seaflowpy-6.2.1/tests/test_time.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:09:20.580244 seaflowpy-6.2.1/tests/testcruise_evt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:09:20.604244 seaflowpy-6.2.1/tests/testcruise_evt/2014_185/
--rw-r--r--   0 root         (0) root         (0)     1468 2022-02-18 02:29:25.000000 seaflowpy-6.2.1/tests/testcruise_evt/2014_185/2014-07-04T00-00-00+00-00.sfl
--rw-r--r--   0 root         (0) root         (0)   960004 2022-02-18 02:29:25.000000 seaflowpy-6.2.1/tests/testcruise_evt/2014_185/2014-07-04T00-00-02+00-00
--rw-r--r--   0 root         (0) root         (0)   467922 2022-02-18 02:29:25.000000 seaflowpy-6.2.1/tests/testcruise_evt/2014_185/2014-07-04T00-03-02+00-00.gz
--rw-r--r--   0 root         (0) root         (0)        0 2022-02-18 02:29:25.000000 seaflowpy-6.2.1/tests/testcruise_evt/2014_185/2014-07-04T00-06-02+00-00
--rw-r--r--   0 root         (0) root         (0)        4 2022-02-18 02:29:25.000000 seaflowpy-6.2.1/tests/testcruise_evt/2014_185/2014-07-04T00-09-02+00-00
--rw-r--r--   0 root         (0) root         (0)        2 2022-02-18 02:29:25.000000 seaflowpy-6.2.1/tests/testcruise_evt/2014_185/2014-07-04T00-12-02+00-00
--rw-r--r--   0 root         (0) root         (0)   289881 2022-02-18 02:29:25.000000 seaflowpy-6.2.1/tests/testcruise_evt/2014_185/2014-07-04T01-15-02+00-00.gz
--rw-r--r--   0 root         (0) root         (0)   467656 2022-02-18 02:29:25.000000 seaflowpy-6.2.1/tests/testcruise_evt/2014_185/2014-07-04T01-17-02+00-00.gz
--rw-r--r--   0 root         (0) root         (0)   960015 2022-02-18 02:29:25.000000 seaflowpy-6.2.1/tests/testcruise_evt/2014_185/2014-07-04T01-21-02+00-00
--rw-r--r--   0 root         (0) root         (0)    90000 2022-02-18 02:29:25.000000 seaflowpy-6.2.1/tests/testcruise_evt/2014_185/2014-07-04T01-27-02+00-00
--rw-r--r--   0 root         (0) root         (0)   960004 2022-02-18 02:29:25.000000 seaflowpy-6.2.1/tests/testcruise_evt/2014_185/2014-07-04T01-30-02+00-00
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:09:20.580244 seaflowpy-6.2.1/tests/testcruise_evt_v2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:09:20.612244 seaflowpy-6.2.1/tests/testcruise_evt_v2/2014_185/
--rw-r--r--   0 root         (0) root         (0)     1468 2022-02-18 02:29:30.000000 seaflowpy-6.2.1/tests/testcruise_evt_v2/2014_185/2014-07-04T00-00-00+00-00.sfl
--rw-r--r--   0 root         (0) root         (0)   560008 2022-02-18 02:29:30.000000 seaflowpy-6.2.1/tests/testcruise_evt_v2/2014_185/2014-07-04T00-00-02+00-00
--rw-r--r--   0 root         (0) root         (0)   367112 2022-02-18 02:29:30.000000 seaflowpy-6.2.1/tests/testcruise_evt_v2/2014_185/2014-07-04T00-03-02+00-00.gz
--rw-r--r--   0 root         (0) root         (0)        0 2022-02-18 02:29:30.000000 seaflowpy-6.2.1/tests/testcruise_evt_v2/2014_185/2014-07-04T00-06-02+00-00
--rw-r--r--   0 root         (0) root         (0)        4 2022-02-18 02:29:30.000000 seaflowpy-6.2.1/tests/testcruise_evt_v2/2014_185/2014-07-04T00-09-02+00-00
--rw-r--r--   0 root         (0) root         (0)        2 2022-02-18 02:29:29.000000 seaflowpy-6.2.1/tests/testcruise_evt_v2/2014_185/2014-07-04T00-12-02+00-00
--rw-r--r--   0 root         (0) root         (0)   217413 2022-02-18 02:29:30.000000 seaflowpy-6.2.1/tests/testcruise_evt_v2/2014_185/2014-07-04T01-15-02+00-00.gz
--rw-r--r--   0 root         (0) root         (0)   366512 2022-02-18 02:29:29.000000 seaflowpy-6.2.1/tests/testcruise_evt_v2/2014_185/2014-07-04T01-17-02+00-00.gz
--rw-r--r--   0 root         (0) root         (0)   560050 2022-02-18 02:29:30.000000 seaflowpy-6.2.1/tests/testcruise_evt_v2/2014_185/2014-07-04T01-21-02+00-00
--rw-r--r--   0 root         (0) root         (0)   559966 2022-02-18 02:29:30.000000 seaflowpy-6.2.1/tests/testcruise_evt_v2/2014_185/2014-07-04T01-27-02+00-00
--rw-r--r--   0 root         (0) root         (0)   560008 2022-02-18 02:29:30.000000 seaflowpy-6.2.1/tests/testcruise_evt_v2/2014_185/2014-07-04T01-30-02+00-00
--rw-r--r--   0 root         (0) root         (0)   110592 2022-02-18 01:48:54.000000 seaflowpy-6.2.1/tests/testcruise_full_one_param.db
--rw-r--r--   0 root         (0) root         (0)   131072 2022-02-18 01:16:58.000000 seaflowpy-6.2.1/tests/testcruise_full_plan.db
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:09:20.613244 seaflowpy-6.2.1/tests/testcruise_opp_one_param/
--rw-r--r--   0 root         (0) root         (0)    27751 2022-02-18 01:52:34.000000 seaflowpy-6.2.1/tests/testcruise_opp_one_param/2014-07-04T00-00-00+00-00.1H.opp.parquet
--rw-r--r--   0 root         (0) root         (0)    16329 2022-02-18 01:52:34.000000 seaflowpy-6.2.1/tests/testcruise_opp_one_param/2014-07-04T01-00-00+00-00.1H.opp.parquet
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 22:09:20.613244 seaflowpy-6.2.1/tests/testcruise_opp_plan/
--rw-r--r--   0 root         (0) root         (0)    26213 2022-02-18 01:18:01.000000 seaflowpy-6.2.1/tests/testcruise_opp_plan/2014-07-04T00-00-00+00-00.1H.opp.parquet
--rw-r--r--   0 root         (0) root         (0)    17096 2022-02-18 01:18:01.000000 seaflowpy-6.2.1/tests/testcruise_opp_plan/2014-07-04T01-00-00+00-00.1H.opp.parquet
--rw-r--r--   0 root         (0) root         (0)   102400 2022-02-18 02:48:34.000000 seaflowpy-6.2.1/tests/testcruise_paramsonly_one_param.db
--rw-r--r--   0 root         (0) root         (0)   102400 2022-02-18 02:47:52.000000 seaflowpy-6.2.1/tests/testcruise_paramsonly_plan.db
--rw-r--r--   0 root         (0) root         (0)    68611 2019-06-01 00:15:35.000000 seaflowpy-6.2.1/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:55:54.083197 seaflowpy-6.3.0/
+-rw-r--r--   0 root         (0) root         (0)    35147 2016-05-27 19:28:44.000000 seaflowpy-6.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      196 2020-07-31 01:20:45.000000 seaflowpy-6.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6771 2023-06-06 19:55:54.083197 seaflowpy-6.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6399 2021-04-02 19:11:59.000000 seaflowpy-6.3.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      245 2023-06-06 19:55:54.085198 seaflowpy-6.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      954 2022-10-27 20:07:07.000000 seaflowpy-6.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:55:54.021197 seaflowpy-6.3.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:55:54.086197 seaflowpy-6.3.0/src/seaflowpy/
+-rw-r--r--   0 root         (0) root         (0)      317 2022-10-26 23:57:59.000000 seaflowpy-6.3.0/src/seaflowpy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-06-06 19:55:54.086197 seaflowpy-6.3.0/src/seaflowpy/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:55:54.041197 seaflowpy-6.3.0/src/seaflowpy/cli/
+-rw-r--r--   0 root         (0) root         (0)       18 2020-03-25 18:47:11.000000 seaflowpy-6.3.0/src/seaflowpy/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      872 2022-08-19 02:08:17.000000 seaflowpy-6.3.0/src/seaflowpy/cli/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:55:54.044197 seaflowpy-6.3.0/src/seaflowpy/cli/commands/
+-rw-r--r--   0 root         (0) root         (0)      192 2022-08-19 02:07:55.000000 seaflowpy-6.3.0/src/seaflowpy/cli/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1025 2020-03-25 18:47:11.000000 seaflowpy-6.3.0/src/seaflowpy/cli/commands/dayofyear_cmd.py
+-rw-r--r--   0 root         (0) root         (0)     5751 2023-06-06 18:39:22.000000 seaflowpy-6.3.0/src/seaflowpy/cli/commands/db_cmd.py
+-rw-r--r--   0 root         (0) root         (0)    12247 2022-10-28 22:17:48.000000 seaflowpy-6.3.0/src/seaflowpy/cli/commands/evt_cmd.py
+-rw-r--r--   0 root         (0) root         (0)     4970 2022-02-21 23:55:50.000000 seaflowpy-6.3.0/src/seaflowpy/cli/commands/filter_cmd.py
+-rw-r--r--   0 root         (0) root         (0)     4876 2022-08-20 19:35:27.000000 seaflowpy-6.3.0/src/seaflowpy/cli/commands/opp_cmd.py
+-rw-r--r--   0 root         (0) root         (0)     3999 2020-03-25 18:47:11.000000 seaflowpy-6.3.0/src/seaflowpy/cli/commands/sds2sfl_cmd.py
+-rw-r--r--   0 root         (0) root         (0)    11035 2022-10-26 19:25:20.000000 seaflowpy-6.3.0/src/seaflowpy/cli/commands/sfl_cmd.py
+-rw-r--r--   0 root         (0) root         (0)      194 2020-03-25 18:47:11.000000 seaflowpy-6.3.0/src/seaflowpy/cli/commands/version_cmd.py
+-rw-r--r--   0 root         (0) root         (0)      889 2022-10-05 00:55:36.000000 seaflowpy-6.3.0/src/seaflowpy/cloud.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:55:54.044197 seaflowpy-6.3.0/src/seaflowpy/data/
+-rw-r--r--   0 root         (0) root         (0)     4882 2022-02-17 23:58:06.000000 seaflowpy-6.3.0/src/seaflowpy/data/popcycle.sql
+-rw-r--r--   0 root         (0) root         (0)    13751 2023-06-06 18:37:53.000000 seaflowpy-6.3.0/src/seaflowpy/db.py
+-rw-r--r--   0 root         (0) root         (0)      405 2022-10-05 00:55:11.000000 seaflowpy-6.3.0/src/seaflowpy/errors.py
+-rw-r--r--   0 root         (0) root         (0)    13696 2022-08-22 23:54:55.000000 seaflowpy-6.3.0/src/seaflowpy/fileio.py
+-rw-r--r--   0 root         (0) root         (0)    13776 2022-04-21 21:40:19.000000 seaflowpy-6.3.0/src/seaflowpy/filterevt.py
+-rw-r--r--   0 root         (0) root         (0)     1802 2020-03-25 18:47:11.000000 seaflowpy-6.3.0/src/seaflowpy/geo.py
+-rw-r--r--   0 root         (0) root         (0)    11203 2022-12-02 21:17:41.000000 seaflowpy-6.3.0/src/seaflowpy/particleops.py
+-rw-r--r--   0 root         (0) root         (0)    10280 2022-10-31 23:12:46.000000 seaflowpy-6.3.0/src/seaflowpy/sample.py
+-rw-r--r--   0 root         (0) root         (0)     9411 2022-08-18 22:28:13.000000 seaflowpy-6.3.0/src/seaflowpy/seaflowfile.py
+-rw-r--r--   0 root         (0) root         (0)    19632 2023-03-09 20:38:00.000000 seaflowpy-6.3.0/src/seaflowpy/sfl.py
+-rw-r--r--   0 root         (0) root         (0)      788 2020-06-11 19:02:16.000000 seaflowpy-6.3.0/src/seaflowpy/time.py
+-rw-r--r--   0 root         (0) root         (0)     3779 2022-10-05 00:08:13.000000 seaflowpy-6.3.0/src/seaflowpy/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:55:54.040197 seaflowpy-6.3.0/src/seaflowpy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6771 2023-06-06 19:55:53.000000 seaflowpy-6.3.0/src/seaflowpy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2961 2023-06-06 19:55:54.000000 seaflowpy-6.3.0/src/seaflowpy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 19:55:53.000000 seaflowpy-6.3.0/src/seaflowpy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-06-06 19:55:53.000000 seaflowpy-6.3.0/src/seaflowpy.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2023-06-06 19:55:53.000000 seaflowpy-6.3.0/src/seaflowpy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-06 19:55:53.000000 seaflowpy-6.3.0/src/seaflowpy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 19:55:53.000000 seaflowpy-6.3.0/src/seaflowpy.egg-info/zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:55:54.050197 seaflowpy-6.3.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     4604 2022-02-18 03:14:13.000000 seaflowpy-6.3.0/tests/file_dates.parquet
+-rw-r--r--   0 root         (0) root         (0)    15333 2020-06-30 22:53:10.000000 seaflowpy-6.3.0/tests/sfl.parquet
+-rw-r--r--   0 root         (0) root         (0)    18822 2022-10-31 23:10:56.000000 seaflowpy-6.3.0/tests/test_evtopp.py
+-rw-r--r--   0 root         (0) root         (0)     3705 2020-06-11 19:02:16.000000 seaflowpy-6.3.0/tests/test_geo.py
+-rw-r--r--   0 root         (0) root         (0)     8000 2022-10-31 23:36:27.000000 seaflowpy-6.3.0/tests/test_sample.py
+-rw-r--r--   0 root         (0) root         (0)    18787 2022-02-18 18:39:19.000000 seaflowpy-6.3.0/tests/test_seaflowfile.py
+-rw-r--r--   0 root         (0) root         (0)     1104 2020-06-11 19:02:16.000000 seaflowpy-6.3.0/tests/test_time.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:55:54.026198 seaflowpy-6.3.0/tests/testcruise_evt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:55:54.064197 seaflowpy-6.3.0/tests/testcruise_evt/2014_185/
+-rw-r--r--   0 root         (0) root         (0)     1468 2022-02-18 02:29:25.000000 seaflowpy-6.3.0/tests/testcruise_evt/2014_185/2014-07-04T00-00-00+00-00.sfl
+-rw-r--r--   0 root         (0) root         (0)   960004 2022-02-18 02:29:25.000000 seaflowpy-6.3.0/tests/testcruise_evt/2014_185/2014-07-04T00-00-02+00-00
+-rw-r--r--   0 root         (0) root         (0)   467922 2022-02-18 02:29:25.000000 seaflowpy-6.3.0/tests/testcruise_evt/2014_185/2014-07-04T00-03-02+00-00.gz
+-rw-r--r--   0 root         (0) root         (0)        0 2022-02-18 02:29:25.000000 seaflowpy-6.3.0/tests/testcruise_evt/2014_185/2014-07-04T00-06-02+00-00
+-rw-r--r--   0 root         (0) root         (0)        4 2022-02-18 02:29:25.000000 seaflowpy-6.3.0/tests/testcruise_evt/2014_185/2014-07-04T00-09-02+00-00
+-rw-r--r--   0 root         (0) root         (0)        2 2022-02-18 02:29:25.000000 seaflowpy-6.3.0/tests/testcruise_evt/2014_185/2014-07-04T00-12-02+00-00
+-rw-r--r--   0 root         (0) root         (0)   289881 2022-02-18 02:29:25.000000 seaflowpy-6.3.0/tests/testcruise_evt/2014_185/2014-07-04T01-15-02+00-00.gz
+-rw-r--r--   0 root         (0) root         (0)   467656 2022-02-18 02:29:25.000000 seaflowpy-6.3.0/tests/testcruise_evt/2014_185/2014-07-04T01-17-02+00-00.gz
+-rw-r--r--   0 root         (0) root         (0)   960015 2022-02-18 02:29:25.000000 seaflowpy-6.3.0/tests/testcruise_evt/2014_185/2014-07-04T01-21-02+00-00
+-rw-r--r--   0 root         (0) root         (0)    90000 2022-02-18 02:29:25.000000 seaflowpy-6.3.0/tests/testcruise_evt/2014_185/2014-07-04T01-27-02+00-00
+-rw-r--r--   0 root         (0) root         (0)   960004 2022-02-18 02:29:25.000000 seaflowpy-6.3.0/tests/testcruise_evt/2014_185/2014-07-04T01-30-02+00-00
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:55:54.027197 seaflowpy-6.3.0/tests/testcruise_evt_v2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:55:54.079198 seaflowpy-6.3.0/tests/testcruise_evt_v2/2014_185/
+-rw-r--r--   0 root         (0) root         (0)     1468 2022-02-18 02:29:30.000000 seaflowpy-6.3.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-00-00+00-00.sfl
+-rw-r--r--   0 root         (0) root         (0)   560008 2022-02-18 02:29:30.000000 seaflowpy-6.3.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-00-02+00-00
+-rw-r--r--   0 root         (0) root         (0)   367112 2022-02-18 02:29:30.000000 seaflowpy-6.3.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-03-02+00-00.gz
+-rw-r--r--   0 root         (0) root         (0)        0 2022-02-18 02:29:30.000000 seaflowpy-6.3.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-06-02+00-00
+-rw-r--r--   0 root         (0) root         (0)        4 2022-02-18 02:29:30.000000 seaflowpy-6.3.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-09-02+00-00
+-rw-r--r--   0 root         (0) root         (0)        2 2022-02-18 02:29:29.000000 seaflowpy-6.3.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-12-02+00-00
+-rw-r--r--   0 root         (0) root         (0)   217413 2022-02-18 02:29:30.000000 seaflowpy-6.3.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-15-02+00-00.gz
+-rw-r--r--   0 root         (0) root         (0)   366512 2022-02-18 02:29:29.000000 seaflowpy-6.3.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-17-02+00-00.gz
+-rw-r--r--   0 root         (0) root         (0)   560050 2022-02-18 02:29:30.000000 seaflowpy-6.3.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-21-02+00-00
+-rw-r--r--   0 root         (0) root         (0)   559966 2022-02-18 02:29:30.000000 seaflowpy-6.3.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-27-02+00-00
+-rw-r--r--   0 root         (0) root         (0)   560008 2022-02-18 02:29:30.000000 seaflowpy-6.3.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-30-02+00-00
+-rw-r--r--   0 root         (0) root         (0)   110592 2022-02-18 01:48:54.000000 seaflowpy-6.3.0/tests/testcruise_full_one_param.db
+-rw-r--r--   0 root         (0) root         (0)   131072 2022-02-18 01:16:58.000000 seaflowpy-6.3.0/tests/testcruise_full_plan.db
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:55:54.082198 seaflowpy-6.3.0/tests/testcruise_opp_one_param/
+-rw-r--r--   0 root         (0) root         (0)    27751 2022-02-18 01:52:34.000000 seaflowpy-6.3.0/tests/testcruise_opp_one_param/2014-07-04T00-00-00+00-00.1H.opp.parquet
+-rw-r--r--   0 root         (0) root         (0)    16329 2022-02-18 01:52:34.000000 seaflowpy-6.3.0/tests/testcruise_opp_one_param/2014-07-04T01-00-00+00-00.1H.opp.parquet
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:55:54.082198 seaflowpy-6.3.0/tests/testcruise_opp_plan/
+-rw-r--r--   0 root         (0) root         (0)    26213 2022-02-18 01:18:01.000000 seaflowpy-6.3.0/tests/testcruise_opp_plan/2014-07-04T00-00-00+00-00.1H.opp.parquet
+-rw-r--r--   0 root         (0) root         (0)    17096 2022-02-18 01:18:01.000000 seaflowpy-6.3.0/tests/testcruise_opp_plan/2014-07-04T01-00-00+00-00.1H.opp.parquet
+-rw-r--r--   0 root         (0) root         (0)   102400 2022-02-18 02:48:34.000000 seaflowpy-6.3.0/tests/testcruise_paramsonly_one_param.db
+-rw-r--r--   0 root         (0) root         (0)   102400 2022-02-18 02:47:52.000000 seaflowpy-6.3.0/tests/testcruise_paramsonly_plan.db
+-rw-r--r--   0 root         (0) root         (0)    68611 2019-06-01 00:15:35.000000 seaflowpy-6.3.0/versioneer.py
```

### Comparing `seaflowpy-6.2.1/LICENSE` & `seaflowpy-6.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/PKG-INFO` & `seaflowpy-6.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seaflowpy
-Version: 6.2.1
+Version: 6.3.0
 Summary: A Python library for SeaFlow data.
 Home-page: https://github.com/armbrustlab/seaflowpy
 Author: Chris T. Berthiaume
 Author-email: chrisbee@uw.edu
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.7.1
 Description-Content-Type: text/markdown
```

### Comparing `seaflowpy-6.2.1/README.md` & `seaflowpy-6.3.0/README.md`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/setup.py` & `seaflowpy-6.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/src/seaflowpy/cli/cli.py` & `seaflowpy-6.3.0/src/seaflowpy/cli/cli.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/src/seaflowpy/cli/commands/dayofyear_cmd.py` & `seaflowpy-6.3.0/src/seaflowpy/cli/commands/dayofyear_cmd.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/src/seaflowpy/cli/commands/db_cmd.py` & `seaflowpy-6.3.0/src/seaflowpy/cli/commands/db_cmd.py`

 * *Files 7% similar despite different names*

```diff
@@ -132,14 +132,27 @@
     df = fileio.read_filter_params_csv(filter_file)
     params = df[df.cruise == cruise]
     if len(params.index) == 0:
         raise click.ClickException('no filter parameters found for cruise %s' % cruise)
     db.save_filter_params(db_file, params.to_dict('index').values())
 
 
+@db_cmd.command('create-filter-plan')
+@click.argument('db-file', nargs=1, type=click.Path(writable=True))
+def db_create_filter_plan_cmd(db_file):
+    """
+    Create a filter plan table if sfl and filter tables are populated.
+    """
+    try:
+        filter_plan_df = db.create_filter_plan(db_file)
+    except SeaFlowpyError as e:
+        raise click.ClickException(e)
+    print("Saved a new filter plan")
+    print(filter_plan_df.to_string(index=False))
+
 @db_cmd.command('merge')
 @click.argument('db1', type=click.Path(exists=True))
 @click.argument('db2', type=click.Path(exists=True, writable=True))
 def db_merge_cmd(db1, db2):
     """Merges SQLite3 DB1 into DB2.
 
     Only merges gating, poly, filter tables.
```

### Comparing `seaflowpy-6.2.1/src/seaflowpy/cli/commands/evt_cmd.py` & `seaflowpy-6.3.0/src/seaflowpy/cli/commands/evt_cmd.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/src/seaflowpy/cli/commands/filter_cmd.py` & `seaflowpy-6.3.0/src/seaflowpy/cli/commands/filter_cmd.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/src/seaflowpy/cli/commands/opp_cmd.py` & `seaflowpy-6.3.0/src/seaflowpy/cli/commands/opp_cmd.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/src/seaflowpy/cli/commands/sds2sfl_cmd.py` & `seaflowpy-6.3.0/src/seaflowpy/cli/commands/sds2sfl_cmd.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/src/seaflowpy/cli/commands/sfl_cmd.py` & `seaflowpy-6.3.0/src/seaflowpy/cli/commands/sfl_cmd.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/src/seaflowpy/cloud.py` & `seaflowpy-6.3.0/src/seaflowpy/cloud.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/src/seaflowpy/data/popcycle.sql` & `seaflowpy-6.3.0/src/seaflowpy/data/popcycle.sql`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/src/seaflowpy/db.py` & `seaflowpy-6.3.0/src/seaflowpy/db.py`

 * *Files 16% similar despite different names*

```diff
@@ -216,14 +216,21 @@
 def get_filter_table(dbpath):
     sql = "SELECT * FROM filter ORDER BY date ASC, quantile ASC"
     with sqlite3.connect(dbpath) as dbcon:
         filterdf = safe_read_sql(sql, dbcon)
     return filterdf
 
 
+def get_filter_plan_table(dbpath):
+    sql = "SELECT * FROM filter_plan"
+    with sqlite3.connect(dbpath) as dbcon:
+        df = safe_read_sql(sql, dbcon)
+    return df
+
+
 def get_serial(dbpath):
     sql = "SELECT inst FROM metadata"
     with sqlite3.connect(dbpath) as dbcon:
         df = safe_read_sql(sql, dbcon)
     if len(df.index) > 1:
         insts = ", ".join([str(c) for c in df.inst.tolist()])
         raise errors.SeaFlowpyError("More than one instrument serial found in database {}: {}".format(dbpath, insts))
@@ -310,14 +317,51 @@
             polydf.to_sql('poly', con2, if_exists='append', index=False)
             filterdf.to_sql('filter', con2, if_exists='append', index=False)
     # Merge opp
     # Merge vct
     # Merge meta
 
 
+def create_filter_plan(dbpath):
+    """
+    Create a filter plan table.
+
+    Only run for the simple case where sfl and filter tables are populated and
+    there is only one set of filter parameters.
+
+    Raise SeaFlowpyError if filter or sfl tables are empty, if more than one set
+    of filter parameters exists in the database, if a filter plan already
+    exists, or for database save errors.
+
+    Return a dataframe of the filter plan.
+    """
+    filter_df = get_filter_table(dbpath)
+    sfl_df = get_sfl_table(dbpath)
+    cur_filter_plan_df = get_filter_plan_table(dbpath)
+    if len(filter_df) == 0:
+        raise errors.SeaFlowpyError("no filter parameters found in db")
+    if len(filter_df["id"].unique()) > 1:
+        raise errors.SeaFlowpyError("more than one filter parameter found in db")
+    if len(sfl_df) == 0:
+        raise errors.SeaFlowpyError("no sfl data found in db")
+    if len(cur_filter_plan_df) > 0:
+        raise errors.SeaFlowpyError("a filter plan already exists in db")
+    filter_plan_df = pd.DataFrame({
+        "start_date": [sfl_df.sort_values(by="date").loc[0, "date"]],
+        "filter_id": [filter_df.loc[0, "id"]]
+    })
+    try:
+        with sqlite3.connect(dbpath) as con:
+            df_sql_insert(filter_plan_df, "filter_plan", con)
+    except sqlite3.Error as e:
+        raise errors.SeaFlowpyError("An error occurred when saving a filter plan: {!s}".format(e))
+
+    return filter_plan_df
+
+
 def execute(dbpath, sql, timeout=120):
     con = sqlite3.connect(dbpath, timeout=timeout)
     try:
         with con:
             con.execute(sql)
     except sqlite3.Error as e:
         raise errors.SeaFlowpyError("An error occurred when executing SQL queries: {!s}".format(e))
@@ -352,7 +396,15 @@
         df = pd.read_sql(sql, con)
         errmsg = ''
     except pd.io.sql.DatabaseError as e:
         errmsg = str(e)
     if errmsg:
         raise errors.SeaFlowpyError(errmsg)
     return df
+
+
+def df_sql_insert(df: pd.DataFrame, table: str, con: sqlite3.Connection):
+    """Insert from df into SQL table without replacing the table schema"""
+    values_str = ", ".join([":" + f for f in df.columns])
+    sql_insert = f"INSERT OR REPLACE INTO {table} VALUES ({values_str})"
+    values = df.to_dict("index").values()
+    con.executemany(sql_insert, values)
```

### Comparing `seaflowpy-6.2.1/src/seaflowpy/fileio.py` & `seaflowpy-6.3.0/src/seaflowpy/fileio.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/src/seaflowpy/filterevt.py` & `seaflowpy-6.3.0/src/seaflowpy/filterevt.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/src/seaflowpy/geo.py` & `seaflowpy-6.3.0/src/seaflowpy/geo.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/src/seaflowpy/particleops.py` & `seaflowpy-6.3.0/src/seaflowpy/particleops.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/src/seaflowpy/sample.py` & `seaflowpy-6.3.0/src/seaflowpy/sample.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/src/seaflowpy/seaflowfile.py` & `seaflowpy-6.3.0/src/seaflowpy/seaflowfile.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/src/seaflowpy/sfl.py` & `seaflowpy-6.3.0/src/seaflowpy/sfl.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/src/seaflowpy/time.py` & `seaflowpy-6.3.0/src/seaflowpy/time.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/src/seaflowpy/util.py` & `seaflowpy-6.3.0/src/seaflowpy/util.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/src/seaflowpy.egg-info/PKG-INFO` & `seaflowpy-6.3.0/src/seaflowpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seaflowpy
-Version: 6.2.1
+Version: 6.3.0
 Summary: A Python library for SeaFlow data.
 Home-page: https://github.com/armbrustlab/seaflowpy
 Author: Chris T. Berthiaume
 Author-email: chrisbee@uw.edu
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.7.1
 Description-Content-Type: text/markdown
```

### Comparing `seaflowpy-6.2.1/src/seaflowpy.egg-info/SOURCES.txt` & `seaflowpy-6.3.0/src/seaflowpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/tests/file_dates.parquet` & `seaflowpy-6.3.0/tests/file_dates.parquet`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/tests/sfl.parquet` & `seaflowpy-6.3.0/tests/sfl.parquet`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/tests/test_evtopp.py` & `seaflowpy-6.3.0/tests/test_evtopp.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/tests/test_geo.py` & `seaflowpy-6.3.0/tests/test_geo.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/tests/test_sample.py` & `seaflowpy-6.3.0/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/tests/test_seaflowfile.py` & `seaflowpy-6.3.0/tests/test_seaflowfile.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/tests/test_time.py` & `seaflowpy-6.3.0/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/tests/testcruise_evt/2014_185/2014-07-04T00-00-00+00-00.sfl` & `seaflowpy-6.3.0/tests/testcruise_evt/2014_185/2014-07-04T00-00-00+00-00.sfl`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/tests/testcruise_evt/2014_185/2014-07-04T00-00-02+00-00` & `seaflowpy-6.3.0/tests/testcruise_evt/2014_185/2014-07-04T00-00-02+00-00`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/tests/testcruise_evt/2014_185/2014-07-04T00-03-02+00-00.gz` & `seaflowpy-6.3.0/tests/testcruise_evt/2014_185/2014-07-04T00-03-02+00-00.gz`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/tests/testcruise_evt/2014_185/2014-07-04T01-15-02+00-00.gz` & `seaflowpy-6.3.0/tests/testcruise_evt/2014_185/2014-07-04T01-15-02+00-00.gz`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/tests/testcruise_evt/2014_185/2014-07-04T01-17-02+00-00.gz` & `seaflowpy-6.3.0/tests/testcruise_evt/2014_185/2014-07-04T01-17-02+00-00.gz`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/tests/testcruise_evt/2014_185/2014-07-04T01-21-02+00-00` & `seaflowpy-6.3.0/tests/testcruise_evt/2014_185/2014-07-04T01-21-02+00-00`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/tests/testcruise_evt/2014_185/2014-07-04T01-27-02+00-00` & `seaflowpy-6.3.0/tests/testcruise_evt/2014_185/2014-07-04T01-27-02+00-00`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/tests/testcruise_evt/2014_185/2014-07-04T01-30-02+00-00` & `seaflowpy-6.3.0/tests/testcruise_evt/2014_185/2014-07-04T01-30-02+00-00`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/tests/testcruise_evt_v2/2014_185/2014-07-04T00-00-00+00-00.sfl` & `seaflowpy-6.3.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-00-00+00-00.sfl`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/tests/testcruise_evt_v2/2014_185/2014-07-04T00-00-02+00-00` & `seaflowpy-6.3.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-00-02+00-00`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/tests/testcruise_evt_v2/2014_185/2014-07-04T00-03-02+00-00.gz` & `seaflowpy-6.3.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-03-02+00-00.gz`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/tests/testcruise_evt_v2/2014_185/2014-07-04T01-15-02+00-00.gz` & `seaflowpy-6.3.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-15-02+00-00.gz`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/tests/testcruise_evt_v2/2014_185/2014-07-04T01-17-02+00-00.gz` & `seaflowpy-6.3.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-17-02+00-00.gz`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/tests/testcruise_evt_v2/2014_185/2014-07-04T01-21-02+00-00` & `seaflowpy-6.3.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-21-02+00-00`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/tests/testcruise_evt_v2/2014_185/2014-07-04T01-27-02+00-00` & `seaflowpy-6.3.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-27-02+00-00`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/tests/testcruise_evt_v2/2014_185/2014-07-04T01-30-02+00-00` & `seaflowpy-6.3.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-30-02+00-00`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/tests/testcruise_full_one_param.db` & `seaflowpy-6.3.0/tests/testcruise_full_one_param.db`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/tests/testcruise_full_plan.db` & `seaflowpy-6.3.0/tests/testcruise_full_plan.db`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/tests/testcruise_opp_one_param/2014-07-04T00-00-00+00-00.1H.opp.parquet` & `seaflowpy-6.3.0/tests/testcruise_opp_one_param/2014-07-04T00-00-00+00-00.1H.opp.parquet`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/tests/testcruise_opp_one_param/2014-07-04T01-00-00+00-00.1H.opp.parquet` & `seaflowpy-6.3.0/tests/testcruise_opp_one_param/2014-07-04T01-00-00+00-00.1H.opp.parquet`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/tests/testcruise_opp_plan/2014-07-04T00-00-00+00-00.1H.opp.parquet` & `seaflowpy-6.3.0/tests/testcruise_opp_plan/2014-07-04T00-00-00+00-00.1H.opp.parquet`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/tests/testcruise_opp_plan/2014-07-04T01-00-00+00-00.1H.opp.parquet` & `seaflowpy-6.3.0/tests/testcruise_opp_plan/2014-07-04T01-00-00+00-00.1H.opp.parquet`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/tests/testcruise_paramsonly_one_param.db` & `seaflowpy-6.3.0/tests/testcruise_paramsonly_one_param.db`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/tests/testcruise_paramsonly_plan.db` & `seaflowpy-6.3.0/tests/testcruise_paramsonly_plan.db`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.2.1/versioneer.py` & `seaflowpy-6.3.0/versioneer.py`

 * *Files identical despite different names*

