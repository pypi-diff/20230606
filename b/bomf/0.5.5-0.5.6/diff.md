# Comparing `tmp/bomf-0.5.5.tar.gz` & `tmp/bomf-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bomf-0.5.5.tar", last modified: Tue Jun  6 20:00:02 2023, max compression
+gzip compressed data, was "bomf-0.5.6.tar", last modified: Tue Jun  6 21:44:57 2023, max compression
```

## Comparing `bomf-0.5.5.tar` & `bomf-0.5.6.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:00:02.687433 bomf-0.5.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:00:02.679433 bomf-0.5.5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-06 19:59:55.000000 bomf-0.5.5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:00:02.683433 bomf-0.5.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-06 19:59:55.000000 bomf-0.5.5/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-06-06 19:59:55.000000 bomf-0.5.5/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-06 19:59:55.000000 bomf-0.5.5/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-06 19:59:55.000000 bomf-0.5.5/.github/workflows/no_byte_order_mark.yml
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-06 19:59:55.000000 bomf-0.5.5/.github/workflows/packaging_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-06 19:59:55.000000 bomf-0.5.5/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-06 19:59:55.000000 bomf-0.5.5/.github/workflows/pythonlint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-06 19:59:55.000000 bomf-0.5.5/.github/workflows/unittests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-06 19:59:55.000000 bomf-0.5.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-06 19:59:55.000000 bomf-0.5.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-06 19:59:55.000000 bomf-0.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-06 20:00:02.687433 bomf-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-06-06 19:59:55.000000 bomf-0.5.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-06 19:59:55.000000 bomf-0.5.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-06 19:59:55.000000 bomf-0.5.5/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-06 19:59:55.000000 bomf-0.5.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-06 20:00:02.687433 bomf-0.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-06 19:59:55.000000 bomf-0.5.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:00:02.679433 bomf-0.5.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:00:02.683433 bomf-0.5.5/src/bomf/
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-06-06 19:59:55.000000 bomf-0.5.5/src/bomf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:00:02.683433 bomf-0.5.5/src/bomf/filter/
--rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-06-06 19:59:55.000000 bomf-0.5.5/src/bomf/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-06-06 19:59:55.000000 bomf-0.5.5/src/bomf/filter/sourcedataproviderfilter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:00:02.683433 bomf-0.5.5/src/bomf/loader/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-06 19:59:55.000000 bomf-0.5.5/src/bomf/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-06-06 19:59:55.000000 bomf-0.5.5/src/bomf/loader/entityloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:00:02.683433 bomf-0.5.5/src/bomf/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-06-06 19:59:55.000000 bomf-0.5.5/src/bomf/mapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:00:02.683433 bomf-0.5.5/src/bomf/model/
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-06 19:59:55.000000 bomf-0.5.5/src/bomf/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:00:02.683433 bomf-0.5.5/src/bomf/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-06-06 19:59:55.000000 bomf-0.5.5/src/bomf/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-06 19:59:55.000000 bomf-0.5.5/src/bomf/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:00:02.683433 bomf-0.5.5/src/bomf/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-06 19:59:55.000000 bomf-0.5.5/src/bomf/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:00:02.687433 bomf-0.5.5/src/bomf/validation/core/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-06 19:59:55.000000 bomf-0.5.5/src/bomf/validation/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-06-06 19:59:55.000000 bomf-0.5.5/src/bomf/validation/core/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-06-06 19:59:55.000000 bomf-0.5.5/src/bomf/validation/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    17577 2023-06-06 19:59:55.000000 bomf-0.5.5/src/bomf/validation/core/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-06 19:59:55.000000 bomf-0.5.5/src/bomf/validation/core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-06 19:59:55.000000 bomf-0.5.5/src/bomf/validation/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-06-06 19:59:55.000000 bomf-0.5.5/src/bomf/validation/core/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-06-06 19:59:55.000000 bomf-0.5.5/src/bomf/validation/path_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-06-06 19:59:55.000000 bomf-0.5.5/src/bomf/validation/query_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-06 19:59:55.000000 bomf-0.5.5/src/bomf/validation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:00:02.683433 bomf-0.5.5/src/bomf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-06 20:00:02.000000 bomf-0.5.5/src/bomf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-06 20:00:02.000000 bomf-0.5.5/src/bomf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 20:00:02.000000 bomf-0.5.5/src/bomf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 20:00:02.000000 bomf-0.5.5/src/bomf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-06 20:00:02.000000 bomf-0.5.5/src/bomf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-06 20:00:02.000000 bomf-0.5.5/src/bomf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-06 19:59:55.000000 bomf-0.5.5/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:00:02.687433 bomf-0.5.5/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-06 19:59:55.000000 bomf-0.5.5/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-06 19:59:55.000000 bomf-0.5.5/unittests/example_source_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-06 19:59:55.000000 bomf-0.5.5/unittests/test_bo4e_data_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-06-06 19:59:55.000000 bomf-0.5.5/unittests/test_entity_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-06-06 19:59:55.000000 bomf-0.5.5/unittests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-06-06 19:59:55.000000 bomf-0.5.5/unittests/test_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-06-06 19:59:55.000000 bomf-0.5.5/unittests/test_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-06-06 19:59:55.000000 bomf-0.5.5/unittests/test_source_data_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    21291 2023-06-06 19:59:55.000000 bomf-0.5.5/unittests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:44:57.079460 bomf-0.5.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:44:57.075460 bomf-0.5.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-06 21:44:49.000000 bomf-0.5.6/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:44:57.075460 bomf-0.5.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-06 21:44:49.000000 bomf-0.5.6/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-06-06 21:44:49.000000 bomf-0.5.6/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-06 21:44:49.000000 bomf-0.5.6/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-06 21:44:49.000000 bomf-0.5.6/.github/workflows/no_byte_order_mark.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-06 21:44:49.000000 bomf-0.5.6/.github/workflows/packaging_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-06 21:44:49.000000 bomf-0.5.6/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-06 21:44:49.000000 bomf-0.5.6/.github/workflows/pythonlint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-06 21:44:49.000000 bomf-0.5.6/.github/workflows/unittests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-06 21:44:49.000000 bomf-0.5.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-06 21:44:49.000000 bomf-0.5.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-06 21:44:49.000000 bomf-0.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-06 21:44:57.079460 bomf-0.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-06-06 21:44:49.000000 bomf-0.5.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-06 21:44:49.000000 bomf-0.5.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-06 21:44:49.000000 bomf-0.5.6/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-06 21:44:49.000000 bomf-0.5.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-06 21:44:57.079460 bomf-0.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-06 21:44:49.000000 bomf-0.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:44:57.071459 bomf-0.5.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:44:57.075460 bomf-0.5.6/src/bomf/
+-rw-r--r--   0 runner    (1001) docker     (123)     7846 2023-06-06 21:44:49.000000 bomf-0.5.6/src/bomf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:44:57.075460 bomf-0.5.6/src/bomf/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-06-06 21:44:49.000000 bomf-0.5.6/src/bomf/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-06-06 21:44:49.000000 bomf-0.5.6/src/bomf/filter/sourcedataproviderfilter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:44:57.075460 bomf-0.5.6/src/bomf/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-06 21:44:49.000000 bomf-0.5.6/src/bomf/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-06-06 21:44:49.000000 bomf-0.5.6/src/bomf/loader/entityloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:44:57.075460 bomf-0.5.6/src/bomf/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-06-06 21:44:49.000000 bomf-0.5.6/src/bomf/mapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:44:57.075460 bomf-0.5.6/src/bomf/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-06 21:44:49.000000 bomf-0.5.6/src/bomf/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:44:57.075460 bomf-0.5.6/src/bomf/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-06-06 21:44:49.000000 bomf-0.5.6/src/bomf/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-06 21:44:49.000000 bomf-0.5.6/src/bomf/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:44:57.075460 bomf-0.5.6/src/bomf/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-06 21:44:49.000000 bomf-0.5.6/src/bomf/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:44:57.079460 bomf-0.5.6/src/bomf/validation/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-06 21:44:49.000000 bomf-0.5.6/src/bomf/validation/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-06-06 21:44:49.000000 bomf-0.5.6/src/bomf/validation/core/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-06-06 21:44:49.000000 bomf-0.5.6/src/bomf/validation/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17577 2023-06-06 21:44:49.000000 bomf-0.5.6/src/bomf/validation/core/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-06 21:44:49.000000 bomf-0.5.6/src/bomf/validation/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-06 21:44:49.000000 bomf-0.5.6/src/bomf/validation/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-06-06 21:44:49.000000 bomf-0.5.6/src/bomf/validation/core/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-06-06 21:44:49.000000 bomf-0.5.6/src/bomf/validation/path_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-06-06 21:44:49.000000 bomf-0.5.6/src/bomf/validation/query_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-06 21:44:49.000000 bomf-0.5.6/src/bomf/validation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:44:57.075460 bomf-0.5.6/src/bomf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-06 21:44:56.000000 bomf-0.5.6/src/bomf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-06 21:44:56.000000 bomf-0.5.6/src/bomf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 21:44:56.000000 bomf-0.5.6/src/bomf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 21:44:56.000000 bomf-0.5.6/src/bomf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-06 21:44:56.000000 bomf-0.5.6/src/bomf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-06 21:44:56.000000 bomf-0.5.6/src/bomf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-06 21:44:49.000000 bomf-0.5.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 21:44:57.079460 bomf-0.5.6/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-06 21:44:49.000000 bomf-0.5.6/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-06 21:44:49.000000 bomf-0.5.6/unittests/example_source_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-06 21:44:49.000000 bomf-0.5.6/unittests/test_bo4e_data_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-06-06 21:44:49.000000 bomf-0.5.6/unittests/test_entity_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-06-06 21:44:49.000000 bomf-0.5.6/unittests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-06-06 21:44:49.000000 bomf-0.5.6/unittests/test_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-06-06 21:44:49.000000 bomf-0.5.6/unittests/test_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-06-06 21:44:49.000000 bomf-0.5.6/unittests/test_source_data_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21291 2023-06-06 21:44:49.000000 bomf-0.5.6/unittests/test_validation.py
```

### Comparing `bomf-0.5.5/.github/dependabot.yml` & `bomf-0.5.6/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.5/.github/workflows/black.yml` & `bomf-0.5.6/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.5/.github/workflows/codeql-analysis.yml` & `bomf-0.5.6/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.5/.github/workflows/coverage.yml` & `bomf-0.5.6/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.5/.github/workflows/packaging_test.yml` & `bomf-0.5.6/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.5/.github/workflows/python-publish.yml` & `bomf-0.5.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.5/.github/workflows/pythonlint.yml` & `bomf-0.5.6/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.5/.github/workflows/unittests.yml` & `bomf-0.5.6/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.5/.gitignore` & `bomf-0.5.6/.gitignore`

 * *Files identical despite different names*

### Comparing `bomf-0.5.5/.pre-commit-config.yaml` & `bomf-0.5.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.5/LICENSE` & `bomf-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bomf-0.5.5/PKG-INFO` & `bomf-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bomf
-Version: 0.5.5
+Version: 0.5.6
 Summary: BO4E Migration Framework
 Home-page: https://github.com/Hochfrequenz/bo4e_migration_framework
 Author: Hochfrequenz Unternehmensberatung GmbH
 Author-email: info@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://github.com/Hochfrequenz/bo4e_migration_framework
 Project-URL: Code, https://github.com/Hochfrequenz/bo4e_migration_framework
