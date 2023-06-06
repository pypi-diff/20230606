# Comparing `tmp/swh.graphql-0.0.94.tar.gz` & `tmp/swh.graphql-0.0.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swh.graphql-0.0.94.tar", last modified: Fri May 26 08:58:56 2023, max compression
+gzip compressed data, was "dist/swh.graphql-0.0.95.tar", last modified: Tue Jun  6 15:45:15 2023, max compression
```

## Comparing `swh.graphql-0.0.94.tar` & `swh.graphql-0.0.95.tar`

### file list

```diff
@@ -1,132 +1,134 @@
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/
--rw-r--r--   0 jenkins    (115) docker     (999)      149 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      848 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/AUTHORS
--rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) docker     (999)      367 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/Dockerfile
--rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/LICENSE
--rw-r--r--   0 jenkins    (115) docker     (999)      109 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/MANIFEST.in
--rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)      758 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/Makefile.local
--rw-r--r--   0 jenkins    (115) docker     (999)     5627 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     4722 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/README.md
--rw-r--r--   0 jenkins    (115) docker     (999)      216 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/docker-compose-dev.yml
--rw-r--r--   0 jenkins    (115) docker     (999)      333 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/docker-compose-staging.yml
--rw-r--r--   0 jenkins    (115) docker     (999)      160 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/docker-compose.yml
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/docs/
--rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/docs/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/docs/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     4722 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/docs/README.rst
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/docs/_static/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/docs/_templates/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/docs/conf.py
--rw-r--r--   0 jenkins    (115) docker     (999)      236 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/docs/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      316 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/mypy.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/pyproject.toml
--rw-r--r--   0 jenkins    (115) docker     (999)       62 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/pytest.ini
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/requirements-dev.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      196 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       32 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/requirements-test.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       52 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/requirements.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/setup.cfg
--rw-r--r--   0 jenkins    (115) docker     (999)     2287 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/setup.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh/graphql/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1892 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/app.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh/graphql/backends/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/backends/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7564 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/backends/archive.py
--rw-r--r--   0 jenkins    (115) docker     (999)      791 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/backends/search.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh/graphql/client/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/client/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5116 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/client/explorer.html
--rw-r--r--   0 jenkins    (115) docker     (999)      747 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/client/view.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh/graphql/config/
--rw-r--r--   0 jenkins    (115) docker     (999)      424 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/config/dev.yml
--rw-r--r--   0 jenkins    (115) docker     (999)      475 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/config/staging.yml
--rw-r--r--   0 jenkins    (115) docker     (999)      276 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/config/test.yml
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh/graphql/errors/
--rw-r--r--   0 jenkins    (115) docker     (999)      604 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/errors/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)      873 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/errors/errors.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1788 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/errors/handlers.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh/graphql/middlewares/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/middlewares/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1054 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/middlewares/logger.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh/graphql/resolvers/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/resolvers/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6228 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/resolvers/base_connection.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3036 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/resolvers/base_node.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4129 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/resolvers/content.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2147 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/resolvers/directory.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2313 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/resolvers/directory_entry.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2194 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/resolvers/origin.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1974 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/resolvers/person.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1919 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/resolvers/release.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5128 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/resolvers/resolver_factory.py
--rw-r--r--   0 jenkins    (115) docker     (999)    11486 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/resolvers/resolvers.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3633 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/resolvers/revision.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1209 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/resolvers/scalars.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1369 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/resolvers/search.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3435 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/resolvers/snapshot.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4202 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/resolvers/snapshot_branch.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1739 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/resolvers/swhid.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3030 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/resolvers/target.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2141 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/resolvers/visit.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2142 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/resolvers/visit_status.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh/graphql/schema/
--rw-r--r--   0 jenkins    (115) docker     (999)    19570 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/schema/schema.graphql
--rw-r--r--   0 jenkins    (115) docker     (999)     4277 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/server.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh/graphql/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2821 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/conftest.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7809 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/data.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh/graphql/tests/functional/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/functional/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     8848 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/functional/test_branch_connection.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7427 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/functional/test_content.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2666 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/functional/test_directory.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6083 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/functional/test_directory_entry.py
--rw-r--r--   0 jenkins    (115) docker     (999)      618 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/functional/test_errors.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3387 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/functional/test_logger.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1647 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/functional/test_origin_connection.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4815 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/functional/test_origin_node.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5388 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/functional/test_pagination.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4468 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/functional/test_query_cost.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5877 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/functional/test_release_node.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6304 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/functional/test_revision.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1740 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/functional/test_search.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1668 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/functional/test_snapshot_node.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4364 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/functional/test_swhid_resolve.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5259 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/functional/test_visit_node.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2706 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/functional/test_visit_status.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1289 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/functional/utils.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh/graphql/tests/unit/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/unit/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh/graphql/tests/unit/backends/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/unit/backends/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)      129 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/unit/backends/test_archive.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh/graphql/tests/unit/errors/
--rw-r--r--   0 jenkins    (115) docker     (999)     2022 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/unit/errors/test_errors.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh/graphql/tests/unit/resolvers/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/unit/resolvers/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)      874 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/unit/resolvers/test_resolver_factory.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3270 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/unit/resolvers/test_resolvers.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1097 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/unit/resolvers/test_scalars.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1056 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/unit/test_server.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh/graphql/tests/unit/utils/
--rw-r--r--   0 jenkins    (115) docker     (999)     2547 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/tests/unit/utils/test_utils.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh/graphql/utils/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/utils/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2102 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/swh/graphql/utils/utils.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh.graphql.egg-info/
--rw-r--r--   0 jenkins    (115) docker     (999)     5627 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh.graphql.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     3408 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh.graphql.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh.graphql.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      171 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh.graphql.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-05-26 08:58:56.000000 swh.graphql-0.0.94/swh.graphql.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1483 2023-05-26 08:58:54.000000 swh.graphql-0.0.94/tox.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/
+-rw-r--r--   0 jenkins    (115) docker     (999)      149 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      848 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/AUTHORS
+-rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) docker     (999)      367 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/Dockerfile
+-rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/LICENSE
+-rw-r--r--   0 jenkins    (115) docker     (999)      109 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/MANIFEST.in
+-rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)      758 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/Makefile.local
+-rw-r--r--   0 jenkins    (115) docker     (999)     5627 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     4722 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/README.md
+-rw-r--r--   0 jenkins    (115) docker     (999)      216 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/docker-compose-dev.yml
+-rw-r--r--   0 jenkins    (115) docker     (999)      333 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/docker-compose-staging.yml
+-rw-r--r--   0 jenkins    (115) docker     (999)      160 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/docker-compose.yml
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/docs/
+-rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/docs/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     4722 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/docs/README.rst
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/docs/_static/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/docs/_templates/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/docs/conf.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      236 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/docs/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      316 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/mypy.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/pyproject.toml
+-rw-r--r--   0 jenkins    (115) docker     (999)       62 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/pytest.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/requirements-dev.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      196 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       32 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       52 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/requirements.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/setup.cfg
+-rw-r--r--   0 jenkins    (115) docker     (999)     2287 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/setup.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh/graphql/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1916 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/app.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh/graphql/backends/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/backends/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7570 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/backends/archive.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      791 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/backends/search.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh/graphql/client/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/client/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5116 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/client/explorer.html
+-rw-r--r--   0 jenkins    (115) docker     (999)      747 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/client/view.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh/graphql/config/
+-rw-r--r--   0 jenkins    (115) docker     (999)      453 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/config/dev.yml
+-rw-r--r--   0 jenkins    (115) docker     (999)      506 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/config/staging.yml
+-rw-r--r--   0 jenkins    (115) docker     (999)      307 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/config/test.yml
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh/graphql/errors/
+-rw-r--r--   0 jenkins    (115) docker     (999)      604 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/errors/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      873 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/errors/errors.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1788 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/errors/handlers.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh/graphql/middlewares/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/middlewares/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1054 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/middlewares/logger.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh/graphql/resolvers/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/resolvers/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6228 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/resolvers/base_connection.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3036 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/resolvers/base_node.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3768 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/resolvers/content.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      984 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/resolvers/content_data.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2147 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/resolvers/directory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2544 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/resolvers/directory_entry.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2194 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/resolvers/origin.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1974 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/resolvers/person.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1919 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/resolvers/release.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5211 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/resolvers/resolver_factory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    11757 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/resolvers/resolvers.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3633 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/resolvers/revision.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1209 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/resolvers/scalars.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1369 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/resolvers/search.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3435 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/resolvers/snapshot.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4202 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/resolvers/snapshot_branch.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1739 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/resolvers/swhid.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3030 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/resolvers/target.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2141 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/resolvers/visit.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2142 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/resolvers/visit_status.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh/graphql/schema/
+-rw-r--r--   0 jenkins    (115) docker     (999)    19943 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/schema/schema.graphql
+-rw-r--r--   0 jenkins    (115) docker     (999)     4367 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/server.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh/graphql/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2821 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/conftest.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     8119 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/data.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh/graphql/tests/functional/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/functional/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     8848 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/functional/test_branch_connection.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7427 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/functional/test_content.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1798 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/functional/test_content_data_node.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2666 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/functional/test_directory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7115 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/functional/test_directory_entry.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      618 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/functional/test_errors.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3387 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/functional/test_logger.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1647 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/functional/test_origin_connection.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4815 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/functional/test_origin_node.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5388 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/functional/test_pagination.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4468 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/functional/test_query_cost.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5877 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/functional/test_release_node.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6304 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/functional/test_revision.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1740 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/functional/test_search.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1668 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/functional/test_snapshot_node.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4364 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/functional/test_swhid_resolve.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5259 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/functional/test_visit_node.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2706 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/functional/test_visit_status.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1289 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/functional/utils.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh/graphql/tests/unit/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/unit/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh/graphql/tests/unit/backends/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/unit/backends/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      129 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/unit/backends/test_archive.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh/graphql/tests/unit/errors/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2022 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/unit/errors/test_errors.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh/graphql/tests/unit/resolvers/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/unit/resolvers/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      874 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/unit/resolvers/test_resolver_factory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3270 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/unit/resolvers/test_resolvers.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1097 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/unit/resolvers/test_scalars.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1056 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/unit/test_server.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh/graphql/tests/unit/utils/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2547 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/tests/unit/utils/test_utils.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh/graphql/utils/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/utils/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2102 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/swh/graphql/utils/utils.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh.graphql.egg-info/
+-rw-r--r--   0 jenkins    (115) docker     (999)     5627 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh.graphql.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     3501 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh.graphql.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh.graphql.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      171 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh.graphql.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-06-06 15:45:15.000000 swh.graphql-0.0.95/swh.graphql.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1483 2023-06-06 15:45:14.000000 swh.graphql-0.0.95/tox.ini
```

### Comparing `swh.graphql-0.0.94/.pre-commit-config.yaml` & `swh.graphql-0.0.95/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/CODE_OF_CONDUCT.md` & `swh.graphql-0.0.95/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/LICENSE` & `swh.graphql-0.0.95/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/Makefile.local` & `swh.graphql-0.0.95/Makefile.local`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/PKG-INFO` & `swh.graphql-0.0.95/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.graphql
-Version: 0.0.94
+Version: 0.0.95
 Summary: Software Heritage GraphQL Apis
 Home-page: https://forge.softwareheritage.org/diffusion/DGQL
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-graphql
```

