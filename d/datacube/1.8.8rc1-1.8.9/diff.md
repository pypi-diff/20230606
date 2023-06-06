# Comparing `tmp/datacube-1.8.8rc1.tar.gz` & `tmp/datacube-1.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datacube-1.8.8rc1.tar", last modified: Thu Sep 29 03:02:56 2022, max compression
+gzip compressed data, was "datacube-1.8.9.tar", last modified: Thu Nov 17 00:48:13 2022, max compression
```

## Comparing `datacube-1.8.8rc1.tar` & `datacube-1.8.9.tar`

### file list

```diff
@@ -1,400 +1,404 @@
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.658266 datacube-1.8.8rc1/
--rw-r--r--   0 odc       (1001) odc        (121)      492 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/.coveragerc
--rw-r--r--   0 odc       (1001) odc        (121)      982 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/.dockerignore
--rw-r--r--   0 odc       (1001) odc        (121)      487 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/.editorconfig
--rw-r--r--   0 odc       (1001) odc        (121)      203 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/.gitattributes
--rw-r--r--   0 odc       (1001) odc        (121)     1072 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/.gitignore
--rw-r--r--   0 odc       (1001) odc        (121)      452 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/.mergify.yml
--rw-r--r--   0 odc       (1001) odc        (121)      751 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/.pre-commit-config.yaml
--rw-r--r--   0 odc       (1001) odc        (121)      923 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/.yamllint
--rw-r--r--   0 odc       (1001) odc        (121)     1231 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/CONTRIBUTING.md
--rw-r--r--   0 odc       (1001) odc        (121)    11357 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/LICENSE
--rw-r--r--   0 odc       (1001) odc        (121)       70 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/MANIFEST.in
--rw-rw-r--   0 odc       (1001) odc        (121)     5284 2022-09-29 03:02:56.658266 datacube-1.8.8rc1/PKG-INFO
--rw-r--r--   0 odc       (1001) odc        (121)     3882 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/README.rst
--rwxr-xr-x   0 odc       (1001) odc        (121)      980 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/check-code.sh
--rw-r--r--   0 odc       (1001) odc        (121)     3507 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/code-of-conduct.md
--rw-r--r--   0 odc       (1001) odc        (121)      503 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/conda-environment.yml
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.618265 datacube-1.8.8rc1/datacube/
--rw-r--r--   0 odc       (1001) odc        (121)     1128 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/__init__.py
--rw-r--r--   0 odc       (1001) odc        (121)      257 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/__main__.py
--rw-rw-r--   0 odc       (1001) odc        (121)      179 2022-09-29 03:02:56.000000 datacube-1.8.8rc1/datacube/_version.py
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.622265 datacube-1.8.8rc1/datacube/api/
--rw-r--r--   0 odc       (1001) odc        (121)      416 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/api/__init__.py
--rw-r--r--   0 odc       (1001) odc        (121)    44021 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/api/core.py
--rw-r--r--   0 odc       (1001) odc        (121)    16365 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/api/grid_workflow.py
--rw-r--r--   0 odc       (1001) odc        (121)    14909 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/api/query.py
--rwxr-xr-x   0 odc       (1001) odc        (121)     9494 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/config.py
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.622265 datacube-1.8.8rc1/datacube/drivers/
--rw-r--r--   0 odc       (1001) odc        (121)      587 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/drivers/__init__.py
--rw-r--r--   0 odc       (1001) odc        (121)     1065 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/drivers/_tools.py
--rw-r--r--   0 odc       (1001) odc        (121)     2938 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/drivers/_types.py
--rw-r--r--   0 odc       (1001) odc        (121)     1739 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/drivers/datasource.py
--rw-r--r--   0 odc       (1001) odc        (121)     2057 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/drivers/driver_cache.py
--rw-r--r--   0 odc       (1001) odc        (121)     1822 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/drivers/indexes.py
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.622265 datacube-1.8.8rc1/datacube/drivers/netcdf/
--rw-r--r--   0 odc       (1001) odc        (121)      432 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/drivers/netcdf/__init__.py
--rw-r--r--   0 odc       (1001) odc        (121)     3014 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/drivers/netcdf/_safestrings.py
--rw-r--r--   0 odc       (1001) odc        (121)     4868 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/drivers/netcdf/_write.py
--rw-r--r--   0 odc       (1001) odc        (121)     2571 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/drivers/netcdf/driver.py
--rw-r--r--   0 odc       (1001) odc        (121)    11299 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/drivers/netcdf/writer.py
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.622265 datacube-1.8.8rc1/datacube/drivers/postgis/
--rw-r--r--   0 odc       (1001) odc        (121)      396 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/drivers/postgis/__init__.py
--rw-r--r--   0 odc       (1001) odc        (121)    37818 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/drivers/postgis/_api.py
--rwxr-xr-x   0 odc       (1001) odc        (121)    11346 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/drivers/postgis/_connections.py
--rw-r--r--   0 odc       (1001) odc        (121)     8756 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/drivers/postgis/_core.py
--rw-r--r--   0 odc       (1001) odc        (121)     6997 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/drivers/postgis/_dynamic.py
--rwxr-xr-x   0 odc       (1001) odc        (121)    19056 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/drivers/postgis/_fields.py
--rw-r--r--   0 odc       (1001) odc        (121)     9130 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/drivers/postgis/_schema.py
--rw-r--r--   0 odc       (1001) odc        (121)     6165 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/drivers/postgis/_spatial.py
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.622265 datacube-1.8.8rc1/datacube/drivers/postgis/samples/
--rw-r--r--   0 odc       (1001) odc        (121)     4023 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/drivers/postgis/samples/range-tests-explicit.sql
--rw-r--r--   0 odc       (1001) odc        (121)     2229 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/drivers/postgis/samples/range-tests-scalar.sql
--rw-r--r--   0 odc       (1001) odc        (121)     2687 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/drivers/postgis/samples/range-tests-view.sql
--rw-r--r--   0 odc       (1001) odc        (121)     4299 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/drivers/postgis/sql.py
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.626265 datacube-1.8.8rc1/datacube/drivers/postgres/
--rw-r--r--   0 odc       (1001) odc        (121)      400 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/drivers/postgres/__init__.py
--rw-r--r--   0 odc       (1001) odc        (121)    38831 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/drivers/postgres/_api.py
--rwxr-xr-x   0 odc       (1001) odc        (121)     9981 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/drivers/postgres/_connections.py
--rw-r--r--   0 odc       (1001) odc        (121)     9488 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/drivers/postgres/_core.py
--rw-r--r--   0 odc       (1001) odc        (121)     6346 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/drivers/postgres/_dynamic.py
--rwxr-xr-x   0 odc       (1001) odc        (121)    19058 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/drivers/postgres/_fields.py
--rw-r--r--   0 odc       (1001) odc        (121)     6455 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/drivers/postgres/_schema.py
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.626265 datacube-1.8.8rc1/datacube/drivers/postgres/samples/
--rw-r--r--   0 odc       (1001) odc        (121)     4029 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/drivers/postgres/samples/range-tests-explicit.sql
--rw-r--r--   0 odc       (1001) odc        (121)     2235 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/drivers/postgres/samples/range-tests-scalar.sql
--rw-r--r--   0 odc       (1001) odc        (121)     2692 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/drivers/postgres/samples/range-tests-view.sql
--rw-r--r--   0 odc       (1001) odc        (121)     4302 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/drivers/postgres/sql.py
--rw-r--r--   0 odc       (1001) odc        (121)     3533 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/drivers/readers.py
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.626265 datacube-1.8.8rc1/datacube/drivers/rio/
--rw-r--r--   0 odc       (1001) odc        (121)      206 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/drivers/rio/__init__.py
--rw-r--r--   0 odc       (1001) odc        (121)     7109 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/drivers/rio/_reader.py
--rw-r--r--   0 odc       (1001) odc        (121)     1538 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/drivers/writers.py
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.626265 datacube-1.8.8rc1/datacube/execution/
--rw-r--r--   0 odc       (1001) odc        (121)      176 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/execution/__init__.py
--rw-r--r--   0 odc       (1001) odc        (121)     1893 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/execution/worker.py
--rw-r--r--   0 odc       (1001) odc        (121)     7203 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/executor.py
--rw-r--r--   0 odc       (1001) odc        (121)     1597 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/helpers.py
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.626265 datacube-1.8.8rc1/datacube/index/
--rw-r--r--   0 odc       (1001) odc        (121)      597 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/index/__init__.py
--rw-r--r--   0 odc       (1001) odc        (121)     1702 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/index/_api.py
--rw-r--r--   0 odc       (1001) odc        (121)    47218 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/index/abstract.py
--rw-r--r--   0 odc       (1001) odc        (121)    10617 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/index/default-metadata-types.yaml
--rw-r--r--   0 odc       (1001) odc        (121)     8192 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/index/eo3.py
--rw-r--r--   0 odc       (1001) odc        (121)      500 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/index/exceptions.py
--rw-r--r--   0 odc       (1001) odc        (121)     2272 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/index/fields.py
--rw-r--r--   0 odc       (1001) odc        (121)    12373 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/index/hl.py
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.626265 datacube-1.8.8rc1/datacube/index/memory/
--rw-r--r--   0 odc       (1001) odc        (121)      191 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/index/memory/__init__.py
--rwxr-xr-x   0 odc       (1001) odc        (121)    30858 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/index/memory/_datasets.py
--rw-r--r--   0 odc       (1001) odc        (121)     1709 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/index/memory/_fields.py
--rw-r--r--   0 odc       (1001) odc        (121)     5382 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/index/memory/_metadata_types.py
--rw-r--r--   0 odc       (1001) odc        (121)     7705 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/index/memory/_products.py
--rw-r--r--   0 odc       (1001) odc        (121)     2462 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/index/memory/_users.py
--rw-r--r--   0 odc       (1001) odc        (121)     3020 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/index/memory/index.py
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.630265 datacube-1.8.8rc1/datacube/index/null/
--rw-r--r--   0 odc       (1001) odc        (121)      191 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/index/null/__init__.py
--rwxr-xr-x   0 odc       (1001) odc        (121)     2986 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/index/null/_datasets.py
--rw-r--r--   0 odc       (1001) odc        (121)     1123 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/index/null/_metadata_types.py
--rw-r--r--   0 odc       (1001) odc        (121)     1178 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/index/null/_products.py
--rw-r--r--   0 odc       (1001) odc        (121)      802 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/index/null/_users.py
--rw-r--r--   0 odc       (1001) odc        (121)     2877 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/index/null/index.py
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.630265 datacube-1.8.8rc1/datacube/index/postgis/
--rw-r--r--   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/index/postgis/__init__.py
--rwxr-xr-x   0 odc       (1001) odc        (121)    35589 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/index/postgis/_datasets.py
--rw-r--r--   0 odc       (1001) odc        (121)     9471 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/index/postgis/_metadata_types.py
--rw-r--r--   0 odc       (1001) odc        (121)    13586 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/index/postgis/_products.py
--rw-r--r--   0 odc       (1001) odc        (121)     2405 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/index/postgis/_transaction.py
--rw-r--r--   0 odc       (1001) odc        (121)     1819 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/index/postgis/_users.py
--rw-r--r--   0 odc       (1001) odc        (121)     8239 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/index/postgis/index.py
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.630265 datacube-1.8.8rc1/datacube/index/postgres/
--rw-r--r--   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/index/postgres/__init__.py
--rwxr-xr-x   0 odc       (1001) odc        (121)    35174 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/index/postgres/_datasets.py
--rw-r--r--   0 odc       (1001) odc        (121)     9611 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/index/postgres/_metadata_types.py
--rw-r--r--   0 odc       (1001) odc        (121)    13856 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/index/postgres/_products.py
--rw-r--r--   0 odc       (1001) odc        (121)     2403 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/index/postgres/_transaction.py
--rw-r--r--   0 odc       (1001) odc        (121)     1839 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/index/postgres/_users.py
--rw-r--r--   0 odc       (1001) odc        (121)     6838 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/index/postgres/index.py
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.630265 datacube-1.8.8rc1/datacube/model/
--rw-r--r--   0 odc       (1001) odc        (121)    38428 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/model/__init__.py
--rw-r--r--   0 odc       (1001) odc        (121)      593 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/model/_base.py
--rw-r--r--   0 odc       (1001) odc        (121)     5933 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/model/fields.py
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.630265 datacube-1.8.8rc1/datacube/model/schema/
--rw-r--r--   0 odc       (1001) odc        (121)     5564 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/model/schema/dataset-type-schema.yaml
--rw-r--r--   0 odc       (1001) odc        (121)     4734 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/model/schema/ingestor-config-type-schema.yaml
--rw-r--r--   0 odc       (1001) odc        (121)     2033 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/model/schema/metadata-type-schema.yaml
--rw-r--r--   0 odc       (1001) odc        (121)    14179 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/model/utils.py
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.630265 datacube-1.8.8rc1/datacube/scripts/
--rw-r--r--   0 odc       (1001) odc        (121)      176 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/scripts/__init__.py
--rw-r--r--   0 odc       (1001) odc        (121)      596 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/scripts/cli_app.py
--rw-r--r--   0 odc       (1001) odc        (121)    24391 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/scripts/dataset.py
--rw-r--r--   0 odc       (1001) odc        (121)    17593 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/scripts/ingest.py
--rw-r--r--   0 odc       (1001) odc        (121)     6010 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/scripts/metadata.py
--rw-r--r--   0 odc       (1001) odc        (121)     9017 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/scripts/product.py
--rwxr-xr-x   0 odc       (1001) odc        (121)     3842 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/scripts/search_tool.py
--rw-r--r--   0 odc       (1001) odc        (121)     3349 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/scripts/system.py
--rw-r--r--   0 odc       (1001) odc        (121)     3268 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/scripts/user.py
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.630265 datacube-1.8.8rc1/datacube/storage/
--rw-r--r--   0 odc       (1001) odc        (121)      594 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/storage/__init__.py
--rw-r--r--   0 odc       (1001) odc        (121)     3677 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/storage/_base.py
--rw-r--r--   0 odc       (1001) odc        (121)      224 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/storage/_hdf5.py
--rw-r--r--   0 odc       (1001) odc        (121)     6150 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/storage/_load.py
--rw-r--r--   0 odc       (1001) odc        (121)     8212 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/storage/_read.py
--rw-r--r--   0 odc       (1001) odc        (121)     7585 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/storage/_rio.py
--rw-r--r--   0 odc       (1001) odc        (121)      372 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/storage/masking.py
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.630265 datacube-1.8.8rc1/datacube/testutils/
--rw-r--r--   0 odc       (1001) odc        (121)    14223 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/testutils/__init__.py
--rw-r--r--   0 odc       (1001) odc        (121)     5003 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/testutils/geom.py
--rw-r--r--   0 odc       (1001) odc        (121)    11871 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/testutils/io.py
--rw-r--r--   0 odc       (1001) odc        (121)     2139 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/testutils/iodriver.py
--rw-r--r--   0 odc       (1001) odc        (121)      797 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/testutils/threads.py
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.630265 datacube-1.8.8rc1/datacube/ui/
--rw-r--r--   0 odc       (1001) odc        (121)      418 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/ui/__init__.py
--rw-r--r--   0 odc       (1001) odc        (121)    11874 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/ui/click.py
--rw-r--r--   0 odc       (1001) odc        (121)     4191 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/ui/common.py
--rw-r--r--   0 odc       (1001) odc        (121)     3786 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/ui/expression.py
--rw-r--r--   0 odc       (1001) odc        (121)    10704 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/ui/task_app.py
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.634265 datacube-1.8.8rc1/datacube/utils/
--rw-r--r--   0 odc       (1001) odc        (121)     1956 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/utils/__init__.py
--rw-r--r--   0 odc       (1001) odc        (121)      502 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/utils/_misc.py
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.634265 datacube-1.8.8rc1/datacube/utils/aws/
--rw-r--r--   0 odc       (1001) odc        (121)    17300 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/utils/aws/__init__.py
--rw-r--r--   0 odc       (1001) odc        (121)     6581 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/utils/changes.py
--rw-r--r--   0 odc       (1001) odc        (121)    14314 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/utils/cog.py
--rw-r--r--   0 odc       (1001) odc        (121)    11374 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/utils/dask.py
--rw-r--r--   0 odc       (1001) odc        (121)     4425 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/utils/dates.py
--rw-r--r--   0 odc       (1001) odc        (121)    16178 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/utils/documents.py
--rw-r--r--   0 odc       (1001) odc        (121)     2761 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/utils/generic.py
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.634265 datacube-1.8.8rc1/datacube/utils/geometry/
--rw-r--r--   0 odc       (1001) odc        (121)     2645 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/utils/geometry/__init__.py
--rw-r--r--   0 odc       (1001) odc        (121)    47511 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/utils/geometry/_base.py
--rw-r--r--   0 odc       (1001) odc        (121)     5948 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/utils/geometry/_warp.py
--rw-r--r--   0 odc       (1001) odc        (121)     7772 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/utils/geometry/gbox.py
--rw-r--r--   0 odc       (1001) odc        (121)    18117 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/utils/geometry/tools.py
--rw-r--r--   0 odc       (1001) odc        (121)     2293 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/utils/io.py
--rw-r--r--   0 odc       (1001) odc        (121)     8989 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/utils/masking.py
--rw-r--r--   0 odc       (1001) odc        (121)     8600 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/utils/math.py
--rw-r--r--   0 odc       (1001) odc        (121)     2225 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/utils/py.py
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.634265 datacube-1.8.8rc1/datacube/utils/rio/
--rw-r--r--   0 odc       (1001) odc        (121)      648 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/utils/rio/__init__.py
--rw-r--r--   0 odc       (1001) odc        (121)     5105 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/utils/rio/_rio.py
--rw-r--r--   0 odc       (1001) odc        (121)     2336 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/utils/serialise.py
--rw-r--r--   0 odc       (1001) odc        (121)     6442 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/utils/uris.py
--rw-r--r--   0 odc       (1001) odc        (121)     5777 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/utils/xarray_geoextensions.py
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.634265 datacube-1.8.8rc1/datacube/virtual/
--rw-r--r--   0 odc       (1001) odc        (121)     7775 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/virtual/__init__.py
--rw-r--r--   0 odc       (1001) odc        (121)     2368 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/virtual/catalog.py
--rw-r--r--   0 odc       (1001) odc        (121)     4712 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/virtual/expr.py
--rw-r--r--   0 odc       (1001) odc        (121)    40209 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/virtual/impl.py
--rw-r--r--   0 odc       (1001) odc        (121)    16795 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/virtual/transformations.py
--rw-r--r--   0 odc       (1001) odc        (121)     1634 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/datacube/virtual/utils.py
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.618265 datacube-1.8.8rc1/datacube.egg-info/
--rw-rw-r--   0 odc       (1001) odc        (121)     5284 2022-09-29 03:02:56.000000 datacube-1.8.8rc1/datacube.egg-info/PKG-INFO
--rw-rw-r--   0 odc       (1001) odc        (121)    13985 2022-09-29 03:02:56.000000 datacube-1.8.8rc1/datacube.egg-info/SOURCES.txt
--rw-rw-r--   0 odc       (1001) odc        (121)        1 2022-09-29 03:02:56.000000 datacube-1.8.8rc1/datacube.egg-info/dependency_links.txt
--rw-rw-r--   0 odc       (1001) odc        (121)      581 2022-09-29 03:02:56.000000 datacube-1.8.8rc1/datacube.egg-info/entry_points.txt
--rw-rw-r--   0 odc       (1001) odc        (121)     1131 2022-09-29 03:02:56.000000 datacube-1.8.8rc1/datacube.egg-info/requires.txt
--rw-rw-r--   0 odc       (1001) odc        (121)        9 2022-09-29 03:02:56.000000 datacube-1.8.8rc1/datacube.egg-info/top_level.txt
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.614264 datacube-1.8.8rc1/examples/
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.634265 datacube-1.8.8rc1/examples/io_plugin/
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.634265 datacube-1.8.8rc1/examples/io_plugin/dcio_example/
--rw-r--r--   0 odc       (1001) odc        (121)      176 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/examples/io_plugin/dcio_example/__init__.py
--rw-r--r--   0 odc       (1001) odc        (121)     3855 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/examples/io_plugin/dcio_example/pickles.py
--rw-r--r--   0 odc       (1001) odc        (121)     5961 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/examples/io_plugin/dcio_example/xarray_3d.py
--rw-r--r--   0 odc       (1001) odc        (121)      607 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/examples/io_plugin/dcio_example/zeros.py
--rw-r--r--   0 odc       (1001) odc        (121)      747 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/examples/io_plugin/setup.py
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.638265 datacube-1.8.8rc1/integration_tests/
--rw-r--r--   0 odc       (1001) odc        (121)      191 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/__init__.py
--rw-r--r--   0 odc       (1001) odc        (121)      276 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/agdcintegration.conf
--rw-r--r--   0 odc       (1001) odc        (121)      366 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/ancillary-collection.yaml
--rw-r--r--   0 odc       (1001) odc        (121)    21327 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/conftest.py
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.614264 datacube-1.8.8rc1/integration_tests/data/
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.638265 datacube-1.8.8rc1/integration_tests/data/dataset_add/
--rw-r--r--   0 odc       (1001) odc        (121)     3112 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/data/dataset_add/datasets.yml
--rw-r--r--   0 odc       (1001) odc        (121)     1624 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/data/dataset_add/datasets_bad1.yml
--rw-r--r--   0 odc       (1001) odc        (121)     1010 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/data/dataset_add/datasets_eo3.yml
--rw-r--r--   0 odc       (1001) odc        (121)      243 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/data/dataset_add/datasets_no_id.yml
--rw-r--r--   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/data/dataset_add/empty_file.yml
--rw-r--r--   0 odc       (1001) odc        (121)     1664 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/data/dataset_add/metadata.yml
--rw-r--r--   0 odc       (1001) odc        (121)      820 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/data/dataset_add/products.yml
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.638265 datacube-1.8.8rc1/integration_tests/data/eo3/
--rw-r--r--   0 odc       (1001) odc        (121)     3527 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/data/eo3/ard_ls8.odc-product.yaml
--rw-r--r--   0 odc       (1001) odc        (121)     7591 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/data/eo3/eo3_landsat_ard.odc-type.yaml
--rw-r--r--   0 odc       (1001) odc        (121)     1473 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/data/eo3/ga_ls_wo_3.odc-product.yaml
--rw-r--r--   0 odc       (1001) odc        (121)     4793 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/data/eo3/ls8_dataset.yaml
--rw-r--r--   0 odc       (1001) odc        (121)     4725 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/data/eo3/ls8_dataset2.yaml
--rw-r--r--   0 odc       (1001) odc        (121)     5271 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/data/eo3/ls8_dataset3.yaml
--rw-r--r--   0 odc       (1001) odc        (121)     5367 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/data/eo3/ls8_dataset4.yaml
--rw-r--r--   0 odc       (1001) odc        (121)     2823 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/data/eo3/s2_africa_dataset.yaml
--rw-r--r--   0 odc       (1001) odc        (121)     2210 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/data/eo3/s2_africa_product.yaml
--rw-r--r--   0 odc       (1001) odc        (121)     3165 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/data/eo3/wo_dataset.yaml
--rw-r--r--   0 odc       (1001) odc        (121)     8571 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/data/eo3/wo_ds_with_lineage.odc-metadata.yaml
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.638265 datacube-1.8.8rc1/integration_tests/data/ingester/
--rw-r--r--   0 odc       (1001) odc        (121)     4787 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/data/ingester/invalid_config.yaml
--rw-r--r--   0 odc       (1001) odc        (121)     4810 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/data/ingester/invalid_src_name.yaml
--rw-r--r--   0 odc       (1001) odc        (121)     6554 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/data_utils.py
--rw-r--r--   0 odc       (1001) odc        (121)     8099 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/example-ls5-nbar.yaml
--rw-r--r--   0 odc       (1001) odc        (121)     2136 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/example-ls5-nbar_302.yaml
--rw-r--r--   0 odc       (1001) odc        (121)     2135 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/example-ls5-nbar_505.yaml
--rw-r--r--   0 odc       (1001) odc        (121)     2130 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/example-ls5-nbar_606.yaml
--rw-r--r--   0 odc       (1001) odc        (121)     3084 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/extensive-eo-metadata.yaml
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.642265 datacube-1.8.8rc1/integration_tests/index/
--rw-r--r--   0 odc       (1001) odc        (121)      191 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/index/__init__.py
--rw-r--r--   0 odc       (1001) odc        (121)     1580 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/index/search_utils.py
--rw-r--r--   0 odc       (1001) odc        (121)    23413 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/index/test_config_docs.py
--rwxr-xr-x   0 odc       (1001) odc        (121)    21199 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/index/test_index_data.py
--rw-r--r--   0 odc       (1001) odc        (121)    25099 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/index/test_memory_index.py
--rw-r--r--   0 odc       (1001) odc        (121)     6653 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/index/test_null_index.py
--rw-r--r--   0 odc       (1001) odc        (121)      863 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/index/test_pluggable_indexes.py
--rw-r--r--   0 odc       (1001) odc        (121)     8471 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/index/test_postgis_index.py
--rw-r--r--   0 odc       (1001) odc        (121)    28100 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/index/test_search_eo3.py
--rw-r--r--   0 odc       (1001) odc        (121)    37077 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/index/test_search_legacy.py
--rw-r--r--   0 odc       (1001) odc        (121)     4046 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/index/test_update_columns.py
--rw-r--r--   0 odc       (1001) odc        (121)    16931 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/test_3d.py
--rw-r--r--   0 odc       (1001) odc        (121)     6568 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/test_cli_output.py
--rw-r--r--   0 odc       (1001) odc        (121)     9298 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/test_config_tool.py
--rw-r--r--   0 odc       (1001) odc        (121)    22762 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/test_dataset_add.py
--rw-r--r--   0 odc       (1001) odc        (121)     3210 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/test_double_ingestion.py
--rw-r--r--   0 odc       (1001) odc        (121)    12134 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/test_end_to_end.py
--rw-r--r--   0 odc       (1001) odc        (121)     2369 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/test_environments.py
--rw-r--r--   0 odc       (1001) odc        (121)    10516 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/test_full_ingestion.py
--rw-r--r--   0 odc       (1001) odc        (121)     6570 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/test_index_datasets_search.py
--rw-r--r--   0 odc       (1001) odc        (121)     3712 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/test_index_out_of_bound.py
--rw-r--r--   0 odc       (1001) odc        (121)     1654 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/test_model.py
--rw-r--r--   0 odc       (1001) odc        (121)     1318 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/test_validate_ingestion.py
--rw-r--r--   0 odc       (1001) odc        (121)     7856 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/integration_tests/utils.py
--rw-r--r--   0 odc       (1001) odc        (121)     1115 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/license-headers.md
--rw-r--r--   0 odc       (1001) odc        (121)      168 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/license-template.txt
--rw-r--r--   0 odc       (1001) odc        (121)       84 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/mypy.ini
--rw-r--r--   0 odc       (1001) odc        (121)     7160 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/pylintrc
--rw-r--r--   0 odc       (1001) odc        (121)      157 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/pyproject.toml
--rw-r--r--   0 odc       (1001) odc        (121)      162 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/pytest.ini
--rw-r--r--   0 odc       (1001) odc        (121)      190 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/readthedocs.yml
--rw-r--r--   0 odc       (1001) odc        (121)      235 2022-09-29 03:02:56.658266 datacube-1.8.8rc1/setup.cfg
--rwxr-xr-x   0 odc       (1001) odc        (121)     4128 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/setup.py
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.646265 datacube-1.8.8rc1/tests/
--rw-r--r--   0 odc       (1001) odc        (121)      176 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/__init__.py
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.646265 datacube-1.8.8rc1/tests/api/
--rw-r--r--   0 odc       (1001) odc        (121)      176 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/api/__init__.py
--rw-r--r--   0 odc       (1001) odc        (121)     4023 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/api/test_core.py
--rw-r--r--   0 odc       (1001) odc        (121)     9416 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/api/test_grid_workflow.py
--rw-r--r--   0 odc       (1001) odc        (121)    13832 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/api/test_masking.py
--rw-r--r--   0 odc       (1001) odc        (121)     8412 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/api/test_query.py
--rw-r--r--   0 odc       (1001) odc        (121)    21799 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/api/test_virtual.py
--rw-r--r--   0 odc       (1001) odc        (121)    10302 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/conftest.py
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.650266 datacube-1.8.8rc1/tests/data/
--rw-r--r--   0 odc       (1001) odc        (121)     8099 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/ds_eo.yaml
--rw-r--r--   0 odc       (1001) odc        (121)      519 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/ds_eo3.yml
--rw-r--r--   0 odc       (1001) odc        (121)      431 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/ds_non-geo.yaml
--rw-r--r--   0 odc       (1001) odc        (121)     2516 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/eo3.yaml
--rw-r--r--   0 odc       (1001) odc        (121)      470 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/ingest_config.yaml
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.614264 datacube-1.8.8rc1/tests/data/lbg/
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.650266 datacube-1.8.8rc1/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/
--rw-r--r--   0 odc       (1001) odc        (121)     2266 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/agdc-metadata.yaml
--rw-r--r--   0 odc       (1001) odc        (121)    10247 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/metadata.xml
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.650266 datacube-1.8.8rc1/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/
--rw-r--r--   0 odc       (1001) odc        (121)   369231 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B10.tif
--rw-r--r--   0 odc       (1001) odc        (121)   369231 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B20.tif
--rw-r--r--   0 odc       (1001) odc        (121)   369231 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B30.tif
--rw-r--r--   0 odc       (1001) odc        (121)   369231 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B40.tif
--rw-r--r--   0 odc       (1001) odc        (121)   369231 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B50.tif
--rw-r--r--   0 odc       (1001) odc        (121)   369231 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B70.tif
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.650266 datacube-1.8.8rc1/tests/data/lbg/LS5_TM_PQ_P55_GAPQ01-002_090_084_19920323/
--rw-r--r--   0 odc       (1001) odc        (121)     4590 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/lbg/LS5_TM_PQ_P55_GAPQ01-002_090_084_19920323/agdc-metadata.yaml
--rw-r--r--   0 odc       (1001) odc        (121)     8550 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/lbg/LS5_TM_PQ_P55_GAPQ01-002_090_084_19920323/metadata.xml
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.650266 datacube-1.8.8rc1/tests/data/lbg/LS5_TM_PQ_P55_GAPQ01-002_090_084_19920323/scene01/
--rw-r--r--   0 odc       (1001) odc        (121)   369213 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/lbg/LS5_TM_PQ_P55_GAPQ01-002_090_084_19920323/scene01/LS5_TM_PQ_P55_GAPQ01-002_090_084_19920323_1111111111111100.tif
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.654265 datacube-1.8.8rc1/tests/data/lbg/gedi/
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.654265 datacube-1.8.8rc1/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/
--rw-r--r--   0 odc       (1001) odc        (121)    39410 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/GEDI02_B_2019228092851_O03828_T04236_02_001_01_cover.xarray_3d
--rw-r--r--   0 odc       (1001) odc        (121)   195417 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/GEDI02_B_2019228092851_O03828_T04236_02_001_01_cover_z.xarray_3d
--rw-r--r--   0 odc       (1001) odc        (121)    39448 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/GEDI02_B_2019228092851_O03828_T04236_02_001_01_pai.xarray_3d
--rw-r--r--   0 odc       (1001) odc        (121)   195809 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/GEDI02_B_2019228092851_O03828_T04236_02_001_01_pai_z.xarray_3d
--rw-r--r--   0 odc       (1001) odc        (121)     2756 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/__GEDI02_B_2019228092851_O03828_T04236_02_001_01_gedi_l2b.yaml
--rw-r--r--   0 odc       (1001) odc        (121)      762 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/__GEDI02_B_2019228092851_O03828_T04236_02_001_01_gedi_l2b_cover_z.yaml
--rw-r--r--   0 odc       (1001) odc        (121)      756 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/__GEDI02_B_2019228092851_O03828_T04236_02_001_01_gedi_l2b_pai_z.yaml
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.654265 datacube-1.8.8rc1/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/
--rw-r--r--   0 odc       (1001) odc        (121)    46171 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/GEDI02_B_2019294155401_O04856_T03859_02_001_01_cover.xarray_3d
--rw-r--r--   0 odc       (1001) odc        (121)   327694 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/GEDI02_B_2019294155401_O04856_T03859_02_001_01_cover_z.xarray_3d
--rw-r--r--   0 odc       (1001) odc        (121)    46287 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/GEDI02_B_2019294155401_O04856_T03859_02_001_01_pai.xarray_3d
--rw-r--r--   0 odc       (1001) odc        (121)   328315 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/GEDI02_B_2019294155401_O04856_T03859_02_001_01_pai_z.xarray_3d
--rw-r--r--   0 odc       (1001) odc        (121)     2756 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/__GEDI02_B_2019294155401_O04856_T03859_02_001_01_gedi_l2b.yaml
--rw-r--r--   0 odc       (1001) odc        (121)      762 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/__GEDI02_B_2019294155401_O04856_T03859_02_001_01_gedi_l2b_cover_z.yaml
--rw-r--r--   0 odc       (1001) odc        (121)      756 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/__GEDI02_B_2019294155401_O04856_T03859_02_001_01_gedi_l2b_pai_z.yaml
--rw-r--r--   0 odc       (1001) odc        (121)     4513 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/lbg/gedi/GEDI02_B_3d_format.yaml
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.614264 datacube-1.8.8rc1/tests/data/ls8-eods-nbar/
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.614264 datacube-1.8.8rc1/tests/data/ls8-eods-nbar/data/
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.654265 datacube-1.8.8rc1/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/
--rw-r--r--   0 odc       (1001) odc        (121)     1012 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/md5sum.txt
--rw-r--r--   0 odc       (1001) odc        (121)     7946 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/metadata.xml
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.658266 datacube-1.8.8rc1/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/
--rw-r--r--   0 odc       (1001) odc        (121)      619 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B1.tif
--rw-r--r--   0 odc       (1001) odc        (121)      619 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B2.tif
--rw-r--r--   0 odc       (1001) odc        (121)      619 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B3.tif
--rw-r--r--   0 odc       (1001) odc        (121)      619 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B4.tif
--rw-r--r--   0 odc       (1001) odc        (121)      619 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B5.tif
--rw-r--r--   0 odc       (1001) odc        (121)      619 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B6.tif
--rw-r--r--   0 odc       (1001) odc        (121)      619 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B7.tif
--rw-r--r--   0 odc       (1001) odc        (121)     2056 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/report.txt
--rw-r--r--   0 odc       (1001) odc        (121)    20914 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/multi_doc.nc
--rw-r--r--   0 odc       (1001) odc        (121)      201 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/multi_doc.yml
--rw-r--r--   0 odc       (1001) odc        (121)      104 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/multi_doc.yml.gz
--rw-r--r--   0 odc       (1001) odc        (121)     6126 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/no_crs_ds.tif
--rw-r--r--   0 odc       (1001) odc        (121)      109 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/sample.json
--rw-r--r--   0 odc       (1001) odc        (121)   174104 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/sample_tile.nc
--rw-r--r--   0 odc       (1001) odc        (121)    32366 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/sample_tile_151_-29.tif
--rw-r--r--   0 odc       (1001) odc        (121)       84 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/single_doc.yaml
--rw-r--r--   0 odc       (1001) odc        (121)   174104 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/test.nc
--rw-r--r--   0 odc       (1001) odc        (121)   255072 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/test.tif
--rw-r--r--   0 odc       (1001) odc        (121)      170 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/data/zeros_no_geo_int16_7x3.tif
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.658266 datacube-1.8.8rc1/tests/drivers/
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.658266 datacube-1.8.8rc1/tests/drivers/fail_drivers/
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.658266 datacube-1.8.8rc1/tests/drivers/fail_drivers/dc_tests_io/
--rw-r--r--   0 odc       (1001) odc        (121)      176 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/drivers/fail_drivers/dc_tests_io/__init__.py
--rw-r--r--   0 odc       (1001) odc        (121)      282 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/drivers/fail_drivers/dc_tests_io/dummy.py
--rw-r--r--   0 odc       (1001) odc        (121)      689 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/drivers/fail_drivers/setup.py
--rw-r--r--   0 odc       (1001) odc        (121)     6659 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/drivers/test_rio_reader.py
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.658266 datacube-1.8.8rc1/tests/index/
--rw-r--r--   0 odc       (1001) odc        (121)      191 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/index/__init__.py
--rw-r--r--   0 odc       (1001) odc        (121)     9642 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/index/test_api_index_dataset.py
--rw-r--r--   0 odc       (1001) odc        (121)     3999 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/index/test_fields.py
--rw-r--r--   0 odc       (1001) odc        (121)      837 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/index/test_hl_index.py
--rw-r--r--   0 odc       (1001) odc        (121)     1046 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/index/test_query.py
--rw-r--r--   0 odc       (1001) odc        (121)     3077 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/index/test_validate_dataset_type.py
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.658266 datacube-1.8.8rc1/tests/scripts/
--rw-r--r--   0 odc       (1001) odc        (121)      191 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/scripts/__init__.py
--rw-r--r--   0 odc       (1001) odc        (121)     2078 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/scripts/test_search_tool.py
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.658266 datacube-1.8.8rc1/tests/storage/
--rw-r--r--   0 odc       (1001) odc        (121)     3099 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/storage/test_base.py
--rw-r--r--   0 odc       (1001) odc        (121)    14515 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/storage/test_netcdfwriter.py
--rw-r--r--   0 odc       (1001) odc        (121)    23952 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/storage/test_storage.py
--rw-r--r--   0 odc       (1001) odc        (121)     2341 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/storage/test_storage_load.py
--rw-r--r--   0 odc       (1001) odc        (121)    11767 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/storage/test_storage_read.py
--rw-r--r--   0 odc       (1001) odc        (121)     4353 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/test_3d.py
--rw-r--r--   0 odc       (1001) odc        (121)     2536 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/test_concurrent_executor.py
--rw-r--r--   0 odc       (1001) odc        (121)     8581 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/test_config.py
--rw-r--r--   0 odc       (1001) odc        (121)     3899 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/test_driver.py
--rw-r--r--   0 odc       (1001) odc        (121)     1038 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/test_dynamic_db_passwd.py
--rw-r--r--   0 odc       (1001) odc        (121)     7451 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/test_eo3.py
--rw-r--r--   0 odc       (1001) odc        (121)     5450 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/test_gbox_ops.py
--rw-r--r--   0 odc       (1001) odc        (121)    51557 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/test_geometry.py
--rw-r--r--   0 odc       (1001) odc        (121)    13380 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/test_load_data.py
--rw-r--r--   0 odc       (1001) odc        (121)     4966 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/test_metadata_fields.py
--rw-r--r--   0 odc       (1001) odc        (121)    13540 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/test_model.py
--rw-r--r--   0 odc       (1001) odc        (121)     3490 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/test_testutils.py
--rw-r--r--   0 odc       (1001) odc        (121)     9030 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/test_utils_aws.py
--rw-r--r--   0 odc       (1001) odc        (121)     3150 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/test_utils_changes.py
--rw-r--r--   0 odc       (1001) odc        (121)     6674 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/test_utils_cog.py
--rw-r--r--   0 odc       (1001) odc        (121)     6045 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/test_utils_dask.py
--rw-r--r--   0 odc       (1001) odc        (121)     2729 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/test_utils_dates.py
--rw-r--r--   0 odc       (1001) odc        (121)    20398 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/test_utils_docs.py
--rw-r--r--   0 odc       (1001) odc        (121)     1463 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/test_utils_generic.py
--rw-r--r--   0 odc       (1001) odc        (121)    23249 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/test_utils_other.py
--rw-r--r--   0 odc       (1001) odc        (121)     5752 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/test_utils_rio.py
--rw-r--r--   0 odc       (1001) odc        (121)     3833 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/test_warp.py
--rw-r--r--   0 odc       (1001) odc        (121)     6513 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/test_xarray_extension.py
-drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-09-29 03:02:56.658266 datacube-1.8.8rc1/tests/ui/
--rw-r--r--   0 odc       (1001) odc        (121)      176 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/ui/__init__.py
--rw-r--r--   0 odc       (1001) odc        (121)     3621 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/ui/test_common.py
--rw-r--r--   0 odc       (1001) odc        (121)     5271 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/ui/test_expression_parsing.py
--rw-r--r--   0 odc       (1001) odc        (121)     6337 2022-09-29 03:02:19.000000 datacube-1.8.8rc1/tests/ui/test_task_app.py
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.818910 datacube-1.8.9/
+-rw-r--r--   0 odc       (1001) odc        (121)      492 2022-11-17 00:47:28.000000 datacube-1.8.9/.coveragerc
+-rw-r--r--   0 odc       (1001) odc        (121)      983 2022-11-17 00:47:28.000000 datacube-1.8.9/.dockerignore
+-rw-r--r--   0 odc       (1001) odc        (121)     4472 2022-11-17 00:47:28.000000 datacube-1.8.9/.doctor-rst.yaml
+-rw-r--r--   0 odc       (1001) odc        (121)      487 2022-11-17 00:47:28.000000 datacube-1.8.9/.editorconfig
+-rw-r--r--   0 odc       (1001) odc        (121)      203 2022-11-17 00:47:28.000000 datacube-1.8.9/.gitattributes
+-rw-r--r--   0 odc       (1001) odc        (121)     1072 2022-11-17 00:47:28.000000 datacube-1.8.9/.gitignore
+-rw-r--r--   0 odc       (1001) odc        (121)      452 2022-11-17 00:47:28.000000 datacube-1.8.9/.mergify.yml
+-rw-r--r--   0 odc       (1001) odc        (121)      800 2022-11-17 00:47:28.000000 datacube-1.8.9/.pre-commit-config.yaml
+-rw-r--r--   0 odc       (1001) odc        (121)      919 2022-11-17 00:47:28.000000 datacube-1.8.9/.yamllint
+-rw-r--r--   0 odc       (1001) odc        (121)     1231 2022-11-17 00:47:28.000000 datacube-1.8.9/CONTRIBUTING.md
+-rw-r--r--   0 odc       (1001) odc        (121)    11357 2022-11-17 00:47:28.000000 datacube-1.8.9/LICENSE
+-rw-r--r--   0 odc       (1001) odc        (121)       70 2022-11-17 00:47:28.000000 datacube-1.8.9/MANIFEST.in
+-rw-rw-r--   0 odc       (1001) odc        (121)     5286 2022-11-17 00:48:13.818910 datacube-1.8.9/PKG-INFO
+-rw-r--r--   0 odc       (1001) odc        (121)     3887 2022-11-17 00:47:28.000000 datacube-1.8.9/README.rst
+-rwxr-xr-x   0 odc       (1001) odc        (121)      980 2022-11-17 00:47:28.000000 datacube-1.8.9/check-code.sh
+-rw-r--r--   0 odc       (1001) odc        (121)     3507 2022-11-17 00:47:28.000000 datacube-1.8.9/code-of-conduct.md
+-rw-r--r--   0 odc       (1001) odc        (121)      503 2022-11-17 00:47:28.000000 datacube-1.8.9/conda-environment.yml
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.738910 datacube-1.8.9/datacube/
+-rw-r--r--   0 odc       (1001) odc        (121)     1128 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (121)      257 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/__main__.py
+-rw-rw-r--   0 odc       (1001) odc        (121)      176 2022-11-17 00:48:13.000000 datacube-1.8.9/datacube/_version.py
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.742910 datacube-1.8.9/datacube/api/
+-rw-r--r--   0 odc       (1001) odc        (121)      416 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/api/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (121)    44022 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/api/core.py
+-rw-r--r--   0 odc       (1001) odc        (121)    16365 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/api/grid_workflow.py
+-rw-r--r--   0 odc       (1001) odc        (121)    14909 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/api/query.py
+-rwxr-xr-x   0 odc       (1001) odc        (121)     9494 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/config.py
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.742910 datacube-1.8.9/datacube/drivers/
+-rw-r--r--   0 odc       (1001) odc        (121)      587 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/drivers/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (121)     1065 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/drivers/_tools.py
+-rw-r--r--   0 odc       (1001) odc        (121)     2938 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/drivers/_types.py
+-rw-r--r--   0 odc       (1001) odc        (121)     1739 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/drivers/datasource.py
+-rw-r--r--   0 odc       (1001) odc        (121)     2057 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/drivers/driver_cache.py
+-rw-r--r--   0 odc       (1001) odc        (121)     1822 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/drivers/indexes.py
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.742910 datacube-1.8.9/datacube/drivers/netcdf/
+-rw-r--r--   0 odc       (1001) odc        (121)      432 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/drivers/netcdf/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (121)     3014 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/drivers/netcdf/_safestrings.py
+-rw-r--r--   0 odc       (1001) odc        (121)     4868 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/drivers/netcdf/_write.py
+-rw-r--r--   0 odc       (1001) odc        (121)     2571 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/drivers/netcdf/driver.py
+-rw-r--r--   0 odc       (1001) odc        (121)    11299 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/drivers/netcdf/writer.py
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.746910 datacube-1.8.9/datacube/drivers/postgis/
+-rw-r--r--   0 odc       (1001) odc        (121)      396 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/drivers/postgis/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (121)    37818 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/drivers/postgis/_api.py
+-rwxr-xr-x   0 odc       (1001) odc        (121)    11346 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/drivers/postgis/_connections.py
+-rw-r--r--   0 odc       (1001) odc        (121)     8756 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/drivers/postgis/_core.py
+-rw-r--r--   0 odc       (1001) odc        (121)     6997 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/drivers/postgis/_dynamic.py
+-rwxr-xr-x   0 odc       (1001) odc        (121)    19069 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/drivers/postgis/_fields.py
+-rw-r--r--   0 odc       (1001) odc        (121)     9130 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/drivers/postgis/_schema.py
+-rw-r--r--   0 odc       (1001) odc        (121)     6172 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/drivers/postgis/_spatial.py
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.746910 datacube-1.8.9/datacube/drivers/postgis/samples/
+-rw-r--r--   0 odc       (1001) odc        (121)     4023 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/drivers/postgis/samples/range-tests-explicit.sql
+-rw-r--r--   0 odc       (1001) odc        (121)     2229 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/drivers/postgis/samples/range-tests-scalar.sql
+-rw-r--r--   0 odc       (1001) odc        (121)     2687 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/drivers/postgis/samples/range-tests-view.sql
+-rw-r--r--   0 odc       (1001) odc        (121)     4299 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/drivers/postgis/sql.py
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.746910 datacube-1.8.9/datacube/drivers/postgres/
+-rw-r--r--   0 odc       (1001) odc        (121)      400 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/drivers/postgres/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (121)    38831 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/drivers/postgres/_api.py
+-rwxr-xr-x   0 odc       (1001) odc        (121)     9981 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/drivers/postgres/_connections.py
+-rw-r--r--   0 odc       (1001) odc        (121)     9488 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/drivers/postgres/_core.py
+-rw-r--r--   0 odc       (1001) odc        (121)     6346 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/drivers/postgres/_dynamic.py
+-rwxr-xr-x   0 odc       (1001) odc        (121)    19071 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/drivers/postgres/_fields.py
+-rw-r--r--   0 odc       (1001) odc        (121)     6455 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/drivers/postgres/_schema.py
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.750910 datacube-1.8.9/datacube/drivers/postgres/samples/
+-rw-r--r--   0 odc       (1001) odc        (121)     4029 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/drivers/postgres/samples/range-tests-explicit.sql
+-rw-r--r--   0 odc       (1001) odc        (121)     2235 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/drivers/postgres/samples/range-tests-scalar.sql
+-rw-r--r--   0 odc       (1001) odc        (121)     2692 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/drivers/postgres/samples/range-tests-view.sql
+-rw-r--r--   0 odc       (1001) odc        (121)     4302 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/drivers/postgres/sql.py
+-rw-r--r--   0 odc       (1001) odc        (121)     3533 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/drivers/readers.py
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.750910 datacube-1.8.9/datacube/drivers/rio/
+-rw-r--r--   0 odc       (1001) odc        (121)      206 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/drivers/rio/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (121)     7109 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/drivers/rio/_reader.py
+-rw-r--r--   0 odc       (1001) odc        (121)     1538 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/drivers/writers.py
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.750910 datacube-1.8.9/datacube/execution/
+-rw-r--r--   0 odc       (1001) odc        (121)      176 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/execution/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (121)     1893 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/execution/worker.py
+-rw-r--r--   0 odc       (1001) odc        (121)     7203 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/executor.py
+-rw-r--r--   0 odc       (1001) odc        (121)     1597 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/helpers.py
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.750910 datacube-1.8.9/datacube/index/
+-rw-r--r--   0 odc       (1001) odc        (121)      597 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/index/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (121)     1702 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/index/_api.py
+-rw-r--r--   0 odc       (1001) odc        (121)    47218 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/index/abstract.py
+-rw-r--r--   0 odc       (1001) odc        (121)    10618 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/index/default-metadata-types.yaml
+-rw-r--r--   0 odc       (1001) odc        (121)     8192 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/index/eo3.py
+-rw-r--r--   0 odc       (1001) odc        (121)      500 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/index/exceptions.py
+-rw-r--r--   0 odc       (1001) odc        (121)     2272 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/index/fields.py
+-rw-r--r--   0 odc       (1001) odc        (121)    12373 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/index/hl.py
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.754910 datacube-1.8.9/datacube/index/memory/
+-rw-r--r--   0 odc       (1001) odc        (121)      191 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/index/memory/__init__.py
+-rwxr-xr-x   0 odc       (1001) odc        (121)    30858 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/index/memory/_datasets.py
+-rw-r--r--   0 odc       (1001) odc        (121)     1709 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/index/memory/_fields.py
+-rw-r--r--   0 odc       (1001) odc        (121)     5382 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/index/memory/_metadata_types.py
+-rw-r--r--   0 odc       (1001) odc        (121)     7705 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/index/memory/_products.py
+-rw-r--r--   0 odc       (1001) odc        (121)     2462 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/index/memory/_users.py
+-rw-r--r--   0 odc       (1001) odc        (121)     3020 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/index/memory/index.py
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.754910 datacube-1.8.9/datacube/index/null/
+-rw-r--r--   0 odc       (1001) odc        (121)      191 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/index/null/__init__.py
+-rwxr-xr-x   0 odc       (1001) odc        (121)     2986 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/index/null/_datasets.py
+-rw-r--r--   0 odc       (1001) odc        (121)     1123 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/index/null/_metadata_types.py
+-rw-r--r--   0 odc       (1001) odc        (121)     1178 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/index/null/_products.py
+-rw-r--r--   0 odc       (1001) odc        (121)      802 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/index/null/_users.py
+-rw-r--r--   0 odc       (1001) odc        (121)     2877 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/index/null/index.py
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.754910 datacube-1.8.9/datacube/index/postgis/
+-rw-r--r--   0 odc       (1001) odc        (121)        0 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/index/postgis/__init__.py
+-rwxr-xr-x   0 odc       (1001) odc        (121)    35589 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/index/postgis/_datasets.py
+-rw-r--r--   0 odc       (1001) odc        (121)     9471 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/index/postgis/_metadata_types.py
+-rw-r--r--   0 odc       (1001) odc        (121)    13586 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/index/postgis/_products.py
+-rw-r--r--   0 odc       (1001) odc        (121)     2405 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/index/postgis/_transaction.py
+-rw-r--r--   0 odc       (1001) odc        (121)     1819 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/index/postgis/_users.py
+-rw-r--r--   0 odc       (1001) odc        (121)     8239 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/index/postgis/index.py
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.758910 datacube-1.8.9/datacube/index/postgres/
+-rw-r--r--   0 odc       (1001) odc        (121)        0 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/index/postgres/__init__.py
+-rwxr-xr-x   0 odc       (1001) odc        (121)    35174 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/index/postgres/_datasets.py
+-rw-r--r--   0 odc       (1001) odc        (121)     9611 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/index/postgres/_metadata_types.py
+-rw-r--r--   0 odc       (1001) odc        (121)    13856 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/index/postgres/_products.py
+-rw-r--r--   0 odc       (1001) odc        (121)     2403 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/index/postgres/_transaction.py
+-rw-r--r--   0 odc       (1001) odc        (121)     1839 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/index/postgres/_users.py
+-rw-r--r--   0 odc       (1001) odc        (121)     6838 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/index/postgres/index.py
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.758910 datacube-1.8.9/datacube/model/
+-rw-r--r--   0 odc       (1001) odc        (121)    38428 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/model/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (121)      593 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/model/_base.py
+-rw-r--r--   0 odc       (1001) odc        (121)     5933 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/model/fields.py
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.758910 datacube-1.8.9/datacube/model/schema/
+-rw-r--r--   0 odc       (1001) odc        (121)     5564 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/model/schema/dataset-type-schema.yaml
+-rw-r--r--   0 odc       (1001) odc        (121)     4681 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/model/schema/ingestor-config-type-schema.yaml
+-rw-r--r--   0 odc       (1001) odc        (121)     2061 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/model/schema/metadata-type-schema.yaml
+-rw-r--r--   0 odc       (1001) odc        (121)    14179 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/model/utils.py
+-rw-r--r--   0 odc       (1001) odc        (121)        0 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/py.typed
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.762910 datacube-1.8.9/datacube/scripts/
+-rw-r--r--   0 odc       (1001) odc        (121)      176 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/scripts/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (121)      596 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/scripts/cli_app.py
+-rw-r--r--   0 odc       (1001) odc        (121)    24391 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/scripts/dataset.py
+-rw-r--r--   0 odc       (1001) odc        (121)    17593 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/scripts/ingest.py
+-rw-r--r--   0 odc       (1001) odc        (121)     6010 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/scripts/metadata.py
+-rw-r--r--   0 odc       (1001) odc        (121)     9017 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/scripts/product.py
+-rwxr-xr-x   0 odc       (1001) odc        (121)     3842 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/scripts/search_tool.py
+-rw-r--r--   0 odc       (1001) odc        (121)     3349 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/scripts/system.py
+-rw-r--r--   0 odc       (1001) odc        (121)     3268 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/scripts/user.py
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.762910 datacube-1.8.9/datacube/storage/
+-rw-r--r--   0 odc       (1001) odc        (121)      594 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/storage/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (121)     3677 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/storage/_base.py
+-rw-r--r--   0 odc       (1001) odc        (121)      224 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/storage/_hdf5.py
+-rw-r--r--   0 odc       (1001) odc        (121)     6150 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/storage/_load.py
+-rw-r--r--   0 odc       (1001) odc        (121)     8212 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/storage/_read.py
+-rw-r--r--   0 odc       (1001) odc        (121)     7585 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/storage/_rio.py
+-rw-r--r--   0 odc       (1001) odc        (121)      372 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/storage/masking.py
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.766910 datacube-1.8.9/datacube/testutils/
+-rw-r--r--   0 odc       (1001) odc        (121)    14223 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/testutils/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (121)     5003 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/testutils/geom.py
+-rw-r--r--   0 odc       (1001) odc        (121)    11871 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/testutils/io.py
+-rw-r--r--   0 odc       (1001) odc        (121)     2139 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/testutils/iodriver.py
+-rw-r--r--   0 odc       (1001) odc        (121)      797 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/testutils/threads.py
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.766910 datacube-1.8.9/datacube/ui/
+-rw-r--r--   0 odc       (1001) odc        (121)      418 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/ui/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (121)    11874 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/ui/click.py
+-rw-r--r--   0 odc       (1001) odc        (121)     4191 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/ui/common.py
+-rw-r--r--   0 odc       (1001) odc        (121)     3786 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/ui/expression.py
+-rw-r--r--   0 odc       (1001) odc        (121)    10704 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/ui/task_app.py
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.770910 datacube-1.8.9/datacube/utils/
+-rw-r--r--   0 odc       (1001) odc        (121)     1956 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/utils/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (121)      502 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/utils/_misc.py
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.770910 datacube-1.8.9/datacube/utils/aws/
+-rw-r--r--   0 odc       (1001) odc        (121)    17300 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/utils/aws/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (121)     6581 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/utils/changes.py
+-rw-r--r--   0 odc       (1001) odc        (121)    14314 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/utils/cog.py
+-rw-r--r--   0 odc       (1001) odc        (121)    11374 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/utils/dask.py
+-rw-r--r--   0 odc       (1001) odc        (121)     4425 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/utils/dates.py
+-rw-r--r--   0 odc       (1001) odc        (121)    16178 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/utils/documents.py
+-rw-r--r--   0 odc       (1001) odc        (121)     2761 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/utils/generic.py
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.770910 datacube-1.8.9/datacube/utils/geometry/
+-rw-r--r--   0 odc       (1001) odc        (121)     2645 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/utils/geometry/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (121)    47662 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/utils/geometry/_base.py
+-rw-r--r--   0 odc       (1001) odc        (121)     5948 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/utils/geometry/_warp.py
+-rw-r--r--   0 odc       (1001) odc        (121)     7772 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/utils/geometry/gbox.py
+-rw-r--r--   0 odc       (1001) odc        (121)    18117 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/utils/geometry/tools.py
+-rw-r--r--   0 odc       (1001) odc        (121)     2293 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/utils/io.py
+-rw-r--r--   0 odc       (1001) odc        (121)     8989 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/utils/masking.py
+-rw-r--r--   0 odc       (1001) odc        (121)     8600 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/utils/math.py
+-rw-r--r--   0 odc       (1001) odc        (121)     2225 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/utils/py.py
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.770910 datacube-1.8.9/datacube/utils/rio/
+-rw-r--r--   0 odc       (1001) odc        (121)      648 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/utils/rio/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (121)     5105 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/utils/rio/_rio.py
+-rw-r--r--   0 odc       (1001) odc        (121)     2336 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/utils/serialise.py
+-rw-r--r--   0 odc       (1001) odc        (121)     6442 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/utils/uris.py
+-rw-r--r--   0 odc       (1001) odc        (121)     5777 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/utils/xarray_geoextensions.py
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.774910 datacube-1.8.9/datacube/virtual/
+-rw-r--r--   0 odc       (1001) odc        (121)     7775 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/virtual/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (121)     2368 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/virtual/catalog.py
+-rw-r--r--   0 odc       (1001) odc        (121)     4712 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/virtual/expr.py
+-rw-r--r--   0 odc       (1001) odc        (121)    40209 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/virtual/impl.py
+-rw-r--r--   0 odc       (1001) odc        (121)    16795 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/virtual/transformations.py
+-rw-r--r--   0 odc       (1001) odc        (121)     1634 2022-11-17 00:47:28.000000 datacube-1.8.9/datacube/virtual/utils.py
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.738910 datacube-1.8.9/datacube.egg-info/
+-rw-rw-r--   0 odc       (1001) odc        (121)     5286 2022-11-17 00:48:13.000000 datacube-1.8.9/datacube.egg-info/PKG-INFO
+-rw-rw-r--   0 odc       (1001) odc        (121)    14049 2022-11-17 00:48:13.000000 datacube-1.8.9/datacube.egg-info/SOURCES.txt
+-rw-rw-r--   0 odc       (1001) odc        (121)        1 2022-11-17 00:48:13.000000 datacube-1.8.9/datacube.egg-info/dependency_links.txt
+-rw-rw-r--   0 odc       (1001) odc        (121)      581 2022-11-17 00:48:13.000000 datacube-1.8.9/datacube.egg-info/entry_points.txt
+-rw-rw-r--   0 odc       (1001) odc        (121)     1131 2022-11-17 00:48:13.000000 datacube-1.8.9/datacube.egg-info/requires.txt
+-rw-rw-r--   0 odc       (1001) odc        (121)        9 2022-11-17 00:48:13.000000 datacube-1.8.9/datacube.egg-info/top_level.txt
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.726910 datacube-1.8.9/examples/
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.774910 datacube-1.8.9/examples/io_plugin/
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.774910 datacube-1.8.9/examples/io_plugin/dcio_example/
+-rw-r--r--   0 odc       (1001) odc        (121)      176 2022-11-17 00:47:28.000000 datacube-1.8.9/examples/io_plugin/dcio_example/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (121)     3855 2022-11-17 00:47:28.000000 datacube-1.8.9/examples/io_plugin/dcio_example/pickles.py
+-rw-r--r--   0 odc       (1001) odc        (121)     5961 2022-11-17 00:47:28.000000 datacube-1.8.9/examples/io_plugin/dcio_example/xarray_3d.py
+-rw-r--r--   0 odc       (1001) odc        (121)      607 2022-11-17 00:47:28.000000 datacube-1.8.9/examples/io_plugin/dcio_example/zeros.py
+-rw-r--r--   0 odc       (1001) odc        (121)      747 2022-11-17 00:47:28.000000 datacube-1.8.9/examples/io_plugin/setup.py
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.778910 datacube-1.8.9/integration_tests/
+-rw-r--r--   0 odc       (1001) odc        (121)      191 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (121)      276 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/agdcintegration.conf
+-rw-r--r--   0 odc       (1001) odc        (121)      366 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/ancillary-collection.yaml
+-rw-r--r--   0 odc       (1001) odc        (121)    21327 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/conftest.py
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.726910 datacube-1.8.9/integration_tests/data/
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.782910 datacube-1.8.9/integration_tests/data/dataset_add/
+-rw-r--r--   0 odc       (1001) odc        (121)     3112 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/data/dataset_add/datasets.yml
+-rw-r--r--   0 odc       (1001) odc        (121)     1624 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/data/dataset_add/datasets_bad1.yml
+-rw-r--r--   0 odc       (1001) odc        (121)     1010 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/data/dataset_add/datasets_eo3.yml
+-rw-r--r--   0 odc       (1001) odc        (121)      243 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/data/dataset_add/datasets_no_id.yml
+-rw-r--r--   0 odc       (1001) odc        (121)        0 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/data/dataset_add/empty_file.yml
+-rw-r--r--   0 odc       (1001) odc        (121)     1664 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/data/dataset_add/metadata.yml
+-rw-r--r--   0 odc       (1001) odc        (121)      820 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/data/dataset_add/products.yml
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.782910 datacube-1.8.9/integration_tests/data/eo3/
+-rw-r--r--   0 odc       (1001) odc        (121)     3527 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/data/eo3/ard_ls8.odc-product.yaml
+-rw-r--r--   0 odc       (1001) odc        (121)     7591 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/data/eo3/eo3_landsat_ard.odc-type.yaml
+-rw-r--r--   0 odc       (1001) odc        (121)     1473 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/data/eo3/ga_ls_wo_3.odc-product.yaml
+-rw-r--r--   0 odc       (1001) odc        (121)     4793 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/data/eo3/ls8_dataset.yaml
+-rw-r--r--   0 odc       (1001) odc        (121)     4725 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/data/eo3/ls8_dataset2.yaml
+-rw-r--r--   0 odc       (1001) odc        (121)     5271 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/data/eo3/ls8_dataset3.yaml
+-rw-r--r--   0 odc       (1001) odc        (121)     5265 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/data/eo3/ls8_dataset4.yaml
+-rw-r--r--   0 odc       (1001) odc        (121)     2823 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/data/eo3/s2_africa_dataset.yaml
+-rw-r--r--   0 odc       (1001) odc        (121)     2210 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/data/eo3/s2_africa_product.yaml
+-rw-r--r--   0 odc       (1001) odc        (121)     3165 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/data/eo3/wo_dataset.yaml
+-rw-r--r--   0 odc       (1001) odc        (121)     8572 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/data/eo3/wo_ds_with_lineage.odc-metadata.yaml
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.786910 datacube-1.8.9/integration_tests/data/ingester/
+-rw-r--r--   0 odc       (1001) odc        (121)     4787 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/data/ingester/invalid_config.yaml
+-rw-r--r--   0 odc       (1001) odc        (121)     4810 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/data/ingester/invalid_src_name.yaml
+-rw-r--r--   0 odc       (1001) odc        (121)     6554 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/data_utils.py
+-rw-r--r--   0 odc       (1001) odc        (121)     8099 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/example-ls5-nbar.yaml
+-rw-r--r--   0 odc       (1001) odc        (121)     2136 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/example-ls5-nbar_302.yaml
+-rw-r--r--   0 odc       (1001) odc        (121)     2135 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/example-ls5-nbar_505.yaml
+-rw-r--r--   0 odc       (1001) odc        (121)     2130 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/example-ls5-nbar_606.yaml
+-rw-r--r--   0 odc       (1001) odc        (121)     3084 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/extensive-eo-metadata.yaml
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.790910 datacube-1.8.9/integration_tests/index/
+-rw-r--r--   0 odc       (1001) odc        (121)      191 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/index/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (121)     1580 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/index/search_utils.py
+-rw-r--r--   0 odc       (1001) odc        (121)    23466 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/index/test_config_docs.py
+-rwxr-xr-x   0 odc       (1001) odc        (121)    21199 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/index/test_index_data.py
+-rw-r--r--   0 odc       (1001) odc        (121)    25099 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/index/test_memory_index.py
+-rw-r--r--   0 odc       (1001) odc        (121)     6653 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/index/test_null_index.py
+-rw-r--r--   0 odc       (1001) odc        (121)      863 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/index/test_pluggable_indexes.py
+-rw-r--r--   0 odc       (1001) odc        (121)     8471 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/index/test_postgis_index.py
+-rw-r--r--   0 odc       (1001) odc        (121)    29080 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/index/test_search_eo3.py
+-rw-r--r--   0 odc       (1001) odc        (121)    37077 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/index/test_search_legacy.py
+-rw-r--r--   0 odc       (1001) odc        (121)     4046 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/index/test_update_columns.py
+-rw-r--r--   0 odc       (1001) odc        (121)    16931 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/test_3d.py
+-rw-r--r--   0 odc       (1001) odc        (121)     6568 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/test_cli_output.py
+-rw-r--r--   0 odc       (1001) odc        (121)     9298 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/test_config_tool.py
+-rw-r--r--   0 odc       (1001) odc        (121)    22762 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/test_dataset_add.py
+-rw-r--r--   0 odc       (1001) odc        (121)     3210 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/test_double_ingestion.py
+-rw-r--r--   0 odc       (1001) odc        (121)    12134 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/test_end_to_end.py
+-rw-r--r--   0 odc       (1001) odc        (121)     2369 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/test_environments.py
+-rw-r--r--   0 odc       (1001) odc        (121)    10516 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/test_full_ingestion.py
+-rw-r--r--   0 odc       (1001) odc        (121)     6570 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/test_index_datasets_search.py
+-rw-r--r--   0 odc       (1001) odc        (121)     3712 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/test_index_out_of_bound.py
+-rw-r--r--   0 odc       (1001) odc        (121)     1654 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/test_model.py
+-rw-r--r--   0 odc       (1001) odc        (121)     1318 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/test_validate_ingestion.py
+-rw-r--r--   0 odc       (1001) odc        (121)     7856 2022-11-17 00:47:28.000000 datacube-1.8.9/integration_tests/utils.py
+-rw-r--r--   0 odc       (1001) odc        (121)     1115 2022-11-17 00:47:28.000000 datacube-1.8.9/license-headers.md
+-rw-r--r--   0 odc       (1001) odc        (121)      168 2022-11-17 00:47:28.000000 datacube-1.8.9/license-template.txt
+-rw-r--r--   0 odc       (1001) odc        (121)       84 2022-11-17 00:47:28.000000 datacube-1.8.9/mypy.ini
+-rw-r--r--   0 odc       (1001) odc        (121)     7160 2022-11-17 00:47:28.000000 datacube-1.8.9/pylintrc
+-rw-r--r--   0 odc       (1001) odc        (121)      157 2022-11-17 00:47:28.000000 datacube-1.8.9/pyproject.toml
+-rw-r--r--   0 odc       (1001) odc        (121)      161 2022-11-17 00:47:28.000000 datacube-1.8.9/pytest.ini
+-rw-r--r--   0 odc       (1001) odc        (121)      190 2022-11-17 00:47:28.000000 datacube-1.8.9/readthedocs.yml
+-rw-r--r--   0 odc       (1001) odc        (121)      235 2022-11-17 00:48:13.818910 datacube-1.8.9/setup.cfg
+-rwxr-xr-x   0 odc       (1001) odc        (121)     4162 2022-11-17 00:47:28.000000 datacube-1.8.9/setup.py
+-rw-r--r--   0 odc       (1001) odc        (121)      357 2022-11-17 00:47:28.000000 datacube-1.8.9/spellcheck.yaml
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.794910 datacube-1.8.9/tests/
+-rw-r--r--   0 odc       (1001) odc        (121)      176 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/__init__.py
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.794910 datacube-1.8.9/tests/api/
+-rw-r--r--   0 odc       (1001) odc        (121)      176 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/api/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (121)     4023 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/api/test_core.py
+-rw-r--r--   0 odc       (1001) odc        (121)     9416 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/api/test_grid_workflow.py
+-rw-r--r--   0 odc       (1001) odc        (121)    13832 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/api/test_masking.py
+-rw-r--r--   0 odc       (1001) odc        (121)     8412 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/api/test_query.py
+-rw-r--r--   0 odc       (1001) odc        (121)    21799 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/api/test_virtual.py
+-rw-r--r--   0 odc       (1001) odc        (121)    10302 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/conftest.py
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.798910 datacube-1.8.9/tests/data/
+-rw-r--r--   0 odc       (1001) odc        (121)     8099 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/ds_eo.yaml
+-rw-r--r--   0 odc       (1001) odc        (121)      520 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/ds_eo3.yml
+-rw-r--r--   0 odc       (1001) odc        (121)      432 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/ds_non-geo.yaml
+-rw-r--r--   0 odc       (1001) odc        (121)     2516 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/eo3.yaml
+-rw-r--r--   0 odc       (1001) odc        (121)      471 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/ingest_config.yaml
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.726910 datacube-1.8.9/tests/data/lbg/
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.798910 datacube-1.8.9/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/
+-rw-r--r--   0 odc       (1001) odc        (121)     2266 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/agdc-metadata.yaml
+-rw-r--r--   0 odc       (1001) odc        (121)    10247 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/metadata.xml
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.802910 datacube-1.8.9/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/
+-rw-r--r--   0 odc       (1001) odc        (121)   369231 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B10.tif
+-rw-r--r--   0 odc       (1001) odc        (121)   369231 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B20.tif
+-rw-r--r--   0 odc       (1001) odc        (121)   369231 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B30.tif
+-rw-r--r--   0 odc       (1001) odc        (121)   369231 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B40.tif
+-rw-r--r--   0 odc       (1001) odc        (121)   369231 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B50.tif
+-rw-r--r--   0 odc       (1001) odc        (121)   369231 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B70.tif
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.806910 datacube-1.8.9/tests/data/lbg/LS5_TM_PQ_P55_GAPQ01-002_090_084_19920323/
+-rw-r--r--   0 odc       (1001) odc        (121)     4590 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/lbg/LS5_TM_PQ_P55_GAPQ01-002_090_084_19920323/agdc-metadata.yaml
+-rw-r--r--   0 odc       (1001) odc        (121)     8550 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/lbg/LS5_TM_PQ_P55_GAPQ01-002_090_084_19920323/metadata.xml
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.806910 datacube-1.8.9/tests/data/lbg/LS5_TM_PQ_P55_GAPQ01-002_090_084_19920323/scene01/
+-rw-r--r--   0 odc       (1001) odc        (121)   369213 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/lbg/LS5_TM_PQ_P55_GAPQ01-002_090_084_19920323/scene01/LS5_TM_PQ_P55_GAPQ01-002_090_084_19920323_1111111111111100.tif
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.806910 datacube-1.8.9/tests/data/lbg/gedi/
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.810910 datacube-1.8.9/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/
+-rw-r--r--   0 odc       (1001) odc        (121)    39410 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/GEDI02_B_2019228092851_O03828_T04236_02_001_01_cover.xarray_3d
+-rw-r--r--   0 odc       (1001) odc        (121)   195417 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/GEDI02_B_2019228092851_O03828_T04236_02_001_01_cover_z.xarray_3d
+-rw-r--r--   0 odc       (1001) odc        (121)    39448 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/GEDI02_B_2019228092851_O03828_T04236_02_001_01_pai.xarray_3d
+-rw-r--r--   0 odc       (1001) odc        (121)   195809 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/GEDI02_B_2019228092851_O03828_T04236_02_001_01_pai_z.xarray_3d
+-rw-r--r--   0 odc       (1001) odc        (121)     2756 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/__GEDI02_B_2019228092851_O03828_T04236_02_001_01_gedi_l2b.yaml
+-rw-r--r--   0 odc       (1001) odc        (121)      762 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/__GEDI02_B_2019228092851_O03828_T04236_02_001_01_gedi_l2b_cover_z.yaml
+-rw-r--r--   0 odc       (1001) odc        (121)      756 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/__GEDI02_B_2019228092851_O03828_T04236_02_001_01_gedi_l2b_pai_z.yaml
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.814910 datacube-1.8.9/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/
+-rw-r--r--   0 odc       (1001) odc        (121)    46171 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/GEDI02_B_2019294155401_O04856_T03859_02_001_01_cover.xarray_3d
+-rw-r--r--   0 odc       (1001) odc        (121)   327694 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/GEDI02_B_2019294155401_O04856_T03859_02_001_01_cover_z.xarray_3d
+-rw-r--r--   0 odc       (1001) odc        (121)    46287 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/GEDI02_B_2019294155401_O04856_T03859_02_001_01_pai.xarray_3d
+-rw-r--r--   0 odc       (1001) odc        (121)   328315 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/GEDI02_B_2019294155401_O04856_T03859_02_001_01_pai_z.xarray_3d
+-rw-r--r--   0 odc       (1001) odc        (121)     2756 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/__GEDI02_B_2019294155401_O04856_T03859_02_001_01_gedi_l2b.yaml
+-rw-r--r--   0 odc       (1001) odc        (121)      762 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/__GEDI02_B_2019294155401_O04856_T03859_02_001_01_gedi_l2b_cover_z.yaml
+-rw-r--r--   0 odc       (1001) odc        (121)      756 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/__GEDI02_B_2019294155401_O04856_T03859_02_001_01_gedi_l2b_pai_z.yaml
+-rw-r--r--   0 odc       (1001) odc        (121)     4513 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/lbg/gedi/GEDI02_B_3d_format.yaml
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.730910 datacube-1.8.9/tests/data/ls8-eods-nbar/
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.730910 datacube-1.8.9/tests/data/ls8-eods-nbar/data/
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.814910 datacube-1.8.9/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/
+-rw-r--r--   0 odc       (1001) odc        (121)     1012 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/md5sum.txt
+-rw-r--r--   0 odc       (1001) odc        (121)     7946 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/metadata.xml
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.814910 datacube-1.8.9/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/
+-rw-r--r--   0 odc       (1001) odc        (121)      619 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B1.tif
+-rw-r--r--   0 odc       (1001) odc        (121)      619 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B2.tif
+-rw-r--r--   0 odc       (1001) odc        (121)      619 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B3.tif
+-rw-r--r--   0 odc       (1001) odc        (121)      619 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B4.tif
+-rw-r--r--   0 odc       (1001) odc        (121)      619 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B5.tif
+-rw-r--r--   0 odc       (1001) odc        (121)      619 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B6.tif
+-rw-r--r--   0 odc       (1001) odc        (121)      619 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B7.tif
+-rw-r--r--   0 odc       (1001) odc        (121)     2055 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/report.txt
+-rw-r--r--   0 odc       (1001) odc        (121)    20914 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/multi_doc.nc
+-rw-r--r--   0 odc       (1001) odc        (121)      201 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/multi_doc.yml
+-rw-r--r--   0 odc       (1001) odc        (121)      104 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/multi_doc.yml.gz
+-rw-r--r--   0 odc       (1001) odc        (121)     6126 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/no_crs_ds.tif
+-rw-r--r--   0 odc       (1001) odc        (121)      109 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/sample.json
+-rw-r--r--   0 odc       (1001) odc        (121)   174104 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/sample_tile.nc
+-rw-r--r--   0 odc       (1001) odc        (121)    32366 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/sample_tile_151_-29.tif
+-rw-r--r--   0 odc       (1001) odc        (121)       84 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/single_doc.yaml
+-rw-r--r--   0 odc       (1001) odc        (121)   174104 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/test.nc
+-rw-r--r--   0 odc       (1001) odc        (121)   255072 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/test.tif
+-rw-r--r--   0 odc       (1001) odc        (121)      170 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/data/zeros_no_geo_int16_7x3.tif
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.814910 datacube-1.8.9/tests/drivers/
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.814910 datacube-1.8.9/tests/drivers/fail_drivers/
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.814910 datacube-1.8.9/tests/drivers/fail_drivers/dc_tests_io/
+-rw-r--r--   0 odc       (1001) odc        (121)      176 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/drivers/fail_drivers/dc_tests_io/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (121)      282 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/drivers/fail_drivers/dc_tests_io/dummy.py
+-rw-r--r--   0 odc       (1001) odc        (121)      689 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/drivers/fail_drivers/setup.py
+-rw-r--r--   0 odc       (1001) odc        (121)     6659 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/drivers/test_rio_reader.py
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.814910 datacube-1.8.9/tests/index/
+-rw-r--r--   0 odc       (1001) odc        (121)      191 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/index/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (121)     9642 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/index/test_api_index_dataset.py
+-rw-r--r--   0 odc       (1001) odc        (121)     3999 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/index/test_fields.py
+-rw-r--r--   0 odc       (1001) odc        (121)      837 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/index/test_hl_index.py
+-rw-r--r--   0 odc       (1001) odc        (121)     1046 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/index/test_query.py
+-rw-r--r--   0 odc       (1001) odc        (121)     3077 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/index/test_validate_dataset_type.py
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.814910 datacube-1.8.9/tests/scripts/
+-rw-r--r--   0 odc       (1001) odc        (121)      191 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/scripts/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (121)     2078 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/scripts/test_search_tool.py
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.818910 datacube-1.8.9/tests/storage/
+-rw-r--r--   0 odc       (1001) odc        (121)     3099 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/storage/test_base.py
+-rw-r--r--   0 odc       (1001) odc        (121)    14515 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/storage/test_netcdfwriter.py
+-rw-r--r--   0 odc       (1001) odc        (121)    23952 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/storage/test_storage.py
+-rw-r--r--   0 odc       (1001) odc        (121)     2341 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/storage/test_storage_load.py
+-rw-r--r--   0 odc       (1001) odc        (121)    11767 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/storage/test_storage_read.py
+-rw-r--r--   0 odc       (1001) odc        (121)     4353 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/test_3d.py
+-rw-r--r--   0 odc       (1001) odc        (121)     2536 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/test_concurrent_executor.py
+-rw-r--r--   0 odc       (1001) odc        (121)     8581 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/test_config.py
+-rw-r--r--   0 odc       (1001) odc        (121)     3899 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/test_driver.py
+-rw-r--r--   0 odc       (1001) odc        (121)     1038 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/test_dynamic_db_passwd.py
+-rw-r--r--   0 odc       (1001) odc        (121)     7451 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/test_eo3.py
+-rw-r--r--   0 odc       (1001) odc        (121)     5450 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/test_gbox_ops.py
+-rw-r--r--   0 odc       (1001) odc        (121)    51557 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/test_geometry.py
+-rw-r--r--   0 odc       (1001) odc        (121)    13585 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/test_load_data.py
+-rw-r--r--   0 odc       (1001) odc        (121)     4966 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/test_metadata_fields.py
+-rw-r--r--   0 odc       (1001) odc        (121)    13540 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/test_model.py
+-rw-r--r--   0 odc       (1001) odc        (121)     3490 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/test_testutils.py
+-rw-r--r--   0 odc       (1001) odc        (121)     9030 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/test_utils_aws.py
+-rw-r--r--   0 odc       (1001) odc        (121)     3150 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/test_utils_changes.py
+-rw-r--r--   0 odc       (1001) odc        (121)     6674 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/test_utils_cog.py
+-rw-r--r--   0 odc       (1001) odc        (121)     6045 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/test_utils_dask.py
+-rw-r--r--   0 odc       (1001) odc        (121)     2729 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/test_utils_dates.py
+-rw-r--r--   0 odc       (1001) odc        (121)    20398 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/test_utils_docs.py
+-rw-r--r--   0 odc       (1001) odc        (121)     1463 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/test_utils_generic.py
+-rw-r--r--   0 odc       (1001) odc        (121)    23249 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/test_utils_other.py
+-rw-r--r--   0 odc       (1001) odc        (121)     5752 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/test_utils_rio.py
+-rw-r--r--   0 odc       (1001) odc        (121)     3833 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/test_warp.py
+-rw-r--r--   0 odc       (1001) odc        (121)     6513 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/test_xarray_extension.py
+drwxrwxr-x   0 odc       (1001) odc        (121)        0 2022-11-17 00:48:13.818910 datacube-1.8.9/tests/ui/
+-rw-r--r--   0 odc       (1001) odc        (121)      176 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/ui/__init__.py
+-rw-r--r--   0 odc       (1001) odc        (121)     3621 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/ui/test_common.py
+-rw-r--r--   0 odc       (1001) odc        (121)     5271 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/ui/test_expression_parsing.py
+-rw-r--r--   0 odc       (1001) odc        (121)     6337 2022-11-17 00:47:28.000000 datacube-1.8.9/tests/ui/test_task_app.py
+-rw-r--r--   0 odc       (1001) odc        (121)     3724 2022-11-17 00:47:28.000000 datacube-1.8.9/wordlist.txt
```

### Comparing `datacube-1.8.8rc1/.dockerignore` & `datacube-1.8.9/.dockerignore`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -75,8 +75,8 @@
 
 # Generated Documentation
 generate/
 docs/notebooks/
 
 #Local Visual Studio Code configurations
 .vscode/
-.env
+.env
```

