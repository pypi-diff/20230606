# Comparing `tmp/swh.loader.mercurial-3.1.1.tar.gz` & `tmp/swh.loader.mercurial-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swh.loader.mercurial-3.1.1.tar", last modified: Fri Apr 29 10:08:28 2022, max compression
+gzip compressed data, was "dist/swh.loader.mercurial-3.3.0.tar", last modified: Tue Jun  6 12:48:47 2023, max compression
```

## Comparing `swh.loader.mercurial-3.1.1.tar` & `swh.loader.mercurial-3.3.0.tar`

### file list

```diff
@@ -1,77 +1,80 @@
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-04-29 10:08:28.000000 swh.loader.mercurial-3.1.1/
--rw-r--r--   0 jenkins    (115) docker     (999)      140 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) docker     (999)      114 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      847 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)      117 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/AUTHORS
--rw-r--r--   0 jenkins    (115) docker     (999)     3397 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) docker     (999)       22 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) docker     (999)    35147 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/LICENSE
--rw-r--r--   0 jenkins    (115) docker     (999)      166 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/MANIFEST.in
--rw-r--r--   0 jenkins    (115) docker     (999)      163 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     1715 2022-04-29 10:08:28.000000 swh.loader.mercurial-3.1.1/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)      739 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/README.md
--rw-r--r--   0 jenkins    (115) docker     (999)      578 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-04-29 10:08:28.000000 swh.loader.mercurial-3.1.1/docs/
--rw-r--r--   0 jenkins    (115) docker     (999)       24 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/docs/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)       39 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/docs/Makefile
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-04-29 10:08:28.000000 swh.loader.mercurial-3.1.1/docs/_static/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-04-29 10:08:28.000000 swh.loader.mercurial-3.1.1/docs/_templates/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) docker     (999)       43 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/docs/conf.py
--rw-r--r--   0 jenkins    (115) docker     (999)      286 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/docs/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      498 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/mypy.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      237 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/pyproject.toml
--rw-r--r--   0 jenkins    (115) docker     (999)      172 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/pytest.ini
--rw-r--r--   0 jenkins    (115) docker     (999)       90 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      148 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/requirements-test.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      286 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/requirements.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      120 2022-04-29 10:08:28.000000 swh.loader.mercurial-3.1.1/setup.cfg
--rwxr-xr-x   0 jenkins    (115) docker     (999)     2454 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/setup.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-04-29 10:08:28.000000 swh.loader.mercurial-3.1.1/swh/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/swh/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-04-29 10:08:28.000000 swh.loader.mercurial-3.1.1/swh/loader/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/swh/loader/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-04-29 10:08:28.000000 swh.loader.mercurial-3.1.1/swh/loader/mercurial/
--rw-r--r--   0 jenkins    (115) docker     (999)      510 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/swh/loader/mercurial/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1981 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/swh/loader/mercurial/archive_extract.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1040 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/swh/loader/mercurial/converters.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4885 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/swh/loader/mercurial/hgutil.py
--rw-r--r--   0 jenkins    (115) docker     (999)    16630 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/swh/loader/mercurial/identify.py
--rw-r--r--   0 jenkins    (115) docker     (999)    29383 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/swh/loader/mercurial/loader.py
--rw-r--r--   0 jenkins    (115) docker     (999)       27 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/swh/loader/mercurial/py.typed
--rw-r--r--   0 jenkins    (115) docker     (999)     1119 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/swh/loader/mercurial/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-04-29 10:08:28.000000 swh.loader.mercurial-3.1.1/swh/loader/mercurial/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/swh/loader/mercurial/tests/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1470 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/swh/loader/mercurial/tests/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-04-29 10:08:28.000000 swh.loader.mercurial-3.1.1/swh/loader/mercurial/tests/data/
--rw-r--r--   0 jenkins    (115) docker     (999)  2757941 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/swh/loader/mercurial/tests/data/anomad-d.tgz
--rwxr-xr-x   0 jenkins    (115) docker     (999)     7621 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/swh/loader/mercurial/tests/data/build.py
--rw-r--r--   0 jenkins    (115) docker     (999)      897 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/swh/loader/mercurial/tests/data/example.json
--rw-r--r--   0 jenkins    (115) docker     (999)     1392 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/swh/loader/mercurial/tests/data/example.sh
--rw-r--r--   0 jenkins    (115) docker     (999)    51200 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/swh/loader/mercurial/tests/data/example.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)      411 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/swh/loader/mercurial/tests/data/hello.json
--rw-r--r--   0 jenkins    (115) docker     (999)     3070 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/swh/loader/mercurial/tests/data/hello.tgz
--rwxr-xr-x   0 jenkins    (115) docker     (999)      465 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/swh/loader/mercurial/tests/data/missing-filelog.sh
--rw-r--r--   0 jenkins    (115) docker     (999)    40960 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/swh/loader/mercurial/tests/data/missing-filelog.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)      456 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/swh/loader/mercurial/tests/data/multiple-heads.json
--rw-r--r--   0 jenkins    (115) docker     (999)      448 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/swh/loader/mercurial/tests/data/multiple-heads.sh
--rw-r--r--   0 jenkins    (115) docker     (999)    40960 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/swh/loader/mercurial/tests/data/multiple-heads.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)     5209 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/swh/loader/mercurial/tests/data/the-sandbox.json
--rw-r--r--   0 jenkins    (115) docker     (999)    13309 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/swh/loader/mercurial/tests/data/the-sandbox.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)      633 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/swh/loader/mercurial/tests/data/transplant.json
--rw-r--r--   0 jenkins    (115) docker     (999)     3206 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/swh/loader/mercurial/tests/data/transplant.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)     2353 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/swh/loader/mercurial/tests/loader_checker.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2155 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/swh/loader/mercurial/tests/test_converters.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3016 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/swh/loader/mercurial/tests/test_identify.py
--rw-r--r--   0 jenkins    (115) docker     (999)    24862 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/swh/loader/mercurial/tests/test_loader.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3272 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/swh/loader/mercurial/tests/test_tasks.py
--rw-r--r--   0 jenkins    (115) docker     (999)      886 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/swh/loader/mercurial/utils.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2022-04-29 10:08:28.000000 swh.loader.mercurial-3.1.1/swh.loader.mercurial.egg-info/
--rw-r--r--   0 jenkins    (115) docker     (999)     1715 2022-04-29 10:08:28.000000 swh.loader.mercurial-3.1.1/swh.loader.mercurial.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     2028 2022-04-29 10:08:28.000000 swh.loader.mercurial-3.1.1/swh.loader.mercurial.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        1 2022-04-29 10:08:28.000000 swh.loader.mercurial-3.1.1/swh.loader.mercurial.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      135 2022-04-29 10:08:28.000000 swh.loader.mercurial-3.1.1/swh.loader.mercurial.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      298 2022-04-29 10:08:28.000000 swh.loader.mercurial-3.1.1/swh.loader.mercurial.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        4 2022-04-29 10:08:28.000000 swh.loader.mercurial-3.1.1/swh.loader.mercurial.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1502 2022-04-29 10:08:25.000000 swh.loader.mercurial-3.1.1/tox.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:48:47.000000 swh.loader.mercurial-3.3.0/
+-rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) docker     (999)      114 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      848 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)      117 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/AUTHORS
+-rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) docker     (999)       22 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/LICENSE
+-rw-r--r--   0 jenkins    (115) docker     (999)      166 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/MANIFEST.in
+-rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     1799 2023-06-06 12:48:47.000000 swh.loader.mercurial-3.3.0/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)      860 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/README.md
+-rw-r--r--   0 jenkins    (115) docker     (999)      578 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:48:47.000000 swh.loader.mercurial-3.3.0/docs/
+-rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/docs/Makefile
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:48:47.000000 swh.loader.mercurial-3.3.0/docs/_static/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:48:47.000000 swh.loader.mercurial-3.3.0/docs/_templates/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/docs/conf.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      394 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/docs/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      548 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/mypy.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/pyproject.toml
+-rw-r--r--   0 jenkins    (115) docker     (999)      195 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/pytest.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)       90 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      148 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      333 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/requirements.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-06-06 12:48:47.000000 swh.loader.mercurial-3.3.0/setup.cfg
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     2454 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/setup.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:48:47.000000 swh.loader.mercurial-3.3.0/swh/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:48:47.000000 swh.loader.mercurial-3.3.0/swh/loader/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:48:47.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/
+-rw-r--r--   0 jenkins    (115) docker     (999)      510 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1981 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/archive_extract.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1040 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/converters.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2806 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/directory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5143 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/hgutil.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    16613 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/identify.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    29492 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/loader.py
+-rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/py.typed
+-rw-r--r--   0 jenkins    (115) docker     (999)     1473 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:48:47.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1671 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:48:47.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/
+-rw-r--r--   0 jenkins    (115) docker     (999)  2757941 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/anomad-d.tgz
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     7621 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/build.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      897 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/example.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     1392 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/example.sh
+-rw-r--r--   0 jenkins    (115) docker     (999)    51200 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/example.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)      411 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/hello.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     3070 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/hello.tgz
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      465 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/missing-filelog.sh
+-rw-r--r--   0 jenkins    (115) docker     (999)    40960 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/missing-filelog.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)      456 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/multiple-heads.json
+-rw-r--r--   0 jenkins    (115) docker     (999)      448 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/multiple-heads.sh
+-rw-r--r--   0 jenkins    (115) docker     (999)    40960 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/multiple-heads.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)     5209 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/the-sandbox.json
+-rw-r--r--   0 jenkins    (115) docker     (999)    13309 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/the-sandbox.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)      633 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/transplant.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     3206 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/transplant.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)     2353 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/loader_checker.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2155 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/test_converters.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6238 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/test_directory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3016 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/test_identify.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    26197 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/test_loader.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1746 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/test_tasks.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1440 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/test_tasks_directory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1462 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/utils.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:48:47.000000 swh.loader.mercurial-3.3.0/swh.loader.mercurial.egg-info/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1799 2023-06-06 12:48:47.000000 swh.loader.mercurial-3.3.0/swh.loader.mercurial.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     2158 2023-06-06 12:48:47.000000 swh.loader.mercurial-3.3.0/swh.loader.mercurial.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-06-06 12:48:47.000000 swh.loader.mercurial-3.3.0/swh.loader.mercurial.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      135 2023-06-06 12:48:47.000000 swh.loader.mercurial-3.3.0/swh.loader.mercurial.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      300 2023-06-06 12:48:47.000000 swh.loader.mercurial-3.3.0/swh.loader.mercurial.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-06-06 12:48:47.000000 swh.loader.mercurial-3.3.0/swh.loader.mercurial.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1549 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/tox.ini
```

### Comparing `swh.loader.mercurial-3.1.1/.pre-commit-config.yaml` & `swh.loader.mercurial-3.3.0/.pre-commit-config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.1.0
+    rev: v4.3.0
     hooks:
       - id: trailing-whitespace
       - id: check-json
       - id: check-yaml
 
