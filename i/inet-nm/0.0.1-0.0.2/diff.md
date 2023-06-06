# Comparing `tmp/inet-nm-0.0.1.tar.gz` & `tmp/inet-nm-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inet-nm-0.0.1.tar", last modified: Tue Jun  6 12:06:08 2023, max compression
+gzip compressed data, was "inet-nm-0.0.2.tar", last modified: Tue Jun  6 15:49:35 2023, max compression
```

## Comparing `inet-nm-0.0.1.tar` & `inet-nm-0.0.2.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxr-x   0 weiss     (1000) weiss     (1000)        0 2023-06-06 12:06:08.486105 inet-nm-0.0.1/
--rw-rw-r--   0 weiss     (1000) weiss     (1000)      590 2023-05-10 11:06:23.000000 inet-nm-0.0.1/.coveragerc
-drwxrwxr-x   0 weiss     (1000) weiss     (1000)        0 2023-06-06 12:06:08.466105 inet-nm-0.0.1/.github/
-drwxrwxr-x   0 weiss     (1000) weiss     (1000)        0 2023-06-06 12:06:08.470105 inet-nm-0.0.1/.github/workflows/
--rw-rw-r--   0 weiss     (1000) weiss     (1000)     3293 2023-06-06 11:53:39.000000 inet-nm-0.0.1/.github/workflows/ci.yml
--rw-rw-r--   0 weiss     (1000) weiss     (1000)      566 2023-05-10 11:06:23.000000 inet-nm-0.0.1/.gitignore
--rw-rw-r--   0 weiss     (1000) weiss     (1000)       55 2023-05-10 11:06:23.000000 inet-nm-0.0.1/.isort.cfg
--rw-rw-r--   0 weiss     (1000) weiss     (1000)     1670 2023-06-05 09:46:26.000000 inet-nm-0.0.1/.pre-commit-config.yaml
--rw-rw-r--   0 weiss     (1000) weiss     (1000)      530 2023-05-10 11:06:23.000000 inet-nm-0.0.1/.readthedocs.yml
--rw-rw-r--   0 weiss     (1000) weiss     (1000)       90 2023-05-10 11:06:23.000000 inet-nm-0.0.1/AUTHORS.md
--rw-rw-r--   0 weiss     (1000) weiss     (1000)      315 2023-06-06 11:38:40.000000 inet-nm-0.0.1/CHANGELOG.md
--rw-rw-r--   0 weiss     (1000) weiss     (1000)    10522 2023-06-05 11:48:42.000000 inet-nm-0.0.1/CONTRIBUTING.md
--rw-rw-r--   0 weiss     (1000) weiss     (1000)     1078 2023-05-10 11:06:23.000000 inet-nm-0.0.1/LICENSE.txt
--rw-rw-r--   0 weiss     (1000) weiss     (1000)    11330 2023-06-06 12:06:08.486105 inet-nm-0.0.1/PKG-INFO
--rw-rw-r--   0 weiss     (1000) weiss     (1000)    10522 2023-06-06 11:29:55.000000 inet-nm-0.0.1/README.md
-drwxrwxr-x   0 weiss     (1000) weiss     (1000)        0 2023-06-06 12:06:08.474105 inet-nm-0.0.1/docs/
--rw-rw-r--   0 weiss     (1000) weiss     (1000)     1154 2023-05-10 11:06:23.000000 inet-nm-0.0.1/docs/Makefile
-drwxrwxr-x   0 weiss     (1000) weiss     (1000)        0 2023-06-06 12:06:08.474105 inet-nm-0.0.1/docs/_static/
--rw-rw-r--   0 weiss     (1000) weiss     (1000)       18 2023-05-10 11:06:23.000000 inet-nm-0.0.1/docs/_static/.gitignore
--rw-rw-r--   0 weiss     (1000) weiss     (1000)       71 2023-05-10 11:06:23.000000 inet-nm-0.0.1/docs/authors.md
--rw-rw-r--   0 weiss     (1000) weiss     (1000)       73 2023-05-10 11:06:23.000000 inet-nm-0.0.1/docs/changelog.md
--rw-rw-r--   0 weiss     (1000) weiss     (1000)    10022 2023-05-10 11:06:23.000000 inet-nm-0.0.1/docs/conf.py
--rw-rw-r--   0 weiss     (1000) weiss     (1000)       76 2023-05-10 11:06:23.000000 inet-nm-0.0.1/docs/contributing.md
--rw-rw-r--   0 weiss     (1000) weiss     (1000)      957 2023-05-10 11:06:23.000000 inet-nm-0.0.1/docs/index.md
--rw-rw-r--   0 weiss     (1000) weiss     (1000)       66 2023-05-10 11:06:23.000000 inet-nm-0.0.1/docs/license.md
--rw-rw-r--   0 weiss     (1000) weiss     (1000)       70 2023-05-10 11:06:23.000000 inet-nm-0.0.1/docs/readme.md
--rw-rw-r--   0 weiss     (1000) weiss     (1000)      254 2023-05-10 11:06:23.000000 inet-nm-0.0.1/docs/requirements.txt
--rw-rw-r--   0 weiss     (1000) weiss     (1000)      346 2023-05-10 11:06:23.000000 inet-nm-0.0.1/pyproject.toml
--rw-rw-r--   0 weiss     (1000) weiss     (1000)       15 2023-06-05 08:56:29.000000 inet-nm-0.0.1/requirements.txt
--rw-rw-r--   0 weiss     (1000) weiss     (1000)     2007 2023-06-06 12:06:08.486105 inet-nm-0.0.1/setup.cfg
--rw-rw-r--   0 weiss     (1000) weiss     (1000)      704 2023-05-10 11:06:23.000000 inet-nm-0.0.1/setup.py
-drwxrwxr-x   0 weiss     (1000) weiss     (1000)        0 2023-06-06 12:06:08.466105 inet-nm-0.0.1/src/
-drwxrwxr-x   0 weiss     (1000) weiss     (1000)        0 2023-06-06 12:06:08.478105 inet-nm-0.0.1/src/inet_nm/
--rw-rw-r--   0 weiss     (1000) weiss     (1000)      492 2023-06-05 11:50:11.000000 inet-nm-0.0.1/src/inet_nm/__init__.py
--rw-rw-r--   0 weiss     (1000) weiss     (1000)     5661 2023-06-06 11:33:50.000000 inet-nm-0.0.1/src/inet_nm/_helpers.py
--rw-rw-r--   0 weiss     (1000) weiss     (1000)     9301 2023-06-06 11:33:50.000000 inet-nm-0.0.1/src/inet_nm/check.py
--rw-rw-r--   0 weiss     (1000) weiss     (1000)     6654 2023-06-06 11:34:32.000000 inet-nm-0.0.1/src/inet_nm/commissioner.py
--rw-rw-r--   0 weiss     (1000) weiss     (1000)     3944 2023-06-05 13:59:29.000000 inet-nm-0.0.1/src/inet_nm/config.py
--rw-rw-r--   0 weiss     (1000) weiss     (1000)     2998 2023-06-05 04:48:38.000000 inet-nm-0.0.1/src/inet_nm/data_types.py
--rw-rw-r--   0 weiss     (1000) weiss     (1000)     3455 2023-06-05 09:01:44.000000 inet-nm-0.0.1/src/inet_nm/filelock.py
--rw-rw-r--   0 weiss     (1000) weiss     (1000)     1444 2023-06-05 06:53:17.000000 inet-nm-0.0.1/src/inet_nm/locking.py
--rw-rw-r--   0 weiss     (1000) weiss     (1000)     4829 2023-06-05 09:01:56.000000 inet-nm-0.0.1/src/inet_nm/runner_apps.py
--rw-rw-r--   0 weiss     (1000) weiss     (1000)     3952 2023-06-05 09:02:28.000000 inet-nm-0.0.1/src/inet_nm/runner_base.py
--rw-rw-r--   0 weiss     (1000) weiss     (1000)     2044 2023-06-01 05:56:05.000000 inet-nm-0.0.1/src/inet_nm/runner_cli.py
--rw-rw-r--   0 weiss     (1000) weiss     (1000)     2381 2023-06-06 11:34:39.000000 inet-nm-0.0.1/src/inet_nm/update_os_board_list.py
-drwxrwxr-x   0 weiss     (1000) weiss     (1000)        0 2023-06-06 12:06:08.482105 inet-nm-0.0.1/src/inet_nm.egg-info/
--rw-rw-r--   0 weiss     (1000) weiss     (1000)    11330 2023-06-06 12:06:08.000000 inet-nm-0.0.1/src/inet_nm.egg-info/PKG-INFO
--rw-rw-r--   0 weiss     (1000) weiss     (1000)     1176 2023-06-06 12:06:08.000000 inet-nm-0.0.1/src/inet_nm.egg-info/SOURCES.txt
--rw-rw-r--   0 weiss     (1000) weiss     (1000)        1 2023-06-06 12:06:08.000000 inet-nm-0.0.1/src/inet_nm.egg-info/dependency_links.txt
--rw-rw-r--   0 weiss     (1000) weiss     (1000)      476 2023-06-06 12:06:08.000000 inet-nm-0.0.1/src/inet_nm.egg-info/entry_points.txt
--rw-rw-r--   0 weiss     (1000) weiss     (1000)        1 2023-06-06 12:06:08.000000 inet-nm-0.0.1/src/inet_nm.egg-info/not-zip-safe
--rw-rw-r--   0 weiss     (1000) weiss     (1000)      109 2023-06-06 12:06:08.000000 inet-nm-0.0.1/src/inet_nm.egg-info/requires.txt
--rw-rw-r--   0 weiss     (1000) weiss     (1000)        8 2023-06-06 12:06:08.000000 inet-nm-0.0.1/src/inet_nm.egg-info/top_level.txt
-drwxrwxr-x   0 weiss     (1000) weiss     (1000)        0 2023-06-06 12:06:08.486105 inet-nm-0.0.1/tests/
--rw-rw-r--   0 weiss     (1000) weiss     (1000)      275 2023-05-10 11:06:23.000000 inet-nm-0.0.1/tests/conftest.py
--rw-rw-r--   0 weiss     (1000) weiss     (1000)     3295 2023-06-04 08:15:05.000000 inet-nm-0.0.1/tests/test_check.py
--rw-rw-r--   0 weiss     (1000) weiss     (1000)     2836 2023-06-05 08:58:32.000000 inet-nm-0.0.1/tests/test_comissioner.py
--rw-rw-r--   0 weiss     (1000) weiss     (1000)     1360 2023-06-05 04:44:26.000000 inet-nm-0.0.1/tests/test_config.py
--rw-rw-r--   0 weiss     (1000) weiss     (1000)     1133 2023-06-05 04:51:14.000000 inet-nm-0.0.1/tests/test_data_types.py
--rw-rw-r--   0 weiss     (1000) weiss     (1000)      553 2023-06-05 06:35:49.000000 inet-nm-0.0.1/tests/test_filelock.py
--rw-rw-r--   0 weiss     (1000) weiss     (1000)     2223 2023-06-04 08:15:05.000000 inet-nm-0.0.1/tests/test_helpers.py
--rw-rw-r--   0 weiss     (1000) weiss     (1000)     2195 2023-06-05 08:52:53.000000 inet-nm-0.0.1/tests/test_locking.py
--rw-rw-r--   0 weiss     (1000) weiss     (1000)     1374 2023-06-05 08:52:18.000000 inet-nm-0.0.1/tests/test_runner_apps.py
--rw-rw-r--   0 weiss     (1000) weiss     (1000)     1689 2023-06-05 07:57:10.000000 inet-nm-0.0.1/tests/test_runner_base.py
--rw-rw-r--   0 weiss     (1000) weiss     (1000)     2779 2023-06-06 11:44:55.000000 inet-nm-0.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:49:35.920820 inet-nm-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-06 15:48:58.000000 inet-nm-0.0.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:49:35.912820 inet-nm-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:49:35.916820 inet-nm-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-06 15:48:58.000000 inet-nm-0.0.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-06 15:48:58.000000 inet-nm-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-06 15:48:58.000000 inet-nm-0.0.2/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-06 15:48:58.000000 inet-nm-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-06 15:48:58.000000 inet-nm-0.0.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-06 15:48:58.000000 inet-nm-0.0.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-06 15:48:58.000000 inet-nm-0.0.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10522 2023-06-06 15:48:58.000000 inet-nm-0.0.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-06 15:48:58.000000 inet-nm-0.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9248 2023-06-06 15:49:35.920820 inet-nm-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-06-06 15:48:58.000000 inet-nm-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:49:35.916820 inet-nm-0.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-06 15:48:58.000000 inet-nm-0.0.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:49:35.916820 inet-nm-0.0.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-06 15:48:58.000000 inet-nm-0.0.2/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-06 15:48:58.000000 inet-nm-0.0.2/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-06 15:48:58.000000 inet-nm-0.0.2/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10022 2023-06-06 15:48:58.000000 inet-nm-0.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-06 15:48:58.000000 inet-nm-0.0.2/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-06 15:48:58.000000 inet-nm-0.0.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-06 15:48:58.000000 inet-nm-0.0.2/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-06 15:48:58.000000 inet-nm-0.0.2/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-06 15:48:58.000000 inet-nm-0.0.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-06 15:48:58.000000 inet-nm-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-06 15:48:58.000000 inet-nm-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-06-06 15:49:35.920820 inet-nm-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-06 15:48:58.000000 inet-nm-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:49:35.912820 inet-nm-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:49:35.916820 inet-nm-0.0.2/src/inet_nm/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-06 15:48:58.000000 inet-nm-0.0.2/src/inet_nm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-06-06 15:48:58.000000 inet-nm-0.0.2/src/inet_nm/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-06-06 15:48:58.000000 inet-nm-0.0.2/src/inet_nm/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-06-06 15:48:58.000000 inet-nm-0.0.2/src/inet_nm/commissioner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-06-06 15:48:58.000000 inet-nm-0.0.2/src/inet_nm/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-06-06 15:48:58.000000 inet-nm-0.0.2/src/inet_nm/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-06-06 15:48:58.000000 inet-nm-0.0.2/src/inet_nm/filelock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-06 15:48:58.000000 inet-nm-0.0.2/src/inet_nm/locking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-06-06 15:48:58.000000 inet-nm-0.0.2/src/inet_nm/runner_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-06-06 15:48:58.000000 inet-nm-0.0.2/src/inet_nm/runner_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-06-06 15:48:58.000000 inet-nm-0.0.2/src/inet_nm/runner_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-06-06 15:48:58.000000 inet-nm-0.0.2/src/inet_nm/update_os_board_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:49:35.920820 inet-nm-0.0.2/src/inet_nm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9248 2023-06-06 15:49:35.000000 inet-nm-0.0.2/src/inet_nm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-06 15:49:35.000000 inet-nm-0.0.2/src/inet_nm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 15:49:35.000000 inet-nm-0.0.2/src/inet_nm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-06-06 15:49:35.000000 inet-nm-0.0.2/src/inet_nm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 15:49:35.000000 inet-nm-0.0.2/src/inet_nm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-06 15:49:35.000000 inet-nm-0.0.2/src/inet_nm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 15:49:35.000000 inet-nm-0.0.2/src/inet_nm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 15:49:35.920820 inet-nm-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-06 15:48:58.000000 inet-nm-0.0.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-06-06 15:48:58.000000 inet-nm-0.0.2/tests/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-06 15:48:58.000000 inet-nm-0.0.2/tests/test_comissioner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-06 15:48:58.000000 inet-nm-0.0.2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-06 15:48:58.000000 inet-nm-0.0.2/tests/test_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-06 15:48:58.000000 inet-nm-0.0.2/tests/test_filelock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-06-06 15:48:58.000000 inet-nm-0.0.2/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-06-06 15:48:58.000000 inet-nm-0.0.2/tests/test_locking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-06 15:48:58.000000 inet-nm-0.0.2/tests/test_runner_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-06 15:48:58.000000 inet-nm-0.0.2/tests/test_runner_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-06-06 15:48:58.000000 inet-nm-0.0.2/tox.ini
```

### Comparing `inet-nm-0.0.1/.coveragerc` & `inet-nm-0.0.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.1/.github/workflows/ci.yml` & `inet-nm-0.0.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.1/.gitignore` & `inet-nm-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.1/.pre-commit-config.yaml` & `inet-nm-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.1/.readthedocs.yml` & `inet-nm-0.0.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.1/CONTRIBUTING.md` & `inet-nm-0.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.1/LICENSE.txt` & `inet-nm-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.1/PKG-INFO` & `inet-nm-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inet-nm
-Version: 0.0.1
+Version: 0.0.2
 Summary: cli application for managing nodes
 Home-page: https://github.com/inetrg/inet-nm
 Author: Kevin Weiss
 Author-email: weiss.kevin604@gmail.com
 License: MIT
 Project-URL: Documentation, https://inet-nm.readthedocs.io/en/stable/
 Project-URL: Source, https://github.com/inetrg/inet-nm