```

### Comparing `bomf-0.5.5/README.md` & `bomf-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `bomf-0.5.5/pyproject.toml` & `bomf-0.5.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.5/requirements.txt` & `bomf-0.5.6/requirements.txt`

 * *Files identical despite different names*

### Comparing `bomf-0.5.5/setup.cfg` & `bomf-0.5.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `bomf-0.5.5/src/bomf/__init__.py` & `bomf-0.5.6/src/bomf/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -104,21 +104,33 @@
         """
         # todo: here we should add some logging and statistics stuff
         self.logger.info("Starting migration %s (w/o pagination)", self.__class__.__name__)
         bo4e_datasets = await self.source_data_to_bo4e_mapper.create_data_sets()
         loading_summaries = await self._map_to_target_validate_and_load(bo4e_datasets)
         return loading_summaries
 
-    async def migrate_paginated(self, chunk_size: int) -> list[LoadingSummary]:
+    async def migrate_paginated(
+        self, chunk_size: int, initial_offset: int = 0, upper_bound: Optional[int] = None
+    ) -> list[LoadingSummary]:
         """
         This is similar to migrate, but it loads the data in chunks of chunk_size.
         Therefore, the source_data_to_bo4e_mapper must support pagination.
+        You can specify an offset on where to start (initial_offset).
+        The upper_bound does not cap the number of entries you want to migrate but instead is a number up to which the
+        offset will definitely be incremented. This allows you to paginate over empty pages (because there's no matching
+        entry within the range covered by one page). If you don't specify an upper_bound, the migration will stop on the
+        first empty page.
         """
-        self.logger.info("Starting migration %s (with page size %i)", self.__class__.__name__, chunk_size)
-        offset = 0
+        self.logger.info(
+            "Starting migration %s (with page size %i and initial offset %i)",
+            self.__class__.__name__,
+            chunk_size,
+            initial_offset,
+        )
+        offset = initial_offset
         loading_summaries = []
         while True:
             self.logger.info("Processing offset=%i, limit=%i", offset, chunk_size)
             try:
                 bo4e_datasets = await self.source_data_to_bo4e_mapper.create_data_sets(
                     limit=chunk_size, offset=offset
                 )  # this might raise an PaginationNotSupportedException
@@ -128,16 +140,19 @@
                     "got an unexpected keyword argument 'limit'" in error_message
                     or "got an unexpected keyword argument 'offset'" in error_message
                 ):
                     # this case should be prevented by the type checker already
                     raise PaginationNotSupportedException() from type_error
                 raise
             self.logger.debug("Received %i datasets (limit was %i)", len(bo4e_datasets), chunk_size)
-            if len(bo4e_datasets) == 0:
-                self.logger.info("Received no more datasets; Stopping")
+            if (upper_bound is None or offset > upper_bound) and len(bo4e_datasets) == 0:
+                if upper_bound is not None:
+                    self.logger.info("Reached first empty page after upper bound %i; Stopping", upper_bound)
+                else:
+                    self.logger.info("Received no more datasets (first empty page; no upper bound defined); Stopping")
                 break
             chunk_loading_summaries = await self._map_to_target_validate_and_load(bo4e_datasets)
             loading_summaries.extend(chunk_loading_summaries)
             await asyncio.sleep(1)  # give the system 1s some time to breathe
             offset += chunk_size
         success_count, failure_count = _get_success_failure_count(loading_summaries)
         self.logger.info(
```

### Comparing `bomf-0.5.5/src/bomf/filter/__init__.py` & `bomf-0.5.6/src/bomf/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.5/src/bomf/filter/sourcedataproviderfilter.py` & `bomf-0.5.6/src/bomf/filter/sourcedataproviderfilter.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.5/src/bomf/loader/entityloader.py` & `bomf-0.5.6/src/bomf/loader/entityloader.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.5/src/bomf/mapper/__init__.py` & `bomf-0.5.6/src/bomf/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.5/src/bomf/model/__init__.py` & `bomf-0.5.6/src/bomf/model/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.5/src/bomf/provider/__init__.py` & `bomf-0.5.6/src/bomf/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.5/src/bomf/validation/core/analysis.py` & `bomf-0.5.6/src/bomf/validation/core/analysis.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.5/src/bomf/validation/core/errors.py` & `bomf-0.5.6/src/bomf/validation/core/errors.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.5/src/bomf/validation/core/execution.py` & `bomf-0.5.6/src/bomf/validation/core/execution.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.5/src/bomf/validation/core/types.py` & `bomf-0.5.6/src/bomf/validation/core/types.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.5/src/bomf/validation/core/utils.py` & `bomf-0.5.6/src/bomf/validation/core/utils.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.5/src/bomf/validation/core/validator.py` & `bomf-0.5.6/src/bomf/validation/core/validator.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.5/src/bomf/validation/path_map.py` & `bomf-0.5.6/src/bomf/validation/path_map.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.5/src/bomf/validation/query_map.py` & `bomf-0.5.6/src/bomf/validation/query_map.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.5/src/bomf/validation/utils.py` & `bomf-0.5.6/src/bomf/validation/utils.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.5/src/bomf.egg-info/PKG-INFO` & `bomf-0.5.6/src/bomf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bomf
-Version: 0.5.5
+Version: 0.5.6
 Summary: BO4E Migration Framework
 Home-page: https://github.com/Hochfrequenz/bo4e_migration_framework
 Author: Hochfrequenz Unternehmensberatung GmbH
 Author-email: info@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://github.com/Hochfrequenz/bo4e_migration_framework
 Project-URL: Code, https://github.com/Hochfrequenz/bo4e_migration_framework
```

### Comparing `bomf-0.5.5/src/bomf.egg-info/SOURCES.txt` & `bomf-0.5.6/src/bomf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bomf-0.5.5/tox.ini` & `bomf-0.5.6/tox.ini`

 * *Files identical despite different names*

### Comparing `bomf-0.5.5/unittests/test_bo4e_data_set.py` & `bomf-0.5.6/unittests/test_bo4e_data_set.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.5/unittests/test_entity_loader.py` & `bomf-0.5.6/unittests/test_entity_loader.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.5/unittests/test_filter.py` & `bomf-0.5.6/unittests/test_filter.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.5/unittests/test_mapper.py` & `bomf-0.5.6/unittests/test_mapper.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.5/unittests/test_migration.py` & `bomf-0.5.6/unittests/test_migration.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.5/unittests/test_source_data_provider.py` & `bomf-0.5.6/unittests/test_source_data_provider.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.5/unittests/test_validation.py` & `bomf-0.5.6/unittests/test_validation.py`

 * *Files identical despite different names*

