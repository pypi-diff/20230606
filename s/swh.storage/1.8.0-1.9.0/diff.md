# Comparing `tmp/swh.storage-1.8.0.tar.gz` & `tmp/swh.storage-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swh.storage-1.8.0.tar", last modified: Wed Feb 15 11:35:47 2023, max compression
+gzip compressed data, was "dist/swh.storage-1.9.0.tar", last modified: Mon Mar  6 13:52:23 2023, max compression
```

## Comparing `swh.storage-1.8.0.tar` & `swh.storage-1.9.0.tar`

### file list

```diff
@@ -1,369 +1,369 @@
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-15 11:35:47.000000 swh.storage-1.8.0/
--rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-02-15 11:35:45.000000 swh.storage-1.8.0/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) docker     (999)      136 2023-02-15 11:35:45.000000 swh.storage-1.8.0/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      916 2023-02-15 11:35:45.000000 swh.storage-1.8.0/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-02-15 11:35:45.000000 swh.storage-1.8.0/AUTHORS
--rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-02-15 11:35:45.000000 swh.storage-1.8.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) docker     (999)       61 2023-02-15 11:35:45.000000 swh.storage-1.8.0/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-02-15 11:35:45.000000 swh.storage-1.8.0/LICENSE
--rw-r--r--   0 jenkins    (115) docker     (999)      242 2023-02-15 11:35:45.000000 swh.storage-1.8.0/MANIFEST.in
--rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-02-15 11:35:45.000000 swh.storage-1.8.0/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)       69 2023-02-15 11:35:45.000000 swh.storage-1.8.0/Makefile.local
--rw-r--r--   0 jenkins    (115) docker     (999)     6708 2023-02-15 11:35:47.000000 swh.storage-1.8.0/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     5761 2023-02-15 11:35:45.000000 swh.storage-1.8.0/README.md
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-15 11:35:47.000000 swh.storage-1.8.0/bin/
--rwxr-xr-x   0 jenkins    (115) docker     (999)     1240 2023-02-15 11:35:45.000000 swh.storage-1.8.0/bin/swh-storage-add-dir
--rw-r--r--   0 jenkins    (115) docker     (999)      323 2023-02-15 11:35:45.000000 swh.storage-1.8.0/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-15 11:35:47.000000 swh.storage-1.8.0/docs/
--rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-02-15 11:35:45.000000 swh.storage-1.8.0/docs/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)       63 2023-02-15 11:35:45.000000 swh.storage-1.8.0/docs/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)      530 2023-02-15 11:35:45.000000 swh.storage-1.8.0/docs/Makefile.local
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-15 11:35:47.000000 swh.storage-1.8.0/docs/_static/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-02-15 11:35:45.000000 swh.storage-1.8.0/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-15 11:35:47.000000 swh.storage-1.8.0/docs/_templates/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-02-15 11:35:45.000000 swh.storage-1.8.0/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) docker     (999)     2206 2023-02-15 11:35:45.000000 swh.storage-1.8.0/docs/archive-copies.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      143 2023-02-15 11:35:45.000000 swh.storage-1.8.0/docs/cli.rst
--rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-02-15 11:35:45.000000 swh.storage-1.8.0/docs/conf.py
--rw-r--r--   0 jenkins    (115) docker     (999)    12957 2023-02-15 11:35:45.000000 swh.storage-1.8.0/docs/extrinsic-metadata-specification.rst
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-15 11:35:47.000000 swh.storage-1.8.0/docs/images/
--rw-r--r--   0 jenkins    (115) docker     (999)       12 2023-02-15 11:35:45.000000 swh.storage-1.8.0/docs/images/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      335 2023-02-15 11:35:45.000000 swh.storage-1.8.0/docs/images/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     3031 2023-02-15 11:35:45.000000 swh.storage-1.8.0/docs/images/swh-archive-copies.dia
--rw-r--r--   0 jenkins    (115) docker     (999)     2965 2023-02-15 11:35:45.000000 swh.storage-1.8.0/docs/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      268 2023-02-15 11:35:45.000000 swh.storage-1.8.0/docs/sql-storage.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     1211 2023-02-15 11:35:45.000000 swh.storage-1.8.0/mypy.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-02-15 11:35:45.000000 swh.storage-1.8.0/pyproject.toml
--rw-r--r--   0 jenkins    (115) docker     (999)      424 2023-02-15 11:35:45.000000 swh.storage-1.8.0/pytest.ini
--rw-r--r--   0 jenkins    (115) docker     (999)       19 2023-02-15 11:35:45.000000 swh.storage-1.8.0/requirements-swh-journal.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       94 2023-02-15 11:35:45.000000 swh.storage-1.8.0/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      372 2023-02-15 11:35:45.000000 swh.storage-1.8.0/requirements-test.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      189 2023-02-15 11:35:45.000000 swh.storage-1.8.0/requirements.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-02-15 11:35:47.000000 swh.storage-1.8.0/setup.cfg
--rwxr-xr-x   0 jenkins    (115) docker     (999)     2469 2023-02-15 11:35:45.000000 swh.storage-1.8.0/setup.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-15 11:35:47.000000 swh.storage-1.8.0/sql/
--rw-r--r--   0 jenkins    (115) docker     (999)       26 2023-02-15 11:35:45.000000 swh.storage-1.8.0/sql/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)     1565 2023-02-15 11:35:45.000000 swh.storage-1.8.0/sql/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     1094 2023-02-15 11:35:45.000000 swh.storage-1.8.0/sql/TODO
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-15 11:35:47.000000 swh.storage-1.8.0/sql/bin/
--rwxr-xr-x   0 jenkins    (115) docker     (999)     1701 2023-02-15 11:35:45.000000 swh.storage-1.8.0/sql/bin/db-upgrade
--rwxr-xr-x   0 jenkins    (115) docker     (999)      538 2023-02-15 11:35:45.000000 swh.storage-1.8.0/sql/bin/dot_add_content
--rw-r--r--   0 jenkins    (115) docker     (999)     2023 2023-02-15 11:35:45.000000 swh.storage-1.8.0/sql/clusters.dot
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-15 11:35:47.000000 swh.storage-1.8.0/sql/doc/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-15 11:35:47.000000 swh.storage-1.8.0/sql/doc/json/
--rw-r--r--   0 jenkins    (115) docker     (999)        8 2023-02-15 11:35:45.000000 swh.storage-1.8.0/sql/doc/json/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      283 2023-02-15 11:35:45.000000 swh.storage-1.8.0/sql/doc/json/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)      223 2023-02-15 11:35:45.000000 swh.storage-1.8.0/sql/doc/json/entity.lister_metadata.schema.json
--rw-r--r--   0 jenkins    (115) docker     (999)      129 2023-02-15 11:35:45.000000 swh.storage-1.8.0/sql/doc/json/entity.metadata.schema.json
--rw-r--r--   0 jenkins    (115) docker     (999)      223 2023-02-15 11:35:45.000000 swh.storage-1.8.0/sql/doc/json/entity_history.lister_metadata.schema.json
--rw-r--r--   0 jenkins    (115) docker     (999)      137 2023-02-15 11:35:45.000000 swh.storage-1.8.0/sql/doc/json/entity_history.metadata.schema.json
--rw-r--r--   0 jenkins    (115) docker     (999)      631 2023-02-15 11:35:45.000000 swh.storage-1.8.0/sql/doc/json/fetch_history.result.schema.json
--rw-r--r--   0 jenkins    (115) docker     (999)      133 2023-02-15 11:35:45.000000 swh.storage-1.8.0/sql/doc/json/list_history.result.schema.json
--rw-r--r--   0 jenkins    (115) docker     (999)      141 2023-02-15 11:35:45.000000 swh.storage-1.8.0/sql/doc/json/listable_entity.list_params.schema.json
--rw-r--r--   0 jenkins    (115) docker     (999)      632 2023-02-15 11:35:45.000000 swh.storage-1.8.0/sql/doc/json/origin_visit.metadata.json
--rw-r--r--   0 jenkins    (115) docker     (999)      252 2023-02-15 11:35:45.000000 swh.storage-1.8.0/sql/doc/json/tool.tool_configuration.schema.json
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-15 11:35:47.000000 swh.storage-1.8.0/sql/json/
--rw-r--r--   0 jenkins    (115) docker     (999)        8 2023-02-15 11:35:45.000000 swh.storage-1.8.0/sql/json/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      283 2023-02-15 11:35:45.000000 swh.storage-1.8.0/sql/json/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)      223 2023-02-15 11:35:45.000000 swh.storage-1.8.0/sql/json/entity.lister_metadata.schema.json
--rw-r--r--   0 jenkins    (115) docker     (999)      129 2023-02-15 11:35:45.000000 swh.storage-1.8.0/sql/json/entity.metadata.schema.json
--rw-r--r--   0 jenkins    (115) docker     (999)      223 2023-02-15 11:35:45.000000 swh.storage-1.8.0/sql/json/entity_history.lister_metadata.schema.json
--rw-r--r--   0 jenkins    (115) docker     (999)      137 2023-02-15 11:35:45.000000 swh.storage-1.8.0/sql/json/entity_history.metadata.schema.json
--rw-r--r--   0 jenkins    (115) docker     (999)      631 2023-02-15 11:35:45.000000 swh.storage-1.8.0/sql/json/fetch_history.result.schema.json
--rw-r--r--   0 jenkins    (115) docker     (999)      133 2023-02-15 11:35:45.000000 swh.storage-1.8.0/sql/json/list_history.result.schema.json
--rw-r--r--   0 jenkins    (115) docker     (999)      141 2023-02-15 11:35:45.000000 swh.storage-1.8.0/sql/json/listable_entity.list_params.schema.json
--rw-r--r--   0 jenkins    (115) docker     (999)      632 2023-02-15 11:35:45.000000 swh.storage-1.8.0/sql/json/origin_visit.metadata.json
--rw-r--r--   0 jenkins    (115) docker     (999)      252 2023-02-15 11:35:45.000000 swh.storage-1.8.0/sql/json/tool.tool_configuration.schema.json
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-15 11:35:47.000000 swh.storage-1.8.0/swh/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-15 11:35:47.000000 swh.storage-1.8.0/swh/storage/
--rw-r--r--   0 jenkins    (115) docker     (999)     4009 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-15 11:35:47.000000 swh.storage-1.8.0/swh/storage/algos/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/algos/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)    15522 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/algos/diff.py
--rw-r--r--   0 jenkins    (115) docker     (999)    12234 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/algos/dir_iterators.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1210 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/algos/directory.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3280 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/algos/origin.py
--rw-r--r--   0 jenkins    (115) docker     (999)    19935 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/algos/revisions_walker.py
--rw-r--r--   0 jenkins    (115) docker     (999)     8395 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/algos/snapshot.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-15 11:35:47.000000 swh.storage-1.8.0/swh/storage/api/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/api/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1979 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/api/client.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2604 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/api/serializers.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5221 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/api/server.py
--rw-r--r--   0 jenkins    (115) docker     (999)    20570 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/backfill.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-15 11:35:47.000000 swh.storage-1.8.0/swh/storage/cassandra/
--rw-r--r--   0 jenkins    (115) docker     (999)      375 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/cassandra/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)      516 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/cassandra/common.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4926 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/cassandra/converters.py
--rw-r--r--   0 jenkins    (115) docker     (999)    53976 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/cassandra/cql.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7705 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/cassandra/model.py
--rw-r--r--   0 jenkins    (115) docker     (999)    10908 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/cassandra/schema.py
--rw-r--r--   0 jenkins    (115) docker     (999)    69986 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/cassandra/storage.py
--rw-r--r--   0 jenkins    (115) docker     (999)     8872 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/cli.py
--rw-r--r--   0 jenkins    (115) docker     (999)      496 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/common.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1856 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/exc.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2010 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/fixer.py
--rw-r--r--   0 jenkins    (115) docker     (999)    29503 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/in_memory.py
--rw-r--r--   0 jenkins    (115) docker     (999)    48423 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/interface.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2168 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/metrics.py
--rw-r--r--   0 jenkins    (115) docker     (999)    48095 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/migrate_extrinsic_metadata.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3555 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/objstorage.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-15 11:35:47.000000 swh.storage-1.8.0/swh/storage/postgresql/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/postgresql/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)    11867 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/postgresql/converters.py
--rw-r--r--   0 jenkins    (115) docker     (999)    49954 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/postgresql/db.py
--rw-r--r--   0 jenkins    (115) docker     (999)    59606 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/postgresql/storage.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-15 11:35:47.000000 swh.storage-1.8.0/swh/storage/proxies/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/proxies/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)    10939 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/proxies/buffer.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2033 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/proxies/counter.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5092 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/proxies/filter.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3229 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/proxies/retry.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6689 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/proxies/tenacious.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2586 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/proxies/validate.py
--rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/py.typed
--rw-r--r--   0 jenkins    (115) docker     (999)     2195 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/pytest_plugin.py
--rw-r--r--   0 jenkins    (115) docker     (999)     9270 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/replay.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-15 11:35:47.000000 swh.storage-1.8.0/swh/storage/sql/
--rw-r--r--   0 jenkins    (115) docker     (999)      758 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/10-superuser-init.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      984 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/15-flavor.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      859 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/20-enums.sql
--rw-r--r--   0 jenkins    (115) docker     (999)    23639 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/30-schema.sql
--rw-r--r--   0 jenkins    (115) docker     (999)    34043 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/40-funcs.sql
--rw-r--r--   0 jenkins    (115) docker     (999)    13835 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/60-indexes.sql
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-15 11:35:47.000000 swh.storage-1.8.0/swh/storage/sql/logical_replication/
--rw-r--r--   0 jenkins    (115) docker     (999)     1380 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/logical_replication/replication_source.sql
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-15 11:35:47.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/
--rw-r--r--   0 jenkins    (115) docker     (999)     6750 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/015.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      854 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/016.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     6452 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/017.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2845 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/018.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      999 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/019.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1416 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/020.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1464 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/021.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1607 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/022.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1561 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/023.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     6282 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/024.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     3272 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/025.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      658 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/026.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     9090 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/027.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1446 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/028.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2788 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/029.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1706 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/030.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     4156 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/032.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1131 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/033.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2599 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/034.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1535 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/035.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2256 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/036.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      654 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/037.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     4588 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/038.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1659 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/039.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      553 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/040.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      542 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/041.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      702 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/042.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2902 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/043.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2130 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/044.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      465 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/045.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     7305 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/046.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2649 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/047.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1795 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/048.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     9599 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/049.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1688 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/050.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     4279 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/051.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     6016 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/052.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      905 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/053.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     3187 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/054.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2309 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/055.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2350 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/056.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      729 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/057.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1428 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/058.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1528 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/059.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1428 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/060.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      724 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/061.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1427 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/062.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2594 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/063.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      604 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/064.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1664 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/065.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      281 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/066.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1257 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/067.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     8795 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/068.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      618 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/069.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      352 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/070.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      687 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/071.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     3843 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/072.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1940 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/073.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2662 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/074.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     3067 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/075.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      551 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/076.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1567 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/077.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     3642 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/078.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      997 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/079.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      631 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/080.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      608 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/081.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     3043 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/082.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1834 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/083.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2392 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/084.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2388 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/085.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1249 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/086.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     8777 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/087.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     3567 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/088.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     3788 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/089.sql
--rw-r--r--   0 jenkins    (115) docker     (999)    21174 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/090.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      959 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/091.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      925 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/092.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1795 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/093.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      735 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/094.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      726 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/095.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1137 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/096.sql
--rw-r--r--   0 jenkins    (115) docker     (999)    18174 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/097.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      280 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/098.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      875 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/099.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2055 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/100.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1037 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/101.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     6608 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/102.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2399 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/103.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     5055 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/104.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1078 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/105.sql
--rw-r--r--   0 jenkins    (115) docker     (999)    13015 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/106.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1755 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/107.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1427 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/108.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      816 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/109.sql
--rw-r--r--   0 jenkins    (115) docker     (999)    13273 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/110.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      784 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/111.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1620 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/112.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1142 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/113.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2334 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/114.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     5180 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/115.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      276 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/116.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1742 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/117.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2768 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/118.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      850 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/119.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1062 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/120.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      274 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/121.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      366 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/122.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2107 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/123.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1371 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/124.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1302 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/125.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      329 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/126.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1039 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/127.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      609 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/128.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      832 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/129.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1572 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/130.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      401 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/131.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      386 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/132.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      425 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/133.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1626 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/134.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      421 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/135.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1036 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/136.sql
--rw-r--r--   0 jenkins    (115) docker     (999)    10048 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/137.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      926 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/138.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      845 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/139.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      456 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/140.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      230 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/141.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      239 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/142.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2897 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/143.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      283 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/144.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      275 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/145.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     3340 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/146.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2676 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/147.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2168 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/148.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     3849 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/149.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      624 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/150.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      373 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/151.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      302 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/152.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      462 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/153.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1546 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/154.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1044 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/155.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      875 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/156.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2606 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/157.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     3118 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/158.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      727 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/159.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1353 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/160.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      548 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/161.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2099 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/162.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1202 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/163.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      304 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/164.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      430 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/165.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      306 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/166.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      591 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/167.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1403 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/168.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1812 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/169.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      614 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/170.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      758 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/171.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      873 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/172.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      561 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/173.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      324 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/174.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1294 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/175.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      886 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/176.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      256 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/177.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      256 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/178.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     6715 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/179.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     3159 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/180.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      661 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/181.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2782 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/182.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1715 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/183.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      910 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/184.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1091 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/185.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      356 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/sql/upgrades/186.sql
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-15 11:35:47.000000 swh.storage-1.8.0/swh/storage/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)      356 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-15 11:35:47.000000 swh.storage-1.8.0/swh/storage/tests/algos/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/algos/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)    12970 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/algos/test_diff.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5545 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/algos/test_dir_iterator.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1649 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/algos/test_directory.py
--rw-r--r--   0 jenkins    (115) docker     (999)    11595 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/algos/test_origin.py
--rw-r--r--   0 jenkins    (115) docker     (999)    18304 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/algos/test_revisions_walker.py
--rw-r--r--   0 jenkins    (115) docker     (999)    16690 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/algos/test_snapshot.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2990 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-15 11:35:47.000000 swh.storage-1.8.0/swh/storage/tests/data/
--rw-r--r--   0 jenkins    (115) docker     (999)      189 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/data/storage.yml
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-15 11:35:47.000000 swh.storage-1.8.0/swh/storage/tests/migrate_extrinsic_metadata/
--rw-r--r--   0 jenkins    (115) docker     (999)    11037 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/migrate_extrinsic_metadata/test_cran.py
--rw-r--r--   0 jenkins    (115) docker     (999)    20296 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/migrate_extrinsic_metadata/test_debian.py
--rw-r--r--   0 jenkins    (115) docker     (999)    52095 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/migrate_extrinsic_metadata/test_deposit.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3702 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/migrate_extrinsic_metadata/test_gnu.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4246 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/migrate_extrinsic_metadata/test_nixguix.py
--rw-r--r--   0 jenkins    (115) docker     (999)    15545 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/migrate_extrinsic_metadata/test_npm.py
--rw-r--r--   0 jenkins    (115) docker     (999)    25031 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/migrate_extrinsic_metadata/test_pypi.py
--rw-r--r--   0 jenkins    (115) docker     (999)    26818 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/storage_data.py
--rw-r--r--   0 jenkins    (115) docker     (999)   209185 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/storage_tests.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5100 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/test_api_client.py
--rw-r--r--   0 jenkins    (115) docker     (999)    14820 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/test_backfill.py
--rw-r--r--   0 jenkins    (115) docker     (999)    23547 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/test_buffer.py
--rw-r--r--   0 jenkins    (115) docker     (999)    27506 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/test_cassandra.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1679 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/test_cassandra_converters.py
--rw-r--r--   0 jenkins    (115) docker     (999)    12396 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/test_cassandra_migration.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3721 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/test_cli.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1887 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/test_counter.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1167 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/test_exception.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5260 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/test_filter.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4083 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/test_in_memory.py
--rw-r--r--   0 jenkins    (115) docker     (999)     8744 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/test_init.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4946 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/test_kafka_writer.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1582 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/test_metrics.py
--rw-r--r--   0 jenkins    (115) docker     (999)    13907 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/test_postgresql.py
--rw-r--r--   0 jenkins    (115) docker     (999)    12253 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/test_postgresql_converters.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1281 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/test_postgresql_flavor_mirror.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1305 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/test_postgresql_flavor_readreplica.py
--rw-r--r--   0 jenkins    (115) docker     (999)      669 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/test_pytest_plugin.py
--rw-r--r--   0 jenkins    (115) docker     (999)    19818 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/test_replay.py
--rw-r--r--   0 jenkins    (115) docker     (999)     8212 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/test_retry.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1589 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/test_revision_bw_compat.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1346 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/test_serializers.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3323 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/test_server.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1186 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/test_storage_data.py
--rw-r--r--   0 jenkins    (115) docker     (999)    13821 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/test_tenacious.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4261 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/test_utils.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4515 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/tests/test_validate.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3454 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/utils.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4041 2023-02-15 11:35:45.000000 swh.storage-1.8.0/swh/storage/writer.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-02-15 11:35:47.000000 swh.storage-1.8.0/swh.storage.egg-info/
--rw-r--r--   0 jenkins    (115) docker     (999)     6708 2023-02-15 11:35:47.000000 swh.storage-1.8.0/swh.storage.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)    11096 2023-02-15 11:35:47.000000 swh.storage-1.8.0/swh.storage.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-02-15 11:35:47.000000 swh.storage-1.8.0/swh.storage.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       48 2023-02-15 11:35:47.000000 swh.storage-1.8.0/swh.storage.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      458 2023-02-15 11:35:47.000000 swh.storage-1.8.0/swh.storage.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-02-15 11:35:47.000000 swh.storage-1.8.0/swh.storage.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1748 2023-02-15 11:35:45.000000 swh.storage-1.8.0/tox.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-06 13:52:23.000000 swh.storage-1.9.0/
+-rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-03-06 13:52:21.000000 swh.storage-1.9.0/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) docker     (999)      136 2023-03-06 13:52:21.000000 swh.storage-1.9.0/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      916 2023-03-06 13:52:21.000000 swh.storage-1.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-03-06 13:52:21.000000 swh.storage-1.9.0/AUTHORS
+-rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-03-06 13:52:21.000000 swh.storage-1.9.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) docker     (999)       61 2023-03-06 13:52:21.000000 swh.storage-1.9.0/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-03-06 13:52:21.000000 swh.storage-1.9.0/LICENSE
+-rw-r--r--   0 jenkins    (115) docker     (999)      242 2023-03-06 13:52:21.000000 swh.storage-1.9.0/MANIFEST.in
+-rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-03-06 13:52:21.000000 swh.storage-1.9.0/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)       69 2023-03-06 13:52:21.000000 swh.storage-1.9.0/Makefile.local
+-rw-r--r--   0 jenkins    (115) docker     (999)     6708 2023-03-06 13:52:23.000000 swh.storage-1.9.0/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     5761 2023-03-06 13:52:21.000000 swh.storage-1.9.0/README.md
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-06 13:52:23.000000 swh.storage-1.9.0/bin/
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     1240 2023-03-06 13:52:21.000000 swh.storage-1.9.0/bin/swh-storage-add-dir
+-rw-r--r--   0 jenkins    (115) docker     (999)      323 2023-03-06 13:52:21.000000 swh.storage-1.9.0/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-06 13:52:23.000000 swh.storage-1.9.0/docs/
+-rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-03-06 13:52:21.000000 swh.storage-1.9.0/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)       63 2023-03-06 13:52:21.000000 swh.storage-1.9.0/docs/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)      530 2023-03-06 13:52:21.000000 swh.storage-1.9.0/docs/Makefile.local
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-06 13:52:23.000000 swh.storage-1.9.0/docs/_static/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-06 13:52:21.000000 swh.storage-1.9.0/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-06 13:52:23.000000 swh.storage-1.9.0/docs/_templates/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-06 13:52:21.000000 swh.storage-1.9.0/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) docker     (999)     2206 2023-03-06 13:52:21.000000 swh.storage-1.9.0/docs/archive-copies.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      143 2023-03-06 13:52:21.000000 swh.storage-1.9.0/docs/cli.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-03-06 13:52:21.000000 swh.storage-1.9.0/docs/conf.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    12957 2023-03-06 13:52:21.000000 swh.storage-1.9.0/docs/extrinsic-metadata-specification.rst
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-06 13:52:23.000000 swh.storage-1.9.0/docs/images/
+-rw-r--r--   0 jenkins    (115) docker     (999)       12 2023-03-06 13:52:21.000000 swh.storage-1.9.0/docs/images/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      335 2023-03-06 13:52:21.000000 swh.storage-1.9.0/docs/images/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     3031 2023-03-06 13:52:21.000000 swh.storage-1.9.0/docs/images/swh-archive-copies.dia
+-rw-r--r--   0 jenkins    (115) docker     (999)     2965 2023-03-06 13:52:21.000000 swh.storage-1.9.0/docs/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      268 2023-03-06 13:52:21.000000 swh.storage-1.9.0/docs/sql-storage.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     1211 2023-03-06 13:52:21.000000 swh.storage-1.9.0/mypy.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-03-06 13:52:21.000000 swh.storage-1.9.0/pyproject.toml
+-rw-r--r--   0 jenkins    (115) docker     (999)      424 2023-03-06 13:52:21.000000 swh.storage-1.9.0/pytest.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)       19 2023-03-06 13:52:21.000000 swh.storage-1.9.0/requirements-swh-journal.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       94 2023-03-06 13:52:21.000000 swh.storage-1.9.0/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      372 2023-03-06 13:52:21.000000 swh.storage-1.9.0/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      189 2023-03-06 13:52:21.000000 swh.storage-1.9.0/requirements.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-03-06 13:52:23.000000 swh.storage-1.9.0/setup.cfg
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     2469 2023-03-06 13:52:21.000000 swh.storage-1.9.0/setup.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-06 13:52:23.000000 swh.storage-1.9.0/sql/
+-rw-r--r--   0 jenkins    (115) docker     (999)       26 2023-03-06 13:52:21.000000 swh.storage-1.9.0/sql/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)     1565 2023-03-06 13:52:21.000000 swh.storage-1.9.0/sql/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     1094 2023-03-06 13:52:21.000000 swh.storage-1.9.0/sql/TODO
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-06 13:52:23.000000 swh.storage-1.9.0/sql/bin/
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     1701 2023-03-06 13:52:21.000000 swh.storage-1.9.0/sql/bin/db-upgrade
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      538 2023-03-06 13:52:21.000000 swh.storage-1.9.0/sql/bin/dot_add_content
+-rw-r--r--   0 jenkins    (115) docker     (999)     2023 2023-03-06 13:52:21.000000 swh.storage-1.9.0/sql/clusters.dot
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-06 13:52:23.000000 swh.storage-1.9.0/sql/doc/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-06 13:52:23.000000 swh.storage-1.9.0/sql/doc/json/
+-rw-r--r--   0 jenkins    (115) docker     (999)        8 2023-03-06 13:52:21.000000 swh.storage-1.9.0/sql/doc/json/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      283 2023-03-06 13:52:21.000000 swh.storage-1.9.0/sql/doc/json/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)      223 2023-03-06 13:52:21.000000 swh.storage-1.9.0/sql/doc/json/entity.lister_metadata.schema.json
+-rw-r--r--   0 jenkins    (115) docker     (999)      129 2023-03-06 13:52:21.000000 swh.storage-1.9.0/sql/doc/json/entity.metadata.schema.json
+-rw-r--r--   0 jenkins    (115) docker     (999)      223 2023-03-06 13:52:21.000000 swh.storage-1.9.0/sql/doc/json/entity_history.lister_metadata.schema.json
+-rw-r--r--   0 jenkins    (115) docker     (999)      137 2023-03-06 13:52:21.000000 swh.storage-1.9.0/sql/doc/json/entity_history.metadata.schema.json
+-rw-r--r--   0 jenkins    (115) docker     (999)      631 2023-03-06 13:52:21.000000 swh.storage-1.9.0/sql/doc/json/fetch_history.result.schema.json
+-rw-r--r--   0 jenkins    (115) docker     (999)      133 2023-03-06 13:52:21.000000 swh.storage-1.9.0/sql/doc/json/list_history.result.schema.json
+-rw-r--r--   0 jenkins    (115) docker     (999)      141 2023-03-06 13:52:21.000000 swh.storage-1.9.0/sql/doc/json/listable_entity.list_params.schema.json
+-rw-r--r--   0 jenkins    (115) docker     (999)      632 2023-03-06 13:52:21.000000 swh.storage-1.9.0/sql/doc/json/origin_visit.metadata.json
+-rw-r--r--   0 jenkins    (115) docker     (999)      252 2023-03-06 13:52:21.000000 swh.storage-1.9.0/sql/doc/json/tool.tool_configuration.schema.json
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-06 13:52:23.000000 swh.storage-1.9.0/sql/json/
+-rw-r--r--   0 jenkins    (115) docker     (999)        8 2023-03-06 13:52:21.000000 swh.storage-1.9.0/sql/json/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      283 2023-03-06 13:52:21.000000 swh.storage-1.9.0/sql/json/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)      223 2023-03-06 13:52:21.000000 swh.storage-1.9.0/sql/json/entity.lister_metadata.schema.json
+-rw-r--r--   0 jenkins    (115) docker     (999)      129 2023-03-06 13:52:21.000000 swh.storage-1.9.0/sql/json/entity.metadata.schema.json
+-rw-r--r--   0 jenkins    (115) docker     (999)      223 2023-03-06 13:52:21.000000 swh.storage-1.9.0/sql/json/entity_history.lister_metadata.schema.json
+-rw-r--r--   0 jenkins    (115) docker     (999)      137 2023-03-06 13:52:21.000000 swh.storage-1.9.0/sql/json/entity_history.metadata.schema.json
+-rw-r--r--   0 jenkins    (115) docker     (999)      631 2023-03-06 13:52:21.000000 swh.storage-1.9.0/sql/json/fetch_history.result.schema.json
+-rw-r--r--   0 jenkins    (115) docker     (999)      133 2023-03-06 13:52:21.000000 swh.storage-1.9.0/sql/json/list_history.result.schema.json
+-rw-r--r--   0 jenkins    (115) docker     (999)      141 2023-03-06 13:52:21.000000 swh.storage-1.9.0/sql/json/listable_entity.list_params.schema.json
+-rw-r--r--   0 jenkins    (115) docker     (999)      632 2023-03-06 13:52:21.000000 swh.storage-1.9.0/sql/json/origin_visit.metadata.json
+-rw-r--r--   0 jenkins    (115) docker     (999)      252 2023-03-06 13:52:21.000000 swh.storage-1.9.0/sql/json/tool.tool_configuration.schema.json
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-06 13:52:23.000000 swh.storage-1.9.0/swh/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-06 13:52:23.000000 swh.storage-1.9.0/swh/storage/
+-rw-r--r--   0 jenkins    (115) docker     (999)     4009 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-06 13:52:23.000000 swh.storage-1.9.0/swh/storage/algos/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/algos/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    15522 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/algos/diff.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    12234 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/algos/dir_iterators.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1210 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/algos/directory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3280 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/algos/origin.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    19935 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/algos/revisions_walker.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     8395 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/algos/snapshot.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-06 13:52:23.000000 swh.storage-1.9.0/swh/storage/api/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/api/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1979 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/api/client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2604 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/api/serializers.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5221 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/api/server.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    20570 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/backfill.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-06 13:52:23.000000 swh.storage-1.9.0/swh/storage/cassandra/
+-rw-r--r--   0 jenkins    (115) docker     (999)      375 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/cassandra/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      516 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/cassandra/common.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4926 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/cassandra/converters.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    55794 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/cassandra/cql.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7705 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/cassandra/model.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    10908 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/cassandra/schema.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    73125 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/cassandra/storage.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     8872 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/cli.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      496 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/common.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1856 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/exc.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2010 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/fixer.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    30600 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/in_memory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    51752 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/interface.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2168 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/metrics.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    48095 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/migrate_extrinsic_metadata.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3555 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/objstorage.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-06 13:52:23.000000 swh.storage-1.9.0/swh/storage/postgresql/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/postgresql/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    11867 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/postgresql/converters.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    52019 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/postgresql/db.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    62835 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/postgresql/storage.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-06 13:52:23.000000 swh.storage-1.9.0/swh/storage/proxies/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/proxies/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    10939 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/proxies/buffer.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2033 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/proxies/counter.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5092 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/proxies/filter.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3229 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/proxies/retry.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6689 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/proxies/tenacious.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2586 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/proxies/validate.py
+-rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/py.typed
+-rw-r--r--   0 jenkins    (115) docker     (999)     2195 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/pytest_plugin.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     9270 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/replay.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-06 13:52:23.000000 swh.storage-1.9.0/swh/storage/sql/
+-rw-r--r--   0 jenkins    (115) docker     (999)      758 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/10-superuser-init.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      984 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/15-flavor.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      859 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/20-enums.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)    23639 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/30-schema.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)    34043 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/40-funcs.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)    13835 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/60-indexes.sql
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-06 13:52:23.000000 swh.storage-1.9.0/swh/storage/sql/logical_replication/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1380 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/logical_replication/replication_source.sql
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-06 13:52:23.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/
+-rw-r--r--   0 jenkins    (115) docker     (999)     6750 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/015.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      854 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/016.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     6452 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/017.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2845 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/018.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      999 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/019.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1416 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/020.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1464 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/021.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1607 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/022.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1561 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/023.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     6282 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/024.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     3272 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/025.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      658 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/026.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     9090 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/027.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1446 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/028.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2788 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/029.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1706 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/030.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     4156 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/032.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1131 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/033.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2599 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/034.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1535 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/035.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2256 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/036.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      654 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/037.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     4588 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/038.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1659 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/039.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      553 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/040.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      542 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/041.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      702 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/042.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2902 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/043.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2130 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/044.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      465 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/045.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     7305 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/046.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2649 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/047.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1795 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/048.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     9599 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/049.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1688 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/050.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     4279 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/051.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     6016 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/052.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      905 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/053.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     3187 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/054.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2309 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/055.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2350 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/056.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      729 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/057.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1428 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/058.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1528 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/059.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1428 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/060.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      724 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/061.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1427 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/062.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2594 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/063.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      604 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/064.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1664 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/065.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      281 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/066.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1257 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/067.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     8795 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/068.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      618 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/069.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      352 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/070.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      687 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/071.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     3843 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/072.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1940 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/073.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2662 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/074.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     3067 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/075.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      551 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/076.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1567 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/077.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     3642 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/078.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      997 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/079.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      631 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/080.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      608 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/081.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     3043 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/082.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1834 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/083.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2392 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/084.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2388 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/085.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1249 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/086.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     8777 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/087.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     3567 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/088.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     3788 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/089.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)    21174 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/090.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      959 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/091.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      925 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/092.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1795 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/093.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      735 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/094.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      726 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/095.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1137 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/096.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)    18174 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/097.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      280 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/098.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      875 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/099.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2055 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/100.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1037 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/101.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     6608 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/102.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2399 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/103.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     5055 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/104.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1078 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/105.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)    13015 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/106.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1755 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/107.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1427 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/108.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      816 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/109.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)    13273 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/110.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      784 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/111.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1620 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/112.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1142 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/113.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2334 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/114.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     5180 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/115.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      276 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/116.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1742 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/117.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2768 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/118.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      850 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/119.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1062 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/120.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      274 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/121.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      366 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/122.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2107 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/123.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1371 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/124.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1302 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/125.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      329 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/126.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1039 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/127.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      609 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/128.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      832 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/129.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1572 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/130.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      401 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/131.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      386 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/132.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      425 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/133.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1626 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/134.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      421 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/135.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1036 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/136.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)    10048 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/137.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      926 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/138.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      845 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/139.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      456 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/140.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      230 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/141.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      239 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/142.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2897 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/143.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      283 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/144.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      275 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/145.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     3340 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/146.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2676 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/147.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2168 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/148.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     3849 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/149.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      624 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/150.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      373 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/151.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      302 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/152.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      462 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/153.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1546 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/154.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1044 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/155.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      875 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/156.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2606 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/157.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     3118 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/158.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      727 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/159.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1353 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/160.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      548 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/161.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2099 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/162.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1202 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/163.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      304 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/164.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      430 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/165.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      306 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/166.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      591 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/167.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1403 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/168.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1812 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/169.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      614 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/170.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      758 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/171.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      873 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/172.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      561 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/173.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      324 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/174.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1294 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/175.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      886 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/176.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      256 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/177.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      256 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/178.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     6715 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/179.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     3159 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/180.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      661 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/181.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2782 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/182.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1715 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/183.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      910 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/184.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1091 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/185.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      356 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/sql/upgrades/186.sql
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-06 13:52:23.000000 swh.storage-1.9.0/swh/storage/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)      356 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-06 13:52:23.000000 swh.storage-1.9.0/swh/storage/tests/algos/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/algos/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    12970 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/algos/test_diff.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5545 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/algos/test_dir_iterator.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1649 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/algos/test_directory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    11595 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/algos/test_origin.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    18304 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/algos/test_revisions_walker.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    16690 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/algos/test_snapshot.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3012 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-06 13:52:23.000000 swh.storage-1.9.0/swh/storage/tests/data/
+-rw-r--r--   0 jenkins    (115) docker     (999)      189 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/data/storage.yml
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-06 13:52:23.000000 swh.storage-1.9.0/swh/storage/tests/migrate_extrinsic_metadata/
+-rw-r--r--   0 jenkins    (115) docker     (999)    11037 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/migrate_extrinsic_metadata/test_cran.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    20296 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/migrate_extrinsic_metadata/test_debian.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    52095 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/migrate_extrinsic_metadata/test_deposit.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3702 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/migrate_extrinsic_metadata/test_gnu.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4246 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/migrate_extrinsic_metadata/test_nixguix.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    15545 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/migrate_extrinsic_metadata/test_npm.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    25031 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/migrate_extrinsic_metadata/test_pypi.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    26818 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/storage_data.py
+-rw-r--r--   0 jenkins    (115) docker     (999)   214264 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/storage_tests.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5100 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/test_api_client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    14820 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/test_backfill.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    23547 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/test_buffer.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    27506 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/test_cassandra.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1679 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/test_cassandra_converters.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    12396 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/test_cassandra_migration.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3721 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/test_cli.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1887 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/test_counter.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1167 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/test_exception.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5260 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/test_filter.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4083 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/test_in_memory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     8744 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/test_init.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4946 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/test_kafka_writer.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1582 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/test_metrics.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    13907 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/test_postgresql.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    12253 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/test_postgresql_converters.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1281 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/test_postgresql_flavor_mirror.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1305 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/test_postgresql_flavor_readreplica.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      669 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/test_pytest_plugin.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    19818 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/test_replay.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     8212 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/test_retry.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1589 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/test_revision_bw_compat.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1346 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/test_serializers.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3323 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/test_server.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1186 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/test_storage_data.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    13821 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/test_tenacious.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4261 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/test_utils.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4515 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/tests/test_validate.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3454 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/utils.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4041 2023-03-06 13:52:21.000000 swh.storage-1.9.0/swh/storage/writer.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-06 13:52:23.000000 swh.storage-1.9.0/swh.storage.egg-info/
+-rw-r--r--   0 jenkins    (115) docker     (999)     6708 2023-03-06 13:52:23.000000 swh.storage-1.9.0/swh.storage.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)    11096 2023-03-06 13:52:23.000000 swh.storage-1.9.0/swh.storage.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-03-06 13:52:23.000000 swh.storage-1.9.0/swh.storage.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       48 2023-03-06 13:52:23.000000 swh.storage-1.9.0/swh.storage.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      458 2023-03-06 13:52:23.000000 swh.storage-1.9.0/swh.storage.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-03-06 13:52:23.000000 swh.storage-1.9.0/swh.storage.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1773 2023-03-06 13:52:21.000000 swh.storage-1.9.0/tox.ini
```

### Comparing `swh.storage-1.8.0/.pre-commit-config.yaml` & `swh.storage-1.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/CODE_OF_CONDUCT.md` & `swh.storage-1.9.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/LICENSE` & `swh.storage-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/PKG-INFO` & `swh.storage-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.storage
-Version: 1.8.0
+Version: 1.9.0
 Summary: Software Heritage storage manager
 Home-page: https://forge.softwareheritage.org/diffusion/DSTO/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-storage