@@ -48,27 +48,48 @@
 
 All these features are designed to make managing numerous development
 boards more manageable and efficient, particularly for teams maintaining
 large open-source projects like RIOT OS.
 
 ## Installation
 
-You can install inet_nm via pip:
+### As a developer or single user
+
+You can install inet_nm via pip or pipx (recommended to use a venv):
 
 ```bash
 pip install inet-nm
 ```
 
+### On a shared computer for CI
+
+If you have one computer where many different users may want to access the
+boards it may be better to setup for all users.
+
+First change the config dir to a shared path (by default we select `/etc/environment`):
+```
+sudo sed -i '/NM_CONFIG_DIR/d' /etc/environment && echo 'NM_CONFIG_DIR=/etc/inet-nm' | sudo tee -a /etc/environment
+```
+
+Then install with pip system-wide
+```
+sudo pip install inet-nm
+```
+
+Now all users should be able to access the cli functions. Note that `sudo` will
+be needed to make any changes such as commissioning boards or updating board
+names.
+
 ## Usage
 
 Below is the usage for each of the command-line applications included in inet_nm:
 
-### inet-nm-update-riot
+### inet-nm-update-from-os
 
-This command is used to cache a list of boards.
+This command is used to cache a list of boards and features.
 
 ```
 $ inet-nm-update-from-os -h
 usage: inet-nm-update-from-os [-h] [-c CONFIG] [-i BOARD_INFO] [-f BOARD_FEATURES] [-n BOARD_ENV_VAR] basedir
 
 Cache a list of boards
 
@@ -85,66 +106,38 @@
                         Command to get board features, defaults to 'make info-features-provided'
   -n BOARD_ENV_VAR, --board-env-var BOARD_ENV_VAR
                         The env var to indicate the board name for features provided, defaults to 'BOARD'
 ```
 
 ### inet-nm-update-commissioned
 
