# Comparing `tmp/pyicat-plus-0.1.4.tar.gz` & `tmp/pyicat-plus-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyicat-plus-0.1.4.tar", last modified: Tue Jun  6 16:29:00 2023, max compression
+gzip compressed data, was "dist/pyicat-plus-0.1.5.tar", last modified: Tue Jun  6 17:09:40 2023, max compression
```

## Comparing `pyicat-plus-0.1.4.tar` & `pyicat-plus-0.1.5.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 16:29:00.000000 pyicat-plus-0.1.4/
--rw-rw-rw-   0 root         (0) root         (0)     7560 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     1648 2023-06-06 16:29:00.000000 pyicat-plus-0.1.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      953 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/README.md
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1387 2023-06-06 16:29:00.000000 pyicat-plus-0.1.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 16:29:00.000000 pyicat-plus-0.1.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 16:29:00.000000 pyicat-plus-0.1.4/src/pyicat_plus/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 16:29:00.000000 pyicat-plus-0.1.4/src/pyicat_plus/apps/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 16:28:54.000000 pyicat-plus-0.1.4/src/pyicat_plus/apps/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1057 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/apps/store_from_file.py
--rw-rw-rw-   0 root         (0) root         (0)      976 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/apps/store_processed.py
--rw-rw-rw-   0 root         (0) root         (0)     2605 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/apps/store_raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 16:29:00.000000 pyicat-plus-0.1.4/src/pyicat_plus/client/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 16:28:54.000000 pyicat-plus-0.1.4/src/pyicat_plus/client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1548 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/client/archive.py
--rw-rw-rw-   0 root         (0) root         (0)      349 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/client/defaults.py
--rw-rw-rw-   0 root         (0) root         (0)     7677 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/client/elogbook.py
--rw-rw-rw-   0 root         (0) root         (0)     3110 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/client/interface.py
--rw-rw-rw-   0 root         (0) root         (0)     6121 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/client/investigation.py
--rw-rw-rw-   0 root         (0) root         (0)    12840 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/client/main.py
--rw-rw-rw-   0 root         (0) root         (0)     3986 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/client/messaging.py
--rw-rw-rw-   0 root         (0) root         (0)     2515 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/client/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     1620 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/client/null.py
--rw-rw-rw-   0 root         (0) root         (0)     1531 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/client/serialize.py
--rw-rw-rw-   0 root         (0) root         (0)     2604 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/client/xmlns.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 16:29:00.000000 pyicat-plus-0.1.4/src/pyicat_plus/concurrency/
--rw-rw-rw-   0 root         (0) root         (0)     1499 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/concurrency/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 16:29:00.000000 pyicat-plus-0.1.4/src/pyicat_plus/concurrency/query_pool/
--rw-rw-rw-   0 root         (0) root         (0)      369 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/concurrency/query_pool/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3637 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/concurrency/query_pool/gevent.py
--rw-rw-rw-   0 root         (0) root         (0)     3565 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/concurrency/query_pool/threading.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 16:29:00.000000 pyicat-plus-0.1.4/src/pyicat_plus/metadata/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 16:28:54.000000 pyicat-plus-0.1.4/src/pyicat_plus/metadata/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10117 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/metadata/definitions.py
--rw-rw-rw-   0 root         (0) root         (0)   108391 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/metadata/hdf5_cfg.xml
--rw-rw-rw-   0 root         (0) root         (0)     1767 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/metadata/namespace_wrapper.py
--rw-rw-rw-   0 root         (0) root         (0)     2018 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/metadata/nexus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 16:29:00.000000 pyicat-plus-0.1.4/src/pyicat_plus/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 16:28:54.000000 pyicat-plus-0.1.4/src/pyicat_plus/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      176 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 16:29:00.000000 pyicat-plus-0.1.4/src/pyicat_plus/tests/fixtures/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 16:28:54.000000 pyicat-plus-0.1.4/src/pyicat_plus/tests/fixtures/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9106 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/tests/fixtures/icat.py
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/tests/fixtures/misc.py
--rw-rw-rw-   0 root         (0) root         (0)     1286 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/tests/fixtures/proc.py
--rw-rw-rw-   0 root         (0) root         (0)     2412 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/tests/fixtures/tcp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 16:29:00.000000 pyicat-plus-0.1.4/src/pyicat_plus/tests/servers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 16:28:54.000000 pyicat-plus-0.1.4/src/pyicat_plus/tests/servers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2866 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/tests/servers/activemq_rest_server.py
--rw-rw-rw-   0 root         (0) root         (0)     8429 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/tests/servers/icatplus_server.py
--rw-rw-rw-   0 root         (0) root         (0)     2378 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/tests/servers/stomp_publisher.py
--rw-rw-rw-   0 root         (0) root         (0)     3795 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/tests/servers/stomp_subscriber.py
--rw-rw-rw-   0 root         (0) root         (0)     1168 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/tests/servers/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2024 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/tests/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)     4316 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/tests/test_elogbook.py
--rw-rw-rw-   0 root         (0) root         (0)     1560 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/tests/test_icat_archive.py
--rw-rw-rw-   0 root         (0) root         (0)     3273 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/tests/test_icat_datasets.py
--rw-rw-rw-   0 root         (0) root         (0)      731 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/tests/test_icat_definitions.py
--rw-rw-rw-   0 root         (0) root         (0)      411 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/tests/test_icat_mockup.py
--rw-rw-rw-   0 root         (0) root         (0)     2804 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/tests/test_icat_nexus.py
--rw-rw-rw-   0 root         (0) root         (0)     1426 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/tests/test_icat_serialize.py
--rw-rw-rw-   0 root         (0) root         (0)      197 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/tests/test_maxsizedict.py
--rw-rw-rw-   0 root         (0) root         (0)     4610 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/tests/test_query_pool.py
--rw-rw-rw-   0 root         (0) root         (0)     1620 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/tests/test_url_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 16:29:00.000000 pyicat-plus-0.1.4/src/pyicat_plus/tests/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 16:28:54.000000 pyicat-plus-0.1.4/src/pyicat_plus/tests/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1492 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/tests/utils/compare.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 16:29:00.000000 pyicat-plus-0.1.4/src/pyicat_plus/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 16:28:54.000000 pyicat-plus-0.1.4/src/pyicat_plus/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      521 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/utils/maxsizedict.py
--rw-rw-rw-   0 root         (0) root         (0)      681 2023-06-06 16:26:46.000000 pyicat-plus-0.1.4/src/pyicat_plus/utils/url.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 16:29:00.000000 pyicat-plus-0.1.4/src/pyicat_plus.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1648 2023-06-06 16:29:00.000000 pyicat-plus-0.1.4/src/pyicat_plus.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2454 2023-06-06 16:29:00.000000 pyicat-plus-0.1.4/src/pyicat_plus.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 16:29:00.000000 pyicat-plus-0.1.4/src/pyicat_plus.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      189 2023-06-06 16:29:00.000000 pyicat-plus-0.1.4/src/pyicat_plus.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      307 2023-06-06 16:29:00.000000 pyicat-plus-0.1.4/src/pyicat_plus.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-06-06 16:29:00.000000 pyicat-plus-0.1.4/src/pyicat_plus.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:09:40.000000 pyicat-plus-0.1.5/
+-rw-rw-rw-   0 root         (0) root         (0)     7560 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     1648 2023-06-06 17:09:40.000000 pyicat-plus-0.1.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      953 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1387 2023-06-06 17:09:40.000000 pyicat-plus-0.1.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:09:40.000000 pyicat-plus-0.1.5/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:09:40.000000 pyicat-plus-0.1.5/src/pyicat_plus/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-06 17:07:25.000000 pyicat-plus-0.1.5/src/pyicat_plus/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:09:40.000000 pyicat-plus-0.1.5/src/pyicat_plus/apps/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 17:09:35.000000 pyicat-plus-0.1.5/src/pyicat_plus/apps/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1057 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/apps/store_from_file.py
+-rw-rw-rw-   0 root         (0) root         (0)      976 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/apps/store_processed.py
+-rw-rw-rw-   0 root         (0) root         (0)     2605 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/apps/store_raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:09:40.000000 pyicat-plus-0.1.5/src/pyicat_plus/client/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 17:09:35.000000 pyicat-plus-0.1.5/src/pyicat_plus/client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1548 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/client/archive.py
+-rw-rw-rw-   0 root         (0) root         (0)      349 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/client/defaults.py
+-rw-rw-rw-   0 root         (0) root         (0)     7677 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/client/elogbook.py
+-rw-rw-rw-   0 root         (0) root         (0)     3110 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/client/interface.py
+-rw-rw-rw-   0 root         (0) root         (0)     6121 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/client/investigation.py
+-rw-rw-rw-   0 root         (0) root         (0)    12919 2023-06-06 17:07:25.000000 pyicat-plus-0.1.5/src/pyicat_plus/client/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     3986 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/client/messaging.py
+-rw-rw-rw-   0 root         (0) root         (0)     2515 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/client/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     1620 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/client/null.py
+-rw-rw-rw-   0 root         (0) root         (0)     1531 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/client/serialize.py
+-rw-rw-rw-   0 root         (0) root         (0)     2604 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/client/xmlns.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:09:40.000000 pyicat-plus-0.1.5/src/pyicat_plus/concurrency/
+-rw-rw-rw-   0 root         (0) root         (0)     1499 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/concurrency/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:09:40.000000 pyicat-plus-0.1.5/src/pyicat_plus/concurrency/query_pool/
+-rw-rw-rw-   0 root         (0) root         (0)      369 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/concurrency/query_pool/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3637 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/concurrency/query_pool/gevent.py
+-rw-rw-rw-   0 root         (0) root         (0)     3565 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/concurrency/query_pool/threading.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:09:40.000000 pyicat-plus-0.1.5/src/pyicat_plus/metadata/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 17:09:35.000000 pyicat-plus-0.1.5/src/pyicat_plus/metadata/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10117 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/metadata/definitions.py
+-rw-rw-rw-   0 root         (0) root         (0)   108391 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/metadata/hdf5_cfg.xml
+-rw-rw-rw-   0 root         (0) root         (0)     1767 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/metadata/namespace_wrapper.py
+-rw-rw-rw-   0 root         (0) root         (0)     2018 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/metadata/nexus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:09:40.000000 pyicat-plus-0.1.5/src/pyicat_plus/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 17:09:35.000000 pyicat-plus-0.1.5/src/pyicat_plus/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      176 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:09:40.000000 pyicat-plus-0.1.5/src/pyicat_plus/tests/fixtures/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 17:09:35.000000 pyicat-plus-0.1.5/src/pyicat_plus/tests/fixtures/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9106 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/tests/fixtures/icat.py
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/tests/fixtures/misc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1286 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/tests/fixtures/proc.py
+-rw-rw-rw-   0 root         (0) root         (0)     2412 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/tests/fixtures/tcp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:09:40.000000 pyicat-plus-0.1.5/src/pyicat_plus/tests/servers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 17:09:35.000000 pyicat-plus-0.1.5/src/pyicat_plus/tests/servers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2866 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/tests/servers/activemq_rest_server.py
+-rw-rw-rw-   0 root         (0) root         (0)     8429 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/tests/servers/icatplus_server.py
+-rw-rw-rw-   0 root         (0) root         (0)     2378 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/tests/servers/stomp_publisher.py
+-rw-rw-rw-   0 root         (0) root         (0)     3795 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/tests/servers/stomp_subscriber.py
+-rw-rw-rw-   0 root         (0) root         (0)     1168 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/tests/servers/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2024 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/tests/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     4316 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/tests/test_elogbook.py
+-rw-rw-rw-   0 root         (0) root         (0)     1560 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/tests/test_icat_archive.py
+-rw-rw-rw-   0 root         (0) root         (0)     3273 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/tests/test_icat_datasets.py
+-rw-rw-rw-   0 root         (0) root         (0)      731 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/tests/test_icat_definitions.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/tests/test_icat_mockup.py
+-rw-rw-rw-   0 root         (0) root         (0)     2804 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/tests/test_icat_nexus.py
+-rw-rw-rw-   0 root         (0) root         (0)     1426 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/tests/test_icat_serialize.py
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/tests/test_maxsizedict.py
+-rw-rw-rw-   0 root         (0) root         (0)     4610 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/tests/test_query_pool.py
+-rw-rw-rw-   0 root         (0) root         (0)     1620 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/tests/test_url_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:09:40.000000 pyicat-plus-0.1.5/src/pyicat_plus/tests/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 17:09:35.000000 pyicat-plus-0.1.5/src/pyicat_plus/tests/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1492 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/tests/utils/compare.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:09:40.000000 pyicat-plus-0.1.5/src/pyicat_plus/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-06 17:09:35.000000 pyicat-plus-0.1.5/src/pyicat_plus/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      521 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/utils/maxsizedict.py
+-rw-rw-rw-   0 root         (0) root         (0)      681 2023-06-06 16:26:46.000000 pyicat-plus-0.1.5/src/pyicat_plus/utils/url.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 17:09:40.000000 pyicat-plus-0.1.5/src/pyicat_plus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1648 2023-06-06 17:09:40.000000 pyicat-plus-0.1.5/src/pyicat_plus.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2454 2023-06-06 17:09:40.000000 pyicat-plus-0.1.5/src/pyicat_plus.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 17:09:40.000000 pyicat-plus-0.1.5/src/pyicat_plus.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      189 2023-06-06 17:09:40.000000 pyicat-plus-0.1.5/src/pyicat_plus.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      307 2023-06-06 17:09:40.000000 pyicat-plus-0.1.5/src/pyicat_plus.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-06 17:09:40.000000 pyicat-plus-0.1.5/src/pyicat_plus.egg-info/top_level.txt
```

### Comparing `pyicat-plus-0.1.4/LICENSE.md` & `pyicat-plus-0.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.4/PKG-INFO` & `pyicat-plus-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyicat-plus
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python client to ICAT+
 Home-page: https://gitlab.esrf.fr/icat/pyicat-plus/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/icat/pyicat-plus/
 Project-URL: Documentation, https://pyicat-plus.readthedocs.io/