-  - repo: https://gitlab.com/pycqa/flake8
-    rev: 4.0.1
+  - repo: https://github.com/pycqa/flake8
+    rev: 5.0.4
     hooks:
       - id: flake8
-        additional_dependencies: [flake8-bugbear==22.3.23]
+        additional_dependencies: [flake8-bugbear==22.9.23]
 
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.1.0
+    rev: v2.2.2
     hooks:
       - id: codespell
         name: Check source code spelling
         stages: [commit]
 
   - repo: local
     hooks:
@@ -26,15 +26,15 @@
         entry: mypy
         args: [swh]
         pass_filenames: false
         language: system
         types: [python]
 
   - repo: https://github.com/PyCQA/isort
-    rev: 5.10.1
+    rev: 5.11.5
     hooks:
       - id: isort
 
   - repo: https://github.com/python/black
-    rev: 22.3.0
+    rev: 22.10.0
     hooks:
       - id: black
```

### Comparing `swh.loader.mercurial-3.1.1/CODE_OF_CONDUCT.md` & `swh.loader.mercurial-3.3.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.1.1/LICENSE` & `swh.loader.mercurial-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.1.1/PKG-INFO` & `swh.loader.mercurial-3.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: swh.loader.mercurial
-Version: 3.1.1
+Version: 3.3.0
 Summary: Software Heritage Mercurial Loader
 Home-page: https://forge.softwareheritage.org/diffusion/DLDHG/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