-This command is used to update commissioned features.
+This command is used to update commissioned features, usually after
+`inet-nm-update-from-os` is called.
 
 ```
 $ inet-nm-update-commissioned -h
 usage: inet-nm-update-commissioned [-h] [-c CONFIG]
-
-optional arguments:
-  -h, --help            show this help message and exit
-  -c CONFIG, --config CONFIG
-                        Path to the config dir
 ```
 
 ### inet-nm-commission
 
-This command is used to commission USB boards.
+This is an interactive prompt to new commission USB boards.
 
 ```
 $ inet-nm-commission -h
 usage: inet-nm-commission [-h] [-c CONFIG] [-b BOARD] [-n]
-
-optional arguments:
-  -h, --help            show this help message and exit
-  -c CONFIG, --config CONFIG
-                        Path to the config dir
-  -b BOARD, --board BOARD
-                        Name of the board to commission
-  -n, --no-cache        Ignore the cache
 ```
 
 ### inet-nm-check
 
-This command is used to check the state of the boards.
+This command is used to check the list of boards given some conditions.
 
 ```
 $ inet-nm-check -h
 usage: inet-nm-check [-h] [-c CONFIG] [-f FEAT_FILTER [FEAT_FILTER ...]] [-a] [-m] [-e FEAT_EVAL] [-u] [-s] [--show-features]
-
-Check the state of the boards
-
-optional arguments:
-  -h, --help            show this help message and exit
-  -c CONFIG, --config CONFIG
-                        Path to the config dir
-  -f FEAT_FILTER [FEAT_FILTER ...], --feat-filter FEAT_FILTER [FEAT_FILTER ...]
-                        Filter all boards that don't provide these features
-  -a, --all-nodes       Show all boards, regardless of connection
-  -m, --missing         Show all missing boards
-  -e FEAT_EVAL, --feat-eval FEAT_EVAL
-                        Evaluate features with this function
-  -u, --used            Show used boards as well
-  -s, --skip-dups       Skip duplicate boards
-  --show-features       Shows all features for all boards
 ```
 
 ### Environment Variables
 
 When executing a script or running interactively,
 [env vars are available](src/inet_nm/data_types.py):
 