### Comparing `datacube-1.8.8rc1/.gitignore` & `datacube-1.8.9/.gitignore`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/.pre-commit-config.yaml` & `datacube-1.8.9/.pre-commit-config.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 repos:
     - repo: https://github.com/adrienverge/yamllint.git
-      rev: v1.19.0
+      rev: v1.28.0
       hooks:
         - id: yamllint
     - repo: https://github.com/pre-commit/pre-commit-hooks
       rev: v2.4.0
       hooks:
         - id: flake8
         - id: end-of-file-fixer
         - id: check-docstring-first
         - id: check-json
         - id: check-yaml
           args: [--allow-multiple-documents]
         - id: debug-statements
         - id: name-tests-test
           args: ['--django']
+          exclude: ^tests/drivers/fail_drivers
         - id: requirements-txt-fixer
         - id: check-added-large-files
         - id: check-merge-conflict
     -   repo: https://github.com/pre-commit/mirrors-pylint
-        rev: v2.4.4  # Use the sha / tag you want to point at
+        rev: v3.0.0a5  # Use the sha / tag you want to point at
         hooks:
         -   id: pylint
```

### Comparing `datacube-1.8.8rc1/.yamllint` & `datacube-1.8.9/.yamllint`

 * *Files 0% similar despite different names*

```diff
@@ -24,11 +24,7 @@
     commas: disable
     new-line-at-end-of-file: disable
     brackets: disable
     hyphens: disable
     colons: disable
     comments: disable
     comments-indentation: disable