-License: UNKNOWN
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-loader-mercurial
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-loader-mercurial/
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -32,14 +30,17 @@
 The main entry points are:
 - :class:`swh.loader.mercurial.loader.HgLoader` which reads and loads a local
   repository into an SWH archive.
 
 - :class:`swh.loader.mercurial.loader.HgArchiveLoader` which reads and loads
   a local repository wrapped within a tarball
 
+- :class:`swh.loader.mercurial.directory.HgDirectoryLoader` which ingests the hg tree at
+  a specific changeset or tag.
+
 # CLI run
 
 ## Configuration file
 
 /tmp/mercurial.yml:
 ``` YAML
 storage:
@@ -49,9 +50,7 @@
 ```
 
 ## Basic use
 
 ``` bash
 swh loader --C /tmp/mercurial.yml run mercurial https://www.mercurial-scm.org/repo/hello
 ```
-
-
```

### Comparing `swh.loader.mercurial-3.1.1/README.md` & `swh.loader.mercurial-3.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 The main entry points are:
 - :class:`swh.loader.mercurial.loader.HgLoader` which reads and loads a local
   repository into an SWH archive.
 
 - :class:`swh.loader.mercurial.loader.HgArchiveLoader` which reads and loads
   a local repository wrapped within a tarball
 
+- :class:`swh.loader.mercurial.directory.HgDirectoryLoader` which ingests the hg tree at
+  a specific changeset or tag.
+
 # CLI run
 
 ## Configuration file
 
 /tmp/mercurial.yml:
 ``` YAML
 storage:
```

