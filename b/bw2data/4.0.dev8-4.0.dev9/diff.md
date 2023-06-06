# Comparing `tmp/bw2data-4.0.dev8.tar.gz` & `tmp/bw2data-4.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw2data-4.0.dev8.tar", last modified: Tue Oct 19 21:14:13 2021, max compression
+gzip compressed data, was "bw2data-4.0.dev9.tar", last modified: Sat Oct 23 12:32:23 2021, max compression
```

## Comparing `bw2data-4.0.dev8.tar` & `bw2data-4.0.dev9.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2021-10-19 21:14:13.344730 bw2data-4.0.dev8/
--rw-r--r--   0 cmutel     (501) staff       (20)     1474 2021-05-06 13:38:14.000000 bw2data-4.0.dev8/LICENSE.txt
--rw-r--r--   0 cmutel     (501) staff       (20)      165 2021-05-06 13:38:14.000000 bw2data-4.0.dev8/MANIFEST.in
--rw-r--r--   0 cmutel     (501) staff       (20)     2214 2021-10-19 21:14:13.344270 bw2data-4.0.dev8/PKG-INFO
--rw-r--r--   0 cmutel     (501) staff       (20)      814 2021-05-16 11:23:49.000000 bw2data-4.0.dev8/README.rst
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2021-10-19 21:14:13.310647 bw2data-4.0.dev8/bw2data/
--rw-r--r--   0 cmutel     (501) staff       (20)     1771 2021-10-13 19:57:39.000000 bw2data-4.0.dev8/bw2data/__init__.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2021-10-19 21:14:13.317527 bw2data-4.0.dev8/bw2data/backends/
--rw-r--r--   0 cmutel     (501) staff       (20)      552 2021-10-13 19:56:22.000000 bw2data-4.0.dev8/bw2data/backends/__init__.py
--rw-r--r--   0 cmutel     (501) staff       (20)    29940 2021-10-13 19:56:25.000000 bw2data-4.0.dev8/bw2data/backends/base.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2021-10-19 21:14:13.318117 bw2data-4.0.dev8/bw2data/backends/iotable/
--rw-r--r--   0 cmutel     (501) staff       (20)     3727 2021-10-13 19:56:22.000000 bw2data-4.0.dev8/bw2data/backends/iotable/__init__.py
--rw-r--r--   0 cmutel     (501) staff       (20)    11776 2021-10-13 19:56:23.000000 bw2data-4.0.dev8/bw2data/backends/proxies.py
--rw-r--r--   0 cmutel     (501) staff       (20)     1197 2021-10-19 21:10:51.000000 bw2data-4.0.dev8/bw2data/backends/schema.py
--rw-r--r--   0 cmutel     (501) staff       (20)     3729 2021-10-13 19:56:00.000000 bw2data-4.0.dev8/bw2data/backends/utils.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2021-10-19 21:14:13.319300 bw2data-4.0.dev8/bw2data/bin/
--rw-r--r--   0 cmutel     (501) staff       (20)        0 2020-03-26 16:27:18.000000 bw2data-4.0.dev8/bw2data/bin/__init__.py
--rw-r--r--   0 cmutel     (501) staff       (20)     1868 2021-10-13 19:56:00.000000 bw2data-4.0.dev8/bw2data/bin/bw2_uptodate.py
--rw-r--r--   0 cmutel     (501) staff       (20)     4218 2021-10-17 20:03:21.000000 bw2data-4.0.dev8/bw2data/compat.py
--rw-r--r--   0 cmutel     (501) staff       (20)      781 2021-10-13 19:31:02.000000 bw2data-4.0.dev8/bw2data/configuration.py
--rw-r--r--   0 cmutel     (501) staff       (20)     7182 2021-10-13 19:56:23.000000 bw2data-4.0.dev8/bw2data/data_store.py
--rw-r--r--   0 cmutel     (501) staff       (20)      724 2021-05-06 13:38:14.000000 bw2data-4.0.dev8/bw2data/database.py
--rw-r--r--   0 cmutel     (501) staff       (20)     1214 2021-05-18 07:21:52.000000 bw2data-4.0.dev8/bw2data/errors.py
--rw-r--r--   0 cmutel     (501) staff       (20)     5529 2021-10-13 19:55:59.000000 bw2data-4.0.dev8/bw2data/fatomic.py
--rw-r--r--   0 cmutel     (501) staff       (20)      722 2021-05-06 13:38:14.000000 bw2data-4.0.dev8/bw2data/filesystem.py
--rw-r--r--   0 cmutel     (501) staff       (20)     3862 2021-10-13 19:56:23.000000 bw2data-4.0.dev8/bw2data/ia_data_store.py
--rw-r--r--   0 cmutel     (501) staff       (20)     2911 2021-10-13 19:56:23.000000 bw2data-4.0.dev8/bw2data/logs.py
--rw-r--r--   0 cmutel     (501) staff       (20)     5043 2021-10-13 19:56:00.000000 bw2data-4.0.dev8/bw2data/meta.py
--rw-r--r--   0 cmutel     (501) staff       (20)     2666 2021-10-13 19:56:00.000000 bw2data-4.0.dev8/bw2data/method.py
--rw-r--r--   0 cmutel     (501) staff       (20)    59183 2021-10-13 19:56:28.000000 bw2data-4.0.dev8/bw2data/parameters.py
--rw-r--r--   0 cmutel     (501) staff       (20)    15811 2021-10-13 19:56:25.000000 bw2data-4.0.dev8/bw2data/project.py
--rw-r--r--   0 cmutel     (501) staff       (20)     8486 2021-10-13 19:55:59.000000 bw2data-4.0.dev8/bw2data/proxies.py
--rw-r--r--   0 cmutel     (501) staff       (20)     5845 2021-10-13 19:55:59.000000 bw2data-4.0.dev8/bw2data/query.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2021-10-19 21:14:13.324828 bw2data-4.0.dev8/bw2data/search/
--rw-r--r--   0 cmutel     (501) staff       (20)       63 2021-05-06 13:38:14.000000 bw2data-4.0.dev8/bw2data/search/__init__.py
--rw-r--r--   0 cmutel     (501) staff       (20)     1762 2021-10-13 19:56:00.000000 bw2data-4.0.dev8/bw2data/search/indices.py
--rw-r--r--   0 cmutel     (501) staff       (20)      371 2021-10-13 19:56:00.000000 bw2data-4.0.dev8/bw2data/search/schema.py
--rw-r--r--   0 cmutel     (501) staff       (20)     3387 2021-10-13 19:56:00.000000 bw2data-4.0.dev8/bw2data/search/search.py
--rw-r--r--   0 cmutel     (501) staff       (20)     7519 2021-10-13 19:56:00.000000 bw2data-4.0.dev8/bw2data/serialization.py
--rw-r--r--   0 cmutel     (501) staff       (20)     1245 2021-10-13 19:55:59.000000 bw2data-4.0.dev8/bw2data/sqlite.py
--rw-r--r--   0 cmutel     (501) staff       (20)     1215 2021-10-13 19:56:00.000000 bw2data-4.0.dev8/bw2data/tests.py
--rw-r--r--   0 cmutel     (501) staff       (20)     8151 2021-10-14 07:32:42.000000 bw2data-4.0.dev8/bw2data/updates.py
--rw-r--r--   0 cmutel     (501) staff       (20)    13276 2021-10-13 19:56:26.000000 bw2data-4.0.dev8/bw2data/utils.py
--rw-r--r--   0 cmutel     (501) staff       (20)     1538 2021-10-13 19:55:59.000000 bw2data-4.0.dev8/bw2data/validate.py
--rw-r--r--   0 cmutel     (501) staff       (20)       25 2021-10-19 21:13:14.000000 bw2data-4.0.dev8/bw2data/version.py
--rw-r--r--   0 cmutel     (501) staff       (20)     2149 2021-10-13 19:55:59.000000 bw2data-4.0.dev8/bw2data/weighting_normalization.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2021-10-19 21:14:13.314022 bw2data-4.0.dev8/bw2data.egg-info/
--rw-r--r--   0 cmutel     (501) staff       (20)     2214 2021-10-19 21:14:12.000000 bw2data-4.0.dev8/bw2data.egg-info/PKG-INFO
--rw-r--r--   0 cmutel     (501) staff       (20)     1492 2021-10-19 21:14:12.000000 bw2data-4.0.dev8/bw2data.egg-info/SOURCES.txt
--rw-r--r--   0 cmutel     (501) staff       (20)        1 2021-10-19 21:14:12.000000 bw2data-4.0.dev8/bw2data.egg-info/dependency_links.txt
--rw-r--r--   0 cmutel     (501) staff       (20)       64 2021-10-19 21:14:12.000000 bw2data-4.0.dev8/bw2data.egg-info/entry_points.txt
--rw-r--r--   0 cmutel     (501) staff       (20)      152 2021-10-19 21:14:12.000000 bw2data-4.0.dev8/bw2data.egg-info/requires.txt
--rw-r--r--   0 cmutel     (501) staff       (20)        8 2021-10-19 21:14:12.000000 bw2data-4.0.dev8/bw2data.egg-info/top_level.txt
--rw-r--r--   0 cmutel     (501) staff       (20)       35 2021-05-06 13:38:14.000000 bw2data-4.0.dev8/pytest.ini
--rw-r--r--   0 cmutel     (501) staff       (20)      189 2021-10-19 21:11:54.000000 bw2data-4.0.dev8/requirements-test.txt
--rw-r--r--   0 cmutel     (501) staff       (20)      152 2021-10-02 06:17:57.000000 bw2data-4.0.dev8/requirements.txt
--rw-r--r--   0 cmutel     (501) staff       (20)       38 2021-10-19 21:14:13.344822 bw2data-4.0.dev8/setup.cfg
--rw-r--r--   0 cmutel     (501) staff       (20)     2423 2021-05-19 17:56:41.000000 bw2data-4.0.dev8/setup.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2021-10-19 21:14:13.343497 bw2data-4.0.dev8/tests/
--rw-r--r--   0 cmutel     (501) staff       (20)        0 2021-05-06 13:38:14.000000 bw2data-4.0.dev8/tests/__init__.py
--rw-r--r--   0 cmutel     (501) staff       (20)     6426 2021-10-13 19:56:32.000000 bw2data-4.0.dev8/tests/activity_proxy.py
--rw-r--r--   0 cmutel     (501) staff       (20)      326 2021-10-13 19:56:16.000000 bw2data-4.0.dev8/tests/base.py
--rw-r--r--   0 cmutel     (501) staff       (20)      633 2021-10-13 19:56:16.000000 bw2data-4.0.dev8/tests/compatibility.py
--rw-r--r--   0 cmutel     (501) staff       (20)      224 2021-10-13 19:56:16.000000 bw2data-4.0.dev8/tests/config.py
--rw-r--r--   0 cmutel     (501) staff       (20)     2135 2021-10-13 19:56:15.000000 bw2data-4.0.dev8/tests/data_store.py
--rw-r--r--   0 cmutel     (501) staff       (20)    21583 2021-10-19 21:11:28.000000 bw2data-4.0.dev8/tests/database.py
--rw-r--r--   0 cmutel     (501) staff       (20)     6384 2021-10-13 19:56:16.000000 bw2data-4.0.dev8/tests/database_querying.py
--rw-r--r--   0 cmutel     (501) staff       (20)    10222 2021-10-13 19:56:32.000000 bw2data-4.0.dev8/tests/exchange_proxy.py
--rw-r--r--   0 cmutel     (501) staff       (20)     2964 2021-10-13 19:56:16.000000 bw2data-4.0.dev8/tests/fixtures.py
--rw-r--r--   0 cmutel     (501) staff       (20)     2450 2021-10-13 19:56:16.000000 bw2data-4.0.dev8/tests/geo.py
--rw-r--r--   0 cmutel     (501) staff       (20)     6000 2021-10-13 19:56:16.000000 bw2data-4.0.dev8/tests/ia.py
--rw-r--r--   0 cmutel     (501) staff       (20)    24447 2021-05-06 13:38:14.000000 bw2data-4.0.dev8/tests/naughty_strings.txt
--rw-r--r--   0 cmutel     (501) staff       (20)    61920 2021-10-13 19:56:36.000000 bw2data-4.0.dev8/tests/parameters.py
--rw-r--r--   0 cmutel     (501) staff       (20)     7969 2021-10-13 19:56:16.000000 bw2data-4.0.dev8/tests/projects.py
--rw-r--r--   0 cmutel     (501) staff       (20)     9889 2021-10-13 19:56:33.000000 bw2data-4.0.dev8/tests/search.py
--rw-r--r--   0 cmutel     (501) staff       (20)     1280 2021-10-13 19:56:16.000000 bw2data-4.0.dev8/tests/serialization.py
--rw-r--r--   0 cmutel     (501) staff       (20)      959 2021-10-13 19:56:16.000000 bw2data-4.0.dev8/tests/sqlite.py
--rw-r--r--   0 cmutel     (501) staff       (20)      605 2021-10-13 19:56:16.000000 bw2data-4.0.dev8/tests/updates.py
--rw-r--r--   0 cmutel     (501) staff       (20)     9880 2021-10-13 19:56:33.000000 bw2data-4.0.dev8/tests/utils.py
--rw-r--r--   0 cmutel     (501) staff       (20)     3824 2021-10-13 19:56:34.000000 bw2data-4.0.dev8/tests/validation.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2021-10-23 12:32:23.778156 bw2data-4.0.dev9/
+-rw-r--r--   0 cmutel     (501) staff       (20)     1474 2021-05-06 13:38:14.000000 bw2data-4.0.dev9/LICENSE.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)      165 2021-05-06 13:38:14.000000 bw2data-4.0.dev9/MANIFEST.in
+-rw-r--r--   0 cmutel     (501) staff       (20)     2214 2021-10-23 12:32:23.776161 bw2data-4.0.dev9/PKG-INFO
+-rw-r--r--   0 cmutel     (501) staff       (20)      814 2021-05-16 11:23:49.000000 bw2data-4.0.dev9/README.rst
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2021-10-23 12:32:23.690386 bw2data-4.0.dev9/bw2data/
+-rw-r--r--   0 cmutel     (501) staff       (20)     1771 2021-10-13 19:57:39.000000 bw2data-4.0.dev9/bw2data/__init__.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2021-10-23 12:32:23.709573 bw2data-4.0.dev9/bw2data/backends/
+-rw-r--r--   0 cmutel     (501) staff       (20)      552 2021-10-13 19:56:22.000000 bw2data-4.0.dev9/bw2data/backends/__init__.py
+-rw-r--r--   0 cmutel     (501) staff       (20)    31309 2021-10-23 11:07:49.000000 bw2data-4.0.dev9/bw2data/backends/base.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2021-10-23 12:32:23.710692 bw2data-4.0.dev9/bw2data/backends/iotable/
+-rw-r--r--   0 cmutel     (501) staff       (20)     3727 2021-10-13 19:56:22.000000 bw2data-4.0.dev9/bw2data/backends/iotable/__init__.py
+-rw-r--r--   0 cmutel     (501) staff       (20)    11776 2021-10-13 19:56:23.000000 bw2data-4.0.dev9/bw2data/backends/proxies.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     1197 2021-10-19 21:10:51.000000 bw2data-4.0.dev9/bw2data/backends/schema.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     3729 2021-10-13 19:56:00.000000 bw2data-4.0.dev9/bw2data/backends/utils.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2021-10-23 12:32:23.712195 bw2data-4.0.dev9/bw2data/bin/
+-rw-r--r--   0 cmutel     (501) staff       (20)        0 2020-03-26 16:27:18.000000 bw2data-4.0.dev9/bw2data/bin/__init__.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     1868 2021-10-13 19:56:00.000000 bw2data-4.0.dev9/bw2data/bin/bw2_uptodate.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     4218 2021-10-17 20:03:21.000000 bw2data-4.0.dev9/bw2data/compat.py
+-rw-r--r--   0 cmutel     (501) staff       (20)      781 2021-10-13 19:31:02.000000 bw2data-4.0.dev9/bw2data/configuration.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     7182 2021-10-13 19:56:23.000000 bw2data-4.0.dev9/bw2data/data_store.py
+-rw-r--r--   0 cmutel     (501) staff       (20)      724 2021-05-06 13:38:14.000000 bw2data-4.0.dev9/bw2data/database.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     1214 2021-05-18 07:21:52.000000 bw2data-4.0.dev9/bw2data/errors.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     5529 2021-10-13 19:55:59.000000 bw2data-4.0.dev9/bw2data/fatomic.py
+-rw-r--r--   0 cmutel     (501) staff       (20)      722 2021-05-06 13:38:14.000000 bw2data-4.0.dev9/bw2data/filesystem.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     3862 2021-10-13 19:56:23.000000 bw2data-4.0.dev9/bw2data/ia_data_store.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     2911 2021-10-13 19:56:23.000000 bw2data-4.0.dev9/bw2data/logs.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     5043 2021-10-13 19:56:00.000000 bw2data-4.0.dev9/bw2data/meta.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     3107 2021-10-23 11:15:41.000000 bw2data-4.0.dev9/bw2data/method.py
+-rw-r--r--   0 cmutel     (501) staff       (20)    59183 2021-10-13 19:56:28.000000 bw2data-4.0.dev9/bw2data/parameters.py
+-rw-r--r--   0 cmutel     (501) staff       (20)    15811 2021-10-13 19:56:25.000000 bw2data-4.0.dev9/bw2data/project.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     8486 2021-10-13 19:55:59.000000 bw2data-4.0.dev9/bw2data/proxies.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     5845 2021-10-13 19:55:59.000000 bw2data-4.0.dev9/bw2data/query.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2021-10-23 12:32:23.724354 bw2data-4.0.dev9/bw2data/search/
+-rw-r--r--   0 cmutel     (501) staff       (20)       63 2021-05-06 13:38:14.000000 bw2data-4.0.dev9/bw2data/search/__init__.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     1762 2021-10-13 19:56:00.000000 bw2data-4.0.dev9/bw2data/search/indices.py
+-rw-r--r--   0 cmutel     (501) staff       (20)      371 2021-10-13 19:56:00.000000 bw2data-4.0.dev9/bw2data/search/schema.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     3387 2021-10-13 19:56:00.000000 bw2data-4.0.dev9/bw2data/search/search.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     7519 2021-10-13 19:56:00.000000 bw2data-4.0.dev9/bw2data/serialization.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     1245 2021-10-13 19:55:59.000000 bw2data-4.0.dev9/bw2data/sqlite.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     1215 2021-10-13 19:56:00.000000 bw2data-4.0.dev9/bw2data/tests.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     8151 2021-10-14 07:32:42.000000 bw2data-4.0.dev9/bw2data/updates.py
+-rw-r--r--   0 cmutel     (501) staff       (20)    13834 2021-10-23 11:10:25.000000 bw2data-4.0.dev9/bw2data/utils.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     1538 2021-10-13 19:55:59.000000 bw2data-4.0.dev9/bw2data/validate.py
+-rw-r--r--   0 cmutel     (501) staff       (20)       25 2021-10-23 11:28:13.000000 bw2data-4.0.dev9/bw2data/version.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     2149 2021-10-13 19:55:59.000000 bw2data-4.0.dev9/bw2data/weighting_normalization.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2021-10-23 12:32:23.693874 bw2data-4.0.dev9/bw2data.egg-info/
+-rw-r--r--   0 cmutel     (501) staff       (20)     2214 2021-10-23 12:32:22.000000 bw2data-4.0.dev9/bw2data.egg-info/PKG-INFO
+-rw-r--r--   0 cmutel     (501) staff       (20)     1492 2021-10-23 12:32:23.000000 bw2data-4.0.dev9/bw2data.egg-info/SOURCES.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)        1 2021-10-23 12:32:22.000000 bw2data-4.0.dev9/bw2data.egg-info/dependency_links.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)       64 2021-10-23 12:32:22.000000 bw2data-4.0.dev9/bw2data.egg-info/entry_points.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)      152 2021-10-23 12:32:22.000000 bw2data-4.0.dev9/bw2data.egg-info/requires.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)        8 2021-10-23 12:32:22.000000 bw2data-4.0.dev9/bw2data.egg-info/top_level.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)       35 2021-05-06 13:38:14.000000 bw2data-4.0.dev9/pytest.ini
+-rw-r--r--   0 cmutel     (501) staff       (20)      189 2021-10-19 21:11:54.000000 bw2data-4.0.dev9/requirements-test.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)      152 2021-10-02 06:17:57.000000 bw2data-4.0.dev9/requirements.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)       38 2021-10-23 12:32:23.778325 bw2data-4.0.dev9/setup.cfg
+-rw-r--r--   0 cmutel     (501) staff       (20)     2423 2021-05-19 17:56:41.000000 bw2data-4.0.dev9/setup.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2021-10-23 12:32:23.773672 bw2data-4.0.dev9/tests/
+-rw-r--r--   0 cmutel     (501) staff       (20)        0 2021-05-06 13:38:14.000000 bw2data-4.0.dev9/tests/__init__.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     6426 2021-10-13 19:56:32.000000 bw2data-4.0.dev9/tests/activity_proxy.py
+-rw-r--r--   0 cmutel     (501) staff       (20)      326 2021-10-13 19:56:16.000000 bw2data-4.0.dev9/tests/base.py
+-rw-r--r--   0 cmutel     (501) staff       (20)      633 2021-10-13 19:56:16.000000 bw2data-4.0.dev9/tests/compatibility.py
+-rw-r--r--   0 cmutel     (501) staff       (20)      224 2021-10-13 19:56:16.000000 bw2data-4.0.dev9/tests/config.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     2135 2021-10-13 19:56:15.000000 bw2data-4.0.dev9/tests/data_store.py
+-rw-r--r--   0 cmutel     (501) staff       (20)    23183 2021-10-23 11:20:12.000000 bw2data-4.0.dev9/tests/database.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     6384 2021-10-13 19:56:16.000000 bw2data-4.0.dev9/tests/database_querying.py
+-rw-r--r--   0 cmutel     (501) staff       (20)    10222 2021-10-13 19:56:32.000000 bw2data-4.0.dev9/tests/exchange_proxy.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     2964 2021-10-13 19:56:16.000000 bw2data-4.0.dev9/tests/fixtures.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     2450 2021-10-13 19:56:16.000000 bw2data-4.0.dev9/tests/geo.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     6692 2021-10-23 11:25:19.000000 bw2data-4.0.dev9/tests/ia.py
+-rw-r--r--   0 cmutel     (501) staff       (20)    24447 2021-05-06 13:38:14.000000 bw2data-4.0.dev9/tests/naughty_strings.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)    61920 2021-10-13 19:56:36.000000 bw2data-4.0.dev9/tests/parameters.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     7969 2021-10-13 19:56:16.000000 bw2data-4.0.dev9/tests/projects.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     9889 2021-10-13 19:56:33.000000 bw2data-4.0.dev9/tests/search.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     1280 2021-10-13 19:56:16.000000 bw2data-4.0.dev9/tests/serialization.py
+-rw-r--r--   0 cmutel     (501) staff       (20)      959 2021-10-13 19:56:16.000000 bw2data-4.0.dev9/tests/sqlite.py
+-rw-r--r--   0 cmutel     (501) staff       (20)      605 2021-10-13 19:56:16.000000 bw2data-4.0.dev9/tests/updates.py
+-rw-r--r--   0 cmutel     (501) staff       (20)    10460 2021-10-23 06:31:32.000000 bw2data-4.0.dev9/tests/utils.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     3824 2021-10-13 19:56:34.000000 bw2data-4.0.dev9/tests/validation.py
```

### Comparing `bw2data-4.0.dev8/LICENSE.txt` & `bw2data-4.0.dev9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/PKG-INFO` & `bw2data-4.0.dev9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: bw2data
-Version: 4.0.dev8
+Version: 4.0.dev9
 Summary: Tools for the management of inventory databases and impact assessment methods. Part of the Brightway2 LCA Framework
 Home-page: https://github.com/brightway-lca/brightway2-data
 Author: Chris Mutel
 Author-email: cmutel@gmail.com
 License: 3-clause BSD
 Description: Brightway2 data management
         ==========================