-
-
-
-
```

### Comparing `datacube-1.8.8rc1/CONTRIBUTING.md` & `datacube-1.8.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/LICENSE` & `datacube-1.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/PKG-INFO` & `datacube-1.8.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datacube
-Version: 1.8.8rc1
+Version: 1.8.9
 Summary: An analysis environment for satellite and other earth observation data
 Home-page: https://github.com/opendatacube/datacube-core
 Author: Open Data Cube
 Maintainer: Open Data Cube
 Maintainer-email: 
 License: Apache License 2.0
 Platform: UNKNOWN
@@ -36,15 +36,25 @@
 Provides-Extra: s3
 Provides-Extra: test
 License-File: LICENSE
 
 Open Data Cube Core
 ===================
 
-|Build Status| |Coverage Status| |Documentation Status|
+.. image:: https://github.com/opendatacube/datacube-core/workflows/build/badge.svg
+    :alt: Build Status
+    :target: https://github.com/opendatacube/datacube-core/actions
+
+.. image:: https://codecov.io/gh/opendatacube/datacube-core/branch/develop/graph/badge.svg
+    :alt: Coverage Status
+    :target: https://codecov.io/gh/opendatacube/datacube-core
+
+.. image:: https://readthedocs.org/projects/datacube-core/badge/?version=latest
+    :alt: Documentation Status
+    :target: http://datacube-core.readthedocs.org/en/latest/
 
 Overview
 ========
 
 The Open Data Cube Core provides an integrated gridded data
 analysis environment for decades of analysis ready earth observation
 satellite and related data from multiple satellite and other acquisition
