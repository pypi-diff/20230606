# Comparing `tmp/lavacli-1.9.tar.gz` & `tmp/lavacli-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavacli-1.9.tar", last modified: Wed Apr 19 07:56:41 2023, max compression
+gzip compressed data, was "lavacli-2.0.tar", last modified: Tue Jun  6 11:14:18 2023, max compression
```

## Comparing `lavacli-1.9.tar` & `lavacli-2.0.tar`

### file list

```diff
@@ -1,65 +1,67 @@
-drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-04-19 07:56:41.306845 lavacli-1.9/
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)      105 2018-07-13 09:52:07.000000 lavacli-1.9/.coveragerc
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     2506 2023-03-17 09:18:40.000000 lavacli-1.9/.gitlab-ci.yml
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    34520 2018-01-18 08:05:38.000000 lavacli-1.9/LICENSE
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)      141 2019-03-13 08:49:12.000000 lavacli-1.9/MANIFEST.in
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1150 2023-04-19 07:56:41.306845 lavacli-1.9/PKG-INFO
-drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-04-19 07:56:41.298845 lavacli-1.9/doc/
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)      604 2018-04-13 14:07:49.000000 lavacli-1.9/doc/Makefile
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     5259 2023-02-24 10:40:23.000000 lavacli-1.9/doc/conf.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     2335 2020-09-09 08:32:09.000000 lavacli-1.9/doc/configuration.rst
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)      379 2019-11-27 05:33:22.000000 lavacli-1.9/doc/index.rst
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)      721 2019-04-24 15:25:09.000000 lavacli-1.9/doc/install.rst
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     4624 2022-05-10 09:55:41.000000 lavacli-1.9/doc/usage.rst
-drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-04-19 07:56:41.298845 lavacli-1.9/lavacli/
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1344 2023-04-19 07:56:07.000000 lavacli-1.9/lavacli/__about__.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     9098 2023-04-12 15:39:30.000000 lavacli-1.9/lavacli/__init__.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)      851 2023-02-24 10:40:23.000000 lavacli-1.9/lavacli/__main__.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)      111 2022-03-31 04:08:12.000000 lavacli-1.9/lavacli/colors.py
-drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-04-19 07:56:41.302845 lavacli-1.9/lavacli/commands/
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)        0 2022-05-09 15:46:10.000000 lavacli-1.9/lavacli/commands/__init__.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     4001 2023-02-24 10:40:23.000000 lavacli-1.9/lavacli/commands/aliases.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    13999 2023-04-07 12:33:18.000000 lavacli-1.9/lavacli/commands/device_types.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    15547 2023-04-07 07:01:47.000000 lavacli-1.9/lavacli/commands/devices.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     9742 2023-03-17 09:10:17.000000 lavacli-1.9/lavacli/commands/events.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     5767 2023-04-07 12:33:18.000000 lavacli-1.9/lavacli/commands/groups.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     4156 2023-02-24 10:40:23.000000 lavacli-1.9/lavacli/commands/identities.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    23030 2023-04-07 07:01:47.000000 lavacli-1.9/lavacli/commands/jobs.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    37032 2023-04-19 07:55:03.000000 lavacli-1.9/lavacli/commands/lab.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     3217 2023-02-24 10:40:23.000000 lavacli-1.9/lavacli/commands/results.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     9213 2023-03-17 09:10:17.000000 lavacli-1.9/lavacli/commands/system.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     3689 2023-02-24 10:40:23.000000 lavacli-1.9/lavacli/commands/tags.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    11354 2023-04-12 15:39:33.000000 lavacli-1.9/lavacli/commands/users.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     4119 2023-04-07 07:01:44.000000 lavacli-1.9/lavacli/commands/utils.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    12997 2023-04-07 07:01:47.000000 lavacli-1.9/lavacli/commands/workers.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1808 2023-03-21 10:08:31.000000 lavacli-1.9/lavacli/utils.py
-drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-04-19 07:56:41.298845 lavacli-1.9/lavacli.egg-info/
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1150 2023-04-19 07:56:41.000000 lavacli-1.9/lavacli.egg-info/PKG-INFO
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1242 2023-04-19 07:56:41.000000 lavacli-1.9/lavacli.egg-info/SOURCES.txt
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)        1 2023-04-19 07:56:41.000000 lavacli-1.9/lavacli.egg-info/dependency_links.txt
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)       41 2023-04-19 07:56:41.000000 lavacli-1.9/lavacli.egg-info/entry_points.txt
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)       36 2023-04-19 07:56:41.000000 lavacli-1.9/lavacli.egg-info/requires.txt
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)        8 2023-04-19 07:56:41.000000 lavacli-1.9/lavacli.egg-info/top_level.txt
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)        1 2023-04-19 07:56:41.000000 lavacli-1.9/lavacli.egg-info/zip-safe
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)       36 2023-03-17 09:09:30.000000 lavacli-1.9/requirements.txt
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)       38 2023-04-19 07:56:41.306845 lavacli-1.9/setup.cfg
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     2417 2023-03-17 09:10:17.000000 lavacli-1.9/setup.py
-drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-04-19 07:56:41.302845 lavacli-1.9/share/
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)      838 2018-04-13 12:29:55.000000 lavacli-1.9/share/lavacli.yaml
-drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-04-19 07:56:41.306845 lavacli-1.9/tests/
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)        0 2023-04-07 07:02:55.000000 lavacli-1.9/tests/__init__.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1806 2023-04-07 07:02:55.000000 lavacli-1.9/tests/conftest.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     8982 2023-04-07 07:02:55.000000 lavacli-1.9/tests/test_aliases.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    20063 2023-04-07 07:02:55.000000 lavacli-1.9/tests/test_device_types.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    32637 2023-04-07 07:02:55.000000 lavacli-1.9/tests/test_devices.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    24515 2023-04-07 07:02:55.000000 lavacli-1.9/tests/test_events.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1324 2023-04-07 07:02:55.000000 lavacli-1.9/tests/test_helpers.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     7504 2023-04-07 07:02:55.000000 lavacli-1.9/tests/test_identities.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    58342 2023-04-07 12:33:40.000000 lavacli-1.9/tests/test_jobs.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    94482 2023-04-19 07:55:03.000000 lavacli-1.9/tests/test_lab.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1615 2023-04-07 07:02:55.000000 lavacli-1.9/tests/test_lavacli.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    11619 2023-04-07 07:02:55.000000 lavacli-1.9/tests/test_results.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    25702 2023-04-07 07:02:55.000000 lavacli-1.9/tests/test_system.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     6550 2023-04-07 07:02:55.000000 lavacli-1.9/tests/test_tags.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)     5479 2023-04-12 15:39:33.000000 lavacli-1.9/tests/test_users.py
--rw-r--r--   0 ivoire    (1000) ivoire    (1000)    24888 2023-04-07 12:33:53.000000 lavacli-1.9/tests/test_workers.py
+drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-06-06 11:14:18.827684 lavacli-2.0/
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)      105 2018-07-13 09:52:07.000000 lavacli-2.0/.coveragerc
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     2112 2023-06-06 09:40:54.000000 lavacli-2.0/.gitlab-ci.yml
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    34520 2018-01-18 08:05:38.000000 lavacli-2.0/LICENSE
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)      141 2019-03-13 08:49:12.000000 lavacli-2.0/MANIFEST.in
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1053 2023-06-06 11:14:18.827684 lavacli-2.0/PKG-INFO
+drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-06-06 11:14:18.823685 lavacli-2.0/doc/
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)      604 2018-04-13 14:07:49.000000 lavacli-2.0/doc/Makefile
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     5259 2023-02-24 10:40:23.000000 lavacli-2.0/doc/conf.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     2335 2020-09-09 08:32:09.000000 lavacli-2.0/doc/configuration.rst
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)      379 2019-11-27 05:33:22.000000 lavacli-2.0/doc/index.rst
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)      711 2023-06-06 09:42:05.000000 lavacli-2.0/doc/install.rst
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     4624 2022-05-10 09:55:41.000000 lavacli-2.0/doc/usage.rst
+drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-06-06 11:14:18.823685 lavacli-2.0/lavacli/
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1334 2023-06-06 10:05:10.000000 lavacli-2.0/lavacli/__about__.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     9240 2023-06-01 10:18:51.000000 lavacli-2.0/lavacli/__init__.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)      851 2023-02-24 10:40:23.000000 lavacli-2.0/lavacli/__main__.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)      111 2022-03-31 04:08:12.000000 lavacli-2.0/lavacli/colors.py
+drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-06-06 11:14:18.823685 lavacli-2.0/lavacli/commands/
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)        0 2022-05-09 15:46:10.000000 lavacli-2.0/lavacli/commands/__init__.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     4001 2023-02-24 10:40:23.000000 lavacli-2.0/lavacli/commands/aliases.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    13999 2023-04-07 12:33:18.000000 lavacli-2.0/lavacli/commands/device_types.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    15547 2023-04-07 07:01:47.000000 lavacli-2.0/lavacli/commands/devices.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     9742 2023-03-17 09:10:17.000000 lavacli-2.0/lavacli/commands/events.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     5767 2023-04-07 12:33:18.000000 lavacli-2.0/lavacli/commands/groups.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     4156 2023-02-24 10:40:23.000000 lavacli-2.0/lavacli/commands/identities.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    23030 2023-06-06 09:43:24.000000 lavacli-2.0/lavacli/commands/jobs.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    44186 2023-06-02 12:23:16.000000 lavacli-2.0/lavacli/commands/lab.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     3217 2023-02-24 10:40:23.000000 lavacli-2.0/lavacli/commands/results.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     9213 2023-03-17 09:10:17.000000 lavacli-2.0/lavacli/commands/system.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     3689 2023-02-24 10:40:23.000000 lavacli-2.0/lavacli/commands/tags.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    11354 2023-04-12 15:39:33.000000 lavacli-2.0/lavacli/commands/users.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     4119 2023-04-07 07:01:44.000000 lavacli-2.0/lavacli/commands/utils.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    12997 2023-04-07 07:01:47.000000 lavacli-2.0/lavacli/commands/workers.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     5070 2023-06-02 11:39:40.000000 lavacli-2.0/lavacli/schemas.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1808 2023-03-21 10:08:31.000000 lavacli-2.0/lavacli/utils.py
+drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-06-06 11:14:18.823685 lavacli-2.0/lavacli.egg-info/
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1053 2023-06-06 11:14:18.000000 lavacli-2.0/lavacli.egg-info/PKG-INFO
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1283 2023-06-06 11:14:18.000000 lavacli-2.0/lavacli.egg-info/SOURCES.txt
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)        1 2023-06-06 11:14:18.000000 lavacli-2.0/lavacli.egg-info/dependency_links.txt
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)       41 2023-06-06 11:14:18.000000 lavacli-2.0/lavacli.egg-info/entry_points.txt
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)       47 2023-06-06 11:14:18.000000 lavacli-2.0/lavacli.egg-info/requires.txt
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)        8 2023-06-06 11:14:18.000000 lavacli-2.0/lavacli.egg-info/top_level.txt
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)        1 2023-06-06 11:13:47.000000 lavacli-2.0/lavacli.egg-info/zip-safe
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)       47 2023-06-01 10:18:51.000000 lavacli-2.0/requirements.txt
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)       38 2023-06-06 11:14:18.827684 lavacli-2.0/setup.cfg
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     2344 2023-06-06 09:44:15.000000 lavacli-2.0/setup.py
+drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-06-06 11:14:18.823685 lavacli-2.0/share/
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)      838 2018-04-13 12:29:55.000000 lavacli-2.0/share/lavacli.yaml
+drwxr-xr-x   0 ivoire    (1000) ivoire    (1000)        0 2023-06-06 11:14:18.827684 lavacli-2.0/tests/
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)        0 2023-04-07 07:02:55.000000 lavacli-2.0/tests/__init__.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1806 2023-04-07 07:02:55.000000 lavacli-2.0/tests/conftest.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     8982 2023-04-07 07:02:55.000000 lavacli-2.0/tests/test_aliases.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    20063 2023-04-07 07:02:55.000000 lavacli-2.0/tests/test_device_types.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    32637 2023-04-07 07:02:55.000000 lavacli-2.0/tests/test_devices.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    24515 2023-04-07 07:02:55.000000 lavacli-2.0/tests/test_events.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1324 2023-04-07 07:02:55.000000 lavacli-2.0/tests/test_helpers.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     7504 2023-04-07 07:02:55.000000 lavacli-2.0/tests/test_identities.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    58342 2023-04-07 12:33:40.000000 lavacli-2.0/tests/test_jobs.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)   111807 2023-06-02 13:09:33.000000 lavacli-2.0/tests/test_lab.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     1615 2023-04-07 07:02:55.000000 lavacli-2.0/tests/test_lavacli.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    11619 2023-04-07 07:02:55.000000 lavacli-2.0/tests/test_results.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     3052 2023-06-01 10:18:51.000000 lavacli-2.0/tests/test_schemas.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    25702 2023-04-07 07:02:55.000000 lavacli-2.0/tests/test_system.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     6550 2023-04-07 07:02:55.000000 lavacli-2.0/tests/test_tags.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)     5479 2023-04-12 15:39:33.000000 lavacli-2.0/tests/test_users.py
+-rw-r--r--   0 ivoire    (1000) ivoire    (1000)    24888 2023-04-07 12:33:53.000000 lavacli-2.0/tests/test_workers.py
```

### Comparing `lavacli-1.9/LICENSE` & `lavacli-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lavacli-1.9/PKG-INFO` & `lavacli-2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: lavacli
-Version: 1.9
+Version: 2.0
 Summary: LAVA XML-RPC command line interface