### Comparing `swh.graphql-0.0.94/README.md` & `swh.graphql-0.0.95/README.md`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/docs/README.rst` & `swh.graphql-0.0.95/docs/README.rst`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/setup.py` & `swh.graphql-0.0.95/setup.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/app.py` & `swh.graphql-0.0.95/swh/graphql/app.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     resolvers.visit_status,
     resolvers.snapshot,
     resolvers.snapshot_branch,
     resolvers.revision,
     resolvers.release,
     resolvers.directory,
     resolvers.directory_entry,
+    resolvers.content,
     resolvers.branch_target,
     resolvers.branch_target_node,
     resolvers.release_target,
     resolvers.release_target_node,
     resolvers.directory_entry_target,
     resolvers.directory_entry_target_node,
     resolvers.resolve_swhid_result,
@@ -44,20 +45,20 @@
     scalars.id_scalar,
     scalars.datetime_scalar,
     scalars.swhid_scalar,
 )
 
 
 def validation_rules(context, document, data):
-    from .server import graphql_cfg
+    from .server import get_config
 
     if context["request"].user.is_authenticated:
-        max_query_cost = graphql_cfg["max_query_cost"]["user"]
+        max_query_cost = get_config()["max_query_cost"]["user"]
     else:
-        max_query_cost = graphql_cfg["max_query_cost"]["anonymous"]
+        max_query_cost = get_config()["max_query_cost"]["anonymous"]
 
     if max_query_cost:
         return [
             cost_validator(maximum_cost=max_query_cost, variables=data.get("variables"))
         ]
     # no limit is applied when max_query_cost is set to 0 or None
     return None