@@ -131,52 +141,45 @@
 
    ./check-code.sh --with-docker integration_tests
 
 
 To run individual test in docker container
 
 ::
+
     docker run -ti -v /home/ubuntu/datacube-core:/code opendatacube/datacube-tests:latest pytest integration_tests/test_filename.py::test_function_name
 
 
 Developer setup on Ubuntu
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Building a Python virtual environment on Ubuntu suitable for development work.
 
 Install dependencies:
 
 ::
 
-   sudo apt-get update
-   sudo apt-get install -y \
-     autoconf automake build-essential make cmake \
-     graphviz \
-     python3-venv \
-     python3-dev \
-     libpq-dev \
-     libyaml-dev \
-     libnetcdf-dev \
-     libudunits2-dev
+    sudo apt-get update
+    sudo apt-get install -y \
+        autoconf automake build-essential make cmake \
+        graphviz \
+        python3-venv \
+        python3-dev \
+        libpq-dev \
+        libyaml-dev \
+        libnetcdf-dev \
+        libudunits2-dev
 
 
 Build the python virtual environment:
 
 ::
 
-   pyenv="${HOME}/.envs/odc"  # Change to suit your needs
-   mkdir -p "${pyenv}"
-   python3 -m venv "${pyenv}"
-   source "${pyenv}/bin/activate"
-   pip install -U pip wheel cython numpy
-   pip install -e '.[dev]'
-   pip install flake8 mypy pylint autoflake black
-
-
-.. |Build Status| image:: https://github.com/opendatacube/datacube-core/workflows/build/badge.svg
-   :target: https://github.com/opendatacube/datacube-core/actions
-.. |Coverage Status| image:: https://codecov.io/gh/opendatacube/datacube-core/branch/develop/graph/badge.svg
-   :target: https://codecov.io/gh/opendatacube/datacube-core
-.. |Documentation Status| image:: https://readthedocs.org/projects/datacube-core/badge/?version=latest
-   :target: http://datacube-core.readthedocs.org/en/latest/
+    pyenv="${HOME}/.envs/odc"  # Change to suit your needs
+    mkdir -p "${pyenv}"
+    python3 -m venv "${pyenv}"
+    source "${pyenv}/bin/activate"
+    pip install -U pip wheel cython numpy
+    pip install -e '.[dev]'
+    pip install flake8 mypy pylint autoflake black
```

### Comparing `datacube-1.8.8rc1/README.rst` & `datacube-1.8.9/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 Open Data Cube Core
 ===================
 