-Home-page: https://git.lavasoftware.org/lava/lavacli
+Home-page: https://gitlab.com/lava/lavacli
 Author: Rémi Duraffort
 Author-email: remi.duraffort@linaro.org
 License: AGPLv3+
-Project-URL: Bug Tracker, https://git.lavasoftware.org/lava/lavacli/issues/
-Project-URL: Documentation, https://docs.lavasoftware.org/lavacli/
-Project-URL: Source Code, https://git.lavasoftware.org/lava/lavacli/
+Project-URL: Bug Tracker, https://gitlab.com/lava/lavacli/issues/
+Project-URL: Source Code, https://gitlab.com/lava/lavacli/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `lavacli-1.9/doc/Makefile` & `lavacli-2.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `lavacli-1.9/doc/conf.py` & `lavacli-2.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.9/doc/configuration.rst` & `lavacli-2.0/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `lavacli-1.9/doc/install.rst` & `lavacli-2.0/doc/install.rst`

 * *Files 12% similar despite different names*

```diff
@@ -24,13 +24,13 @@
 Development versions
 =====================
 
 It's also possible to use lavacli directly from the sources:
 
 .. code-block:: shell
 
-    git clone https://git.lavasoftware.org/lava/lavacli.git
+    git clone https://gitlab.com/lava/lavacli.git
     cd lavacli
     virtualenv -p python3 venv
     source venv/bin/activate
     pip install -r requirements.txt
     python3 -m lavacli
```

### Comparing `lavacli-1.9/doc/usage.rst` & `lavacli-2.0/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `lavacli-1.9/lavacli/__about__.py` & `lavacli-2.0/lavacli/__about__.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,9 +37,9 @@
         return "git"
 
 
 __author__ = "Rémi Duraffort"
 __author_email__ = "remi.duraffort@linaro.org"
 __description__ = "LAVA XML-RPC command line interface"
 __license__ = "AGPLv3+"
-__url__ = "https://git.lavasoftware.org/lava/lavacli"
-__version__ = "1.9"
+__url__ = "https://gitlab.com/lava/lavacli"
+__version__ = "2.0"
```

### Comparing `lavacli-1.9/lavacli/__init__.py` & `lavacli-2.0/lavacli/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,16 +219,19 @@
 
     # Load the configuration (if any)
     uri = options.uri
     proxy = None
     version = VERSION_LATEST
     config = {}
 
-    # Skip when sub_command is "identities"
-    if remaining[0] not in ["identities", "utils"]:
+    lab_validate = False
+    if len(remaining) > 2 and remaining[0] == "lab" and remaining[1] == "validate":
+        lab_validate = True
+    # Skip when not needed.
+    if remaining[0] not in ["identities", "utils"] and not lab_validate:
         if uri is None:
             config = load_config(options.identity)
             if config.get("uri") is None:
                 print("Unknown identity '%s'" % options.identity, file=sys.stderr)
                 return 1
             username = config.get("username")
             token = config.get("token")
```

### Comparing `lavacli-1.9/lavacli/__main__.py` & `lavacli-2.0/lavacli/__main__.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.9/lavacli/commands/aliases.py` & `lavacli-2.0/lavacli/commands/aliases.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.9/lavacli/commands/device_types.py` & `lavacli-2.0/lavacli/commands/device_types.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.9/lavacli/commands/devices.py` & `lavacli-2.0/lavacli/commands/devices.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.9/lavacli/commands/events.py` & `lavacli-2.0/lavacli/commands/events.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.9/lavacli/commands/groups.py` & `lavacli-2.0/lavacli/commands/groups.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.9/lavacli/commands/identities.py` & `lavacli-2.0/lavacli/commands/identities.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.9/lavacli/commands/jobs.py` & `lavacli-2.0/lavacli/commands/jobs.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.9/lavacli/commands/lab.py` & `lavacli-2.0/lavacli/commands/lab.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,21 +15,22 @@
 #
 # You should have received a copy of the GNU Affero General Public License
 # along with lavacli.  If not, see <http://www.gnu.org/licenses/>
 
 import contextlib
 import difflib
 import xmlrpc
-from dataclasses import MISSING, asdict, dataclass, field, fields
+from dataclasses import MISSING, InitVar, asdict, dataclass, field, fields
 from pathlib import Path
 from typing import Any, Dict, List, Set
 
 import ruamel.yaml
+from voluptuous import MultipleInvalid
 
-from lavacli import colors
+from lavacli import colors, schemas
 
 
 def print_file_diff(src, dst):
     if src is None:
         print("    | + None")
     elif dst is None:
         print("    | - None")
@@ -75,26 +76,37 @@
 class Device(Base):
     hostname: str
     device_type: str
     worker: str
     description: str = None
     tags: Set[str] = field(default_factory=set)
     permissions: Set[GroupDevicePermission] = field(default_factory=set)
+    health: str = None
+    retire: InitVar[bool] = None
 
-    def __post_init__(self):
+    def __post_init__(self, retire):
         self.tags = set(self.tags)
         self.permissions = set([GroupDevicePermission(**p) for p in self.permissions])
+        self.retire = retire
+        if self.retire is True:
+            self.health = "RETIRED"
 
     def diff(self, data: Dict[str, Any]) -> List[str]:
         data = data.copy()
         data["tags"] = set(data["tags"])
         if data["description"] is None:
             data["description"] = ""
         if self.description is None:
             self.description = ""
+        if self.health is None:
+            # Do nothing if not defined.
+            self.health = data["health"]
+        if self.retire is False and data["health"] == "RETIRED":
+            # set health to UNKNOWN to un-retire.
+            self.health = "UNKNOWN"
         return super().diff(data)
 
     def dump(self):
         defaults = {f.name: f.default for f in fields(self) if f.default != MISSING}
         data = {}
         for k, v in asdict(self).items():
             if k in defaults and v == defaults[k]:
@@ -108,14 +120,18 @@
         else:
             data["tags"] = sorted(data["tags"])
         del data["hostname"]
         if not data["permissions"]:
             del data["permissions"]
         else:
             data["permissions"] = [p.dump() for p in sorted(data["permissions"])]
+        # Add `retire: true` for retired device.
+        if data["health"] == "Retired":
+            data["retire"] = True
+        del data["health"]
         return data if data else None
 
     def get_dict(self, base):
         with contextlib.suppress(FileNotFoundError):
             return (base / "devices" / f"{self.hostname}.jinja2").read_text(
                 encoding="utf-8"
             )
@@ -129,15 +145,15 @@
             )
 
 
 @dataclass
 class DeviceType(Base):
     name: str
     description: str = ""
-    health_disabled: str = False
+    health_disabled: bool = False
     health_denominator: str = "hours"
     health_frequency: int = 24
     aliases: Set[str] = field(default_factory=set)
     display: bool = True
     permissions: Set[GroupDevicePermission] = field(default_factory=set)
 
     def __post_init__(self):
@@ -293,34 +309,51 @@
 
 
 @dataclass
 class Worker(Base):
     hostname: str
     description: str = ""
     job_limit: int = 0
+    health: str = None
+    retire: InitVar[bool] = False
+
+    def __post_init__(self, retire):
+        self.retire = retire
+        if self.retire is True:
+            self.health = "RETIRED"
 
     def diff(self, data: Dict[str, Any]) -> List[str]:
         data = data.copy()
         if data["description"] is None:
             data["description"] = ""
         if self.description is None:
             self.description = ""
+        if self.health is None:
+            # Do nothing if not defined.
+            self.health = data["health"]
+        if self.retire is False and data["health"] == "RETIRED":
+            # Set health to ACTIVE to un-retire.
+            self.health = "ACTIVE"
         return super().diff(data)
 
     def dump(self):
         defaults = {f.name: f.default for f in fields(self) if f.default != MISSING}
         data = {}
         for k, v in asdict(self).items():
             if k in defaults and v == defaults[k]:
                 continue
             data[k] = v
 
         if "description" in data and data["description"] in ["", None]:
             del data["description"]
         del data["hostname"]
+        # Add `retire: true` for retired worker.
+        if data["health"] == "Retired":
+            data["retire"] = True
+        del data["health"]
         return data if data else None
 
     def get_config(self, base):
         with contextlib.suppress(FileNotFoundError):
             return (base / "workers" / self.hostname / "dispatcher.yaml").read_text(
                 encoding="utf-8"
             )
@@ -388,14 +421,99 @@
             "device_types": {k: self.device_types[k].dump() for k in self.device_types},
             "devices": {k: self.devices[k].dump() for k in self.devices},
             "groups": {k: self.groups[k].dump() for k in self.groups},
             "users": {k: self.users[k].dump() for k in self.users},
             "workers": {k: self.workers[k].dump() for k in self.workers},
         }
 
+    def dump_device_types(self):
+        return {
+            "device_types": {k: self.device_types[k].dump() for k in self.device_types}
+        }
+
+    def dump_devices(self):
+        return {
+            "devices": {k: self.devices[k].dump() for k in self.devices},
+        }
+
+    def dump_groups(self):
+        return {
+            "groups": {k: self.groups[k].dump() for k in self.groups},
+        }
+
+    def dump_users(self):
+        return {
+            "users": {k: self.users[k].dump() for k in self.users},
+        }
+
+    def dump_workers(self):
+        return {
+            "workers": {k: self.workers[k].dump() for k in self.workers},
+        }
+
+
+class ConfigFile:
+    def __init__(self, filepath):
+        self.filepath = filepath
+
+    @property
+    def filepath(self):
+        return self._filepath
+
+    @filepath.setter
+    def filepath(self, value):
+        if not isinstance(value, Path):
+            raise ValueError("filepath must be a pathlib.Path object!")
+        self._filepath = value.resolve()
+
+    def is_yaml_file(self):
+        with contextlib.suppress(AttributeError):
+            if self.filepath.suffix == ".yaml":
+                return True
+        return False
+
+    def is_dir(self):
+        """Treat non yaml file as a directory"""
+        if self.is_yaml_file():
+            return False
+        return True
+
+    @property
+    def base_dir(self):
+        base_dir = self.filepath
+        if self.is_yaml_file():
+            base_dir = (self.filepath / ".." / self.filepath.stem).resolve()
+        return base_dir
+
+    def write(self, filename, data):
+        print(f"{colors.yellow}> {filename}{colors.reset}")
+        filename.write_text(ruamel.yaml.round_trip_dump(data), encoding="utf-8")
+
+    def load(self):
+        if self.is_yaml_file():
+            return ruamel.yaml.safe_load(self.filepath.read_text(encoding="utf-8"))
+        if self.is_dir():
+            data = {}
+            files = [*sorted(self.filepath.glob("*.yaml"))]
+            for _file in files:
+                _config = ruamel.yaml.safe_load(_file.read_text(encoding="utf-8"))
+                data.update(_config)
+            return data
+        return {}
+
+    def dump(self, lab):
+        if self.is_yaml_file():
+            self.write(self.filepath, lab.dump())
+        if self.is_dir():
+            self.write((self.base_dir / "groups.yaml"), lab.dump_groups())
+            self.write((self.base_dir / "users.yaml"), lab.dump_users())
+            self.write((self.base_dir / "device-types.yaml"), lab.dump_device_types())
+            self.write((self.base_dir / "workers.yaml"), lab.dump_workers())
+            self.write((self.base_dir / "devices.yaml"), lab.dump_devices())
+
 
 def configure_parser(parser, version):
     sub = parser.add_subparsers(dest="sub_sub_command", help="Sub commands")
     sub.required = True
 
     if version < (2022, 4):
         return
@@ -410,31 +528,63 @@
     )
     lab_apply.add_argument(
         "--resources",
         default=[],
         action="append",
         help="resources to sync",
     )
-    lab_apply.add_argument("config", type=Path, help="configuration file")
+    lab_apply.add_argument(
+        "--delete",
+        action="store_true",
+        default=False,
+        help="Delete resource that not found in config file",
+    )
+    lab_apply.add_argument(
+        "config",
+        type=Path,
+        help="Path to a single config file using '.yaml' extension or a directory containing a set of config files",
+    )
 
     # "import"
     lab_apply = sub.add_parser("import", help="import configuration")
-    lab_apply.add_argument("config", type=Path, help="configuration file")
+    lab_apply.add_argument(
+        "config",
+        type=Path,
+        help="Path to a single config file using '.yaml' extension or a directory containing a set of config files",
+    )
+
+    # validate
+    lab_validate = sub.add_parser("validate", help="validate configuration")
+    lab_validate.add_argument("config", type=Path, help="configuration file")
 
 
 def help_string():
     return "manage lab configuration"
 
 
+def validate(data: dict) -> bool:
+    try:
+        schemas.config_schema(data)
+        return True
+    except MultipleInvalid as exc:
+        print(str(exc))
+        print(f"{colors.red}Config invalid!{colors.reset}")
+        return False
+
+
 def handle_apply(proxy, options, config):
     if not options.resources:
         options.resources = ["devices", "device-types", "groups", "users", "workers"]
 
-    lab = Config(**ruamel.yaml.safe_load(options.config.read_text(encoding="utf-8")))
-    base = (options.config / ".." / options.config.stem).resolve()
+    config_file = ConfigFile(options.config)
+    data = config_file.load()
+    if not validate(data):
+        return 1
+    lab = Config(**data)
+    base = config_file.base_dir
 
     print(f"{colors.cyan}> groups{colors.reset}")
     if "groups" not in options.resources:
         print(f"  {colors.yellow}-> SKIP{colors.reset}")
     elif config["version"] >= (2023, 3):
         groups = proxy.auth.groups.list()
         for group in lab.groups.values():
@@ -463,14 +613,21 @@
                 for perm in missing:
                     print(f"      {colors.red}- {perm}{colors.reset}")
                     if not options.dry_run:
                         proxy.auth.groups.perms.delete(
                             group.name, perm.app, perm.model, perm.codename
                         )
 
+        if options.delete:
+            for group in groups:
+                if group not in lab.groups:
+                    print(f"  {colors.red}* {group}{colors.reset}")
+                    if not options.dry_run:
+                        proxy.auth.groups.delete(group)
+
     print(f"{colors.cyan}> users{colors.reset}")
     if "users" not in options.resources:
         print(f"  {colors.yellow}-> SKIP{colors.reset}")
     elif config["version"] >= (2023, 3):
         users = [user["username"] for user in proxy.auth.users.list()]
         for user in lab.users.values():
             if user.username in users:
@@ -536,14 +693,21 @@
                 for perm in missing:
                     print(f"      {colors.red}- {perm}{colors.reset}")
                     if not options.dry_run:
                         proxy.auth.users.perms.delete(
                             user.username, perm.app, perm.model, perm.codename
                         )
 
+        if options.delete:
+            for user in users:
+                if user not in lab.users:
+                    print(f"  {colors.red}* {user}{colors.reset}")
+                    if not options.dry_run:
+                        proxy.auth.users.delete(user)
+
     print(f"{colors.cyan}> device-types{colors.reset}")
     if "device-types" not in options.resources:
         print(f"  {colors.yellow}-> SKIP{colors.reset}")
     else:
         device_types = [dt["name"] for dt in proxy.scheduler.device_types.list(False)]
         for dt in lab.device_types.values():
             if dt.name in device_types:
@@ -637,39 +801,57 @@
                     print(f"    {colors.yellow}-> template{colors.reset}")
                     print_file_diff(template, dt.get_template(base))
                     if not options.dry_run:
                         proxy.scheduler.device_types.set_template(
                             dt.name, dt.get_template(base)
                         )
 
+        if options.delete:
+            for dt in device_types:
+                if dt not in lab.device_types:
+                    print(f"  {colors.red}* {dt}{colors.reset}")
+                    if not options.dry_run:
+                        # Hide the device type in the GUI.
+                        proxy.scheduler.device_types.update(
+                            dt,
+                            None,
+                            False,
+                            None,
+                            None,
+                            None,
+                            None,
+                        )
+
     print(f"{colors.cyan}> workers{colors.reset}")
     if "workers" not in options.resources:
         print(f"  {colors.yellow}-> SKIP{colors.reset}")
     else:
-        workers = proxy.scheduler.workers.list()
+        workers = proxy.scheduler.workers.list(True)
         for worker in lab.workers.values():
             if worker.hostname in workers:
                 print(f"  {colors.green}* {worker.hostname}{colors.reset}")
             else:
                 print(f"  {colors.yellow}* {worker.hostname}{colors.reset}")
                 if not options.dry_run:
                     proxy.scheduler.workers.add(
                         worker.hostname, worker.description, False
                     )
             data = proxy.scheduler.workers.show(worker.hostname)
+            # Active/Maintenance/Retired -> ACTIVE/MAINTENANCE/RETRIED for comparison.
+            data["health"] = data["health"].upper()
             diff = worker.diff(data)
             for name in diff:
                 print(
                     f"    {colors.yellow}-> {name}: '{data[name]}' => '{getattr(worker, name)}'{colors.reset}"
                 )
             if diff and not options.dry_run:
                 proxy.scheduler.workers.update(
                     worker.hostname,
                     worker.description if "description" in diff else None,
-                    None,
+                    worker.health if "health" in diff else None,
                     worker.job_limit if "job_limit" in diff else None,
                 )
 
             if not data["default_config"] or worker.get_config(base) is not None:
                 try:
                     wconfig = str(proxy.scheduler.workers.get_config(worker.hostname))
                 except xmlrpc.client.Fault as exc:
@@ -710,14 +892,21 @@
                     print(f"    {colors.yellow}-> env-dut{colors.reset}")
                     print_file_diff(wenv_dut, worker.get_env_dut(base))
                     if not options.dry_run:
                         proxy.scheduler.workers.set_env_dut(
                             worker.hostname, worker.get_env_dut(base)
                         )
 
+        if options.delete and config["version"] >= (2023, 5):
+            for worker in workers:
+                if worker not in lab.workers:
+                    print(f"  {colors.red}* {worker}{colors.reset}")
+                    if not options.dry_run:
+                        proxy.scheduler.workers.delete(worker)
+
     print(f"{colors.cyan}> devices{colors.reset}")
     if "devices" not in options.resources:
         print(f"  {colors.yellow}-> SKIP{colors.reset}")
     else:
         devices = [d["hostname"] for d in proxy.scheduler.devices.list(True)]
         for device in lab.devices.values():
             if device.hostname in devices:
@@ -732,14 +921,17 @@
                         None,
                         None,
                         None,
                         None,
                         device.description,
                     )
             data = proxy.scheduler.devices.show(device.hostname)
+            # Good/Unknow/Looping/Bad/Maintenance/Retired ->
+            # GOOD/UNKNOWN/LOOPING/BAD/MAINTENANCE/RETIRED for comparison
+            data["health"] = data["health"].upper()
             if config["version"] >= (2023, 3):
                 data["permissions"] = set(
                     [GroupDevicePermission(**p) for p in data.get("permissions", [])]
                 )
             diff = device.diff(data)
             device_diff = [n for n in diff if n not in ["tags", "permissions"]]
             if device_diff:
@@ -750,15 +942,15 @@
                 if not options.dry_run:
                     proxy.scheduler.devices.update(
                         device.hostname,
                         device.worker if "worker" in diff else None,
                         None,
                         None,
                         None,
-                        None,
+                        device.health if "health" in diff else None,
                         device.description if "description" in diff else None,
                         device.device_type if "device_type" in diff else None,
                     )
             if "tags" in diff:
                 print(f"    {colors.yellow}-> tags{colors.reset}")
                 missing = device.tags.difference(set(data["tags"]))
                 for tag in missing:
@@ -803,20 +995,30 @@
                 print(f"    {colors.yellow}-> dictionary{colors.reset}")
                 print_file_diff(ddict, device.get_dict(base))
                 if not options.dry_run:
                     proxy.scheduler.devices.set_dictionary(
                         device.hostname, device.get_dict(base)
                     )
 
+        if options.delete and config["version"] >= (2023, 5):
+            for device in devices:
+                if device not in lab.devices:
+                    print(f"  {colors.red}* {device}{colors.reset}")
+                    if not options.dry_run:
+                        proxy.scheduler.devices.delete(device)
+
     return 0
 
 
 def handle_import(proxy, options, config):
     lab = Config({}, {}, {}, {}, {})
-    base = (options.config / ".." / options.config.stem).resolve()
+
+    config_file = ConfigFile(options.config)
+    base = config_file.base_dir
+    base.mkdir(parents=True, exist_ok=True)
 
     if config["version"] >= (2023, 3):
         print(f"{colors.cyan}> groups{colors.reset}")
         groups = [grp for grp in proxy.auth.groups.list()]
         for grp in groups:
             print(f"  {colors.green}* {grp}{colors.reset}")
             data = proxy.auth.groups.show(grp)
@@ -858,15 +1060,15 @@
                     raise
                 template = None
             if template is not None:
                 print(f"  {colors.green}  -> template{colors.reset}")
                 lab.device_types[dt].set_template(base, template)
 
     print(f"{colors.cyan}> workers{colors.reset}")
-    workers = proxy.scheduler.workers.list()
+    workers = proxy.scheduler.workers.list(True)
     for worker in workers:
         print(f"  {colors.green}* {worker}{colors.reset}")
         data = proxy.scheduler.workers.show(worker)
         lab.workers[worker] = Worker.new(**data)
 
         if data["default_config"]:
             print(f"  {colors.green}  -> default config{colors.reset}")
@@ -919,19 +1121,28 @@
             if exc.faultCode != 404:
                 raise
             ddict = None
         if ddict is not None:
             print(f"  {colors.green}  -> dictionary{colors.reset}")
             lab.devices[device].set_dict(base, ddict)
 
-    print(f"{colors.yellow}> {options.config}{colors.reset}")
-    options.config.write_text(ruamel.yaml.round_trip_dump(lab.dump()), encoding="utf-8")
+    config_file.dump(lab)
 
     return 0
 
 
+def handle_validate(proxy, options, config):
+    config_file = ConfigFile(options.config)
+    data = config_file.load()
+    if validate(data):
+        print(f"{colors.green}Config valid.{colors.reset}")
+        return 0
+    return 1
+
+
 def handle(proxy, options, config):
     handlers = {
         "apply": handle_apply,
         "import": handle_import,
+        "validate": handle_validate,
     }
     return handlers[options.sub_sub_command](proxy, options, config)
```

### Comparing `lavacli-1.9/lavacli/commands/results.py` & `lavacli-2.0/lavacli/commands/results.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.9/lavacli/commands/system.py` & `lavacli-2.0/lavacli/commands/system.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.9/lavacli/commands/tags.py` & `lavacli-2.0/lavacli/commands/tags.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.9/lavacli/commands/users.py` & `lavacli-2.0/lavacli/commands/users.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.9/lavacli/commands/utils.py` & `lavacli-2.0/lavacli/commands/utils.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.9/lavacli/commands/workers.py` & `lavacli-2.0/lavacli/commands/workers.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.9/lavacli/utils.py` & `lavacli-2.0/lavacli/utils.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.9/lavacli.egg-info/PKG-INFO` & `lavacli-2.0/lavacli.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: lavacli
-Version: 1.9
+Version: 2.0
 Summary: LAVA XML-RPC command line interface
-Home-page: https://git.lavasoftware.org/lava/lavacli
+Home-page: https://gitlab.com/lava/lavacli
 Author: Rémi Duraffort
 Author-email: remi.duraffort@linaro.org
 License: AGPLv3+
-Project-URL: Bug Tracker, https://git.lavasoftware.org/lava/lavacli/issues/
-Project-URL: Documentation, https://docs.lavasoftware.org/lavacli/
-Project-URL: Source Code, https://git.lavasoftware.org/lava/lavacli/
+Project-URL: Bug Tracker, https://gitlab.com/lava/lavacli/issues/
+Project-URL: Source Code, https://gitlab.com/lava/lavacli/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `lavacli-1.9/lavacli.egg-info/SOURCES.txt` & `lavacli-2.0/lavacli.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 doc/index.rst
 doc/install.rst
 doc/usage.rst
 lavacli/__about__.py
 lavacli/__init__.py
 lavacli/__main__.py
 lavacli/colors.py
+lavacli/schemas.py
 lavacli/utils.py
 lavacli.egg-info/PKG-INFO
 lavacli.egg-info/SOURCES.txt
 lavacli.egg-info/dependency_links.txt
 lavacli.egg-info/entry_points.txt
 lavacli.egg-info/requires.txt
 lavacli.egg-info/top_level.txt
@@ -46,11 +47,12 @@
 tests/test_events.py
 tests/test_helpers.py
 tests/test_identities.py
 tests/test_jobs.py
 tests/test_lab.py
 tests/test_lavacli.py
 tests/test_results.py