```

### Comparing `swh.graphql-0.0.94/swh/graphql/backends/archive.py` & `swh.graphql-0.0.95/swh/graphql/backends/archive.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     Directory,
     DirectoryEntry,
     Origin,
     OriginVisit,
     OriginVisitStatus,
     Release,
     Revision,
+    Sha1,
     Sha1Git,
     Snapshot,
     SnapshotBranch,
 )
 from swh.model.swhids import ObjectType
 from swh.storage.algos.origin import origin_get_latest_visit_status
 from swh.storage.algos.snapshot import snapshot_resolve_branch_target
@@ -184,16 +185,16 @@
             ObjectType.SNAPSHOT: self.storage.snapshot_missing,
         }
         return not list(mapping[object_type]([object_id]))
 
     def get_contents(self, hashes: HashDict) -> List[Content]:
         return self.storage.content_find(content=hashes)
 
-    # def get_content_data(self, content_sha1: Sha1) -> Optional[bytes]:
-    #     return self.storage.content_get_data(content=content_sha1)
+    def get_content_data(self, content_sha1: Sha1) -> Optional[bytes]:
+        return self.storage.content_get_data(content=content_sha1)
 
     def get_branch_target(
         self,
         snapshot_id: Sha1Git,
         branch_obj: Optional[SnapshotBranch],
         max_length: int,
     ) -> Tuple[Optional[SnapshotBranch], List[bytes]]:
```

### Comparing `swh.graphql-0.0.94/swh/graphql/backends/search.py` & `swh.graphql-0.0.95/swh/graphql/backends/search.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/client/explorer.html` & `swh.graphql-0.0.95/swh/graphql/client/explorer.html`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/client/view.py` & `swh.graphql-0.0.95/swh/graphql/client/view.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/errors/__init__.py` & `swh.graphql-0.0.95/swh/graphql/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/errors/errors.py` & `swh.graphql-0.0.95/swh/graphql/errors/errors.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/errors/handlers.py` & `swh.graphql-0.0.95/swh/graphql/errors/handlers.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/middlewares/logger.py` & `swh.graphql-0.0.95/swh/graphql/middlewares/logger.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/resolvers/base_connection.py` & `swh.graphql-0.0.95/swh/graphql/resolvers/base_connection.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/resolvers/base_node.py` & `swh.graphql-0.0.95/swh/graphql/resolvers/base_node.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/resolvers/content.py` & `swh.graphql-0.0.95/swh/graphql/resolvers/content.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,24 +37,14 @@
         return {k: v.hex() for (k, v) in self._node.hashes().items()}
 
     @property
     def id(self):
         return self._node.sha1_git
 
     @property
-    def data(self):
-        # FIXME, return a Node object
-        # FIXME, add more ways to retrieve data like binary string
-        archive_url = "https://archive.softwareheritage.org/api/1/"
-        content_sha1 = self._node.hashes()["sha1"]
-        return {
-            "url": f"{archive_url}content/sha1:{content_sha1.hex()}/raw/",
-        }
-
-    @property
     def mimeType(self):
         # FIXME, fetch data from the indexers
         return None
 
     @property
     def language(self):
         # FIXME, fetch data from the indexers
```

### Comparing `swh.graphql-0.0.94/swh/graphql/resolvers/directory.py` & `swh.graphql-0.0.95/swh/graphql/resolvers/directory.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/resolvers/directory_entry.py` & `swh.graphql-0.0.95/swh/graphql/resolvers/directory_entry.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,24 +49,28 @@
 
     from .directory import BaseDirectoryNode
 
     obj: BaseDirectoryNode
 
     _node_class = BaseDirectoryEntryNode
 