-|Build Status| |Coverage Status| |Documentation Status|
+.. image:: https://github.com/opendatacube/datacube-core/workflows/build/badge.svg
+    :alt: Build Status
+    :target: https://github.com/opendatacube/datacube-core/actions
+
+.. image:: https://codecov.io/gh/opendatacube/datacube-core/branch/develop/graph/badge.svg
+    :alt: Coverage Status
+    :target: https://codecov.io/gh/opendatacube/datacube-core
+
+.. image:: https://readthedocs.org/projects/datacube-core/badge/?version=latest
+    :alt: Documentation Status
+    :target: http://datacube-core.readthedocs.org/en/latest/
 
 Overview
 ========
 
 The Open Data Cube Core provides an integrated gridded data
 analysis environment for decades of analysis ready earth observation
 satellite and related data from multiple satellite and other acquisition
@@ -92,50 +102,43 @@
 
    ./check-code.sh --with-docker integration_tests
 
 
 To run individual test in docker container
 
 ::
+
     docker run -ti -v /home/ubuntu/datacube-core:/code opendatacube/datacube-tests:latest pytest integration_tests/test_filename.py::test_function_name
 
 
 Developer setup on Ubuntu
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Building a Python virtual environment on Ubuntu suitable for development work.
 
 Install dependencies:
 
 ::
 