+tests/test_schemas.py
 tests/test_system.py
 tests/test_tags.py
 tests/test_users.py
 tests/test_workers.py
```

### Comparing `lavacli-1.9/setup.py` & `lavacli-2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,17 +30,16 @@
     version=metadata["__version__"],
     description=metadata["__description__"],
     author=metadata["__author__"],
     author_email=metadata["__author_email__"],
     license=metadata["__license__"],
     url=metadata["__url__"],
     project_urls={
-        "Bug Tracker": "https://git.lavasoftware.org/lava/lavacli/issues/",
-        "Documentation": "https://docs.lavasoftware.org/lavacli/",
-        "Source Code": "https://git.lavasoftware.org/lava/lavacli/",
+        "Bug Tracker": "https://gitlab.com/lava/lavacli/issues/",
+        "Source Code": "https://gitlab.com/lava/lavacli/",
     },
     python_requires=">=3.7",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
@@ -52,12 +51,12 @@
         "Programming Language :: Python :: 3 :: Only",
         "Topic :: Communications",
         "Topic :: Software Development :: Testing",
         "Topic :: System :: Networking",
     ],
     packages=["lavacli", "lavacli.commands"],
     entry_points={"console_scripts": ["lavacli = lavacli:main"]},
-    install_requires=["aiohttp", "jinja2", "requests", "ruamel.yaml"],
+    install_requires=["aiohttp", "jinja2", "requests", "ruamel.yaml", "voluptuous"],
     setup_requires=[],
     tests_require=["pytest", "pytest-runner"],
     zip_safe=True,
 )
```

### Comparing `lavacli-1.9/share/lavacli.yaml` & `lavacli-2.0/share/lavacli.yaml`

 * *Files identical despite different names*

### Comparing `lavacli-1.9/tests/conftest.py` & `lavacli-2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.9/tests/test_aliases.py` & `lavacli-2.0/tests/test_aliases.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.9/tests/test_device_types.py` & `lavacli-2.0/tests/test_device_types.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.9/tests/test_devices.py` & `lavacli-2.0/tests/test_devices.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.9/tests/test_events.py` & `lavacli-2.0/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.9/tests/test_helpers.py` & `lavacli-2.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.9/tests/test_identities.py` & `lavacli-2.0/tests/test_identities.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.9/tests/test_jobs.py` & `lavacli-2.0/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.9/tests/test_lab.py` & `lavacli-2.0/tests/test_lab.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import sys
 import xmlrpc.client
 
 import pytest
 import ruamel.yaml
 
 from lavacli import main
+from lavacli.commands.lab import ConfigFile
+from lavacli.utils import safe_yaml
 
 
 @pytest.fixture
 def mock_get():
     class GetData:
         def __init__(self):
             self.system_version_2023_2 = {
@@ -17,14 +19,19 @@
                 "ret": 2023.2,
             }
             self.system_version_2023_3 = {
                 "request": "system.version",
                 "args": (),
                 "ret": 2023.3,
             }