+    def _name_filter(self, dir_entry_name, name_include):
+        if not self.kwargs.get("caseSensitive", False):
+            return name_include.casefold() in dir_entry_name.decode().casefold()
+        return name_include in dir_entry_name.decode()
+
     def _get_connection_data(self) -> ConnectionData:
         # FIXME, using dummy(local) pagination, move pagination to backend
         # STORAGE-TODO
         entries: List[DirectoryEntry] = self.archive.get_directory_entries(
             self.obj.swhid.object_id
         ).results
-        name_include = self.kwargs.get("nameInclude")
-        if name_include is not None:
+        if self.kwargs.get("nameInclude") is not None:
             # STORAGE-TODO, move this filter to swh-storage
             entries = [
-                x
-                for x in entries
-                if name_include.casefold() in x.name.decode().casefold()
+                entry
+                for entry in entries
+                if self._name_filter(entry.name, self.kwargs.get("nameInclude"))
             ]
         return utils.get_local_paginated_data(
             entries, self._get_first_arg(), self._get_after_arg()
         )
```

### Comparing `swh.graphql-0.0.94/swh/graphql/resolvers/origin.py` & `swh.graphql-0.0.95/swh/graphql/resolvers/origin.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/resolvers/person.py` & `swh.graphql-0.0.95/swh/graphql/resolvers/person.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/resolvers/release.py` & `swh.graphql-0.0.95/swh/graphql/resolvers/release.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/resolvers/resolver_factory.py` & `swh.graphql-0.0.95/swh/graphql/resolvers/resolver_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from .base_node import BaseNode
 from .content import (
     ContentbyHashesNode,
     ContentHashList,
     ContentSwhidList,
     TargetContentNode,
 )