-   sudo apt-get update
-   sudo apt-get install -y \
-     autoconf automake build-essential make cmake \
-     graphviz \
-     python3-venv \
-     python3-dev \
-     libpq-dev \
-     libyaml-dev \
-     libnetcdf-dev \
-     libudunits2-dev
+    sudo apt-get update
+    sudo apt-get install -y \
+        autoconf automake build-essential make cmake \
+        graphviz \
+        python3-venv \
+        python3-dev \
+        libpq-dev \
+        libyaml-dev \
+        libnetcdf-dev \
+        libudunits2-dev
 
 
 Build the python virtual environment:
 
 ::
 
-   pyenv="${HOME}/.envs/odc"  # Change to suit your needs
-   mkdir -p "${pyenv}"
-   python3 -m venv "${pyenv}"
-   source "${pyenv}/bin/activate"
-   pip install -U pip wheel cython numpy
-   pip install -e '.[dev]'
-   pip install flake8 mypy pylint autoflake black
-
-
-.. |Build Status| image:: https://github.com/opendatacube/datacube-core/workflows/build/badge.svg
-   :target: https://github.com/opendatacube/datacube-core/actions
-.. |Coverage Status| image:: https://codecov.io/gh/opendatacube/datacube-core/branch/develop/graph/badge.svg
-   :target: https://codecov.io/gh/opendatacube/datacube-core
-.. |Documentation Status| image:: https://readthedocs.org/projects/datacube-core/badge/?version=latest
-   :target: http://datacube-core.readthedocs.org/en/latest/
+    pyenv="${HOME}/.envs/odc"  # Change to suit your needs
+    mkdir -p "${pyenv}"
+    python3 -m venv "${pyenv}"
+    source "${pyenv}/bin/activate"
+    pip install -U pip wheel cython numpy
+    pip install -e '.[dev]'
+    pip install flake8 mypy pylint autoflake black
```

### Comparing `datacube-1.8.8rc1/check-code.sh` & `datacube-1.8.9/check-code.sh`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/code-of-conduct.md` & `datacube-1.8.9/code-of-conduct.md`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/__init__.py` & `datacube-1.8.9/datacube/__init__.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/api/core.py` & `datacube-1.8.9/datacube/api/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -622,15 +622,15 @@
         return xarray.Dataset({m.name: mk_data_var(m, shape, coords, dims, data_func)
                                for m, shape, coords, dims in arrays},
                               coords=ds_coords,
                               attrs=crs_attrs)
 
     @staticmethod
     def _dask_load(sources, geobox, measurements, dask_chunks,
-                   skip_broken_datasets=False, extra_dims=None):
+                   skip_broken_datasets=False, extra_dims=None, patch_url=None):
         chunk_sizes = _calculate_chunk_sizes(sources, geobox, dask_chunks, extra_dims)
         needed_irr_chunks = chunk_sizes[0]
         if extra_dims:
             extra_dim_chunks = chunk_sizes[1]
         grid_chunks = chunk_sizes[-1]
         gbt = GeoboxTiles(geobox, grid_chunks)
         dsk = {}