```

### Comparing `swh.storage-1.8.0/README.md` & `swh.storage-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/bin/swh-storage-add-dir` & `swh.storage-1.9.0/bin/swh-storage-add-dir`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/docs/Makefile.local` & `swh.storage-1.9.0/docs/Makefile.local`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/docs/archive-copies.rst` & `swh.storage-1.9.0/docs/archive-copies.rst`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/docs/extrinsic-metadata-specification.rst` & `swh.storage-1.9.0/docs/extrinsic-metadata-specification.rst`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/docs/images/swh-archive-copies.dia` & `swh.storage-1.9.0/docs/images/swh-archive-copies.dia`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/docs/index.rst` & `swh.storage-1.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/mypy.ini` & `swh.storage-1.9.0/mypy.ini`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/setup.py` & `swh.storage-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/sql/Makefile` & `swh.storage-1.9.0/sql/Makefile`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/sql/TODO` & `swh.storage-1.9.0/sql/TODO`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/sql/bin/db-upgrade` & `swh.storage-1.9.0/sql/bin/db-upgrade`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/sql/bin/dot_add_content` & `swh.storage-1.9.0/sql/bin/dot_add_content`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/sql/clusters.dot` & `swh.storage-1.9.0/sql/clusters.dot`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/sql/doc/json/fetch_history.result.schema.json` & `swh.storage-1.9.0/sql/doc/json/fetch_history.result.schema.json`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/sql/doc/json/origin_visit.metadata.json` & `swh.storage-1.9.0/sql/doc/json/origin_visit.metadata.json`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/sql/json/fetch_history.result.schema.json` & `swh.storage-1.9.0/sql/json/fetch_history.result.schema.json`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/sql/json/origin_visit.metadata.json` & `swh.storage-1.9.0/sql/json/origin_visit.metadata.json`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/__init__.py` & `swh.storage-1.9.0/swh/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/algos/diff.py` & `swh.storage-1.9.0/swh/storage/algos/diff.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/algos/dir_iterators.py` & `swh.storage-1.9.0/swh/storage/algos/dir_iterators.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/algos/directory.py` & `swh.storage-1.9.0/swh/storage/algos/directory.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/algos/origin.py` & `swh.storage-1.9.0/swh/storage/algos/origin.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/algos/revisions_walker.py` & `swh.storage-1.9.0/swh/storage/algos/revisions_walker.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/algos/snapshot.py` & `swh.storage-1.9.0/swh/storage/algos/snapshot.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/api/client.py` & `swh.storage-1.9.0/swh/storage/api/client.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/api/serializers.py` & `swh.storage-1.9.0/swh/storage/api/serializers.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/api/server.py` & `swh.storage-1.9.0/swh/storage/api/server.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/backfill.py` & `swh.storage-1.9.0/swh/storage/backfill.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/cassandra/common.py` & `swh.storage-1.9.0/swh/storage/cassandra/common.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/cassandra/converters.py` & `swh.storage-1.9.0/swh/storage/cassandra/converters.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/cassandra/cql.py` & `swh.storage-1.9.0/swh/storage/cassandra/cql.py`

 * *Files 3% similar despite different names*

