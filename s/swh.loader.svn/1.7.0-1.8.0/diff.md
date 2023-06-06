# Comparing `tmp/swh.loader.svn-1.7.0.tar.gz` & `tmp/swh.loader.svn-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swh.loader.svn-1.7.0.tar", last modified: Fri May 26 14:57:02 2023, max compression
+gzip compressed data, was "dist/swh.loader.svn-1.8.0.tar", last modified: Tue Jun  6 12:50:23 2023, max compression
```

## Comparing `swh.loader.svn-1.7.0.tar` & `swh.loader.svn-1.8.0.tar`

### file list

```diff
@@ -1,93 +1,96 @@
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 14:57:02.000000 swh.loader.svn-1.7.0/
--rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) docker     (999)      135 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      848 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/AUTHORS
--rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) docker     (999)       14 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/LICENSE
--rw-r--r--   0 jenkins    (115) docker     (999)      160 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/MANIFEST.in
--rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     1922 2023-05-26 14:57:02.000000 swh.loader.svn-1.7.0/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)      994 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/README.md
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 14:57:02.000000 swh.loader.svn-1.7.0/bin/
--rwxr-xr-x   0 jenkins    (115) docker     (999)      552 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/bin/init-svn-repository.sh
--rwxr-xr-x   0 jenkins    (115) docker     (999)      761 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/bin/swh-svn
--rw-r--r--   0 jenkins    (115) docker     (999)      567 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 14:57:02.000000 swh.loader.svn-1.7.0/docs/
--rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/docs/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/docs/Makefile
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 14:57:02.000000 swh.loader.svn-1.7.0/docs/_static/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 14:57:02.000000 swh.loader.svn-1.7.0/docs/_templates/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/docs/conf.py
--rw-r--r--   0 jenkins    (115) docker     (999)      391 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/docs/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     6651 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/docs/swh-loader-svn.txt
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 14:57:02.000000 swh.loader.svn-1.7.0/install/
--rwxr-xr-x   0 jenkins    (115) docker     (999)      644 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/install/install-pysvn.sh
--rwxr-xr-x   0 jenkins    (115) docker     (999)      109 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/install/install-subvertpy.sh
--rw-r--r--   0 jenkins    (115) docker     (999)      347 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/mypy.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/pyproject.toml
--rw-r--r--   0 jenkins    (115) docker     (999)      248 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/pytest.ini
--rw-r--r--   0 jenkins    (115) docker     (999)       90 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       96 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/requirements-test.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      292 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/requirements.txt
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 14:57:02.000000 swh.loader.svn-1.7.0/resources/
--rw-r--r--   0 jenkins    (115) docker     (999)      860 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/resources/svn.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-05-26 14:57:02.000000 swh.loader.svn-1.7.0/setup.cfg
--rwxr-xr-x   0 jenkins    (115) docker     (999)     5522 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/setup.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5873 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/svn-lib-client-analysis.org
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 14:57:02.000000 swh.loader.svn-1.7.0/swh/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 14:57:02.000000 swh.loader.svn-1.7.0/swh/loader/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 14:57:02.000000 swh.loader.svn-1.7.0/swh/loader/svn/
--rw-r--r--   0 jenkins    (115) docker     (999)      491 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2427 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/converters.py
--rw-r--r--   0 jenkins    (115) docker     (999)      667 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/exception.py
--rw-r--r--   0 jenkins    (115) docker     (999)     9055 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/fast_crawler.cpp
--rw-r--r--   0 jenkins    (115) docker     (999)      515 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/fast_crawler.pyi
--rw-r--r--   0 jenkins    (115) docker     (999)    34162 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/loader.py
--rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/py.typed
--rw-r--r--   0 jenkins    (115) docker     (999)    33820 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/replay.py
--rw-r--r--   0 jenkins    (115) docker     (999)    23534 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/svn_repo.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1521 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/svn_retry.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1511 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 14:57:02.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2459 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 14:57:02.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/data/
--rw-r--r--   0 jenkins    (115) docker     (999)   360057 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/data/httthttt.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)   389343 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/data/mediawiki-repo-r407-eol-native-crlf.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)      201 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/data/penguinsdbtools2018.dump.gz
--rw-r--r--   0 jenkins    (115) docker     (999)   419840 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pkg-doc-linux-r10.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)   430080 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pkg-doc-linux-r11.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)   911360 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pkg-doc-linux-r12.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)    28495 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pkg-gourmet-add-remove-dir.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)   133120 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pkg-gourmet-tampered-rev6-log.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)   163840 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pkg-gourmet-with-edge-case-links-and-files.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)    35440 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pkg-gourmet-with-external-id.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)    30908 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pkg-gourmet-with-updates.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)   163840 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pkg-gourmet-with-wrong-link-cases.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)    28193 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pkg-gourmet.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)   406052 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pyang-repo-r343-eol-native-mixed-lf-crlf.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)     3985 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/test_converters.py
--rw-r--r--   0 jenkins    (115) docker     (999)    62193 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/test_externals.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2371 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/test_fast_crawler.py
--rw-r--r--   0 jenkins    (115) docker     (999)    17874 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/test_loader.org
--rw-r--r--   0 jenkins    (115) docker     (999)    79106 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/test_loader.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3260 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/test_svn_repo.py
--rw-r--r--   0 jenkins    (115) docker     (999)    12997 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/test_svn_retry.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2471 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/test_task.py
--rw-r--r--   0 jenkins    (115) docker     (999)    21336 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/test_utils.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3734 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/tests/utils.py
--rw-r--r--   0 jenkins    (115) docker     (999)    15984 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/swh/loader/svn/utils.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 14:57:02.000000 swh.loader.svn-1.7.0/swh.loader.svn.egg-info/
--rw-r--r--   0 jenkins    (115) docker     (999)     1922 2023-05-26 14:57:02.000000 swh.loader.svn-1.7.0/swh.loader.svn.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     2360 2023-05-26 14:57:02.000000 swh.loader.svn-1.7.0/swh.loader.svn.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-05-26 14:57:02.000000 swh.loader.svn-1.7.0/swh.loader.svn.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       51 2023-05-26 14:57:02.000000 swh.loader.svn-1.7.0/swh.loader.svn.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      250 2023-05-26 14:57:02.000000 swh.loader.svn-1.7.0/swh.loader.svn.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-05-26 14:57:02.000000 swh.loader.svn-1.7.0/swh.loader.svn.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1531 2023-05-26 14:57:00.000000 swh.loader.svn-1.7.0/tox.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:50:23.000000 swh.loader.svn-1.8.0/
+-rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) docker     (999)      135 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      848 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/AUTHORS
+-rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) docker     (999)       14 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/LICENSE
+-rw-r--r--   0 jenkins    (115) docker     (999)      160 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/MANIFEST.in
+-rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     2023 2023-06-06 12:50:23.000000 swh.loader.svn-1.8.0/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     1095 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/README.md
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:50:23.000000 swh.loader.svn-1.8.0/bin/
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      552 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/bin/init-svn-repository.sh
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      761 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/bin/swh-svn
+-rw-r--r--   0 jenkins    (115) docker     (999)      567 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:50:23.000000 swh.loader.svn-1.8.0/docs/
+-rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/docs/Makefile
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:50:23.000000 swh.loader.svn-1.8.0/docs/_static/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:50:23.000000 swh.loader.svn-1.8.0/docs/_templates/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/docs/conf.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      391 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/docs/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     6651 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/docs/swh-loader-svn.txt
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:50:23.000000 swh.loader.svn-1.8.0/install/
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      644 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/install/install-pysvn.sh
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      109 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/install/install-subvertpy.sh
+-rw-r--r--   0 jenkins    (115) docker     (999)      347 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/mypy.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/pyproject.toml
+-rw-r--r--   0 jenkins    (115) docker     (999)      248 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/pytest.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)       90 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       96 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      292 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/requirements.txt
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:50:23.000000 swh.loader.svn-1.8.0/resources/
+-rw-r--r--   0 jenkins    (115) docker     (999)      860 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/resources/svn.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-06-06 12:50:23.000000 swh.loader.svn-1.8.0/setup.cfg
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     5522 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/setup.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5873 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/svn-lib-client-analysis.org
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:50:23.000000 swh.loader.svn-1.8.0/swh/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:50:23.000000 swh.loader.svn-1.8.0/swh/loader/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:50:23.000000 swh.loader.svn-1.8.0/swh/loader/svn/
+-rw-r--r--   0 jenkins    (115) docker     (999)      491 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2427 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/converters.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2334 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/directory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      667 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/exception.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     9055 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/fast_crawler.cpp
+-rw-r--r--   0 jenkins    (115) docker     (999)      515 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/fast_crawler.pyi
+-rw-r--r--   0 jenkins    (115) docker     (999)    33376 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/loader.py
+-rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/py.typed
+-rw-r--r--   0 jenkins    (115) docker     (999)    33988 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/replay.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    25221 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/svn_repo.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1521 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/svn_retry.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1785 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:50:23.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2690 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:50:23.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/data/
+-rw-r--r--   0 jenkins    (115) docker     (999)   360057 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/data/httthttt.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)   389343 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/data/mediawiki-repo-r407-eol-native-crlf.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)      201 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/data/penguinsdbtools2018.dump.gz
+-rw-r--r--   0 jenkins    (115) docker     (999)   419840 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pkg-doc-linux-r10.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)   430080 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pkg-doc-linux-r11.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)   911360 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pkg-doc-linux-r12.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)    28495 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pkg-gourmet-add-remove-dir.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)   133120 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pkg-gourmet-tampered-rev6-log.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)   163840 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pkg-gourmet-with-edge-case-links-and-files.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)    35440 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pkg-gourmet-with-external-id.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)    30908 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pkg-gourmet-with-updates.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)   163840 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pkg-gourmet-with-wrong-link-cases.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)    28193 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pkg-gourmet.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)   406052 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pyang-repo-r343-eol-native-mixed-lf-crlf.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)     3985 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/test_converters.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4548 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/test_directory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    62193 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/test_externals.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2371 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/test_fast_crawler.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    17874 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/test_loader.org
+-rw-r--r--   0 jenkins    (115) docker     (999)    79798 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/test_loader.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4415 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/test_svn_repo.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    12997 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/test_svn_retry.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2338 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/test_task.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1475 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/test_task_directory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    21336 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/test_utils.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3734 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/utils.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    16004 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/utils.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:50:23.000000 swh.loader.svn-1.8.0/swh.loader.svn.egg-info/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2023 2023-06-06 12:50:23.000000 swh.loader.svn-1.8.0/swh.loader.svn.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     2471 2023-06-06 12:50:23.000000 swh.loader.svn-1.8.0/swh.loader.svn.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-06-06 12:50:23.000000 swh.loader.svn-1.8.0/swh.loader.svn.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       51 2023-06-06 12:50:23.000000 swh.loader.svn-1.8.0/swh.loader.svn.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      250 2023-06-06 12:50:23.000000 swh.loader.svn-1.8.0/swh.loader.svn.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-06-06 12:50:23.000000 swh.loader.svn-1.8.0/swh.loader.svn.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1531 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/tox.ini
```

### Comparing `swh.loader.svn-1.7.0/.pre-commit-config.yaml` & `swh.loader.svn-1.8.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.7.0/CODE_OF_CONDUCT.md` & `swh.loader.svn-1.8.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.7.0/LICENSE` & `swh.loader.svn-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.7.0/PKG-INFO` & `swh.loader.svn-1.8.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.loader.svn
-Version: 1.7.0
+Version: 1.8.0
 Summary: Software Heritage Loader SVN
 Home-page: https://forge.softwareheritage.org/diffusion/DLDSVN
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-loader-svn
@@ -33,14 +33,17 @@
 
 - `swh.loader.svn.loader.SvnLoaderFromDumpArchive` which mounts a repository out of a
   svn dump prior to ingest it.
 
 - `swh.loader.svn.loader.SvnLoaderFromRemoteDump` which mounts a repository with
   svnrdump prior to ingest its content.
 