```

### Comparing `pyicat-plus-0.1.4/README.md` & `pyicat-plus-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.4/setup.cfg` & `pyicat-plus-0.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.4/src/pyicat_plus/apps/store_from_file.py` & `pyicat-plus-0.1.5/src/pyicat_plus/apps/store_from_file.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.4/src/pyicat_plus/apps/store_processed.py` & `pyicat-plus-0.1.5/src/pyicat_plus/apps/store_processed.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.4/src/pyicat_plus/apps/store_raw.py` & `pyicat-plus-0.1.5/src/pyicat_plus/apps/store_raw.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.4/src/pyicat_plus/client/archive.py` & `pyicat-plus-0.1.5/src/pyicat_plus/client/archive.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.4/src/pyicat_plus/client/elogbook.py` & `pyicat-plus-0.1.5/src/pyicat_plus/client/elogbook.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.4/src/pyicat_plus/client/interface.py` & `pyicat-plus-0.1.5/src/pyicat_plus/client/interface.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.4/src/pyicat_plus/client/investigation.py` & `pyicat-plus-0.1.5/src/pyicat_plus/client/investigation.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.4/src/pyicat_plus/client/main.py` & `pyicat-plus-0.1.5/src/pyicat_plus/client/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,19 +52,21 @@
             )
         else:
             self._archive_client = None
         if elogbook_url and elogbook_token:
             self._investigation_client = IcatInvestigationClient(
                 url=elogbook_url, api_key=elogbook_token, timeout=feedback_timeout
             )