```diff
@@ -149,15 +149,15 @@
     """Returns a decorator usable on methods of CqlRunner, to
     inject them with a 'statement' argument, that is a prepared
     statement corresponding to the query.
 
     This only works on methods of CqlRunner, as preparing a
     statement requires a connection to a Cassandra server."""
 
-    def decorator(f):
+    def decorator(f: Callable[..., TRet]):
         @functools.wraps(f)
         def newf(self: "CqlRunner", *args, **kwargs) -> TRet:
             if f.__name__ not in self._prepared_statements:
                 statement: PreparedStatement = self._session.prepare(
                     query.format(keyspace=self.keyspace)
                 )
                 self._prepared_statements[f.__name__] = statement
@@ -223,15 +223,15 @@
 ) -> Callable[[Callable[..., TRet]], Callable[..., TRet]]:
     """Like _prepared_statement, but supports multiple statements, passed a dict,
     and passes a dict of prepared statements to the decorated method"""
     cols = row_class.cols()
 
     statement_template = "SELECT {cols} FROM {keyspace}.{table} {rest}"
 
-    def decorator(f):
+    def decorator(f: Callable[..., TRet]):
         @functools.wraps(f)
         def newf(self: "CqlRunner", *args, **kwargs) -> TRet:
             if f.__name__ not in self._prepared_statements:
                 self._prepared_statements[f.__name__] = {
                     key: self._session.prepare(
                         statement_template.format(
                             cols=", ".join(cols),
@@ -467,15 +467,15 @@
     )
     def content_get_random(self, *, statement) -> Optional[ContentRow]:
         return self._get_random_row(ContentRow, statement)
 
     @_prepared_select_token_range_statement(ContentRow, "LIMIT ?")
     def content_get_token_range(
         self, start: int, end: int, limit: int, *, statement
-    ) -> Iterable[Tuple[int, ContentRow]]:
+    ) -> Iterator[Tuple[int, ContentRow]]:
         """Returns an iterable of (token, row)"""
         return (
             (row["tok"], ContentRow.from_dict(remove_keys(row, ("tok",))))
             for row in self._execute_with_retries(statement, [start, end, limit])
         )
 
     ##########################
@@ -629,14 +629,24 @@
         """Return fields from the main directory table (e.g. raw_manifest, but not
         entries)"""
         return map(
             DirectoryRow.from_dict,
             self._execute_with_retries(statement, [directory_ids]),
         )
 
+    @_prepared_select_token_range_statement(DirectoryRow, "LIMIT ?")
+    def directory_get_token_range(
+        self, start: int, end: int, limit: int, *, statement
+    ) -> Iterator[Tuple[int, DirectoryRow]]:
+        """Returns an iterable of (token, row)"""
+        return (
+            (row["tok"], DirectoryRow.from_dict(remove_keys(row, ("tok",))))
+            for row in self._execute_with_retries(statement, [start, end, limit])
+        )
+
     ##########################
     # 'directory_entry' table
     ##########################
 
     @_prepared_insert_statement(DirectoryEntryRow)
     def directory_entry_add_one(self, entry: DirectoryEntryRow, *, statement) -> None:
         self._add_one(statement, entry)
@@ -713,15 +723,15 @@
         return self._missing(statement, ids)
 
     @_prepared_insert_statement(RevisionRow)
     def revision_add_one(self, revision: RevisionRow, *, statement) -> None:
         self._add_one(statement, revision)
 
     @_prepared_select_statement(RevisionRow, "WHERE id IN ?", ["id"])
-    def revision_get_ids(self, revision_ids, *, statement) -> Iterable[int]:
+    def revision_get_ids(self, revision_ids, *, statement) -> Iterable[Sha1Git]:
         return (
             row["id"] for row in self._execute_with_retries(statement, [revision_ids])
         )
 
     @_prepared_select_statement(RevisionRow, "WHERE id IN ?")
     def revision_get(
         self, revision_ids: List[Sha1Git], *, statement
@@ -730,14 +740,24 @@
             RevisionRow.from_dict, self._execute_with_retries(statement, [revision_ids])
         )
 
     @_prepared_select_statement(RevisionRow, "WHERE token(id) > ? LIMIT 1")
     def revision_get_random(self, *, statement) -> Optional[RevisionRow]:
         return self._get_random_row(RevisionRow, statement)
 
+    @_prepared_select_token_range_statement(RevisionRow, "LIMIT ?")
+    def revision_get_token_range(
+        self, start: int, end: int, limit: int, *, statement
+    ) -> Iterator[Tuple[int, RevisionRow]]:
+        """Returns an iterable of (token, row)"""
+        return (
+            (row["tok"], RevisionRow.from_dict(remove_keys(row, ("tok",))))
+            for row in self._execute_with_retries(statement, [start, end, limit])
+        )
+
     ##########################
     # 'revision_parent' table
     ##########################
 
     @_prepared_insert_statement(RevisionParentRow)
     def revision_parent_add_one(
         self, revision_parent: RevisionParentRow, *, statement
@@ -773,14 +793,24 @@
             ReleaseRow.from_dict, self._execute_with_retries(statement, [release_ids])
         )
 
     @_prepared_select_statement(ReleaseRow, "WHERE token(id) > ? LIMIT 1")
     def release_get_random(self, *, statement) -> Optional[ReleaseRow]:
         return self._get_random_row(ReleaseRow, statement)
 
+    @_prepared_select_token_range_statement(ReleaseRow, "LIMIT ?")
+    def release_get_token_range(
+        self, start: int, end: int, limit: int, *, statement
+    ) -> Iterator[Tuple[int, ReleaseRow]]:
+        """Returns an iterable of (token, row)"""
+        return (
+            (row["tok"], ReleaseRow.from_dict(remove_keys(row, ("tok",))))
+            for row in self._execute_with_retries(statement, [start, end, limit])
+        )
+
     ##########################
     # 'snapshot' table
     ##########################
 
     @_prepared_exists_statement("snapshot")
     def snapshot_missing(self, ids: List[bytes], *, statement) -> List[bytes]:
         return self._missing(statement, ids)
@@ -789,14 +819,24 @@
     def snapshot_add_one(self, snapshot: SnapshotRow, *, statement) -> None:
         self._add_one(statement, snapshot)
 
     @_prepared_select_statement(SnapshotRow, "WHERE token(id) > ? LIMIT 1")
     def snapshot_get_random(self, *, statement) -> Optional[SnapshotRow]:
         return self._get_random_row(SnapshotRow, statement)
 
+    @_prepared_select_token_range_statement(SnapshotRow, "LIMIT ?")
+    def snapshot_get_token_range(
+        self, start: int, end: int, limit: int, *, statement
+    ) -> Iterator[Tuple[int, SnapshotRow]]:
+        """Returns an iterable of (token, row)"""
+        return (
+            (row["tok"], SnapshotRow.from_dict(remove_keys(row, ("tok",))))
+            for row in self._execute_with_retries(statement, [start, end, limit])
+        )
+
     ##########################
     # 'snapshot_branch' table
     ##########################
 
     @_prepared_insert_statement(SnapshotBranchRow)
     def snapshot_branch_add_one(self, branch: SnapshotBranchRow, *, statement) -> None:
         self._add_one(statement, branch)
```