### Comparing `swh.loader.mercurial-3.1.1/conftest.py` & `swh.loader.mercurial-3.3.0/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.1.1/setup.py` & `swh.loader.mercurial-3.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.1.1/swh/loader/mercurial/archive_extract.py` & `swh.loader.mercurial-3.3.0/swh/loader/mercurial/archive_extract.py`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.1.1/swh/loader/mercurial/converters.py` & `swh.loader.mercurial-3.3.0/swh/loader/mercurial/converters.py`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.1.1/swh/loader/mercurial/hgutil.py` & `swh.loader.mercurial-3.3.0/swh/loader/mercurial/hgutil.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Copyright (C) 2020-2021  The Software Heritage developers
+# Copyright (C) 2020-2023  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 from collections import defaultdict
 from dataclasses import dataclass
 from functools import partial
 from typing import Dict, List, Mapping, NewType, Optional, Set
 
 # The internal Mercurial API is not guaranteed to be stable.
-from mercurial import bookmarks, context, error, hg, smartset, util  # type: ignore
-import mercurial.ui  # type: ignore
+from mercurial import bookmarks, context, error, hg, smartset, util
+import mercurial.ui
 
 from swh.loader.core.utils import clone_with_timeout
 
 NULLID = mercurial.node.nullid
 HgNodeId = NewType("HgNodeId", bytes)
 Repository = hg.localrepo
 BaseContext = context.basectx
@@ -108,17 +108,25 @@
         bookmarks=branch_bookmarks,
         open_heads=branch_open_heads,
         closed_heads=branch_closed_heads,
         default_branch_alias=default_rev_alias,
     )
 
 
