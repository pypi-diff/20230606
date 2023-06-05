# Comparing `tmp/dql-alpha-0.8.0.tar.gz` & `tmp/dql-alpha-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dql-alpha-0.8.0.tar", last modified: Wed Feb 15 09:17:23 2023, max compression
+gzip compressed data, was "dql-alpha-0.9.0.tar", last modified: Fri Feb 17 12:59:20 2023, max compression
```

## Comparing `dql-alpha-0.8.0.tar` & `dql-alpha-0.9.0.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:17:23.752973 dql-alpha-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:17:23.744973 dql-alpha-0.8.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:17:23.744973 dql-alpha-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/.github/workflows/benchmarks.yml
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-02-15 09:17:23.752973 dql-alpha-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-02-15 09:17:23.752973 dql-alpha-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:17:23.744973 dql-alpha-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:17:23.748973 dql-alpha-0.8.0/src/dql/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-15 09:17:23.000000 dql-alpha-0.8.0/src/dql/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    24168 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    22821 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/cli_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:17:23.748973 dql-alpha-0.8.0/src/dql/client/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/client/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/client/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/client/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/client/gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/client/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:17:23.748973 dql-alpha-0.8.0/src/dql/data_storage/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/data_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/data_storage/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/data_storage/query.py
--rw-r--r--   0 runner    (1001) docker     (123)    26659 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/data_storage/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:17:23.748973 dql-alpha-0.8.0/src/dql/jmes_sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/jmes_sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/jmes_sql/field_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/jmes_sql/functions_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/jmes_sql/transpiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    10176 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/listing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/nodes_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/nodes_thread_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:17:23.748973 dql-alpha-0.8.0/src/dql/remote/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/remote/studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:17:23.748973 dql-alpha-0.8.0/src/dql/vendored/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/vendored/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:17:23.748973 dql-alpha-0.8.0/src/dql/vendored/adlfs/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/vendored/adlfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18456 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/vendored/adlfs/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/vendored/adlfs/gen1.py
--rw-r--r--   0 runner    (1001) docker     (123)    74008 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/vendored/adlfs/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/vendored/adlfs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:17:23.748973 dql-alpha-0.8.0/src/dql/vendored/gcsfs/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/vendored/gcsfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18458 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/vendored/gcsfs/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/vendored/gcsfs/checkers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:17:23.748973 dql-alpha-0.8.0/src/dql/vendored/gcsfs/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/vendored/gcsfs/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/vendored/gcsfs/cli/gcsfuse.py
--rw-r--r--   0 runner    (1001) docker     (123)    60351 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/vendored/gcsfs/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/vendored/gcsfs/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/vendored/gcsfs/dask_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/vendored/gcsfs/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/src/dql/vendored/gcsfs/retry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:17:23.752973 dql-alpha-0.8.0/src/dql_alpha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-02-15 09:17:23.000000 dql-alpha-0.8.0/src/dql_alpha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-02-15 09:17:23.000000 dql-alpha-0.8.0/src/dql_alpha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 09:17:23.000000 dql-alpha-0.8.0/src/dql_alpha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-15 09:17:23.000000 dql-alpha-0.8.0/src/dql_alpha.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 09:17:23.000000 dql-alpha-0.8.0/src/dql_alpha.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-02-15 09:17:23.000000 dql-alpha-0.8.0/src/dql_alpha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-15 09:17:23.000000 dql-alpha-0.8.0/src/dql_alpha.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:17:23.752973 dql-alpha-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:17:23.752973 dql-alpha-0.8.0/tests/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/tests/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/tests/benchmarks/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/tests/benchmarks/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/tests/benchmarks/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:17:23.752973 dql-alpha-0.8.0/tests/func/
--rw-r--r--   0 runner    (1001) docker     (123)    32052 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/tests/func/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     9499 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/tests/func/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/tests/test_dql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 09:17:23.752973 dql-alpha-0.8.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/tests/unit/test_cli_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/tests/unit/test_client_s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/tests/unit/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/tests/unit/test_listing.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/tests/unit/test_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/tests/unit/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-02-15 09:16:59.000000 dql-alpha-0.8.0/tests/unit/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:59:20.838804 dql-alpha-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:59:20.830804 dql-alpha-0.9.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:59:20.830804 dql-alpha-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/.github/workflows/benchmarks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-02-17 12:59:20.838804 dql-alpha-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-02-17 12:59:20.838804 dql-alpha-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:59:20.826804 dql-alpha-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:59:20.830804 dql-alpha-0.9.0/src/dql/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-17 12:59:20.000000 dql-alpha-0.9.0/src/dql/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27641 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24755 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/cli_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:59:20.830804 dql-alpha-0.9.0/src/dql/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/client/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/client/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/client/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/client/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/client/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:59:20.830804 dql-alpha-0.9.0/src/dql/data_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/data_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/data_storage/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/data_storage/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31819 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/data_storage/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:59:20.830804 dql-alpha-0.9.0/src/dql/jmes_sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/jmes_sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/jmes_sql/field_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/jmes_sql/functions_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/jmes_sql/transpiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10176 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/listing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/nodes_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/nodes_thread_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:59:20.834804 dql-alpha-0.9.0/src/dql/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/remote/studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:59:20.834804 dql-alpha-0.9.0/src/dql/vendored/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/vendored/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:59:20.834804 dql-alpha-0.9.0/src/dql/vendored/adlfs/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/vendored/adlfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18456 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/vendored/adlfs/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/vendored/adlfs/gen1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74008 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/vendored/adlfs/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/vendored/adlfs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:59:20.834804 dql-alpha-0.9.0/src/dql/vendored/gcsfs/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/vendored/gcsfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18458 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/vendored/gcsfs/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/vendored/gcsfs/checkers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:59:20.834804 dql-alpha-0.9.0/src/dql/vendored/gcsfs/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/vendored/gcsfs/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/vendored/gcsfs/cli/gcsfuse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60351 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/vendored/gcsfs/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/vendored/gcsfs/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/vendored/gcsfs/dask_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/vendored/gcsfs/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/src/dql/vendored/gcsfs/retry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:59:20.834804 dql-alpha-0.9.0/src/dql_alpha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-02-17 12:59:20.000000 dql-alpha-0.9.0/src/dql_alpha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-02-17 12:59:20.000000 dql-alpha-0.9.0/src/dql_alpha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 12:59:20.000000 dql-alpha-0.9.0/src/dql_alpha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-17 12:59:20.000000 dql-alpha-0.9.0/src/dql_alpha.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 12:59:20.000000 dql-alpha-0.9.0/src/dql_alpha.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-02-17 12:59:20.000000 dql-alpha-0.9.0/src/dql_alpha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-17 12:59:20.000000 dql-alpha-0.9.0/src/dql_alpha.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:59:20.834804 dql-alpha-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:59:20.834804 dql-alpha-0.9.0/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/tests/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/tests/benchmarks/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/tests/benchmarks/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/tests/benchmarks/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:59:20.834804 dql-alpha-0.9.0/tests/func/
+-rw-r--r--   0 runner    (1001) docker     (123)    32093 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/tests/func/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9499 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/tests/func/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/tests/test_dql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 12:59:20.838804 dql-alpha-0.9.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/tests/unit/test_cli_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/tests/unit/test_client_s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/tests/unit/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/tests/unit/test_listing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/tests/unit/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/tests/unit/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-02-17 12:59:00.000000 dql-alpha-0.9.0/tests/unit/test_utils.py
```

### Comparing `dql-alpha-0.8.0/.cruft.json` & `dql-alpha-0.9.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/.github/dependabot.yml` & `dql-alpha-0.9.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/.github/workflows/benchmarks.yml` & `dql-alpha-0.9.0/.github/workflows/benchmarks.yml`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/.github/workflows/release.yml` & `dql-alpha-0.9.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/.github/workflows/tests.yml` & `dql-alpha-0.9.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/.gitignore` & `dql-alpha-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/.pre-commit-config.yaml` & `dql-alpha-0.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/CODE_OF_CONDUCT.rst` & `dql-alpha-0.9.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/CONTRIBUTING.rst` & `dql-alpha-0.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/LICENSE` & `dql-alpha-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/PKG-INFO` & `dql-alpha-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dql-alpha
-Version: 0.8.0
+Version: 0.9.0
 Summary: DQL
 Home-page: https://github.com/iterative/dql
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dql-alpha-0.8.0/README.rst` & `dql-alpha-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/noxfile.py` & `dql-alpha-0.9.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/pyproject.toml` & `dql-alpha-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/setup.cfg` & `dql-alpha-0.9.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 	=src
 packages = find:
 install_requires = 
 	pyyaml
 	tomlkit
 	tqdm
 	reflink
+	python-dateutil>=2
 	attrs>=21.3.0
 	funcy>=1.14
 	s3fs>=2023.1.0
 	decorator>4.1.2
 	fsspec==2023.1.0
 	google-auth>=1.2
 	google-auth-oauthlib
```