```

### Comparing `bw2data-4.0.dev8/README.rst` & `bw2data-4.0.dev9/README.rst`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/bw2data/__init__.py` & `bw2data-4.0.dev9/bw2data/__init__.py`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/bw2data/backends/__init__.py` & `bw2data-4.0.dev9/bw2data/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/bw2data/backends/base.py` & `bw2data-4.0.dev9/bw2data/backends/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,25 @@
 import random
 import sqlite3
 import warnings
 
 import pandas
 import pyprind
 from bw_processing import clean_datapackage_name, create_datapackage
+from collections import defaultdict
 from fs.zipfs import ZipFS
 from peewee import DoesNotExist, fn
 
 from .. import config, databases, geomapping
 from ..data_store import ProcessedDataStore
 from ..errors import InvalidExchange, UnknownObject, UntypedExchange, WrongDatabase
 from ..project import writable_project
 from ..query import Query
 from ..search import IndexManager, Searcher
-from ..utils import as_uncertainty_dict
+from ..utils import as_uncertainty_dict, get_geocollection
 from . import sqlite3_lci_db
 from .proxies import Activity
 from .schema import ActivityDataset, ExchangeDataset, get_id
 from .utils import (
     check_exchange,
     dict_as_activitydataset,
     dict_as_exchangedataset,
@@ -496,15 +497,21 @@
             raise WrongDatabase(
                 "Can't write activities in databases {} to database {}".format(
                     wrong_database, self.name
                 )
             )
 
         databases[self.name]["number"] = len(data)
+
         databases.set_modified(self.name)
+        geocollections = {get_geocollection(x.get('location')) for x in data.values()}
+        if None in geocollections:
+            print('Not able to determine geocollections for all datasets. This database is not ready for regionalization.')
+            geocollections.discard(None)
+        databases[self.name]["geocollections"] = sorted(geocollections)
 
         geomapping.add({x["location"] for x in data.values() if x.get("location")})
         if data:
             try:
                 self._efficient_write_many_data(data)
             except:
                 # Purge all data from database, then reraise
@@ -831,7 +838,29 @@
         from bw2calc import LCA
 
         lca = LCA({self.random(): 1})
         lca.lci()
 
         smg = SparseMatrixGrapher(lca.technosphere_matrix)
         return smg.ordered_graph(filename, **kwargs)
+
+    def delete_duplicate_exchanges(self, fields=['amount', 'type']):
+        """Delete exchanges which are exact duplicates. Useful if you accidentally ran your input data notebook twice.
+
+        To determine uniqueness, we look at the exchange input and output nodes, and at the exchanges values for fields ``fields``."""
+        def get_uniqueness_key(exchange, fields):
+            lst = [exchange.input.key, exchange.output.key]
+            for field in fields:
+                lst.append(exchange.get(field))
+            return tuple(lst)
+
+        exchange_mapping = defaultdict(list)
+
+        for act in self:
+            for exchange in act.exchanges():
+                exchange_mapping[get_uniqueness_key(exchange, fields)].append(exchange)
+
+        for lst in exchange_mapping.values():
+            if len(lst) > 1:
+                for exc in lst[-1:0:-1]:
+                    print("Deleting exchange:", exc)
+                    exc.delete()
```

### Comparing `bw2data-4.0.dev8/bw2data/backends/iotable/__init__.py` & `bw2data-4.0.dev9/bw2data/backends/iotable/__init__.py`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/bw2data/backends/proxies.py` & `bw2data-4.0.dev9/bw2data/backends/proxies.py`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/bw2data/backends/schema.py` & `bw2data-4.0.dev9/bw2data/backends/schema.py`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/bw2data/backends/utils.py` & `bw2data-4.0.dev9/bw2data/backends/utils.py`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/bw2data/bin/bw2_uptodate.py` & `bw2data-4.0.dev9/bw2data/bin/bw2_uptodate.py`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/bw2data/compat.py` & `bw2data-4.0.dev9/bw2data/compat.py`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/bw2data/configuration.py` & `bw2data-4.0.dev9/bw2data/configuration.py`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/bw2data/data_store.py` & `bw2data-4.0.dev9/bw2data/data_store.py`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/bw2data/database.py` & `bw2data-4.0.dev9/bw2data/database.py`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/bw2data/errors.py` & `bw2data-4.0.dev9/bw2data/errors.py`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/bw2data/fatomic.py` & `bw2data-4.0.dev9/bw2data/fatomic.py`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/bw2data/filesystem.py` & `bw2data-4.0.dev9/bw2data/filesystem.py`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/bw2data/ia_data_store.py` & `bw2data-4.0.dev9/bw2data/ia_data_store.py`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/bw2data/logs.py` & `bw2data-4.0.dev9/bw2data/logs.py`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/bw2data/meta.py` & `bw2data-4.0.dev9/bw2data/meta.py`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/bw2data/method.py` & `bw2data-4.0.dev9/bw2data/method.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from . import config, geomapping, methods
 from .backends.schema import get_id
 from .ia_data_store import ImpactAssessmentDataStore
-from .utils import as_uncertainty_dict
+from .utils import as_uncertainty_dict, get_geocollection
 from .validate import ia_validator
 
 
 class Method(ImpactAssessmentDataStore):
     """A manager for an impact assessment method. This class can register or deregister methods, write intermediate data, process data to parameter arrays, validate, and copy methods.
 
     The Method class never holds intermediate data, but it can load or write intermediate data. The only attribute is *name*, which is the name of the method being managed.
@@ -55,13 +55,22 @@
     def write(self, data, process=True):
         """Serialize intermediate data to disk.
 
         Sets the metadata key ``num_cfs`` automatically."""
         if self.name not in self._metadata:
             self.register()
         self.metadata["num_cfs"] = len(data)
+
+        third = lambda x: x[2] if len(x) == 3 else None
+
+        geocollections = {get_geocollection(third(elem), default_global_location=True) for elem in data}
+        if None in geocollections:
+            print('Not able to determine geocollections for all CFs. This method is not ready for regionalization.')
+            geocollections.discard(None)
+
+        self.metadata['geocollections'] = sorted(geocollections)
         self._metadata.flush()
         super(Method, self).write(data)
 
     def process(self, **extra_metadata):
         extra_metadata["global_index"] = geomapping[config.global_location]
         super().process(**extra_metadata)
```

### Comparing `bw2data-4.0.dev8/bw2data/parameters.py` & `bw2data-4.0.dev9/bw2data/parameters.py`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/bw2data/project.py` & `bw2data-4.0.dev9/bw2data/project.py`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/bw2data/proxies.py` & `bw2data-4.0.dev9/bw2data/proxies.py`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/bw2data/query.py` & `bw2data-4.0.dev9/bw2data/query.py`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/bw2data/search/indices.py` & `bw2data-4.0.dev9/bw2data/search/indices.py`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/bw2data/search/search.py` & `bw2data-4.0.dev9/bw2data/search/search.py`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/bw2data/serialization.py` & `bw2data-4.0.dev9/bw2data/serialization.py`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/bw2data/sqlite.py` & `bw2data-4.0.dev9/bw2data/sqlite.py`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/bw2data/tests.py` & `bw2data-4.0.dev9/bw2data/tests.py`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/bw2data/updates.py` & `bw2data-4.0.dev9/bw2data/updates.py`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/bw2data/utils.py` & `bw2data-4.0.dev9/bw2data/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -383,19 +383,36 @@
 
 
 def get_activity(key):
     from .backends import Activity
     from .backends import ActivityDataset as AD
     from .database import Database
 
-    if isinstance(key, int):
+    if isinstance(key, Activity):
+        return key
+    elif isinstance(key, int):
         try:
             return Activity(AD.get(AD.id == key))
         except DoesNotExist:
             raise UnknownObject
 
     try:
         return Database(key[0]).get(key[1])
     except TypeError:
         raise UnknownObject(
             "Key {} cannot be understood as an activity" " or `(database, code)` tuple."
         )
+
+
+def get_geocollection(location, default_global_location=False):
+    '''conservative approach to finding geocollections. Won't guess about ecoinvent or other databases.'''
+    if not location:
+        if default_global_location:
+            return 'world'
+        else:
+            return None
+    elif isinstance(location, tuple):
+        return location[0]
+    elif isinstance(location, str) and (len(location) == 2 or location.lower() == 'glo'):
+        return 'world'
+    else:
+        return None
```

### Comparing `bw2data-4.0.dev8/bw2data/validate.py` & `bw2data-4.0.dev9/bw2data/validate.py`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/bw2data/weighting_normalization.py` & `bw2data-4.0.dev9/bw2data/weighting_normalization.py`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/bw2data.egg-info/PKG-INFO` & `bw2data-4.0.dev9/bw2data.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: bw2data
-Version: 4.0.dev8
+Version: 4.0.dev9
 Summary: Tools for the management of inventory databases and impact assessment methods. Part of the Brightway2 LCA Framework
 Home-page: https://github.com/brightway-lca/brightway2-data
 Author: Chris Mutel
 Author-email: cmutel@gmail.com
 License: 3-clause BSD
 Description: Brightway2 data management
         ==========================
```

### Comparing `bw2data-4.0.dev8/bw2data.egg-info/SOURCES.txt` & `bw2data-4.0.dev9/bw2data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/setup.py` & `bw2data-4.0.dev9/setup.py`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/tests/activity_proxy.py` & `bw2data-4.0.dev9/tests/activity_proxy.py`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/tests/compatibility.py` & `bw2data-4.0.dev9/tests/compatibility.py`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/tests/data_store.py` & `bw2data-4.0.dev9/tests/data_store.py`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/tests/database.py` & `bw2data-4.0.dev9/tests/database.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import warnings
 
 import numpy as np
 import pytest
 from bw_processing import load_datapackage
 from fs.zipfs import ZipFS
 
-from bw2data import geomapping, get_id
+from bw2data import geomapping, get_id, databases, Database
 from bw2data.backends import Activity as PWActivity
 from bw2data.backends import sqlite3_lci_db
-from bw2data.database import DatabaseChooser
+from bw2data.database import Database
 from bw2data.errors import (
     InvalidExchange,
     UnknownObject,
     UntypedExchange,
     WrongDatabase,
 )
 from bw2data.meta import databases
@@ -30,57 +30,57 @@
 from .fixtures import food as food_data
 from .fixtures import get_naughty
 
 
 @pytest.fixture
 @bw2test
 def food():
-    d = DatabaseChooser("biosphere")
+    d = Database("biosphere")
     d.write(biosphere)
-    d = DatabaseChooser("food")
+    d = Database("food")
     d.write(food_data)
 
 
 def test_food(food):
     assert len(databases) == 2
     assert sorted(x for x in databases) == ["biosphere", "food"]
 
 
 ### Basic functions
 
 
 @bw2test
 def test_get():
-    d = DatabaseChooser("biosphere")
+    d = Database("biosphere")
     d.write(biosphere)
     activity = d.get("1")
     assert isinstance(activity, PWActivity)
     assert activity["name"] == "an emission"
 
 
 @bw2test
 def test_iter():
-    d = DatabaseChooser("biosphere")
+    d = Database("biosphere")
     d.write(biosphere)
     activity = next(iter(d))
     assert isinstance(activity, PWActivity)
     assert activity["name"] in ("an emission", "another emission")
 
 
 @bw2test
 def test_get_random():
-    d = DatabaseChooser("biosphere")
+    d = Database("biosphere")
     d.write(biosphere)
     activity = d.random()
     assert isinstance(activity, PWActivity)
     assert activity["name"] in ("an emission", "another emission")
 
 
 def test_copy(food):
-    d = DatabaseChooser("food")
+    d = Database("food")
     with pytest.raises(AssertionError):
         d.copy("food")
     d.copy("repas")
     assert "repas" in databases
 
 
 @bw2test
@@ -88,34 +88,34 @@
     data = {
         ("old name", "1"): {
             "exchanges": [
                 {"input": ("old name", "1"), "amount": 1.0, "type": "technosphere"}
             ]
         }
     }
-    d = DatabaseChooser("old name")
+    d = Database("old name")
     d.write(data)
     new_db = d.copy("new name")
     new_data = new_db.load()
     assert list(new_data.values())[0]["exchanges"][0]["input"] == ("new name", "1")
     assert list(data.values())[0]["exchanges"][0]["input"] == ("old name", "1")
     assert list(d.load().values())[0]["exchanges"][0]["input"] == ("old name", "1")
 
 
 @bw2test
 def test_raise_wrong_database():
     data = {("foo", "1"): {}}
-    d = DatabaseChooser("bar")
+    d = Database("bar")
     with pytest.raises(WrongDatabase):
         d.write(data)
 
 
 @bw2test
 def test_deletes_from_database():
-    d = DatabaseChooser("biosphere")
+    d = Database("biosphere")
     d.write(biosphere)
     assert "biosphere" in databases
     del databases["biosphere"]
     assert next(
         sqlite3_lci_db.execute_sql(
             "select count(*) from activitydataset where database = 'biosphere'"
         )
@@ -125,15 +125,15 @@
             "select count(*) from exchangedataset where output_database = 'biosphere'"
         )
     ) == (0,)
 
 
 @bw2test
 def test_delete_warning():