@@ -152,88 +145,49 @@
 NM_IDX: Index of the node.
 NM_UID: Unique ID of the node.
 NM_SERIAL: Serial number of the node.
 NM_BOARD: Board of the node.
 NM_PORT: Port of the node.
 ```
 
-### inet-nm-exec
+There is also an environment variable to specify the default configuration
+directory.
+```
+NM_CONFIG_DIR
+```
 
-This command is used to send commands after starting
+### inet-nm-exec
 
- a tmux session.
+This command is used to send execute a command or script. It will block the nodes
+until it is finished.
 
 ```
 $ inet-nm-exec -h
 usage: inet-nm-exec [-h] [-t TIMEOUT] [-c CONFIG] [-f FEAT_FILTER [FEAT_FILTER ...]] [-a] [-m] [-e FEAT_EVAL] [-u] [-s] cmd
-
-positional arguments:
-  cmd                   Command to send after starting tmux session.
-
-optional arguments:
-  -h, --help            show this help message and exit
-  -t TIMEOUT, --timeout TIMEOUT
-                        Wait until node available in seconds.
-  -c CONFIG, --config CONFIG
-                        Path to the config dir
-  -f FEAT_FILTER [FEAT_FILTER ...], --feat-filter FEAT_FILTER [FEAT_FILTER ...]
-                        Filter all boards that do not provide these features
-  -a, --all-nodes       Show all boards, regardless of connection
-  -m, --missing         Show all missing boards
-  -e FEAT_EVAL, --feat-eval FEAT_EVAL
-                        Evaluate features with this function
-  -u, --used            Show used boards as well
-  -s, --skip-dups       Skip duplicate boards
 ```
 
 ### inet-nm-tmux
 
-This command is used to manage nodes in a tmux session.
+This command is used to manage nodes in a tmux session. It will block the nodes
+until the session is over.
 
 ```
 inet-nm-tmux -h
 usage: inet-nm-tmux [-h] [-w] [-t TIMEOUT] [-x CMD] [-c CONFIG] [-f FEAT_FILTER [FEAT_FILTER ...]] [-a] [-m] [-e FEAT_EVAL] [-u] [-s]