+            self.system_version_2023_05 = {
+                "request": "system.version",
+                "args": (),
+                "ret": 2023.05,
+            }
             self.auth_groups_list_empty = {
                 "request": "auth.groups.list",
                 "args": (),
                 "ret": [],
             }
             self.auth_groups_list = {
                 "request": "auth.groups.list",
@@ -283,20 +290,25 @@
             self.scheduler_device_types_get_template_qemu = {
                 "request": "scheduler.device_types.get_template",
                 "args": ("qemu",),
                 "ret": "template content",
             }
             self.scheduler_workers_list_empty = {
                 "request": "scheduler.workers.list",
-                "args": (),
+                "args": (True,),
                 "ret": [],
             }
             self.scheduler_workers_list = {
                 "request": "scheduler.workers.list",
-                "args": (),
+                "args": (True,),
+                "ret": ["worker01", "worker02"],
+            }
+            self.scheduler_workers_list_all = {
+                "request": "scheduler.workers.list",
+                "args": (True,),
                 "ret": ["worker01", "worker02"],
             }
             self.scheduler_workers_show_worker01 = {
                 "request": "scheduler.workers.show",
                 "args": ("worker01",),
                 "ret": {
                     "hostname": "worker01",
@@ -307,14 +319,30 @@
                     "job_limit": 0,
                     "version": "2023.03",
                     "default_config": True,
                     "default_env": True,
                     "default_env_dut": True,
                 },
             }
+            self.scheduler_workers_show_retired_worker01 = {
+                "request": "scheduler.workers.show",
+                "args": ("worker01",),
+                "ret": {
+                    "hostname": "worker01",
+                    "description": "",
+                    "state": "Online",
+                    "health": "Retired",
+                    "devices": ["docker-01", "qemu-01"],
+                    "job_limit": 0,
+                    "version": "2023.03",
+                    "default_config": True,
+                    "default_env": True,
+                    "default_env_dut": True,
+                },
+            }
             self.scheduler_workers_show_worker01_custom_config = {
                 "request": "scheduler.workers.show",
                 "args": ("worker01",),
                 "ret": {
                     "hostname": "worker01",
                     "description": "",
                     "state": "Online",
@@ -509,14 +537,31 @@
                     "pipeline": True,
                     "has_device_dict": True,
                     "worker": "worker01",
                     "current_job": None,
                     "tags": [],
                 },
             }
+            self.scheduler_devices_show_retired_qemu_01 = {
+                "request": "scheduler.devices.show",
+                "args": ("qemu-01",),
+                "ret": {
+                    "hostname": "qemu-01",
+                    "device_type": "qemu",
+                    "health": "Retired",
+                    "state": "Idle",
+                    "health_job": True,
+                    "description": "Created automatically by LAVA.",
+                    "pipeline": True,
+                    "has_device_dict": True,
+                    "worker": "worker01",
+                    "current_job": None,
+                    "tags": [],
+                },
+            }
             self.scheduler_devices_get_dictionary_qemu_01 = {
                 "request": "scheduler.devices.get_dictionary",
                 "args": ("qemu-01",),
                 "ret": "yaml_dict",
             }
             self.scheduler_devices_show_qemu_02 = {
                 "request": "scheduler.devices.show",
@@ -571,14 +616,19 @@
     class PostData:
         def __init__(self):
             self.auth_groups_add_group3 = {
                 "request": "auth.groups.add",
                 "args": ("group3",),
                 "ret": None,
             }
+            self.auth_groups_delete_group2 = {
+                "request": "auth.groups.delete",
+                "args": ("group2",),
+                "ret": None,
+            }
             self.auth_groups_perms_add_group1 = {
                 "request": "auth.groups.perms.add",
                 "args": ("group1", "auth", "user", "delete_user"),
                 "ret": None,
             }
             self.auth_groups_perms_delete_group1 = {
                 "request": "auth.groups.perms.delete",
@@ -591,14 +641,19 @@
                 "ret": None,
             }
             self.auth_users_add_user3_ldap = {
                 "request": "auth.users.add",
                 "args": ("user3", None, None, None, True, False, False, True),
                 "ret": None,
             }
+            self.auth_users_delete_user2 = {
+                "request": "auth.users.delete",
+                "args": ("user2",),
+                "ret": None,
+            }
             self.auth_users_perms_add_user1 = {
                 "request": "auth.users.perms.add",
                 "args": ("user1", "lava_scheduler_app", "device", "delete_device"),
                 "ret": None,
             }
             self.auth_users_update_user1 = {
                 "request": "auth.users.update",
@@ -626,14 +681,19 @@
                 "ret": None,
             }
             self.scheduler_device_types_add_bbb = {
                 "request": "scheduler.device_types.add",
                 "args": ("bbb", None, True, None, 24, "hours"),
                 "ret": None,
             }
+            self.scheduler_device_types_hide_qemu = {
+                "request": "scheduler.device_types.update",
+                "args": ("qemu", None, False, None, None, None, None),
+                "ret": None,
+            }
             self.scheduler_device_types_update_docker = {
                 "request": "scheduler.device_types.update",
                 "args": ("docker", "new", False, None, 12, "jobs", True),
                 "ret": None,
             }
             self.scheduler_device_types_set_health_check_docker = {
                 "request": "scheduler.device_types.set_health_check",
@@ -656,19 +716,34 @@
                 "ret": None,
             }
             self.scheduler_workers_add_worker03 = {
                 "request": "scheduler.workers.add",
                 "args": ("worker03", "", False),
                 "ret": None,
             }
+            self.scheduler_workers_delete_worker02 = {
+                "request": "scheduler.workers.delete",
+                "args": ("worker02",),
+                "ret": None,
+            }
             self.scheduler_workers_update_worker01 = {
                 "request": "scheduler.workers.update",
                 "args": ("worker01", "new", None, 10),
                 "ret": None,
             }
+            self.scheduler_workers_retire_worker01 = {
+                "request": "scheduler.workers.update",
+                "args": ("worker01", None, "RETIRED", None),
+                "ret": None,
+            }
+            self.scheduler_workers_unretire_worker01 = {
+                "request": "scheduler.workers.update",
+                "args": ("worker01", None, "ACTIVE", None),
+                "ret": None,
+            }
             self.scheduler_workers_set_config_worker01 = {
                 "request": "scheduler.workers.set_config",
                 "args": ("worker01", "local config content"),
                 "ret": True,
             }
             self.scheduler_workers_set_env_worker01 = {
                 "request": "scheduler.workers.set_env",
@@ -690,28 +765,61 @@
                     None,
                     None,
                     None,
                     "qemu03",
                 ),
                 "ret": None,
             }
+            self.scheduler_devices_delete_qemu_02 = {
+                "request": "scheduler.devices.delete",
+                "args": ("qemu-02",),
+                "ret": None,
+            }
             self.scheduler_devices_update_qemu_01 = {
                 "request": "scheduler.devices.update",
                 "args": (
                     "qemu-01",
                     "worker02",
                     None,
                     None,
                     None,
                     None,
                     "qemu01",
                     "qemu-aarch64",
                 ),
                 "ret": None,
             }
+            self.scheduler_devices_retire_qemu_01 = {
+                "request": "scheduler.devices.update",
+                "args": (
+                    "qemu-01",
+                    None,
+                    None,
+                    None,
+                    None,
+                    "RETIRED",
+                    None,
+                    None,
+                ),
+                "ret": None,
+            }
+            self.scheduler_devices_unretire_qemu_01 = {
+                "request": "scheduler.devices.update",
+                "args": (
+                    "qemu-01",
+                    None,
+                    None,
+                    None,
+                    None,
+                    "UNKNOWN",
+                    None,
+                    None,
+                ),
+                "ret": None,
+            }
             self.scheduler_devices_set_dictionary_docker_01 = {
                 "request": "scheduler.devices.set_dictionary",
                 "args": ("docker-01", "new_yaml_dict"),
                 "ret": False,
             }
             self.scheduler_devices_tags_add_docker_01 = {
                 "request": "scheduler.devices.tags.add",
@@ -739,14 +847,19 @@
 
 @pytest.fixture
 def config_file(tmp_path):
     return tmp_path / "lab.yaml"
 
 
 @pytest.fixture
+def config_dir(tmp_path):
+    return tmp_path / "lab"
+
+
+@pytest.fixture
 def config_def():
     return """device_types:
   docker:
     permissions:
     - name: change_devicetype
       group: group1
   qemu:
@@ -856,15 +969,17 @@
     assert capsys.readouterr()[1] == ""
 
     assert config_file.exists()
     yaml = ruamel.yaml.YAML(typ="safe")
     assert yaml.load(config_file.read_text()) == yaml.load(expected_def)
 
 
-def test_lab_import_all(setup, monkeypatch, capsys, config_file, config_def, mock_get):
+def test_lab_import_config_file(
+    setup, monkeypatch, capsys, config_file, config_def, mock_get
+):
     monkeypatch.setattr(sys, "argv", ["lavacli", "lab", "import", str(config_file)])
     monkeypatch.setattr(
         xmlrpc.client.ServerProxy,
         "data",
         [
             mock_get.system_version_2023_3,
             mock_get.auth_groups_list,
@@ -874,15 +989,15 @@
             mock_get.auth_users_show_user1,
             mock_get.auth_users_show_user2,
             mock_get.scheduler_device_types_list,
             mock_get.scheduler_device_types_show_docker,
             mock_get.scheduler_device_types_get_health_check_docker,
             mock_get.scheduler_device_types_show_qemu,
             mock_get.scheduler_device_types_get_health_check_qemu,
-            mock_get.scheduler_workers_list,
+            mock_get.scheduler_workers_list_all,
             mock_get.scheduler_workers_show_worker01,
             mock_get.scheduler_workers_show_worker02,
             mock_get.scheduler_devices_list,
             mock_get.scheduler_devices_show_docker_01,
             mock_get.scheduler_devices_get_dictionary_docker_01,
             mock_get.scheduler_devices_show_docker_02,
             mock_get.scheduler_devices_get_dictionary_docker_02,
@@ -906,14 +1021,70 @@
     assert (config_dir / "devices/qemu-01.jinja2").exists()
     assert (config_dir / "devices/qemu-02.jinja2").exists()
     assert not (config_dir / "device-types/docker.jinja2").exists()
     assert not (config_dir / "device-types/qemu.jinja2").exists()
     assert (config_dir / "health-checks/docker.yaml").exists()
     assert (config_dir / "health-checks/qemu.yaml").exists()
 
+    config = ConfigFile(config_file)
+    assert config.is_yaml_file()
+    assert not config.is_dir()
+    assert config.load() == safe_yaml.load(config_def)
+
+
+def test_lab_import_config_dir(
+    setup, monkeypatch, capsys, config_dir, config_def, mock_get
+):
+    monkeypatch.setattr(sys, "argv", ["lavacli", "lab", "import", str(config_dir)])
+    monkeypatch.setattr(
+        xmlrpc.client.ServerProxy,
+        "data",
+        [
+            mock_get.system_version_2023_3,
+            mock_get.auth_groups_list,
+            mock_get.auth_groups_show_group1,
+            mock_get.auth_groups_show_group2,
+            mock_get.auth_users_list,
+            mock_get.auth_users_show_user1,
+            mock_get.auth_users_show_user2,
+            mock_get.scheduler_device_types_list,
+            mock_get.scheduler_device_types_show_docker,
+            mock_get.scheduler_device_types_get_health_check_docker,
+            mock_get.scheduler_device_types_show_qemu,
+            mock_get.scheduler_device_types_get_health_check_qemu,
+            mock_get.scheduler_workers_list,
+            mock_get.scheduler_workers_show_worker01,
+            mock_get.scheduler_workers_show_worker02,
+            mock_get.scheduler_devices_list,
+            mock_get.scheduler_devices_show_docker_01,
+            mock_get.scheduler_devices_get_dictionary_docker_01,
+            mock_get.scheduler_devices_show_docker_02,
+            mock_get.scheduler_devices_get_dictionary_docker_02,
+            mock_get.scheduler_devices_show_qemu_01,
+            mock_get.scheduler_devices_get_dictionary_qemu_01,
+            mock_get.scheduler_devices_show_qemu_02,
+            mock_get.scheduler_devices_get_dictionary_qemu_02,
+        ],
+    )
+
+    assert main() == 0
+    assert capsys.readouterr()[1] == ""
+
+    assert config_dir.exists()
+    assert (config_dir / "device-types.yaml").exists()
+    assert (config_dir / "devices.yaml").exists()
+    assert (config_dir / "groups.yaml").exists()
+    assert (config_dir / "users.yaml").exists()
+    assert (config_dir / "workers.yaml").exists()
+
+    config = ConfigFile(config_dir)
+    assert config.is_dir()
+    assert not config.is_yaml_file()
+    assert config.load() == safe_yaml.load(config_def)
+
 
 def test_lab_import_custom_template(setup, monkeypatch, capsys, config_file, mock_get):
     monkeypatch.setattr(sys, "argv", ["lavacli", "lab", "import", str(config_file)])
     monkeypatch.setattr(
         xmlrpc.client.ServerProxy,
         "data",
         [
@@ -1039,14 +1210,53 @@
 
     assert main() == 0
     out, err = capsys.readouterr()
     assert out == expected_out
     assert err == ""
 
 
+def test_lab_apply_groups_delete(
+    setup, monkeypatch, capsys, config_file, config_def, mock_get, mock_post
+):
+    monkeypatch.setattr(
+        sys,
+        "argv",
+        [
+            "lavacli",
+            "lab",
+            "apply",
+            "--resource",
+            "groups",
+            "--delete",
+            str(config_file),
+        ],
+    )
+    monkeypatch.setattr(
+        xmlrpc.client.ServerProxy,
+        "data",
+        [
+            mock_get.system_version_2023_3,
+            mock_get.auth_groups_list,
+            mock_get.auth_groups_show_group1,
+            mock_post.auth_groups_delete_group2,
+        ],
+    )
+
+    data = safe_yaml.load(config_def)
+    del data["groups"]["group2"]
+    del data["users"]["user2"]["groups"]
+    with open(config_file, "w") as f:
+        safe_yaml.dump(data, f)
+
+    assert main() == 0
+    out, err = capsys.readouterr()
+    assert "  \x1b[91m* group2\x1b[0m\n" in out
+    assert err == ""
+
+
 def test_lab_apply_groups_perms_add(
     setup, monkeypatch, capsys, config_file, config_def, mock_get, mock_post
 ):
     monkeypatch.setattr(
         sys,
         "argv",
         ["lavacli", "lab", "apply", "--resource", "groups", str(config_file)],
@@ -1182,14 +1392,15 @@
             mock_get.auth_users_show_user3,
         ],
     )
 
     yaml = ruamel.yaml.YAML(typ="safe")
     data = yaml.load(config_def)
     data["users"]["user3"] = {"groups": ["group3"], "permissions": []}
+    data["groups"]["group3"] = None
     with open(config_file, "w") as f:
         yaml.dump(data, f)
     expected_out = "\x1b[36m> groups\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> users\x1b[0m\n  \x1b[32m* user1\x1b[0m\n  \x1b[32m* user2\x1b[0m\n  \x1b[33m* user3\x1b[0m\n\x1b[36m> device-types\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> workers\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> devices\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n"
 
     assert main() == 0
     out, err = capsys.readouterr()
     assert out == expected_out
@@ -1216,24 +1427,63 @@
             mock_get.auth_users_show_user3_ldap,
         ],
     )
 
     yaml = ruamel.yaml.YAML(typ="safe")
     data = yaml.load(config_def)
     data["users"]["user3"] = {"ldap": True, "groups": ["group3"], "permissions": []}
+    data["groups"]["group3"] = None
     with open(config_file, "w") as f:
         yaml.dump(data, f)
     expected_out = "\x1b[36m> groups\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> users\x1b[0m\n  \x1b[32m* user1\x1b[0m\n  \x1b[32m* user2\x1b[0m\n  \x1b[33m* user3\x1b[0m\n\x1b[36m> device-types\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> workers\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> devices\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n"
 
     assert main() == 0
     out, err = capsys.readouterr()
     assert out == expected_out
     assert err == ""
 
 
+def test_lab_apply_users_delete(
+    setup, monkeypatch, capsys, config_file, config_def, mock_get, mock_post
+):
+    monkeypatch.setattr(
+        sys,
+        "argv",
+        [
+            "lavacli",
+            "lab",
+            "apply",
+            "--resource",
+            "users",
+            "--delete",
+            str(config_file),
+        ],
+    )
+    monkeypatch.setattr(
+        xmlrpc.client.ServerProxy,
+        "data",
+        [
+            mock_get.system_version_2023_3,
+            mock_get.auth_users_list,
+            mock_get.auth_users_show_user1,
+            mock_post.auth_users_delete_user2,
+        ],
+    )
+
+    data = safe_yaml.load(config_def)
+    del data["users"]["user2"]
+    with open(config_file, "w") as f:
+        safe_yaml.dump(data, f)
+
+    assert main() == 0
+    out, err = capsys.readouterr()
+    assert "  \x1b[91m* user2\x1b[0m\n" in out
+    assert err == ""
+
+
 def test_lab_apply_users_update(
     setup, monkeypatch, capsys, config_file, config_def, mock_get, mock_post
 ):
     monkeypatch.setattr(
         sys,
         "argv",
         ["lavacli", "lab", "apply", "--resource", "users", str(config_file)],
@@ -1476,14 +1726,56 @@
 
     assert main() == 0
     out, err = capsys.readouterr()
     assert out == expected_out
     assert err == ""
 
 
+def test_lab_apply_dt_hide(
+    setup, monkeypatch, capsys, config_file, config_def, mock_get, mock_post, dt_hc
+):
+    monkeypatch.setattr(
+        sys,
+        "argv",
+        [
+            "lavacli",
+            "lab",
+            "apply",
+            "--resource",
+            "device-types",
+            "--delete",
+            str(config_file),
+        ],
+    )
+    monkeypatch.setattr(
+        xmlrpc.client.ServerProxy,
+        "data",
+        [
+            mock_get.system_version_2023_3,
+            mock_get.scheduler_device_types_list,
+            mock_get.scheduler_device_types_show_docker,
+            mock_get.scheduler_device_types_get_health_check_docker,
+            mock_post.scheduler_device_types_hide_qemu,
+        ],
+    )
+
+    data = safe_yaml.load(config_def)
+    del data["device_types"]["qemu"]
+    # delete devices need the device type.
+    del data["devices"]["qemu-01"]
+    del data["devices"]["qemu-02"]
+    with open(config_file, "w") as f:
+        safe_yaml.dump(data, f)
+
+    assert main() == 0
+    out, err = capsys.readouterr()
+    assert "  \x1b[91m* qemu\x1b[0m\n" in out
+    assert err == ""
+
+
 def test_lab_apply_dt_update(
     setup, monkeypatch, capsys, config_file, config_def, mock_get, mock_post, dt_hc
 ):
     monkeypatch.setattr(
         sys,
         "argv",
         ["lavacli", "lab", "apply", "--resource", "device-types", str(config_file)],
@@ -1753,15 +2045,15 @@
         ["lavacli", "lab", "apply", "--resource", "workers", str(config_file)],
     )
     monkeypatch.setattr(
         xmlrpc.client.ServerProxy,
         "data",
         [
             mock_get.system_version_2023_3,
-            mock_get.scheduler_workers_list,
+            mock_get.scheduler_workers_list_all,
             mock_get.scheduler_workers_show_worker01,
             mock_get.scheduler_workers_show_worker02,
         ],
     )
 
     config_file.write_text(config_def, encoding="utf-8")
     expected_out = "\x1b[36m> groups\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> users\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> device-types\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> workers\x1b[0m\n  \x1b[32m* worker01\x1b[0m\n  \x1b[32m* worker02\x1b[0m\n\x1b[36m> devices\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n"
@@ -1781,15 +2073,15 @@
         ["lavacli", "lab", "apply", "--resource", "workers", str(config_file)],
     )
     monkeypatch.setattr(
         xmlrpc.client.ServerProxy,
         "data",
         [
             mock_get.system_version_2023_3,
-            mock_get.scheduler_workers_list,
+            mock_get.scheduler_workers_list_all,
             mock_get.scheduler_workers_show_worker01,
             mock_get.scheduler_workers_show_worker02,
             mock_post.scheduler_workers_add_worker03,
             mock_get.scheduler_workers_show_worker03,
         ],
     )
 
@@ -1802,28 +2094,69 @@
 
     assert main() == 0
     out, err = capsys.readouterr()
     assert out == expected_out
     assert err == ""
 
 
+def test_lab_apply_workers_delete(
+    setup, monkeypatch, capsys, config_file, config_def, mock_get, mock_post
+):
+    monkeypatch.setattr(
+        sys,
+        "argv",
+        [
+            "lavacli",
+            "lab",
+            "apply",
+            "--resource",
+            "workers",
+            "--delete",
+            str(config_file),
+        ],
+    )
+    monkeypatch.setattr(
+        xmlrpc.client.ServerProxy,
+        "data",
+        [
+            mock_get.system_version_2023_05,
+            mock_get.scheduler_workers_list_all,
+            mock_get.scheduler_workers_show_worker01,
+            mock_post.scheduler_workers_delete_worker02,
+        ],
+    )
+
+    data = safe_yaml.load(config_def)
+    del data["workers"]["worker02"]
+    # delete devices need the worker.
+    del data["devices"]["docker-02"]
+    del data["devices"]["qemu-02"]
+    with open(config_file, "w") as f:
+        safe_yaml.dump(data, f)
+
+    assert main() == 0
+    out, err = capsys.readouterr()
+    assert "  \x1b[91m* worker02\x1b[0m\n" in out
+    assert err == ""
+
+
 def test_lab_apply_workers_update(
     setup, monkeypatch, capsys, config_file, config_def, mock_get, mock_post
 ):
     monkeypatch.setattr(
         sys,
         "argv",
         ["lavacli", "lab", "apply", "--resource", "workers", str(config_file)],
     )
     monkeypatch.setattr(
         xmlrpc.client.ServerProxy,
         "data",
         [
             mock_get.system_version_2023_3,
-            mock_get.scheduler_workers_list,
+            mock_get.scheduler_workers_list_all,
             mock_get.scheduler_workers_show_worker01,
             mock_post.scheduler_workers_update_worker01,
             mock_get.scheduler_workers_show_worker02,
         ],
     )
 
     yaml = ruamel.yaml.YAML(typ="safe")
@@ -1838,14 +2171,80 @@
 
     assert main() == 0
     out, err = capsys.readouterr()
     assert out == expected_out
     assert err == ""
 
 
+def test_lab_apply_workers_retire(
+    setup, monkeypatch, capsys, config_file, config_def, mock_get, mock_post
+):
+    monkeypatch.setattr(
+        sys,
+        "argv",
+        ["lavacli", "lab", "apply", "--resource", "workers", str(config_file)],
+    )
+    monkeypatch.setattr(
+        xmlrpc.client.ServerProxy,
+        "data",
+        [
+            mock_get.system_version_2023_3,
+            mock_get.scheduler_workers_list_all,
+            mock_get.scheduler_workers_show_worker01,
+            mock_post.scheduler_workers_retire_worker01,
+            mock_get.scheduler_workers_show_worker02,
+        ],
+    )
+
+    data = safe_yaml.load(config_def)
+    if data["workers"]["worker01"] is None:
+        data["workers"]["worker01"] = {}
+    data["workers"]["worker01"]["retire"] = True
+    with open(config_file, "w") as f:
+        safe_yaml.dump(data, f)
+
+    assert main() == 0
+    out, err = capsys.readouterr()
+    assert "    \x1b[33m-> health: 'ACTIVE' => 'RETIRED'\x1b[0m\n" in out
+    assert err == ""
+
+
+def test_lab_apply_workers_unretire(
+    setup, monkeypatch, capsys, config_file, config_def, mock_get, mock_post
+):
+    monkeypatch.setattr(
+        sys,
+        "argv",
+        ["lavacli", "lab", "apply", "--resource", "workers", str(config_file)],
+    )
+    monkeypatch.setattr(
+        xmlrpc.client.ServerProxy,
+        "data",
+        [
+            mock_get.system_version_2023_3,
+            mock_get.scheduler_workers_list_all,
+            mock_get.scheduler_workers_show_retired_worker01,
+            mock_post.scheduler_workers_unretire_worker01,
+            mock_get.scheduler_workers_show_worker02,
+        ],
+    )
+
+    data = safe_yaml.load(config_def)
+    if data["workers"]["worker01"] is None:
+        data["workers"]["worker01"] = {}
+    data["workers"]["worker01"]["retire"] = False
+    with open(config_file, "w") as f:
+        safe_yaml.dump(data, f)
+
+    assert main() == 0
+    out, err = capsys.readouterr()
+    assert "    \x1b[33m-> health: 'RETIRED' => 'ACTIVE'\x1b[0m\n" in out
+    assert err == ""
+
+
 @pytest.fixture
 def worker_config(config_file):
     config_dir = config_file.parent / config_file.name.split(".")[0]
     worker_dir = config_dir / "workers/worker01"
     worker_dir.mkdir(parents=True, exist_ok=True)
     return worker_dir
 
@@ -1866,15 +2265,15 @@
         ["lavacli", "lab", "apply", "--resource", "workers", str(config_file)],
     )
     monkeypatch.setattr(
         xmlrpc.client.ServerProxy,
         "data",
         [
             mock_get.system_version_2023_3,
-            mock_get.scheduler_workers_list,
+            mock_get.scheduler_workers_list_all,
             mock_get.scheduler_workers_show_worker01_custom_config,
             mock_get.scheduler_workers_get_config_worker01,
             mock_post.scheduler_workers_set_config_worker01,
             mock_get.scheduler_workers_show_worker02,
         ],
     )
 
@@ -1906,15 +2305,15 @@
         ["lavacli", "lab", "apply", "--resource", "workers", str(config_file)],
     )
     monkeypatch.setattr(
         xmlrpc.client.ServerProxy,
         "data",
         [
             mock_get.system_version_2023_3,
-            mock_get.scheduler_workers_list,
+            mock_get.scheduler_workers_list_all,
             mock_get.scheduler_workers_show_worker01_custom_env,
             mock_get.scheduler_workers_get_env_worker01,
             mock_post.scheduler_workers_set_env_worker01,
             mock_get.scheduler_workers_show_worker02,
         ],
     )
 
@@ -1944,15 +2343,15 @@
         ["lavacli", "lab", "apply", "--resource", "workers", str(config_file)],
     )
     monkeypatch.setattr(
         xmlrpc.client.ServerProxy,
         "data",
         [
             mock_get.system_version_2023_3,
-            mock_get.scheduler_workers_list,
+            mock_get.scheduler_workers_list_all,
             mock_get.scheduler_workers_show_worker01_custom_env_dut,
             mock_get.scheduler_workers_get_env_dut_worker01,
             mock_post.scheduler_workers_set_env_dut_worker01,
             mock_get.scheduler_workers_show_worker02,
         ],
     )
 
@@ -2063,14 +2462,64 @@
 
     assert main() == 0
     out, err = capsys.readouterr()
     assert out == expected_out
     assert err == ""
 
 
+def test_lab_apply_devices_delete(
+    setup,
+    monkeypatch,
+    capsys,
+    config_file,
+    config_def,
+    mock_get,
+    mock_post,
+    device_dict,
+):
+    monkeypatch.setattr(
+        sys,
+        "argv",
+        [
+            "lavacli",
+            "lab",
+            "apply",
+            "--resource",
+            "devices",
+            "--delete",
+            str(config_file),
+        ],
+    )
+    monkeypatch.setattr(
+        xmlrpc.client.ServerProxy,
+        "data",
+        [
+            mock_get.system_version_2023_05,
+            mock_get.scheduler_devices_list,
+            mock_get.scheduler_devices_show_docker_01,
+            mock_get.scheduler_devices_get_dictionary_docker_01,
+            mock_get.scheduler_devices_show_docker_02,
+            mock_get.scheduler_devices_get_dictionary_docker_02,
+            mock_get.scheduler_devices_show_qemu_01,
+            mock_get.scheduler_devices_get_dictionary_qemu_01,
+            mock_post.scheduler_devices_delete_qemu_02,
+        ],
+    )
+
+    data = safe_yaml.load(config_def)
+    del data["devices"]["qemu-02"]
+    with open(config_file, "w") as f:
+        safe_yaml.dump(data, f)
+
+    assert main() == 0
+    out, err = capsys.readouterr()
+    assert "  \x1b[91m* qemu-02\x1b[0m\n" in out
+    assert err == ""
+
+
 def test_lab_apply_devices_update(
     setup,
     monkeypatch,
     capsys,
     config_file,
     config_def,
     mock_get,
@@ -2103,24 +2552,113 @@
     yaml = ruamel.yaml.YAML(typ="safe")
     data = yaml.load(config_def)
     data["devices"]["qemu-01"] = {
         "device_type": "qemu-aarch64",
         "worker": "worker02",
         "description": "qemu01",
     }
+    data["device_types"]["qemu-aarch64"] = None
     with open(config_file, "w") as f:
         yaml.dump(data, f)
     expected_out = "\x1b[36m> groups\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> users\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> device-types\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> workers\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> devices\x1b[0m\n  \x1b[32m* docker-01\x1b[0m\n  \x1b[32m* docker-02\x1b[0m\n  \x1b[32m* qemu-01\x1b[0m\n    \x1b[33m-> device_type: 'qemu' => 'qemu-aarch64'\x1b[0m\n    \x1b[33m-> worker: 'worker01' => 'worker02'\x1b[0m\n    \x1b[33m-> description: 'Created automatically by LAVA.' => 'qemu01'\x1b[0m\n  \x1b[32m* qemu-02\x1b[0m\n"
 
     assert main() == 0
     out, err = capsys.readouterr()
     assert out == expected_out
     assert err == ""
 
 
+def test_lab_apply_devices_retire(
+    setup,
+    monkeypatch,
+    capsys,
+    config_file,
+    config_def,
+    mock_get,
+    mock_post,
+    device_dict,
+):
+    monkeypatch.setattr(
+        sys,
+        "argv",
+        ["lavacli", "lab", "apply", "--resource", "devices", str(config_file)],
+    )
+    monkeypatch.setattr(
+        xmlrpc.client.ServerProxy,
+        "data",
+        [
+            mock_get.system_version_2023_3,
+            mock_get.scheduler_devices_list,
+            mock_get.scheduler_devices_show_docker_01,
+            mock_get.scheduler_devices_get_dictionary_docker_01,
+            mock_get.scheduler_devices_show_docker_02,
+            mock_get.scheduler_devices_get_dictionary_docker_02,
+            mock_get.scheduler_devices_show_qemu_01,
+            mock_post.scheduler_devices_retire_qemu_01,
+            mock_get.scheduler_devices_get_dictionary_qemu_01,
+            mock_get.scheduler_devices_show_qemu_02,
+            mock_get.scheduler_devices_get_dictionary_qemu_02,
+        ],
+    )
+
+    data = safe_yaml.load(config_def)
+    data["devices"]["qemu-01"]["retire"] = True
+    with open(config_file, "w") as f:
+        safe_yaml.dump(data, f)
+
+    assert main() == 0
+    out, err = capsys.readouterr()
+    assert "    \x1b[33m-> health: 'GOOD' => 'RETIRED'\x1b[0m\n" in out
+    assert err == ""
+
+
+def test_lab_apply_devices_unretire(
+    setup,
+    monkeypatch,
+    capsys,
+    config_file,
+    config_def,
+    mock_get,
+    mock_post,
+    device_dict,
+):
+    monkeypatch.setattr(
+        sys,
+        "argv",
+        ["lavacli", "lab", "apply", "--resource", "devices", str(config_file)],
+    )
+    monkeypatch.setattr(
+        xmlrpc.client.ServerProxy,
+        "data",
+        [
+            mock_get.system_version_2023_3,
+            mock_get.scheduler_devices_list,
+            mock_get.scheduler_devices_show_docker_01,
+            mock_get.scheduler_devices_get_dictionary_docker_01,
+            mock_get.scheduler_devices_show_docker_02,
+            mock_get.scheduler_devices_get_dictionary_docker_02,
+            mock_get.scheduler_devices_show_retired_qemu_01,
+            mock_post.scheduler_devices_unretire_qemu_01,
+            mock_get.scheduler_devices_get_dictionary_qemu_01,
+            mock_get.scheduler_devices_show_qemu_02,
+            mock_get.scheduler_devices_get_dictionary_qemu_02,
+        ],
+    )
+
+    data = safe_yaml.load(config_def)
+    data["devices"]["qemu-01"]["retire"] = False
+    with open(config_file, "w") as f:
+        safe_yaml.dump(data, f)
+
+    assert main() == 0
+    out, err = capsys.readouterr()
+    assert "    \x1b[33m-> health: 'RETIRED' => 'UNKNOWN'\x1b[0m\n" in out
+    assert err == ""
+
+
 def test_lab_apply_devices_set_dictionary(
     setup,
     monkeypatch,
     capsys,
     config_file,
     config_def,
     mock_get,
@@ -2451,7 +2989,31 @@
         yaml.dump(data, f)
     expected_out = "\x1b[36m> groups\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> users\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> device-types\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> workers\x1b[0m\n  \x1b[33m-> SKIP\x1b[0m\n\x1b[36m> devices\x1b[0m\n  \x1b[32m* docker-01\x1b[0m\n  \x1b[32m* docker-02\x1b[0m\n  \x1b[32m* qemu-01\x1b[0m\n  \x1b[32m* qemu-02\x1b[0m\n"
 
     assert main() == 0
     out, err = capsys.readouterr()
     assert out == expected_out
     assert err == ""
+
+
+class TestConfigFile:
+    def test_filepath_setter(self, tmp_path):
+        with pytest.raises(ValueError) as exc:
+            _config = ConfigFile("path_str")
+        assert str(exc.value) == "filepath must be a pathlib.Path object!"
+
+    def test_is_dir(self, tmp_path):
+        config = ConfigFile(tmp_path / "lab")
+        assert config.is_dir()
+
+    def test_is_yaml_file(self, tmp_path):
+        config = ConfigFile(tmp_path / "lab.yaml")
+        assert config.is_yaml_file()
+
+    def test_base_dir(self, tmp_path):
+        """
+        Test 'lab.yaml/../lab' is resolved to 'lab'. If not, 'lab.yaml'
+        will be created as an parent dir of 'lab' which leads to file
+        writing error.
+        """
+        config = ConfigFile(tmp_path / "lab.yaml")
+        assert str(config.base_dir) == str(config.filepath).split(".")[0]
```

### Comparing `lavacli-1.9/tests/test_lavacli.py` & `lavacli-2.0/tests/test_lavacli.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.9/tests/test_results.py` & `lavacli-2.0/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.9/tests/test_system.py` & `lavacli-2.0/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.9/tests/test_tags.py` & `lavacli-2.0/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.9/tests/test_users.py` & `lavacli-2.0/tests/test_users.py`

 * *Files identical despite different names*

### Comparing `lavacli-1.9/tests/test_workers.py` & `lavacli-2.0/tests/test_workers.py`

 * *Files identical despite different names*