+- `swh.loader.svn.directory.SvnDirectoryLoader` which ingests an svn tree at a specific
+  revision.
+
 ## CLI run
 
 With the configuration:
 
 /tmp/loader_svn.yml:
 ```yml
 storage:
```

### Comparing `swh.loader.svn-1.7.0/README.md` & `swh.loader.svn-1.8.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 
 - `swh.loader.svn.loader.SvnLoaderFromDumpArchive` which mounts a repository out of a
   svn dump prior to ingest it.
 
 - `swh.loader.svn.loader.SvnLoaderFromRemoteDump` which mounts a repository with
   svnrdump prior to ingest its content.
 
+- `swh.loader.svn.directory.SvnDirectoryLoader` which ingests an svn tree at a specific
+  revision.
+
 ## CLI run
 
 With the configuration:
 
 /tmp/loader_svn.yml:
 ```yml
 storage:
```

### Comparing `swh.loader.svn-1.7.0/bin/init-svn-repository.sh` & `swh.loader.svn-1.8.0/bin/init-svn-repository.sh`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.7.0/bin/swh-svn` & `swh.loader.svn-1.8.0/bin/swh-svn`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.7.0/conftest.py` & `swh.loader.svn-1.8.0/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.7.0/docs/swh-loader-svn.txt` & `swh.loader.svn-1.8.0/docs/swh-loader-svn.txt`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.7.0/install/install-pysvn.sh` & `swh.loader.svn-1.8.0/install/install-pysvn.sh`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.7.0/resources/svn.ini` & `swh.loader.svn-1.8.0/resources/svn.ini`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.7.0/setup.py` & `swh.loader.svn-1.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.7.0/svn-lib-client-analysis.org` & `swh.loader.svn-1.8.0/svn-lib-client-analysis.org`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.7.0/swh/loader/svn/converters.py` & `swh.loader.svn-1.8.0/swh/loader/svn/converters.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.7.0/swh/loader/svn/exception.py` & `swh.loader.svn-1.8.0/swh/loader/svn/exception.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.7.0/swh/loader/svn/fast_crawler.cpp` & `swh.loader.svn-1.8.0/swh/loader/svn/fast_crawler.cpp`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.7.0/swh/loader/svn/fast_crawler.pyi` & `swh.loader.svn-1.8.0/swh/loader/svn/fast_crawler.pyi`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.7.0/swh/loader/svn/loader.py` & `swh.loader.svn-1.8.0/swh/loader/svn/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,20 +13,18 @@
 import pty
 import re
 import shutil
 from subprocess import PIPE, Popen
 import tempfile
 from typing import Any, Dict, Iterator, List, Optional, Sequence, Tuple
 