+            if elogbook_metadata is None:
+                elogbook_metadata = dict()
             self._elogbook_client = IcatElogbookClient(
                 url=elogbook_url,
                 api_key=elogbook_token,
                 timeout=elogbook_timeout,
-                payload=elogbook_metadata,
+                **elogbook_metadata,
             )
         else:
             self._investigation_client = None
             self._elogbook_client = None
 
     @property
     def metadata_client(self):
```

### Comparing `pyicat-plus-0.1.4/src/pyicat_plus/client/messaging.py` & `pyicat-plus-0.1.5/src/pyicat_plus/client/messaging.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.4/src/pyicat_plus/client/metadata.py` & `pyicat-plus-0.1.5/src/pyicat_plus/client/metadata.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.4/src/pyicat_plus/client/null.py` & `pyicat-plus-0.1.5/src/pyicat_plus/client/null.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.4/src/pyicat_plus/client/serialize.py` & `pyicat-plus-0.1.5/src/pyicat_plus/client/serialize.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.4/src/pyicat_plus/client/xmlns.py` & `pyicat-plus-0.1.5/src/pyicat_plus/client/xmlns.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.4/src/pyicat_plus/concurrency/__init__.py` & `pyicat-plus-0.1.5/src/pyicat_plus/concurrency/__init__.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.4/src/pyicat_plus/concurrency/query_pool/gevent.py` & `pyicat-plus-0.1.5/src/pyicat_plus/concurrency/query_pool/gevent.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.4/src/pyicat_plus/concurrency/query_pool/threading.py` & `pyicat-plus-0.1.5/src/pyicat_plus/concurrency/query_pool/threading.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.4/src/pyicat_plus/metadata/definitions.py` & `pyicat-plus-0.1.5/src/pyicat_plus/metadata/definitions.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.4/src/pyicat_plus/metadata/hdf5_cfg.xml` & `pyicat-plus-0.1.5/src/pyicat_plus/metadata/hdf5_cfg.xml`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.4/src/pyicat_plus/metadata/namespace_wrapper.py` & `pyicat-plus-0.1.5/src/pyicat_plus/metadata/namespace_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.4/src/pyicat_plus/metadata/nexus.py` & `pyicat-plus-0.1.5/src/pyicat_plus/metadata/nexus.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.4/src/pyicat_plus/tests/fixtures/icat.py` & `pyicat-plus-0.1.5/src/pyicat_plus/tests/fixtures/icat.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.4/src/pyicat_plus/tests/fixtures/proc.py` & `pyicat-plus-0.1.5/src/pyicat_plus/tests/fixtures/proc.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.4/src/pyicat_plus/tests/fixtures/tcp.py` & `pyicat-plus-0.1.5/src/pyicat_plus/tests/fixtures/tcp.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.4/src/pyicat_plus/tests/servers/activemq_rest_server.py` & `pyicat-plus-0.1.5/src/pyicat_plus/tests/servers/activemq_rest_server.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.4/src/pyicat_plus/tests/servers/icatplus_server.py` & `pyicat-plus-0.1.5/src/pyicat_plus/tests/servers/icatplus_server.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.4/src/pyicat_plus/tests/servers/stomp_publisher.py` & `pyicat-plus-0.1.5/src/pyicat_plus/tests/servers/stomp_publisher.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.4/src/pyicat_plus/tests/servers/stomp_subscriber.py` & `pyicat-plus-0.1.5/src/pyicat_plus/tests/servers/stomp_subscriber.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.4/src/pyicat_plus/tests/servers/utils.py` & `pyicat-plus-0.1.5/src/pyicat_plus/tests/servers/utils.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.4/src/pyicat_plus/tests/test_cli.py` & `pyicat-plus-0.1.5/src/pyicat_plus/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.4/src/pyicat_plus/tests/test_elogbook.py` & `pyicat-plus-0.1.5/src/pyicat_plus/tests/test_elogbook.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.4/src/pyicat_plus/tests/test_icat_archive.py` & `pyicat-plus-0.1.5/src/pyicat_plus/tests/test_icat_archive.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.4/src/pyicat_plus/tests/test_icat_datasets.py` & `pyicat-plus-0.1.5/src/pyicat_plus/tests/test_icat_datasets.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.4/src/pyicat_plus/tests/test_icat_definitions.py` & `pyicat-plus-0.1.5/src/pyicat_plus/tests/test_icat_definitions.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.4/src/pyicat_plus/tests/test_icat_nexus.py` & `pyicat-plus-0.1.5/src/pyicat_plus/tests/test_icat_nexus.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.4/src/pyicat_plus/tests/test_icat_serialize.py` & `pyicat-plus-0.1.5/src/pyicat_plus/tests/test_icat_serialize.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.4/src/pyicat_plus/tests/test_query_pool.py` & `pyicat-plus-0.1.5/src/pyicat_plus/tests/test_query_pool.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.4/src/pyicat_plus/tests/test_url_utils.py` & `pyicat-plus-0.1.5/src/pyicat_plus/tests/test_url_utils.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.4/src/pyicat_plus/tests/utils/compare.py` & `pyicat-plus-0.1.5/src/pyicat_plus/tests/utils/compare.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.4/src/pyicat_plus/utils/maxsizedict.py` & `pyicat-plus-0.1.5/src/pyicat_plus/utils/maxsizedict.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.4/src/pyicat_plus/utils/url.py` & `pyicat-plus-0.1.5/src/pyicat_plus/utils/url.py`

 * *Files identical despite different names*

### Comparing `pyicat-plus-0.1.4/src/pyicat_plus.egg-info/PKG-INFO` & `pyicat-plus-0.1.5/src/pyicat_plus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyicat-plus
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python client to ICAT+
 Home-page: https://gitlab.esrf.fr/icat/pyicat-plus/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/icat/pyicat-plus/
 Project-URL: Documentation, https://pyicat-plus.readthedocs.io/
```

### Comparing `pyicat-plus-0.1.4/src/pyicat_plus.egg-info/SOURCES.txt` & `pyicat-plus-0.1.5/src/pyicat_plus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