+from .content_data import ContentDataNode
 from .directory import DirectoryNode, RevisionDirectoryNode, TargetDirectoryNode
 from .directory_entry import DirectoryEntryConnection, DirectoryEntryNode
 from .origin import OriginConnection, OriginNode, TargetOriginNode
 from .person import ReleaseAuthorList, RevisionAuthorList, RevisionCommitterList
 from .release import ReleaseNode, TargetReleaseNode
 from .revision import (
     LogRevisionConnection,
@@ -57,14 +58,15 @@
         "snapshot": SnapshotNode,
         "revision": RevisionNode,
         "revision-directory": RevisionDirectoryNode,
         "release": ReleaseNode,
         "directory": DirectoryNode,
         "directory-entry": DirectoryEntryNode,
         "content-by-hashes": ContentbyHashesNode,
+        "content-data": ContentDataNode,
         "generic-target": TargetNode,
         "branch-target": BranchTargetNode,
         "target-origin": TargetOriginNode,
         "target-snapshot": TargetSnapshotNode,
         "target-revision": TargetRevisionNode,
         "target-release": TargetReleaseNode,
         "target-directory": TargetDirectoryNode,
```

### Comparing `swh.graphql-0.0.94/swh/graphql/resolvers/resolvers.py` & `swh.graphql-0.0.95/swh/graphql/resolvers/resolvers.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 visit_status: ObjectType = ObjectType("VisitStatus")
 snapshot: ObjectType = ObjectType("Snapshot")
 snapshot_branch: ObjectType = ObjectType("Branch")
 revision: ObjectType = ObjectType("Revision")
 release: ObjectType = ObjectType("Release")
 directory: ObjectType = ObjectType("Directory")
 directory_entry: ObjectType = ObjectType("DirectoryEntry")
+content: ObjectType = ObjectType("Content")
 binary_string: ObjectType = ObjectType("BinaryString")
 date: ObjectType = ObjectType("Date")
 branch_target: ObjectType = ObjectType("BranchTarget")
 release_target: ObjectType = ObjectType("ReleaseTarget")
 directory_entry_target: ObjectType = ObjectType("DirectoryEntryTarget")
 origin_search_result: ObjectType = ObjectType("OriginSearchResult")
 
@@ -182,14 +183,21 @@
 @query.field("contentByHashes")
 def content_by_hashes_resolver(
     obj: None, info: GraphQLResolveInfo, **kw
 ) -> rs.content.ContentbyHashesNode:
     return NodeObjectFactory.create("content-by-hashes", obj, info, **kw)
 
 
+@content.field("data")
+def content_data_resolver(
+    obj: rs.content.BaseContentNode, info: GraphQLResolveInfo, **kw
+) -> rs.content_data.ContentDataNode:
+    return NodeObjectFactory.create("content-data", obj, info, **kw)
+
+
 @origin_search_result.field("node")
 def origin_search_node_resolver(
     obj: None, info: GraphQLResolveInfo, **kw
 ) -> rs.origin.TargetOriginNode:
     return NodeObjectFactory.create("target-origin", obj, info, **kw)
```

### Comparing `swh.graphql-0.0.94/swh/graphql/resolvers/revision.py` & `swh.graphql-0.0.95/swh/graphql/resolvers/revision.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/resolvers/scalars.py` & `swh.graphql-0.0.95/swh/graphql/resolvers/scalars.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/resolvers/search.py` & `swh.graphql-0.0.95/swh/graphql/resolvers/search.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/resolvers/snapshot.py` & `swh.graphql-0.0.95/swh/graphql/resolvers/snapshot.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/resolvers/snapshot_branch.py` & `swh.graphql-0.0.95/swh/graphql/resolvers/snapshot_branch.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/resolvers/swhid.py` & `swh.graphql-0.0.95/swh/graphql/resolvers/swhid.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/resolvers/target.py` & `swh.graphql-0.0.95/swh/graphql/resolvers/target.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/resolvers/visit.py` & `swh.graphql-0.0.95/swh/graphql/resolvers/visit.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/resolvers/visit_status.py` & `swh.graphql-0.0.95/swh/graphql/resolvers/visit_status.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/schema/schema.graphql` & `swh.graphql-0.0.95/swh/graphql/schema/schema.graphql`

 * *Files 4% similar despite different names*

```diff
@@ -921,14 +921,19 @@
     """
     after: String
 
     """
     Filter by entry name
     """
     nameInclude: String
+
+    """
+    Case-sensitivity of the nameInclude argument, False by default
+    """
+    caseSensitive: Boolean = false
   ): DirectoryEntryConnection @cost(complexity: 2, multipliers: ["first"]) # pagination is local, hence adding a higher value for cost
 }
 
 """
 An object with different content hashes
 """
 type ContentHashes {
@@ -942,14 +947,20 @@
 Object with different content data representations
 """
 type ContentData {
   """
   URL to download the file data
   """
   url: String
+
+  """
+  Raw content data
+  This is available only for contents with a reasonable size, use the url field to download larger files otherwise.
+  """
+  raw: BinaryString @cost(complexity: 5)  # contents could be as long as 10000 bytes, hence a higher cost
 }
 
 type ContentMimeType {
   """
   Detected content encoding
   """
   encoding: String
```

### Comparing `swh.graphql-0.0.94/swh/graphql/server.py` & `swh.graphql-0.0.95/swh/graphql/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,22 @@
 def get_search() -> SearchInterface:
     global search
     if not search:
         search = get_swh_search(**graphql_cfg["search"])
     return search
 
 
+def get_config() -> Dict[str, Any]:
+    global graphql_cfg
+    if not graphql_cfg:
+        config_path = os.environ.get("SWH_CONFIG_FILENAME")
+        graphql_cfg = load_and_check_config(config_path)
+    return graphql_cfg
+
+
 class AnonymousAuthBackend(AuthenticationBackend):
     async def authenticate(self, conn):
         return AuthCredentials(["anonymous"]), UnauthenticatedUser()
 
 
 def load_and_check_config(config_path: Optional[str]) -> Dict[str, Any]:
     """Check the minimal configuration is set to run the api or raise an
@@ -85,20 +93,15 @@
     SWH_CONFIG_FILENAME environment variable defines the
     configuration path to load.
     """
     from .app import schema, validation_rules
     from .errors import format_error, on_auth_error
     from .middlewares.logger import LogMiddleware
 
-    global graphql_cfg
-
-    if not graphql_cfg:
-        config_path = os.environ.get("SWH_CONFIG_FILENAME")
-        graphql_cfg = load_and_check_config(config_path)
-
+    graphql_cfg = get_config()
     ariadne_app = GraphQL(
         schema,
         debug=graphql_cfg["debug"],
         introspection=graphql_cfg["introspection"],
         validation_rules=validation_rules,
         error_formatter=format_error,
     )
```

### Comparing `swh.graphql-0.0.94/swh/graphql/tests/conftest.py` & `swh.graphql-0.0.95/swh/graphql/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/tests/data.py` & `swh.graphql-0.0.95/swh/graphql/tests/data.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import datetime
 
 from swh.model.model import (
+    Content,
     Directory,
     DirectoryEntry,
+    MultiHash,
     ObjectType,
     OriginVisitStatus,
     Release,
     Revision,
     RevisionType,
     Snapshot,
     SnapshotBranch,
@@ -250,21 +252,33 @@
                     target_type=TargetType.ALIAS, target=b"target/alias1"
                 ),
             },
         ),
     ]
 
 