-    d = DatabaseChooser("biosphere")
+    d = Database("biosphere")
     d.write(biosphere)
     with pytest.warns(UserWarning):
         d.delete()
 
 
 @bw2test
 def test_relabel_data():
@@ -149,69 +149,69 @@
         ("shiny new", "1"): {
             "exchanges": [{"input": ("old and boring", "42"), "amount": 1.0}]
         },
         ("shiny new", "2"): {
             "exchanges": [{"input": ("shiny new", "1"), "amount": 4.0}]
         },
     }
-    db = DatabaseChooser("foo")
+    db = Database("foo")
     assert shiny_new == db.relabel_data(old_data, "shiny new")
 
 
 ### Metadata
 
 
 @bw2test
 def test_find_graph_dependents():
     databases["one"] = {"depends": ["two", "three"]}
     databases["two"] = {"depends": ["four", "five"]}
     databases["three"] = {"depends": ["four"]}
     databases["four"] = {"depends": ["six"]}
     databases["five"] = {"depends": ["two"]}
     databases["six"] = {"depends": []}
-    assert DatabaseChooser("one").find_graph_dependents() == {
+    assert Database("one").find_graph_dependents() == {
         "one",
         "two",
         "three",
         "four",
         "five",
         "six",
     }
 
 
 @bw2test
 def test_register():
-    database = DatabaseChooser("testy")
+    database = Database("testy")
     database.register()
     assert "testy" in databases
     assert "depends" in databases["testy"]
 
 
 @bw2test
 def test_deregister():
-    d = DatabaseChooser("food")
+    d = Database("food")
     d.register()
     assert "food" in databases
     d.deregister()
     assert "food" not in databases
 
 
 @bw2test
 def test_write_sets_databases_number_attribute():
-    d = DatabaseChooser("biosphere")
+    d = Database("biosphere")
     d.write(biosphere)
     assert databases["biosphere"]["number"] == len(biosphere)
 
 
 ### Processed arrays
 
 
 @bw2test
 def test_process_unknown_object():
-    database = DatabaseChooser("testy")
+    database = Database("testy")
     data = {
         ("testy", "A"): {},
         ("testy", "B"): {
             "exchanges": [
                 {"input": ("testy", "A"), "amount": 1, "type": "technosphere"},
                 {"input": ("testy", "C"), "amount": 1, "type": "technosphere"},
             ]
@@ -222,48 +222,48 @@
 
 
 ### String handling
 
 
 @bw2test
 def test_naughty_activity_codes():
-    db = DatabaseChooser("foo")
+    db = Database("foo")
     data = {("foo", str(i)): {"name": x} for i, x in enumerate(get_naughty())}
     db.write(data)
     assert set(get_naughty()) == set(x["name"] for x in db)
 
 
 @bw2test
 def test_setup():
-    d = DatabaseChooser("biosphere")
+    d = Database("biosphere")
     d.write(biosphere)
-    d = DatabaseChooser("food")
+    d = Database("food")
     d.write(food_data)
 
 
 @bw2test
 def test_rename():
-    d = DatabaseChooser("biosphere")
+    d = Database("biosphere")
     d.write(biosphere)
-    d = DatabaseChooser("food")
+    d = Database("food")
     d.write(copy.deepcopy(food_data))
     ndb = d.rename("buildings")
     ndb_data = ndb.load()
     assert ndb.name == "buildings"
     assert d.name == "buildings"
     assert len(ndb_data) == len(food_data)
     for key in ndb_data:
         assert key[0] == "buildings"
         for exc in ndb_data[key]["exchanges"]:
             assert exc["input"][0] in ("biosphere", "buildings")
 
 
 @bw2test
 def test_exchange_save():
-    database = DatabaseChooser("testy")
+    database = Database("testy")
     data = {
         ("testy", "A"): {},
         ("testy", "C"): {"type": "biosphere"},
         ("testy", "B"): {
             "exchanges": [
                 {"input": ("testy", "A"), "amount": 1, "type": "technosphere"},
                 {"input": ("testy", "B"), "amount": 1, "type": "production"},
@@ -284,15 +284,15 @@
     exc = [x for x in act.production()][0]
     assert exc["amount"] == 2
 
 
 @bw2test
 @pytest.mark.skip()
 def test_dirty_activities():
-    database = DatabaseChooser("testy")
+    database = Database("testy")
     data = {
         ("testy", "A"): {},
         ("testy", "C"): {"type": "biosphere"},
         ("testy", "B"): {
             "exchanges": [
                 {"input": ("testy", "A"), "amount": 1, "type": "technosphere"},
                 {"input": ("testy", "B"), "amount": 1, "type": "production"},
@@ -309,15 +309,15 @@
     lca = act.lca()
     assert not databases["testy"].get("dirty")
     assert lca.supply_array[lca.activity_dict[("testy", "A")]] == 0.5
 
 
 @bw2test
 def test_process_invalid_exchange_value():
-    database = DatabaseChooser("testy")
+    database = Database("testy")
     data = {
         ("testy", "A"): {},
         ("testy", "B"): {
             "exchanges": [
                 {"input": ("testy", "A"), "amount": np.nan, "type": "technosphere"},
                 {"input": ("testy", "C"), "amount": 1, "type": "technosphere"},
             ]
@@ -325,74 +325,74 @@
     }
     with pytest.raises(ValueError):
         database.write(data)
 
 
 @bw2test
 def test_untyped_exchange_error():
-    database = DatabaseChooser("testy")
+    database = Database("testy")
     database_data = {
         ("testy", "A"): {"exchanges": [{"amount": 1, "input": ("testy", "A")}]},
     }
     with pytest.raises(UntypedExchange):
         database.write(database_data, process=False)
 
 
 @bw2test
 def test_no_input_raises_invalid_exchange():
-    database = DatabaseChooser("testy")
+    database = Database("testy")
     database_data = {
         ("testy", "A"): {"exchanges": [{"amount": 1}]},
     }
     with pytest.raises(InvalidExchange):
         database.write(database_data, process=False)
 
 
 @bw2test
 def test_no_amount_raises_invalid_exchange():
-    database = DatabaseChooser("testy")
+    database = Database("testy")
     database_data = {
         ("testy", "A"): {
             "exchanges": [{"input": ("testy", "A"), "type": "technosphere"}]
         },
     }
     with pytest.raises(InvalidExchange):
         database.write(database_data, process=False)
 
 
 @bw2test
 def test_zero_amount_is_valid_exchange():
-    database = DatabaseChooser("testy")
+    database = Database("testy")
     database_data = {
         ("testy", "A"): {
             "exchanges": [
                 {"input": ("testy", "A"), "type": "technosphere", "amount": 0.0}
             ]
         },
     }
     database.write(database_data, process=False)
 
 
 @bw2test
 def test_process_checks_process_type():
-    database = DatabaseChooser("a database")
+    database = Database("a database")
     database.write(
         {
             ("a database", "foo"): {"exchanges": [], "type": "process"},
             ("a database", "bar"): {"type": "definitely not a process"},
         },
         process=True,
     )
     # This shouldn't raise an error
     assert database.process() is None
 
 
 @bw2test
 def test_geomapping_array_includes_only_processes():
-    database = DatabaseChooser("a database")
+    database = Database("a database")
     database.write(
         {
             ("a database", "foo"): {
                 "exchanges": [],
                 "type": "process",
                 "location": "bar",
             },
@@ -403,15 +403,15 @@
     array = package.get_resource("a_database_inventory_geomapping_matrix.indices")[0]
     assert array.shape == (1,)
     assert array[0]["col"] == geomapping["bar"]
 
 
 @bw2test
 def test_processed_array():
-    database = DatabaseChooser("a database")
+    database = Database("a database")
     database.write(
         {
             ("a database", "2"): {
                 "type": "process",
                 "exchanges": [
                     {
                         "input": ("a database", "2"),
@@ -433,21 +433,21 @@
     array = package.get_resource("a_database_technosphere_matrix.distributions")[0]
     assert array.shape == (1,)
     assert array[0]["uncertainty_type"] == 7
 
 
 @bw2test
 def test_base_class():
-    database = DatabaseChooser("a database")
+    database = Database("a database")
     assert database._metadata is databases
 
 
 @bw2test
 def test_find_dependents():
-    database = DatabaseChooser("a database")
+    database = Database("a database")
     database.write(
         {
             ("a database", "foo"): {
                 "exchanges": [
                     {
                         "input": ("foo", "bar"),
                         "type": "technosphere",
@@ -493,42 +493,42 @@
         process=False,
     )
     assert database.find_dependents(ignore={"awkward"}) == ["biosphere", "foo"]
 
 
 @bw2test
 def test_set_dependents():
-    foo = DatabaseChooser("foo")
+    foo = Database("foo")
     foo.write(
         {
             ("foo", "bar"): {
                 "exchanges": [],
                 "type": "process",
             },
         }
     )
-    baz = DatabaseChooser("baz")
+    baz = Database("baz")
     baz.write(
         {
             ("baz", "w00t"): {
                 "exchanges": [],
                 "type": "process",
             },
         }
     )
-    biosphere = DatabaseChooser("biosphere")
+    biosphere = Database("biosphere")
     biosphere.write(
         {
             ("biosphere", "bar"): {
                 "exchanges": [],
                 "type": "process",
             },
         }
     )
-    database = DatabaseChooser("a database")
+    database = Database("a database")
     database.register()
     assert databases["a database"]["depends"] == []
     database.write(
         {
             ("a database", "foo"): {
                 "exchanges": [
                     {"input": ("foo", "bar"), "type": "technosphere", "amount": 1},
@@ -550,49 +550,49 @@
         }
     )
     assert databases["a database"]["depends"] == ["baz", "biosphere", "foo"]
 
 
 @bw2test
 def test_process_without_exchanges_still_in_processed_array():
-    database = DatabaseChooser("a database")
+    database = Database("a database")
     database.write({("a database", "foo"): {}})
 
     package = load_datapackage(ZipFS(database.filepath_processed()))
     array = package.get_resource("a_database_technosphere_matrix.data")[0]
     assert array[0] == 1
     assert array.shape == (1,)
 
 
 @bw2test
 def test_random_empty():
-    database = DatabaseChooser("a database")
+    database = Database("a database")
     database.write({})
     with warnings.catch_warnings() as w:
         warnings.simplefilter("ignore")
         assert database.random() is None
 
 
 @bw2test
 def test_new_activity():
-    database = DatabaseChooser("a database")
+    database = Database("a database")
     database.register()
     act = database.new_activity("foo", this="that", name="something")
     act.save()
 
     act = database.get("foo")
     assert act["database"] == "a database"
     assert act["code"] == "foo"
     assert act["location"] == "GLO"
     assert act["this"] == "that"
 
 
 @bw2test
 def test_can_split_processes_products():
-    database = DatabaseChooser("a database")
+    database = Database("a database")
     database.write(
         {
             # No implicit production because type specified and not process
             ("a database", "product"): {"type": "product"},
             ("a database", "foo"): {
                 "exchanges": [
                     {
@@ -617,15 +617,15 @@
     assert array.shape == (1,)
     assert array["col"][0] == get_id(("a database", "foo"))
     assert array["row"][0] == get_id(("a database", "product"))
 
 
 @bw2test
 def test_sqlite_processed_array_order():
-    database = DatabaseChooser("testy_new")
+    database = Database("testy_new")
     data = {
         ("testy_new", "C"): {},
         ("testy_new", "A"): {},
         ("testy_new", "B"): {
             "exchanges": [
                 {"input": ("testy_new", "A"), "amount": 1, "type": "technosphere"},
                 {"input": ("testy_new", "A"), "amount": 2, "type": "technosphere"},
@@ -680,15 +680,15 @@
     assert array.shape == (2,)
     assert np.allclose(array["row"], [x[0] for x in b])
     assert np.allclose(array["col"], [x[1] for x in b])
 
 
 @bw2test
 def test_no_distributions_if_no_uncertainty():
-    database = DatabaseChooser("a database")
+    database = Database("a database")
     database.write(
         {
             ("a database", "2"): {
                 "type": "process",
                 "exchanges": [
                     {
                         "input": ("a database", "2"),
@@ -704,15 +704,15 @@
     print(package.resources)
     with pytest.raises(KeyError):
         package.get_resource("a_database_technosphere_matrix.distributions")
 
 
 @bw2test
 def test_database_delete_parameters():
-    db = DatabaseChooser("example")
+    db = Database("example")
     db.register()
 
     a = db.new_activity(code="A", name="An activity")
     a.save()
     b = db.new_activity(code="B", name="Another activity")
     b.save()
     a.new_exchange(
@@ -749,7 +749,75 @@
     assert ParameterizedExchange.select().count() == 1
     assert DatabaseParameter.select().count() == 2
     assert len(parameters) == 4
 
     del databases["example"]
     assert not len(parameters)
     assert not ParameterizedExchange.select().count()
+
+
+@bw2test
+def test_delete_duplicate_exchanges():
+    all_exchanges = lambda db: [exc for ds in db for exc in ds.exchanges()]
+
+    db = Database("test-case")
+
+    db.write({
+        ("test-case", "1"): {
+            "exchanges": []
+        },
+        ("test-case", "2"): {
+            "exchanges": []
+        },
+        ("test-case", "3"): {
+            "exchanges": [
+                {"input": ("test-case", "2"), "type": "foo", "amount": 1},
+                {"input": ("test-case", "2"), "type": "foo", "amount": 2},
+                {"input": ("test-case", "2"), "type": "bar", "amount": 2},
+                {"input": ("test-case", "1"), "type": "foo", "amount": 12},
+                {"input": ("test-case", "1"), "type": "foo", "amount": 12},
+            ]
+        },
+    })
+
+    assert len(all_exchanges(db)) == 5
+    db.delete_duplicate_exchanges()
+    assert len(all_exchanges(db)) == 4
+    db.delete_duplicate_exchanges(fields=['amount'])
+    assert len(all_exchanges(db)) == 3
+
+
+@bw2test
+def test_add_geocollections(capsys):
+    db = Database("test-case")
+    db.write({
+        ("test-case", "1"): {
+            'location': 'RU',
+            "exchanges": []
+        },
+        ("test-case", "2"): {
+            "exchanges": []
+        },
+        ("test-case", "3"): {
+            "exchanges": [],
+            'location': ('foo', 'bar')
+        },
+    })
+    assert db.metadata['geocollections'] == ['foo', 'world']
+    assert "Not able" in capsys.readouterr().out
+
+
+@bw2test
+def test_add_geocollections_unable(capsys):
+    db = Database("test-case")
+    db.write({
+        ("test-case", "1"): {
+            'location': 'Russia',
+            "exchanges": []
+        },
+        ("test-case", "3"): {
+            "exchanges": [],
+            'location': ('foo', 'bar')
+        },
+    })
+    assert db.metadata['geocollections'] == ['foo']
+    assert "Not able" in capsys.readouterr().out
```

### Comparing `bw2data-4.0.dev8/tests/database_querying.py` & `bw2data-4.0.dev9/tests/database_querying.py`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/tests/exchange_proxy.py` & `bw2data-4.0.dev9/tests/exchange_proxy.py`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/tests/fixtures.py` & `bw2data-4.0.dev9/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/tests/geo.py` & `bw2data-4.0.dev9/tests/geo.py`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/tests/ia.py` & `bw2data-4.0.dev9/tests/ia.py`

 * *Files 14% similar despite different names*

```diff
@@ -203,7 +203,38 @@
 
     data = package.get_resource("foo_matrix_data.data")[0]
     assert np.allclose(data, [42])
 
     indices = package.get_resource("foo_matrix_data.indices")[0]
     assert np.allclose(indices["row"], get_id(("foo", "bar")))
     assert np.allclose(indices["col"], get_id(("foo", "bar")))
+
+
+@bw2test
+def test_method_geocollection(capsys):
+    m = Method(('foo',))
+    m.write([
+        (1, 2, "RU"),
+        (3, 4, ("foo", "bar"))
+    ])
+    assert m.metadata['geocollections'] == ['foo', 'world']
+    assert "Not able" not in capsys.readouterr().out
+
+
+@bw2test
+def test_method_geocollection_missing_ok(capsys):
+    m = Method(('foo',))
+    m.write([
+        (1, 2, None),
+        (1, 2),
+    ])
+    assert m.metadata['geocollections'] == ['world']
+    assert "Not able" not in capsys.readouterr().out
+
+
+@bw2test
+def test_method_geocollection_warning(capsys):
+    m = Method(('foo',))
+    m.write([
+        (1, 2, "Russia"),
+    ])
+    assert "Not able" in capsys.readouterr().out
```

### Comparing `bw2data-4.0.dev8/tests/naughty_strings.txt` & `bw2data-4.0.dev9/tests/naughty_strings.txt`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/tests/parameters.py` & `bw2data-4.0.dev9/tests/parameters.py`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/tests/projects.py` & `bw2data-4.0.dev9/tests/projects.py`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/tests/search.py` & `bw2data-4.0.dev9/tests/search.py`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/tests/serialization.py` & `bw2data-4.0.dev9/tests/serialization.py`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/tests/sqlite.py` & `bw2data-4.0.dev9/tests/sqlite.py`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/tests/updates.py` & `bw2data-4.0.dev9/tests/updates.py`

 * *Files identical despite different names*

### Comparing `bw2data-4.0.dev8/tests/utils.py` & `bw2data-4.0.dev9/tests/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # from bw_processing import load_package
 import pytest
 import stats_arrays as sa
 
 from bw2data import Database, Method, methods
 from bw2data.backends import Activity as PWActivity
+from bw2data.backends.schema import ActivityDataset as AD
 from bw2data.errors import ValidityError
 from bw2data.tests import BW2DataTest, bw2test
 from bw2data.utils import (
     as_uncertainty_dict,
     combine_methods,
     get_activity,
     merge_databases,
@@ -169,14 +170,29 @@
     assert as_uncertainty_dict({}) == {}
     assert as_uncertainty_dict(1) == {"amount": 1.0}
     with pytest.raises(TypeError):
         as_uncertainty_dict("foo")
 
 
 @bw2test
+def test_get_activity():
+    database = Database("a database", "sqlite")
+    database.write(
+        {
+            ("a database", "foo"): {"exchanges": [], "name": "baz"}
+        }
+    )
+    doc = AD.select().where(AD.name == 'baz').get()
+    assert isinstance(get_activity((doc.database, doc.code)), PWActivity)
+    assert get_activity((doc.database, doc.code)).id == doc.id
+    assert get_activity(doc.id).id == doc.id
+    act = get_activity((doc.database, doc.code))
+    assert get_activity(act).id == doc.id
+
+@bw2test
 def test_merge_databases_nonunique_activity_codes():
     first = Database("a database")
     first.write(
         {
             ("a database", "foo"): {
                 "exchanges": [
                     {
```

### Comparing `bw2data-4.0.dev8/tests/validation.py` & `bw2data-4.0.dev9/tests/validation.py`

 * *Files identical despite different names*

