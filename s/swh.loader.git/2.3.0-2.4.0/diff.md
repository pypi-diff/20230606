# Comparing `tmp/swh.loader.git-2.3.0.tar.gz` & `tmp/swh.loader.git-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swh.loader.git-2.3.0.tar", last modified: Tue May  2 12:39:38 2023, max compression
+gzip compressed data, was "dist/swh.loader.git-2.4.0.tar", last modified: Tue Jun  6 12:46:27 2023, max compression
```

## Comparing `swh.loader.git-2.3.0.tar` & `swh.loader.git-2.4.0.tar`

### file list

```diff
@@ -1,76 +1,79 @@
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/
--rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) docker     (999)      290 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      848 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/AUTHORS
--rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) docker     (999)       15 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/LICENSE
--rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/MANIFEST.in
--rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     2834 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     1907 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/README.md
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/bin/
--rwxr-xr-x   0 jenkins    (115) docker     (999)      605 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/bin/dir-git-repo-meta.sh
--rw-r--r--   0 jenkins    (115) docker     (999)      567 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/docs/
--rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/docs/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/docs/Makefile
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/docs/_static/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/docs/_templates/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/docs/_templates/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/docs/attic/
--rw-r--r--   0 jenkins    (115) docker     (999)     6851 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/docs/attic/api-backend-protocol.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     5476 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/docs/attic/git-loading-design.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/docs/conf.py
--rw-r--r--   0 jenkins    (115) docker     (999)      360 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/docs/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      399 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/mypy.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/pyproject.toml
--rw-r--r--   0 jenkins    (115) docker     (999)      241 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/pytest.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      109 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      115 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/requirements-test.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       34 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/requirements.txt
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/resources/
--rw-r--r--   0 jenkins    (115) docker     (999)      307 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/resources/local-loader-git.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      307 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/resources/remote-loader-git.ini
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/resources/test/
--rw-r--r--   0 jenkins    (115) docker     (999)      502 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/resources/test/back.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      125 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/resources/test/db-manager.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      307 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/resources/updater.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/setup.cfg
--rwxr-xr-x   0 jenkins    (115) docker     (999)     2387 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/setup.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/swh/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/swh/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/swh/loader/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/swh/loader/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/swh/loader/git/
--rw-r--r--   0 jenkins    (115) docker     (999)      653 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/swh/loader/git/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4603 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/swh/loader/git/base.py
--rw-r--r--   0 jenkins    (115) docker     (999)     9812 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/swh/loader/git/converters.py
--rw-r--r--   0 jenkins    (115) docker     (999)     8043 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/swh/loader/git/dumb.py
--rw-r--r--   0 jenkins    (115) docker     (999)    15166 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/swh/loader/git/from_disk.py
--rw-r--r--   0 jenkins    (115) docker     (999)    28204 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/swh/loader/git/loader.py
--rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/swh/loader/git/py.typed
--rw-r--r--   0 jenkins    (115) docker     (999)     1581 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/swh/loader/git/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/swh/loader/git/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)      251 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/swh/loader/git/tests/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1134 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/swh/loader/git/tests/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/swh/loader/git/tests/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/swh/loader/git/tests/data/git-repos/
--rw-r--r--   0 jenkins    (115) docker     (999)     5433 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/swh/loader/git/tests/data/git-repos/example-submodule.bundle
--rw-r--r--   0 jenkins    (115) docker     (999)    10630 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/swh/loader/git/tests/data/testrepo.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)    33966 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/swh/loader/git/tests/test_converters.py
--rw-r--r--   0 jenkins    (115) docker     (999)    20607 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/swh/loader/git/tests/test_from_disk.py
--rw-r--r--   0 jenkins    (115) docker     (999)    39895 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/swh/loader/git/tests/test_loader.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2522 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/swh/loader/git/tests/test_tasks.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1491 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/swh/loader/git/tests/test_utils.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4070 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/swh/loader/git/utils.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/swh.loader.git.egg-info/
--rw-r--r--   0 jenkins    (115) docker     (999)     2834 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/swh.loader.git.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     1464 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/swh.loader.git.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/swh.loader.git.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      103 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/swh.loader.git.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      255 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/swh.loader.git.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-05-02 12:39:38.000000 swh.loader.git-2.3.0/swh.loader.git.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1727 2023-05-02 12:39:36.000000 swh.loader.git-2.3.0/tox.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/
+-rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) docker     (999)      290 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      848 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/AUTHORS
+-rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) docker     (999)       15 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/LICENSE
+-rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/MANIFEST.in
+-rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     2954 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     2027 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/README.md
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/bin/
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      605 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/bin/dir-git-repo-meta.sh
+-rw-r--r--   0 jenkins    (115) docker     (999)      567 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/docs/
+-rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/docs/Makefile
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/docs/_static/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/docs/_templates/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/docs/_templates/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/docs/attic/
+-rw-r--r--   0 jenkins    (115) docker     (999)     6851 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/docs/attic/api-backend-protocol.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     5476 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/docs/attic/git-loading-design.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/docs/conf.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      360 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/docs/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      399 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/mypy.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/pyproject.toml
+-rw-r--r--   0 jenkins    (115) docker     (999)      241 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/pytest.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      109 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      115 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       35 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/requirements.txt
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/resources/
+-rw-r--r--   0 jenkins    (115) docker     (999)      307 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/resources/local-loader-git.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      307 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/resources/remote-loader-git.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/resources/test/
+-rw-r--r--   0 jenkins    (115) docker     (999)      502 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/resources/test/back.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      125 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/resources/test/db-manager.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      307 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/resources/updater.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/setup.cfg
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     2387 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/setup.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/swh/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/swh/loader/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/swh/loader/git/
+-rw-r--r--   0 jenkins    (115) docker     (999)      653 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/git/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4603 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/git/base.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     9923 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/git/converters.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2731 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/git/directory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     8043 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/git/dumb.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    15273 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/git/from_disk.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    27520 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/git/loader.py
+-rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/git/py.typed
+-rw-r--r--   0 jenkins    (115) docker     (999)     1904 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/git/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/swh/loader/git/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)      251 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/git/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1331 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/git/tests/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/swh/loader/git/tests/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/swh/loader/git/tests/data/git-repos/
+-rw-r--r--   0 jenkins    (115) docker     (999)     5433 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/git/tests/data/git-repos/example-submodule.bundle
+-rw-r--r--   0 jenkins    (115) docker     (999)    10630 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/git/tests/data/testrepo.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)    33966 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/git/tests/test_converters.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5875 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/git/tests/test_directory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    20607 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/git/tests/test_from_disk.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    39895 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/git/tests/test_loader.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2390 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/git/tests/test_tasks.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1261 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/git/tests/test_tasks_directory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2799 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/git/tests/test_utils.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5449 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/git/utils.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/swh.loader.git.egg-info/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2954 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/swh.loader.git.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     1576 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/swh.loader.git.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/swh.loader.git.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      103 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/swh.loader.git.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      256 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/swh.loader.git.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/swh.loader.git.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1727 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/tox.ini
```

### Comparing `swh.loader.git-2.3.0/.pre-commit-config.yaml` & `swh.loader.git-2.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.3.0/CODE_OF_CONDUCT.md` & `swh.loader.git-2.4.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.3.0/LICENSE` & `swh.loader.git-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.3.0/PKG-INFO` & `swh.loader.git-2.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.loader.git
-Version: 2.3.0
+Version: 2.4.0
 Summary: Software Heritage git loader
 Home-page: https://forge.softwareheritage.org/diffusion/DLDG/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-loader-git