+def get_too_big_contents():
+    return [
+        Content(
+            length=20000,
+            data="too big data".encode(),
+            status="visible",
+            **MultiHash.from_data("too big data".encode()).digest(),
+        )
+    ]
+
+
 GRAPHQL_EXTRA_TEST_OBJECTS = {
     "snapshot": get_snapshots_with_multiple_alias(),
     "release": get_releases_with_target() + get_releases_with_empty_target(),
     "revision": get_revisions_with_parents() + get_revisions_with_none_date(),
     "directory": get_directories_with_nested_path()
     + get_directories_with_special_name_entries(),
     "origin_visit_status": get_visit_with_multiple_status(),
+    "content": get_too_big_contents(),
 }
 
 
 def populate_dummy_data(storage):
     for object_type, objects in swh_model_data.TEST_OBJECTS.items():
         method = getattr(storage, object_type + "_add")
         method(objects)
```

### Comparing `swh.graphql-0.0.94/swh/graphql/tests/functional/test_branch_connection.py` & `swh.graphql-0.0.95/swh/graphql/tests/functional/test_branch_connection.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/tests/functional/test_content.py` & `swh.graphql-0.0.95/swh/graphql/tests/functional/test_content.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/tests/functional/test_directory.py` & `swh.graphql-0.0.95/swh/graphql/tests/functional/test_directory.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/tests/functional/test_directory_entry.py` & `swh.graphql-0.0.95/swh/graphql/tests/functional/test_directory_entry.py`

 * *Files 10% similar despite different names*

```diff
@@ -206,7 +206,46 @@
     )
     assert data["directory"]["entries"]["nodes"][0] == {
         "name": {"text": "ßßétEÉt"},
         "target": {
             "type": "content",
         },
     }