### Comparing `dql-alpha-0.8.0/src/dql/catalog.py` & `dql-alpha-0.9.0/src/dql/catalog.py`

 * *Files 15% similar despite different names*

```diff
@@ -511,41 +511,79 @@
         self,
         dataset_name: str,
         new_dataset_name: Optional[str] = None,
         version: Optional[int] = None,
         description: Optional[str] = None,
         labels: Optional[List[str]] = None,
     ):
+        version = version or 1
+
         dataset = self.data_storage.get_dataset(dataset_name)
         if not dataset:
-            raise RuntimeError(f"Dataset with name: {dataset_name} doesn't exist")
+            raise ValueError(f"Dataset {dataset_name} doesn't exist")
 
         if not dataset.shadow:
-            raise RuntimeError(f"Dataset is already registered: {dataset_name}")
+            raise ValueError(f"Dataset {dataset_name} is already registered")
 
         update_data = {
-            "version": version or 1,
             "shadow": False,
             "description": description,
             "labels": labels,
         }
 
         if new_dataset_name:
             update_data["name"] = new_dataset_name
 
         self.data_storage.update_dataset(dataset_name, **update_data)
+        self.data_storage.create_dataset_version(
+            new_dataset_name or dataset_name, version, create_rows_table=False
+        )
+        self.data_storage.rename_dataset_rows(new_dataset_name or dataset_name, version)
 
     def ls_datasets(self, shadow_only=None) -> Iterable[DatasetRecord]:
         yield from self.data_storage.get_datasets(shadow_only=shadow_only)
 
-    def ls_dataset_rows(self, name: str, limit=None) -> Iterable[DatasetRow]:
-        yield from self.data_storage.get_dataset_rows(name, limit=limit)
+    def ls_dataset_rows(
+        self, name: str, limit=None, version=None
+    ) -> Iterable[DatasetRow]:
+        dataset = self.data_storage.get_dataset(name)
+        assert dataset
+        if not dataset.shadow and not version:
+            raise ValueError(
+                f"Missing dataset version from input for registered dataset {name}"
+            )
+
+        yield from self.data_storage.get_dataset_rows(
+            name, limit=limit, version=version
+        )
 
-    def remove_dataset(self, name: str):
-        self.data_storage.remove_dataset(name)
+    def remove_dataset(
+        self,
+        name: str,
+        version: Optional[int] = None,
+        force: Optional[bool] = False,
+    ):
+        dataset = self.data_storage.get_dataset(name)
+        assert dataset
+        if dataset.registered and not version and not force:
+            raise ValueError(
+                f"Missing dataset version from input for registered dataset {name}"
+            )
+        if version and not dataset.has_version(version):
+            raise RuntimeError(f"Dataset {name} doesn't have version {version}")
+
+        if dataset.registered and version:
+            # removing one version of registered dataset
+            self.data_storage.remove_dataset_version(dataset, version)
+
+        elif dataset.registered and force:
+            for version in dataset.versions.copy():  # type: ignore [union-attr]
+                self.data_storage.remove_dataset_version(dataset, version)
+        else:
+            self.data_storage.remove_shadow_dataset(dataset)
 
     def edit_dataset(
         self,
         name: str,
         new_name: Optional[str] = None,
         description: Optional[str] = None,
         labels: Optional[List[str]] = None,
@@ -556,14 +594,72 @@
         if description:
             update_data["description"] = description
         if labels:
             update_data["labels"] = labels  # type: ignore[assignment]
 
         self.data_storage.update_dataset(name, **update_data)
 
+    def merge_datasets(
+        self,
+        src_name: str,
+        dst_name: str,
+        src_version: Optional[int] = None,
+        dst_version: Optional[int] = None,
+    ) -> DatasetRecord:
+        """
+        Merges records from source to destination dataset.
+        If destination dataset is shadow, it will copy all the records from source
+        dataset to shadow one
+        If destination dataset is registered, it will create a new version
+        of dataset with records merged from old version and the source
+        """
+
+        src = self.data_storage.get_dataset(src_name)
+        dst = self.data_storage.get_dataset(dst_name)
+
+        # validation
+        if not src:
+            raise ValueError(f"Source dataset {src_name} doesn't exist")
+        if src.shadow and src_version:
+            raise ValueError(
+                f"Source dataset {src_name} is shadow, cannot use it with versions"
+            )
+        if not src.shadow and not src_version:
+            raise ValueError(f"Source dataset {src_name} is registered, need a version")
+        if not dst:
+            raise ValueError(f"Dataset {dst_name} doesn't exist")
+        if dst.shadow and dst_version:
+            raise ValueError(
+                f"Dataset {dst_name} is shadow, cannot use it with versions"
+            )
+
+        if dst_version and not dst.is_valid_next_version(dst_version):
+            raise ValueError(
+                f"Version {dst_version} must be higher than the current latest one"
+            )
+
+        if dst.shadow:
+            self.data_storage.merge_dataset_rows(
+                src,
+                dst,
+                src_version,
+                dst_version=None,
+            )
+        else:
+            dst_version = dst_version or dst.next_version
+            dst = self.data_storage.create_dataset_version(dst_name, dst_version)
+            self.data_storage.merge_dataset_rows(
+                src,
+                dst,
+                src_version,
+                dst_version,
+            )
+
+        return dst
+
     def ls(
         self,
         sources: List[str],
         ttl=TTL_INT,
         update=False,
         skip_indexing=False,
         *,
```