@@ -35,14 +35,17 @@
 
 - :class:`swh.loader.git.from_disk.GitLoaderFromDisk` which ingests only local git clone
   repository.
 
 - :class:`swh.loader.git.loader.GitLoaderFromArchive` which ingests a git repository
   wrapped in an archive.
 
+- :class:`swh.loader.git.directory.GitDirectoryLoader` which ingests a git tree at a
+  specific commit, branch or tag.
+
 
 License
 -------
 
 This program is free software: you can redistribute it and/or modify it
 under the terms of the GNU General Public License as published by the
 Free Software Foundation, either version 3 of the License, or (at your
```

### Comparing `swh.loader.git-2.3.0/README.md` & `swh.loader.git-2.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 
 - :class:`swh.loader.git.from_disk.GitLoaderFromDisk` which ingests only local git clone
   repository.
 
 - :class:`swh.loader.git.loader.GitLoaderFromArchive` which ingests a git repository
   wrapped in an archive.
 
+- :class:`swh.loader.git.directory.GitDirectoryLoader` which ingests a git tree at a
+  specific commit, branch or tag.
+
 
 License
 -------
 
 This program is free software: you can redistribute it and/or modify it
 under the terms of the GNU General Public License as published by the
 Free Software Foundation, either version 3 of the License, or (at your
```

### Comparing `swh.loader.git-2.3.0/bin/dir-git-repo-meta.sh` & `swh.loader.git-2.4.0/bin/dir-git-repo-meta.sh`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.3.0/conftest.py` & `swh.loader.git-2.4.0/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.3.0/docs/attic/api-backend-protocol.txt` & `swh.loader.git-2.4.0/docs/attic/api-backend-protocol.txt`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.3.0/docs/attic/git-loading-design.txt` & `swh.loader.git-2.4.0/docs/attic/git-loading-design.txt`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.3.0/setup.py` & `swh.loader.git-2.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.3.0/swh/loader/git/__init__.py` & `swh.loader.git-2.4.0/swh/loader/git/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.3.0/swh/loader/git/base.py` & `swh.loader.git-2.4.0/swh/loader/git/base.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.3.0/swh/loader/git/converters.py` & `swh.loader.git-2.4.0/swh/loader/git/converters.py`

 * *Files 8% similar despite different names*

```diff
@@ -184,18 +184,20 @@
     commit = cast(Commit, obj)
 
     author_timezone = None
     committer_timezone = None
     assert commit._chunked_text is not None  # to keep mypy happy
     for (field, value) in _parse_message(commit._chunked_text):
         if field == b"author":
+            assert value is not None
             m = AUTHORSHIP_LINE_RE.match(value)
             if m:
                 author_timezone = m.group("timezone")
         elif field == b"committer":
+            assert value is not None
             m = AUTHORSHIP_LINE_RE.match(value)
             if m:
                 committer_timezone = m.group("timezone")
 
     extra_headers = []
     if commit.encoding is not None:
         extra_headers.append((b"encoding", commit.encoding))
@@ -274,14 +276,15 @@
         raise ValueError("Argument is not a tag.")
     tag = cast(Tag, obj)
 
     tagger_timezone = None
     # FIXME: _parse_message is a private function from Dulwich.
     for (field, value) in _parse_message(tag.as_raw_chunks()):
         if field == b"tagger":
+            assert value is not None
             m = AUTHORSHIP_LINE_RE.match(value)
             if m:
                 tagger_timezone = m.group("timezone")
 
     target_type, target = tag.object
     if tag.tagger:
         author: Optional[Person] = parse_author(tag.tagger)
```

### Comparing `swh.loader.git-2.3.0/swh/loader/git/dumb.py` & `swh.loader.git-2.4.0/swh/loader/git/dumb.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.3.0/swh/loader/git/from_disk.py` & `swh.loader.git-2.4.0/swh/loader/git/from_disk.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2015-2021  The Software Heritage developers
+# Copyright (C) 2015-2023  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 from collections import defaultdict
 from datetime import datetime
 import logging
 import os
@@ -17,14 +17,15 @@
     # dulwich >= 0.20
     from dulwich.objects import EmptyFileException
 
 from deprecated import deprecated
 import dulwich.objects
 import dulwich.repo
 
+from swh.loader.git.utils import raise_not_found_repository
 from swh.model import hashutil
 from swh.model.model import Snapshot, SnapshotBranch, TargetType
 from swh.storage.algos.origin import origin_get_latest_visit_status
 from swh.storage.interface import StorageInterface
 
 from . import converters, utils
 from .base import BaseGitLoader
@@ -101,15 +102,16 @@
         **kwargs,
     ):
         super().__init__(storage=storage, origin_url=url, **kwargs)
         self.visit_date = visit_date or self.visit_date
         self.directory = directory
 
     def prepare(self):
-        self.repo = dulwich.repo.Repo(self.directory)
+        with raise_not_found_repository():
+            self.repo = dulwich.repo.Repo(self.directory)
 
     def iter_objects(self):
         object_store = self.repo.object_store
 
         for pack in object_store.packs:
             objs = list(pack.index.iterentries())
             objs.sort(key=lambda x: x[1])
```

### Comparing `swh.loader.git-2.3.0/swh/loader/git/loader.py` & `swh.loader.git-2.4.0/swh/loader/git/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,21 +22,20 @@
     Optional,
     Set,
     Tuple,
     Type,
 )
 
 import dulwich.client
