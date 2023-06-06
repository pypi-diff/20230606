# Comparing `tmp/bomf-0.5.4.tar.gz` & `tmp/bomf-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bomf-0.5.4.tar", last modified: Tue Jun  6 06:41:22 2023, max compression
+gzip compressed data, was "bomf-0.5.5.tar", last modified: Tue Jun  6 20:00:02 2023, max compression
```

## Comparing `bomf-0.5.4.tar` & `bomf-0.5.5.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:41:22.561216 bomf-0.5.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:41:22.557216 bomf-0.5.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-06 06:41:15.000000 bomf-0.5.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:41:22.561216 bomf-0.5.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-06 06:41:15.000000 bomf-0.5.4/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-06-06 06:41:15.000000 bomf-0.5.4/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-06 06:41:15.000000 bomf-0.5.4/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-06 06:41:15.000000 bomf-0.5.4/.github/workflows/no_byte_order_mark.yml
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-06 06:41:15.000000 bomf-0.5.4/.github/workflows/packaging_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-06 06:41:15.000000 bomf-0.5.4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-06 06:41:15.000000 bomf-0.5.4/.github/workflows/pythonlint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-06 06:41:15.000000 bomf-0.5.4/.github/workflows/unittests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-06 06:41:15.000000 bomf-0.5.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-06 06:41:15.000000 bomf-0.5.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-06 06:41:15.000000 bomf-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-06 06:41:22.561216 bomf-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-06-06 06:41:15.000000 bomf-0.5.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-06 06:41:15.000000 bomf-0.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-06 06:41:15.000000 bomf-0.5.4/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-06 06:41:15.000000 bomf-0.5.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-06 06:41:22.561216 bomf-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-06 06:41:15.000000 bomf-0.5.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:41:22.557216 bomf-0.5.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:41:22.561216 bomf-0.5.4/src/bomf/
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-06-06 06:41:15.000000 bomf-0.5.4/src/bomf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:41:22.561216 bomf-0.5.4/src/bomf/filter/
--rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-06-06 06:41:15.000000 bomf-0.5.4/src/bomf/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-06-06 06:41:15.000000 bomf-0.5.4/src/bomf/filter/sourcedataproviderfilter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:41:22.561216 bomf-0.5.4/src/bomf/loader/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-06 06:41:15.000000 bomf-0.5.4/src/bomf/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-06-06 06:41:15.000000 bomf-0.5.4/src/bomf/loader/entityloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:41:22.561216 bomf-0.5.4/src/bomf/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-06-06 06:41:15.000000 bomf-0.5.4/src/bomf/mapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:41:22.561216 bomf-0.5.4/src/bomf/model/
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-06 06:41:15.000000 bomf-0.5.4/src/bomf/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:41:22.561216 bomf-0.5.4/src/bomf/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-06-06 06:41:15.000000 bomf-0.5.4/src/bomf/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-06 06:41:15.000000 bomf-0.5.4/src/bomf/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:41:22.561216 bomf-0.5.4/src/bomf/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-06 06:41:15.000000 bomf-0.5.4/src/bomf/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:41:22.561216 bomf-0.5.4/src/bomf/validation/core/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-06 06:41:15.000000 bomf-0.5.4/src/bomf/validation/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-06-06 06:41:15.000000 bomf-0.5.4/src/bomf/validation/core/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-06-06 06:41:15.000000 bomf-0.5.4/src/bomf/validation/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    17577 2023-06-06 06:41:15.000000 bomf-0.5.4/src/bomf/validation/core/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-06 06:41:15.000000 bomf-0.5.4/src/bomf/validation/core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-06 06:41:15.000000 bomf-0.5.4/src/bomf/validation/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-06-06 06:41:15.000000 bomf-0.5.4/src/bomf/validation/core/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-06-06 06:41:15.000000 bomf-0.5.4/src/bomf/validation/path_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-06-06 06:41:15.000000 bomf-0.5.4/src/bomf/validation/query_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-06 06:41:15.000000 bomf-0.5.4/src/bomf/validation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:41:22.561216 bomf-0.5.4/src/bomf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-06 06:41:22.000000 bomf-0.5.4/src/bomf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-06 06:41:22.000000 bomf-0.5.4/src/bomf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 06:41:22.000000 bomf-0.5.4/src/bomf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 06:41:22.000000 bomf-0.5.4/src/bomf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-06 06:41:22.000000 bomf-0.5.4/src/bomf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-06 06:41:22.000000 bomf-0.5.4/src/bomf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-06 06:41:15.000000 bomf-0.5.4/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 06:41:22.561216 bomf-0.5.4/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-06 06:41:15.000000 bomf-0.5.4/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-06 06:41:15.000000 bomf-0.5.4/unittests/example_source_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-06 06:41:15.000000 bomf-0.5.4/unittests/test_bo4e_data_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-06-06 06:41:15.000000 bomf-0.5.4/unittests/test_entity_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-06-06 06:41:15.000000 bomf-0.5.4/unittests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-06-06 06:41:15.000000 bomf-0.5.4/unittests/test_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-06-06 06:41:15.000000 bomf-0.5.4/unittests/test_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-06-06 06:41:15.000000 bomf-0.5.4/unittests/test_source_data_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    21291 2023-06-06 06:41:15.000000 bomf-0.5.4/unittests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:00:02.687433 bomf-0.5.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:00:02.679433 bomf-0.5.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-06 19:59:55.000000 bomf-0.5.5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:00:02.683433 bomf-0.5.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-06 19:59:55.000000 bomf-0.5.5/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-06-06 19:59:55.000000 bomf-0.5.5/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-06 19:59:55.000000 bomf-0.5.5/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-06 19:59:55.000000 bomf-0.5.5/.github/workflows/no_byte_order_mark.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-06 19:59:55.000000 bomf-0.5.5/.github/workflows/packaging_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-06 19:59:55.000000 bomf-0.5.5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-06 19:59:55.000000 bomf-0.5.5/.github/workflows/pythonlint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-06 19:59:55.000000 bomf-0.5.5/.github/workflows/unittests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-06 19:59:55.000000 bomf-0.5.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-06 19:59:55.000000 bomf-0.5.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-06 19:59:55.000000 bomf-0.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-06 20:00:02.687433 bomf-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-06-06 19:59:55.000000 bomf-0.5.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-06 19:59:55.000000 bomf-0.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-06 19:59:55.000000 bomf-0.5.5/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-06 19:59:55.000000 bomf-0.5.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-06 20:00:02.687433 bomf-0.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-06 19:59:55.000000 bomf-0.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:00:02.679433 bomf-0.5.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:00:02.683433 bomf-0.5.5/src/bomf/
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-06-06 19:59:55.000000 bomf-0.5.5/src/bomf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:00:02.683433 bomf-0.5.5/src/bomf/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-06-06 19:59:55.000000 bomf-0.5.5/src/bomf/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-06-06 19:59:55.000000 bomf-0.5.5/src/bomf/filter/sourcedataproviderfilter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:00:02.683433 bomf-0.5.5/src/bomf/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-06 19:59:55.000000 bomf-0.5.5/src/bomf/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-06-06 19:59:55.000000 bomf-0.5.5/src/bomf/loader/entityloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:00:02.683433 bomf-0.5.5/src/bomf/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-06-06 19:59:55.000000 bomf-0.5.5/src/bomf/mapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:00:02.683433 bomf-0.5.5/src/bomf/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-06 19:59:55.000000 bomf-0.5.5/src/bomf/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:00:02.683433 bomf-0.5.5/src/bomf/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-06-06 19:59:55.000000 bomf-0.5.5/src/bomf/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-06 19:59:55.000000 bomf-0.5.5/src/bomf/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:00:02.683433 bomf-0.5.5/src/bomf/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-06 19:59:55.000000 bomf-0.5.5/src/bomf/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:00:02.687433 bomf-0.5.5/src/bomf/validation/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-06 19:59:55.000000 bomf-0.5.5/src/bomf/validation/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-06-06 19:59:55.000000 bomf-0.5.5/src/bomf/validation/core/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-06-06 19:59:55.000000 bomf-0.5.5/src/bomf/validation/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17577 2023-06-06 19:59:55.000000 bomf-0.5.5/src/bomf/validation/core/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-06 19:59:55.000000 bomf-0.5.5/src/bomf/validation/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-06 19:59:55.000000 bomf-0.5.5/src/bomf/validation/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-06-06 19:59:55.000000 bomf-0.5.5/src/bomf/validation/core/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-06-06 19:59:55.000000 bomf-0.5.5/src/bomf/validation/path_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-06-06 19:59:55.000000 bomf-0.5.5/src/bomf/validation/query_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-06 19:59:55.000000 bomf-0.5.5/src/bomf/validation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:00:02.683433 bomf-0.5.5/src/bomf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-06 20:00:02.000000 bomf-0.5.5/src/bomf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-06 20:00:02.000000 bomf-0.5.5/src/bomf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 20:00:02.000000 bomf-0.5.5/src/bomf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 20:00:02.000000 bomf-0.5.5/src/bomf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-06 20:00:02.000000 bomf-0.5.5/src/bomf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-06 20:00:02.000000 bomf-0.5.5/src/bomf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-06 19:59:55.000000 bomf-0.5.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:00:02.687433 bomf-0.5.5/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-06 19:59:55.000000 bomf-0.5.5/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-06 19:59:55.000000 bomf-0.5.5/unittests/example_source_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-06 19:59:55.000000 bomf-0.5.5/unittests/test_bo4e_data_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-06-06 19:59:55.000000 bomf-0.5.5/unittests/test_entity_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-06-06 19:59:55.000000 bomf-0.5.5/unittests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-06-06 19:59:55.000000 bomf-0.5.5/unittests/test_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-06-06 19:59:55.000000 bomf-0.5.5/unittests/test_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-06-06 19:59:55.000000 bomf-0.5.5/unittests/test_source_data_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21291 2023-06-06 19:59:55.000000 bomf-0.5.5/unittests/test_validation.py
```

### Comparing `bomf-0.5.4/.github/dependabot.yml` & `bomf-0.5.5/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.4/.github/workflows/black.yml` & `bomf-0.5.5/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.4/.github/workflows/codeql-analysis.yml` & `bomf-0.5.5/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.4/.github/workflows/coverage.yml` & `bomf-0.5.5/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.4/.github/workflows/packaging_test.yml` & `bomf-0.5.5/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.4/.github/workflows/python-publish.yml` & `bomf-0.5.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.4/.github/workflows/pythonlint.yml` & `bomf-0.5.5/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.4/.github/workflows/unittests.yml` & `bomf-0.5.5/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.4/.gitignore` & `bomf-0.5.5/.gitignore`

 * *Files identical despite different names*

### Comparing `bomf-0.5.4/.pre-commit-config.yaml` & `bomf-0.5.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.4/LICENSE` & `bomf-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bomf-0.5.4/PKG-INFO` & `bomf-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bomf
-Version: 0.5.4
+Version: 0.5.5
 Summary: BO4E Migration Framework
 Home-page: https://github.com/Hochfrequenz/bo4e_migration_framework
 Author: Hochfrequenz Unternehmensberatung GmbH
 Author-email: info@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://github.com/Hochfrequenz/bo4e_migration_framework
 Project-URL: Code, https://github.com/Hochfrequenz/bo4e_migration_framework