-from subvertpy import SubversionException
-
 from swh.loader.core.loader import BaseLoader
 from swh.loader.core.utils import clean_dangling_folders
 from swh.loader.exception import NotFound
-from swh.loader.svn.svn_repo import SvnRepo
+from swh.loader.svn.svn_repo import get_svn_repo
 from swh.model import from_disk, hashutil
 from swh.model.model import (
     Content,
     Directory,
     Revision,
     SkippedContent,
     Snapshot,
@@ -112,15 +110,14 @@
         self._load_status = "uneventful"
         self.visit_date = visit_date or self.visit_date
         self.incremental = incremental
         self.snapshot: Optional[Snapshot] = None
         # state from previous visit
         self.latest_snapshot = None
         self.latest_revision: Optional[Revision] = None
-        self.from_dump = False
 
     def pre_cleanup(self):
         """Cleanup potential dangling files from prior runs (e.g. OOM killed
         tasks)
 
         """
         clean_dangling_folders(
@@ -439,49 +436,31 @@
             yield _contents, _skipped_contents, _directories, swh_revision
 
         if not self.debug and self.svnrepo:
             # clean directory where revisions were replayed to gain some disk space
             # before the post_load operation
             self.svnrepo.clean_fs(self.svnrepo.local_url)
 
-    def svn_repo(self, *args, **kwargs):
-        """Wraps the creation of SvnRepo object and handles not found repository
-        errors."""
-        try:
-            return SvnRepo(*args, **kwargs)
-        except SubversionException as e:
-            error_msgs = [
-                "Unable to connect to a repository at URL",
-                "Unknown URL type",
-                "is not a working copy",
-            ]
-            for msg in error_msgs:
-                if msg in e.args[0]:
-                    self._load_status = "uneventful"
-                    raise NotFound(e)
-            raise
-
     def prepare(self):
         latest_snapshot_revision = self._latest_snapshot_revision(self.origin.url)
         if latest_snapshot_revision:
             self.latest_snapshot, self.latest_revision = latest_snapshot_revision
             self._snapshot = self.latest_snapshot
             if self.incremental:
                 self._last_revision = self.latest_revision
             else:
                 self.latest_revision = None
 
         local_dirname = self._create_tmp_dir(self.temp_directory)
 
-        self.svnrepo = self.svn_repo(
+        self.svnrepo = get_svn_repo(
             self.svn_url,
             self.origin.url,
             local_dirname,
             self.max_content_size,
-            self.from_dump,
             debug=self.debug,
         )
 
         try:
             revision_start, revision_end = self.start_from()
             self.swh_revision_gen = self.process_svn_revisions(
                 self.svnrepo, revision_start, revision_end
@@ -656,15 +635,14 @@
             debug=debug,
             check_revision=check_revision,
             **kwargs,
         )
         self.archive_path = archive_path
         self.temp_dir = None
         self.repo_path = None
-        self.from_dump = True
 
     def prepare(self):
         self.log.info("Archive to mount and load %s", self.archive_path)
         self.temp_dir, self.repo_path = init_svn_repo_from_archive_dump(
             self.archive_path,
             prefix=TEMPORARY_DIR_PREFIX_PATTERN,
             suffix="-%s" % os.getpid(),
@@ -710,15 +688,14 @@
             incremental=incremental,
             visit_date=visit_date,
             temp_directory=temp_directory,
             debug=debug,
             check_revision=check_revision,
             **kwargs,
         )
-        self.from_dump = True
         self.temp_dir = self._create_tmp_dir(self.temp_directory)
         self.repo_path = None
         self.truncated_dump = False
 
     def get_last_loaded_svn_rev(self, svn_url: str) -> int:
         """Check if the svn repository has already been visited and return the last
         loaded svn revision number or -1 otherwise.
@@ -846,21 +823,20 @@
         )
 
     def prepare(self):
         # First, check if previous revisions have been loaded for the
         # subversion origin and get the number of the last one
         last_loaded_svn_rev = self.get_last_loaded_svn_rev(self.origin.url)
 
-        self.svnrepo = self.svn_repo(
+        self.svnrepo = get_svn_repo(
             self.origin.url,
             self.origin.url,
             self.temp_dir,
             self.max_content_size,
             debug=self.debug,
-            from_dump=True,
         )
 
         # Ensure to use remote URL retrieved by SvnRepo as origin URL might redirect
         # and svnrdump does not handle URL redirection
         self.svn_url = self.svnrepo.remote_url
 
         # Then for stale repository, check if the last loaded revision in the archive
```

### Comparing `swh.loader.svn-1.7.0/swh/loader/svn/replay.py` & `swh.loader.svn-1.8.0/swh/loader/svn/replay.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,16 +117,17 @@
 
         """
         if self.editor.debug:
             logger.debug("Closing file %s", self.path)
 
         if self.path not in self.editor.external_paths:
             # export file to disk if its path does not match an external
+            url = svn_urljoin(self.svnrepo.repos_root_url, os.fsdecode(self.path))
             self.svnrepo.export(
-                os.path.join(self.svnrepo.remote_url, os.fsdecode(self.path)),
+                url,
                 to=self.fullpath,
                 rev=self.editor.revnum,
                 peg_rev=self.editor.revnum,
                 ignore_keywords=True,
                 overwrite=True,
             )
 
@@ -176,14 +177,16 @@
         svnrepo: SvnRepo,
     ):
         self.directory = directory
         self.rootpath = rootpath
         self.path = path
         # build directory on init
         os.makedirs(rootpath, exist_ok=True)
+        if path and path not in self.directory:
+            self.directory[path] = from_disk.Directory()
         self.dir_states = dir_states
         self.svnrepo = svnrepo
         self.editor = svnrepo.swhreplay.editor
         self.externals: Dict[str, List[ExternalDefinition]] = {}
 
     def remove_child(self, path: bytes) -> None:
         """Remove a path from the current objects.
@@ -235,15 +238,15 @@
         fullpath = os.path.join(self.rootpath, path_bytes)
 
         os.makedirs(fullpath, exist_ok=True)
         if copyfrom_rev == -1:
             if path_bytes and path_bytes not in self.directory:
                 self.directory[path_bytes] = from_disk.Directory()
         else:
-            url = svn_urljoin(self.svnrepo.remote_url, copyfrom_path)
+            url = svn_urljoin(self.svnrepo.repos_root_url, copyfrom_path)
             self.remove_child(path_bytes)
             self.svnrepo.export(
                 url,
                 to=fullpath,
                 peg_rev=copyfrom_rev,
                 ignore_keywords=True,
                 overwrite=True,
@@ -328,15 +331,15 @@
 
         path_bytes = os.fsencode(path)
         fullpath = os.path.join(self.rootpath, path_bytes)
 
         if copyfrom_rev == -1:
             self.directory[path_bytes] = from_disk.Content()
         else:
-            url = svn_urljoin(self.svnrepo.remote_url, copyfrom_path)
+            url = svn_urljoin(self.svnrepo.repos_root_url, copyfrom_path)
             self.remove_child(path_bytes)
             self.svnrepo.export(
                 url,
                 to=fullpath,
                 peg_rev=copyfrom_rev,
                 ignore_keywords=True,
                 overwrite=True,
@@ -707,29 +710,30 @@
         if remove_subpaths:
             subpath_split = fullpath.split(b"/")[:-1]
             for i in reversed(range(1, len(subpath_split) + 1)):
                 # delete external sub-directory only if it is not versioned
                 subpath = b"/".join(subpath_split[0:i])
                 try:
                     self.svnrepo.info(
-                        svn_urljoin(self.svnrepo.remote_url, os.fsdecode(subpath)),
+                        svn_urljoin(self.svnrepo.repos_root_url, os.fsdecode(subpath)),
                         peg_revision=self.editor.revnum,
                         revision=self.editor.revnum,
                     )
                 except SubversionException:
                     self.remove_child(subpath)
                 else:
                     break
 
         try:
             # externals can overlap with versioned files so we must restore
             # them after removing the path above
             dest_path = os.path.join(self.rootpath, fullpath)
+            url = svn_urljoin(self.svnrepo.repos_root_url, os.fsdecode(fullpath))
             self.svnrepo.export(
-                svn_urljoin(self.svnrepo.remote_url, os.fsdecode(fullpath)),
+                url,
                 to=dest_path,
                 peg_rev=self.editor.revnum,
                 ignore_keywords=True,
                 remove_dest_path=False,
             )
             if os.path.isfile(dest_path) or os.path.islink(dest_path):
                 self.directory[fullpath] = from_disk.Content.from_file(path=dest_path)
```

### Comparing `swh.loader.svn-1.7.0/swh/loader/svn/svn_repo.py` & `swh.loader.svn-1.8.0/swh/loader/svn/svn_repo.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from subvertpy.ra import (
     Auth,
     RemoteAccess,
     get_simple_prompt_provider,
     get_username_provider,
 )
 
+from swh.loader.exception import NotFound
 from swh.model.from_disk import Directory as DirectoryFromDisk
 from swh.model.model import Content, Directory, SkippedContent
 
 from . import converters, fast_crawler, replay
 from .svn_retry import svn_retry
 from .utils import is_recursive_external, parse_external_definition
 
@@ -55,74 +56,73 @@
 
     def __init__(
         self,
         remote_url: str,
         origin_url: Optional[str] = None,
         local_dirname: Optional[str] = None,
         max_content_length: int = 100000,
-        from_dump: bool = False,
         debug: bool = False,
+        username: str = "",
+        password: str = "",
     ):
         if origin_url is None:
             origin_url = remote_url
 
         self.manage_directory = False
         if local_dirname is None:
             local_dirname = tempfile.mkdtemp()
             self.manage_directory = True
         self.local_dirname = local_dirname
 
         self.origin_url = origin_url
-        self.from_dump = from_dump
 
         # default auth provider for anonymous access
         auth_providers = [get_username_provider()]
 
         # check if basic auth is required
         parsed_origin_url = urlparse(origin_url)
-        self.username = parsed_origin_url.username or ""
-        self.password = parsed_origin_url.password or ""
+        self.username = parsed_origin_url.username or username
+        self.password = parsed_origin_url.password or password
+
         if self.username:
             # add basic auth provider for username/password
             auth_providers.append(
                 get_simple_prompt_provider(
                     lambda realm, uname, may_save: (
                         self.username,
                         self.password,
                         False,
                     ),
                     0,
                 )
             )
 
-            # we need to remove the authentication part in the origin URL to avoid
-            # errors when calling subversion API through subvertpy
-            self.origin_url = urlunparse(
-                parsed_origin_url._replace(
-                    netloc=parsed_origin_url.netloc.split("@", 1)[1]
+            if "@" in origin_url:
+                # we need to remove the authentication part in the origin URL to avoid
+                # errors when calling subversion API through subvertpy
+                self.origin_url = urlunparse(
+                    parsed_origin_url._replace(
+                        netloc=parsed_origin_url.netloc.split("@", 1)[1]
+                    )
                 )
-            )
-            if origin_url == remote_url:
-                remote_url = self.origin_url
+                if origin_url == remote_url:
+                    remote_url = self.origin_url
 
         self.remote_url = remote_url.rstrip("/")
 
         self.auth = Auth(auth_providers)
         # one client for update operation
         self.client = client.Client(auth=self.auth)
 
         if not self.remote_url.startswith("file://"):
             # use redirection URL if any for remote operations
             self.remote_url = self.info(self.remote_url).url
 
         self.remote_access_url = self.remote_url
 
-        if not self.from_dump:
-            self.remote_url = self.info(self.remote_url).repos_root_url
-
         local_name = os.path.basename(self.remote_url)
         self.local_url = os.path.join(self.local_dirname, local_name).encode("utf-8")
 
         conn = self.remote_access()
         self.uuid = conn.get_uuid().encode("utf-8")
         self.swhreplay = replay.Replay(
             conn=conn,
@@ -132,20 +132,20 @@
             debug=debug,
         )
         self.max_content_length = max_content_length
         self.has_relative_externals = False
         self.has_recursive_externals = False
         self.replay_started = False
 
-        # compute root directory path from the remote repository URL, required to
+        # compute root directory path from the origin URL, required to
         # properly load the sub-tree of a repository mounted from a dump file
-        self.repos_root_url = self.info(self.origin_url).repos_root_url
-        self.root_directory = self.origin_url.rstrip("/").replace(
-            self.repos_root_url, "", 1
-        )
+        repos_root_url = self.info(self.origin_url).repos_root_url
+        self.root_directory = self.origin_url.rstrip("/").replace(repos_root_url, "", 1)
+        # get root repository URL from the remote URL
+        self.repos_root_url = self.info(self.remote_url).repos_root_url
 
     def __del__(self):
         # ensure temporary directory is removed when created by constructor
         if self.manage_directory:
             self.clean_fs()
 
     def __str__(self):
@@ -175,21 +175,17 @@
 
         author = converters.svn_author_to_swh_person(
             revprops.get(properties.PROP_REVISION_AUTHOR)
         )
 
         message = revprops.get(properties.PROP_REVISION_LOG, DEFAULT_AUTHOR_MESSAGE)
 
-        has_changes = (
-            not self.from_dump
-            or changed_paths is not None
-            and any(
-                changed_path.startswith(self.root_directory)
-                for changed_path in changed_paths.keys()
-            )
+        has_changes = changed_paths is not None and any(
+            changed_path.startswith(self.root_directory)
+            for changed_path in changed_paths.keys()
         )
 
         return {
             "rev": rev,
             "author_date": author_date,
             "author_name": author,
             "message": message,
@@ -652,7 +648,50 @@
                 commit_info = self.svn_repo.commit_info(self.rev_ids[i])
                 return commit_info["author_date"].to_datetime()
 
         if self.commit_info(1)["author_date"].to_datetime() > date:
             raise ValueError("First revision date is greater than reference date")
 
         return bisect.bisect_right(RevisionList(self), date)
+
+
+def get_svn_repo(*args, **kwargs):
+    """Instantiate an SvnRepo class and trap SubversionException if any raises.
+    In case of connection error to the repository, its read access using anonymous
+    credentials is also attempted.
+
+    Raises:
+        NotFound: if the repository is not found
+        SubversionException: if any other kind of subversion problems arise
+    """
+    credentials = [(None, None), ("anonymous", ""), ("anonymous", "anonymous")]
+    for i, (username, password) in enumerate(credentials):
+        try:
+            if username is not None:
+                logger.debug(
+                    "Retrying to connect to %s with username '%s' and password '%s'",
+                    args[0],
+                    username,
+                    password,
+                )
+                kwargs["username"] = username
+                kwargs["password"] = password
+            return SvnRepo(*args, **kwargs)
+        except SubversionException as e:
+            connection_error_message = "Unable to connect to a repository at URL"
+            error_msgs = [
+                "Unknown URL type",
+                "is not a working copy",
+            ]
+            # no more credentials to test, raise NotFound
+            if i == len(credentials) - 1:
+                error_msgs.append(connection_error_message)
+            for msg in error_msgs:
+                if msg in e.args[0]:
+                    raise NotFound(e)
+
+            if connection_error_message in e.args[0]:
+                # still some credentials to test, continue attempting to connect
+                # to the repository
+                continue
+            else:
+                raise
```

### Comparing `swh.loader.svn-1.7.0/swh/loader/svn/svn_retry.py` & `swh.loader.svn-1.8.0/swh/loader/svn/svn_retry.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.7.0/swh/loader/svn/tasks.py` & `swh.loader.svn-1.8.0/swh/loader/svn/tasks.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-# Copyright (C) 2015-2022  The Software Heritage developers
+# Copyright (C) 2015-2023  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 
 from celery import shared_task
 
 from swh.loader.core.utils import parse_visit_date
 
+from .directory import SvnDirectoryLoader
 from .loader import SvnLoader, SvnLoaderFromDumpArchive, SvnLoaderFromRemoteDump
 
 
 def _process_kwargs(kwargs):
     if "visit_date" in kwargs:
         kwargs["visit_date"] = parse_visit_date(kwargs["visit_date"])
     return kwargs
@@ -40,7 +41,14 @@
     """
     1. Mount a remote svn dump as a local svn repository.
     2. Load it through the svn loader.
     3. Clean up mounted svn repository archive.
     """
     loader = SvnLoaderFromRemoteDump.from_configfile(**_process_kwargs(kwargs))
     return loader.load()
+
+
+@shared_task(name=f"{__name__}.LoadSvnDirectory")
+def load_svn_directory(**kwargs):
+    """Load svn tree into the swh archive."""
+    loader = SvnDirectoryLoader.from_configfile(**_process_kwargs(kwargs))
+    return loader.load()
```

### Comparing `swh.loader.svn-1.7.0/swh/loader/svn/tests/conftest.py` & `swh.loader.svn-1.8.0/swh/loader/svn/tests/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 # Copyright (C) 2019-2023  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import subprocess
 from typing import Any, Dict
+import uuid
 
 import pytest
 
-from swh.loader.svn.loader import SvnLoader, SvnLoaderFromRemoteDump, SvnRepo
+from swh.loader.svn.loader import SvnLoader, SvnLoaderFromRemoteDump
+from swh.loader.svn.svn_repo import SvnRepo
+from swh.scheduler.model import Lister
 
 from .utils import create_repo
 
+NAMESPACE = "swh.loader.svn"
+
 
 @pytest.fixture(params=[SvnLoader, SvnLoaderFromRemoteDump])
 def svn_loader_cls(request):
     return request.param
 
 
 @pytest.fixture
@@ -84,7 +89,12 @@
                 repo_root,
             ]
         )
 
     yield run_svnserve
 
     svnserve_proc.terminate()
+
+
+@pytest.fixture
+def svn_lister():
+    return Lister(name="svn-lister", instance_name="example", id=uuid.uuid4())
```

### Comparing `swh.loader.svn-1.7.0/swh/loader/svn/tests/data/httthttt.tgz` & `swh.loader.svn-1.8.0/swh/loader/svn/tests/data/httthttt.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.7.0/swh/loader/svn/tests/data/mediawiki-repo-r407-eol-native-crlf.tgz` & `swh.loader.svn-1.8.0/swh/loader/svn/tests/data/mediawiki-repo-r407-eol-native-crlf.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pkg-doc-linux-r10.tgz` & `swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pkg-doc-linux-r10.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pkg-doc-linux-r11.tgz` & `swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pkg-doc-linux-r11.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pkg-doc-linux-r12.tgz` & `swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pkg-doc-linux-r12.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pkg-gourmet-add-remove-dir.tgz` & `swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pkg-gourmet-add-remove-dir.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pkg-gourmet-tampered-rev6-log.tgz` & `swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pkg-gourmet-tampered-rev6-log.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pkg-gourmet-with-edge-case-links-and-files.tgz` & `swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pkg-gourmet-with-edge-case-links-and-files.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pkg-gourmet-with-external-id.tgz` & `swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pkg-gourmet-with-external-id.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pkg-gourmet-with-updates.tgz` & `swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pkg-gourmet-with-updates.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pkg-gourmet-with-wrong-link-cases.tgz` & `swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pkg-gourmet-with-wrong-link-cases.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pkg-gourmet.tgz` & `swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pkg-gourmet.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.7.0/swh/loader/svn/tests/data/pyang-repo-r343-eol-native-mixed-lf-crlf.tgz` & `swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pyang-repo-r343-eol-native-mixed-lf-crlf.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.7.0/swh/loader/svn/tests/test_converters.py` & `swh.loader.svn-1.8.0/swh/loader/svn/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.7.0/swh/loader/svn/tests/test_externals.py` & `swh.loader.svn-1.8.0/swh/loader/svn/tests/test_externals.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.7.0/swh/loader/svn/tests/test_fast_crawler.py` & `swh.loader.svn-1.8.0/swh/loader/svn/tests/test_fast_crawler.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.7.0/swh/loader/svn/tests/test_loader.org` & `swh.loader.svn-1.8.0/swh/loader/svn/tests/test_loader.org`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.7.0/swh/loader/svn/tests/test_loader.py` & `swh.loader.svn-1.8.0/swh/loader/svn/tests/test_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         "Unknown URL type",
     ],
 )
 def test_loader_svn_not_found(
     svn_loader_cls, swh_storage, tmp_path, exception_msg, mocker
 ):
     """Given unknown repository issues, the loader visit ends up in status not_found"""
-    mock = mocker.patch("swh.loader.svn.loader.SvnRepo")
+    mock = mocker.patch("swh.loader.svn.svn_repo.SvnRepo")
     mock.side_effect = SubversionException(exception_msg, 0)
 
     unknown_repo_url = "unknown-repository"
     loader = svn_loader_cls(swh_storage, unknown_repo_url, temp_directory=tmp_path)
 
     assert loader.load() == {"status": "uneventful"}
 
@@ -102,15 +102,15 @@
         SubversionException("Irrelevant message, considered a failure", 10),
         SubversionException("Present but fails to read, considered a failure", 20),
         ValueError("considered a failure"),
     ],
 )
 def test_loader_svn_failures(svn_loader_cls, swh_storage, tmp_path, exception, mocker):
     """Given any errors raised, the loader visit ends up in status failed"""
-    mock = mocker.patch("swh.loader.svn.loader.SvnRepo")
+    mock = mocker.patch("swh.loader.svn.svn_repo.SvnRepo")
     mock.side_effect = exception
 
     existing_repo_url = "existing-repo-url"
     loader = svn_loader_cls(swh_storage, existing_repo_url, temp_directory=tmp_path)
 
     assert loader.load() == {"status": "failed"}
 
@@ -1302,17 +1302,15 @@
     svn_loader_cls, swh_storage, mocker, repo_url, tmp_path
 ):
     class SvnRepoSkipFirstRevision(SvnRepo):
         def logs(self, revision_start, revision_end):
             """Overrides logs method to skip revision number one in yielded revisions"""
             yield from super().logs(revision_start + 1, revision_end)
 
-    from swh.loader.svn import loader
-
-    mocker.patch.object(loader, "SvnRepo", SvnRepoSkipFirstRevision)
+    mocker.patch("swh.loader.svn.svn_repo.SvnRepo", SvnRepoSkipFirstRevision)
 
     for filename in ("foo", "bar", "baz"):
         add_commit(
             repo_url,
             f"Add {filename} file",
             [
                 CommitChange(
@@ -1647,15 +1645,17 @@
                 for root, _, files in os.walk(self.local_url)
                 for name in files
             ]
             yield from super().swh_hash_data_per_revision(start_revision, end_revision)
 
     from swh.loader.svn import loader
 
-    mocker.patch.object(loader, "SvnRepo", SvnRepoCheckReplayStartWithEmptyDirectory)
+    mocker.patch(
+        "swh.loader.svn.svn_repo.SvnRepo", SvnRepoCheckReplayStartWithEmptyDirectory
+    )
 
     # second load, incremental
     loader = svn_loader_cls(swh_storage, repo_url, temp_directory=tmp_path)
     loader.load()
 
     # check work directory was empty before replaying revisions
     assert loader.svnrepo.replay_dir_content_before_start == []
@@ -1938,50 +1938,50 @@
     # first commit
     add_commit(
         repo_url,
         "Add first project in repository",
         [
             CommitChange(
                 change_type=CommitChangeType.AddOrUpdate,
-                path="project1/foo.sh",
+                path="projects/project1/foo.sh",
                 data=b"#!/bin/bash\necho foo",
             ),
         ],
     )
 
     # second commit
     add_commit(
         repo_url,
         "Add second project in repository",
         [
             CommitChange(
                 change_type=CommitChangeType.AddOrUpdate,
-                path="project2/bar.sh",
+                path="projects/project2/bar.sh",
                 data=b"#!/bin/bash\necho bar",
             ),
         ],
     )
 
     # third commit
     add_commit(
         repo_url,
         "Add third project in repository",
         [
             CommitChange(
                 change_type=CommitChangeType.AddOrUpdate,
-                path="project3/baz.sh",
+                path="projects/project3/baz.sh",
                 data=b"#!/bin/bash\necho baz",
             ),
         ],
     )
 
     for i in range(1, 4):
         # load each project in the repository separately and check behavior
         # is the same if origin URL has a trailing slash or not
-        origin_url = f"{repo_url}/project{i}{'/' if i%2 else ''}"
+        origin_url = f"{repo_url}/projects/project{i}{'/' if i%2 else ''}"
 
         loader_params = {
             "storage": swh_storage,
             "url": origin_url,
             "origin_url": origin_url,
             "temp_directory": tmp_path,
             "incremental": True,
@@ -2001,28 +2001,36 @@
             loader.storage,
             origin_url,
             status="full",
             type="svn",
         )
         check_snapshot(loader.snapshot, loader.storage)
 
+        # check that head revision targets a directory with a single file
+        head_rev_id = loader.snapshot.branches[b"HEAD"].target
+        head_rev = swh_storage.revision_get([head_rev_id])[0]
+        root_dir = list(swh_storage.directory_ls(head_rev.directory))
+        assert len(root_dir) == 1 and root_dir[0]["type"] == "file"
+
         if svn_loader_cls == SvnLoaderFromRemoteDump:
             dump_revisions.assert_called_once_with(origin_url.rstrip("/"), -1)
 
         if svn_loader_cls == SvnLoaderFromDumpArchive:
             loader_params["archive_path"] = _dump_project(tmp_path, origin_url)
 
         loader = svn_loader_cls(**loader_params)
 
         assert loader.load() == {"status": "uneventful"}
 
         # each project origin must have
         assert get_stats(loader.storage) == {
             "content": i,  # one content
-            "directory": 2 * i,  # two directories
+            # three directories (we load them all but head revision is rooted to
+            # the subproject directory)
+            "directory": 3 * i,
             "origin": i,
             "origin_visit": 2 * i,  # two visits
             "release": 0,
             "revision": i,  # one revision
             "skipped_content": 0,
             "snapshot": i,  # one snapshot
         }
@@ -2166,16 +2174,19 @@
     # prepare loading
     loader.prepare()
 
     # check redirection URL has been used to dump repository
     assert loader.dump_svn_revisions.call_args_list[0][0][0] == repo_redirect_url
 
 
+@pytest.mark.parametrize(
+    "credentials", [("johndoe", "toto"), ("anonymous", "anonymous")]
+)
 def test_loader_basic_authentication_required(
-    swh_storage, repo_url, tmp_path, svn_loader_cls, svnserve
+    swh_storage, repo_url, tmp_path, svn_loader_cls, svnserve, credentials
 ):
 
     # add file to empty test repo
     add_commit(
         repo_url,
         "Add project in repository",
         [
@@ -2187,16 +2198,15 @@
         ],
     )
 
     # compute repo URLs that will be made available by svnserve
     repo_path = repo_url.replace("file://", "")
     repo_root = os.path.dirname(repo_path)
     repo_name = os.path.basename(repo_path)
-    username = "anonymous"
-    password = "anonymous"
+    username, password = credentials
     port = 12000
     repo_url_no_auth = f"svn://localhost:{port}/{repo_name}"
     repo_url = f"svn://{username}:{password}@localhost:{port}/{repo_name}"
 
     # disable anonymous access and require authentication on test repo
     with open(os.path.join(repo_path, "conf", "svnserve.conf"), "w") as svnserve_conf:
         svnserve_conf.write(
@@ -2220,17 +2230,21 @@
     # add a user with read/write access on test repo
     with open(os.path.join(repo_path, "conf", "passwd"), "w") as passwd:
         passwd.write(f"[users]\n{username} = {password}")
 
     # execute svnserve
     svnserve(repo_root, port)
 
-    # check loading failed with no authentication
+    # check loading failed with no authentication in URL apart for anonymous credentials
     loader = svn_loader_cls(swh_storage, repo_url_no_auth, temp_directory=tmp_path)
-    assert loader.load() == {"status": "uneventful"}
+    assert (
+        loader.load() == {"status": "uneventful"}
+        if username != "anonymous"
+        else {"status": "eventful"}
+    )
 
     # check loading succeeded with authentication
     loader = svn_loader_cls(swh_storage, repo_url, temp_directory=tmp_path)
     assert loader.load() == {"status": "eventful"}
     assert_last_visit_matches(
         loader.storage,
         repo_url,
```

### Comparing `swh.loader.svn-1.7.0/swh/loader/svn/tests/test_svn_repo.py` & `swh.loader.svn-1.8.0/swh/loader/svn/tests/test_svn_repo.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,27 +11,33 @@
 
 from swh.loader.svn.svn_repo import SvnRepo
 
 from .utils import CommitChange, CommitChangeType, add_commit
 
 FIRST_COMMIT_DATE = datetime(year=2019, month=1, day=1, tzinfo=timezone.utc)
 NB_DAYS_BETWEEN_COMMITS = 2
+FILENAMES = ("foo", "bar", "baz")
 COMMITS = [
     {
-        "message": f"Create trunk/{file} file",
+        "message": f"Create trunk/{file} file and tags/1.0/{file}",
         "date": FIRST_COMMIT_DATE + i * timedelta(days=NB_DAYS_BETWEEN_COMMITS),
         "changes": [
             CommitChange(
                 change_type=CommitChangeType.AddOrUpdate,
                 path=f"trunk/{file}",
                 data=file.encode(),
             ),
+            CommitChange(
+                change_type=CommitChangeType.AddOrUpdate,
+                path=f"tags/1.0/{file}",
+                data=file.encode(),
+            ),
         ],
     }
-    for i, file in enumerate(("foo", "bar", "baz"))
+    for i, file in enumerate(FILENAMES)
 ]
 
 
 @pytest.fixture
 def repo_url(repo_url):
     for commit in COMMITS:
         add_commit(
@@ -53,14 +59,19 @@
 
 
 @pytest.fixture
 def svn_repo(repo_url):
     return SvnRepo(repo_url)
 
 
+@pytest.fixture
+def svn_repo_first_tag(repo_url):
+    return SvnRepo(repo_url + "/tags/1.0")
+
+
 def test_svn_repo_head_revision(svn_repo):
     assert svn_repo.head_revision() == len(COMMITS)
 
 
 def _assert_commit(i, commit):
     assert commit["rev"] == i + 1
     assert commit["message"] == COMMITS[i]["message"].encode()
@@ -106,7 +117,25 @@
             )
             assert (
                 svn_repo.get_head_revision_at_date(
                     COMMITS[i]["date"] + timedelta(days=NB_DAYS_BETWEEN_COMMITS - 1)
                 )
                 == i + 1
             )
+
+
+def test_svn_repo_export_temporary_subproject(svn_repo_first_tag, mocker):
+    svn_repo_export = mocker.spy(svn_repo_first_tag, "export")
+    # export tags/1.0/ directory of the repository at HEAD revision
+    _, local_url = svn_repo_first_tag.export_temporary(len(COMMITS))
+    # check first tag URL was used as export URL
+    assert svn_repo_export.call_args_list[0][0][0].endswith("tags/1.0")
+    # get exported filesystem
+    export_content = list(os.walk(local_url))
+    # should be a single directory containing only files
+    assert len(export_content) == 1
+    _, subdirs, files = export_content[0]
+    assert len(subdirs) == 0
+    assert len(files) == len(FILENAMES)
+    # check that paths outside the export path were not exported
+    trunk_path = os.path.join(local_url, b"../../trunk")
+    assert not os.path.exists(trunk_path)
```

### Comparing `swh.loader.svn-1.7.0/swh/loader/svn/tests/test_svn_retry.py` & `swh.loader.svn-1.8.0/swh/loader/svn/tests/test_svn_retry.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.7.0/swh/loader/svn/tests/test_task.py` & `swh.loader.svn-1.8.0/swh/loader/svn/tests/test_task.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,17 @@
-# Copyright (C) 2019-2022  The Software Heritage developers
+# Copyright (C) 2019-2023  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
-import uuid
-
 import pytest
 
-from swh.scheduler.model import ListedOrigin, Lister
-
-NAMESPACE = "swh.loader.svn"
+from swh.scheduler.model import ListedOrigin
 
-
-@pytest.fixture
-def svn_lister():
-    return Lister(name="svn-lister", instance_name="example", id=uuid.uuid4())
+from .conftest import NAMESPACE
 
 
 @pytest.fixture
 def svn_listed_origin(svn_lister):
     return ListedOrigin(
         lister_id=svn_lister.id, url="svn://example.org/repo", visit_type="svn"
     )
```

### Comparing `swh.loader.svn-1.7.0/swh/loader/svn/tests/test_utils.py` & `swh.loader.svn-1.8.0/swh/loader/svn/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.7.0/swh/loader/svn/tests/utils.py` & `swh.loader.svn-1.8.0/swh/loader/svn/tests/utils.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.7.0/swh/loader/svn/utils.py` & `swh.loader.svn-1.8.0/swh/loader/svn/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -384,25 +384,25 @@
     Returns:
         the revision number of the HEAD revision at that date
 
     Raises:
         SubversionException: repository URL is not valid
         ValueError: first revision date is greater than given date
     """
-    from swh.loader.svn.svn_repo import SvnRepo
+    from swh.loader.svn.svn_repo import get_svn_repo
 
-    return SvnRepo(svn_url).get_head_revision_at_date(date)
+    return get_svn_repo(svn_url).get_head_revision_at_date(date)
 
 
 @lru_cache()
 def _get_repo_root_url(svn_url: str) -> str:
 
-    from swh.loader.svn.svn_repo import SvnRepo
+    from swh.loader.svn.svn_repo import get_svn_repo
 
-    return SvnRepo(svn_url).repos_root_url
+    return get_svn_repo(svn_url).repos_root_url
 
 
 def get_repo_root_url(svn_url):
     """Get root URL for a repository.
 
     Suversion URL might target a sub-project in a repository.
     That function computes the root URL of the repository and
```

### Comparing `swh.loader.svn-1.7.0/swh.loader.svn.egg-info/PKG-INFO` & `swh.loader.svn-1.8.0/swh.loader.svn.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.loader.svn
-Version: 1.7.0
+Version: 1.8.0
 Summary: Software Heritage Loader SVN
 Home-page: https://forge.softwareheritage.org/diffusion/DLDSVN
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-loader-svn
@@ -33,14 +33,17 @@
 
 - `swh.loader.svn.loader.SvnLoaderFromDumpArchive` which mounts a repository out of a
   svn dump prior to ingest it.
 
 - `swh.loader.svn.loader.SvnLoaderFromRemoteDump` which mounts a repository with
   svnrdump prior to ingest its content.
 
+- `swh.loader.svn.directory.SvnDirectoryLoader` which ingests an svn tree at a specific
+  revision.
+
 ## CLI run
 
 With the configuration:
 
 /tmp/loader_svn.yml:
 ```yml
 storage:
```

### Comparing `swh.loader.svn-1.7.0/swh.loader.svn.egg-info/SOURCES.txt` & `swh.loader.svn-1.8.0/swh.loader.svn.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -37,34 +37,37 @@
 swh.loader.svn.egg-info/dependency_links.txt
 swh.loader.svn.egg-info/entry_points.txt
 swh.loader.svn.egg-info/requires.txt
 swh.loader.svn.egg-info/top_level.txt
 swh/loader/__init__.py
 swh/loader/svn/__init__.py
 swh/loader/svn/converters.py
+swh/loader/svn/directory.py
 swh/loader/svn/exception.py
 swh/loader/svn/fast_crawler.cpp
 swh/loader/svn/fast_crawler.pyi
 swh/loader/svn/loader.py
 swh/loader/svn/py.typed
 swh/loader/svn/replay.py
 swh/loader/svn/svn_repo.py
 swh/loader/svn/svn_retry.py
 swh/loader/svn/tasks.py
 swh/loader/svn/utils.py
 swh/loader/svn/tests/__init__.py
 swh/loader/svn/tests/conftest.py
 swh/loader/svn/tests/test_converters.py
+swh/loader/svn/tests/test_directory.py
 swh/loader/svn/tests/test_externals.py
 swh/loader/svn/tests/test_fast_crawler.py
 swh/loader/svn/tests/test_loader.org
 swh/loader/svn/tests/test_loader.py
 swh/loader/svn/tests/test_svn_repo.py
 swh/loader/svn/tests/test_svn_retry.py
 swh/loader/svn/tests/test_task.py
+swh/loader/svn/tests/test_task_directory.py
 swh/loader/svn/tests/test_utils.py
 swh/loader/svn/tests/utils.py
 swh/loader/svn/tests/data/httthttt.tgz
 swh/loader/svn/tests/data/mediawiki-repo-r407-eol-native-crlf.tgz
 swh/loader/svn/tests/data/penguinsdbtools2018.dump.gz
 swh/loader/svn/tests/data/pkg-doc-linux-r10.tgz
 swh/loader/svn/tests/data/pkg-doc-linux-r11.tgz
```

### Comparing `swh.loader.svn-1.7.0/tox.ini` & `swh.loader.svn-1.8.0/tox.ini`

 * *Files identical despite different names*