### Comparing `swh.storage-1.8.0/swh/storage/cassandra/model.py` & `swh.storage-1.9.0/swh/storage/cassandra/model.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/cassandra/schema.py` & `swh.storage-1.9.0/swh/storage/cassandra/schema.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/cassandra/storage.py` & `swh.storage-1.9.0/swh/storage/cassandra/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 import re
 from typing import (
     Any,
     Callable,
     Counter,
     Dict,
     Iterable,
+    Iterator,
     List,
     Optional,
     Sequence,
     Set,
     Tuple,
+    TypeVar,
     Union,
     cast,
 )
 
 import attr
 
 from swh.core.api.classes import stream_results
@@ -73,39 +75,93 @@
     UnknownMetadataAuthority,
     UnknownMetadataFetcher,
 )
 from ..utils import remove_keys
 from .common import TOKEN_BEGIN, TOKEN_END, hash_url
 from .cql import CqlRunner
 from .model import (
+    BaseRow,
     ContentRow,
     DirectoryEntryRow,
     DirectoryRow,
     ExtIDByTargetRow,
     ExtIDRow,
     MetadataAuthorityRow,
     MetadataFetcherRow,
     OriginRow,
     OriginVisitRow,
     OriginVisitStatusRow,
     RawExtrinsicMetadataByIdRow,
     RawExtrinsicMetadataRow,
     RevisionParentRow,
+    RevisionRow,
     SkippedContentRow,
     SnapshotBranchRow,
     SnapshotRow,
 )
 from .schema import HASH_ALGORITHMS
 
 # Max block size of contents to return
 BULK_BLOCK_CONTENT_LEN_MAX = 10000
 
 DIRECTORY_ENTRIES_INSERT_ALGOS = ["one-by-one", "concurrent", "batch"]
 
 