```

### Comparing `bomf-0.5.4/README.md` & `bomf-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `bomf-0.5.4/pyproject.toml` & `bomf-0.5.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.4/requirements.txt` & `bomf-0.5.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `bomf-0.5.4/setup.cfg` & `bomf-0.5.5/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 zip_safe = False
 include_package_data = True
 python_requires = >=3.10
 install_requires = 
 	attrs
 	bo4e
 	pydantic
-	typeguard
+	typeguard==2.13.3
 	frozendict
 	bidict
 	networkx
 	injector
 
 [options.packages.find]
 where = src
```

### Comparing `bomf-0.5.4/src/bomf/__init__.py` & `bomf-0.5.5/src/bomf/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.4/src/bomf/filter/__init__.py` & `bomf-0.5.5/src/bomf/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.4/src/bomf/filter/sourcedataproviderfilter.py` & `bomf-0.5.5/src/bomf/filter/sourcedataproviderfilter.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.4/src/bomf/loader/entityloader.py` & `bomf-0.5.5/src/bomf/loader/entityloader.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.4/src/bomf/mapper/__init__.py` & `bomf-0.5.5/src/bomf/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.4/src/bomf/model/__init__.py` & `bomf-0.5.5/src/bomf/model/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.4/src/bomf/provider/__init__.py` & `bomf-0.5.5/src/bomf/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.4/src/bomf/validation/core/analysis.py` & `bomf-0.5.5/src/bomf/validation/core/analysis.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.4/src/bomf/validation/core/errors.py` & `bomf-0.5.5/src/bomf/validation/core/errors.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.4/src/bomf/validation/core/execution.py` & `bomf-0.5.5/src/bomf/validation/core/execution.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.4/src/bomf/validation/core/types.py` & `bomf-0.5.5/src/bomf/validation/core/types.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.4/src/bomf/validation/core/utils.py` & `bomf-0.5.5/src/bomf/validation/core/utils.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.4/src/bomf/validation/core/validator.py` & `bomf-0.5.5/src/bomf/validation/core/validator.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.4/src/bomf/validation/path_map.py` & `bomf-0.5.5/src/bomf/validation/path_map.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.4/src/bomf/validation/query_map.py` & `bomf-0.5.5/src/bomf/validation/query_map.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.4/src/bomf/validation/utils.py` & `bomf-0.5.5/src/bomf/validation/utils.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.4/src/bomf.egg-info/PKG-INFO` & `bomf-0.5.5/src/bomf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bomf
-Version: 0.5.4
+Version: 0.5.5
 Summary: BO4E Migration Framework
 Home-page: https://github.com/Hochfrequenz/bo4e_migration_framework
 Author: Hochfrequenz Unternehmensberatung GmbH
 Author-email: info@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://github.com/Hochfrequenz/bo4e_migration_framework
 Project-URL: Code, https://github.com/Hochfrequenz/bo4e_migration_framework
```

### Comparing `bomf-0.5.4/src/bomf.egg-info/SOURCES.txt` & `bomf-0.5.5/src/bomf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bomf-0.5.4/tox.ini` & `bomf-0.5.5/tox.ini`

 * *Files identical despite different names*

### Comparing `bomf-0.5.4/unittests/test_bo4e_data_set.py` & `bomf-0.5.5/unittests/test_bo4e_data_set.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.4/unittests/test_entity_loader.py` & `bomf-0.5.5/unittests/test_entity_loader.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.4/unittests/test_filter.py` & `bomf-0.5.5/unittests/test_filter.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.4/unittests/test_mapper.py` & `bomf-0.5.5/unittests/test_mapper.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.4/unittests/test_migration.py` & `bomf-0.5.5/unittests/test_migration.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.4/unittests/test_source_data_provider.py` & `bomf-0.5.5/unittests/test_source_data_provider.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.4/unittests/test_validation.py` & `bomf-0.5.5/unittests/test_validation.py`

 * *Files identical despite different names*