+
+
+def test_directory_entry_connection_filter_by_path_case_sensitive(client):
+    directory = get_directories()[1]
+    query_str = """
+    query getDirectory($swhid: SWHID!, $nameInclude: String, $caseSensitive: Boolean) {
+      directory(swhid: $swhid) {
+        entries(nameInclude: $nameInclude, caseSensitive: $caseSensitive) {
+          nodes {
+            name {
+              text
+            }
+            target {
+              type
+            }
+          }
+        }
+      }
+    }
+    """
+    data, _ = utils.get_query_response(
+        client,
+        query_str,
+        swhid=str(directory.swhid()),
+        nameInclude="diR",
+        caseSensitive=False,
+    )
+    assert data["directory"]["entries"]["nodes"] == [
+        {"name": {"text": "dir1"}, "target": {"type": "directory"}}
+    ]
+
+    data, _ = utils.get_query_response(
+        client,
+        query_str,
+        swhid=str(directory.swhid()),
+        nameInclude="diR",
+        caseSensitive=True,
+    )
+    assert data["directory"]["entries"]["nodes"] == []
```

### Comparing `swh.graphql-0.0.94/swh/graphql/tests/functional/test_errors.py` & `swh.graphql-0.0.95/swh/graphql/tests/functional/test_errors.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/tests/functional/test_logger.py` & `swh.graphql-0.0.95/swh/graphql/tests/functional/test_logger.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/tests/functional/test_origin_connection.py` & `swh.graphql-0.0.95/swh/graphql/tests/functional/test_origin_connection.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/tests/functional/test_origin_node.py` & `swh.graphql-0.0.95/swh/graphql/tests/functional/test_origin_node.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/tests/functional/test_pagination.py` & `swh.graphql-0.0.95/swh/graphql/tests/functional/test_pagination.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/tests/functional/test_query_cost.py` & `swh.graphql-0.0.95/swh/graphql/tests/functional/test_query_cost.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/tests/functional/test_release_node.py` & `swh.graphql-0.0.95/swh/graphql/tests/functional/test_release_node.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/tests/functional/test_revision.py` & `swh.graphql-0.0.95/swh/graphql/tests/functional/test_revision.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/tests/functional/test_search.py` & `swh.graphql-0.0.95/swh/graphql/tests/functional/test_search.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/tests/functional/test_snapshot_node.py` & `swh.graphql-0.0.95/swh/graphql/tests/functional/test_snapshot_node.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/tests/functional/test_swhid_resolve.py` & `swh.graphql-0.0.95/swh/graphql/tests/functional/test_swhid_resolve.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/tests/functional/test_visit_node.py` & `swh.graphql-0.0.95/swh/graphql/tests/functional/test_visit_node.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/tests/functional/test_visit_status.py` & `swh.graphql-0.0.95/swh/graphql/tests/functional/test_visit_status.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/tests/functional/utils.py` & `swh.graphql-0.0.95/swh/graphql/tests/functional/utils.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/tests/unit/errors/test_errors.py` & `swh.graphql-0.0.95/swh/graphql/tests/unit/errors/test_errors.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/tests/unit/resolvers/test_resolver_factory.py` & `swh.graphql-0.0.95/swh/graphql/tests/unit/resolvers/test_resolver_factory.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/tests/unit/resolvers/test_resolvers.py` & `swh.graphql-0.0.95/swh/graphql/tests/unit/resolvers/test_resolvers.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/tests/unit/resolvers/test_scalars.py` & `swh.graphql-0.0.95/swh/graphql/tests/unit/resolvers/test_scalars.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/tests/unit/test_server.py` & `swh.graphql-0.0.95/swh/graphql/tests/unit/test_server.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/tests/unit/utils/test_utils.py` & `swh.graphql-0.0.95/swh/graphql/tests/unit/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh/graphql/utils/utils.py` & `swh.graphql-0.0.95/swh/graphql/utils/utils.py`

 * *Files identical despite different names*

### Comparing `swh.graphql-0.0.94/swh.graphql.egg-info/PKG-INFO` & `swh.graphql-0.0.95/swh.graphql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.graphql
-Version: 0.0.94
+Version: 0.0.95
 Summary: Software Heritage GraphQL Apis
 Home-page: https://forge.softwareheritage.org/diffusion/DGQL
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-graphql
```

### Comparing `swh.graphql-0.0.94/swh.graphql.egg-info/SOURCES.txt` & `swh.graphql-0.0.95/swh.graphql.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 swh/graphql/errors/handlers.py
 swh/graphql/middlewares/__init__.py
 swh/graphql/middlewares/logger.py
 swh/graphql/resolvers/__init__.py
 swh/graphql/resolvers/base_connection.py
 swh/graphql/resolvers/base_node.py
 swh/graphql/resolvers/content.py
+swh/graphql/resolvers/content_data.py
 swh/graphql/resolvers/directory.py
 swh/graphql/resolvers/directory_entry.py
 swh/graphql/resolvers/origin.py
 swh/graphql/resolvers/person.py
 swh/graphql/resolvers/release.py
 swh/graphql/resolvers/resolver_factory.py
 swh/graphql/resolvers/resolvers.py
@@ -75,14 +76,15 @@
 swh/graphql/schema/schema.graphql
 swh/graphql/tests/__init__.py
 swh/graphql/tests/conftest.py
 swh/graphql/tests/data.py
 swh/graphql/tests/functional/__init__.py
 swh/graphql/tests/functional/test_branch_connection.py
 swh/graphql/tests/functional/test_content.py
+swh/graphql/tests/functional/test_content_data_node.py
 swh/graphql/tests/functional/test_directory.py
 swh/graphql/tests/functional/test_directory_entry.py
 swh/graphql/tests/functional/test_errors.py
 swh/graphql/tests/functional/test_logger.py
 swh/graphql/tests/functional/test_origin_connection.py
 swh/graphql/tests/functional/test_origin_node.py
 swh/graphql/tests/functional/test_pagination.py
```

### Comparing `swh.graphql-0.0.94/tox.ini` & `swh.graphql-0.0.95/tox.ini`

 * *Files identical despite different names*