+TResult = TypeVar("TResult")
+TRow = TypeVar("TRow", bound=BaseRow)
+
+
+def _get_paginated_sha1_partition(
+    partition_id: int,
+    nb_partitions: int,
+    page_token: Optional[str],
+    limit: int,
+    get_range: Callable[[int, int, int], Iterator[Tuple[int, TRow]]],
+    convert: Callable[[TRow], TResult],
+    skip_row: Callable[[TRow], bool] = lambda row: False,
+) -> PagedResult[TResult]:
+    """Implements the bulk of ``content_get_partition``, ``directory_get_partition``,
+    ...:
+
+    1. computes range bounds
+    2. applies pagination token
+    3. converts to final objects
+    4. extracts next pagination token
+    """
+    if limit is None:
+        raise StorageArgumentException("limit should not be None")
+
+    # Compute start and end of the range of tokens covered by the
+    # requested partition
+    partition_size = (TOKEN_END - TOKEN_BEGIN) // nb_partitions
+    range_start = TOKEN_BEGIN + partition_id * partition_size
+    range_end = TOKEN_BEGIN + (partition_id + 1) * partition_size
+
+    # offset the range start according to the `page_token`.
+    if page_token is not None:
+        if not (range_start <= int(page_token) <= range_end):
+            raise StorageArgumentException("Invalid page_token.")
+        range_start = int(page_token)
+
+    next_page_token: Optional[str] = None
+
+    rows = get_range(range_start, range_end, limit + 1)
+    results = []
+    for counter, (tok, row) in enumerate(rows):
+        if skip_row(row):
+            continue
+        if counter >= limit:
+            next_page_token = str(tok)
+            break
+        results.append(convert(row))
+
+    assert len(results) <= limit
+    return PagedResult(results=results, next_page_token=next_page_token)
+
+
 class CassandraStorage:
     def __init__(
         self,
         hosts,
         keyspace,
         objstorage,
         port=9042,
@@ -303,47 +359,31 @@
     def content_get_partition(
         self,
         partition_id: int,
         nb_partitions: int,
         page_token: Optional[str] = None,
         limit: int = 1000,
     ) -> PagedResult[Content]:
-        if limit is None:
-            raise StorageArgumentException("limit should not be None")
-
-        # Compute start and end of the range of tokens covered by the
-        # requested partition
-        partition_size = (TOKEN_END - TOKEN_BEGIN) // nb_partitions
-        range_start = TOKEN_BEGIN + partition_id * partition_size
-        range_end = TOKEN_BEGIN + (partition_id + 1) * partition_size
-
-        # offset the range start according to the `page_token`.
-        if page_token is not None:
-            if not (range_start <= int(page_token) <= range_end):
-                raise StorageArgumentException("Invalid page_token.")
-            range_start = int(page_token)
-
-        next_page_token: Optional[str] = None
-
-        rows = self._cql_runner.content_get_token_range(
-            range_start, range_end, limit + 1
-        )
-        contents = []
-        for counter, (tok, row) in enumerate(rows):
-            if row.status == "absent":
-                continue
+        def convert(row: ContentRow) -> Content:
             row_d = row.to_dict()
-            if counter >= limit:
-                next_page_token = str(tok)
-                break
             row_d.pop("ctime")
-            contents.append(Content(**row_d))
+            return Content(**row_d)
+
+        def is_absent(row: ContentRow) -> bool:
+            return row.status == "absent"
 
-        assert len(contents) <= limit
-        return PagedResult(results=contents, next_page_token=next_page_token)
+        return _get_paginated_sha1_partition(
+            partition_id,
+            nb_partitions,
+            page_token,
+            limit,
+            self._cql_runner.content_get_token_range,
+            convert,
+            skip_row=is_absent,
+        )
 
     def content_get(
         self, contents: List[bytes], algo: str = "sha1"
     ) -> List[Optional[Content]]:
         if algo not in DEFAULT_ALGORITHMS:
             raise StorageArgumentException(
                 "algo should be one of {','.join(DEFAULT_ALGORITHMS)}"
@@ -711,14 +751,30 @@
         }
 
     def directory_get_random(self) -> Sha1Git:
         directory = self._cql_runner.directory_get_random()
         assert directory, "Could not find any directory"
         return directory.id
 
+    def directory_get_id_partition(
+        self,
+        partition_id: int,
+        nb_partitions: int,
+        page_token: Optional[str] = None,
+        limit: int = 1000,
+    ) -> PagedResult[Sha1Git]:
+        return _get_paginated_sha1_partition(
+            partition_id,
+            nb_partitions,
+            page_token,
+            limit,
+            self._cql_runner.directory_get_token_range,
+            operator.attrgetter("id"),
+        )
+
     ##########################
     # Revision
     ##########################
 
     def revision_add(self, revisions: List[Revision]) -> Dict[str, int]:
         # Filter-out revisions already in the database
         if not self._allow_overwrite:
@@ -814,28 +870,55 @@
                 # parent_rank is the clustering key, so results are already
                 # sorted by rank.
 
                 rev = converters.revision_from_db(row, parents=parents)
                 yield rev.to_dict()
                 yield from self._get_parent_revs(parents, seen, limit, short)
 
+    def revision_get_partition(
+        self,
+        partition_id: int,
+        nb_partitions: int,
+        page_token: Optional[str] = None,
+        limit: int = 1000,
+    ) -> PagedResult[Revision]:
+        def convert(row: RevisionRow) -> Revision:
+            return converters.revision_from_db(
+                row, parents=tuple(self._cql_runner.revision_parent_get(row.id))
+            )
+
+        return _get_paginated_sha1_partition(
+            partition_id,
+            nb_partitions,
+            page_token,
+            limit,
+            self._cql_runner.revision_get_token_range,
+            convert,
+        )
+
     def revision_log(
         self,
         revisions: List[Sha1Git],
         ignore_displayname: bool = False,
         limit: Optional[int] = None,
     ) -> Iterable[Optional[Dict[str, Any]]]:
         seen: Set[Sha1Git] = set()
-        yield from self._get_parent_revs(revisions, seen, limit, False)
+        yield from cast(
+            Iterable[Optional[Dict[str, Any]]],
+            self._get_parent_revs(revisions, seen, limit, short=False),
+        )
 
     def revision_shortlog(
         self, revisions: List[Sha1Git], limit: Optional[int] = None
     ) -> Iterable[Optional[Tuple[Sha1Git, Tuple[Sha1Git, ...]]]]:
         seen: Set[Sha1Git] = set()
-        yield from self._get_parent_revs(revisions, seen, limit, True)
+        yield from cast(
+            Iterable[Optional[Tuple[Sha1Git, Tuple[Sha1Git, ...]]]],
+            self._get_parent_revs(revisions, seen, limit, short=True),
+        )
 
     def revision_get_random(self) -> Sha1Git:
         revision = self._cql_runner.revision_get_random()
         assert revision, "Could not find any revision"
         return revision.id
 
     ##########################
@@ -865,14 +948,30 @@
         rels: Dict[Sha1Git, Release] = {}
         for row in rows:
             release = converters.release_from_db(row)
             rels[row.id] = release
 
         return [rels.get(rel_id) for rel_id in releases]
 
+    def release_get_partition(
+        self,
+        partition_id: int,
+        nb_partitions: int,
+        page_token: Optional[str] = None,
+        limit: int = 1000,
+    ) -> PagedResult[Release]:
+        return _get_paginated_sha1_partition(
+            partition_id,
+            nb_partitions,
+            page_token,
+            limit,
+            self._cql_runner.release_get_token_range,
+            lambda row: converters.release_from_db(row),
+        )
+
     def release_get_random(self) -> Sha1Git:
         release = self._cql_runner.release_get_random()
         assert release, "Could not find any release"
         return release.id
 
     ##########################
     # Snapshot
@@ -923,14 +1022,30 @@
             "branches": {
                 name: branch.to_dict() if branch else None
                 for (name, branch) in d["branches"].items()
             },
             "next_branch": d["next_branch"],
         }
 
+    def snapshot_get_id_partition(
+        self,
+        partition_id: int,
+        nb_partitions: int,
+        page_token: Optional[str] = None,
+        limit: int = 1000,
+    ) -> PagedResult[Sha1Git]:
+        return _get_paginated_sha1_partition(
+            partition_id,
+            nb_partitions,
+            page_token,
+            limit,
+            self._cql_runner.snapshot_get_token_range,
+            operator.attrgetter("id"),
+        )
+
     def snapshot_count_branches(
         self,
         snapshot_id: Sha1Git,
         branch_name_exclude_prefix: Optional[bytes] = None,
     ) -> Optional[Dict[Optional[str], int]]:
         if self._cql_runner.snapshot_missing([snapshot_id]):
             # Makes sure we don't fetch branches for a snapshot that is
```

### Comparing `swh.storage-1.8.0/swh/storage/cli.py` & `swh.storage-1.9.0/swh/storage/cli.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/exc.py` & `swh.storage-1.9.0/swh/storage/exc.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/fixer.py` & `swh.storage-1.9.0/swh/storage/fixer.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/in_memory.py` & `swh.storage-1.9.0/swh/storage/in_memory.py`

 * *Files 3% similar despite different names*

```diff
@@ -169,14 +169,26 @@
         self._metadata_authorities = Table(MetadataAuthorityRow)
         self._metadata_fetchers = Table(MetadataFetcherRow)
         self._raw_extrinsic_metadata = Table(RawExtrinsicMetadataRow)
         self._raw_extrinsic_metadata_by_id = Table(RawExtrinsicMetadataByIdRow)
         self._extid = Table(ExtIDRow)
         self._stat_counters = defaultdict(int)
 
+    def _get_token_range(
+        self, table: Table[TRow], start: int, end: int, limit: int
+    ) -> Iterator[Tuple[int, TRow]]:
+        matches = [
+            (token, row)
+            for (token, partition) in table.data.items()
+            for (clustering_key, row) in partition.items()
+            if start <= token <= end
+        ]
+        matches.sort()
+        return iter(matches[0:limit])
+
     def increment_counter(self, object_type: str, nb: int):
         self._stat_counters[object_type] += nb
 
     def stat_counters(self) -> Iterable[ObjectCountRow]:
         for (object_type, count) in self._stat_counters.items():
             yield ObjectCountRow(partition_key=0, object_type=object_type, count=count)
 
@@ -206,22 +218,15 @@
 
     def content_get_token_range(
         self,
         start: int,
         end: int,
         limit: int,
     ) -> Iterable[Tuple[int, ContentRow]]:
-        matches = [
-            (token, row)
-            for (token, partition) in self._contents.data.items()
-            for (clustering_key, row) in partition.items()
-            if start <= token <= end
-        ]
-        matches.sort()
-        return matches[0:limit]
+        return self._get_token_range(self._contents, start, end, limit)
 
     def content_missing_from_all_hashes(
         self, contents_hashes: List[Dict[str, bytes]]
     ) -> Iterator[Dict[str, bytes]]:
         for content_hashes in contents_hashes:
             if not self.content_get_from_pk(content_hashes):
                 yield content_hashes
@@ -304,14 +309,22 @@
 
     def directory_get(self, directory_ids: List[Sha1Git]) -> Iterable[DirectoryRow]:
         for id_ in directory_ids:
             row = self._directories.get_from_primary_key((id_,))
             if row:
                 yield row
 
+    def directory_get_token_range(
+        self,
+        start: int,
+        end: int,
+        limit: int,
+    ) -> Iterable[Tuple[int, DirectoryRow]]:
+        return self._get_token_range(self._directories, start, end, limit)
+
     ##########################
     # 'directory_entry' table
     ##########################
 
     def directory_entry_add_one(self, entry: DirectoryEntryRow) -> None:
         self._directory_entries.insert(entry)
 
@@ -355,14 +368,22 @@
         self, revision_ids: List[Sha1Git], ignore_displayname: bool = False
     ) -> Iterable[RevisionRow]:
         for id_ in revision_ids:
             row = self._revisions.get_from_primary_key((id_,))
             if row:
                 yield row
 
+    def revision_get_token_range(
+        self,
+        start: int,
+        end: int,
+        limit: int,
+    ) -> Iterable[Tuple[int, RevisionRow]]:
+        return self._get_token_range(self._revisions, start, end, limit)
+
     def revision_get_random(self) -> Optional[RevisionRow]:
         return self._revisions.get_random()
 
     ##########################
     # 'revision_parent' table
     ##########################
 
@@ -392,14 +413,22 @@
         self, release_ids: List[str], ignore_displayname: bool = False
     ) -> Iterable[ReleaseRow]:
         for id_ in release_ids:
             row = self._releases.get_from_primary_key((id_,))
             if row:
                 yield row
 
+    def release_get_token_range(
+        self,
+        start: int,
+        end: int,
+        limit: int,
+    ) -> Iterable[Tuple[int, ReleaseRow]]:
+        return self._get_token_range(self._releases, start, end, limit)
+
     def release_get_random(self) -> Optional[ReleaseRow]:
         return self._releases.get_random()
 
     ##########################
     # 'snapshot' table
     ##########################
 
@@ -410,14 +439,22 @@
                 missing.append(id_)
         return missing
 
     def snapshot_add_one(self, snapshot: SnapshotRow) -> None:
         self._snapshots.insert(snapshot)
         self.increment_counter("snapshot", 1)
 
+    def snapshot_get_token_range(
+        self,
+        start: int,
+        end: int,
+        limit: int,
+    ) -> Iterable[Tuple[int, SnapshotRow]]:
+        return self._get_token_range(self._snapshots, start, end, limit)
+
     def snapshot_get_random(self) -> Optional[SnapshotRow]:
         return self._snapshots.get_random()
 
     ##########################
     # 'snapshot_branch' table
     ##########################
```

### Comparing `swh.storage-1.8.0/swh/storage/interface.py` & `swh.storage-1.9.0/swh/storage/interface.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2015-2022  The Software Heritage developers
+# Copyright (C) 2015-2023  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import datetime
 from enum import Enum
 from typing import Any, Dict, Iterable, List, Optional, Sequence, Tuple, TypeVar, Union
@@ -504,14 +504,41 @@
         """Finds a random directory id.
 
         Returns:
             a sha1_git
         """
         ...
 