-def clone(src: str, dest: str, timeout: float):
+def clone(src: str, dest: str, timeout: float = 7200, rev: Optional[str] = None):
+    """Clone a hg repository `src` in `dest`. Optionally, this can clone at the specific
+    revision if provided.
+
+    Raises:
+        CloneFailure: when there is an issue during the cloning step
+
+    """
     closure = partial(
         hg.clone,
         ui=mercurial.ui.ui.load(),
         peeropts={},
         source=src.encode(),
         dest=dest.encode(),
         update=False,
+        revs=None if not rev else [rev.encode()],
     )
     clone_with_timeout(src, dest, closure, timeout)
```

### Comparing `swh.loader.mercurial-3.1.1/swh/loader/mercurial/identify.py` & `swh.loader.mercurial-3.3.0/swh/loader/mercurial/identify.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (C) 2020-2021  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
-from codecs import escape_decode  # type: ignore
+from codecs import escape_decode
 import json
 from pathlib import Path
 import re
 import subprocess
 from typing import Any, Dict, Iterator, List, NamedTuple, Optional, Union
 
 # WARNING: do not import unnecessary things here to keep cli startup time under
@@ -193,15 +193,15 @@
 class Hg:
     """Provide methods to extract data from a Mercurial repository."""
 
     def __init__(self, repository_root: Path) -> None:
         self._root = repository_root
 
     def _output(self, *args) -> bytes:
-        """Return the outpout of a `hg` call."""
+        """Return the output of a `hg` call."""
         return subprocess.check_output(
             ["hg", *args], cwd=self._root, env=get_minimum_env()
         )
 
     def _call(self, *args) -> None:
         """Perform a `hg` call."""
         subprocess.check_call(
```

### Comparing `swh.loader.mercurial-3.1.1/swh/loader/mercurial/loader.py` & `swh.loader.mercurial-3.3.0/swh/loader/mercurial/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2020-2022  The Software Heritage developers
+# Copyright (C) 2020-2023  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 """Loaders for ingesting Mercurial repositories either local from disk, or remote, see
 :class:`swh.loader.mercurial.loader.HgLoader` or from an archive, see
 :class:`swh.loader.mercurial.from_disk.HgArchiveLoader`.
@@ -26,15 +26,15 @@
     TypeVar,
     Union,
 )
 
 from swh.core.utils import grouper
 from swh.loader.core.loader import BaseLoader
 from swh.loader.core.utils import clean_dangling_folders
-from swh.loader.mercurial.utils import get_minimum_env
+from swh.loader.mercurial.utils import get_minimum_env, raise_not_found_repository
 from swh.model import swhids
 from swh.model.from_disk import Content, DentryPerms, Directory
 from swh.model.hashutil import hash_to_bytehex
 from swh.model.model import (
     ExtID,
     ObjectType,
     Person,
@@ -338,15 +338,16 @@
                 suffix=f"-{os.getpid()}",
                 dir=self._temp_directory,
             )
             self.log.debug(
                 f"Cloning {self.origin.url} to {self._repo_directory} "
                 f"with timeout {self._clone_timeout} seconds"
             )
-            hgutil.clone(self.origin.url, self._repo_directory, self._clone_timeout)
+            with raise_not_found_repository():
+                hgutil.clone(self.origin.url, self._repo_directory, self._clone_timeout)
         else:  # existing local repository
             # Allow to load on disk repository without cloning
             # for testing purpose.
             self._repo_directory = self.directory
 
         self._repo = hgutil.repository(self._repo_directory)
 
@@ -358,15 +359,15 @@
         assert self._repo is not None
         existing_heads = []
 
         for hg_nodeid in heads:
             try:
                 rev = self._repo[hg_nodeid].rev()
                 existing_heads.append(rev)
-            except KeyError:  # the node does not exist anymore
+            except hgutil.error.RepoLookupError:  # the node does not exist anymore
                 pass
 
         # select revisions that are not ancestors of heads
         # and not the heads themselves
         new_revs = self._repo.revs("not ::(%ld)", existing_heads)
 
         if new_revs:
@@ -787,15 +788,15 @@
     """Mercurial loader for repository wrapped within tarballs."""
 
     def __init__(
         self,
         storage: StorageInterface,
         url: str,
         visit_date: Optional[datetime] = None,
-        archive_path: str = None,
+        archive_path: Optional[str] = None,
         temp_directory: str = "/tmp",
         **kwargs: Any,
     ):
         super().__init__(
             storage=storage,
             url=url,
             visit_date=visit_date,
```

### Comparing `swh.loader.mercurial-3.1.1/swh/loader/mercurial/tasks.py` & `swh.loader.mercurial-3.3.0/swh/loader/mercurial/tasks.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-# Copyright (C) 2020-2022  The Software Heritage developers
+# Copyright (C) 2020-2023  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 from celery import shared_task
 
 from swh.loader.core.utils import parse_visit_date
+from swh.loader.mercurial.directory import HgDirectoryLoader
 
 from .loader import HgArchiveLoader, HgLoader
 
 
 def _process_kwargs(kwargs):
     if "visit_date" in kwargs:
         kwargs["visit_date"] = parse_visit_date(kwargs["visit_date"])
@@ -33,7 +34,17 @@
 def load_hg_from_archive(**kwargs):
     """Import a mercurial tarball into swh.
 
     Args: see :func:`HgArchiveLoader` constructor.
     """
     loader = HgArchiveLoader.from_configfile(**_process_kwargs(kwargs))
     return loader.load()
+
+
+@shared_task(name=__name__ + ".LoadMercurialDirectory")
+def load_hg_directory(**kwargs):
+    """Import a mercurial tree into swh.
+
+    Args: see :func:`HgDirectoryLoader` constructor.
+    """
+    loader = HgDirectoryLoader.from_configfile(**_process_kwargs(kwargs))
+    return loader.load()
```

### Comparing `swh.loader.mercurial-3.1.1/swh/loader/mercurial/tests/conftest.py` & `swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,27 @@
-# Copyright (C) 2019-2021  The Software Heritage developers
+# Copyright (C) 2019-2023  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import os
 from typing import Any, Dict
+import uuid
 
 import pytest
 
+from swh.scheduler.model import Lister
+
+NAMESPACE = "swh.loader.mercurial"
+
+
+@pytest.fixture
+def hg_lister():
+    return Lister(name="hg-lister", instance_name="example", id=uuid.uuid4())
+
 
 @pytest.fixture
 def swh_storage_backend_config(swh_storage_backend_config):
     """Basic pg storage configuration with no journal collaborator
     (to avoid pulling optional dependency on clients of this fixture)
 
     """
```

### Comparing `swh.loader.mercurial-3.1.1/swh/loader/mercurial/tests/data/anomad-d.tgz` & `swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/anomad-d.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.1.1/swh/loader/mercurial/tests/data/build.py` & `swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/build.py`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.1.1/swh/loader/mercurial/tests/data/example.json` & `swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/example.json`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.1.1/swh/loader/mercurial/tests/data/example.sh` & `swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/example.sh`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.1.1/swh/loader/mercurial/tests/data/example.tgz` & `swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/example.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.1.1/swh/loader/mercurial/tests/data/hello.tgz` & `swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/hello.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.1.1/swh/loader/mercurial/tests/data/missing-filelog.tgz` & `swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/missing-filelog.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.1.1/swh/loader/mercurial/tests/data/multiple-heads.tgz` & `swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/multiple-heads.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.1.1/swh/loader/mercurial/tests/data/the-sandbox.json` & `swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/the-sandbox.json`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.1.1/swh/loader/mercurial/tests/data/the-sandbox.tgz` & `swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/the-sandbox.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.1.1/swh/loader/mercurial/tests/data/transplant.json` & `swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/transplant.json`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.1.1/swh/loader/mercurial/tests/data/transplant.tgz` & `swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/transplant.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.1.1/swh/loader/mercurial/tests/loader_checker.py` & `swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/loader_checker.py`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.1.1/swh/loader/mercurial/tests/test_converters.py` & `swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.1.1/swh/loader/mercurial/tests/test_identify.py` & `swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/test_identify.py`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.1.1/swh/loader/mercurial/tests/test_loader.py` & `swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/test_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -723,7 +723,42 @@
     archive_name = "anomad-d"
     archive_path = os.path.join(datadir, f"{archive_name}.tgz")
     repo_url = prepare_repository_from_archive(archive_path, archive_name, tmp_path)
 
     loader = HgLoader(swh_storage, url=repo_url)
 
     assert loader.load() == {"status": "eventful"}
+
+
+def test_loader_missing_hg_node_on_reload(swh_storage, datadir, tmp_path):
+    """hg node previously seen in a first load but whose does not exist in second load
+    must be filtered out"""
+    archive_name = "the-sandbox"
+    archive_path = os.path.join(datadir, f"{archive_name}.tgz")
+    repo_url = prepare_repository_from_archive(archive_path, archive_name, tmp_path)
+
+    # first load
+    loader = HgLoader(swh_storage, url=repo_url)
+    assert loader.load() == {"status": "eventful"}
+
+    # second load to populate the _latest_heads list
+    loader = HgLoader(swh_storage, url=repo_url)
+    assert loader.load() == {"status": "uneventful"}
+    assert loader._latest_heads
+
+    # add an unknown hg node to the latest heads list
+    loader._latest_heads.append(hash_to_bytes("1" * 40))
+    # check it is filtered out by the get_hg_revs_to_load method
+    assert list(loader.get_hg_revs_to_load()) == []
+
+
+def test_loader_not_found_hg_repository(swh_storage, datadir, tmp_path):
+    """Ingesting an inexistent repository should be a not-found uneventful visit"""
+    repo_url = "file:///origin/not/found"
+    loader = HgLoader(swh_storage, url=repo_url)
+    assert loader.load() == {"status": "uneventful"}
+    assert_last_visit_matches(
+        swh_storage,
+        repo_url,
+        status="not_found",
+        type="hg",
+    )
```

### Comparing `swh.loader.mercurial-3.1.1/swh.loader.mercurial.egg-info/PKG-INFO` & `swh.loader.mercurial-3.3.0/swh.loader.mercurial.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: swh.loader.mercurial
-Version: 3.1.1
+Version: 3.3.0
 Summary: Software Heritage Mercurial Loader
 Home-page: https://forge.softwareheritage.org/diffusion/DLDHG/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
-License: UNKNOWN
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-loader-mercurial
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-loader-mercurial/
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -32,14 +30,17 @@
 The main entry points are:
 - :class:`swh.loader.mercurial.loader.HgLoader` which reads and loads a local
   repository into an SWH archive.
 
 - :class:`swh.loader.mercurial.loader.HgArchiveLoader` which reads and loads
   a local repository wrapped within a tarball
 
+- :class:`swh.loader.mercurial.directory.HgDirectoryLoader` which ingests the hg tree at
+  a specific changeset or tag.
+
 # CLI run
 
 ## Configuration file
 
 /tmp/mercurial.yml:
 ``` YAML
 storage:
@@ -49,9 +50,7 @@
 ```
 
 ## Basic use
 
 ``` bash
 swh loader --C /tmp/mercurial.yml run mercurial https://www.mercurial-scm.org/repo/hello
 ```
-
-
```

### Comparing `swh.loader.mercurial-3.1.1/swh.loader.mercurial.egg-info/SOURCES.txt` & `swh.loader.mercurial-3.3.0/swh.loader.mercurial.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -31,27 +31,30 @@
 swh.loader.mercurial.egg-info/entry_points.txt
 swh.loader.mercurial.egg-info/requires.txt
 swh.loader.mercurial.egg-info/top_level.txt
 swh/loader/__init__.py
 swh/loader/mercurial/__init__.py
 swh/loader/mercurial/archive_extract.py
 swh/loader/mercurial/converters.py
+swh/loader/mercurial/directory.py
 swh/loader/mercurial/hgutil.py
 swh/loader/mercurial/identify.py
 swh/loader/mercurial/loader.py
 swh/loader/mercurial/py.typed
 swh/loader/mercurial/tasks.py
 swh/loader/mercurial/utils.py
 swh/loader/mercurial/tests/__init__.py
 swh/loader/mercurial/tests/conftest.py
 swh/loader/mercurial/tests/loader_checker.py
 swh/loader/mercurial/tests/test_converters.py
+swh/loader/mercurial/tests/test_directory.py
 swh/loader/mercurial/tests/test_identify.py
 swh/loader/mercurial/tests/test_loader.py
 swh/loader/mercurial/tests/test_tasks.py
+swh/loader/mercurial/tests/test_tasks_directory.py
 swh/loader/mercurial/tests/data/anomad-d.tgz
 swh/loader/mercurial/tests/data/build.py
 swh/loader/mercurial/tests/data/example.json
 swh/loader/mercurial/tests/data/example.sh
 swh/loader/mercurial/tests/data/example.tgz
 swh/loader/mercurial/tests/data/hello.json
 swh/loader/mercurial/tests/data/hello.tgz
```

### Comparing `swh.loader.mercurial-3.1.1/tox.ini` & `swh.loader.mercurial-3.3.0/tox.ini`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 [tox]
+requires =
+  tox>4
 envlist=black,flake8,mypy,py3
 
 [testenv]
 extras =
   testing
 deps =
   pytest-cov
@@ -12,64 +14,62 @@
   pytest --cov={envsitepackagesdir}/swh/loader/mercurial \
          {envsitepackagesdir}/swh/loader/mercurial \
          --cov-branch {posargs}
 
 [testenv:black]
 skip_install = true
 deps =
-  black==22.3.0
+  black==22.10.0
 commands =
   {envpython} -m black --check swh
 
 [testenv:flake8]
 skip_install = true
 deps =
-  flake8==4.0.1
-  flake8-bugbear==22.3.23
+  flake8==5.0.4
+  flake8-bugbear==22.9.23
+  pycodestyle==2.9.1
 commands =
   {envpython} -m flake8
 
 [testenv:mypy]
 extras =
   testing
 deps =
-  mypy==0.942
+  mypy==1.0.1
 commands =
   mypy swh
 
 # build documentation outside swh-environment using the current
 # git HEAD of swh-docs, is executed on CI for each diff to prevent
 # breaking doc build
 [testenv:sphinx]
-whitelist_externals = make
+allowlist_externals = make
 usedevelop = true
 extras =
   testing
 deps =
   # fetch and install swh-docs in develop mode
-  -e git+https://forge.softwareheritage.org/source/swh-docs#egg=swh.docs
-
+  -e git+https://gitlab.softwareheritage.org/swh/devel/swh-docs.git\#egg=swh.docs
 setenv =
   SWH_PACKAGE_DOC_TOX_BUILD = 1
   # turn warnings into errors
   SPHINXOPTS = -W
 commands =
   make -I ../.tox/sphinx/src/swh-docs/swh/ -C docs
 
-
 # build documentation only inside swh-environment using local state
 # of swh-docs package
 [testenv:sphinx-dev]
-whitelist_externals = make
+allowlist_externals = make
 usedevelop = true
 extras =
   testing
 deps =
   # install swh-docs in develop mode
   -e ../swh-docs
-
 setenv =
   SWH_PACKAGE_DOC_TOX_BUILD = 1
   # turn warnings into errors
   SPHINXOPTS = -W
 commands =
   make -I ../.tox/sphinx-dev/src/swh-docs/swh/ -C docs
```