-
-optional arguments:
-  -h, --help            show this help message and exit
-  -w, --window          Open a window for each node.
-  -t TIMEOUT, --timeout TIMEOUT
-                        Wait until node available in seconds.
-  -x CMD, --cmd CMD     Command to send after starting tmux session.
-  -c CONFIG, --config CONFIG
-                        Path to the config dir
-  -f FEAT_FILTER [FEAT_FILTER ...], --feat-filter FEAT_FILTER [FEAT_FILTER ...]
-                        Filter all boards that do not provide these features
-  -a, --all-nodes       Show all boards, regardless of connection
-  -m, --missing         Show all missing boards
-  -e FEAT_EVAL, --feat-eval FEAT_EVAL
-                        Evaluate features with this function
-  -u, --used            Show used boards as well
-  -s, --skip-dups       Skip duplicate boards
 ```
 
 
 ### inet-nm-from-uid
 
 This command finds the tty of a node given the UID. This is useful if a node
 gets reconnected during an interactive session.
 
 ```
 $ inet-nm-tty-from-uid -h
 usage: inet-nm-tty-from-uid [-h] [-c CONFIG] uid
-
-Get the TTY device node string for a given NmNode UID.
-
-positional arguments:
-  uid                   Node UID string.
-
-optional arguments:
-  -h, --help            show this help message and exit
-  -c CONFIG, --config CONFIG
-                        Path to the config di
 ```
 
 ## Example Workflow
 
 1. First update the boards list in the cache to allow for autocomplete and
 features.
 ```