+    @remote_api_endpoint("directory/partition/id")
+    def directory_get_id_partition(
+        self,
+        partition_id: int,
+        nb_partitions: int,
+        page_token: Optional[str] = None,
+        limit: int = 1000,
+    ) -> PagedResult[Sha1Git]:
+        """Splits directories into nb_partitions, and returns all the ids and
+        raw manifests in one of these based on partition_id (which must be in
+        [0, nb_partitions-1]).
+        This does not return directory entries themselves; they should be
+        retrieved using :meth:`directory_get_entries` and
+        :meth:`directory_get_raw_manifest` instead.
+
+        There is no guarantee on how the partitioning is done, or the
+        result order.
+
+        Args:
+            partition_id: index of the partition to fetch
+            nb_partitions: total number of partitions to split into
+
+        Returns:
+            Page of the directories' sha1_git hashes.
+        """
+        ...
+
     ##########################
     # Revision
     ##########################
 
     @remote_api_endpoint("revision/add")
     def revision_add(self, revisions: List[Revision]) -> Dict[str, int]:
         """Add revisions to the storage
@@ -561,14 +588,38 @@
 
         Yields:
             missing revision ids
 
         """
         ...
 
+    @remote_api_endpoint("revision/partition")
+    def revision_get_partition(
+        self,
+        partition_id: int,
+        nb_partitions: int,
+        page_token: Optional[str] = None,
+        limit: int = 1000,
+    ) -> PagedResult[Revision]:
+        """Splits revisions into nb_partitions, and returns one of these based on
+        partition_id (which must be in [0, nb_partitions-1])
+
+        There is no guarantee on how the partitioning is done, or the
+        result order.
+
+        Args:
+            partition_id: index of the partition to fetch
+            nb_partitions: total number of partitions to split into
+
+        Returns:
+            Page of Revision model objects within the partition.
+
+        """
+        ...
+
     @remote_api_endpoint("revision")
     def revision_get(
         self, revision_ids: List[Sha1Git], ignore_displayname: bool = False
     ) -> List[Optional[Revision]]:
         """Get revisions from storage
 
         Args:
@@ -759,14 +810,38 @@
         """Finds a random release id.
 
         Returns:
             a sha1_git
         """
         ...
 
+    @remote_api_endpoint("release/partition")
+    def release_get_partition(
+        self,
+        partition_id: int,
+        nb_partitions: int,
+        page_token: Optional[str] = None,
+        limit: int = 1000,
+    ) -> PagedResult[Release]:
+        """Splits releases into nb_partitions, and returns one of these based on
+        partition_id (which must be in [0, nb_partitions-1])
+
+        There is no guarantee on how the partitioning is done, or the
+        result order.
+
+        Args:
+            partition_id: index of the partition to fetch
+            nb_partitions: total number of partitions to split into
+
+        Returns:
+            Page of Release model objects within the partition.
+
+        """
+        ...
+
     ##########################
     # Snapshot
     ##########################
 
     @remote_api_endpoint("snapshot/add")
     def snapshot_add(self, snapshots: List[Snapshot]) -> Dict[str, int]:
         """Add snapshots to the storage.
@@ -906,14 +981,40 @@
         """Finds a random snapshot id.
 
         Returns:
             a sha1_git
         """
         ...
 
+    @remote_api_endpoint("snapshot/partition/id")
+    def snapshot_get_id_partition(
+        self,
+        partition_id: int,
+        nb_partitions: int,
+        page_token: Optional[str] = None,
+        limit: int = 1000,
+    ) -> PagedResult[Sha1Git]:
+        """Splits directories into nb_partitions, and returns all the ids and
+        raw manifests in one of these based on partition_id (which must be in
+        [0, nb_partitions-1]).
+        This does not return directory entries themselves; they should be
+        retrieved using :meth:`snapshot_get_branches` instead.
+
+        There is no guarantee on how the partitioning is done, or the
+        result order.
+
+        Args:
+            partition_id: index of the partition to fetch
+            nb_partitions: total number of partitions to split into
+
+        Returns:
+            Page of the snapshots' sha1_git hashes
+        """
+        ...
+
     ##########################
     # OriginVisit and OriginVisitStatus
     ##########################
 
     @remote_api_endpoint("origin/visit/add")
     def origin_visit_add(self, visits: List[OriginVisit]) -> Iterable[OriginVisit]:
         """Add visits to storage. If the visits have no id, they will be created and assigned
```

### Comparing `swh.storage-1.8.0/swh/storage/metrics.py` & `swh.storage-1.9.0/swh/storage/metrics.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/migrate_extrinsic_metadata.py` & `swh.storage-1.9.0/swh/storage/migrate_extrinsic_metadata.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/objstorage.py` & `swh.storage-1.9.0/swh/storage/objstorage.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/postgresql/converters.py` & `swh.storage-1.9.0/swh/storage/postgresql/converters.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/postgresql/db.py` & `swh.storage-1.9.0/swh/storage/postgresql/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import datetime
 import logging
 import random
-from typing import Any, Dict, Iterable, List, Optional, Tuple
+from typing import Any, Dict, Iterable, Iterator, List, Optional, Tuple
 
 from swh.core.db import BaseDb
 from swh.core.db.db_utils import execute_values_generator
 from swh.core.db.db_utils import jsonize as _jsonize
 from swh.core.db.db_utils import stored_procedure
 from swh.model.hashutil import DEFAULT_ALGORITHMS
 from swh.model.model import SHA1_SIZE, OriginVisit, OriginVisitStatus, Sha1Git
@@ -138,15 +138,15 @@
         """
         yield from execute_values_generator(
             cur,
             query,
             ((hash_,) for hash_ in hashes),
         )
 
-    def content_get_range(self, start, end, limit=None, cur=None):
+    def content_get_range(self, start, end, limit=None, cur=None) -> Iterator[Tuple]:
         """Retrieve contents within range [start, end]."""
         cur = self._cursor(cur)
         query = """select %s from content
                    where %%s <= sha1 and sha1 <= %%s
                    order by sha1
                    limit %%s""" % ", ".join(
             self.content_get_metadata_keys
@@ -362,14 +362,28 @@
             """
             SELECT t.id, raw_manifest FROM (VALUES %s) as t(id)
             INNER JOIN directory ON (t.id=directory.id)
             """,
             ((id_,) for id_ in directory_ids),
         )
 
+    def directory_get_id_range(
+        self, start, end, limit=None, cur=None
+    ) -> Iterator[Tuple[Sha1Git]]:
+        cur = self._cursor(cur)
+        cur.execute(
+            """
+            SELECT id FROM directory
+            WHERE %s <= id AND id <= %s
+            LIMIT %s
+            """,
+            (start, end, limit),
+        )
+        yield from cur
+
     def directory_get_random(self, cur=None):
         return self._get_random_row_from_table("directory", ["id"], "id", cur)
 
     ##########################
     # 'revision' table
     ##########################
 
@@ -411,23 +425,23 @@
         "extra_headers",
         "raw_manifest",
     ]
 
     revision_get_cols = revision_add_cols + ["parents"]
 
     @staticmethod
-    def mangle_query_key(key, main_table, ignore_displayname=False):
+    def mangle_query_key(key, main_table, id_col, ignore_displayname=False):
         if key == "id":
-            return "t.id"
+            return id_col
         if key == "parents":
-            return """
+            return f"""
             ARRAY(
             SELECT rh.parent_id::bytea
             FROM revision_history rh
-            WHERE rh.id = t.id
+            WHERE rh.id = {id_col}
             ORDER BY rh.parent_rank
             )"""
 
         if "_" not in key:
             return f"{main_table}.{key}"
 
         head, tail = key.split("_", 1)
@@ -459,15 +473,15 @@
 
         assert False, "All cases should have been handled here"
 
     def revision_get_from_list(self, revisions, ignore_displayname=False, cur=None):
         cur = self._cursor(cur)
 
         query_keys = ", ".join(
-            self.mangle_query_key(k, "revision", ignore_displayname)
+            self.mangle_query_key(k, "revision", "t.id", ignore_displayname)
             for k in self.revision_get_cols
         )
 
         yield from execute_values_generator(
             cur,
             """
             SELECT %s FROM (VALUES %%s) as t(sortkey, id)
@@ -476,14 +490,35 @@
             LEFT JOIN person committer ON revision.committer = committer.id
             ORDER BY sortkey
             """
             % query_keys,
             ((sortkey, id) for sortkey, id in enumerate(revisions)),
         )
 
+    def revision_get_range(self, start, end, limit, cur=None) -> Iterator[Tuple]:
+        cur = self._cursor(cur)
+
+        query_keys = ", ".join(
+            self.mangle_query_key(k, "revision", "revision.id")
+            for k in self.revision_get_cols
+        )
+
+        cur.execute(
+            """
+            SELECT %s FROM revision
+            LEFT JOIN person author ON revision.author = author.id
+            LEFT JOIN person committer ON revision.committer = committer.id
+            WHERE %%s <= revision.id AND revision.id <= %%s
+            LIMIT %%s
+            """
+            % query_keys,
+            (start, end, limit),
+        )
+        yield from cur
+
     def revision_log(
         self, root_revisions, ignore_displayname=False, limit=None, cur=None
     ):
         cur = self._cursor(cur)
 
         query = """\
         SELECT %s
@@ -520,15 +555,15 @@
     extid_cols = ["extid", "extid_version", "extid_type", "target", "target_type"]
 
     def extid_get_from_extid_list(
         self, extid_type: str, ids: List[bytes], version: Optional[int] = None, cur=None
     ):
         cur = self._cursor(cur)
         query_keys = ", ".join(
-            self.mangle_query_key(k, "extid") for k in self.extid_cols
+            self.mangle_query_key(k, "extid", "t.id") for k in self.extid_cols
         )
         filter_query = ""
         if version is not None:
             filter_query = cur.mogrify(
                 f"WHERE extid_version={version}", (version,)
             ).decode()
 
@@ -555,15 +590,15 @@
         cur=None,
     ):
         cur = self._cursor(cur)
         target_type = ObjectType(
             target_type
         ).name.lower()  # aka "rev" -> "revision", ...
         query_keys = ", ".join(
-            self.mangle_query_key(k, "extid") for k in self.extid_cols
+            self.mangle_query_key(k, "extid", "t.id") for k in self.extid_cols
         )
         filter_query = ""
         if extid_version is not None and extid_type is not None:
             filter_query = cur.mogrify(
                 "WHERE extid_version=%s AND extid_type=%s",
                 (
                     extid_version,
@@ -620,15 +655,15 @@
         "author_email",
     ]
     release_get_cols = release_add_cols
 
     def release_get_from_list(self, releases, ignore_displayname=False, cur=None):
         cur = self._cursor(cur)
         query_keys = ", ".join(
-            self.mangle_query_key(k, "release", ignore_displayname)
+            self.mangle_query_key(k, "release", "t.id", ignore_displayname)
             for k in self.release_get_cols
         )
 
         yield from execute_values_generator(
             cur,
             """
             SELECT %s FROM (VALUES %%s) as t(sortkey, id)
@@ -636,14 +671,34 @@
             LEFT JOIN person author ON release.author = author.id
             ORDER BY sortkey
             """
             % query_keys,
             ((sortkey, id) for sortkey, id in enumerate(releases)),
         )
 
+    def release_get_range(self, start, end, limit, cur=None) -> Iterator[Tuple]:
+        cur = self._cursor(cur)
+
+        query_keys = ", ".join(
+            self.mangle_query_key(k, "release", "release.id")
+            for k in self.release_get_cols
+        )
+
+        cur.execute(
+            """
+            SELECT %s FROM release
+            LEFT JOIN person author ON release.author = author.id
+            WHERE %%s <= release.id AND release.id <= %%s
+            LIMIT %%s
+            """
+            % query_keys,
+            (start, end, limit),
+        )
+        yield from cur
+
     def release_get_random(self, cur=None):
         return self._get_random_row_from_table("release", ["id"], "id", cur)
 
     ##########################
     # 'snapshot' table
     ##########################
 
@@ -723,14 +778,29 @@
                 branch_name_include_substring,
                 branch_name_exclude_prefix,
             ),
         )
 
         yield from cur
 
+    def snapshot_get_id_range(
+        self, start, end, limit=None, cur=None
+    ) -> Iterator[Tuple[Sha1Git]]:
+        cur = self._cursor(cur)
+        cur.execute(
+            """
+            SELECT id FROM snapshot
+            WHERE %s <= id AND id <= %s
+            LIMIT %s
+            """,
+            (start, end, limit),
+        )
+
+        yield from cur
+
     def snapshot_get_random(self, cur=None):
         return self._get_random_row_from_table("snapshot", ["id"], "id", cur)
 
     ##########################
     # 'origin_visit' and 'origin_visit_status' tables
     ##########################
```

### Comparing `swh.storage-1.8.0/swh/storage/postgresql/storage.py` & `swh.storage-1.9.0/swh/storage/postgresql/storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,28 @@
 from collections import defaultdict
 import contextlib
 from contextlib import contextmanager
 import datetime
 import itertools
 import logging
 import operator
-from typing import Any, Counter, Dict, Iterable, List, Optional, Sequence, Tuple, Union
+from typing import (
+    Any,
+    Callable,
+    Counter,
+    Dict,
+    Iterable,
+    Iterator,
+    List,
+    Optional,
+    Sequence,
+    Tuple,
+    TypeVar,
+    Union,
+)
 
 import attr
 import psycopg2
 import psycopg2.errors
 import psycopg2.pool
 
 from swh.core.api.serializers import msgpack_dumps, msgpack_loads
@@ -108,14 +121,65 @@
         # a subclass of IntegrityError; so we need to catch and reraise it
         # before the next clause converts it to StorageArgumentException.
         raise
     except VALIDATION_EXCEPTIONS as e:
         raise StorageArgumentException(str(e))
 
 