-from dulwich.errors import GitProtocolError, NotGitRepository
 from dulwich.object_store import ObjectStoreGraphWalker
 from dulwich.objects import Blob, Commit, ShaFile, Tag, Tree
 from dulwich.pack import PackData, PackInflater
 
 from swh.core.statsd import Statsd
-from swh.loader.exception import NotFound
+from swh.loader.git.utils import raise_not_found_repository
 from swh.model import hashutil
 from swh.model.git_objects import (
     content_git_object,
     directory_git_object,
     release_git_object,
     revision_git_object,
 )
@@ -341,33 +340,18 @@
         )
 
         def do_progress(msg: bytes) -> None:
             sys.stderr.buffer.write(msg)
             sys.stderr.flush()
 
         try:
-            fetch_info = self.fetch_pack_from_origin(
-                self.origin.url, base_repo, do_progress
-            )
-        except (dulwich.client.HTTPUnauthorized, NotGitRepository) as e:
-            raise NotFound(e)
-        except GitProtocolError as e:
-            # unfortunately, that kind of error is not specific to a not found
-            # scenario... It depends on the value of message within the exception.
-            for msg in [
-                " unavailable",  # e.g DMCA takedown
-                " not found",
-                "unexpected http resp 401",
-                "unexpected http resp 403",
-                "unexpected http resp 410",
-            ]:
-                if msg in str(e.args[0]):
-                    raise NotFound(e)
-            # otherwise transmit the error
-            raise
+            with raise_not_found_repository():
+                fetch_info = self.fetch_pack_from_origin(
+                    self.origin.url, base_repo, do_progress
+                )
         except (AttributeError, NotImplementedError, ValueError):
             # with old dulwich versions, those exceptions types can be raised
             # by the fetch_pack operation when encountering a repository with
             # dumb transfer protocol so we check if the repository supports it
             # here to continue the loading if it is the case
             self.dumb = dumb.check_protocol(self.origin.url)
             if not self.dumb:
```

### Comparing `swh.loader.git-2.3.0/swh/loader/git/tasks.py` & `swh.loader.git-2.4.0/swh/loader/git/tasks.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-# Copyright (C) 2015-2022  The Software Heritage developers
+# Copyright (C) 2015-2023  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 from typing import Any, Dict
 
 from celery import shared_task
 
 from swh.loader.core.utils import parse_visit_date
+from swh.loader.git.directory import GitDirectoryLoader
 from swh.loader.git.from_disk import GitLoaderFromArchive, GitLoaderFromDisk
 from swh.loader.git.loader import GitLoader
 
 
 def _process_kwargs(kwargs):
     if "visit_date" in kwargs:
         kwargs["visit_date"] = parse_visit_date(kwargs["visit_date"])
@@ -39,7 +40,14 @@
     1. Uncompress an archive repository in a local and temporary folder
     2. Load it through the git disk loader
     3. Clean up the temporary folder
 
     """
     loader = GitLoaderFromArchive.from_configfile(**_process_kwargs(kwargs))
     return loader.load()
+
+
+@shared_task(name=__name__ + ".LoadGitDirectory")
+def load_git_directory(**kwargs) -> Dict[str, Any]:
+    """Load a git tree at a specific commit, tag or branch."""
+    loader = GitDirectoryLoader.from_configfile(**_process_kwargs(kwargs))
+    return loader.load()
```

### Comparing `swh.loader.git-2.3.0/swh/loader/git/tests/data/git-repos/example-submodule.bundle` & `swh.loader.git-2.4.0/swh/loader/git/tests/data/git-repos/example-submodule.bundle`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.3.0/swh/loader/git/tests/data/testrepo.tgz` & `swh.loader.git-2.4.0/swh/loader/git/tests/data/testrepo.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.3.0/swh/loader/git/tests/test_converters.py` & `swh.loader.git-2.4.0/swh/loader/git/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.3.0/swh/loader/git/tests/test_from_disk.py` & `swh.loader.git-2.4.0/swh/loader/git/tests/test_from_disk.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.3.0/swh/loader/git/tests/test_loader.py` & `swh.loader.git-2.4.0/swh/loader/git/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.3.0/swh/loader/git/tests/test_tasks.py` & `swh.loader.git-2.4.0/swh/loader/git/tests/test_tasks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,18 @@
-# Copyright (C) 2018-2022  The Software Heritage developers
+# Copyright (C) 2018-2023  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
-import uuid
 
 import pytest
 
-from swh.scheduler.model import ListedOrigin, Lister
+from swh.scheduler.model import ListedOrigin
 
-NAMESPACE = "swh.loader.git"
-
-
-@pytest.fixture
-def git_lister():
-    return Lister(name="git-lister", instance_name="example", id=uuid.uuid4())
+from .conftest import NAMESPACE
 
 
 @pytest.fixture
 def git_listed_origin(git_lister):
     return ListedOrigin(
         lister_id=git_lister.id, url="https://git.example.org/repo", visit_type="git"
     )
```

### Comparing `swh.loader.git-2.3.0/swh/loader/git/utils.py` & `swh.loader.git-2.4.0/swh/loader/git/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,27 @@
-# Copyright (C) 2017-2021  The Software Heritage developers
+# Copyright (C) 2017-2023  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 """Utilities helper functions"""
 
+from contextlib import contextmanager
 import datetime
 import logging
 import os
 import shutil
 import tempfile
 from typing import Dict, Mapping, NewType, Optional, Union
 
+from dulwich.client import HTTPUnauthorized
+from dulwich.errors import GitProtocolError, NotGitRepository
+
 from swh.core import tarball
+from swh.loader.exception import NotFound
 from swh.model.model import SnapshotBranch
 
 # The hexadecimal representation of the hash in bytes
 HexBytes = NewType("HexBytes", bytes)
 
 
 def init_git_repo_from_archive(project_name, archive_path, root_temp_dir="/tmp"):
@@ -120,7 +125,39 @@
             ", ".join(descr),
             extra={
                 "swh_type": "swh_loader_git_dangling_symrefs",
                 "swh_refs": descr,
                 "origin_url": origin_url,
             },
         )
+
+
+@contextmanager
+def raise_not_found_repository():
+    """Catches all kinds of exceptions which translate to an inexistent repository and
+    reraise as a NotFound exception. Any other exceptions are propagated to the caller.
+
+    Raises:
+        NotFound: instead of HTTPUnauthorized, NotGitRepository and any GitProtocol with
+            specific error message relative to an inexistent repository.
+        *: Any other exceptions raised within the try block
+
+    """
+    try:
+        yield
+    except (HTTPUnauthorized, NotGitRepository) as e:
+        raise NotFound(e)
+    except GitProtocolError as e:
+        # that kind of error is unfortunately not specific to a not found scenario... It
+        # depends on the value of message within the exception. So parse the exception
+        # message to detect if it's a not found or not.
+        for msg in [
+            " unavailable",  # e.g DMCA takedown
+            " not found",
+            "unexpected http resp 401",
+            "unexpected http resp 403",
+            "unexpected http resp 410",
+        ]:
+            if msg in str(e.args[0]):
+                raise NotFound(e)
+        # otherwise transmit the error
+        raise
```

### Comparing `swh.loader.git-2.3.0/swh.loader.git.egg-info/PKG-INFO` & `swh.loader.git-2.4.0/swh.loader.git.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.loader.git
-Version: 2.3.0
+Version: 2.4.0
 Summary: Software Heritage git loader
 Home-page: https://forge.softwareheritage.org/diffusion/DLDG/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-loader-git
@@ -35,14 +35,17 @@
 
 - :class:`swh.loader.git.from_disk.GitLoaderFromDisk` which ingests only local git clone
   repository.
 
 - :class:`swh.loader.git.loader.GitLoaderFromArchive` which ingests a git repository
   wrapped in an archive.
 
+- :class:`swh.loader.git.directory.GitDirectoryLoader` which ingests a git tree at a
+  specific commit, branch or tag.
+
 
 License
 -------
 
 This program is free software: you can redistribute it and/or modify it
 under the terms of the GNU General Public License as published by the
 Free Software Foundation, either version 3 of the License, or (at your
```

### Comparing `swh.loader.git-2.3.0/swh.loader.git.egg-info/SOURCES.txt` & `swh.loader.git-2.4.0/swh.loader.git.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -39,22 +39,25 @@
 swh.loader.git.egg-info/entry_points.txt
 swh.loader.git.egg-info/requires.txt
 swh.loader.git.egg-info/top_level.txt
 swh/loader/__init__.py
 swh/loader/git/__init__.py
 swh/loader/git/base.py
 swh/loader/git/converters.py
+swh/loader/git/directory.py
 swh/loader/git/dumb.py
 swh/loader/git/from_disk.py
 swh/loader/git/loader.py
 swh/loader/git/py.typed
 swh/loader/git/tasks.py
 swh/loader/git/utils.py
 swh/loader/git/tests/__init__.py
 swh/loader/git/tests/conftest.py
 swh/loader/git/tests/test_converters.py
+swh/loader/git/tests/test_directory.py
 swh/loader/git/tests/test_from_disk.py
 swh/loader/git/tests/test_loader.py
 swh/loader/git/tests/test_tasks.py
+swh/loader/git/tests/test_tasks_directory.py
 swh/loader/git/tests/test_utils.py
 swh/loader/git/tests/data/testrepo.tgz
 swh/loader/git/tests/data/git-repos/example-submodule.bundle
```

### Comparing `swh.loader.git-2.3.0/tox.ini` & `swh.loader.git-2.4.0/tox.ini`

 * *Files identical despite different names*