@@ -652,15 +652,16 @@
                 chunks = needed_irr_chunks + extra_dim_chunks + grid_chunks
             else:
                 chunks = needed_irr_chunks + grid_chunks
             return _make_dask_array(chunked_srcs, dsk, gbt,
                                     measurement,
                                     chunks=chunks,
                                     skip_broken_datasets=skip_broken_datasets,
-                                    extra_dims=extra_dims)
+                                    extra_dims=extra_dims,
+                                    patch_url=patch_url)
 
         return Datacube.create_storage(sources.coords, geobox, measurements, data_func, extra_dims)
 
     @staticmethod
     def _xr_load(sources, geobox, measurements,
                  skip_broken_datasets=False,
                  progress_cbk=None, extra_dims=None,
@@ -770,20 +771,18 @@
         :rtype: xarray.Dataset
 
         .. seealso:: :meth:`find_datasets` :meth:`group_datasets`
         """
         measurements = per_band_load_data_settings(measurements, resampling=resampling, fuse_func=fuse_func)
 
         if dask_chunks is not None:
-            if patch_url is not None:
-                # TODO: url mangler for Dask?
-                raise ValueError("The patch_url arguments is not currently supported for Dask loading.")
             return Datacube._dask_load(sources, geobox, measurements, dask_chunks,
                                        skip_broken_datasets=skip_broken_datasets,
-                                       extra_dims=extra_dims)
+                                       extra_dims=extra_dims,
+                                       patch_url=patch_url)
         else:
             return Datacube._xr_load(sources, geobox, measurements,
                                      skip_broken_datasets=skip_broken_datasets,
                                      progress_cbk=progress_cbk,
                                      extra_dims=extra_dims,
                                      patch_url=patch_url)
 
@@ -993,15 +992,16 @@
 # pylint: disable=too-many-locals
 def _make_dask_array(chunked_srcs,
                      dsk,
                      gbt,
                      measurement,
                      chunks,
                      skip_broken_datasets=False,
-                     extra_dims=None):
+                     extra_dims=None,
+                     patch_url=None):
     dsk = dsk.copy()  # this contains mapping from dataset id to dataset object
 
     token = uuid.uuid4().hex
     dsk_name = 'dc_load_{name}-{token}'.format(name=measurement.name, token=token)
 
     needed_irr_chunks, grid_chunks = chunks[:-2], chunks[-2:]
     actual_irr_chunks = (1,) * len(needed_irr_chunks)
@@ -1048,19 +1048,19 @@
                        len(needed_irr_chunks))
 
                 # 3D case
                 if 'extra_dim' in measurement:
                     # Do extra_dim subsetting here
                     index_subset = extra_dims.measurements_index(measurement.extra_dim)
                     for result_index, extra_dim_index in enumerate(range(*index_subset)):
-                        dsk[key_prefix + (result_index,) + idx] = val + (extra_dim_index,)
+                        dsk[key_prefix + (result_index,) + idx] = val + (extra_dim_index, patch_url)
                 else:
                     # Get extra_dim index if available
                     extra_dim_index = measurement.get('extra_dim_index', None)
-                    dsk[key_prefix + idx] = val + (extra_dim_index,)
+                    dsk[key_prefix + idx] = val + (extra_dim_index, patch_url)
 
     y_shapes = [grid_chunks[0]]*gbt.shape[0]
     x_shapes = [grid_chunks[1]]*gbt.shape[1]
 
     y_shapes[-1], x_shapes[-1] = gbt.chunk_shape(tuple(n-1 for n in gbt.shape))
 
     extra_dim_shape = ()
```

### Comparing `datacube-1.8.8rc1/datacube/api/grid_workflow.py` & `datacube-1.8.9/datacube/api/grid_workflow.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/api/query.py` & `datacube-1.8.9/datacube/api/query.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/config.py` & `datacube-1.8.9/datacube/config.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/drivers/__init__.py` & `datacube-1.8.9/datacube/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/drivers/_tools.py` & `datacube-1.8.9/datacube/drivers/_tools.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/drivers/_types.py` & `datacube-1.8.9/datacube/drivers/_types.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/drivers/datasource.py` & `datacube-1.8.9/datacube/drivers/datasource.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/drivers/driver_cache.py` & `datacube-1.8.9/datacube/drivers/driver_cache.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/drivers/indexes.py` & `datacube-1.8.9/datacube/drivers/indexes.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/drivers/netcdf/_safestrings.py` & `datacube-1.8.9/datacube/drivers/netcdf/_safestrings.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/drivers/netcdf/_write.py` & `datacube-1.8.9/datacube/drivers/netcdf/_write.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/drivers/netcdf/driver.py` & `datacube-1.8.9/datacube/drivers/netcdf/driver.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/drivers/netcdf/writer.py` & `datacube-1.8.9/datacube/drivers/netcdf/writer.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/drivers/postgis/_api.py` & `datacube-1.8.9/datacube/drivers/postgis/_api.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/drivers/postgis/_connections.py` & `datacube-1.8.9/datacube/drivers/postgis/_connections.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/drivers/postgis/_core.py` & `datacube-1.8.9/datacube/drivers/postgis/_core.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/drivers/postgis/_dynamic.py` & `datacube-1.8.9/datacube/drivers/postgis/_dynamic.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/drivers/postgis/_fields.py` & `datacube-1.8.9/datacube/drivers/postgis/_fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -487,15 +487,15 @@
         self.low_value = low_value
         self.high_value = high_value
         self._range_class = _range_class
 
     @property
     def alchemy_expression(self):
         return self.field.alchemy_expression.overlaps(
-            self._range_class(self.low_value, self.high_value)
+            self._range_class(self.low_value, self.high_value, bounds='[]')
         )
 
 
 class RangeContainsExpression(PgExpression):
     def __init__(self, field, value):
         super(RangeContainsExpression, self).__init__(field)
         self.value = value
```

### Comparing `datacube-1.8.8rc1/datacube/drivers/postgis/_schema.py` & `datacube-1.8.9/datacube/drivers/postgis/_schema.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/drivers/postgis/_spatial.py` & `datacube-1.8.9/datacube/drivers/postgis/_spatial.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         sir.register(epsg)
         spindex = sir.get(epsg)
     return spindex
 
 
 def spindex_for_crs(crs: CRS) -> Type[SpatialIndex]:
     """Return ORM class of a SpatialIndex for CRS - dynamically creating if necessary"""
-    if not (str(crs).startswith('EPSG') and crs.epsg):
+    if not str(crs).startswith("EPSG:") and crs.epsg is None:
         # Postgis identifies CRSs by a numeric "SRID" which is equivalent to EPSG number.
         _LOG.error("Cannot create a postgis spatial index for a non-EPSG-style CRS.")
         return None
 
     return spindex_for_epsg(crs.epsg)
```

### Comparing `datacube-1.8.8rc1/datacube/drivers/postgis/samples/range-tests-explicit.sql` & `datacube-1.8.9/datacube/drivers/postgis/samples/range-tests-explicit.sql`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/drivers/postgis/samples/range-tests-scalar.sql` & `datacube-1.8.9/datacube/drivers/postgis/samples/range-tests-scalar.sql`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/drivers/postgis/samples/range-tests-view.sql` & `datacube-1.8.9/datacube/drivers/postgis/samples/range-tests-view.sql`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/drivers/postgis/sql.py` & `datacube-1.8.9/datacube/drivers/postgis/sql.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/drivers/postgres/_api.py` & `datacube-1.8.9/datacube/drivers/postgres/_api.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/drivers/postgres/_connections.py` & `datacube-1.8.9/datacube/drivers/postgres/_connections.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/drivers/postgres/_core.py` & `datacube-1.8.9/datacube/drivers/postgres/_core.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/drivers/postgres/_dynamic.py` & `datacube-1.8.9/datacube/drivers/postgres/_dynamic.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/drivers/postgres/_fields.py` & `datacube-1.8.9/datacube/drivers/postgres/_fields.py`

 * *Files 1% similar despite different names*

```diff
@@ -487,15 +487,15 @@
         self.low_value = low_value
         self.high_value = high_value
         self._range_class = _range_class
 
     @property
     def alchemy_expression(self):
         return self.field.alchemy_expression.overlaps(
-            self._range_class(self.low_value, self.high_value)
+            self._range_class(self.low_value, self.high_value, bounds="[]")
         )
 
 
 class RangeContainsExpression(PgExpression):
     def __init__(self, field, value):
         super(RangeContainsExpression, self).__init__(field)
         self.value = value
```

### Comparing `datacube-1.8.8rc1/datacube/drivers/postgres/_schema.py` & `datacube-1.8.9/datacube/drivers/postgres/_schema.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/drivers/postgres/samples/range-tests-explicit.sql` & `datacube-1.8.9/datacube/drivers/postgres/samples/range-tests-explicit.sql`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/drivers/postgres/samples/range-tests-scalar.sql` & `datacube-1.8.9/datacube/drivers/postgres/samples/range-tests-scalar.sql`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/drivers/postgres/samples/range-tests-view.sql` & `datacube-1.8.9/datacube/drivers/postgres/samples/range-tests-view.sql`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/drivers/postgres/sql.py` & `datacube-1.8.9/datacube/drivers/postgres/sql.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/drivers/readers.py` & `datacube-1.8.9/datacube/drivers/readers.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/drivers/rio/_reader.py` & `datacube-1.8.9/datacube/drivers/rio/_reader.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/drivers/writers.py` & `datacube-1.8.9/datacube/drivers/writers.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/execution/worker.py` & `datacube-1.8.9/datacube/execution/worker.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/executor.py` & `datacube-1.8.9/datacube/executor.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/helpers.py` & `datacube-1.8.9/datacube/helpers.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/index/__init__.py` & `datacube-1.8.9/datacube/index/__init__.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/index/_api.py` & `datacube-1.8.9/datacube/index/_api.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/index/abstract.py` & `datacube-1.8.9/datacube/index/abstract.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/index/default-metadata-types.yaml` & `datacube-1.8.9/datacube/index/default-metadata-types.yaml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -306,8 +306,8 @@
 
             type: integer-range
             min_offset:
             - [image, satellite_ref_point_start, y]
             max_offset:
             - [image, satellite_ref_point_end, y]
             # If an end is not specified, use the start.
-            - [image, satellite_ref_point_start, y]
+            - [image, satellite_ref_point_start, y]
```

### Comparing `datacube-1.8.8rc1/datacube/index/eo3.py` & `datacube-1.8.9/datacube/index/eo3.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/index/fields.py` & `datacube-1.8.9/datacube/index/fields.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/index/hl.py` & `datacube-1.8.9/datacube/index/hl.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/index/memory/_datasets.py` & `datacube-1.8.9/datacube/index/memory/_datasets.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/index/memory/_fields.py` & `datacube-1.8.9/datacube/index/memory/_fields.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/index/memory/_metadata_types.py` & `datacube-1.8.9/datacube/index/memory/_metadata_types.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/index/memory/_products.py` & `datacube-1.8.9/datacube/index/memory/_products.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/index/memory/_users.py` & `datacube-1.8.9/datacube/index/memory/_users.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/index/memory/index.py` & `datacube-1.8.9/datacube/index/memory/index.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/index/null/_datasets.py` & `datacube-1.8.9/datacube/index/null/_datasets.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/index/null/_metadata_types.py` & `datacube-1.8.9/datacube/index/null/_metadata_types.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/index/null/_products.py` & `datacube-1.8.9/datacube/index/null/_products.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/index/null/_users.py` & `datacube-1.8.9/datacube/index/null/_users.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/index/null/index.py` & `datacube-1.8.9/datacube/index/null/index.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/index/postgis/_datasets.py` & `datacube-1.8.9/datacube/index/postgis/_datasets.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/index/postgis/_metadata_types.py` & `datacube-1.8.9/datacube/index/postgis/_metadata_types.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/index/postgis/_products.py` & `datacube-1.8.9/datacube/index/postgis/_products.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/index/postgis/_transaction.py` & `datacube-1.8.9/datacube/index/postgis/_transaction.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/index/postgis/_users.py` & `datacube-1.8.9/datacube/index/postgis/_users.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/index/postgis/index.py` & `datacube-1.8.9/datacube/index/postgis/index.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/index/postgres/_datasets.py` & `datacube-1.8.9/datacube/index/postgres/_datasets.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/index/postgres/_metadata_types.py` & `datacube-1.8.9/datacube/index/postgres/_metadata_types.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/index/postgres/_products.py` & `datacube-1.8.9/datacube/index/postgres/_products.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/index/postgres/_transaction.py` & `datacube-1.8.9/datacube/index/postgres/_transaction.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/index/postgres/_users.py` & `datacube-1.8.9/datacube/index/postgres/_users.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/index/postgres/index.py` & `datacube-1.8.9/datacube/index/postgres/index.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/model/__init__.py` & `datacube-1.8.9/datacube/model/__init__.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/model/_base.py` & `datacube-1.8.9/datacube/model/_base.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/model/fields.py` & `datacube-1.8.9/datacube/model/fields.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/model/schema/dataset-type-schema.yaml` & `datacube-1.8.9/datacube/model/schema/dataset-type-schema.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/model/schema/ingestor-config-type-schema.yaml` & `datacube-1.8.9/datacube/model/schema/ingestor-config-type-schema.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -53,16 +53,14 @@
                 type: string
             license:
                 type: string
             naming_authority:
                 type: string
             acknowkledgment:
                 type: string
-            references:
-                type: string
     ingestion_bounds:
         type: object
         properties:
             left:
                 type: number
             bottom:
                 type: number
```

### Comparing `datacube-1.8.8rc1/datacube/model/schema/metadata-type-schema.yaml` & `datacube-1.8.9/datacube/model/schema/metadata-type-schema.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,15 @@
                                     "$ref": "#/definitions/offset"
                         additionalProperties: false
         required:
             - id
             - creation_dt
             - label
             - sources
+            - search_fields
         additionalProperties: false
 required:
     - name
     - description
     - dataset
 additionalProperties: false
```

### Comparing `datacube-1.8.8rc1/datacube/model/utils.py` & `datacube-1.8.9/datacube/model/utils.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/scripts/cli_app.py` & `datacube-1.8.9/datacube/scripts/cli_app.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/scripts/dataset.py` & `datacube-1.8.9/datacube/scripts/dataset.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/scripts/ingest.py` & `datacube-1.8.9/datacube/scripts/ingest.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/scripts/metadata.py` & `datacube-1.8.9/datacube/scripts/metadata.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/scripts/product.py` & `datacube-1.8.9/datacube/scripts/product.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/scripts/search_tool.py` & `datacube-1.8.9/datacube/scripts/search_tool.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/scripts/system.py` & `datacube-1.8.9/datacube/scripts/system.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/scripts/user.py` & `datacube-1.8.9/datacube/scripts/user.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/storage/__init__.py` & `datacube-1.8.9/datacube/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/storage/_base.py` & `datacube-1.8.9/datacube/storage/_base.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/storage/_load.py` & `datacube-1.8.9/datacube/storage/_load.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/storage/_read.py` & `datacube-1.8.9/datacube/storage/_read.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/storage/_rio.py` & `datacube-1.8.9/datacube/storage/_rio.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/testutils/__init__.py` & `datacube-1.8.9/datacube/testutils/__init__.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/testutils/geom.py` & `datacube-1.8.9/datacube/testutils/geom.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/testutils/io.py` & `datacube-1.8.9/datacube/testutils/io.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/testutils/iodriver.py` & `datacube-1.8.9/datacube/testutils/iodriver.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/testutils/threads.py` & `datacube-1.8.9/datacube/testutils/threads.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/ui/click.py` & `datacube-1.8.9/datacube/ui/click.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/ui/common.py` & `datacube-1.8.9/datacube/ui/common.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/ui/expression.py` & `datacube-1.8.9/datacube/ui/expression.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/ui/task_app.py` & `datacube-1.8.9/datacube/ui/task_app.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/utils/__init__.py` & `datacube-1.8.9/datacube/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/utils/aws/__init__.py` & `datacube-1.8.9/datacube/utils/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/utils/changes.py` & `datacube-1.8.9/datacube/utils/changes.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/utils/cog.py` & `datacube-1.8.9/datacube/utils/cog.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/utils/dask.py` & `datacube-1.8.9/datacube/utils/dask.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/utils/dates.py` & `datacube-1.8.9/datacube/utils/dates.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/utils/documents.py` & `datacube-1.8.9/datacube/utils/documents.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/utils/generic.py` & `datacube-1.8.9/datacube/utils/generic.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/utils/geometry/__init__.py` & `datacube-1.8.9/datacube/utils/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/utils/geometry/_base.py` & `datacube-1.8.9/datacube/utils/geometry/_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,33 +112,33 @@
         :param p1: (x, y)
         :param p2: (x, y)
         """
         return BoundingBox.from_xy((p1[0], p2[0]),
                                    (p1[1], p2[1]))
 
 
-def _make_crs_key(crs_spec: Union[str, _CRS]) -> str:
+def _make_crs_key(crs_spec: Union[str, int, _CRS]) -> str:
     if isinstance(crs_spec, str):
         normed_epsg = crs_spec.upper()
         if normed_epsg.startswith("EPSG:"):
             return normed_epsg
         return crs_spec
+    if isinstance(crs_spec, int):
+        return f"EPSG:{crs_spec}"
     return crs_spec.to_wkt()
 
 
 @cachetools.cached({}, key=_make_crs_key)  # type: ignore[misc]
-def _make_crs(crs: Union[str, _CRS]) -> Tuple[_CRS, str, Optional[int]]:
-    if isinstance(crs, str):
-        crs = _CRS.from_user_input(crs)
-    epsg = crs.to_epsg()
-    if epsg is not None:
-        crs_str = f"EPSG:{epsg}"
-    else:
-        crs_str = crs.to_wkt()
-    return (crs, crs_str, crs.to_epsg())
+def _make_crs(crs: Union[str, int, _CRS]) -> Tuple[_CRS, str, Optional[int]]:
+    epsg = False
+    crs = _CRS.from_user_input(crs)
+    crs_str = crs.srs
+    if crs_str.upper().startswith("EPSG:"):
+        epsg = int(crs_str.split(":", maxsplit=1)[-1])
+    return (crs, crs_str, epsg)
 
 
 def _make_crs_transform_key(from_crs, to_crs, always_xy):
     return (id(from_crs), id(to_crs), always_xy)
 
 
 @cachetools.cached({}, key=_make_crs_transform_key)
@@ -168,27 +168,27 @@
             self._str = crs_spec._str
         elif isinstance(crs_spec, _CRS):
             self._crs, self._str, self._epsg = _make_crs(crs_spec)
         elif isinstance(crs_spec, dict):
             self._crs, self._str, self._epsg = _make_crs(_CRS.from_dict(crs_spec))
         else:
             try:
-                epsg = crs_spec.to_epsg()
-            except AttributeError:
-                epsg = None
-            if epsg is not None:
-                self._crs, self._str, self._epsg = _make_crs(f"EPSG:{epsg}")
-                return
-            try:
                 wkt = crs_spec.to_wkt()
             except AttributeError:
                 wkt = None
             if wkt is not None:
                 self._crs, self._str, self._epsg = _make_crs(wkt)
                 return
+            try:
+                epsg = crs_spec.to_epsg()
+            except AttributeError:
+                epsg = None
+            if epsg is not None:
+                self._crs, self._str, self._epsg = _make_crs(epsg)
+                return
 
             raise CRSError(
                 "Expect string or any object with `.to_epsg()` or `.to_wkt()` methods"
             )
 
     def __getstate__(self):
         return {'crs_str': self._str}
@@ -209,19 +209,22 @@
     def wkt(self) -> str:
         return self.to_wkt(version=WktVersion.WKT1_GDAL)
 
     def to_epsg(self) -> Optional[int]:
         """
         EPSG Code of the CRS or None
         """
+        if self._epsg is not False:
+            return self._epsg
+        self._epsg = self._crs.to_epsg()
         return self._epsg
 
     @property
     def epsg(self) -> Optional[int]:
-        return self._epsg
+        return self.to_epsg()
 
     @property
     def semi_major_axis(self):
         return self._crs.ellipsoid.semi_major_metre
 
     @property
     def semi_minor_axis(self):
```

### Comparing `datacube-1.8.8rc1/datacube/utils/geometry/_warp.py` & `datacube-1.8.9/datacube/utils/geometry/_warp.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/utils/geometry/gbox.py` & `datacube-1.8.9/datacube/utils/geometry/gbox.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/utils/geometry/tools.py` & `datacube-1.8.9/datacube/utils/geometry/tools.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/utils/io.py` & `datacube-1.8.9/datacube/utils/io.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/utils/masking.py` & `datacube-1.8.9/datacube/utils/masking.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/utils/math.py` & `datacube-1.8.9/datacube/utils/math.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/utils/py.py` & `datacube-1.8.9/datacube/utils/py.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/utils/rio/__init__.py` & `datacube-1.8.9/datacube/utils/rio/__init__.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/utils/rio/_rio.py` & `datacube-1.8.9/datacube/utils/rio/_rio.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/utils/serialise.py` & `datacube-1.8.9/datacube/utils/serialise.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/utils/uris.py` & `datacube-1.8.9/datacube/utils/uris.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/utils/xarray_geoextensions.py` & `datacube-1.8.9/datacube/utils/xarray_geoextensions.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/virtual/__init__.py` & `datacube-1.8.9/datacube/virtual/__init__.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/virtual/catalog.py` & `datacube-1.8.9/datacube/virtual/catalog.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/virtual/expr.py` & `datacube-1.8.9/datacube/virtual/expr.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/virtual/impl.py` & `datacube-1.8.9/datacube/virtual/impl.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/virtual/transformations.py` & `datacube-1.8.9/datacube/virtual/transformations.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube/virtual/utils.py` & `datacube-1.8.9/datacube/virtual/utils.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube.egg-info/PKG-INFO` & `datacube-1.8.9/datacube.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datacube
-Version: 1.8.8rc1
+Version: 1.8.9
 Summary: An analysis environment for satellite and other earth observation data
 Home-page: https://github.com/opendatacube/datacube-core
 Author: Open Data Cube
 Maintainer: Open Data Cube
 Maintainer-email: 
 License: Apache License 2.0
 Platform: UNKNOWN
@@ -36,15 +36,25 @@
 Provides-Extra: s3
 Provides-Extra: test
 License-File: LICENSE
 
 Open Data Cube Core
 ===================
 
-|Build Status| |Coverage Status| |Documentation Status|
+.. image:: https://github.com/opendatacube/datacube-core/workflows/build/badge.svg
+    :alt: Build Status
+    :target: https://github.com/opendatacube/datacube-core/actions
+
+.. image:: https://codecov.io/gh/opendatacube/datacube-core/branch/develop/graph/badge.svg
+    :alt: Coverage Status
+    :target: https://codecov.io/gh/opendatacube/datacube-core
+
+.. image:: https://readthedocs.org/projects/datacube-core/badge/?version=latest
+    :alt: Documentation Status
+    :target: http://datacube-core.readthedocs.org/en/latest/
 
 Overview
 ========
 
 The Open Data Cube Core provides an integrated gridded data
 analysis environment for decades of analysis ready earth observation
 satellite and related data from multiple satellite and other acquisition
@@ -131,52 +141,45 @@
 
    ./check-code.sh --with-docker integration_tests
 
 
 To run individual test in docker container
 
 ::
+
     docker run -ti -v /home/ubuntu/datacube-core:/code opendatacube/datacube-tests:latest pytest integration_tests/test_filename.py::test_function_name
 
 
 Developer setup on Ubuntu
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Building a Python virtual environment on Ubuntu suitable for development work.
 
 Install dependencies:
 
 ::
 
-   sudo apt-get update
-   sudo apt-get install -y \
-     autoconf automake build-essential make cmake \
-     graphviz \
-     python3-venv \
-     python3-dev \
-     libpq-dev \
-     libyaml-dev \
-     libnetcdf-dev \
-     libudunits2-dev
+    sudo apt-get update
+    sudo apt-get install -y \
+        autoconf automake build-essential make cmake \
+        graphviz \
+        python3-venv \
+        python3-dev \
+        libpq-dev \
+        libyaml-dev \
+        libnetcdf-dev \
+        libudunits2-dev
 
 
 Build the python virtual environment:
 
 ::
 
-   pyenv="${HOME}/.envs/odc"  # Change to suit your needs
-   mkdir -p "${pyenv}"
-   python3 -m venv "${pyenv}"
-   source "${pyenv}/bin/activate"
-   pip install -U pip wheel cython numpy
-   pip install -e '.[dev]'
-   pip install flake8 mypy pylint autoflake black
-
-
-.. |Build Status| image:: https://github.com/opendatacube/datacube-core/workflows/build/badge.svg
-   :target: https://github.com/opendatacube/datacube-core/actions
-.. |Coverage Status| image:: https://codecov.io/gh/opendatacube/datacube-core/branch/develop/graph/badge.svg
-   :target: https://codecov.io/gh/opendatacube/datacube-core
-.. |Documentation Status| image:: https://readthedocs.org/projects/datacube-core/badge/?version=latest
-   :target: http://datacube-core.readthedocs.org/en/latest/
+    pyenv="${HOME}/.envs/odc"  # Change to suit your needs
+    mkdir -p "${pyenv}"
+    python3 -m venv "${pyenv}"
+    source "${pyenv}/bin/activate"
+    pip install -U pip wheel cython numpy
+    pip install -e '.[dev]'
+    pip install flake8 mypy pylint autoflake black
```

### Comparing `datacube-1.8.8rc1/datacube.egg-info/SOURCES.txt` & `datacube-1.8.9/datacube.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .coveragerc
 .dockerignore
+.doctor-rst.yaml
 .editorconfig
 .gitattributes
 .gitignore
 .mergify.yml
 .pre-commit-config.yaml
 .yamllint
 CONTRIBUTING.md
@@ -18,20 +19,23 @@
 mypy.ini
 pylintrc
 pyproject.toml
 pytest.ini
 readthedocs.yml
 setup.cfg
 setup.py
+spellcheck.yaml
+wordlist.txt
 datacube/__init__.py
 datacube/__main__.py
 datacube/_version.py
 datacube/config.py
 datacube/executor.py
 datacube/helpers.py
+datacube/py.typed
 datacube.egg-info/PKG-INFO
 datacube.egg-info/SOURCES.txt
 datacube.egg-info/dependency_links.txt
 datacube.egg-info/entry_points.txt
 datacube.egg-info/requires.txt
 datacube.egg-info/top_level.txt
 datacube/api/__init__.py
```

### Comparing `datacube-1.8.8rc1/datacube.egg-info/entry_points.txt` & `datacube-1.8.9/datacube.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/datacube.egg-info/requires.txt` & `datacube-1.8.9/datacube.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/examples/io_plugin/dcio_example/pickles.py` & `datacube-1.8.9/examples/io_plugin/dcio_example/pickles.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/examples/io_plugin/dcio_example/xarray_3d.py` & `datacube-1.8.9/examples/io_plugin/dcio_example/xarray_3d.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/examples/io_plugin/dcio_example/zeros.py` & `datacube-1.8.9/examples/io_plugin/dcio_example/zeros.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/examples/io_plugin/setup.py` & `datacube-1.8.9/examples/io_plugin/setup.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/conftest.py` & `datacube-1.8.9/integration_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/data/dataset_add/datasets.yml` & `datacube-1.8.9/integration_tests/data/dataset_add/datasets.yml`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/data/dataset_add/datasets_bad1.yml` & `datacube-1.8.9/integration_tests/data/dataset_add/datasets_bad1.yml`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/data/dataset_add/datasets_eo3.yml` & `datacube-1.8.9/integration_tests/data/dataset_add/datasets_eo3.yml`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/data/dataset_add/metadata.yml` & `datacube-1.8.9/integration_tests/data/dataset_add/metadata.yml`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/data/dataset_add/products.yml` & `datacube-1.8.9/integration_tests/data/dataset_add/products.yml`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/data/eo3/ard_ls8.odc-product.yaml` & `datacube-1.8.9/integration_tests/data/eo3/ard_ls8.odc-product.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/data/eo3/eo3_landsat_ard.odc-type.yaml` & `datacube-1.8.9/integration_tests/data/eo3/eo3_landsat_ard.odc-type.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/data/eo3/ga_ls_wo_3.odc-product.yaml` & `datacube-1.8.9/integration_tests/data/eo3/ga_ls_wo_3.odc-product.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/data/eo3/ls8_dataset.yaml` & `datacube-1.8.9/integration_tests/data/eo3/ls8_dataset.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/data/eo3/ls8_dataset2.yaml` & `datacube-1.8.9/integration_tests/data/eo3/ls8_dataset2.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/data/eo3/ls8_dataset3.yaml` & `datacube-1.8.9/integration_tests/data/eo3/ls8_dataset3.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/data/eo3/ls8_dataset4.yaml` & `datacube-1.8.9/integration_tests/data/eo3/ls8_dataset4.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -32,16 +32,14 @@
     shape: [7781, 7691]
     transform: [3.e+01, 0.e+00, 4.32885e+05, 0.e+00, -3.e+01, -2.599185e+06, 0.e+00,
       0.e+00, 1.e+00]
 
 properties:
   datetime: '2013-07-21T00:57:26.432563Z'
   dea:dataset_maturity: final
-  dtr:end_datetime: '2013-07-21T00:57:41.398421Z'
-  dtr:start_datetime: '2013-07-21T00:57:11.356786Z'
   eo:cloud_cover: 1.828773330949106e+01
   eo:gsd: 1.5e+01  # Ground sample distance (m)
   eo:instrument: OLI_TIRS
   eo:platform: landsat-8
   eo:sun_azimuth: 3.722609952e+01
   eo:sun_elevation: 3.539504069e+01
   fmask:clear: 7.716319419426578e+01
```

### Comparing `datacube-1.8.8rc1/integration_tests/data/eo3/s2_africa_dataset.yaml` & `datacube-1.8.9/integration_tests/data/eo3/s2_africa_dataset.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/data/eo3/s2_africa_product.yaml` & `datacube-1.8.9/integration_tests/data/eo3/s2_africa_product.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/data/eo3/wo_dataset.yaml` & `datacube-1.8.9/integration_tests/data/eo3/wo_dataset.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/data/eo3/wo_ds_with_lineage.odc-metadata.yaml` & `datacube-1.8.9/integration_tests/data/eo3/wo_ds_with_lineage.odc-metadata.yaml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -215,8 +215,8 @@
     accessories:
       thumbnail:nbart:
         path: ga_ls8c_nbart_3-0-0_090086_2016-05-12_final_thumbnail.jpg
       checksum:sha1:
         path: ga_ls8c_ard_3-0-0_090086_2016-05-12_final.sha1
       metadata:processor:
         path: ga_ls8c_ard_3-0-0_090086_2016-05-12_final.proc-info.yaml
-...
+...
```

### Comparing `datacube-1.8.8rc1/integration_tests/data/ingester/invalid_config.yaml` & `datacube-1.8.9/integration_tests/data/ingester/invalid_config.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/data/ingester/invalid_src_name.yaml` & `datacube-1.8.9/integration_tests/data/ingester/invalid_src_name.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/data_utils.py` & `datacube-1.8.9/integration_tests/data_utils.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/example-ls5-nbar.yaml` & `datacube-1.8.9/integration_tests/example-ls5-nbar.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/example-ls5-nbar_302.yaml` & `datacube-1.8.9/integration_tests/example-ls5-nbar_302.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/example-ls5-nbar_505.yaml` & `datacube-1.8.9/integration_tests/example-ls5-nbar_505.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/example-ls5-nbar_606.yaml` & `datacube-1.8.9/integration_tests/example-ls5-nbar_606.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/extensive-eo-metadata.yaml` & `datacube-1.8.9/integration_tests/extensive-eo-metadata.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/index/search_utils.py` & `datacube-1.8.9/integration_tests/index/search_utils.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/index/test_config_docs.py` & `datacube-1.8.9/integration_tests/index/test_config_docs.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,14 +155,15 @@
 
 
 @pytest.mark.parametrize('datacube_env_name', ('experimental', ))
 def test_field_expression_unchanged_postgis(
         default_metadata_type: MetadataType,
         telemetry_metadata_type: MetadataType) -> None:
     # We're checking for accidental changes here in our field-to-SQL code
+    # Dubious test as it uses non-EO3 metadata types
 
     # If we started outputting a different expression they would quietly no longer match the expression
     # indexes that exist in our DBs.
 
     # The time field on the default 'eo' metadata type.
     field = default_metadata_type.dataset_fields['time']
     assert isinstance(field, PgrPgField) or isinstance(field, PgsPgField)
```

### Comparing `datacube-1.8.8rc1/integration_tests/index/test_index_data.py` & `datacube-1.8.9/integration_tests/index/test_index_data.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/index/test_memory_index.py` & `datacube-1.8.9/integration_tests/index/test_memory_index.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/index/test_null_index.py` & `datacube-1.8.9/integration_tests/index/test_null_index.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/index/test_pluggable_indexes.py` & `datacube-1.8.9/integration_tests/index/test_pluggable_indexes.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/index/test_postgis_index.py` & `datacube-1.8.9/integration_tests/index/test_postgis_index.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/index/test_search_eo3.py` & `datacube-1.8.9/integration_tests/index/test_search_eo3.py`

 * *Files 5% similar despite different names*

```diff
@@ -147,14 +147,35 @@
     datasets = index.datasets.search_eager(
         lat=Range(-37.5, -36.5),
         time=datetime.datetime(2016, 5, 12, 23, 0, 0)
     )
     assert len(datasets) == 0
 
 
+def test_zero_width_range_search(index: Index, ls8_eo3_dataset4: Dataset) -> None:
+    # Test time search against zero-width time metadata
+    datasets = index.datasets.search_eager(time=Range(
+        begin=datetime.datetime(2013, 7, 21, 0, 57, 26, 432563, tzinfo=datetime.timezone.utc),
+        end=datetime.datetime(2013, 7, 21, 0, 57, 26, 432563, tzinfo=datetime.timezone.utc)
+    ))
+    assert len(datasets) == 1
+
+    datasets = index.datasets.search_eager(time=Range(
+        begin=datetime.datetime(2013, 7, 21, 0, 57, 26, 432563, tzinfo=datetime.timezone.utc),
+        end=datetime.datetime(2013, 7, 21, 0, 57, 27, 432563, tzinfo=datetime.timezone.utc)
+    ))
+    assert len(datasets) == 1
+
+    datasets = index.datasets.search_eager(time=Range(
+        begin=datetime.datetime(2013, 7, 21, 0, 57, 25, 432563, tzinfo=datetime.timezone.utc),
+        end=datetime.datetime(2013, 7, 21, 0, 57, 26, 432563, tzinfo=datetime.timezone.utc)
+    ))
+    assert len(datasets) == 1
+
+
 def test_search_globally_eo3(index: Index, ls8_eo3_dataset: Dataset) -> None:
     # No expressions means get all.
     results = list(index.datasets.search())
     assert len(results) == 1
 
     # Dataset sources aren't loaded by default
     assert results[0].sources is None
```

### Comparing `datacube-1.8.8rc1/integration_tests/index/test_search_legacy.py` & `datacube-1.8.9/integration_tests/index/test_search_legacy.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/index/test_update_columns.py` & `datacube-1.8.9/integration_tests/index/test_update_columns.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/test_3d.py` & `datacube-1.8.9/integration_tests/test_3d.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/test_cli_output.py` & `datacube-1.8.9/integration_tests/test_cli_output.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/test_config_tool.py` & `datacube-1.8.9/integration_tests/test_config_tool.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/test_dataset_add.py` & `datacube-1.8.9/integration_tests/test_dataset_add.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/test_double_ingestion.py` & `datacube-1.8.9/integration_tests/test_double_ingestion.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/test_end_to_end.py` & `datacube-1.8.9/integration_tests/test_end_to_end.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/test_environments.py` & `datacube-1.8.9/integration_tests/test_environments.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/test_full_ingestion.py` & `datacube-1.8.9/integration_tests/test_full_ingestion.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/test_index_datasets_search.py` & `datacube-1.8.9/integration_tests/test_index_datasets_search.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/test_index_out_of_bound.py` & `datacube-1.8.9/integration_tests/test_index_out_of_bound.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/test_model.py` & `datacube-1.8.9/integration_tests/test_model.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/test_validate_ingestion.py` & `datacube-1.8.9/integration_tests/test_validate_ingestion.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/integration_tests/utils.py` & `datacube-1.8.9/integration_tests/utils.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/license-headers.md` & `datacube-1.8.9/license-headers.md`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/pylintrc` & `datacube-1.8.9/pylintrc`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/setup.py` & `datacube-1.8.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,15 @@
 
     packages=find_packages(
         exclude=('tests', 'tests.*',
                  'integration_tests', 'integration_tests.*')
     ),
     package_data={
         '': ['*.yaml', '*/*.yaml'],
+        'datacube': ['py.typed'],
     },
     scripts=[],
     install_requires=[
         'affine',
         'pyproj>=2.5',
         'shapely>=1.6.4',
         'cachetools',
```

### Comparing `datacube-1.8.8rc1/tests/api/test_core.py` & `datacube-1.8.9/tests/api/test_core.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/api/test_grid_workflow.py` & `datacube-1.8.9/tests/api/test_grid_workflow.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/api/test_masking.py` & `datacube-1.8.9/tests/api/test_masking.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/api/test_query.py` & `datacube-1.8.9/tests/api/test_query.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/api/test_virtual.py` & `datacube-1.8.9/tests/api/test_virtual.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/conftest.py` & `datacube-1.8.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/data/ds_eo.yaml` & `datacube-1.8.9/tests/data/ds_eo.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/data/ds_eo3.yml` & `datacube-1.8.9/tests/data/ds_eo3.yml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,8 @@
     default:
        shape: [100, 200]
        transform: [10, 0, 100000, 0, -10, 200000, 0, 0, 1]
 lineage:
   a: [f80c30a5-1036-5607-a62f-fde5e3fec985]
   bc:
     - fb077e47-f62e-5869-9bd1-03584c2d7380
-    - 13d3d75a-1d90-5ec0-8b86-e8be78275660
+    - 13d3d75a-1d90-5ec0-8b86-e8be78275660
```

### Comparing `datacube-1.8.8rc1/tests/data/eo3.yaml` & `datacube-1.8.9/tests/data/eo3.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/agdc-metadata.yaml` & `datacube-1.8.9/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/agdc-metadata.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/metadata.xml` & `datacube-1.8.9/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/metadata.xml`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B10.tif` & `datacube-1.8.9/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B10.tif`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B20.tif` & `datacube-1.8.9/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B20.tif`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B30.tif` & `datacube-1.8.9/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B30.tif`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B40.tif` & `datacube-1.8.9/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B40.tif`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B50.tif` & `datacube-1.8.9/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B50.tif`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B70.tif` & `datacube-1.8.9/tests/data/lbg/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323/scene01/LS5_TM_NBAR_P54_GANBAR01-002_090_084_19920323_B70.tif`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/data/lbg/LS5_TM_PQ_P55_GAPQ01-002_090_084_19920323/agdc-metadata.yaml` & `datacube-1.8.9/tests/data/lbg/LS5_TM_PQ_P55_GAPQ01-002_090_084_19920323/agdc-metadata.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/data/lbg/LS5_TM_PQ_P55_GAPQ01-002_090_084_19920323/metadata.xml` & `datacube-1.8.9/tests/data/lbg/LS5_TM_PQ_P55_GAPQ01-002_090_084_19920323/metadata.xml`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/data/lbg/LS5_TM_PQ_P55_GAPQ01-002_090_084_19920323/scene01/LS5_TM_PQ_P55_GAPQ01-002_090_084_19920323_1111111111111100.tif` & `datacube-1.8.9/tests/data/lbg/LS5_TM_PQ_P55_GAPQ01-002_090_084_19920323/scene01/LS5_TM_PQ_P55_GAPQ01-002_090_084_19920323_1111111111111100.tif`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/GEDI02_B_2019228092851_O03828_T04236_02_001_01_cover.xarray_3d` & `datacube-1.8.9/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/GEDI02_B_2019228092851_O03828_T04236_02_001_01_cover.xarray_3d`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/GEDI02_B_2019228092851_O03828_T04236_02_001_01_cover_z.xarray_3d` & `datacube-1.8.9/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/GEDI02_B_2019228092851_O03828_T04236_02_001_01_cover_z.xarray_3d`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/GEDI02_B_2019228092851_O03828_T04236_02_001_01_pai.xarray_3d` & `datacube-1.8.9/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/GEDI02_B_2019228092851_O03828_T04236_02_001_01_pai.xarray_3d`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/GEDI02_B_2019228092851_O03828_T04236_02_001_01_pai_z.xarray_3d` & `datacube-1.8.9/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/GEDI02_B_2019228092851_O03828_T04236_02_001_01_pai_z.xarray_3d`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/__GEDI02_B_2019228092851_O03828_T04236_02_001_01_gedi_l2b.yaml` & `datacube-1.8.9/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/__GEDI02_B_2019228092851_O03828_T04236_02_001_01_gedi_l2b.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/__GEDI02_B_2019228092851_O03828_T04236_02_001_01_gedi_l2b_cover_z.yaml` & `datacube-1.8.9/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/__GEDI02_B_2019228092851_O03828_T04236_02_001_01_gedi_l2b_cover_z.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/__GEDI02_B_2019228092851_O03828_T04236_02_001_01_gedi_l2b_pai_z.yaml` & `datacube-1.8.9/tests/data/lbg/gedi/GEDI02_B_2019228092851_O03828_T04236_02_001_01/__GEDI02_B_2019228092851_O03828_T04236_02_001_01_gedi_l2b_pai_z.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/GEDI02_B_2019294155401_O04856_T03859_02_001_01_cover.xarray_3d` & `datacube-1.8.9/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/GEDI02_B_2019294155401_O04856_T03859_02_001_01_cover.xarray_3d`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/GEDI02_B_2019294155401_O04856_T03859_02_001_01_cover_z.xarray_3d` & `datacube-1.8.9/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/GEDI02_B_2019294155401_O04856_T03859_02_001_01_cover_z.xarray_3d`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/GEDI02_B_2019294155401_O04856_T03859_02_001_01_pai.xarray_3d` & `datacube-1.8.9/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/GEDI02_B_2019294155401_O04856_T03859_02_001_01_pai.xarray_3d`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/GEDI02_B_2019294155401_O04856_T03859_02_001_01_pai_z.xarray_3d` & `datacube-1.8.9/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/GEDI02_B_2019294155401_O04856_T03859_02_001_01_pai_z.xarray_3d`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/__GEDI02_B_2019294155401_O04856_T03859_02_001_01_gedi_l2b.yaml` & `datacube-1.8.9/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/__GEDI02_B_2019294155401_O04856_T03859_02_001_01_gedi_l2b.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/__GEDI02_B_2019294155401_O04856_T03859_02_001_01_gedi_l2b_cover_z.yaml` & `datacube-1.8.9/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/__GEDI02_B_2019294155401_O04856_T03859_02_001_01_gedi_l2b_cover_z.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/__GEDI02_B_2019294155401_O04856_T03859_02_001_01_gedi_l2b_pai_z.yaml` & `datacube-1.8.9/tests/data/lbg/gedi/GEDI02_B_2019294155401_O04856_T03859_02_001_01/__GEDI02_B_2019294155401_O04856_T03859_02_001_01_gedi_l2b_pai_z.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/data/lbg/gedi/GEDI02_B_3d_format.yaml` & `datacube-1.8.9/tests/data/lbg/gedi/GEDI02_B_3d_format.yaml`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/md5sum.txt` & `datacube-1.8.9/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/md5sum.txt`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/metadata.xml` & `datacube-1.8.9/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/metadata.xml`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B1.tif` & `datacube-1.8.9/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B1.tif`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B2.tif` & `datacube-1.8.9/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B2.tif`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B3.tif` & `datacube-1.8.9/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B3.tif`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B4.tif` & `datacube-1.8.9/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B4.tif`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B5.tif` & `datacube-1.8.9/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B5.tif`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B6.tif` & `datacube-1.8.9/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B6.tif`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B7.tif` & `datacube-1.8.9/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012_B7.tif`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/report.txt` & `datacube-1.8.9/tests/data/ls8-eods-nbar/data/LS8_OLI_TIRS_NBAR_P54_GANBAR01-015_101_078_20141012/scene01/report.txt`

 * *Files 0% similar despite different names*

```diff
@@ -46,8 +46,7 @@
   |                                                |
   |                                                |
   |                                                |
   Lat:   -26.9652800              Lat:   -26.9633800
   Long:  133.9623300              Long:  136.2696200
   North: 7016987.500              North: 7016987.500
   East:   397012.500 ------------ East:   626012.500
-
```

### Comparing `datacube-1.8.8rc1/tests/data/multi_doc.nc` & `datacube-1.8.9/tests/data/multi_doc.nc`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/data/no_crs_ds.tif` & `datacube-1.8.9/tests/data/no_crs_ds.tif`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/data/sample_tile.nc` & `datacube-1.8.9/tests/data/sample_tile.nc`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/data/sample_tile_151_-29.tif` & `datacube-1.8.9/tests/data/sample_tile_151_-29.tif`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/data/test.nc` & `datacube-1.8.9/tests/data/test.nc`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/data/test.tif` & `datacube-1.8.9/tests/data/test.tif`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/drivers/fail_drivers/setup.py` & `datacube-1.8.9/tests/drivers/fail_drivers/setup.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/drivers/test_rio_reader.py` & `datacube-1.8.9/tests/drivers/test_rio_reader.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/index/test_api_index_dataset.py` & `datacube-1.8.9/tests/index/test_api_index_dataset.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/index/test_fields.py` & `datacube-1.8.9/tests/index/test_fields.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/index/test_hl_index.py` & `datacube-1.8.9/tests/index/test_hl_index.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/index/test_query.py` & `datacube-1.8.9/tests/index/test_query.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/index/test_validate_dataset_type.py` & `datacube-1.8.9/tests/index/test_validate_dataset_type.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/scripts/test_search_tool.py` & `datacube-1.8.9/tests/scripts/test_search_tool.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/storage/test_base.py` & `datacube-1.8.9/tests/storage/test_base.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/storage/test_netcdfwriter.py` & `datacube-1.8.9/tests/storage/test_netcdfwriter.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/storage/test_storage.py` & `datacube-1.8.9/tests/storage/test_storage.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/storage/test_storage_load.py` & `datacube-1.8.9/tests/storage/test_storage_load.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/storage/test_storage_read.py` & `datacube-1.8.9/tests/storage/test_storage_read.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/test_3d.py` & `datacube-1.8.9/tests/test_3d.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/test_concurrent_executor.py` & `datacube-1.8.9/tests/test_concurrent_executor.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/test_config.py` & `datacube-1.8.9/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/test_driver.py` & `datacube-1.8.9/tests/test_driver.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/test_dynamic_db_passwd.py` & `datacube-1.8.9/tests/test_dynamic_db_passwd.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/test_eo3.py` & `datacube-1.8.9/tests/test_eo3.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/test_gbox_ops.py` & `datacube-1.8.9/tests/test_gbox_ops.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/test_geometry.py` & `datacube-1.8.9/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/test_load_data.py` & `datacube-1.8.9/tests/test_load_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,18 @@
     mm = ['aa']
     mm = [ds.type.measurements[k] for k in mm]
 
     ds_data = Datacube.load_data(sources, gbox, mm, patch_url=url_mangler)
     assert ds_data.aa.nodata == nodata
     np.testing.assert_array_equal(aa, ds_data.aa.values[0])
 
+    ds_data = Datacube.load_data(sources, gbox, mm, dask_chunks={'x': 8, 'y': 8}, patch_url=url_mangler)
+    assert ds_data.aa.nodata == nodata
+    np.testing.assert_array_equal(aa, ds_data.aa.values[0])
+
     custom_fuser_call_count = 0
 
     def custom_fuser(dest, delta):
         nonlocal custom_fuser_call_count
         custom_fuser_call_count += 1
         dest[:] += delta
```

### Comparing `datacube-1.8.8rc1/tests/test_metadata_fields.py` & `datacube-1.8.9/tests/test_metadata_fields.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/test_model.py` & `datacube-1.8.9/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/test_testutils.py` & `datacube-1.8.9/tests/test_testutils.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/test_utils_aws.py` & `datacube-1.8.9/tests/test_utils_aws.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/test_utils_changes.py` & `datacube-1.8.9/tests/test_utils_changes.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/test_utils_cog.py` & `datacube-1.8.9/tests/test_utils_cog.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/test_utils_dask.py` & `datacube-1.8.9/tests/test_utils_dask.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/test_utils_dates.py` & `datacube-1.8.9/tests/test_utils_dates.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/test_utils_docs.py` & `datacube-1.8.9/tests/test_utils_docs.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/test_utils_generic.py` & `datacube-1.8.9/tests/test_utils_generic.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/test_utils_other.py` & `datacube-1.8.9/tests/test_utils_other.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/test_utils_rio.py` & `datacube-1.8.9/tests/test_utils_rio.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/test_warp.py` & `datacube-1.8.9/tests/test_warp.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/test_xarray_extension.py` & `datacube-1.8.9/tests/test_xarray_extension.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/ui/test_common.py` & `datacube-1.8.9/tests/ui/test_common.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/ui/test_expression_parsing.py` & `datacube-1.8.9/tests/ui/test_expression_parsing.py`

 * *Files identical despite different names*

### Comparing `datacube-1.8.8rc1/tests/ui/test_task_app.py` & `datacube-1.8.9/tests/ui/test_task_app.py`

 * *Files identical despite different names*