+TRow = TypeVar("TRow", bound=Tuple)
+TResult = TypeVar("TResult")
+
+
+def _get_paginated_sha1_partition(
+    cur,
+    partition_id: int,
+    nb_partitions: int,
+    page_token: Optional[str],
+    limit: int,
+    get_range: Callable[[bytes, bytes, int, Any], Iterator[TRow]],
+    convert: Callable[[TRow], TResult],
+    get_id: Optional[Callable[[TResult], Any]] = None,
+) -> PagedResult[TResult]:
+    """Implements the bulk of ``content_get_partition``, ``directory_get_partition``,
+    ...:
+
+    1. computes range bounds
+    2. applies pagination token
+    3. converts to final objects
+    4. extracts next pagination token
+    """
+    if limit is None:
+        raise StorageArgumentException("limit should not be None")
+    if get_id is None:
+
+        def get_id(obj: TResult):
+            return obj.id  # type: ignore[attr-defined]
+
+    assert get_id is not None  # to please mypy
+
+    (start, end) = get_partition_bounds_bytes(partition_id, nb_partitions, SHA1_SIZE)
+    if page_token:
+        start = hash_to_bytes(page_token)
+    if end is None:
+        end = b"\xff" * SHA1_SIZE
+
+    next_page_token: Optional[str] = None
+    results = []
+    for counter, row in enumerate(get_range(start, end, limit + 1, cur)):
+        result = convert(row)
+        if counter >= limit:
+            # take the last content for the next page starting from this
+            next_page_token = hash_to_hex(get_id(result))
+            break
+        results.append(result)
+
+    assert len(results) <= limit
+    return PagedResult(results=results, next_page_token=next_page_token)
+
+
 class Storage:
     """SWH storage datastore proxy, encompassing DB and object storage"""
 
     current_version: int = 186
 
     def __init__(
         self,
@@ -367,37 +431,24 @@
         nb_partitions: int,
         page_token: Optional[str] = None,
         limit: int = 1000,
         *,
         db: Db,
         cur=None,
     ) -> PagedResult[Content]:
-        if limit is None:
-            raise StorageArgumentException("limit should not be None")
-        (start, end) = get_partition_bounds_bytes(
-            partition_id, nb_partitions, SHA1_SIZE
-        )
-        if page_token:
-            start = hash_to_bytes(page_token)
-        if end is None:
-            end = b"\xff" * SHA1_SIZE
-
-        next_page_token: Optional[str] = None
-        contents = []
-        for counter, row in enumerate(db.content_get_range(start, end, limit + 1, cur)):
-            row_d = dict(zip(db.content_get_metadata_keys, row))
-            content = Content(**row_d)
-            if counter >= limit:
-                # take the last content for the next page starting from this
-                next_page_token = hash_to_hex(content.sha1)
-                break
-            contents.append(content)
-
-        assert len(contents) <= limit
-        return PagedResult(results=contents, next_page_token=next_page_token)
+        return _get_paginated_sha1_partition(
+            cur,
+            partition_id,
+            nb_partitions,
+            page_token,
+            limit,
+            db.content_get_range,
+            lambda row: Content(**dict(zip(db.content_get_metadata_keys, row))),
+            lambda row: row.sha1,
+        )
 
     @db_transaction(statement_timeout=500)
     def content_get(
         self, contents: List[bytes], algo: str = "sha1", *, db: Db, cur=None
     ) -> List[Optional[Content]]:
         contents_by_hash: Dict[bytes, Optional[Content]] = {}
         if algo not in DEFAULT_ALGORITHMS:
@@ -669,14 +720,36 @@
 
     @db_transaction()
     def directory_get_raw_manifest(
         self, directory_ids: List[Sha1Git], *, db: Db, cur=None
     ) -> Dict[Sha1Git, Optional[bytes]]:
         return dict(db.directory_get_raw_manifest(directory_ids, cur=cur))
 
+    @db_transaction()
+    def directory_get_id_partition(
+        self,
+        partition_id: int,
+        nb_partitions: int,
+        page_token: Optional[str] = None,
+        limit: int = 1000,
+        *,
+        db: Db,
+        cur=None,
+    ) -> PagedResult[Sha1Git]:
+        return _get_paginated_sha1_partition(
+            cur,
+            partition_id,
+            nb_partitions,
+            page_token,
+            limit,
+            db.directory_get_id_range,
+            operator.itemgetter(0),
+            lambda id_: id_,
+        )
+
     ##########################
     # Revision
     ##########################
 
     @db_transaction()
     def revision_add(
         self, revisions: List[Revision], *, db: Db, cur=None
@@ -730,14 +803,35 @@
     ) -> Iterable[Sha1Git]:
         if not revisions:
             return None
 
         for obj in db.revision_missing_from_list(revisions, cur):
             yield obj[0]
 
+    @db_transaction()
+    def revision_get_partition(
+        self,
+        partition_id: int,
+        nb_partitions: int,
+        page_token: Optional[str] = None,
+        limit: int = 1000,
+        *,
+        db: Db,
+        cur=None,
+    ) -> PagedResult[Revision]:
+        return _get_paginated_sha1_partition(
+            cur,
+            partition_id,
+            nb_partitions,
+            page_token,
+            limit,
+            db.revision_get_range,
+            lambda row: converters.db_to_revision(dict(zip(db.revision_get_cols, row))),
+        )
+
     @db_transaction(statement_timeout=2000)
     def revision_get(
         self,
         revision_ids: List[Sha1Git],
         ignore_displayname: bool = False,
         *,
         db: Db,
@@ -909,14 +1003,35 @@
             rel = converters.db_to_optional_release(
                 dict(zip(db.release_get_cols, release))
             )
             rels.append(rel)
         return rels
 
     @db_transaction()
+    def release_get_partition(
+        self,
+        partition_id: int,
+        nb_partitions: int,
+        page_token: Optional[str] = None,
+        limit: int = 1000,
+        *,
+        db: Db,
+        cur=None,
+    ) -> PagedResult[Release]:
+        return _get_paginated_sha1_partition(
+            cur,
+            partition_id,
+            nb_partitions,
+            page_token,
+            limit,
+            db.release_get_range,
+            lambda row: converters.db_to_release(dict(zip(db.release_get_cols, row))),
+        )
+
+    @db_transaction()
     def release_get_random(self, *, db: Db, cur=None) -> Sha1Git:
         return db.release_get_random(cur)
 
     ##########################
     # Snapshot
     ##########################
 
@@ -976,14 +1091,36 @@
             "branches": {
                 name: branch.to_dict() if branch else None
                 for (name, branch) in d["branches"].items()
             },
             "next_branch": d["next_branch"],
         }
 