```

### Comparing `inet-nm-0.0.1/README.md` & `inet-nm-0.0.2/src/inet_nm.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: inet-nm
+Version: 0.0.2
+Summary: cli application for managing nodes
+Home-page: https://github.com/inetrg/inet-nm
+Author: Kevin Weiss
+Author-email: weiss.kevin604@gmail.com
+License: MIT
+Project-URL: Documentation, https://inet-nm.readthedocs.io/en/stable/
+Project-URL: Source, https://github.com/inetrg/inet-nm
+Project-URL: Changelog, https://github.com/inetrg/inet-nm/blob/master/CHANGELOG.md
+Project-URL: Tracker, https://github.com/inetrg/inet-nm/issues
+Project-URL: Download, https://pypi.org/project/inet-nm/#files
+Platform: any
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Provides-Extra: testing
+Provides-Extra: all
+License-File: LICENSE.txt
+
 [![ReadTheDocs](https://readthedocs.org/projects/inet-nm/badge/?version=latest)](https://inet-nm.readthedocs.io/en/stable/)
 [![PyPI-Server](https://img.shields.io/pypi/v/inet-nm.svg)](https://pypi.org/project/inet-nm/)
 [![Monthly Downloads](https://pepy.tech/badge/inet-nm/month)](https://pepy.tech/project/inet-nm)
 
 # inet_nm - INET Node Manager
 
 INET Node Manager (inet_nm) is a comprehensive suite of command-line
@@ -26,27 +48,48 @@
 
 All these features are designed to make managing numerous development
 boards more manageable and efficient, particularly for teams maintaining
 large open-source projects like RIOT OS.
 
 ## Installation
 
-You can install inet_nm via pip:
+### As a developer or single user
+
+You can install inet_nm via pip or pipx (recommended to use a venv):
 
 ```bash
 pip install inet-nm
 ```
 
+### On a shared computer for CI
+
+If you have one computer where many different users may want to access the
+boards it may be better to setup for all users.
+
+First change the config dir to a shared path (by default we select `/etc/environment`):
+```
+sudo sed -i '/NM_CONFIG_DIR/d' /etc/environment && echo 'NM_CONFIG_DIR=/etc/inet-nm' | sudo tee -a /etc/environment
+```
+
+Then install with pip system-wide
+```
+sudo pip install inet-nm
+```
+
+Now all users should be able to access the cli functions. Note that `sudo` will
+be needed to make any changes such as commissioning boards or updating board
+names.
+
 ## Usage
 
 Below is the usage for each of the command-line applications included in inet_nm:
 
-### inet-nm-update-riot
+### inet-nm-update-from-os
 
-This command is used to cache a list of boards.
+This command is used to cache a list of boards and features.
 
 ```
 $ inet-nm-update-from-os -h
 usage: inet-nm-update-from-os [-h] [-c CONFIG] [-i BOARD_INFO] [-f BOARD_FEATURES] [-n BOARD_ENV_VAR] basedir
 
 Cache a list of boards
 
@@ -63,66 +106,38 @@
                         Command to get board features, defaults to 'make info-features-provided'
   -n BOARD_ENV_VAR, --board-env-var BOARD_ENV_VAR
                         The env var to indicate the board name for features provided, defaults to 'BOARD'
 ```
 
 ### inet-nm-update-commissioned
 
-This command is used to update commissioned features.
+This command is used to update commissioned features, usually after
+`inet-nm-update-from-os` is called.
 
 ```
 $ inet-nm-update-commissioned -h
 usage: inet-nm-update-commissioned [-h] [-c CONFIG]
-
-optional arguments:
-  -h, --help            show this help message and exit
-  -c CONFIG, --config CONFIG
-                        Path to the config dir
 ```
 
 ### inet-nm-commission
 
-This command is used to commission USB boards.
+This is an interactive prompt to new commission USB boards.
 
 ```
 $ inet-nm-commission -h
 usage: inet-nm-commission [-h] [-c CONFIG] [-b BOARD] [-n]
-
-optional arguments:
-  -h, --help            show this help message and exit
-  -c CONFIG, --config CONFIG
-                        Path to the config dir
-  -b BOARD, --board BOARD
-                        Name of the board to commission
-  -n, --no-cache        Ignore the cache
 ```
 
 ### inet-nm-check
 
-This command is used to check the state of the boards.
+This command is used to check the list of boards given some conditions.
 
 ```
 $ inet-nm-check -h
 usage: inet-nm-check [-h] [-c CONFIG] [-f FEAT_FILTER [FEAT_FILTER ...]] [-a] [-m] [-e FEAT_EVAL] [-u] [-s] [--show-features]
-
-Check the state of the boards
-
-optional arguments:
-  -h, --help            show this help message and exit
-  -c CONFIG, --config CONFIG
-                        Path to the config dir
-  -f FEAT_FILTER [FEAT_FILTER ...], --feat-filter FEAT_FILTER [FEAT_FILTER ...]
-                        Filter all boards that don't provide these features
-  -a, --all-nodes       Show all boards, regardless of connection
-  -m, --missing         Show all missing boards
-  -e FEAT_EVAL, --feat-eval FEAT_EVAL
-                        Evaluate features with this function
-  -u, --used            Show used boards as well
-  -s, --skip-dups       Skip duplicate boards
-  --show-features       Shows all features for all boards
 ```
 
 ### Environment Variables
 
 When executing a script or running interactively,
 [env vars are available](src/inet_nm/data_types.py):
 
@@ -130,88 +145,49 @@
 NM_IDX: Index of the node.
 NM_UID: Unique ID of the node.
 NM_SERIAL: Serial number of the node.
 NM_BOARD: Board of the node.
 NM_PORT: Port of the node.
 ```
 
-### inet-nm-exec
+There is also an environment variable to specify the default configuration
+directory.
+```
+NM_CONFIG_DIR
+```
 
-This command is used to send commands after starting
+### inet-nm-exec
 
- a tmux session.
+This command is used to send execute a command or script. It will block the nodes
+until it is finished.
 
 ```
 $ inet-nm-exec -h
 usage: inet-nm-exec [-h] [-t TIMEOUT] [-c CONFIG] [-f FEAT_FILTER [FEAT_FILTER ...]] [-a] [-m] [-e FEAT_EVAL] [-u] [-s] cmd
-
-positional arguments:
-  cmd                   Command to send after starting tmux session.
-
-optional arguments:
-  -h, --help            show this help message and exit
-  -t TIMEOUT, --timeout TIMEOUT
-                        Wait until node available in seconds.
-  -c CONFIG, --config CONFIG
-                        Path to the config dir
-  -f FEAT_FILTER [FEAT_FILTER ...], --feat-filter FEAT_FILTER [FEAT_FILTER ...]
-                        Filter all boards that do not provide these features
-  -a, --all-nodes       Show all boards, regardless of connection
-  -m, --missing         Show all missing boards
-  -e FEAT_EVAL, --feat-eval FEAT_EVAL
-                        Evaluate features with this function
-  -u, --used            Show used boards as well
-  -s, --skip-dups       Skip duplicate boards
 ```
 
 ### inet-nm-tmux
 
-This command is used to manage nodes in a tmux session.
+This command is used to manage nodes in a tmux session. It will block the nodes
+until the session is over.
 
 ```
 inet-nm-tmux -h
 usage: inet-nm-tmux [-h] [-w] [-t TIMEOUT] [-x CMD] [-c CONFIG] [-f FEAT_FILTER [FEAT_FILTER ...]] [-a] [-m] [-e FEAT_EVAL] [-u] [-s]
-
-optional arguments:
-  -h, --help            show this help message and exit
-  -w, --window          Open a window for each node.
-  -t TIMEOUT, --timeout TIMEOUT
-                        Wait until node available in seconds.
-  -x CMD, --cmd CMD     Command to send after starting tmux session.
-  -c CONFIG, --config CONFIG
-                        Path to the config dir
-  -f FEAT_FILTER [FEAT_FILTER ...], --feat-filter FEAT_FILTER [FEAT_FILTER ...]
-                        Filter all boards that do not provide these features
-  -a, --all-nodes       Show all boards, regardless of connection
-  -m, --missing         Show all missing boards
-  -e FEAT_EVAL, --feat-eval FEAT_EVAL
-                        Evaluate features with this function
-  -u, --used            Show used boards as well
-  -s, --skip-dups       Skip duplicate boards
 ```
 
 
 ### inet-nm-from-uid
 
 This command finds the tty of a node given the UID. This is useful if a node
 gets reconnected during an interactive session.
 
 ```
 $ inet-nm-tty-from-uid -h
 usage: inet-nm-tty-from-uid [-h] [-c CONFIG] uid
-
-Get the TTY device node string for a given NmNode UID.
-
-positional arguments:
-  uid                   Node UID string.
-
-optional arguments:
-  -h, --help            show this help message and exit
-  -c CONFIG, --config CONFIG
-                        Path to the config di
 ```
 
 ## Example Workflow
 
 1. First update the boards list in the cache to allow for autocomplete and
 features.
 ```
```

### Comparing `inet-nm-0.0.1/docs/Makefile` & `inet-nm-0.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.1/docs/conf.py` & `inet-nm-0.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.1/setup.cfg` & `inet-nm-0.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.1/setup.py` & `inet-nm-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.1/src/inet_nm/_helpers.py` & `inet-nm-0.0.2/src/inet_nm/_helpers.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.1/src/inet_nm/check.py` & `inet-nm-0.0.2/src/inet_nm/check.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.1/src/inet_nm/commissioner.py` & `inet-nm-0.0.2/src/inet_nm/commissioner.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.1/src/inet_nm/config.py` & `inet-nm-0.0.2/src/inet_nm/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 It includes functionality for saving and loading information about
 the boards and nodes, as well as for handling the path configuration.
 """
 
 import argparse
 import json
+import os
 from pathlib import Path
 from typing import Dict, List, Union
 
 from inet_nm.data_types import NmNode
 
 
 def _file_from_path(config_dir: Union[Path, str], file_name: str) -> Path:
@@ -140,10 +141,15 @@
 def config_arg(parser: argparse.ArgumentParser):
     """
     Add a configuration argument to the provided parser.
 
     Args:
         parser (argparse.ArgumentParser): ArgumentParser object.
     """
+    nm_config_dir = os.environ.get("NM_CONFIG_DIR", "~/.config/inet_nm")
     parser.add_argument(
-        "-c", "--config", default="~/.config/inet_nm", help="Path to the config dir"
+        "-c",
+        "--config",
+        default=nm_config_dir,
+        help="Path to the config dir, defaults to NM_CONFIG_DIR or "
+        "~/.config/inet_nm if NM_CONFIG_DIR is not set",
     )
```

### Comparing `inet-nm-0.0.1/src/inet_nm/data_types.py` & `inet-nm-0.0.2/src/inet_nm/data_types.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.1/src/inet_nm/filelock.py` & `inet-nm-0.0.2/src/inet_nm/filelock.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.1/src/inet_nm/locking.py` & `inet-nm-0.0.2/src/inet_nm/locking.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.1/src/inet_nm/runner_apps.py` & `inet-nm-0.0.2/src/inet_nm/runner_apps.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.1/src/inet_nm/runner_base.py` & `inet-nm-0.0.2/src/inet_nm/runner_base.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.1/src/inet_nm/runner_cli.py` & `inet-nm-0.0.2/src/inet_nm/runner_cli.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.1/src/inet_nm/update_os_board_list.py` & `inet-nm-0.0.2/src/inet_nm/update_os_board_list.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.1/src/inet_nm.egg-info/PKG-INFO` & `inet-nm-0.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: inet-nm
-Version: 0.0.1
-Summary: cli application for managing nodes
-Home-page: https://github.com/inetrg/inet-nm
-Author: Kevin Weiss
-Author-email: weiss.kevin604@gmail.com
-License: MIT
-Project-URL: Documentation, https://inet-nm.readthedocs.io/en/stable/
-Project-URL: Source, https://github.com/inetrg/inet-nm
-Project-URL: Changelog, https://github.com/inetrg/inet-nm/blob/master/CHANGELOG.md
-Project-URL: Tracker, https://github.com/inetrg/inet-nm/issues
-Project-URL: Download, https://pypi.org/project/inet-nm/#files
-Platform: any
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Provides-Extra: testing
-Provides-Extra: all
-License-File: LICENSE.txt
-
 [![ReadTheDocs](https://readthedocs.org/projects/inet-nm/badge/?version=latest)](https://inet-nm.readthedocs.io/en/stable/)
 [![PyPI-Server](https://img.shields.io/pypi/v/inet-nm.svg)](https://pypi.org/project/inet-nm/)
 [![Monthly Downloads](https://pepy.tech/badge/inet-nm/month)](https://pepy.tech/project/inet-nm)
 
 # inet_nm - INET Node Manager
 
 INET Node Manager (inet_nm) is a comprehensive suite of command-line
@@ -48,27 +26,48 @@
 
 All these features are designed to make managing numerous development
 boards more manageable and efficient, particularly for teams maintaining
 large open-source projects like RIOT OS.
 
 ## Installation
 
-You can install inet_nm via pip:
+### As a developer or single user
+
+You can install inet_nm via pip or pipx (recommended to use a venv):
 
 ```bash
 pip install inet-nm
 ```
 
+### On a shared computer for CI
+
+If you have one computer where many different users may want to access the
+boards it may be better to setup for all users.
+
+First change the config dir to a shared path (by default we select `/etc/environment`):
+```
+sudo sed -i '/NM_CONFIG_DIR/d' /etc/environment && echo 'NM_CONFIG_DIR=/etc/inet-nm' | sudo tee -a /etc/environment
+```
+
+Then install with pip system-wide
+```
+sudo pip install inet-nm
+```
+
+Now all users should be able to access the cli functions. Note that `sudo` will
+be needed to make any changes such as commissioning boards or updating board
+names.
+
 ## Usage
 
 Below is the usage for each of the command-line applications included in inet_nm:
 
-### inet-nm-update-riot
+### inet-nm-update-from-os
 
-This command is used to cache a list of boards.
+This command is used to cache a list of boards and features.
 
 ```
 $ inet-nm-update-from-os -h
 usage: inet-nm-update-from-os [-h] [-c CONFIG] [-i BOARD_INFO] [-f BOARD_FEATURES] [-n BOARD_ENV_VAR] basedir
 
 Cache a list of boards
 
@@ -85,66 +84,38 @@
                         Command to get board features, defaults to 'make info-features-provided'
   -n BOARD_ENV_VAR, --board-env-var BOARD_ENV_VAR
                         The env var to indicate the board name for features provided, defaults to 'BOARD'
 ```
 
 ### inet-nm-update-commissioned
 
-This command is used to update commissioned features.
+This command is used to update commissioned features, usually after
+`inet-nm-update-from-os` is called.
 
 ```
 $ inet-nm-update-commissioned -h
 usage: inet-nm-update-commissioned [-h] [-c CONFIG]
-
-optional arguments:
-  -h, --help            show this help message and exit
-  -c CONFIG, --config CONFIG
-                        Path to the config dir
 ```
 
 ### inet-nm-commission
 
-This command is used to commission USB boards.
+This is an interactive prompt to new commission USB boards.
 
 ```
 $ inet-nm-commission -h
 usage: inet-nm-commission [-h] [-c CONFIG] [-b BOARD] [-n]
-
-optional arguments:
-  -h, --help            show this help message and exit
-  -c CONFIG, --config CONFIG
-                        Path to the config dir
-  -b BOARD, --board BOARD
-                        Name of the board to commission
-  -n, --no-cache        Ignore the cache
 ```
 
 ### inet-nm-check
 
-This command is used to check the state of the boards.
+This command is used to check the list of boards given some conditions.
 
 ```
 $ inet-nm-check -h
 usage: inet-nm-check [-h] [-c CONFIG] [-f FEAT_FILTER [FEAT_FILTER ...]] [-a] [-m] [-e FEAT_EVAL] [-u] [-s] [--show-features]
-
-Check the state of the boards
-
-optional arguments:
-  -h, --help            show this help message and exit
-  -c CONFIG, --config CONFIG
-                        Path to the config dir
-  -f FEAT_FILTER [FEAT_FILTER ...], --feat-filter FEAT_FILTER [FEAT_FILTER ...]
-                        Filter all boards that don't provide these features
-  -a, --all-nodes       Show all boards, regardless of connection
-  -m, --missing         Show all missing boards
-  -e FEAT_EVAL, --feat-eval FEAT_EVAL
-                        Evaluate features with this function
-  -u, --used            Show used boards as well
-  -s, --skip-dups       Skip duplicate boards
-  --show-features       Shows all features for all boards
 ```
 
 ### Environment Variables
 
 When executing a script or running interactively,
 [env vars are available](src/inet_nm/data_types.py):
 
@@ -152,88 +123,49 @@
 NM_IDX: Index of the node.
 NM_UID: Unique ID of the node.
 NM_SERIAL: Serial number of the node.
 NM_BOARD: Board of the node.
 NM_PORT: Port of the node.
 ```
 
-### inet-nm-exec
+There is also an environment variable to specify the default configuration
+directory.
+```
+NM_CONFIG_DIR
+```
 
-This command is used to send commands after starting
+### inet-nm-exec
 
- a tmux session.
+This command is used to send execute a command or script. It will block the nodes
+until it is finished.
 
 ```
 $ inet-nm-exec -h
 usage: inet-nm-exec [-h] [-t TIMEOUT] [-c CONFIG] [-f FEAT_FILTER [FEAT_FILTER ...]] [-a] [-m] [-e FEAT_EVAL] [-u] [-s] cmd
-
-positional arguments:
-  cmd                   Command to send after starting tmux session.
-
-optional arguments:
-  -h, --help            show this help message and exit
-  -t TIMEOUT, --timeout TIMEOUT
-                        Wait until node available in seconds.
-  -c CONFIG, --config CONFIG
-                        Path to the config dir
-  -f FEAT_FILTER [FEAT_FILTER ...], --feat-filter FEAT_FILTER [FEAT_FILTER ...]
-                        Filter all boards that do not provide these features
-  -a, --all-nodes       Show all boards, regardless of connection
-  -m, --missing         Show all missing boards
-  -e FEAT_EVAL, --feat-eval FEAT_EVAL
-                        Evaluate features with this function
-  -u, --used            Show used boards as well
-  -s, --skip-dups       Skip duplicate boards
 ```
 
 ### inet-nm-tmux
 
-This command is used to manage nodes in a tmux session.
+This command is used to manage nodes in a tmux session. It will block the nodes
+until the session is over.
 
 ```
 inet-nm-tmux -h
 usage: inet-nm-tmux [-h] [-w] [-t TIMEOUT] [-x CMD] [-c CONFIG] [-f FEAT_FILTER [FEAT_FILTER ...]] [-a] [-m] [-e FEAT_EVAL] [-u] [-s]
-
-optional arguments:
-  -h, --help            show this help message and exit
-  -w, --window          Open a window for each node.
-  -t TIMEOUT, --timeout TIMEOUT
-                        Wait until node available in seconds.
-  -x CMD, --cmd CMD     Command to send after starting tmux session.
-  -c CONFIG, --config CONFIG
-                        Path to the config dir
-  -f FEAT_FILTER [FEAT_FILTER ...], --feat-filter FEAT_FILTER [FEAT_FILTER ...]
-                        Filter all boards that do not provide these features
-  -a, --all-nodes       Show all boards, regardless of connection
-  -m, --missing         Show all missing boards
-  -e FEAT_EVAL, --feat-eval FEAT_EVAL
-                        Evaluate features with this function
-  -u, --used            Show used boards as well
-  -s, --skip-dups       Skip duplicate boards
 ```
 
 
 ### inet-nm-from-uid
 
 This command finds the tty of a node given the UID. This is useful if a node
 gets reconnected during an interactive session.
 
 ```
 $ inet-nm-tty-from-uid -h
 usage: inet-nm-tty-from-uid [-h] [-c CONFIG] uid
-
-Get the TTY device node string for a given NmNode UID.
-
-positional arguments:
-  uid                   Node UID string.
-
-optional arguments:
-  -h, --help            show this help message and exit
-  -c CONFIG, --config CONFIG
-                        Path to the config di
 ```
 
 ## Example Workflow
 
 1. First update the boards list in the cache to allow for autocomplete and
 features.
 ```
```

### Comparing `inet-nm-0.0.1/src/inet_nm.egg-info/SOURCES.txt` & `inet-nm-0.0.2/src/inet_nm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.1/tests/test_check.py` & `inet-nm-0.0.2/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.1/tests/test_comissioner.py` & `inet-nm-0.0.2/tests/test_comissioner.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.1/tests/test_config.py` & `inet-nm-0.0.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.1/tests/test_data_types.py` & `inet-nm-0.0.2/tests/test_data_types.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.1/tests/test_filelock.py` & `inet-nm-0.0.2/tests/test_filelock.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.1/tests/test_helpers.py` & `inet-nm-0.0.2/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.1/tests/test_locking.py` & `inet-nm-0.0.2/tests/test_locking.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.1/tests/test_runner_apps.py` & `inet-nm-0.0.2/tests/test_runner_apps.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.1/tests/test_runner_base.py` & `inet-nm-0.0.2/tests/test_runner_base.py`

 * *Files identical despite different names*

### Comparing `inet-nm-0.0.1/tox.ini` & `inet-nm-0.0.2/tox.ini`

 * *Files identical despite different names*