### Comparing `dql-alpha-0.8.0/src/dql/cli.py` & `dql-alpha-0.9.0/src/dql/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -235,19 +235,69 @@
         help="List only shadow datasets, or only registered datasets",
     )
 
     ls_dataset_rows_parser = subp.add_parser(
         "ls-dataset-rows", parents=[parent_parser], help="List dataset rows"
     )
     ls_dataset_rows_parser.add_argument("name", type=str, help="Dataset name")
+    ls_dataset_rows_parser.add_argument(
+        "--version",
+        action="store",
+        default=None,
+        type=int,
+        help="Dataset version",
+    )
 
     rm_dataset_parser = subp.add_parser(
         "rm-dataset", parents=[parent_parser], help="Removes dataset"
     )
     rm_dataset_parser.add_argument("name", type=str, help="Dataset name")
+    rm_dataset_parser.add_argument(
+        "--version",
+        action="store",
+        default=None,
+        type=int,
+        help="Dataset version",
+    )
+    rm_dataset_parser.add_argument(
+        "--force",
+        default=False,
+        action=BooleanOptionalAction,
+        help="Force delete registered dataset with all of it's versions",
+    )
+
+    parse_merge_datasets = subp.add_parser(
+        "merge-datasets", parents=[parent_parser], help="Merges datasets"
+    )
+    parse_merge_datasets.add_argument(
+        "--src",
+        action="store",
+        default=None,
+        help="Source dataset name",
+    )
+    parse_merge_datasets.add_argument(
+        "--dst",
+        action="store",
+        default=None,
+        help="Destination dataset name",
+    )
+    parse_merge_datasets.add_argument(
+        "--src-version",
+        action="store",
+        default=None,
+        type=int,
+        help="Source dataset version",
+    )
+    parse_merge_datasets.add_argument(
+        "--dst-version",
+        action="store",
+        default=None,
+        type=int,
+        help="Destination dataset version",
+    )
 
     parse_ls = subp.add_parser(
         "ls", parents=[parent_parser], help="List storage contents"
     )
     add_sources_arg(parse_ls, nargs="*")
     parse_ls.add_argument(
         "-l",
@@ -411,14 +461,20 @@
 
 def edit_dataset(name, **kwargs):
     data_storage = SQLiteDataStorage()
     catalog = Catalog(data_storage)
     catalog.edit_dataset(name, **kwargs)
 
 
+def merge_datasets(src, dst, **kwargs):
+    data_storage = SQLiteDataStorage()
+    catalog = Catalog(data_storage)
+    catalog.merge_datasets(src, dst, **kwargs)
+
+
 def ls_urls(
     sources,
     long: bool = False,
     *,
     client_config=None,
     catalog: Optional[Catalog] = None,
     **kwargs,
@@ -578,25 +634,26 @@
 
 
 def ls_datasets(shadow_only=None):
     for d in Catalog(SQLiteDataStorage()).ls_datasets(shadow_only=shadow_only):
         if d.shadow:
             print(f"(tmp) {d.name}")
         else:
-            print(d.name)
+            for v in d.versions or []:
+                print(f"{d.name} (v{v})")
 
 
-def ls_dataset_rows(name: str):
-    for row in Catalog(SQLiteDataStorage()).ls_dataset_rows(name):
+def ls_dataset_rows(name: str, version: Optional[int] = None):
+    for row in Catalog(SQLiteDataStorage()).ls_dataset_rows(name, version=version):
         entry = row.name + ("/" if row.dir_type else "")  # type: ignore[attr-defined]
         print(format_ls_entry(entry))
 
 
-def rm_dataset(name: str):
-    Catalog(SQLiteDataStorage()).remove_dataset(name)
+def rm_dataset(name: str, version: Optional[int] = None, force: Optional[bool] = False):
+    Catalog(SQLiteDataStorage()).remove_dataset(name, version=version, force=force)
 
 
 def du(sources, show_bytes=False, si=False, **kwargs):
     data_storage = SQLiteDataStorage()
     catalog = Catalog(data_storage)
     for path, size in catalog.du(sources, **kwargs):
         if show_bytes:
@@ -690,29 +747,36 @@
         elif args.command == "edit-dataset":
             edit_dataset(
                 args.name,
                 description=args.description,
                 new_name=args.new_name,
                 labels=args.labels,
             )
+        elif args.command == "merge-datasets":
+            merge_datasets(
+                args.src,
+                args.dst,
+                src_version=args.src_version,
+                dst_version=args.dst_version,
+            )
         elif args.command == "ls":
             ls(
                 args.sources,
                 long=bool(args.long),
                 remote=args.remote,
                 ttl=args.ttl,
                 update=bool(args.update),
                 client_config=client_config,
             )
         elif args.command == "ls-datasets":
             ls_datasets(args.shadow)
         elif args.command == "ls-dataset-rows":
-            ls_dataset_rows(args.name)
+            ls_dataset_rows(args.name, args.version)
         elif args.command == "rm-dataset":
-            rm_dataset(args.name)
+            rm_dataset(args.name, version=args.version, force=args.force)
         elif args.command == "du":
             du(
                 args.sources,
                 show_bytes=args.bytes,
                 depth=args.depth,
                 si=args.si,
                 ttl=args.ttl,
```

### Comparing `dql-alpha-0.8.0/src/dql/cli_utils.py` & `dql-alpha-0.9.0/src/dql/cli_utils.py`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/src/dql/client/azure.py` & `dql-alpha-0.9.0/src/dql/client/azure.py`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/src/dql/client/base.py` & `dql-alpha-0.9.0/src/dql/client/base.py`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/src/dql/client/fsspec.py` & `dql-alpha-0.9.0/src/dql/client/fsspec.py`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/src/dql/client/gcs.py` & `dql-alpha-0.9.0/src/dql/client/gcs.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 from base64 import b64decode
+from datetime import datetime
+
+from dateutil.parser import isoparse
 
 from dql.vendored.gcsfs import GCSFileSystem
 
 from .fsspec import FSSpecClient
 
 # Patch gcsfs for consistency with s3fs
 # pylint:disable-next=protected-access
@@ -13,14 +16,25 @@
     FS_CLASS = GCSFileSystem
     PREFIX = "gcs://"
     protocol = "gcs"
 
     def __init__(self, name, **kwargs):
         super().__init__(name, self.create_fs(**kwargs))
 
+    @staticmethod
+    def parse_timestamp(timestamp: str) -> datetime:
+        """
+        Parse timestamp string returned by GCSFileSystem.
+
+        This ensures that the passed timestamp is timezone aware.
+        """
+        dt = isoparse(timestamp)
+        assert dt.tzinfo is not None
+        return dt
+
     @classmethod
     def _dict_from_info(cls, v, parent_id, delimiter, path):
         name = v.get("name", "").split(delimiter)[-1]
         if "generation" in v:
             gen = f"#{v['generation']}"
             if name.endswith(gen):
                 name = name[: -len(gen)]
@@ -30,14 +44,14 @@
             "path": path,
             "name": name,
             # 'expires': expires,
             "checksum": b64decode(v.get("md5Hash", "")).hex(),
             "etag": v.get("etag", ""),
             "version": v.get("generation", ""),
             "is_latest": not v.get("timeDeleted"),
-            "last_modified": v["updated"],
+            "last_modified": cls.parse_timestamp(v["updated"]),
             "size": v.get("size", ""),
             # 'storage_class': v.get('StorageClass'),
             "owner_name": "",
             "owner_id": "",
             "anno": None,
         }
```

### Comparing `dql-alpha-0.8.0/src/dql/client/s3.py` & `dql-alpha-0.9.0/src/dql/client/s3.py`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/src/dql/data_storage/abstract.py` & `dql-alpha-0.9.0/src/dql/data_storage/abstract.py`

 * *Files 15% similar despite different names*

```diff
@@ -41,30 +41,68 @@
     @abstractmethod
     def insert_into_shadow_dataset(
         self, name: str, uri: str, path: str, recursive: bool = False
     ) -> None:
         """Inserts data to shadow dataset based on bucket uri and glob path"""
 
     @abstractmethod
+    def rename_dataset_rows(self, name: str, version: int) -> None:
+        """
+        When registering dataset, we need to rename rows table from
+        ds_<id>_shadow to ds_<id>_<version>.
+        Example: from ds_24_shadow to ds_24_1
+        """
+
+    @abstractmethod
+    def create_dataset_version(
+        self, name: str, version: int, create_rows_table=True
+    ) -> "DatasetRecord":
+        """Creates new dataset version, optionally creating new rows table"""
+
+    @abstractmethod
+    def merge_dataset_rows(
+        self,
+        src: "DatasetRecord",
+        dst: "DatasetRecord",
+        src_version: Optional[int] = None,
+        dst_version: Optional[int] = None,
+    ) -> None:
+        """
+        Merges source dataset rows and current latest destination dataset rows
+        into a new rows table created for new destination dataset version.
+        Note that table for new destination version must be created upfront.
+        Merge results should not contain duplicates.
+        """
+
+    @abstractmethod
     def update_dataset(self, dataset_name: str, **kwargs) -> None:
         """Updates dataset fields"""
 
     @abstractmethod
     def get_dataset(self, name: str) -> Optional["DatasetRecord"]:
         """Finds dataset by name"""
 
     @abstractmethod
     def get_dataset_rows(
-        self, name: str, limit: Optional[int] = None
+        self, name: str, limit: Optional[int] = None, version: Optional[int] = None
     ) -> Iterable["DatasetRow"]:
         """Gets dataset rows"""
 
     @abstractmethod
-    def remove_dataset(self, name: str) -> None:
-        """Removes dataset by name and it's corresponding entries"""
+    def remove_dataset_version(self, dataset: "DatasetRecord", version: int) -> None:
+        """
+        Deletes one single dataset version. If it was last version,
+        it removes dataset completely
+        """
+
+    @abstractmethod
+    def remove_shadow_dataset(self, dataset: "DatasetRecord") -> None:
+        """
+        Removes shadow dataset and it's corresponding rows
+        """
 
     @abstractmethod
     async def insert_entry(self, entry: Dict[str, Any]) -> int:
         """
         Inserts file or directory node into the database
         and returns the id of the newly added node
         """
```

### Comparing `dql-alpha-0.8.0/src/dql/data_storage/query.py` & `dql-alpha-0.9.0/src/dql/data_storage/query.py`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/src/dql/data_storage/sqlite.py` & `dql-alpha-0.9.0/src/dql/data_storage/sqlite.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import hashlib
 import json
 import logging
+import operator
 import posixpath
 import sqlite3
-from datetime import datetime, timezone
+from datetime import MAXYEAR, MINYEAR, datetime, timezone
 from functools import partial, wraps
+from itertools import groupby
 from time import sleep
 from typing import Any, Dict, Iterable, Iterator, List, Optional, Tuple, Union
 
 from dql.data_storage.abstract import AbstractDataStorage
 from dql.dataset import DatasetRecord, DatasetRow
 from dql.error import DQLError
 from dql.node import AnyNode, DirType, Node, NodeWithPath
@@ -21,14 +23,36 @@
 logger = logging.getLogger("dql")
 
 RETRY_START_SEC = 0.01
 RETRY_MAX_TIMES = 10
 RETRY_FACTOR = 2
 
 
+def adapt_datetime(val: datetime) -> str:
+    if not (val.tzinfo is timezone.utc or val.tzname() == "UTC"):
+        try:
+            val = val.astimezone(timezone.utc)
+        except (OverflowError, ValueError, OSError):
+            if val.year == MAXYEAR:
+                val = datetime.max
+            elif val.year == MINYEAR:
+                val = datetime.min
+            else:
+                raise
+    return val.replace(tzinfo=None).isoformat(" ")
+
+
+def convert_datetime(val: bytes) -> datetime:
+    return datetime.fromisoformat(val.decode()).replace(tzinfo=timezone.utc)
+
+
+sqlite3.register_adapter(datetime, adapt_datetime)
+sqlite3.register_converter("datetime", convert_datetime)
+
+
 class NodeSchema(Schema):
     fields = [
         "id",
         "dir_type",
         "parent_id",
         "name",
         "checksum",
@@ -55,14 +79,33 @@
 DATASET_FIELDS = [
     "name",
     "shadow",
     "description",
     "version",
     "labels",
 ]
+
+DATASET_ROW_FIELDS = [
+    "id",
+    "dir_type",
+    "parent_id",
+    "name",
+    "checksum",
+    "etag",
+    "version",
+    "is_latest",
+    "last_modified",
+    "size",
+    "owner_name",
+    "owner_id",
+    "path_str",
+    "anno",
+    "source",
+]
+
 PATH_STR_INDEX = NodeSchema.fields.index("path_str")
 
 
 class StorageSchema(Schema):
     table = "buckets"
     fields = ["uri", "timestamp", "expires", "status"]
 
@@ -118,31 +161,33 @@
     LISTING_TABLE_NAME_PREFIX = "dsrc_"
     DATASET_TABLE_PREFIX = "ds_"
     TABLE_NAME_SHA_LIMIT = 12
 
     def __init__(self, db_file: Optional[str] = None, table_name: str = ""):
         self.table_name = table_name
         self.db_file = db_file if db_file else DQLDir.find().db
-
+        detect_types = sqlite3.PARSE_DECLTYPES | sqlite3.PARSE_COLNAMES
         try:
             if self.db_file == ":memory:":
                 # Enable multithreaded usage of the same in-memory db
-                self.db = sqlite3.connect("file::memory:?cache=shared", uri=True)
+                self.db = sqlite3.connect(
+                    "file::memory:?cache=shared", uri=True, detect_types=detect_types
+                )
             else:
-                self.db = sqlite3.connect(self.db_file)
+                self.db = sqlite3.connect(self.db_file, detect_types=detect_types)
             self.db.isolation_level = None  # Use autocommit mode
             self.db.execute("PRAGMA foreign_keys = ON")
             self.db.execute("PRAGMA cache_size = -102400")  # 100 MiB
             # Enable Write-Ahead Log Journaling
             self.db.execute("PRAGMA journal_mode = WAL")
             self.db.execute("PRAGMA synchronous = NORMAL")
             self.db.execute("PRAGMA case_sensitive_like = ON")
 
             self._init_storage_table()
-            self._init_datasets_table()
+            self._init_datasets_tables()
         except RuntimeError:
             raise DQLError("Can't connect to SQLite DB")
 
     def _init_storage_table(self):
         """Initialize only tables related to storage, e.g s3"""
         self.db.execute(
             """
@@ -152,26 +197,34 @@
                 timestamp   DATETIME,
                 expires     DATETIME,
                 status      INTEGER NOT NULL
             )
         """
         )
 
-    def _init_datasets_table(self) -> None:
-        self.db.execute(
+    def _init_datasets_tables(self) -> None:
+        self.db.executescript(
             """
             CREATE TABLE IF NOT EXISTS datasets
             (
                 id              INTEGER PRIMARY KEY,
                 name            TEXT NOT NULL UNIQUE,
                 description     TEXT,
-                version         INTEGER,
                 labels          JSON DEFAULT('[]'),
                 shadow          BOOL NOT NULL
             );
+            CREATE TABLE IF NOT EXISTS datasets_versions
+            (
+                id              INTEGER PRIMARY KEY,
+                dataset_id      INTEGER NOT NULL,
+                version         INTEGER NOT NULL,
+                created_at      DATETIME,
+                FOREIGN KEY(dataset_id) REFERENCES datasets(id) ON DELETE CASCADE,
+                UNIQUE(dataset_id, version)
+            );
             """
         )
 
     def init_db(self, prefix: str = "", is_new: bool = True):
         # Note that an index on the primary key (id) is automatically created
         if not prefix or is_new:
             self.db.executescript(
@@ -227,16 +280,22 @@
         return prefix + sha[: cls.TABLE_NAME_SHA_LIMIT]
 
     @classmethod
     def _listing_table_name(cls, uri) -> str:
         return cls._table_name(uri, cls.LISTING_TABLE_NAME_PREFIX)
 
     @classmethod
-    def _dataset_table_name(cls, dataset_id: int) -> str:
-        return cls.DATASET_TABLE_PREFIX + str(dataset_id)
+    def _dataset_table_name(cls, dataset_id: int, version=None) -> str:
+        name = cls.DATASET_TABLE_PREFIX + str(dataset_id)
+        if version:
+            name += f"_{version}"
+        else:
+            name += "_shadow"
+
+        return name
 
     def clone(self, uri: Optional[str] = None) -> "SQLiteDataStorage":
         table_name = self._listing_table_name(uri) if uri else self.table_name
         return SQLiteDataStorage(db_file=self.db_file, table_name=table_name)
 
     # Query starters
     @property
@@ -275,18 +334,23 @@
         return q.wrap(_with_path).all()
 
     def _get_node_by_path_list(self, path_list: List[str]) -> NodeWithPath:
         """
         Gets node that correspond some path list, e.g ["data-lakes", "dogs-and-cats"]
         """
         path_str = "/".join(path_list)
-        node = self.nodes.with_path().where(path_str=path_str, is_latest=True).get()
-        if not node:
+        nodes = (
+            self.nodes.with_path()
+            .where(path_str=path_str, is_latest=True)
+            .order_by("dir_type")
+            .all()
+        )
+        if not nodes:
             raise FileNotFoundError(f"Unable to resolve path {path_str}")
-        return node
+        return nodes[-1]
 
     def _populate_nodes_by_path(
         self, path_list: List[str], num: int, res: List[NodeWithPath]
     ) -> None:
         """
         Puts all nodes found by path_list into the res input variable.
         Note that path can have GLOB like pattern matching which means that
@@ -344,37 +408,70 @@
 
     def get_datasets(
         self, shadow_only: Optional[bool] = None
     ) -> Iterator["DatasetRecord"]:
         if shadow_only is None:
             cond = ""
         elif shadow_only:
-            cond = "WHERE shadow"
+            cond = "WHERE datasets.shadow"
         else:
-            cond = "WHERE NOT shadow"
-        for row in self.db.execute(
+            cond = "WHERE NOT datasets.shadow"
+
+        rows = self.db.execute(
             f"""
             SELECT
-                id,
-                name,
-                description,
-                version,
-                labels,
-                shadow
+                datasets.id,
+                datasets.name,
+                datasets.description,
+                datasets.labels,
+                datasets.shadow,
+                datasets_versions.version
             FROM datasets
+            LEFT JOIN datasets_versions ON datasets.id = datasets_versions.dataset_id
             {cond}
             """,
-        ).fetchall():
-            yield DatasetRecord.parse(*row)
+        ).fetchall()
+
+        for _, g in groupby(rows, operator.itemgetter(0)):
+            dataset = self._parse_dataset(list(g))
+            if dataset:
+                yield dataset
+
+    def create_dataset_rows_table(self, name):
+        # creates special shadow dataset table to store rows
+        self.db.execute(
+            f"""
+            CREATE TABLE IF NOT EXISTS {name}
+            (
+                id              INTEGER PRIMARY KEY,
+                dir_type        INTEGER,
+                parent_id       INTEGER,
+                name            TEXT NOT NULL,
+                checksum        TEXT,
+                etag            TEXT,
+                version         TEXT,
+                is_latest       BOOL,
+                last_modified   DATETIME,
+                size            BIGINT NOT NULL,
+                owner_name      TEXT,
+                owner_id        TEXT,
+                path_str        TEXT,
+                anno            JSON,
+                source          TEXT NOT NULL,
+                UNIQUE(source, path_str)
+            );
+            """
+        )
 
-    def get_dataset_rows(self, name: str, limit=20) -> Iterable[DatasetRow]:
-        # TODO implement listing specific versions
+    def get_dataset_rows(
+        self, name: str, limit=20, version=None
+    ) -> Iterable[DatasetRow]:
         dataset = self.get_dataset(name)
         assert dataset
-        dataset_table_name = self._dataset_table_name(dataset.id)
+        dataset_table_name = self._dataset_table_name(dataset.id, version)
 
         limit_q = ""
         args = []
         if limit:
             limit_q = "LIMIT ?"
             args.append(limit)
 
@@ -394,45 +491,24 @@
                 """INSERT INTO datasets(name, shadow) VALUES (?, ?)
                 ON CONFLICT(name) DO NOTHING
                 """,
                 [name, True],
             )
             dataset = self.get_dataset(name)
             assert dataset
+            assert dataset.shadow
             table_name = self._dataset_table_name(dataset.id)
-
-            # creates special shadow dataset table to store entries
-            self.db.execute(
-                f"""
-                CREATE TABLE IF NOT EXISTS {table_name}
-                (
-                    id              INTEGER PRIMARY KEY,
-                    dir_type        INTEGER,
-                    parent_id       INTEGER,
-                    name            TEXT NOT NULL,
-                    checksum        TEXT,
-                    etag            TEXT,
-                    version         TEXT,
-                    is_latest       BOOL,
-                    last_modified   DATETIME,
-                    size            BIGINT NOT NULL,
-                    owner_name      TEXT,
-                    owner_id        TEXT,
-                    path_str        TEXT,
-                    anno            JSON,
-                    source          TEXT NOT NULL
-                );
-                """
-            )
+            self.create_dataset_rows_table(table_name)
 
     def insert_into_shadow_dataset(
         self, name: str, uri: str, path: str, recursive=False
     ) -> None:
         dataset = self.get_dataset(name)
         assert dataset
+        assert dataset.shadow
 
         source_table_name = self._listing_table_name(uri)
         dataset_table_name = self._dataset_table_name(dataset.id)
 
         self.table_name = source_table_name  # needed for parent node and .nodes
         if recursive:
             if not path.endswith("*"):
@@ -484,14 +560,23 @@
             """
         self.db.execute(
             insert_q,
             [uri] + where_params,
         )
         self.db.commit()
 
+    def rename_dataset_rows(self, name: str, version: int) -> None:
+        dataset = self.get_dataset(name)
+        assert dataset
+
+        old_name = self._dataset_table_name(dataset.id, None)
+        new_name = self._dataset_table_name(dataset.id, version)
+
+        self.db.execute(f"ALTER TABLE {old_name} RENAME TO {new_name}")
+
     def update_dataset(self, dataset_name: str, **kwargs) -> None:
         args = []
         fields = []
         for field, value in kwargs.items():
             if field in DATASET_FIELDS:
                 fields.append(field)
                 if field == "labels":
@@ -504,33 +589,112 @@
             return
 
         args.append(dataset_name)  # for WHERE part
 
         set_query = "SET " + ", ".join(f"{field} = ?" for field in fields)
         self.db.execute(f"UPDATE datasets {set_query} WHERE name = ?", args)
 
+    def create_dataset_version(
+        self, name: str, version: int, create_rows_table=True
+    ) -> DatasetRecord:
+        with self.db:
+            self.db.execute("begin")
+
+            dataset = self.get_dataset(name)
+            assert dataset
+
+            self.db.execute(
+                """INSERT INTO datasets_versions(
+                    dataset_id, version, created_at
+                ) VALUES (?, ?, ?)
+                ON CONFLICT(dataset_id, version) DO NOTHING
+                """,
+                [dataset.id, version, datetime.now(timezone.utc)],
+            )
+
+            if create_rows_table:
+                table_name = self._dataset_table_name(dataset.id, version)
+                self.create_dataset_rows_table(table_name)
+
+            return dataset
+
+    def merge_dataset_rows(
+        self,
+        src: DatasetRecord,
+        dst: DatasetRecord,
+        src_version: Optional[int] = None,
+        dst_version: Optional[int] = None,
+    ) -> None:
+        src_table_name = self._dataset_table_name(src.id, src_version)
+        dst_table_name = self._dataset_table_name(dst.id, dst_version)
+        dst_table_name_latest = self._dataset_table_name(dst.id, dst.latest_version)
+
+        select_fields = ",".join([f for f in DATASET_ROW_FIELDS if f != "id"])
+        self.db.execute(
+            f"""
+            INSERT OR IGNORE INTO {dst_table_name} ({select_fields})
+            SELECT {select_fields} FROM {src_table_name}
+            UNION SELECT {select_fields} from {dst_table_name_latest}
+            """,
+        )
+
+    @staticmethod
+    def _parse_dataset(rows) -> Optional[DatasetRecord]:
+        dataset = None
+        for r in rows:
+            if not dataset:
+                dataset = DatasetRecord.parse(*r)
+                continue
+            dataset.merge_versions(DatasetRecord.parse(*r))  # type: ignore[unreachable]
+
+        return dataset
+
     def get_dataset(self, name: str) -> Optional[DatasetRecord]:
-        res = self.db.execute(
-            "SELECT * from datasets WHERE name = ?", [name]
+        rows = self.db.execute(
+            """
+            SELECT
+                datasets.id,
+                datasets.name,
+                datasets.description,
+                datasets.labels,
+                datasets.shadow,
+                datasets_versions.version
+            FROM datasets
+            LEFT JOIN datasets_versions ON datasets.id = datasets_versions.dataset_id
+            WHERE datasets.name = ?
+            """,
+            [name],
         ).fetchall()
-        if not res:
+        if not rows:
             return None
 
-        assert len(res) == 1, f"Dataset duplication: {name}"
-        return DatasetRecord.parse(*res[0])
+        return self._parse_dataset(rows)
 
-    def remove_dataset(self, name: str) -> None:
-        with self.db:
-            self.db.execute("begin")
-            dataset = self.get_dataset(name)
-            assert dataset
-            dataset_table_name = self._dataset_table_name(dataset.id)
+    def remove_dataset_version(self, dataset: DatasetRecord, version: int) -> None:
+        if not dataset.has_version(version):
+            return
+
+        self.db.execute(
+            """
+            DELETE FROM datasets_versions WHERE dataset_id = ? and version = ?
+            """,
+            [dataset.id, version],
+        )
 
+        if dataset.versions and len(dataset.versions) == 1:
+            # had only one version, fully deleting dataset
             self.db.execute("DELETE FROM datasets WHERE id = ?", [dataset.id])
-            self.db.execute(f"DROP TABLE {dataset_table_name}")
+
+        dataset.remove_version(version)
+
+        self.db.execute(f"DROP TABLE {self._dataset_table_name(dataset.id, version)}")
+
+    def remove_shadow_dataset(self, dataset: DatasetRecord) -> None:
+        self.db.execute("DELETE FROM datasets WHERE id = ?", [dataset.id])
+        self.db.execute(f"DROP TABLE {self._dataset_table_name(dataset.id)}")
 
     @retry_sqlite_locks_async
     async def insert_entry(self, entry: Dict[str, Any]) -> int:
         return self.nodes.insert(self._prepare_node(entry))
 
     @retry_sqlite_locks_async
     async def insert_entries(self, entries: List[Dict[str, Any]]) -> None:
```

### Comparing `dql-alpha-0.8.0/src/dql/jmes_sql/field_ops.py` & `dql-alpha-0.9.0/src/dql/jmes_sql/field_ops.py`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/src/dql/jmes_sql/functions_sql.py` & `dql-alpha-0.9.0/src/dql/jmes_sql/functions_sql.py`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/src/dql/jmes_sql/transpiler.py` & `dql-alpha-0.9.0/src/dql/jmes_sql/transpiler.py`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/src/dql/listing.py` & `dql-alpha-0.9.0/src/dql/listing.py`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/src/dql/node.py` & `dql-alpha-0.9.0/src/dql/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     dir_type: Optional[int] = None
     parent_id: Optional[int] = None
     name: Optional[str] = None
     checksum: str = ""
     etag: str = ""
     version: Optional[str] = None
     is_latest: bool = True
-    last_modified: datetime = datetime.now()
+    last_modified: Optional[datetime] = None
     size: int = 0
     owner_name: str = ""
     owner_id: str = ""
     path_str: str = ""
     anno: Optional[str] = None
```

### Comparing `dql-alpha-0.8.0/src/dql/nodes_fetcher.py` & `dql-alpha-0.9.0/src/dql/nodes_fetcher.py`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/src/dql/nodes_thread_pool.py` & `dql-alpha-0.9.0/src/dql/nodes_thread_pool.py`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/src/dql/remote/studio.py` & `dql-alpha-0.9.0/src/dql/remote/studio.py`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/src/dql/storage.py` & `dql-alpha-0.9.0/src/dql/storage.py`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/src/dql/utils.py` & `dql-alpha-0.9.0/src/dql/utils.py`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/src/dql/vendored/adlfs/_version.py` & `dql-alpha-0.9.0/src/dql/vendored/adlfs/_version.py`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/src/dql/vendored/adlfs/gen1.py` & `dql-alpha-0.9.0/src/dql/vendored/adlfs/gen1.py`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/src/dql/vendored/adlfs/spec.py` & `dql-alpha-0.9.0/src/dql/vendored/adlfs/spec.py`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/src/dql/vendored/adlfs/utils.py` & `dql-alpha-0.9.0/src/dql/vendored/adlfs/utils.py`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/src/dql/vendored/gcsfs/_version.py` & `dql-alpha-0.9.0/src/dql/vendored/gcsfs/_version.py`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/src/dql/vendored/gcsfs/checkers.py` & `dql-alpha-0.9.0/src/dql/vendored/gcsfs/checkers.py`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/src/dql/vendored/gcsfs/cli/gcsfuse.py` & `dql-alpha-0.9.0/src/dql/vendored/gcsfs/cli/gcsfuse.py`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/src/dql/vendored/gcsfs/core.py` & `dql-alpha-0.9.0/src/dql/vendored/gcsfs/core.py`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/src/dql/vendored/gcsfs/credentials.py` & `dql-alpha-0.9.0/src/dql/vendored/gcsfs/credentials.py`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/src/dql/vendored/gcsfs/retry.py` & `dql-alpha-0.9.0/src/dql/vendored/gcsfs/retry.py`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/src/dql_alpha.egg-info/PKG-INFO` & `dql-alpha-0.9.0/src/dql_alpha.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dql-alpha
-Version: 0.8.0
+Version: 0.9.0
 Summary: DQL
 Home-page: https://github.com/iterative/dql
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dql-alpha-0.8.0/src/dql_alpha.egg-info/SOURCES.txt` & `dql-alpha-0.9.0/src/dql_alpha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/src/dql_alpha.egg-info/requires.txt` & `dql-alpha-0.9.0/src/dql_alpha.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 pyyaml
 tomlkit
 tqdm
 reflink
+python-dateutil>=2
 attrs>=21.3.0
 funcy>=1.14
 s3fs>=2023.1.0
 decorator>4.1.2
 fsspec==2023.1.0
 google-auth>=1.2
 google-auth-oauthlib
```

### Comparing `dql-alpha-0.8.0/tests/benchmarks/conftest.py` & `dql-alpha-0.9.0/tests/benchmarks/conftest.py`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/tests/conftest.py` & `dql-alpha-0.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/tests/func/test_catalog.py` & `dql-alpha-0.9.0/tests/func/test_catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -860,15 +860,15 @@
         client_config=cloud_test_catalog.client_config,
         recursive=True,
     )
 
     dataset = catalog.data_storage.get_dataset(shadow_dataset_name)
     assert dataset.name == shadow_dataset_name
     assert dataset.description is None
-    assert dataset.version is None
+    assert dataset.versions is None
     assert dataset.labels == []
     assert dataset.shadow is True
 
     dataset_table_name = catalog.data_storage._dataset_table_name(dataset.id)
     data = catalog.data_storage.db.execute(
         f"select * from {dataset_table_name}"
     ).fetchall()
@@ -881,18 +881,18 @@
     catalog.register(
         dogs_shadow_dataset.name,
         description="dogs dataset",
         labels=["dogs", "dataset"],
     )
 
     dataset = catalog.data_storage.get_dataset(dogs_shadow_dataset.name)
-    dataset_table_name = catalog.data_storage._dataset_table_name(dataset.id)
+    dataset_table_name = catalog.data_storage._dataset_table_name(dataset.id, 1)
     assert dataset.name == dogs_shadow_dataset.name
     assert dataset.description == "dogs dataset"
-    assert dataset.version == 1
+    assert dataset.versions == [1]
     assert dataset.labels == ["dogs", "dataset"]
     assert dataset.shadow is False
     data = catalog.data_storage.db.execute(
         f"select * from {dataset_table_name}"
     ).fetchall()
     assert data
 
@@ -905,15 +905,15 @@
         dogs_shadow_dataset.name,
         new_dataset_name=new_dataset_name,
         description="dogs dataset",
         labels=["dogs", "dataset"],
     )
     dataset = catalog.data_storage.get_dataset(new_dataset_name)
     assert dataset
-    dataset_table_name = catalog.data_storage._dataset_table_name(dataset.id)
+    dataset_table_name = catalog.data_storage._dataset_table_name(dataset.id, 1)
     assert dataset.name == new_dataset_name
     data = catalog.data_storage.db.execute(
         f"select * from {dataset_table_name}"
     ).fetchall()
     assert data
 
 
@@ -926,15 +926,15 @@
         dogs_shadow_dataset.name,
         version=5,
         description="dogs dataset",
         labels=["dogs", "dataset"],
     )
 
     dataset = catalog.data_storage.get_dataset(dogs_shadow_dataset.name)
-    assert dataset.version == 5
+    assert dataset.versions == [5]
 
 
 def test_removing_dataset(cloud_test_catalog, dogs_shadow_dataset):
     catalog = cloud_test_catalog.catalog
 
     dataset_table_name = catalog.data_storage._dataset_table_name(
         dogs_shadow_dataset.id
@@ -961,22 +961,24 @@
         dogs_registered_dataset.name,
         new_name=dataset_new_name,
         description="new description",
         labels=["cats", "birds"],
     )
 
     dataset = catalog.data_storage.get_dataset(dataset_new_name)
-    assert dataset.version == 1
+    assert dataset.versions == [1]
     assert dataset.name == dataset_new_name
     assert dataset.description == "new description"
     assert dataset.labels == ["cats", "birds"]
 
 
 def test_ls_dataset_rows(cloud_test_catalog, dogs_registered_dataset):
     catalog = cloud_test_catalog.catalog
 
-    assert [r.name for r in catalog.ls_dataset_rows(dogs_registered_dataset.name)] == [
+    assert [
+        r.name for r in catalog.ls_dataset_rows(dogs_registered_dataset.name, version=1)
+    ] == [
         "dog1",
         "dog2",
         "dog3",
         "dog4",
     ]
```

### Comparing `dql-alpha-0.8.0/tests/func/test_ls.py` & `dql-alpha-0.9.0/tests/func/test_ls.py`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/tests/unit/test_cli_parsing.py` & `dql-alpha-0.9.0/tests/unit/test_cli_parsing.py`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/tests/unit/test_client_s3.py` & `dql-alpha-0.9.0/tests/unit/test_client_s3.py`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/tests/unit/test_json.py` & `dql-alpha-0.9.0/tests/unit/test_json.py`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/tests/unit/test_listing.py` & `dql-alpha-0.9.0/tests/unit/test_listing.py`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/tests/unit/test_storage.py` & `dql-alpha-0.9.0/tests/unit/test_storage.py`

 * *Files identical despite different names*

### Comparing `dql-alpha-0.8.0/tests/unit/test_utils.py` & `dql-alpha-0.9.0/tests/unit/test_utils.py`

 * *Files identical despite different names*