+    @db_transaction()
+    def snapshot_get_id_partition(
+        self,
+        partition_id: int,
+        nb_partitions: int,
+        page_token: Optional[str] = None,
+        limit: int = 1000,
+        *,
+        db: Db,
+        cur=None,
+    ) -> PagedResult[Sha1Git]:
+        return _get_paginated_sha1_partition(
+            cur,
+            partition_id,
+            nb_partitions,
+            page_token,
+            limit,
+            db.snapshot_get_id_range,
+            operator.itemgetter(0),
+            lambda id_: id_,
+        )
+
     @db_transaction(statement_timeout=2000)
     def snapshot_count_branches(
         self,
         snapshot_id: Sha1Git,
         branch_name_exclude_prefix: Optional[bytes] = None,
         *,
         db: Db,
```

### Comparing `swh.storage-1.8.0/swh/storage/proxies/buffer.py` & `swh.storage-1.9.0/swh/storage/proxies/buffer.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/proxies/counter.py` & `swh.storage-1.9.0/swh/storage/proxies/counter.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/proxies/filter.py` & `swh.storage-1.9.0/swh/storage/proxies/filter.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/proxies/retry.py` & `swh.storage-1.9.0/swh/storage/proxies/retry.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/proxies/tenacious.py` & `swh.storage-1.9.0/swh/storage/proxies/tenacious.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/proxies/validate.py` & `swh.storage-1.9.0/swh/storage/proxies/validate.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/pytest_plugin.py` & `swh.storage-1.9.0/swh/storage/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/replay.py` & `swh.storage-1.9.0/swh/storage/replay.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/10-superuser-init.sql` & `swh.storage-1.9.0/swh/storage/sql/10-superuser-init.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/15-flavor.sql` & `swh.storage-1.9.0/swh/storage/sql/15-flavor.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/20-enums.sql` & `swh.storage-1.9.0/swh/storage/sql/20-enums.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/30-schema.sql` & `swh.storage-1.9.0/swh/storage/sql/30-schema.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/40-funcs.sql` & `swh.storage-1.9.0/swh/storage/sql/40-funcs.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/60-indexes.sql` & `swh.storage-1.9.0/swh/storage/sql/60-indexes.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/logical_replication/replication_source.sql` & `swh.storage-1.9.0/swh/storage/sql/logical_replication/replication_source.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/015.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/015.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/016.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/016.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/017.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/017.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/018.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/018.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/019.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/019.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/020.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/020.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/021.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/021.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/022.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/022.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/023.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/023.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/024.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/024.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/025.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/025.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/026.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/026.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/027.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/027.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/028.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/028.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/029.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/029.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/030.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/030.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/032.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/032.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/033.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/033.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/034.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/034.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/035.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/035.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/036.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/036.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/037.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/037.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/038.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/038.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/039.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/039.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/040.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/040.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/041.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/041.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/042.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/042.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/043.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/043.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/044.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/044.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/046.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/046.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/047.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/047.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/048.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/048.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/049.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/049.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/050.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/050.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/051.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/051.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/052.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/052.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/053.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/053.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/054.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/054.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/055.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/055.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/056.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/056.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/057.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/057.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/058.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/058.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/059.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/059.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/060.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/060.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/061.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/061.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/062.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/062.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/063.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/063.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/064.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/064.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/065.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/065.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/067.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/067.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/068.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/068.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/069.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/069.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/071.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/071.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/072.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/072.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/073.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/073.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/074.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/074.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/075.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/075.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/076.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/076.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/077.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/077.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/078.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/078.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/079.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/079.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/080.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/080.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/081.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/081.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/082.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/082.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/083.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/083.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/084.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/084.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/085.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/085.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/086.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/086.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/087.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/087.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/088.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/088.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/089.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/089.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/090.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/090.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/091.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/091.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/092.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/092.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/093.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/093.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/094.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/094.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/095.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/095.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/096.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/096.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/097.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/097.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/099.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/099.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/100.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/100.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/101.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/101.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/102.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/102.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/103.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/103.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/104.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/104.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/105.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/105.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/106.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/106.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/107.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/107.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/108.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/108.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/109.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/109.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/110.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/110.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/111.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/111.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/112.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/112.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/113.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/113.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/114.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/114.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/115.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/115.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/117.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/117.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/118.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/118.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/119.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/119.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/120.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/120.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/123.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/123.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/124.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/124.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/125.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/125.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/127.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/127.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/128.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/128.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/129.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/129.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/130.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/130.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/134.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/134.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/136.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/136.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/137.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/137.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/138.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/138.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/139.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/139.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/143.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/143.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/146.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/146.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/147.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/147.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/148.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/148.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/149.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/149.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/150.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/150.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/154.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/154.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/155.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/155.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/156.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/156.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/157.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/157.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/158.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/158.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/159.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/159.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/160.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/160.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/161.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/161.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/162.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/162.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/163.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/163.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/167.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/167.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/168.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/168.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/169.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/169.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/170.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/170.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/171.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/171.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/172.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/172.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/173.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/173.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/175.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/175.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/176.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/176.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/179.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/179.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/180.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/180.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/181.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/181.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/182.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/182.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/183.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/183.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/184.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/184.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/sql/upgrades/185.sql` & `swh.storage-1.9.0/swh/storage/sql/upgrades/185.sql`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/tests/algos/test_diff.py` & `swh.storage-1.9.0/swh/storage/tests/algos/test_diff.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/tests/algos/test_dir_iterator.py` & `swh.storage-1.9.0/swh/storage/tests/algos/test_dir_iterator.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/tests/algos/test_directory.py` & `swh.storage-1.9.0/swh/storage/tests/algos/test_directory.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/tests/algos/test_origin.py` & `swh.storage-1.9.0/swh/storage/tests/algos/test_origin.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/tests/algos/test_revisions_walker.py` & `swh.storage-1.9.0/swh/storage/tests/algos/test_revisions_walker.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/tests/algos/test_snapshot.py` & `swh.storage-1.9.0/swh/storage/tests/algos/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/tests/conftest.py` & `swh.storage-1.9.0/swh/storage/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,17 +39,18 @@
 if pytest_cov is not None and int(pytest_cov.__version__.split(".")[0]) < 4:
     # pytest_cov + multiprocessing can cause a segmentation fault when starting
     # the child process <https://forge.softwareheritage.org/P706>; so we're
     # removing pytest-coverage's hook that runs when a child process starts.
     # This means code run in child processes won't be counted in the coverage
     # report, but this is not an issue because the only code that runs only in
     # child processes is the RPC server.
-    for (key, value) in multiprocessing.util._afterfork_registry.items():
+    registry = multiprocessing.util._afterfork_registry  # type: ignore[attr-defined]
+    for (key, value) in registry.items():
         if value is pytest_cov.embed.multiprocessing_start:
-            del multiprocessing.util._afterfork_registry[key]
+            del registry[key]
             break
     else:
         assert False, "missing pytest_cov.embed.multiprocessing_start?"
 
 
 @pytest.fixture
 def swh_storage_backend_config(swh_storage_backend_config):
```

### Comparing `swh.storage-1.8.0/swh/storage/tests/migrate_extrinsic_metadata/test_cran.py` & `swh.storage-1.9.0/swh/storage/tests/migrate_extrinsic_metadata/test_cran.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/tests/migrate_extrinsic_metadata/test_debian.py` & `swh.storage-1.9.0/swh/storage/tests/migrate_extrinsic_metadata/test_debian.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/tests/migrate_extrinsic_metadata/test_deposit.py` & `swh.storage-1.9.0/swh/storage/tests/migrate_extrinsic_metadata/test_deposit.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/tests/migrate_extrinsic_metadata/test_gnu.py` & `swh.storage-1.9.0/swh/storage/tests/migrate_extrinsic_metadata/test_gnu.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/tests/migrate_extrinsic_metadata/test_nixguix.py` & `swh.storage-1.9.0/swh/storage/tests/migrate_extrinsic_metadata/test_nixguix.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/tests/migrate_extrinsic_metadata/test_npm.py` & `swh.storage-1.9.0/swh/storage/tests/migrate_extrinsic_metadata/test_npm.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/tests/migrate_extrinsic_metadata/test_pypi.py` & `swh.storage-1.9.0/swh/storage/tests/migrate_extrinsic_metadata/test_pypi.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/tests/storage_data.py` & `swh.storage-1.9.0/swh/storage/tests/storage_data.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/tests/storage_tests.py` & `swh.storage-1.9.0/swh/storage/tests/storage_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,32 +18,31 @@
 import pytest
 
 from swh.core.api import RemoteException
 from swh.core.api.classes import stream_results
 from swh.model import from_disk, hypothesis_strategies
 from swh.model.hashutil import DEFAULT_ALGORITHMS, hash_to_bytes
 from swh.model.model import (
-    Content,
-    Directory,
-    DirectoryEntry,
-    ExtID,
     Origin,
     OriginVisit,
     OriginVisitStatus,
     Person,
     RawExtrinsicMetadata,
+    Release,
     Revision,
     RevisionType,
     SkippedContent,
     Snapshot,
     SnapshotBranch,
     TargetType,
     Timestamp,
     TimestampWithTimezone,
 )
+from swh.model.model import Content, Directory, DirectoryEntry, ExtID
+from swh.model.model import ObjectType as ModelObjectType
 from swh.model.swhids import CoreSWHID, ObjectType
 from swh.storage import get_storage
 from swh.storage.cassandra.storage import CassandraStorage
 from swh.storage.common import origin_url_to_sha1 as sha1
 from swh.storage.exc import (
     HashCollision,
     StorageArgumentException,
@@ -942,14 +941,50 @@
                 [b"name1"]
             )
 
         # used in TestCassandraStorage by
         # test_directory_add_raw_manifest__different_entries__allow_overwrite
         return dir1.id
 
+    def test_directory_get_id_partition(self, swh_storage, sample_data):
+        directories = list(sample_data.directories) + [
+            Directory(
+                entries=(
+                    DirectoryEntry(
+                        name=f"entry{i}".encode(),
+                        type="file",
+                        target=b"\x00" * 20,
+                        perms=0,
+                    ),
+                )
+            )
+            for i in range(100)
+        ]
+        swh_storage.directory_add(directories)
+
+        expected_results = {dir_.id for dir_ in directories}
+        # nb_partitions = smallest power of 2 such that at least one of
+        # the partitions is empty
+        nb_partitions = 1 << math.floor(math.log2(len(expected_results)) + 1)
+
+        actual_results = []
+
+        for i in range(nb_partitions):
+            result = list(
+                stream_results(swh_storage.directory_get_id_partition, i, nb_partitions)
+            )
+
+            # Technically not guaranteed, but it is statistically very unlikely
+            # all directories are in the same partition
+            assert len(result) < len(expected_results)
+
+            actual_results.extend(result)
+
+        assert set(actual_results) == expected_results
+
     def test_directory_ls_recursive(self, swh_storage, sample_data):
         # create consistent dataset regarding the directories we want to list
         content, content2 = sample_data.contents[:2]
         swh_storage.content_add([content, content2])
         dir1, dir2, dir3 = sample_data.directories[:3]
 
         dir_ids = [d.id for d in [dir1, dir2, dir3]]
@@ -1358,14 +1393,53 @@
         actual_revisions = swh_storage.revision_get([revision.id, revision2.id])
         assert actual_revisions == [revision, revision2]
 
         # order 2
         actual_revisions2 = swh_storage.revision_get([revision2.id, revision.id])
         assert actual_revisions2 == [revision2, revision]
 
+    def test_revision_get_partition(self, swh_storage, sample_data):
+        revisions = list(sample_data.revisions) + [
+            Revision(
+                message=f"hello{i}".encode(),
+                author=None,
+                date=None,
+                committer=None,
+                committer_date=None,
+                parents=(),
+                type=RevisionType.GIT,
+                directory=b"\x00" * 20,
+                synthetic=True,
+            )
+            for i in range(100)
+        ]
+        swh_storage.revision_add(revisions)
+
+        # nb_partitions = smallest power of 2 such that at least one of
+        # the partitions is empty
+        nb_partitions = 1 << math.floor(math.log2(len(revisions)) + 1)
+
+        actual_revisions = []
+
+        for i in range(nb_partitions):
+            result = list(
+                stream_results(swh_storage.revision_get_partition, i, nb_partitions)
+            )
+
+            # Technically not guaranteed, but it is statistically very unlikely
+            # all revisions are in the same partition
+            assert len(result) < len(revisions)
+
+            actual_revisions.extend(result)
+
+        # TODO: use set equality once Revision.metadata is removed
+        actual_revisions.sort(key=lambda rev: rev.id)
+        revisions.sort(key=lambda rev: rev.id)
+        assert actual_revisions == revisions
+
     def test_revision_log(self, swh_storage, sample_data):
         revision1, revision2, revision3, revision4 = sample_data.revisions[:4]
 
         # rev4 -is-child-of-> rev3 -> rev1, (rev2 -> rev1)
         swh_storage.revision_add([revision1, revision2, revision3, revision4])
 
         # when
@@ -1946,14 +2020,48 @@
         actual_releases = swh_storage.release_get([release.id, release2.id])
         assert actual_releases == [release, release2]
 
         # order 2
         actual_releases2 = swh_storage.release_get([release2.id, release.id])
         assert actual_releases2 == [release2, release]
 
+    def test_release_get_partition(self, swh_storage, sample_data):
+        releases = list(sample_data.releases) + [
+            Release(
+                name=f"release{i}".encode(),
+                message=f"hello{i}".encode(),
+                author=None,
+                date=None,
+                target=b"\x00" * 20,
+                target_type=ModelObjectType.REVISION,
+                synthetic=True,
+            )
+            for i in range(100)
+        ]
+        swh_storage.release_add(releases)
+
+        # nb_partitions = smallest power of 2 such that at least one of
+        # the partitions is empty
+        nb_partitions = 1 << math.floor(math.log2(len(releases)) + 1)
+
+        actual_releases = []
+
+        for i in range(nb_partitions):
+            result = list(
+                stream_results(swh_storage.release_get_partition, i, nb_partitions)
+            )
+
+            # Technically not guaranteed, but it is statistically very unlikely
+            # all releases are in the same partition
+            assert len(result) < len(releases)
+
+            actual_releases.extend(result)
+
+        assert set(actual_releases) == set(releases)
+
     def test_release_get_random(self, swh_storage, sample_data):
         release, release2, release3 = sample_data.releases[:3]
 
         swh_storage.release_add([release, release2, release3])
 
         assert swh_storage.release_get_random() in {
             release.id,
@@ -4674,14 +4782,48 @@
         assert actual_visit == ov1
 
         visit_status = swh_storage.origin_visit_status_get_latest(
             origin.url, ov1.visit, require_snapshot=True
         )
         assert visit_status.snapshot == snapshot.id
 
+    def test_snapshot_get_id_partition(self, swh_storage, sample_data):
+        snapshots = list(sample_data.snapshots) + [
+            Snapshot(
+                branches={
+                    f"branch{i}".encode(): SnapshotBranch(
+                        target=b"\x00" * 20,
+                        target_type=TargetType.REVISION,
+                    ),
+                },
+            )
+            for i in range(100)
+        ]
+        swh_storage.snapshot_add(snapshots)
+
+        expected_results = {snp.id for snp in snapshots}
+        # nb_partitions = smallest power of 2 such that at least one of
+        # the partitions is empty
+        nb_partitions = 1 << math.floor(math.log2(len(expected_results)) + 1)
+
+        actual_results = []
+
+        for i in range(nb_partitions):
+            result = list(
+                stream_results(swh_storage.snapshot_get_id_partition, i, nb_partitions)
+            )
+
+            # Technically not guaranteed, but it is statistically very unlikely
+            # all snapshots are in the same partition
+            assert len(result) < len(expected_results)
+
+            actual_results.extend(result)
+
+        assert set(actual_results) == expected_results
+
     def test_snapshot_get_random(self, swh_storage, sample_data):
         snapshot, empty_snapshot, complete_snapshot = sample_data.snapshots[:3]
         swh_storage.snapshot_add([snapshot, empty_snapshot, complete_snapshot])
 
         assert swh_storage.snapshot_get_random() in {
             snapshot.id,
             empty_snapshot.id,
```

### Comparing `swh.storage-1.8.0/swh/storage/tests/test_api_client.py` & `swh.storage-1.9.0/swh/storage/tests/test_api_client.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/tests/test_backfill.py` & `swh.storage-1.9.0/swh/storage/tests/test_backfill.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/tests/test_buffer.py` & `swh.storage-1.9.0/swh/storage/tests/test_buffer.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/tests/test_cassandra.py` & `swh.storage-1.9.0/swh/storage/tests/test_cassandra.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/tests/test_cassandra_converters.py` & `swh.storage-1.9.0/swh/storage/tests/test_cassandra_converters.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/tests/test_cassandra_migration.py` & `swh.storage-1.9.0/swh/storage/tests/test_cassandra_migration.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/tests/test_cli.py` & `swh.storage-1.9.0/swh/storage/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/tests/test_counter.py` & `swh.storage-1.9.0/swh/storage/tests/test_counter.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/tests/test_exception.py` & `swh.storage-1.9.0/swh/storage/tests/test_exception.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/tests/test_filter.py` & `swh.storage-1.9.0/swh/storage/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/tests/test_in_memory.py` & `swh.storage-1.9.0/swh/storage/tests/test_in_memory.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/tests/test_init.py` & `swh.storage-1.9.0/swh/storage/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/tests/test_kafka_writer.py` & `swh.storage-1.9.0/swh/storage/tests/test_kafka_writer.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/tests/test_metrics.py` & `swh.storage-1.9.0/swh/storage/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/tests/test_postgresql.py` & `swh.storage-1.9.0/swh/storage/tests/test_postgresql.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/tests/test_postgresql_converters.py` & `swh.storage-1.9.0/swh/storage/tests/test_postgresql_converters.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/tests/test_postgresql_flavor_mirror.py` & `swh.storage-1.9.0/swh/storage/tests/test_postgresql_flavor_mirror.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/tests/test_postgresql_flavor_readreplica.py` & `swh.storage-1.9.0/swh/storage/tests/test_postgresql_flavor_readreplica.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/tests/test_pytest_plugin.py` & `swh.storage-1.9.0/swh/storage/tests/test_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/tests/test_replay.py` & `swh.storage-1.9.0/swh/storage/tests/test_replay.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/tests/test_retry.py` & `swh.storage-1.9.0/swh/storage/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/tests/test_revision_bw_compat.py` & `swh.storage-1.9.0/swh/storage/tests/test_revision_bw_compat.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/tests/test_serializers.py` & `swh.storage-1.9.0/swh/storage/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/tests/test_server.py` & `swh.storage-1.9.0/swh/storage/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/tests/test_storage_data.py` & `swh.storage-1.9.0/swh/storage/tests/test_storage_data.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/tests/test_tenacious.py` & `swh.storage-1.9.0/swh/storage/tests/test_tenacious.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/tests/test_utils.py` & `swh.storage-1.9.0/swh/storage/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/tests/test_validate.py` & `swh.storage-1.9.0/swh/storage/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/utils.py` & `swh.storage-1.9.0/swh/storage/utils.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh/storage/writer.py` & `swh.storage-1.9.0/swh/storage/writer.py`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/swh.storage.egg-info/PKG-INFO` & `swh.storage-1.9.0/swh.storage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.storage
-Version: 1.8.0
+Version: 1.9.0
 Summary: Software Heritage storage manager
 Home-page: https://forge.softwareheritage.org/diffusion/DSTO/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-storage
```

### Comparing `swh.storage-1.8.0/swh.storage.egg-info/SOURCES.txt` & `swh.storage-1.9.0/swh.storage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swh.storage-1.8.0/tox.ini` & `swh.storage-1.9.0/tox.ini`

 * *Files 9% similar despite different names*

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
@@ -36,50 +38,47 @@
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
+  -e git+https://gitlab.softwareheritage.org/swh/devel/swh-docs.git\#egg=swh.docs
   pifpaf
-
 setenv =
   SWH_PACKAGE_DOC_TOX_BUILD = 1
   # turn warnings into errors
   SPHINXOPTS = -W
 commands =
   {envpython} -m pifpaf run postgresql -- make -I ../.tox/sphinx/src/swh-docs/swh/ -C docs
 
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
   pifpaf
-
 setenv =
   SWH_PACKAGE_DOC_TOX_BUILD = 1
   # turn warnings into errors
   SPHINXOPTS = -W
 commands =
   {envpython} -m pifpaf run postgresql -- make -I ../.tox/sphinx-dev/src/swh-docs/swh/ -C docs
```

